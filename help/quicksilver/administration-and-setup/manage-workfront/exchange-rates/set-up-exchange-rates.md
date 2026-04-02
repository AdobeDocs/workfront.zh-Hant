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
source-git-commit: b16523bf6c37747702efe3b5ecfcc33801526af1
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 4%

---

# 設定匯率

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

{{highlighted-preview}}

身為Adobe Workfront管理員，您可以在Workfront中設定貨幣匯率。 這包含下列專案：

* 設定Workfront系統的預設貨幣
* 更新Workfront中的匯率以符合目前的匯率
* 設定多種貨幣的匯率（如此可讓使用者為個別專案選擇預設貨幣）

匯率會影響Workfront中的所有財務元素。 基本貨幣是整個系統內所有專案和報表的預設貨幣，除非針對特定專案或工作角色覆寫基本貨幣。 清單中目前的基本貨幣或預設貨幣會以圖示![預設貨幣圖示](assets/default-icon.png)表示。 您也可以選取在報表或清單中檢視時，以系統中可用的貨幣顯示財務資訊，這些貨幣與基礎貨幣或專案中的貨幣不同。 如需詳細資訊，請參閱[建立具有唯一匯率的財務資料報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md)。

如需為專案和工作角色覆寫Workfront中基本貨幣的相關資訊，請參閱下列文章：

* [變更專案貨幣](../../../manage-work/projects/project-finances/change-project-currency.md)
* [建立和管理職務角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)

您設定匯率的方式會影響使用者是否可以修改指定專案的匯率。

>[!IMPORTANT]
>
>Workfront中的匯率不是動態的；您設定的值必須在匯率發生變更時更新。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 封裝</td> 
   <td><p>若要設定匯率：任何Workfront或Workflow套件</p>
       <p>若要套用有效日期至匯率：工作流程Ultimate套件</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td><p>標準</p>
       <p>規劃</p></td>
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td>系統管理員</td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

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

     新的預設貨幣已更新，圖示為![預設貨幣圖示](assets/default-icon.png)。

     >[!NOTE]
     >
     >預設貨幣一律顯示在清單的第一位，無論清單如何排序。

1. （選擇性）若要刪除貨幣，請選取貨幣名稱旁的核取方塊，然後在畫面底部的動作列中選取&#x200B;**刪除**。 您無法刪除預設貨幣。

<div class="preview">

## 設定貨幣匯率的有效日期

幣別匯率的有效日期設定為匯率值在特定日期結束，而另一個匯率開始。 然後會在財務計算中使用正確日期的匯率。

{{step-1-to-setup}}

1. 按一下&#x200B;**專案偏好設定** > **匯率**。
1. 在清單中選取貨幣，然後按一下動作列上的&#x200B;**管理日期**。
1. 在&#x200B;**（貨幣名稱）日期有效匯率**&#x200B;對話方塊中，選擇目前匯率的&#x200B;**結束日期**。

   或

   選擇新匯率的&#x200B;**開始日期**。

   第一個匯率沒有開始日期，最後一個匯率沒有結束日期。 部分日期會自動新增。 例如，如果第一個匯率沒有結束日期，而您新增了開始日期為2025年12月1日的匯率，則結束日期為2025年11月30日的匯率會新增到第一個匯率，這樣就不會有間隙。

   ![日期有效匯率對話方塊](assets/euro-date-effective-rates.png)

1. 輸入新的&#x200B;**匯率**&#x200B;值。
1. （選擇性）按一下&#x200B;**新增日期有效匯率**&#x200B;以新增此貨幣的有效日期匯率。
1. 按一下「**儲存**」。

</div>

## 讓使用者修改專案的預設貨幣

使用者可在符合下列條件時修改專案的預設貨幣：

* 使用者擁有對匯率具有管理存取權的標準或計畫授權。

  如需詳細資訊，請參閱[授予使用者對特定區域的管理存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)。

* Workfront系統啟用多種貨幣。

若要瞭解使用者如何變更特定專案的預設貨幣，請參閱[變更專案貨幣](../../../manage-work/projects/project-finances/change-project-currency.md)。

## 允許使用者修改工作角色的預設貨幣

當滿足以下條件時，使用者可以修改工作角色的貨幣：

* 使用者擁有對工作角色具有管理存取權的標準或計畫授權。

  如需詳細資訊，請參閱[授予使用者對特定區域的管理存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)。

* Workfront系統中啟用了多種貨幣。

若要瞭解使用者如何變更指定工作角色的預設貨幣，請參閱[建立和管理工作角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)。



