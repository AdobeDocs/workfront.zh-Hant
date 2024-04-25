---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data lake
title: 建立與Workfront資料湖的連線
description: Workfront data lake可讓您將組織的Workfront資料與熱門的商業智慧工具搭配使用，或將其儲存在外部資料倉儲中。
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 8348f5ff-c1f8-4608-b683-15f6407c6128
source-git-commit: e5bd25315062ad15ccd3448e008dfe94f1b616da
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 1%

---

# 建立與Workfront資料湖的連線

Workfront data lake可讓您透過商業智慧工具使用組織的Workfront資料，或將其儲存在外部資料倉儲中。

為了將您的Workfront資料湖資料與外部產品連線，您必須先將任何必要的IP新增到允許清單，如中所述 [將IP新增至允許清單](#add-ips-to-the-allowlist) 底下。 此外，大部分產品在建立連線時，都需要您提供資料湖的其他相關資訊：

| 欄位名稱 | 值 |
|---------------|-------------|
| 伺服器 | 連線的URL，不含 `https://` 部分(可在 **資料存取** 頁面(在Workfront中) |
| 連接埠 | `443` |
| 資料庫 | `WORKFRONT` |
| 倉儲 | `READER_WH` |
| 結構描述 | `WF` |
| 角色 | `READER_ROLE` |
| 使用者名稱 | 建立連線時選擇的使用者名稱(可在 **資料存取** 頁面(在Workfront中) |
| 密碼 | 首次Snowflake登入時選擇的密碼* |

*如需在何處尋找 **資料存取** 包含資料湖連線的頁面，請參閱 [建立用於Snowflake的讀取器（服務）帳戶](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md).

>[!IMPORTANT]
>
>將一個專案新增到IP允許清單後，將不再允許所有其他IP位址。 在嘗試使用視覺化工具之前，請確定您已輸入所有必要的IP位址（包括建置和讀取視覺化工具的體驗）。 否則，您可能會遇到有關無效認證的錯誤。

## 將IP新增至允許清單

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon.png) 在Adobe Workfront的右上角，或（如果有的話）按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon-left-nav.png) 然後按一下「 」 **設定**.

1. 在左側面板中，按一下 **系統** > **資料存取**.

1. 按一下 **允許的IP** 標籤，然後按一下 **新增IP位址到您的允許清單** 按鈕。

1. 在中輸入IP位址的名稱 **IP位址說明** 並輸入您要用於工具的網址 **IP位址**，然後按一下 **新增IP至允許清單**.

   ![新增IP位址](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

## 從允許清單中移除IP位址

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon.png) 在Adobe Workfront的右上角，或（如果有的話）按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon-left-nav.png) 然後按一下「 」 **設定**.

1. 在左側面板中，按一下 **系統** > **資料存取**.

1. 按一下 **允許的IP** 標籤，然後按一下垃圾桶圖示 ![「刪除」圖示](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) 右邊的IP位址。

1. 在出現的視窗中，核取方塊以確認，然後按一下 **刪除**.

## 與商業智慧工具共用資料

以下列出許多常見的業務智慧工具；這些連結會帶您前往服務的檔案網站，以進一步瞭解如何連線至您的資料湖。

* [Tableau](https://help.tableau.com/current/pro/desktop/en-us/basicconnectoverview.htm)
* [Power BI](https://learn.microsoft.com/power-query/connectors/snowflake)
* [Domo](https://www.domo.com/appstore/connector/snowflake-connector/overview)
* SAP HANA

## 將資料儲存在外部資料倉儲中

以下列出許多常見的資料倉儲；連結會帶您前往每個服務的檔案網站，讓您瞭解更多有關連線至資料湖的資訊。

* [資料庫資料](https://docs.databricks.com/en/connect/index.html)
* [AWS Redshift](https://docs.aws.amazon.com/redshift/latest/gsg/federated-query.html)
