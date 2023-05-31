---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 在工作負載平衡器中顯示專案和方案的角色分配
description: 在連線專案和方案後，您可以並排管理其資源配置，以確保它們
author: Alina
feature: Workfront Scenario Planner
exl-id: cdc3a1b0-7021-4853-9b51-c3682fd55430
source-git-commit: 9c0160dc5e43f36b65d9f2d4a3498a9c5f39f6f1
workflow-type: tm+mt
source-wordcount: '877'
ht-degree: 0%

---

# 在中顯示專案和方案的角色分配 [!UICONTROL 工作負載平衡器]

>[!IMPORTANT]
>
>您的組織必須購買額外的授權 [!DNL Adobe Workfront Scenario Planner] 以便您檢視專案的方案資訊。 如需關於取得 [!DNL Workfront Scenario Planner]，請參閱 [使用所需的存取權 [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

連線專案和方案後，您可以並排管理其資源配置，以確保它們相符。 這樣可避免過度配置或利用不足。

本文說明如何使用 [!UICONTROL 角色分配] 面板於 [!UICONTROL 工作負載平衡器] 專案的。

如需有關協調專案與方案之間資源的一般資訊，包括先決條件，請參閱 [協調專案與方案之間的資源配置概要](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

## 存取需求

您需要遵循下列步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> 計劃*</b> </p> </td> 
   <td>[！UICONTROL Business]或更高版本</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> 授權*</b> </p> </td> 
   <td> <p>[！UICONTROL Review]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td><b>產品</b> </td> 
   <td> <p>您必須為以下專案購買額外的授權： [!DNL Adobe Workfront Scenario Planner] 以存取本文所述的功能。</p> <p>如需關於取得 [!DNL Workfront Scenario Planner]，請參閱 <a href="../scenario-planner/access-needed-to-use-sp.md">使用所需的存取權 [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>存取層級設定*</strong> </td> 
   <td> <p>[！UICONTROL檢視]或更高的專案存取權 </p> <p>注意：如果您仍然沒有存取權，請詢問您的 [!DNL Workfront] 管理員是否對您的存取層級設定其他限制。 如需如何進行 [!DNL Workfront] 管理員可以變更您的存取層級，請參閱 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>物件許可權</strong> </p> </td> 
   <td> <p>[！UICONTROL檢視]或更高的專案許可權</p> <p>如需請求對計畫的額外存取許可權的詳細資訊，請參閱 <a href="../scenario-planner/request-access-to-plan.md">[！UICONTROL Request]存取中的計畫 [!DNL Workfront Scenario Planner]</a>.</p> <p>如需請求專案其他存取許可權的相關資訊，請參閱 <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有哪些計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 在中顯示專案和方案的角色分配 [!UICONTROL 工作負載平衡器]

如果您的公司已購買 [!DNL Workfront Scenario Planner] 授權，您可以在專案層級協調方案與連結至方案的專案之間的資源配置 [!UICONTROL 工作負載平衡器].

1. （視條件而定）使用下列文章中說明的方法之一，將專案與行動方案連線：

   * [將專案匯入至中的計畫 [!DNL Adobe Workfront Scenario Planner]](import-projects-to-plans.md).
   * [透過發佈中的方案來更新或建立專案 [!DNL Adobe Workfront Scenario Planner]](publish-scenarios-update-projects.md).

   >[!IMPORTANT]
   >
   >如果您對方案上的資源進行變更，則必須重新發佈方案所屬的情境，以便從方案取得最新的資源資訊以在專案上更新。

1. 前往您要檢閱專案和相關方案之職務角色配置的專案。
1. 按一下 [!UICONTROL 工作負載平衡器] 在左側面板中。

   您可能需要按一下 **[!UICONTROL 排程]**，則 **[!UICONTROL 切換至工作負載平衡器]**.

1. 執行下列任一項作業：

   * 按一下 **[!UICONTROL 月]** 若要按月檢視工作負載平衡器，請按一下時間軸中一個月旁的下拉式功能表 ![](assets/drop-down-next-to-month-month-view-wb.png)，然後按一下 **[!UICONTROL 更多]**.
   * 按一下 **[!UICONTROL 顯示角色分配]** 圖示 ![](assets/show-role-allocation-icon.png) 工具列的右上角。

   此 [!UICONTROL 角色分配] 面板顯示。

   ![](assets/role-allocation-panel-months-collapsed-350x319.png)

   >[!CAUTION]
   >
   >雖然您可以檢視 [!UICONTROL 角色分配] 即使貴組織未購買 [!DNL Workfront Scenario Planner] 授權，您無法檢視關於行動方案工作角色的資訊。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this step stays 5 to match the mention of it in the section below)</p>
   -->

1. 檢閱下列資訊： **[!UICONTROL 專案總計]** 「角色配置」面板的區域：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL工作角色]</td> 
      <td> <p>與下列任一專案關聯的工作角色名稱：</p> 
       <ul> 
        <li> <p>專案任務</p> </li> 
        <li> <p>專案問題</p> </li> 
        <li> <p>連結至專案的方案</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL行動方案時數]</td> 
      <td>在方案總期間內，與方案上每個工作角色相關聯的所需時數。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL計畫時數]</td> 
      <td>在專案總期間內，專案上任務或問題中每個工作角色關聯的計畫時數。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL變異數]</td> 
      <td> <p>方案所需時數與專案工作相關計畫時數之間的差異。 [!DNL Workfront] 使用此公式計算[！UICONTROL變異數]：</p> <p><code>Role Allocation Variance = Initiative Hours - Planned Hours</code> </p> <p>當資源計畫的時數超過方案所需的時，該[！UICONTROL差異]為負數且以紅色顯示。 這表示您的資源配置過度。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >專案中的計畫時數未顯示在下列案例中：
   >
   >   
   >   
   >   * 未將任務或問題指派給工作角色時，或具有與其相關聯工作角色的使用者時。
   >   * 當任務或問題具有 [!UICONTROL 持續時間] 零。




1. （選擇性）如果 [!UICONTROL 變數] 欄顯示您的資源已過度配置，請調整下列其中一項：

   * 降低顯示過度配置之工作角色的計畫時數或新增更多資源至任務，並將更多計畫時數分配至新資源。 您可以在編輯任務或問題時，更新任務或問題的指派或計畫時數。 如需詳細資訊，請參閱下列文章：

      * [編輯任務](../manage-work/tasks/manage-tasks/edit-tasks.md)
      * [編輯問題](../manage-work/issues/manage-issues/edit-issues.md)

      >[!NOTE]
      >
      >您必須有額外的存取權和許可權才能編輯任務和問題。

   * 增加顯示方案上過度配置的角色所需時數。 如需詳細資訊，請參閱 [在中建立和編輯方案 [!DNL Adobe Workfront Scenario Planner]](create-and-edit-initiatives.md).

      >[!NOTE]
      >
      >您必須擁有其他存取權和許可權才能編輯計畫。


1. （可選）按一下下拉式圖示，以展開 [!UICONTROL 角色分配] 面板或的時間軸中 [!UICONTROL 工作負載平衡器].

   ![](assets/month-expanded-highlighted-role-allocation-panel-wb-350x145.png)

   在中顯示的相同資訊型別 [!UICONTROL 專案總計] 區域也會每月顯示。

   >[!TIP]
   >
   >中列出的月份 [!UICONTROL 角色分配] 面板是時間軸中的月份，顯示在畫面的畫面中 [!UICONTROL 工作負載平衡器]. 在時間軸上前後捲動以檢視其他月份。

   <!--
   <li value="8" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p> </p> </li>
   -->


