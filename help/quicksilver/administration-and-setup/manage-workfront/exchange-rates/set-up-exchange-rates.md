---
user-type: administrator
product-area: system-administration;setup
navigation-topic: exchange-rates
title: 身為Adobe Workfront管理員，您可以在Workfront中設定貨幣匯率。
description: 設定匯率
feature: System Setup and Administration
role: Admin
exl-id: 149c08de-fd3a-465a-afd1-0b53012d30d8
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 0%

---

# 設定匯率

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

身為Adobe Workfront管理員，您可以在Workfront中設定貨幣匯率。 這包括下列項目：

* 設定Workfront系統的預設貨幣
* 更新Workfront的匯率以匹配當前匯率
* 為多種貨幣設定匯率（這樣可讓使用者為個別專案選擇預設貨幣）

匯率影響了Workfront的所有金融因素。 「基本貨幣」是整個系統中所有項目的預設貨幣，除非為給定項目或職務職責改寫它。 在報表或清單中查看財務資訊時，您也可以選擇以系統中可用的貨幣或項目貨幣以外的貨幣顯示財務資訊。 如需詳細資訊，請參閱 [使用獨特的匯率建立財務資料報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

如需針對專案和工作角色在Workfront中覆寫基本貨幣的詳細資訊，請參閱下列文章：

* [更改項目幣種](../../../manage-work/projects/project-finances/change-project-currency.md)
* [建立和管理作業角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)

設定匯率的方式會影響用戶是否可以修改給定項目的匯率。

>[!IMPORTANT]
>
>Workfront的匯率並非動態的；當匯率發生變化時，必須更新您設定的值。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置</td> 
   <td> <p>您必須是Workfront管理員。</p> <p><b>注意</b>:如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 設定匯率

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **專案偏好設定** > **匯率。**

1. 按一下 **新增貨幣。**
1. 開始輸入貨幣名稱，然後在貨幣出現在下拉式清單中時按一下。

1. 在提供的欄位中，指定所選貨幣的匯率，因為它與在系統中設定為基本貨幣的貨幣相關。
1. （選用）將貨幣設為Workfront的基本（預設）貨幣。

   這是系統中所有專案和報表的預設貨幣。

1. 按一下 **儲存** 來儲存變更。

## 讓使用者修改專案的預設貨幣

符合下列條件時，使用者可以修改專案的預設貨幣：

* 用戶具有對匯率的管理訪問權限的計畫許可證。

   如需詳細資訊，請參閱 [授予用戶對特定區域的管理訪問權限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* 在Workfront系統上啟用了多個貨幣。

如需使用者如何變更指定專案的預設貨幣的詳細資訊，請參閱 [更改項目幣種](../../../manage-work/projects/project-finances/change-project-currency.md).

## 允許用戶修改作業角色的預設貨幣

滿足以下條件時，用戶可以修改作業角色的貨幣：

* 用戶具有對「作業角色」的管理訪問權限的計畫許可證。

   如需詳細資訊，請參閱 [授予用戶對特定區域的管理訪問權限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* 在Workfront系統中啟用了多個貨幣。

有關用戶如何更改指定職務角色的預設貨幣的資訊，請參閱 [建立和管理作業角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
