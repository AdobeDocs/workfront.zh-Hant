---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 啟用項目的自定義季數
description: 為了報告目的，如果組織的季度基於日曆日期以外的特定標準（如工作天或購物天），則您可能希望建立自定義季度。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 0f643d36-6235-4fd3-b6d3-54fbd03c9b33
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 0%

---

# 啟用項目的自定義季數

為了報告目的，如果組織的季度基於日曆日期以外的特定標準（如工作天或購物天），則您可能希望建立自定義季度。

您可以為 [!DNL Adobe Workfront] 系統。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td>[!UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置</td> 
   <td> <p>您必須是 [!DNL Workfront] 管理員。</p> <p><b>注意</b>:如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 為 [!DNL Workfront] 系統

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 按一下 **[!UICONTROL 專案偏好設定]** > **[!UICONTROL 專案].**

1. 在 **[!UICONTROL 時間軸]** 部分，選擇 **[!UICONTROL 啟用自定義季度]**.

1. 輸入自訂季度的名稱，例如「2021財政季度1」。
1. 選擇自定義季度的開始和結束日期。

   ![](assets/custom-quarters-nwe.png)

1. （選用）按一下 **[!UICONTROL 新增自訂季度]** 向系統添加其他自定義季度。
1. （可選）建立引用會計季度的報告元素。

   **範例：** 為 [!UICONTROL 專案] 列出並包括引用自定義季度的項目的計畫完成日期。

   ![](assets/example-of-project-filter-with-custom-quarters.png)

   對「本季度」、「下一季度」和「上一季度」的引用將替換為對自定義季度的新引用。

   如需報表元素的相關資訊，請參閱 [報表元素：篩選器、檢視和群組](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

   如需建立篩選器的相關資訊，請參閱 [在中建立或編輯篩選器 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
