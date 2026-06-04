---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: 建立與Workfront資料連線的連線
description: Workfront Data Connect可讓您將組織的Workfront資料與商業智慧工具搭配使用，或將其儲存在外部資料倉儲中。
author: Courtney
feature: Reports and Dashboards
exl-id: 8348f5ff-c1f8-4608-b683-15f6407c6128
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/pPk3qt9-o3QhAajyI4eGhwe0J2tRphXDstrJxmdW8Ww
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 1489
ht-degree: 1%

---

# 建立與Workfront資料連線的連線

Workfront Data Connect可讓您將組織的Workfront資料與商業智慧工具搭配使用，或將其儲存在外部資料倉儲中。

若要將您的Data Connect Data Lake與外部產品連線，您必須先建立連線，如[建立Snowflake的讀取器帳戶或連線中所述](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md)。 然後，您必須依照以下[新增IP至允許清單](#add-ips-to-the-allowlist)中的說明，將任何必要的IP新增至允許清單。

大部分產品在建立連線時，都需要下列資料湖相關資訊：

| 欄位名稱 | 價值 |
|---------------|-------------|
| 伺服器 | 連線的URL，不含`https://`部分（可在Workfront的&#x200B;**資料連線**&#x200B;頁面上找到*） |
| 連接埠 | `443` |
| 資料庫 | `WORKFRONT` |
| 倉儲 | `READER_WH` |
| 結構描述 | `WF` |
| 角色 | `READER_ROLE` |
| 使用者名稱 | 建立連線時選擇的使用者名稱（可在Workfront的&#x200B;**Data Connect**&#x200B;頁面上找到*） |
| 密碼 | 首次Snowflake登入時選擇的密碼* |

*如需在何處尋找包含您連線的&#x200B;**資料連線**&#x200B;頁面的詳細資訊，請參閱[建立Snowflake的讀取器帳戶或連線](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md)。

>[!IMPORTANT]
>
>將一個專案新增到IP允許清單後，將不再允許所有其他IP位址。 在嘗試使用視覺化工具之前，請確定您已輸入所有必要的IP位址（包括建置和讀取視覺化工具的體驗）。 否則，您可能會遇到有關無效認證的錯誤。
>
>如果您的允許清單中未包含任何IP位址，但連線至BI工具時仍有問題，請檢查BI工具的Proxy伺服器設定。

## 存取權要求

+++ 展開以檢視存取需求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 封裝</td> 
   <td><p>Ultimate</p>
    <p>Workflow Ultimate</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>
   <p>標準</p>
   <p>規劃</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員</p></td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 將IP新增至允許清單

1. 按一下Adobe Workfront右上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon.png)，或（如果有的話）按一下左上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon-left-nav.png)，然後按一下&#x200B;**設定**。

1. 在左側面板中，按一下&#x200B;**系統** > **資料連線**。

1. 按一下「**允許的IP**」標籤，然後按一下「**新增IP位址至您的允許清單**」按鈕。

1. 在&#x200B;**IP位址描述**&#x200B;中輸入IP位址的名稱，並輸入您要在&#x200B;**IP位址**&#x200B;中使用的工具的IP位址（或CIDR區塊），然後按一下&#x200B;**新增IP至允許清單**。

   ![新增IP位址](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

## 尋找Microsoft Power BI的Azure IP範圍

Microsoft Power BI與Data Connect的流量並非來自單一固定位址。 Microsoft會將IP範圍發佈為大型JSON檔案中的CIDR區塊。 本節說明如何為您實際使用的區域尋找區塊。

### Azure IP範圍和服務標籤的官方Microsoft來源

Microsoft會在[Azure IP範圍和服務標籤 — 公用雲端下載頁面](https://www.microsoft.com/en-us/download/details.aspx?id=56519)上發佈清單。 下載目前的JSON檔案（檔案名稱通常類似於`ServiceTags_Public_YYYYMMDD.json`）。 當Microsoft更新此檔案，或在Microsoft變更後出現連線問題時，請重新整理允許清單。

>[!NOTE]
>
>JSON檔案非常大，通常超過100,000行。 這是預期中的情形。 您需要的區段很小；您不需要手動讀取整個檔案。

### Power BI與Power Query Online比較

客戶有時會在流量實際來自Power Query元件時報告「Power BI」，而Microsoft會將此類元件視為服務標籤清單中的個別Azure服務。

| 如果您的使用者…… | 在JSON中尋找此服務編號 |
|----------------|---------------------------------------|
| 使用Power BI服務、在Azure中託管的資料集或雲端內容中的閘道 | `PowerBI` （全域或區域專案，例如`PowerBI.EastUS`） |
| 使用Power Query Online、雲端資料流和類似的體驗 | `PowerQueryOnline` （全域或區域專案，例如`PowerQueryOnline.EastUS`） |

如果您的組織同時使用這兩種體驗，請為相同區域同時新增`PowerBI`和`PowerQueryOnline`的CIDR區塊。 如果您只新增使用者，有些使用者仍會被封鎖，而其他使用者則會成功。

### 選擇區域標籤，而非全域彙總

JSON檔案包含`PowerBI`的單一全區域專案（以及類似的`PowerQueryOnline`），可彙總許多區域且可包含數百個CIDR區塊，加上許多較小的區域專案，例如`PowerBI.WestUS`、`PowerBI.WestUS2`和`PowerBI.WestUS3`。 每個區域物件僅列出該區域的字首，通常最多數十行。 我們不建議新增全域專案，除非您有書面要求允許每個Azure區域。 對於大多數Data Connect客戶，區域專案是正確的預設值。 新增Power BI租使用者和使用者實際執行的地區，再加上用於備援的小緩衝區（例如貴公司使用的次要災難回覆地區）。

### 選擇您的地區

Microsoft在檔案中的區域名稱看起來像`EastUS`、`WestEurope`、`GermanyWestCentral`等等。 使用Power BI容量和使用者託管的地區，而非您的辦公室所在的地區，不過這些地區通常會保持一致。

| 情境 | 先新增什麼 |
|----------|-------------------|
| 美國使用情況 | 從您知道租使用者使用的美國地區開始（範例： `EastUS`、`EastUS2`、`WestUS`、`WestUS2`、`WestUS3`、`CentralUS`、`SouthCentralUS`）。 除非您的Microsoft管理員確認多地區託管，否則您不需要每個美國地區。 |
| 歐盟或英國使用方式 | 從您的租使用者使用的地區開始（範例： `WestEurope`、`NorthEurope`、`FranceCentral`、`GermanyWestCentral`、`SwedenCentral`、`UKSouth`）。 只有在使用者跨越其他Microsoft區域時才新增更多。 |
| 亞太地區使用情況 | 新增您的Power BI或Azure管理員確認的區域（範例： `SoutheastAsia`、`EastAsia`、`AustraliaEast`）。 |
| 多個地理位置 | 針對每個服務(`PowerBI`和`PowerQueryOnline` （如果兩者皆已使用），新增兩組地區標籤（例如EU和US）。 |
| 未知區域 | 請詢問您的Microsoft 365或Power BI管理員哪些Azure區域代管您的Power BI資源，或檢閱您的Power BI管理員租使用者設定。 如果您必須快速解除封鎖以進行測試，請新增一個已知區域配對（例如，`EastUS`和`WestUS`）並監視，然後在確認後縮小清單。 |

### 尋找IP範圍並將其新增至允許清單

若要從Microsoft收集IP範圍並將其新增至您的Workfront允許清單：

1. 開啟[Azure IP範圍和服務標籤 — 公用雲端下載頁面](https://www.microsoft.com/en-us/download/details.aspx?id=56519)，下載服務標籤JSON檔案，並將其儲存在本機（例如，`Downloads\ServiceTags_Public_YYYYMMDD.json`）。

1. 在任何可處理大型JSON的編輯器中（例如Visual Studio Code）開啟檔案。

1. 使用編輯器的尋找功能(`Ctrl+F` （在Windows上）或`Cmd+F` （在macOS上）尋找其`"name"`欄位等於服務標籤（例如`PowerBI.EastUS`或`PowerQueryOnline.WestEurope`）的JSON物件。 有用的搜尋：

   * `"name": "PowerBI.WestUS"` — 跳至West US Power BI。
   * `"name": "PowerQueryOnline.WestUS"` — 跳至West US Power Query Online。
   * `PowerBI.` — 列出所有Power BI地區標籤，然後調整為您的地區名稱。

1. 在每個相符的物件下，尋找名為`addressPrefixes`的陣列。 該陣列中的每個字串都是CIDR區塊（例如，`20.59.79.96/27`或IPv6首碼）。 這些是您將新增至Workfront允許清單的值。

1. 依照本文中[新增IP至允許清單](#add-ips-to-the-allowlist)的說明，將每個CIDR新增至Workfront允許清單。 如果您的環境快取規則，請等待幾分鐘讓原則傳播。

1. 從Power BI或Power Query Online，對Data Connect執行小型測試查詢以驗證連線。 如果失敗，請擷取約略時間，並詢問您的網路團隊拒絕次數是否與缺少的範圍一致。 重新檢查您是否在僅新增`PowerBI`時錯過`PowerQueryOnline`，這是常見的間隔。

例如，如果您的Microsoft管理員確認您的Power BI工作負荷使用West US、West US 2和West US 3，而您的使用者同時使用Power BI和Power Query Online，您會開啟六個物件： `PowerBI.WestUS`、`PowerBI.WestUS2`、`PowerBI.WestUS3`以及每個物件的相符`PowerQueryOnline.<Region>`，然後從所有六個物件複製`addressPrefixes`。

### JSON結構參考

每個產品服務編號區塊在概念上看起來類似以下內容。 真實檔案包含更多中繼資料。

```json
{
  "name": "PowerBI.WestUS2",
  "id": "PowerBI.WestUS2",
  "properties": {
    "region": "westus2",
    "systemService": "PowerBI",
    "addressPrefixes": [
      "203.0.113.0/24",
      "2001:db8::/32"
    ],
    "networkFeatures": ["API", "NSG", "UDR", "FW"]
  }
}
```

`addressPrefixes`陣列包含您將新增至Workfront的CIDR區塊。 其他欄位適用於Azure網路案例，不適用於此處。

### 維護允許清單

* Microsoft會隨著時間變更IP範圍。 當Microsoft發佈更新的JSON檔案時，請定期重新整理或比較您的允許清單，尤其是在連線事件發生後。
* 如果您的環境支援從IPv6到Snowflake，而Microsoft列出IPv6首碼，如果您的安全性原則允許IPv6，請包含這些首碼。 否則，請與您的網路團隊協調。

## 從允許清單中移除IP位址

1. 按一下Adobe Workfront右上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon.png)，或（如果有的話）按一下左上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon-left-nav.png)，然後按一下&#x200B;**設定**。

1. 在左側面板中，按一下&#x200B;**系統** > **資料連線**。

1. 按一下&#x200B;**允許的IP**&#x200B;標籤，然後按一下您要移除的IP位址右側的垃圾桶圖示![刪除圖示](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png)。

1. 在出現的視窗中，核取方塊以確認，然後按一下[刪除]。****

## 與商業智慧工具共用資料

以下列出許多常用的商業智慧工具；請造訪其檔案網站，以進一步瞭解如何連線至您的資料湖。

* Tableau
* Power BI
* Domo
* SAP HANA

## 將資料儲存在外部資料倉儲中

以下列出許多常見的資料倉儲；請造訪其檔案網站，以進一步瞭解如何連線至您的資料湖。

* Databricks
* AWS Redshift
