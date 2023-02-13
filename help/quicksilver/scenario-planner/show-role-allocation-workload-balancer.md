---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 在工作負載平衡器中顯示項目和方案的角色分配
description: 在您連結項目和方案後，您可以並排管理其資源分配，以確保它們
author: Alina
feature: Workfront Scenario Planner
exl-id: cdc3a1b0-7021-4853-9b51-c3682fd55430
source-git-commit: 82a5102d28700368a094502dcd6026462c149eb1
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 0%

---

# 顯示 [!DNL Workload Balancer]

>[!IMPORTANT]
>
>貴組織必須購買 [!DNL Adobe Workfront Scenario Planner] 以便您查看項目的計畫資訊。 如需有關取得 [!DNL Workfront Scenario Planner]，請參閱 [使用 [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

在您連結專案和方案後，您可以並排管理其資源分配，確保兩者相符。 這可避免過度分配或利用這些資源。

本文說明如何使用 [!UICONTROL 角色分配] 面板 [!UICONTROL 工作負載平衡器] 一個項目。

有關協調項目和計畫之間的資源（包括先決條件）的一般資訊，請參見 [協調項目和舉措之間資源分配的概覽](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

## 存取需求

您需要遵循：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> 計劃*</b> </p> </td> 
   <td>[!UICONTROL Business]或更高版本</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> 授權*</b> </p> </td> 
   <td> <p>[!UICONTROL Review]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td><b>產品</b> </td> 
   <td> <p>您必須為 [!DNL Adobe Workfront Scenario Planner] 存取本文所述功能。</p> <p>如需有關取得 [!DNL Workfront Scenario Planner]，請參閱 <a href="../scenario-planner/access-needed-to-use-sp.md">使用 [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>訪問級別配置*</strong> </td> 
   <td> <p>[!UICONTROL視圖]或更高的項目訪問權限 </p> <p>注意：如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可以更改您的訪問級別，請參閱 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>物件權限</strong> </p> </td> 
   <td> <p>[!UICONTROL視圖]或更高的項目權限</p> <p>有關請求對計畫進行額外訪問的資訊，請參閱 <a href="../scenario-planner/request-access-to-plan.md">[!UICONTROL要求]存取 [!DNL Workfront Scenario Planner]</a>.</p> <p>如需要求額外存取專案的詳細資訊，請參閱 <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 顯示 [!DNL Workload Balancer]

如果貴公司已購買 [!DNL Workfront Scenario Planner] 許可證，您可以在項目級中協調方案和與其連結的項目之間的資源分配 [!DNL Workload Balancer].

1. （條件性）使用下列文章所述的其中一種方法，將專案與方案連結：

   * [將專案匯入至 [!DNL Adobe Workfront Scenario Planner]](import-projects-to-plans.md).
   * [更新或建立專案，方法是在 [!DNL Adobe Workfront Scenario Planner]](publish-scenarios-update-projects.md).

   >[!IMPORTANT]
   >
   >如果對方案的資源進行更改，則必須重新發佈方案所屬的方案，以便從方案獲取最新的資源資訊以更新項目。

1. 轉至項目，在該項目中複查項目以及關聯方案的職務分配。
1. 按一下 [!DNL Workload Balancer] 中。

   您可能必須按一下 **[!UICONTROL 排程]**，然後 **[!UICONTROL 切換到工作負載平衡器]**.

1. 執行下列任一項作業：

   * 按一下 **[!UICONTROL 月]** 要按月查看工作負載平衡器，請按一下時間軸中一個月旁邊的下拉菜單 ![](assets/drop-down-next-to-month-month-view-wb.png)，然後按一下 **[!UICONTROL 更多]**.
   * 按一下 **[!UICONTROL 顯示角色分配]** 圖示 ![](assets/show-role-allocation-icon.png) 的上角。

   此 [!UICONTROL 角色分配] 面板隨即顯示。

   ![](assets/role-allocation-panel-months-collapsed-350x319.png)

   >[!CAUTION]
   >
   >雖然您可以檢視 [!UICONTROL 角色分配] 面板，即使您的組織未購買 [!DNL Workfront Scenario Planner] 許可證，則無法查看有關方案的作業角色的資訊。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this step stays 5 to match the mention of it in the section below)</p>
   -->

1. 請參閱 **[!UICONTROL 專案總計]** 「角色分配」面板的區域：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL作業角色]</td> 
      <td> <p>與以下任一項關聯的作業角色的名稱：</p> 
       <ul> 
        <li> <p>項目任務</p> </li> 
        <li> <p>專案的問題</p> </li> 
        <li> <p>與項目相關的倡議</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL計畫小時數]</td> 
      <td>在計畫的總持續時間內與計畫上每個職務相關的所需小時數。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL計畫小時數]</td> 
      <td>在項目的總持續時間內，與項目任務或問題中每個職務角色關聯的計畫小時數。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL變數]</td> 
      <td> <p>計畫所需小時數與與項目工作相關的計畫小時數之間的差異。 [!DNL Workfront] 使用以下公式計算[!UICONTROL Variance]:</p> <p><code>Role Allocation Variance = Initiative Hours - Planned Hours</code> </p> <p>當計畫資源的時間超過計畫要求的時間時，[!UICONTROL差異]為負，以紅色顯示。 這表示您的資源被過度分配。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >在下列情況中，不會顯示來自項目的計畫時數：
   >
   >   
   >   
   >   * 未將任務或問題指派給作業角色或具有與其相關聯的作業角色的使用者時。
   >   * 當任務或問題具有 [!UICONTROL 持續時間] 零。




1. （選用）若 [!UICONTROL 變異數] 欄顯示資源被過度分配，請調整以下任一項：

   * 減少顯示分配過多或向任務添加更多資源的某個任務角色的「計畫小時數」，並將更多「計畫小時數」分配給新資源。 您可以在編輯任務或問題時更新分配或計畫小時數。 如需詳細資訊，請參閱下列文章：

      * [編輯任務](../manage-work/tasks/manage-tasks/edit-tasks.md)
      * [編輯問題](../manage-work/issues/manage-issues/edit-issues.md)

      >[!NOTE]
      >
      >您必須有其他存取權和權限才能編輯工作和問題。

   * 增加顯示方案上超額分配的職責所需小時數。 如需詳細資訊，請參閱 [在 [!DNL Adobe Workfront Scenario Planner]](create-and-edit-initiatives.md).

      >[!NOTE]
      >
      >您必須有其他存取權和權限才能編輯計畫。


1. （選用）按一下下拉式圖示，以展開 [!UICONTROL 角色分配] 或 [!UICONTROL 工作負載平衡器].

   ![](assets/month-expanded-highlighted-role-allocation-panel-wb-350x145.png)

   顯示在 [!UICONTROL 專案總計] 區域也會顯示於每月。

   >[!TIP]
   >
   >列於 [!UICONTROL 角色分配] 面板是時間軸中顯示在畫面上的月份 [!UICONTROL 工作負載平衡器]. 在時間軸上向後捲動，以檢視其他月份。

   <!--
   <li value="8" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p> </p> </li>
   -->


