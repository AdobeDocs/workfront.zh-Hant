---
content-type: reference
product-area: reports and dashboards
navigation-topic: data lake
title: 建立用於Snowflake的讀取器（服務）帳戶
description: 若要存取Workfront Data Lake中的資料，您必須先建立讀取器帳戶以進行Snowflake。
author: Nolan
feature: Reports and Dashboards
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 7d24659833f0ac0ceeecb245358f2ade8bd08a17
workflow-type: tm+mt
source-wordcount: '556'
ht-degree: 0%

---

# 建立用於Snowflake的讀取器（服務）帳戶

若要存取Workfront Data Lake資料，您必須先建立讀取器帳戶以進行Snowflake。 此外，您必須將IP新增至您打算連線至資料的任何外部工具的允許清單。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td>Ultimate</td> 
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

1. 您現在可以使用使用者名稱和新密碼來存取Snowflake中的Workfront Data Lake。

## 將IP新增至允許清單

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon.png) 在Adobe Workfront的右上角，或（如果有的話）按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon-left-nav.png) 然後按一下「 」 **設定**.

1. 在左側面板中，按一下 **系統** > **資料存取**.

1. 按一下 **允許的IP** 標籤，然後按一下 **新增IP位址到您的允許清單** 按鈕。

   ![新增IP位址](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

1. 在中輸入IP位址的名稱 **IP位址說明** 並輸入您要用於工具的網址 **IP位址**，然後按一下 **新增IP至允許清單**.

## 撤銷Reader帳戶或從允許清單中移除IP位址

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon.png) 在Adobe Workfront的右上角，或（如果有的話）按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon-left-nav.png) 然後按一下「 」 **設定**.

1. 在左側面板中，按一下 **系統** > **資料存取**.

1. 按一下垃圾桶圖示 ![「刪除」圖示](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) 位於您要撤銷之帳戶的右側。

   或

   按一下 **允許的IP** 標籤，然後按一下垃圾桶圖示 ![「刪除」圖示](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) 右邊的IP位址。

1. 在出現的視窗中，核取方塊以確認，然後按一下 **刪除**.
