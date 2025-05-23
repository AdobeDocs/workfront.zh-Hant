---
user-type: administrator
product-area: system-administration;setup
navigation-topic: exchange-rates
title: 設定匯率
description: 身為Adobe Workfront管理員，您可以在Workfront中設定貨幣匯率。
feature: System Setup and Administration
role: Admin
author: Lisa
exl-id: 149c08de-fd3a-465a-afd1-0b53012d30d8
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 2%

---

# 設定匯率

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

身為Adobe Workfront管理員，您可以在Workfront中設定貨幣匯率。 這包含下列專案：

* 設定Workfront系統的預設貨幣
* 更新Workfront中的匯率以符合目前的匯率
* 設定多種貨幣的匯率（如此可讓使用者為個別專案選擇預設貨幣）

匯率會影響Workfront中的所有財務元素。 「基本貨幣」是整個系統內所有專案的預設貨幣，除非針對指定的專案或工作角色覆寫它。 您也可以選取在報表或清單中檢視時，以系統中可用的貨幣顯示財務資訊，這些貨幣與基礎貨幣或專案中的貨幣不同。 如需詳細資訊，請參閱[建立具有唯一匯率的財務資料報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md)。

如需為專案和工作角色覆寫Workfront中基本貨幣的相關資訊，請參閱下列文章：

* [變更專案貨幣](../../../manage-work/projects/project-finances/change-project-currency.md)
* [建立和管理職務角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)

您設定匯率的方式會影響使用者是否可以修改指定專案的匯率。

>[!IMPORTANT]
>
>Workfront中的匯率不是動態的；您設定的值必須在匯率發生變更時更新。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>新增：標準</p>
       <p>或</p>
       <p>目前：計畫</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td>[!UICONTROL 系統管理員]</td>
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 設定匯率

{{step-1-to-setup}}

1. 按一下&#x200B;**專案偏好設定** > **匯率。**

1. 按一下&#x200B;**新增貨幣。**
1. 開始輸入貨幣名稱，然後在貨幣出現在下拉式清單中時按一下貨幣。

1. 在提供的欄位中，指定所選貨幣的匯率，因為該匯率與系統中設定為基本貨幣的貨幣相關。
1. （選用）將貨幣設為Workfront的基礎（預設）貨幣。

   此貨幣是用作整個系統中所有專案和報表的預設貨幣。

1. 按一下[儲存]儲存變更。**&#x200B;**

## 讓使用者修改專案的預設貨幣

使用者可在符合下列條件時修改專案的預設貨幣：

* 使用者擁有管理匯率存取權的計畫授權。

  如需詳細資訊，請參閱[授予使用者對特定區域的管理存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)。

* Workfront系統啟用多種貨幣。

若要瞭解使用者如何變更特定專案的預設貨幣，請參閱[變更專案貨幣](../../../manage-work/projects/project-finances/change-project-currency.md)。

## 允許使用者修改工作角色的預設貨幣

當滿足以下條件時，使用者可以修改工作角色的貨幣：

* 使用者擁有對工作角色具有管理存取權的計畫授權。

  如需詳細資訊，請參閱[授予使用者對特定區域的管理存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)。

* Workfront系統中啟用了多種貨幣。

若要瞭解使用者如何變更指定工作角色的預設貨幣，請參閱[建立和管理工作角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)。
