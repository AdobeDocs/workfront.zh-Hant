---
user-type: administrator
product-area: system-administration;setup
navigation-topic: exchange-rates
title: 設定匯率
description: 匯率會影響Workfront中的所有財務元素。 基礎貨幣是整個系統內所有專案的預設貨幣。
feature: System Setup and Administration
role: Admin
author: Lisa
exl-id: 149c08de-fd3a-465a-afd1-0b53012d30d8
source-git-commit: cb12c715d6b20dd4737e2d2e29d9849f08ce67e9
workflow-type: tm+mt
source-wordcount: '634'
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

匯率會影響Workfront中的所有財務元素。 基本貨幣是整個系統內所有專案的預設貨幣，除非指定專案或工作角色會覆寫基本貨幣。 清單中目前的基本貨幣或預設貨幣會以圖示![預設貨幣圖示](assets/default-icon.png)表示。 您也可以選取在報表或清單中檢視時，以系統中可用的貨幣顯示財務資訊，這些貨幣與基礎貨幣或專案中的貨幣不同。 如需詳細資訊，請參閱[建立具有唯一匯率的財務資料報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md)。

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

1. 按一下&#x200B;**專案偏好設定** > **匯率**。

1. 按一下&#x200B;**新增貨幣**。
1. 在&#x200B;**新增貨幣**&#x200B;方塊中，開始輸入貨幣的名稱，然後當它出現在下拉式清單中時按一下它。
1. 在&#x200B;**匯率**&#x200B;欄位中，輸入您所選取貨幣的匯率，與系統中設定為基礎貨幣的匯率比較。
1. 按一下&#x200B;**新增**&#x200B;以新增貨幣及其匯率。
1. （選用）若要變更基本（預設）貨幣，請執行下列任一項作業：

   * 選取貨幣名稱旁的核取方塊，並在熒幕底部的動作列中選取&#x200B;**設定預設值**。
   * 將滑鼠停留在貨幣名稱上，然後按一下出現的&#x200B;**更多**&#x200B;功能表。 然後，選取&#x200B;**設定預設值**。

     新的預設貨幣會以圖示更新。

1. （選擇性）若要刪除貨幣，請選取貨幣名稱旁的核取方塊，然後在畫面底部的動作列中選取&#x200B;**刪除**。 您無法刪除預設貨幣。

## 讓使用者修改專案的預設貨幣

使用者可在符合下列條件時修改專案的預設貨幣：

* 使用者的「標準」或「計畫」授權具有「匯率」的管理存取權。

  如需詳細資訊，請參閱[授予使用者對特定區域的管理存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)。

* Workfront系統啟用多種貨幣。

若要瞭解使用者如何變更特定專案的預設貨幣，請參閱[變更專案貨幣](../../../manage-work/projects/project-finances/change-project-currency.md)。

## 允許使用者修改工作角色的預設貨幣

當滿足以下條件時，使用者可以修改工作角色的貨幣：

* 使用者擁有對工作角色具有管理存取權的標準或計畫授權。

  如需詳細資訊，請參閱[授予使用者對特定區域的管理存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)。

* Workfront系統中啟用了多種貨幣。

若要瞭解使用者如何變更指定工作角色的預設貨幣，請參閱[建立和管理工作角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)。


<!--The default currency is the currency that is used as the default for all projects and reports throughout the system. The current default is indicated with an icon ![Default currency icon](assets/default-icon.png).-->
