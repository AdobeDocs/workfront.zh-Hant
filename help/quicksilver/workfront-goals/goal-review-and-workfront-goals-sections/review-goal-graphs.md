---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: 檢閱圖表以了解Adobe Workfront目標中的目標進度趨勢
description: 您可以在Adobe Workfront目標的「圖表」區段中，檢視目標的整體運作狀況及其進度趨勢。 本節中的圖表不會劃分每個目標的進度，而是提供所有目標進度狀態及其在指定期間內進度趨勢的整體快照。
author: Alina
feature: Workfront Goals
exl-id: 8d5f3617-c7bf-44ce-99b0-d4ebda106f25
source-git-commit: 3989903687f2ea64ebd5ad754119ce1a9d70b9f3
workflow-type: tm+mt
source-wordcount: '951'
ht-degree: 0%

---

# 檢閱圖表以了解Adobe Workfront目標中的目標進度趨勢

<!-- drafted mostly for P&P release-->

您可以在Adobe Workfront目標的「圖表」區段中，檢視目標的整體運作狀況及其進度趨勢。 本節中的圖表不會劃分每個目標的進度，而是提供所有目標進度狀態及其在指定期間內進度趨勢的整體快照。

>[!IMPORTANT]
>
>您可以在「圖表」區段中查看所選時段內目標的總計。 不過，在計算整體目標進度狀態和完成百分比時，Workfront目標僅考慮狀態為「作用中」和「已關閉」的目標。

## 存取需求

<!--drafted for P&P release: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront plan*</td>
   <td>
   <p>Current plan: Select or higher</p>
   Or
   <p>Legacy plan: Pro or higher</p>
   
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license*</td>
   <td>
   <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Product</td>
   <td>
   <p> Current product requirement: If you have the Select or Prime Adobe Workfront plan, you must also buy an additional Adobe Workfront Goals license.  Workfront Goals are included in the Ultimate Workfront Plan.</p>
   Or
   <p>Legacy product requirement: You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Edit access to Goals</p> <p><b>NOTE</b><p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p>
     <ul>
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li>
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li>
     </ul> </p> </td>
  </tr>
  <tr data-mc-conditions="">
   <td role="rowheader">Object permissions</td>
   <td>
    <div>
     <p>View or higher permissions to the goal to view it</p>
     <p>Manage permissions to the goal to edit it</p>
     <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
    </div> </td>
  </tr>
 </tbody>
</table>

-->

您必須具備下列存取權，才能執行本文所述的動作：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>Pro或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>要求或更高版本</p> <p>如需詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront授權概觀</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td> <p>您必須購買額外的Adobe Workfront目標授權才能存取本文所述的功能。 </p> <p>如需詳細資訊，請參閱 <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">使用Workfront目標的需求</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級*</td> 
   <td> <p>檢視或更高程度地存取目標</p> <p><b>附註</b><p>如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱：</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">授予Adobe Workfront目標的存取權</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">物件權限</td> 
   <td> 
    <div> 
     <p>檢視目標的或更高權限</p> 
     <p>如需共用目標的相關資訊，請參閱 <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">在Workfront目標中共用目標</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

您必須具備下列條件，才能開始：

* 一種佈局模板，在主菜單中包括目標區域。

## Workfront目標中的圖表類型

以下圖表可在「圖表」區段或Workfront目標中使用：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">目標運行狀況圖</td> 
   <td> <p>量規圖顯示下列內容：</p> 
    <ul> 
     <li>所選時段的目標總數。 任何狀態的目標都會納入考量。 </li> 
     <li>狀態為「活動」和「已關閉」的目標的進度狀態。</li> 
    </ul> <p>如需Workfront Target如何計算進度狀態的相關資訊，請參閱 <a href="../../workfront-goals/goal-management/calculate-goal-progress.md" class="MCXref xref">Adobe Workfront目標中的目標進度和條件概覽</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">目標進度圖</td> 
   <td> <p>折線圖，在目標期間以每週增量顯示目標的更新。 目標進度圖顯示以下內容：</p> 
    <ul> 
     <li>在所選期間內所有活動和已結束目標的平均預期和實際完成百分比。 完成百分比會細分為以節點標示的每週增量。 </li> 
     <li>自前一週以來，活動和已結束目標的總體平均進度百分比。 </li> 
    </ul> <p>提示：在所選時段之外對目標進行更新時，目標進度圖可能不顯示任何資訊。 </p> </td> 
  </tr> 
 </tbody> 
</table>

## 查看圖表中的目標進度

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) > **目標** 在右上角。

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   這會開啟Workfront目標區域。

1. 按一下 **圖表** 中。

   ![](assets/graphs-in-left-panel.png)

   圖表區段隨即顯示。

   依預設，「圖表」區段中顯示的目標會受下列條件限制：

   * 套用至「圖形」區域的篩選器。
   * 處於「活動」和「草稿」狀態的目標。

1. （可選）更新「圖形」區段右上角的篩選器，以選取您要顯示的資訊類型。

   如需篩選目標的詳細資訊，請參閱 [篩選Adobe Workfront目標中的資訊](../../workfront-goals/goal-management/filter-information-wf-goals.md).

   >[!TIP]
   如果您選取顯示多個時段，則會針對每個時段顯示健康圖（量規）和進度圖（線）。

1. 查看「目標運行狀況圖」時，請查看下表中的資訊。

   ![](assets/gauge-graph-wf-align-350x230.png)

   | 目標總數 | 圖表底部的數字表示所選期間內所有目標的數量，顯示在您選擇的所有狀態中。 |
   |---|---|
   | 平均完成百分比 | 在圖表頂端，此數字代表所選時段內作用中和結束目標的平均完成百分比。 |
   | 目標及其進展 | 將滑鼠指標暫留在圖表的區段上時，每個進度狀態區段的目標數量。 只有處於「作用中」或「已關閉」狀態的目標才會計入區段。 |


1. 查看目標進度表時，請查看下表中的資訊。

   ![](assets/line-graph-wf-align-350x161.png)

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>基線進度</td> 
      <td>綠色斜率線表示所選時段內活動和關閉目標的預期整體完成百分比平均值。 預期一個期間內的所有目標都將完成，因此，基線進展在該期間結束時總是100%。 </td> 
     </tr> 
     <tr> 
      <td>實際進度</td> 
      <td> <p>藍線以每週增量表示所選時段內活動和關閉目標的實際整體完成百分比平均值。 目標期間的每週都會由行中的節點標示。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 將滑鼠指標暫留在目標進度圖中，並檢閱下列項目：

   * **週日期**:所選周的月、日和年。
   * **進度**:所選周內所有目標的實際完成百分比的平均值。
   * **基線**:所選周內所有目標的預期完成百分比的平均值。

1. （選用）按一下 **進度** 在進度圖底部，刪除實際的總體進度線

   或

   按一下 **基線** 在進度圖底部，從圖表中刪除預期的進度。

 
