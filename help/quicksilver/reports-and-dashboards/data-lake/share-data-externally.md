---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: 建立與Workfront資料湖的連線
description: Workfront data lake可讓您將組織的Workfront資料與熱門的商業智慧工具搭配使用，或將其儲存在外部資料倉儲中。
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 8348f5ff-c1f8-4608-b683-15f6407c6128
source-git-commit: 1723609ce790566c072d071f9ac627dba7dc5350
workflow-type: tm+mt
source-wordcount: '611'
ht-degree: 1%

---

# 建立與Workfront資料連線的連線

Workfront Data Connect可讓您將組織的Workfront資料與商業智慧工具搭配使用，或將其儲存在外部資料倉儲中。

若要將您的Data Connect資料湖連線到外部產品，您必須先將任何必要的IP新增到允許清單，如下文[將IP新增到允許清單](#add-ips-to-the-allowlist)中所述。 此外，大部分產品在建立連線時，都需要您提供資料湖的其他相關資訊：

| 欄位名稱 | 值 |
|---------------|-------------|
| 伺服器 | 連線的URL，不含`https://`部分(可在Workfront的&#x200B;**資料存取**&#x200B;頁面上找到*) |
| 連接埠 | `443` |
| 資料庫 | `WORKFRONT` |
| 倉儲 | `READER_WH` |
| 結構描述 | `WF` |
| 角色 | `READER_ROLE` |
| 使用者名稱 | 建立連線時選擇的使用者名稱(可在Workfront的&#x200B;**資料存取**&#x200B;頁面上找到*) |
| 密碼 | 首次Snowflake登入時選擇的密碼* |

*如需在何處尋找包含您的Data Connect連線的&#x200B;**資料存取**&#x200B;頁面的詳細資訊，請參閱[為Snowflake建立讀取器（服務）帳戶](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md)。

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

## 將IP新增至允許清單

1. 按一下Adobe Workfront右上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon.png)，或（如果有的話）按一下左上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon-left-nav.png)，然後按一下&#x200B;**設定**。

1. 在左側面板中，按一下&#x200B;**系統** > **資料存取**。

1. 按一下「**允許的IP**」標籤，然後按一下「**新增IP位址至您的允許清單**」按鈕。

1. 在&#x200B;**IP位址描述**&#x200B;中輸入IP位址的名稱，並輸入您要在&#x200B;**IP位址**&#x200B;中使用的工具的IP位址（或CIDR區塊），然後按一下&#x200B;**新增IP至允許清單**。

   ![新增IP位址](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

## 從允許清單中移除IP位址

1. 按一下Adobe Workfront右上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon.png)，或（如果有的話）按一下左上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon-left-nav.png)，然後按一下&#x200B;**設定**。

1. 在左側面板中，按一下&#x200B;**系統** > **資料存取**。

1. 按一下&#x200B;**允許的IP**&#x200B;標籤，然後按一下您要移除的IP位址右側的垃圾桶圖示![刪除圖示](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png)。

1. 在出現的視窗中，核取方塊以確認，然後按一下[刪除]。****

## 與商業智慧工具共用資料

以下列出許多常見的業務智慧工具；這些連結會帶您前往服務的檔案網站，以進一步瞭解如何連線至您的資料湖。

* [Tableau](https://help.tableau.com/current/pro/desktop/en-us/basicconnectoverview.htm)
* [Power BI](https://learn.microsoft.com/power-query/connectors/snowflake)
* [Domo](https://www.domo.com/appstore/connector/snowflake-connector/overview)
* SAP HANA

## 將資料儲存在外部資料倉儲中

以下列出許多常見的資料倉儲；連結會帶您前往每個服務的檔案網站，讓您瞭解更多有關連線至資料湖的資訊。

* [資料庫](https://docs.databricks.com/en/connect/index.html)
* [AWS Redshift](https://docs.aws.amazon.com/redshift/latest/gsg/federated-query.html)
