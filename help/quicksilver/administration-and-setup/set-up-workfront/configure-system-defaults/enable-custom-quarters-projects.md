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
source-git-commit: 20ebcb74c79aea67ea7cb1ba083dfea623fe7c16
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 0%

---

# 啟用自訂季度

<!--Audited: 11/2024-->

若您組織的季度是根據行事曆日期以外的特定條件（例如營業日或購物日），基於報表目的，您可能會想要建立自訂季度。

根據貴公司已購買的產品，您可以在Workfront設定區域中設定下列季度數：

* 僅購買[!DNL Workfront]的客戶，最多可以為其[!DNL Adobe Workfront]系統設定8個自訂季度。
* 購買[!DNL Workfront]和[!DNL Workfront Planning]的客戶可以為其[!DNL Workfront]系統設定最多100個季度，這些季度也可在[!DNL Planning]中使用。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

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
   <td><p>[！UICONTROL標準]</p>
       <p>[！UICONTROL計畫]</p></td>
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td>[！UICONTROL系統管理員]</td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 為您的[!DNL Workfront]系統設定自訂季度

{{step-1-to-setup}}

1. 按一下&#x200B;**[!UICONTROL 專案偏好設定]** > **[!UICONTROL 專案]。**

1. 在&#x200B;**[!UICONTROL 時間表]**&#x200B;區段中，選取&#x200B;**[!UICONTROL 啟用自訂季度]**。

1. 輸入自訂季度的名稱，例如「2021年第一財政年度」。
1. 選取自訂季度的開始和結束日期。

   ![自訂季度](assets/custom-quarters-nwe.png)

1. （選擇性）按一下&#x200B;**[!UICONTROL 新增自訂季度]**&#x200B;以新增其他自訂季度至系統。

   >[!IMPORTANT]
   >
   > 如果貴公司已購買[!DNL Workfront Planning]，如果季度之間存在間隔或重疊，則您無法儲存自訂季度。
   >![含有重疊警告的自訂季度](assets/custom-quarters-with-overlap-warning.png)
   >只有[!DNL Workfront]個客戶才允許季之間的間隔和重疊。

1. （選擇性和條件性）如果貴公司只購買了[!DNL Workfront]，而沒有購買[!DNL Workfront Planning]，請建立參考會計季的報表元素。


   **範例：**&#x200B;為[!UICONTROL 專案]清單建立篩選器，並包含參考自訂季度的專案計畫完成日期。

   ![包含自訂季數的專案篩選器](assets/example-of-project-filter-with-custom-quarters.png)

   「本季」、「下一季」和「上一季」的參考資料會取代為自訂季度的新參考資料。

   如需有關報告元素的資訊，請參閱[報告元素：篩選器、檢視和群組](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)。

   如需建立篩選的詳細資訊，請參閱[在 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)中建立或編輯篩選。
1. （選擇性和條件性）如果您可以存取[!DNL Workfront Planning]，請移至記錄型別頁面並開啟時間表檢視。 檢視會顯示新的自訂季度。
如需詳細資訊，請參閱[管理時間表檢視](/help/quicksilver/planning/views/manage-the-timeline-view.md)。
