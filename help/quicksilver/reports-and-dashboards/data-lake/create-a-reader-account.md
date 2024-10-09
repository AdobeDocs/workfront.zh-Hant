---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: 建立用於Snowflake的讀取器（服務）帳戶
description: 若要存取Data Connect資料，您必須先建立Snowflake讀取器帳戶。
author: Nolan
feature: Reports and Dashboards
exl-id: 70d83a10-f926-4229-ac10-7659f2ca5e7a
source-git-commit: 4c8b7e7f33ec593b2942725eb9160f7fbe2962e3
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 0%

---

# 建立用於Snowflake的讀取器（服務）帳戶

若要存取Data Connect資料，您必須先為每個新連線建立Snowflake讀取器（或服務）帳戶。 建立連線後，您可以在&#x200B;**現有連線**&#x200B;標籤下的&#x200B;**資料存取**&#x200B;頁面（**主功能表** > **設定** > **系統** > **資料存取**）上按一下連線，以找到其相關聯的URL和使用者名稱。

如需有關使用新建立的外部產品連線的資訊，請參閱[建立與Workfront Data Connect的連線](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md)。

## 存取需求

+++ 展開以檢視存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td><p>包含在下列計畫中：</p>
    <ul>
        <li>Ultimate</li> 
    </ul>    
   <p>可作為下列計畫的附加元件購買：</p> 
    <ul>
        <li>選取</li> 
        <li>Prime</li>
    </ul> 
    <p>Workfront Data Connect不適用於舊版Workfront計畫。</p> 
   </td> </td> 
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

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 建立讀者帳戶

1. 按一下Adobe Workfront右上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon.png)，或（如果有的話）按一下左上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon-left-nav.png)，然後按一下&#x200B;**設定**。

1. 在左側面板中，按一下&#x200B;**系統** > **資料存取**。

1. 按一下&#x200B;**建立新連線**

1. 在出現的視窗中，在&#x200B;**連線參考描述**&#x200B;中輸入連線的名稱，並在&#x200B;**連線使用者**&#x200B;中輸入使用者名稱，然後按一下&#x200B;**產生連線**。

   ![建立讀取器帳戶](/help/quicksilver/reports-and-dashboards/data-lake/assets/new-reader-connection.png) {width="500"}

1. 將會產生&#x200B;**預設密碼**，以及可透過Snowflake檢視您資料的URL。 您必須使用密碼搭配您選擇用來首次Snowflake的使用者名稱，以確保您同時保留該密碼和URL的記錄。 核取宣告您已完成此作業的方塊，然後按一下&#x200B;**關閉**。

   ![預設帳戶密碼](/help/quicksilver/reports-and-dashboards/data-lake/assets/default-password-reader-account.png) {width="500"}

1. 使用瀏覽器開啟Snowflake以瀏覽至上一步驟的URL，輸入您選取的使用者名稱和上一步驟的預設密碼，然後按一下&#x200B;**登入**。

1. 第一次成功登入後，系統會提示您選擇新密碼。 在&#x200B;**新密碼**&#x200B;和&#x200B;**確認密碼**&#x200B;欄位中輸入您選擇的密碼，然後按一下&#x200B;**提交**。

   ![重設Snowflake密碼](/help/quicksilver/reports-and-dashboards/data-lake/assets/reset-snowflake-password.png) {width="300"}

1. 您現在可以使用使用者名稱和新密碼，在Snowflake或您選擇的商業視覺化工具中存取您的Data Connect Data Lake。

## 撤銷Reader帳戶

1. 按一下Adobe Workfront右上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon.png)，或（如果有的話）按一下左上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon-left-nav.png)，然後按一下&#x200B;**設定**。

1. 在左側面板中，按一下&#x200B;**系統** > **資料存取**。

1. 按一下您要撤銷之帳戶右側的垃圾桶圖示![刪除圖示](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png)。

1. 在出現的視窗中，核取方塊以確認，然後按一下[刪除]。****
