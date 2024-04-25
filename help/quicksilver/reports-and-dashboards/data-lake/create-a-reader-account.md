---
content-type: reference
product-area: reports and dashboards
navigation-topic: data lake
title: 建立用於Snowflake的讀取器（服務）帳戶
description: 若要存取Workfront Data Lake中的資料，您必須先建立讀取器帳戶以進行Snowflake。
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 70d83a10-f926-4229-ac10-7659f2ca5e7a
source-git-commit: e5bd25315062ad15ccd3448e008dfe94f1b616da
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# 建立用於Snowflake的讀取器（服務）帳戶

若要存取Workfront Data Lake資料，您必須先為每個新連線建立Snowflake讀取器（或服務）帳戶。 建立連線後，按一下 **資料存取** 頁面(**主功能表** > **設定** > **系統** > **資料存取**)下 **現有連線** 標籤。

如需將新建立的連線與外部產品搭配使用的詳細資訊，請參閱 [建立與Workfront資料湖的連線](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md).

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td>待定</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員。</p></td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 建立讀者帳戶

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon.png) 在Adobe Workfront的右上角，或（如果有的話）按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon-left-nav.png) 然後按一下「 」 **設定**.

1. 在左側面板中，按一下 **系統** > **資料存取**.

1. 按一下 **建立新連線**

1. 在出現的視窗中，輸入連線的名稱 **連線參考說明** 和中的使用者名稱 **連線使用者**，然後按一下 **產生連線**.

   ![建立讀者帳戶](/help/quicksilver/reports-and-dashboards/data-lake/assets/new-reader-connection.png) {width="500"}

1. A **預設密碼** 將會產生，以及可透過Snowflake檢視您資料的URL。 您必須使用密碼搭配您選擇用來首次Snowflake的使用者名稱，以確保您同時保留該密碼和URL的記錄。 勾選宣告您已完成此作業的方塊，然後按一下 **關閉**.

   ![預設帳戶密碼](/help/quicksilver/reports-and-dashboards/data-lake/assets/default-password-reader-account.png) {width="500"}

1. 使用瀏覽器開啟Snowflake以瀏覽至上一步驟的URL，輸入您選取的使用者名稱和上一步驟的預設密碼，然後按一下 **登入**.

1. 第一次成功登入後，系統會提示您選擇新密碼。 輸入您選擇的密碼，在 **新密碼** 和 **確認密碼** 欄位，然後按一下 **提交**.

   ![重設Snowflake密碼](/help/quicksilver/reports-and-dashboards/data-lake/assets/reset-snowflake-password.png) {width="300"}

1. 您現在可以使用使用者名稱和新密碼，在Snowflake或您選擇的業務視覺化工具中存取您的Workfront Data Lake。

## 撤銷Reader帳戶

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon.png) 在Adobe Workfront的右上角，或（如果有的話）按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon-left-nav.png) 然後按一下「 」 **設定**.

1. 在左側面板中，按一下 **系統** > **資料存取**.

1. 按一下垃圾桶圖示 ![「刪除」圖示](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) 位於您要撤銷之帳戶的右側。

1. 在出現的視窗中，核取方塊以確認，然後按一下 **刪除**.
