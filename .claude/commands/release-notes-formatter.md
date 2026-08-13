---
name: release-notes-formatter
description: 格式化及驗證Workfront發行說明，以取得一致性、正確結構和正確連結。 僅用於產品版本目錄中的版本注意事項檔案，或者當使用者提及版本注意事項、產品版本或季度版本時。 請勿套用至作法文章或一般檔案。
source-git-commit: dac869369d6d9ef32741aa0972ccf9cb25b2633c
workflow-type: tm+mt
source-wordcount: '2183'
ht-degree: 2%

---


# 發行說明格式化程式

格式化和驗證`help/quicksilver/product-announcements/product-releases/`目錄中的Adobe Workfront發行說明。

## 頁面型別

識別檔案路徑和內容的頁面型別：

| 頁面類型 | 檔案模式 | 範本 |
|-----------|-------------|----------|
| **概觀** | `{YY}-q{N}-release-overview.md` | 請參閱。#overview-page-template |
| **產品區域** | `{YY}-q{N}-{area}.md` | 請參閱。#product-area-page-template |
| **規劃** | `planning-release-activity-{YY}-q{N}.md` | 與產品區域相似 |
| **外觀** | `look-and-feel-updates-{YY}-q{N}.md` | 請參閱。#look-and-feel-page-template |

## 步驟0：決定季度（請先執行此動作，然後再執行其他動作）

>[!IMPORTANT]
>
>切勿在「預覽」或「生產」日期使用行事曆季度數學將功能指派給doc-quarter。 Doc-quarter是根據Workfront的內部發行 — 行事曆群組（與行事曆季度位移），功能會以&#x200B;**每月發行**&#x200B;為基礎 — 請參閱此檔案結尾附近的[2026年發行行事曆](#2026-release-calendar)表格。 例如，生產日期為2026年8月13日的功能屬於doc-quarter `26-q4`，而非`26-q3`，因為8月每月發行對應至`26-q4`。
>
>進一步向下的「季度對應」表格（書面形式/月份）用於寫出標題中的季度名稱（例如，Q3的「第三季」） — 它自己&#x200B;**不足**&#x200B;來決定功能屬於哪個季度的檔案。 在建立或編輯任何檔案之前，請務必交叉核對「發行行事曆」表格。
>
>如果功能的生產日期未出現在發行行事曆表格中（例如，超出表格的日期範圍），請要求使用者提供更新的行事曆，而非猜測。

## 格式化工作流程

### 步驟1：驗證Frontmatter

所有發行說明頁面的必填欄位：

```yaml
---
title: <descriptive title>
description: <matches or summarizes the title>
author: <author name>
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: <existing UUID — never generate or change>
---
```

規則：
- `feature`必須剛好`Product Announcements`
- `recommendations`必須剛好`noDisplay, noCatalog`
- 絕不建立`exl-id` — 僅包含已存在的專案
- 請勿將`draft: Probably`新增至實際頁面（僅限範本）

### 步驟2：依頁面型別驗證結構

#### 產品區域頁面

1. **H1**： `{Written Quarter} {Area} enhancements`
   - 範例：`# Second Quarter 2026 Administrator enhancements`
   - 季必須寫成：「第一季」、「第二季」、「第三季」、「第四季」

2. **簡介段落**：說明概觀的區域和連結
   - 必須連結至&#x200B;**正確季的**&#x200B;概觀檔案
   - 常見錯誤：連結至上一季（例如`26-q1`而非`26-q2`）

3. **H2每個功能**：功能標題做為標題
   - **最新功能在前** — 最新的發行說明必須顯示為介紹段落之後的第一個H2
   - 較舊的功能會以反向時間順序遵循

4. 每個H2之後的&#x200B;**日期圖說文字區塊**：

```markdown
>[!NOTE]
>
>Preview: {Month Day, Year}
>Production fast release: {Month Day, Year}
>Production for everyone: {Month Day, Year}
```

5. **內文**：功能說明，然後連結到說明檔案

#### 總覽頁面

1. **H1**： `{Written Quarter} release overview`

2. **將段落**&#x200B;與排定的發行月份一起介紹

3. 使用發行排程表的&#x200B;**`>[!IMPORTANT]`區塊**

4. **H2`Adobe Workfront enhancements`**&#x200B;包含錨點連結的專案符號清單：

```markdown
* [Administrator enhancements](#administrator-enhancements)
* [Document enhancements](#document-enhancements)
```

5. 每個產品區域有&#x200B;**H3**&#x200B;搭配HTML功能表（請參閱。claude/commands/_release-notes-formatter-reference.md#overview-feature-table）
   - 在每個表格中，**最新功能排在前** — 最近的列會顯示在表格頂端（標題列之後）

6. **尾端區段** (H2)：其他區域的發行說明、案頭校訂檢視器更新、公告、API版本、維護更新、訓練更新

### 步驟3：驗證連結

- **產品區域頁面中的總覽連結**：必須指向同一季
  - 正確： `26-q2-release-activity/26-q2-release-overview.md`
  - 錯誤： `26-q1-release-activity/26-q1-release-overview.md`
- 總覽中的&#x200B;**錨點連結**：必須符合H3 ID （小寫、連字型大小）
- 總覽資料表中的&#x200B;**功能連結**：必須使用`class="MCXref xref" xrefformat="{para}"`
- **說明檔案連結**：必須以`/help/quicksilver/`開頭

### 步驟4：驗證日期

- 格式： `{Month} {Day}, {Year}` （例如「2026年3月12日」）
- 將`TBD`用於未知日期
- 產品區域頁面`>[!NOTE]`區塊中的日期必須符合對應的概觀表格列
- 預覽日期應早於生產日期

### 步驟5：常見修正

格式化時套用這些修正：

| 問題 | 修正 |
|-------|-----|
| 錯誤的概觀連結季度 | 更新以符合檔案自己的季度 |
| 缺少`>[!NOTE]`日期區塊 | H2功能標題後新增區塊 |
| 日期格式不一致 | 標準化為`Month Day, Year` |
| `>[!NOTE]`前遺漏空白行 | 新增空白行 |
| 編號說明行中的額外空格 | 修剪尾隨空格 |
| 產品區域頁面中的HTML | 維持為Markdown （HTML僅適用於概觀表格） |
| 遺失`exl-id` | 將其忽略 — 不要產生一個 |

### 步驟6：同步概觀頁面

每當您將&#x200B;**新功能**&#x200B;新增至產品區域頁面時，請以相同變更在該季的`{YY}-q{N}-release-overview.md`中新增或更新相符的列。 僅存在於產品區域頁面上而不存在於總覽表格中的功能，將從發行版本總覽索引中隱藏。

- 尋找該產品區域的H3區段（例如，`### Reporting enhancements`），並在表格的&#x200B;**頂端**&#x200B;新增新的`<tr>`列（在標題列之後），符合現有的列格式（請參閱。#overview-feature-table）。
- 此列中的日期必須符合該功能的產品區域頁面上的`>[!NOTE]`區塊（步驟4）。
- 如果將功能重新分類至不同的產品區域（例如，從報表移至管理員），請將其列移至新區域的H3區段 — 不要在舊區域中留下舊的副本。
- 僅限Planning的功能不會新增至概觀表格 — Planning有自己的發行活動頁面，在「其他區域的發行說明」底下連結一次（不需要每個功能列）。

當功能已經有列，而且其內容/日期未變更時，請勿觸碰概觀頁面。

要避免的常見錯誤：

- 將功能的H2新增至產品區域頁面，而不將相符的列新增至概觀表格。
- 將內容移至不同區域的頁面後，在舊產品區域區段中保留過時的概觀列。
- 不符合產品區域頁面`>[!NOTE]`區塊的概述列日期。

### 步驟7：更新目錄

每當您建立&#x200B;**新**&#x200B;發行說明頁面（總覽或產品區域）時，請將其新增至`help/quicksilver/TOC.md`，並進行相同變更。 不在目錄中的頁面不會出現在發佈的導覽中，即使概觀表格中的連結指向該頁面。

要新增的位置：

- 目錄(TOC)在標題下有每季的區段，例如`* 2026 Q3 Release {#release-26-q3}`。 如果季度標題尚不存在（新季度的第一頁），請將其新增到上一季度的上方，這樣最新季度就會位於最上方。
- 在該季度標題下，以下列順序列出頁面：
  1. **概觀**&#x200B;優先(`Third Quarter 2026 release overview`)。
  2. **產品區域頁面**&#x200B;依區域名稱的字母順序（管理員、檔案、企業作業、專案、報告、請求）。
  3. **其他增強功能**&#x200B;最後會出現（一律在按字母順序排列的產品區域之後）。

每個TOC專案都是一個Markdown連結，使用頁面標題和絕對存放庫路徑：

```markdown
      * [Third Quarter 2026 Documents enhancements](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-documents.md)
```

將縮排（六個空格）與周圍的專案配對。 使用頁面H1逐字做為連結文字 — 例如`Documents enhancements`、`Requesting enhancements` （不是`Requests`） — 因此TOC標籤會比對先前的季度。

要避免的常見錯誤：

- 建立產品區域頁面，而不將其新增至目錄。
- 從新產品區域頁面連結至其他季度的概述（步驟3）。
- 在上一個季度的標題下插入新季度的頁面。

### 步驟8：更新首頁

每當您建立&#x200B;**新季度的總覽頁面** （亦即，這是新季度的第一頁，而不僅僅是新增到現有季度的新產品區域頁面）時，請以相同變更更新`help/quicksilver/home.md`：

- 在`>[!TAB Latest release]`區段中，將發行版本總覽連結取代為新季度的總覽連結。
- 也在該區段中，更新Adobe Workfront Planning發行活動連結以指向新季度的計畫檔案(`planning-release-activity-{YY}-q{N}.md`) （如果有的話）。
- 在目前年度的`>[!TAB {YYYY} releases]`標籤中，將新季度的概述連結新增至清單頂端、前一個季度的專案上方。

僅將產品區域頁面新增至已列出概觀頁面的季度時，請勿觸及`home.md`。

要避免的常見錯誤：

- 建立新季度的總覽頁面，而不更新`home.md`的「最新版本」索引標籤（它將持續指向舊季度）。
- 忘記還要將新季度新增到當年索引標籤清單中。

&lt;&lt;&lt;&lt;&lt;&lt;&lt;已更新上游
### 步驟8：更新產品發行索引頁面
=======
### 步驟9：更新產品發行索引頁面
>>>>>>>>>>隱藏的變更
> 
每當您建立&#x200B;**新季度的總覽頁面**&#x200B;時，也需在同一變更中更新`help/quicksilver/product-announcements/product-releases/product-releases.md`：

- 在「Workfront發行版本」欄中尋找目前年份的`<p>Releases in {year}</p>`區塊。
- 在該年度清單的&#x200B;**前**&#x200B;新增新的`<li>`，連結到新季度的總覽頁面，格式與現有專案相同：

  ```html
  <li><a href="/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md" class="MCXref xref" xrefformat="{para}">Fourth Quarter 2026 release overview</a></li>
  ```

- 如果新季度的Planning發行活動頁面存在(`planning-release-activity-{YY}-q{N}.md`)，請在相同列的「其他產品發行」欄頂端新增相符的`<li>`。
- 如果目前年份還沒有列（新年份的第一季），請依照現有的列結構，在前一年列上方新增新的`<tr data-mc-conditions="">`。

僅將產品區域頁面新增至已列出概觀頁面的季度時，請勿觸及`product-releases.md`。

要避免的常見錯誤：

- 建立新季度的總覽頁面而不將其新增到`product-releases.md` （該頁面將只繼續顯示以前的季度）。
- 新增總覽連結，但忘記對應的Planning發行活動連結。

## 檔案命名慣例

| 類型 | 模式 | 範例 |
|------|---------|---------|
| 概觀 | `{YY}-q{N}-release-overview.md` | `26-q2-release-overview.md` |
| 產品區域 | `{YY}-q{N}-{area-slug}.md` | `26-q2-admin-and-setup.md` |
| 目錄 | `{YY}-q{N}-release-activity/` | `26-q2-release-activity/` |

標準區域概要： `admin-and-setup`、`documents`、`projects`、`reports`、`requests`、`other`

## 季度對應

>[!NOTE]
>
>此表用於寫出季度名稱（例如，在H1或標題中）。 它無法判斷某個功能所屬的季度檔案 — 請使用下方的[2026年發行行事曆](#2026-release-calendar)表格來判斷該功能，因為doc-quarter與calendar-quarter是位移。

| 季度 | 書面形式 | 月 |
|---------|-------------|--------|
| Q1 | 第一季 | 3月1日 |
| Q2 | 第二季 | 4月6日 |
| Q3 | 第三季 | 2020年7月 |
| Q4 | 第四季 | 10月至12月 |

**重要 — 用於檔案名稱（`26-q3`、`26-q4`等）的doc季度 從這個行事曆對應位移一個月。** 它遵循Workfront的內部發行行事曆分組，其中每個檔案季度=前兩個每月發行+季度發行月份。 例如，檔案季度`26-q3`涵蓋2026年5月/6月/7月月月發行（季度發行`2026.07`），而檔案季度`26-q4`涵蓋2026年8月/9月/10月月月月月月月發行（季度發行`2026.10`）。 請務必檢視下方的發行行事曆（或要求更新行事曆），然後再根據上方的行事曆季度表假設檔案的季度。

## 2026年發行行事曆

Source： 「2026年每月發行行事曆」（Adobe corp wiki、AWF空間 — `wiki.corp.adobe.com`、空間索引鍵AWF、標題「2026年每月發行行事曆」）。 WebFetch無法存取此頁面（需要Adobe SSO）；當需要的日期超過這裡擷取的日期時，請要求使用者貼上更新的PDF/表格。

| 發行月份 | 最終預覽 | 生產 | 每月發行 | 每季發行 | 檔案季度 |
|---|---|---|---|---|---|
| 2025年11 | 2025年10月30日 | 2025年11月13日 | 2025.11 | 2026.01 | 26-q1 |
| 2025年12 | 2025年11月27日 | 2025年12月11日 | 2025.12 | 2026.01 | 26-q1 |
| 2026年1月 | 2025年12月23日 | 2026年1月15日 | 2026.01 | 2026.01 | 26-q1 |
| 2026年2月 | 2026年1月29日 | 2026年2月12日 | 2026.02 | 2026.04 | 26-q2 |
| 2026年3月 | 2026年2月26日 | 2026年3月12日 | 2026.03 | 2026.04 | 26-q2 |
| 2026年4月 | 2026年4月2日 | 2026年4月16日 | 2026.04 | 2026.04 | 26-q2 |
| 2026年5月 | 2026年4月30日 | 2026年5月14日 | 2026.05 | 2026.07 | 26-q3 |
| 2026年6月 | 2026年5月28日 | 2026年6月11日 | 2026.06 | 2026.07 | 26-q3 |
| 2026年7月 | 2026年7月7日 | 2026年7月16日 | 2026.07 | 2026.07 | 26-q3 |
| 2026年8月 | 2026年7月30日 | 2026年8月13日 | 2026.08 | 2026.10 | 26-q4 |
| 2026年9月 | 2026年9月3日 | 2026年9月17日 | 2026.09 | 2026.10 | 26-q4 |
| 2026年10 | 2026年10月01日 | 2026年10月15日 | 2026.10 | 2026.10 | 26-q4 |
| 2026年11 | 2026年10月29日 | 2026年11月12日 | 2026.11 | 2027.01 | 27-q1 |
| 2026年12 | 2026年11月26日 | 2026年12月10日 | 2026.12 | 2027.01 | 27-q1 |
| 2027年1月 | 2027年1月5日 | 2027年1月14日 | 2027.01 | 2027.01 | 27-q1 |

使用此表格的注意事項：

- **最終預覽**&#x200B;是該月版本預覽中功能可能顯示的最後日期 — 將它用於概覽頁面的「功能可能出現在預覽環境中的最後日期」專案符號（僅限季末月份）。
- **Production**&#x200B;是該月發行版本的正式人人皆可使用的生產日期。
- 對於季末月份（符合「每季發行」資料欄的月份），概觀頁面的排程表格會列出該月的發行&#x200B;**兩次**：一次在「每月發行」資料欄中，日期為&#x200B;**生產日期（快速發行日期）前一天**，另一次在「每季發行」資料欄中，日期為實際生產日期。 一個季度的非最終月份在每月清單和任何「快速發行」參考中都使用相同的生產日期 — 不需要調整。
- 此表格僅填滿2027年1月。 需要較晚的日期時，請要求使用者提供更新的行事曆，而非猜測。

每季的製作版本通常會在當季最後一個月的第二個整週的星期四推出。

## 驗證檢查清單

檢閱發行說明檔案時，請確認：

- [ ] Frontmatter的所有必要欄位都具有正確的值
- [ ] H1符合頁面型別格式
- [ ]概觀連結指向正確的季度
- [ ]每個功能都有`>[!NOTE]`個日期區塊（產品區域頁面）
- [ ]日期格式一致(`Month Day, Year`)
- [ 概覽中的]功能表格列符合產品區域頁面內容
- [ ]沒有中斷的內部連結
- [ 總覽中的]個錨點連結符合H3區段ID
- [ ]功能是以最新優先順序排列（產品區域頁面和概觀表格）
- [ ]新發行說明頁面列在正確季度下的`help/quicksilver/TOC.md`中，概覽在前，產品區域按字母順序（其他在後）
- [ ]如果建立了新季度的總覽頁面，`help/quicksilver/home.md` 「最新版本」索引標籤和當年的索引標籤指向它
- [ ]如果建立了新季度的總覽頁面，`help/quicksilver/product-announcements/product-releases/product-releases.md`會將其列在當前年度的「Workfront發行版本」清單頂端（如果存在的話，另加規劃連結）

## 其他資源

- 如需完整的HTML範本和範例，請參閱。claude/commands/_release-notes-formatter-reference.md
