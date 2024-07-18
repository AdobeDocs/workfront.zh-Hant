---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 啟用專案的自訂季度
description: 若您組織的季度是根據行事曆日期以外的特定條件（例如營業日或購物日），基於報表目的，您可能會想要建立自訂季度。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 0f643d36-6235-4fd3-b6d3-54fbd03c9b33
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 0%

---

# 啟用專案的自訂季度

若您組織的季度是根據行事曆日期以外的特定條件（例如營業日或購物日），基於報表目的，您可能會想要建立自訂季度。

您最多可以為您的[!DNL Adobe Workfront]系統設定8個自訂季度。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td>[！UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是[!DNL Workfront]管理員。</p> <p><b>注意</b>：如果您仍然沒有存取權，請詢問您的[!DNL Workfront]管理員是否對您的存取層級設定了其他限制。 如需[!DNL Workfront]管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 為您的[!DNL Workfront]系統設定自訂季度

1. 按一下[!DNL Adobe Workfront]右上角的&#x200B;**[!UICONTROL 主要功能表]**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下&#x200B;**[!UICONTROL 設定]** ![](assets/gear-icon-settings.png)。

1. 按一下&#x200B;**[!UICONTROL 專案偏好設定]** > **[!UICONTROL 專案]。**

1. 在&#x200B;**[!UICONTROL 時間表]**&#x200B;區段中，選取&#x200B;**[!UICONTROL 啟用自訂季度]**。

1. 輸入自訂季度的名稱，例如「2021年第一財政年度」。
1. 選取自訂季度的開始和結束日期。

   ![](assets/custom-quarters-nwe.png)

1. （選擇性）按一下&#x200B;**[!UICONTROL 新增自訂季度]**&#x200B;以新增其他自訂季度至系統。
1. （選擇性）建立參考會計季的報表元素。

   **範例：**&#x200B;為[!UICONTROL 專案]清單建立篩選器，並包含參考自訂季度的專案計畫完成日期。

   ![](assets/example-of-project-filter-with-custom-quarters.png)

   「本季」、「下一季」和「上一季」的參考資料會取代為自訂季度的新參考資料。

   如需有關報告元素的資訊，請參閱[報告元素：篩選器、檢視和群組](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)。

   如需建立篩選的詳細資訊，請參閱[在 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)中建立或編輯篩選。
