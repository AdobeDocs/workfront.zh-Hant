---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 在工作負載平衡器顯示專案和方案的角色分配
description: 在連線專案和方案後，您可以並排管理其資源配置，以確保它們
author: Alina
feature: Workfront Scenario Planner
exl-id: cdc3a1b0-7021-4853-9b51-c3682fd55430
source-git-commit: aa2e9a012a60ab10e2d027dedae520b5e06686c7
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

# 顯示[!UICONTROL 工作負載平衡器]中專案和行動方案的角色分配

<!--Audited: 07/2024-->

在連線專案和方案後，您可以並排管理其資源配置以確保它們相符。 這可避免過度配置或利用不足。

本文說明如何使用專案的[!UICONTROL 工作負載平衡器]中的[!UICONTROL 角色配置]面板來調解資源。

如需有關協調專案與方案之間資源的一般資訊，包括先決條件，請參閱[協調專案與方案之間資源配置的概述](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 封裝</p> </td> 
   <td> 
   <p>Workfront Ultimate</p>
<p><b>附註</b></p>
<p>如果您有不同的Workfront套件，請洽詢您的Workfront代表。</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 授權</p> </td> 
   <td> <p>[!UICONTROL Light]或更高</p> 
   <p>[!UICONTROL Review]或更高版本</p> </td> 
  </tr> 
    <tr> 
   <td>存取層級設定</td> 
   <td> <p>檢視或更高的專案存取權。</p></td> 
  </tr> 
  <tr> 
   <td> <p>物件許可權 </p> </td> 
   <td> <p> 檢視專案或更高許可權。</p></td> 
  </tr> 
 </tbody> 
</table>

如需有關存取Scenario Planner的詳細資訊，請參閱[使用 [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md)所需的存取。

如需Workfront存取需求的相關資訊，請參閱[Workfront檔案的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <ul></li>
   <li><p>New: Ultimate </p></li>
   <p>The Scenario Planner is not available for the new Workfront Select or Workfront Prime plans. </p>
   <li><p>Current: [!UICONTROL Business] or higher</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td> <p>New: Light or higher</p> 
   <p>Current: [!UICONTROL Review] or higher</p> </td> 
  </tr> 
  <tr> 
   <td>Product* </td> 
   <td> <ul><li><p>For the new Workfront plans:</p><p> Adobe Workfront</li></p>
   <li><p>For the current Workfront plans: </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront Scenario Planner</p></li></ul>
   
   <p>For more information, see <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level </td> 
   <td> <p>View or higher access to Projects.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p> View or higher permission to a project.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 顯示[!UICONTROL 工作負載平衡器]中專案和行動方案的角色分配

如果您的公司已購買[!DNL Workfront Scenario Planner]授權，您可以在專案層級[!UICONTROL 工作負載平衡器]中協調方案與連結至該方案的專案之間的資源配置。

1. （視條件而定）使用下列文章所述的方法之一，將專案與行動方案連線：

   * [將專案匯入 [!DNL Adobe Workfront Scenario Planner]](import-projects-to-plans.md)中的計畫。
   * [在 [!DNL Adobe Workfront Scenario Planner]](publish-scenarios-update-projects.md)中發佈行動方案以更新或建立專案。

   >[!IMPORTANT]
   >
   >如果您對方案上的資源進行變更，則必須重新發佈方案所屬的情境，才能從方案取得最新的資源資訊以更新專案。

1. 移至您要檢視專案以及相關方案之工作角色配置的專案。
1. 按一下左側面板中的[!UICONTROL 工作負載平衡器]。

   您可能需要按一下&#x200B;**[!UICONTROL 排程]**，然後&#x200B;**[!UICONTROL 切換到工作負載平衡器]**。

1. 執行下列其中一項：

   * 按一下&#x200B;**[!UICONTROL 月]**&#x200B;以依月檢視工作負載平衡器，按一下時間表![月](assets/drop-down-next-to-month-month-view-wb.png)旁的下拉式清單中月份旁的下拉式功能表，然後按一下&#x200B;**[!UICONTROL 更多]**。
   * 按一下工具列右上角的&#x200B;**[!UICONTROL 顯示角色配置]**&#x200B;圖示![顯示角色配置](assets/show-role-allocation-icon.png)。

   [!UICONTROL 角色配置]面板隨即顯示。

   ![角色配置面板](assets/role-allocation-panel-months-collapsed-350x319.png)

   >[!CAUTION]
   >
   >雖然即使您的組織未購買[!UICONTROL 授權，您仍可檢視]角色配置[!DNL Workfront Scenario Planner]面板，但您無法檢視行動方案工作角色的資訊。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this step stays 5 to match the mention of it in the section below)</p>
   -->

1. 檢閱角色配置面板的&#x200B;**[!UICONTROL 專案總計]**&#x200B;區域中的下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 工作角色]</td> 
      <td> <p>與下列任一專案關聯的工作角色名稱：</p> 
       <ul> 
        <li> <p>專案任務</p> </li> 
        <li> <p>專案問題</p> </li> 
        <li> <p>連結至專案的方案</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 方案時數]</td> 
      <td>在方案總期間內，與方案上每個工作角色相關聯的所需時數。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 計畫時數]</td> 
      <td>在專案總期間中，與專案上任務或問題中的每個工作角色關聯的計畫時數。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 變數]</td> 
      <td> <p>方案所需時數與專案工作相關計畫時數之間的差異。 [!DNL Workfront]使用此公式計算[!UICONTROL 變異數]：</p> <p><code>Role Allocation Variance = Initiative Hours - Planned Hours</code> </p> <p>當計畫資源的時數超過方案所需的時，該[!UICONTROL 差異]為負數且以紅色顯示。 這表示您的資源配置過度。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >專案的計畫時數未顯示在下列案例中：
   >
   >   
   >   
   >   * 當任務或問題未指派給工作角色時，或具有與其關聯的工作角色的使用者時。
   >   * 當任務或問題的[!UICONTROL 持續時間]為零時。
   >   
   >

1. （選擇性）如果[!UICONTROL Variance]欄顯示您的資源過度配置，請調整下列其中一項：

   * 針對顯示過度配置的一個工作角色，降低其計畫時數或新增更多資源至任務，並將更多計畫時數分配至新資源。 您可以在編輯任務或問題時更新指派或計畫時數。 如需詳細資訊，請參閱下列文章：

      * [編輯任務](../manage-work/tasks/manage-tasks/edit-tasks.md)
      * [編輯問題](../manage-work/issues/manage-issues/edit-issues.md)

     >[!NOTE]
     >
     >您必須有其他存取權和許可權才能編輯任務和問題。

   * 針對在方案上顯示過度配置的角色，增加所需時數。 如需詳細資訊，請參閱[在 [!DNL Adobe Workfront Scenario Planner]](create-and-edit-initiatives.md)中建立和編輯方案。

     >[!NOTE]
     >
     >您必須擁有其他存取權和許可權才能編輯計畫。

1. （選擇性）按一下下拉式圖示，以展開[!UICONTROL 角色配置]面板或[!UICONTROL 工作負載平衡器]的時間軸中的其中一個月。

   ![在角色配置面板中展開月份](assets/month-expanded-highlighted-role-allocation-panel-wb-350x145.png)

   每個月也會顯示[!UICONTROL 專案總計]區域中顯示的相同資訊型別。

   >[!TIP]
   >
   >[!UICONTROL 角色配置]面板中列出的月份是[!UICONTROL 工作負載平衡器]中熒幕上顯示的時間軸中的月份。 在時間軸上前後捲動以檢視其他月份。

   <!--
   <li value="8" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p> </p> </li>
   -->


