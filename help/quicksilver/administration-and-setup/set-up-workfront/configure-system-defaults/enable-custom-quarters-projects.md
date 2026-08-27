---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 啟用自訂季度
description: 若您組織的季度是根據行事曆日期以外的特定條件（例如營業日或購物日），基於報表目的，您可能會想要建立自訂季度。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0f643d36-6235-4fd3-b6d3-54fbd03c9b33
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/8kRfZ17zcgN0-hlc16wh328YGRjTlzuI3LAe-Yjj25s
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 914f1f8a25aa5b9e1045d2f940ed15061301c21b
workflow-type: tm+mt
source-wordcount: 376
ht-degree: 4%

---

# 啟用自訂季度

<!--Audited: 03/2026-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

若您組織的季度是根據行事曆日期以外的特定條件（例如營業日或購物日），基於報表目的，您可能會想要建立自訂季度。

根據貴公司已購買的產品，您可以在Workfront設定區域中設定下列季度數：

* 僅購買[!DNL Workfront]的客戶，最多可以為其[!DNL Adobe Workfront]系統設定8個自訂季度。
* 購買[!DNL Workfront]和[!DNL Workfront Planning]的客戶可以為其[!DNL Workfront]系統設定最多100個季度，這些季度也可在[!DNL Planning]中使用。

<!--
<div class="preview">
* Customers who purchased [!DNL Workfront] and [!DNL Workfront Planning], can configure custom weeks for each custom quarter which are visible in the [!DNL Planning] timeline views. 
</div>
-->


## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 封裝</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 授權</td> 
   <td><p>[!UICONTROL Workflow Standard]或[!UICONTROL Workfront Plan]授權</p>
       <p></p></td>
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td>[!UICONTROL 系統管理員]</td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--
When we release fiscal weeks, replace the table above with this:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td>
   <ul>
   <li><p>To configure custom quarters:</p>
   <p>Any Workfront or Workflow package</p></li>
   <li>
   <div class="preview">
   <p>To configure custom weeks:</p>
   <p>Any Planning package, including Planning as a standalone product</p>
   </div>
   </li>
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] license</td> 
   <td>
   
   <ul>
   <li><p>To configure custom quarters:</p>
   <p>[!UICONTROL Workflow Standard] or [!UICONTROL Workfront Plan] license</p></li>
   <li>
   <div class="preview">
   <p>To configure custom weeks:</p>
   <p>A [!UICONTROL Planning Standard] license, in addition to a Workfront or a Workflow license</p>
   </div>
   </li>
   </ul>
    </td>
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

-->


## 為您的[!DNL Workfront]系統設定自訂季度

<!--
Setting up custom quarters differs depending on which environment you use. 

### Set up custom quarters for your [!DNL Workfront] system in the Production environment
-->

{{step-1-to-setup}}

1. 按一下&#x200B;**[!UICONTROL 自訂季度]**。

1. 選取&#x200B;**[!UICONTROL 啟用自訂季度]**。

1. 輸入自訂季度的名稱，例如「2021年第一財政年度」。
1. 選取自訂季度的開始和結束日期。

   ![自訂季度](assets/custom-quarters-nwe.png)

1. （選擇性）按一下&#x200B;**[!UICONTROL 新增自訂季度]**&#x200B;以新增其他自訂季度至系統。

   >[!IMPORTANT]
   >
   > 如果貴公司已購買[!DNL Workfront Planning]，如果季度之間存在間隔或重疊，則您無法儲存自訂季度。
   >![自訂季度有重疊警告](assets/custom-quarters-with-overlap-warning.png)
   >只有[!DNL Workfront]個客戶才允許季之間的間隔和重疊。

1. （選擇性和條件性）如果貴公司只購買了[!DNL Workfront]，而沒有購買[!DNL Workfront Planning]，請建立參考會計季的報表元素。

   **範例：**&#x200B;為[!UICONTROL 專案]清單建立篩選器，並包含參考自訂季度的專案計畫完成日期。

   ![包含自訂季數的專案篩選器](assets/example-of-project-filter-with-custom-quarters.png)

   「本季」、「下一季」和「上一季」的參考資料會取代為自訂季度的新參考資料。

   如需有關報告元素的資訊，請參閱[報告元素：篩選器、檢視和群組](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)。

   如需建立篩選的詳細資訊，請參閱[在 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)中建立或編輯篩選。
1. （選擇性和條件性）如果貴公司已購買Workfront Planning，而您擁有[!DNL Workfront Planning]的存取權，請移至記錄型別頁面並開啟時間表檢視。 檢視會顯示新的自訂季度。
如需詳細資訊，請參閱[管理時間表檢視](/help/quicksilver/planning/views/manage-the-timeline-view.md)。

<!--
<div class="preview">

### Set up custom quarters for your [!DNL Workfront] system in the Preview environment

>[!NOTE]
>
>If your organization purchased a Planning package in addition to a Workflow package, or if they purchased  Workfront Planning as a standalone package, you can configure custom quarters as well as custom weeks. 


{{step-1-to-setup}}

1. Click **[!UICONTROL Custom Quarters]**.

1. Select **[!UICONTROL Enable Custom Quarters]**.

1. Type a name for the custom quarter, such as "Fiscal Q1 2021."
1. Select start and end dates for the custom quarter.

1. (Optional) Select the **Starts a new custom week sequence** option

1. (Optional) Click **[!UICONTROL Add Custom Quarter]** to add additional custom quarters to the system.

      >[!IMPORTANT]
      >
      > If your company purchased [!DNL Workfront Planning], you cannot save your custom quarters if there are gaps or overlaps between the quarters. 
      >![Custom quarters with overlap warning](assets/custom-quarters-with-overlap-warning.png)
      >Gaps and overlaps between the quarters are allowed for [!DNL Workfront] only customers. 

1. (Optional and conditional) If your company purchased only [!DNL Workfront], without [!DNL Workfront Planning], create a reporting element that refers to the fiscal quarters.

   **Example:** Create a filter for a [!UICONTROL project] list and include the Planned Completion Date of a project referencing the custom quarters.

   ![Project filter with custom quarters](assets/example-of-project-filter-with-custom-quarters.png)

   The references to "This Quarter", "Next Quarter", and "Last Quarter" are replaced with new references to the custom quarters.

   For information about reporting elements, see [Reporting elements: filters, views, and groupings](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

   For information about creating filters, see [Create or edit filters in [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
1. (Optional and conditional) If your company purchased Workfront Planning and you have access to [!DNL Workfront Planning], go to a record type page and open a timeline view. The view displays the new custom quarters. 
For information, see [Manage the timeline view](/help/quicksilver/planning/views/manage-the-timeline-view.md). 

</div>
-->