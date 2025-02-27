---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: 建立與Workfront資料連線的連線
description: Workfront Data Connect可讓您將組織的Workfront資料與商業智慧工具搭配使用，或將其儲存在外部資料倉儲中。
author: Nolan
feature: Reports and Dashboards
exl-id: 8348f5ff-c1f8-4608-b683-15f6407c6128
source-git-commit: ea9c674b798c48927c7a0a542d36d5ded15ea3f1
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 1%

---

# 建立與Workfront資料連線的連線

Workfront Data Connect可讓您將組織的Workfront資料與商業智慧工具搭配使用，或將其儲存在外部資料倉儲中。

若要將您的Data Connect Data Lake與外部產品連線，您必須先建立連線，如[建立Snowflake的讀取器帳戶或連線中所述](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md)。 然後，您必須依照以下[新增IP至允許清單](#add-ips-to-the-allowlist)中的說明，將任何必要的IP新增至允許清單。

大部分產品在建立連線時，都需要下列資料湖相關資訊：

| 欄位名稱 | 值 |
|---------------|-------------|
| 伺服器 | 連線的URL，不含`https://`部分(可在Workfront的&#x200B;**資料連線**&#x200B;頁面上找到*) |
| 連接埠 | `443` |
| 資料庫 | `WORKFRONT` |
| 倉儲 | `READER_WH` |
| 結構描述 | `WF` |
| 角色 | `READER_ROLE` |
| 使用者名稱 | 建立連線時選擇的使用者名稱(可在Workfront的&#x200B;**Data Connect**&#x200B;頁面上找到*) |
| 密碼 | 首次Snowflake登入時選擇的密碼* |

*如需在何處尋找包含您連線的&#x200B;**資料連線**&#x200B;頁面的詳細資訊，請參閱[建立Snowflake的讀取器帳戶或連線](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md)。

>[!IMPORTANT]
>
>將一個專案新增到IP允許清單後，將不再允許所有其他IP位址。 在嘗試使用視覺化工具之前，請確定您已輸入所有必要的IP位址（包括建置和讀取視覺化工具的體驗）。 否則，您可能會遇到有關無效認證的錯誤。
>
>如果您的允許清單中未包含任何IP位址，但連線至BI工具時仍有問題，請檢查BI工具的Proxy伺服器設定。

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
        <li><p>Ultimate</p></li> 
    </ul>    
   <!--<p>Can be purchased as an add-on to the following plans:</p> 
    <ul>
        <li>Select</li> 
        <li>Prime</li>
    </ul>--> 
    <p>Workfront Data Connect不適用於舊版Workfront計畫。</p> 
   </td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>規劃</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員。</p></td> 
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

* 資料庫資料
* AWS Redshift
