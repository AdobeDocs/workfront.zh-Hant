---
name: clean-el-traffic-csv
description: 清除原始Experience League / Adobe Analytics流量CSV匯出至僅限Workfront的頁面，依頁面檢視排序。 當使用者提供Experience League頁面流量CSV （「頁面URL一般」、「不重複訪客」、「造訪」、「頁面檢視」等欄）並要求清除、篩選或處理它，或提及「檔案追蹤」/「檢視次數最多的文章」試算表時使用。
source-git-commit: e22d43e9962b2b00793577fd14ac00587e8a2a6d
workflow-type: tm+mt
source-wordcount: '876'
ht-degree: 0%

---


# 清除Experience League流量CSV

將Experience League頁面流量的原始Adobe Analytics自由格式表格匯出變更為依頁面檢視排序的純Workfront、重複資料刪除的CSV，覆寫原始檔案並將過期的復本儲存到案頭。

## 輸入形狀

輸入可以是兩種形狀之一：

1. **原始匯出** — 以中繼資料註解行（`#===`、`# Freeform`、`# Report suite: ...`、`"# Date: <range>"`等）開頭，後面接著階層劃分表格（例如`Solution (v2)` → `workfront` → `Page URL Generic (v33)`→個別URL列）。 常值儲存格`Page URL Generic (v33)` （或類似的`Page URL Generic ...`標籤）會出現在第二欄中。
2. **已經清除的CSV** — 第一列已經是像`Page URL Generic (v33),Unique Visitors,Visits,Page Views`一樣的純標題，沒有中繼資料列或額外的行距。

在開始之前偵測您具有的形狀：如果列1是符合形狀2的純標題列，請直接跳至步驟2 （無法使用日期範圍，因此也請跳過步驟7，除非使用者另外提供日期範圍）。

## 工作流程

### 步驟0：擷取日期範圍（僅原始匯出，刪除任何專案前）

尋找最上方符合`# Date: <range>`的中繼資料行（例如`"# Date: Jul 1, 2026 - Jul 31, 2026"`）。 記錄`<range>` （例如`Jul 1, 2026 - Jul 31, 2026`） — 稍後在步驟7中需要它。 刪除任何列前請先執行此動作。

### 步驟1：將原始資料匯出簡化為純資料表（僅限原始資料匯出）

1. 尋找包含儲存格`Page URL Generic (...)`的列（位於標準匯出的第二欄）。
2. 刪除該列上方的每一列，包括中繼資料註解行和`Solution (v2)` / `workfront`小計列。
3. 刪除`Page URL Generic`儲存格左側的每一欄（在標準匯出中，這只是欄A）。
4. 在同一列（現在為標題列），將`Page URL Generic (...)`右側的數值小計值取代為常值標題，順序為： `Unique Visitors`、`Visits`、`Page Views`。 保留`Page URL Generic (...)`儲存格本身不變。

結果：標頭為`Page URL Generic (v33),Unique Visitors,Visits,Page Views`的純CSV，每個URL後面接著一列。

### 步驟2：僅保留Workfront列

針對每個資料列，檢查URL是否包含常值子字串`/workfront/` （兩側的斜線）。 地區設定首碼並不重要（`/en/`、`/zh-hans/`等 — 只要產品區段相符，都保持不變）。

- 如果URL **不**&#x200B;包含`/workfront/`作為路徑區段，請刪除該列 — 這會移除其他產品，例如`workfront-fusion`、`workfront-learn`、`proofhqpapi`等。（像`tutorials-workfront`這樣的子字串不會&#x200B;**不會**&#x200B;計數 — 相符專案必須是完全相同的區段`/workfront/`）。
- 否則，請保留該列。

### 步驟3：修剪URL

對於每個存活的資料列，在URL中尋找`/using`，並僅保留其後`/`的後續部分（及包含），捨棄之前的所有內容，並包含`/using`。

範例： `https://experienceleague.adobe.com/en/docs/workfront/using/home` → `/home`

如果在Workfront列的URL中找不到`/using`，請保持該URL不變，並為使用者加上旗標，而非猜測。

### 步驟4：移除片段/查詢尾碼

如果修剪過的URL包含`#`或`?`，請刪除該字元及其後面的所有內容。

範例： `/manage-scenarios/restore-a-scenario-version#compare-scenario-versions` → `/manage-scenarios/restore-a-scenario-version`

### 步驟5：合併重複專案

修剪後，多列現在可以共用相同的URL （例如，兩個不同的地區設定列摺疊到相同的路徑）。 將所有具有相同URL的資料列合併為一列，分別加總`Unique Visitors`、`Visits`和`Page Views`。

範例： `/home,2,2,3`和`/home,5,6,7` → `/home,7,8,10`

### 步驟6：依頁面檢視排序

依`Page Views`遞減排序所有資料列（最大為前）。 標頭列固定在頂端已排序資料的上方。

### 步驟7：新增日期範圍列（只有在步驟0中擷取時，才會原始匯出）

插入之前，請移除擷取日期範圍以外的任何逗號（例如`Jul 1, 2026 - Jul 31, 2026` → `Jul 1 2026 - Jul 31 2026`） — 原始範圍具有逗號，否則會誤讀為該列的CSV欄分隔符號。

在標題列的最上方插入新的一列，僅包含以逗號去除的日期範圍。

最終列順序：日期範圍列→標題列→已排序的資料列。

### 步驟8：儲存

以清除的結果覆寫原處的原始輸入檔案。

### 步驟9：將日期副本儲存至案頭（僅當在步驟0中擷取了日期範圍時，才使用原始匯出）

建立日期範圍的檔案名稱安全版本：移除逗號，並將任何`\ / : * ? " < > |`取代為`-` （這些字元在Windows檔案名稱中無效，否則可能會根據匯出地區設定/格式出現在日期範圍內）。

將已清理的CSV的額外復本（與步驟8的內容相同）儲存到目前使用者的案頭，並命名為：

`Documentation tracking report <filename-safe date range>.csv`

範例：擷取的`Apr 1, 2026 - Apr 30, 2026`範圍變成`Documentation tracking report Apr 1 2026 - Apr 30 2026.csv`。

針對已清除的CSV （形狀2）跳過此步驟，除非使用者另外提供日期範圍。

## 超出範圍

張貼或共用清理過的CSV （例如放到Slack）是另一個尚未定義的步驟 — 請勿在此技能範圍內嘗試在任何地方附加或上傳檔案。

## 實作（原始匯出）

對於原始匯出，請使用此經過測試的PowerShell指令碼執行步驟0到8，而不是手動編輯列 — 對於有數百列的檔案而言，這樣會更快且不易出錯。 將真實檔案路徑取代為`$path`。

執行之前，檢查檔案是否已鎖定（例如在Excel中開啟） — 如果`Set-Content`因「被其他處理序使用」而失敗，請要求使用者關閉檔案，然後重新執行。

```powershell
$path = "<full path to the CSV>"
$lines = Get-Content -Path $path -Encoding UTF8

# Step 0: capture the date range
$dateLine = $lines | Where-Object { $_ -match '# Date:\s*(.+?)"?\s*$' } | Select-Object -First 1
$null = $dateLine -match '# Date:\s*(.+?)"?\s*$'
$dateRange = $matches[1].Trim('"').Trim()

# Step 1: find the "Page URL Generic" row and strip everything above/left of it
$headerIdx = -1
for ($i = 0; $i -lt $lines.Count; $i++) {
    if ($lines[$i] -match 'Page URL Generic') { $headerIdx = $i; break }
}
$headerParts = $lines[$headerIdx].Split(',')
$urlHeaderLabel = $headerParts[1]
$newHeader = "$urlHeaderLabel,Unique Visitors,Visits,Page Views"

$dataLines = $lines[($headerIdx + 1)..($lines.Count - 1)] | Where-Object { $_.Trim() -ne '' }

$rows = @()
foreach ($line in $dataLines) {
    $comma1 = $line.IndexOf(',')
    $rest = $line.Substring($comma1 + 1)   # drop column(s) left of the URL
    $parts = $rest.Split(',')
    if ($parts.Count -ne 4) { continue }
    $url = $parts[0]
    $uv = [int]$parts[1]
    $vi = [int]$parts[2]
    $pv = [int]$parts[3]

    # Step 2: keep only /workfront/ rows
    if ($url -notmatch '/workfront/') { continue }

    # Step 3: trim to from "/using" onward
    $usingIdx = $url.IndexOf('/using')
    if ($usingIdx -lt 0) { continue }   # flag/report these separately if any occur
    $trimmed = $url.Substring($usingIdx + 6)   # 6 = length of "/using"

    # Step 4: strip # or ? suffix
    $hashIdx = $trimmed.IndexOfAny(@('#', '?'))
    if ($hashIdx -ge 0) { $trimmed = $trimmed.Substring(0, $hashIdx) }

    $rows += [PSCustomObject]@{ URL = $trimmed; UV = $uv; Visits = $vi; PV = $pv }
}

# Step 5: merge duplicates
$grouped = $rows | Group-Object URL | ForEach-Object {
    [PSCustomObject]@{
        URL    = $_.Name
        UV     = ($_.Group | Measure-Object UV -Sum).Sum
        Visits = ($_.Group | Measure-Object Visits -Sum).Sum
        PV     = ($_.Group | Measure-Object PV -Sum).Sum
    }
}

# Step 6: sort by Page Views descending
$sorted = $grouped | Sort-Object -Property PV -Descending

# Step 7 + 8: prepend date range (commas stripped) + header, then save
$dateRangeNoCommas = $dateRange -replace ',', ''
$outLines = @()
$outLines += $dateRangeNoCommas
$outLines += $newHeader
$outLines += $sorted | ForEach-Object { "$($_.URL),$($_.UV),$($_.Visits),$($_.PV)" }

Set-Content -Path $path -Value $outLines -Encoding UTF8

# Step 9: also save a dated copy to the Desktop
$safeDateRange = ($dateRange -replace ',', '') -replace '[\\/:*?"<>|]', '-'
$desktopPath = Join-Path ([Environment]::GetFolderPath('Desktop')) "Documentation tracking report $safeDateRange.csv"
Set-Content -Path $desktopPath -Value $outLines -Encoding UTF8
```

對於已經清除的CSV （輸入圖形2），請略過標題重新定位、日期範圍邏輯和步驟9 — 直接在現有標題/列上執行步驟2-6和8。
