---
content-type: overview
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: 將專案新增至Adobe Workfront目標中的目標
description: 您可以根據專案的實際進度，將專案與目標連結，以指出目標的進度。 項目成為目標的進度指標。
author: Alina
feature: Workfront Goals
exl-id: 683c9cd9-6c7b-4d50-b326-b4000c9863e8
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '888'
ht-degree: 1%

---

# 將專案新增至Adobe Workfront目標中的目標

<!--
THIS MIGHT NEED TO BE RENAMED BECAUSE THERE WILL BE OTHER OBJECTS CONNECTED TO GOALS IN THE FUTURE
-->

您可以根據專案的實際進度，將專案與目標連結，以指出目標的進度。 項目成為目標的進度指標。

通過將項目與目標連接起來，您可以將貴組織的戰略規劃（目標）與您的人員正在執行的實際工作關聯起來，並完成每天的工作（項目）。

>[!IMPORTANT]
>
>在專案的「業務案例」區域中建立的專案層級目標與在Workfront目標中建立的策略目標無關。 有關業務案例項目目標的資訊，請參閱 [建立業務案例目標](../../manage-work/projects/define-a-business-case/create-business-case-goals.md).


## 存取需求

<!--drafted for P&P release: replace the table below with this: 

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
您必須具備下列條件：

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
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯目標的存取權</p> <p><b>附註</b>

<p>如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱：</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">授予Adobe Workfront目標的存取權</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">物件權限</td> 
   <td> 
    <div> 
     <p>管理目標的權限</p> 
     <p>如需共用目標的相關資訊，請參閱 <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">在Workfront目標中共用目標</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

如需存取Workfront目標的詳細資訊，請參閱 [使用Workfront目標的需求](../goal-management/access-needed-for-wf-goals.md).

## 關於將項目連接到目標的考慮

* 您可以將符合下列條件的專案新增至目標：

   * 您至少必須擁有「檢視」的權限。

      >[!NOTE]
      >
      >如果在將專案附加至目標後，您失去檢視專案的權限，您仍可以看到目標的專案資訊，但無法再存取專案。

   * 項目不能處於「已死」狀態。

* 您可以將多個專案與目標建立關聯。
* 您可以將相同的專案與多個目標建立關聯。
* 您無法從項目附加的目標手動更新項目的進度。 相反地，Workfront會計算專案的完成百分比，而Workfront目標則會使用此完成百分比計算目標進度。 這會在專案百分比更新後即時更新目標。
* 專案持續時間可能超出目標的時段。 如果專案持續時間超過目標的截止時間，您仍可以關閉目標並將其視為已完成，但目標完成百分比不會是100%。 專案完成百分比不再更新目標。

<!--this is no longer visible in the new redesigned interface for goals: logged a bug for this: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/63ceb049000080d30022aab9a359f6f1/updates - but confirmed that this will not be brought back at least for now - Jan 2023. 

There is an indication on the goal list that the project no longer updates progress for the goal.

  ![](assets/goal-closed-project-active-warning-goal-list-350x94.png)
-->

* 刪除附加至目標的專案時，該專案也會從目標中刪除。

   >[!CAUTION]
   >
   >如果目標在您刪除項目之前處於活動狀態，且目標上沒有其他進度指標，則目標將變為非活動狀態。


## 新增專案至目標

1. 按一下 **主菜單** ![](assets/main-menu-icon.png) (為殼層繪製此內容：或按一下 **主菜單** ![](assets/three-line-main-menu-icon.png) 在左上角，如果可用)，則 **目標**.
1. 從「目標清單」中，按一下目標名稱以開啟目標頁面。
1. 按一下 **進度指標** 中。
1. 從 **新進展指標** 下拉式功能表，按一下 **新增現有專案**.

   「新增專案至目標」方塊隨即顯示。
1. （選用）更新 **檢視**, **篩選**，或 **分組** 按一下清單右上角的個別圖示，以修改專案清單的顯示方式。
1. （選用）按一下 **搜尋** 圖示 ![](assets/search-icon.png) 然後開始鍵入項目名稱，以便快速在清單中找到它。
1. 選取您要新增至目標的專案，然後按一下 **新增**.

   選取的專案會新增至目標，且會顯示在目標頁面下方的「進度指標」區段中 **專案** 分組。

   在您啟動目標後，目標的進度會在專案進度更新時自動更新。 如需啟動目標的相關資訊，請參閱 [啟用Adobe Workfront目標中的目標](../goal-management/activate-goals.md).

## 找到目標的專案資訊

<p>
目標頁面的「進度指標」區段中的目標層級會顯示下列專案資訊：

</p>

<table>
  <tr>
   <td>專案名稱
   </td>
   <td>專案名稱中的任何變更也會反映在連線的專案中。
   </td>
  </tr>
  <tr>
   <td>專案所有者
   </td>
   <td>專案擁有者中的任何變更也會反映在連線的專案中。
   </td>
  </tr>
    <tr>
   <td>實際進度
   </td>
   <td> <p>專案的完成百分比。 您無法手動更新目標中的專案完成百分比。 Workfront會根據工作完成百分比自動計算。 </p>
   </td>
  </tr>
  <tr>
   <td>進度
   </td>
   <td>專案的完成百分比，以長條表示。 項目完成百分比的任何更改都會自動更新目標進度，除非目標已關閉。
   </td>
  </tr>

</table>

## 找出專案的目標資訊

項目清單或報表中會顯示以下目標資訊：

| 目標資訊 | 說明 |
|---|---|
| 目標 | 具有與其關聯的項目的所有目標的清單。 |
| 目標階層 | 目標所屬的階層。 此欄位中只會顯示目標和目標的父項。 子項目標不會顯示。 |
| 連結目標數 | 連結至一個專案的目標數。 |
