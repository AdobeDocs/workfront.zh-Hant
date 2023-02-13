---
product-previous: workfront-goals
navigation-topic: goal-management
title: 篩選Adobe Workfront目標中的資訊
description: 您可以檢視您或Adobe Workfront目標中新增的任何其他人。 如需建立目標的相關資訊，請參閱在Adobe Workfront目標中建立目標。 檢視目標時，您可以篩選Workfront目標中的資訊，以僅檢視對您而言重要的目標。
author: Alina
feature: Workfront Goals
exl-id: ec9b6789-fffe-425c-8316-eefe670ad0d6
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '1342'
ht-degree: 2%

---

# 篩選Adobe Workfront目標中的資訊

您可以檢視您或Adobe Workfront目標中新增的任何其他人。 如需建立目標的相關資訊，請參閱 [在Adobe Workfront目標中建立目標](../../workfront-goals/goal-management/create-goals.md). 檢視目標時，您可以篩選Workfront目標中的資訊，以僅檢視對您而言重要的目標。

## 存取需求

<!--drafted - replace the table below with this one when P&P releases: 

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
   <td> <p>檢視或更高程度地存取目標</p> <p><b>附註</b>

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

## Workfront目標中的篩選器概觀

>[!NOTE]
>
>若要有效尋找並著重於正確的目標，建議您在Workfront目標中使用篩選器。 這可讓您在開始管理對您而言重要的目標之前，先顯示正確的資訊。 依預設，Workfront目標會顯示系統中的所有目標。

您可以在Workfront中「目標」區域的下列章節中找到並篩選目標：

* 目標清單
* 圖表
* 目標校準

如需「目標」區域的相關資訊，請參閱 [Adobe Workfront目標章節概覽](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md).

>[!IMPORTANT]
>
>您可以設定一個區段的篩選器，且在移至Workfront目標的其他區段時，這些篩選器會持續存在。

在Workfront目標中使用篩選器時，請考量下列事項：

* 您可以建立並套用篩選器而不儲存，也可以儲存篩選器以供稍後重複使用。

   存在下列情況：

   * 儲存篩選器時，它會成為您每次登入Workfront目標時的預設篩選器。
   * 如果您未儲存篩選器，則可重新整理頁面，回復成原始清單。

* 您只能檢視和套用您建立的篩選器。 其他使用者建立的篩選器只會針對這些使用者顯示。
* 您無法與其他使用者共用您建立的篩選器。

## 在Workfront目標中套用快速篩選

您可以在目標清單中使用快速篩選，協助您僅找出對您而言重要的項目。 您無法儲存快速篩選，且這些篩選不具持續性。 Workfront會在您重新整理頁面時清除快速篩選的結果。

如需詳細資訊，請參閱 [將快速篩選器應用於清單](../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).

## 在Workfront目標中建立和套用篩選器

針對Workfront目標的任何區段，建立篩選器的程式相同。

您可以從頭建立篩選器，或編輯其中一個內建篩選器。

1. 前往Workfront目標。

   如需存取Workfront目標的相關資訊，請參閱 [存取與Adobe Workfront目標中的開放目標](../../workfront-goals/goal-management/access-goals-in-wf-goals.md)

   依預設， 「目標清單」區段隨即顯示。

1. 按一下 **篩選** 在清單的右上角。

   ![](assets/filter-icon-and-label.png)

   依預設，Workfront會套用 **全部** 篩選器，可顯示您系統中的所有目標。

   >[!TIP]
   >
   >您無法編輯或刪除全部篩選器。

1. 執行下列任一項作業：

   * 按一下下列任何預先定義的篩選器，以僅顯示下列擁有者的目標：

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td>全部</td> 
        <td> <p>系統中的所有目標，無論是誰建立的目標、目標的時段為何，或目標擁有者是誰。 這是預設篩選器，您無法加以編輯。 </p> <!--
          <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: what the ALL filter displays might change; right now, it displays all, regardless of status, period, owner, etc)</p>
         --> </td> 
       </tr> 
       <tr> 
        <td>個人</td> 
        <td>您是其擁有者的目標。</td> 
       </tr> 
       <tr> 
        <td>我的團隊</td> 
        <td> <p>任何團隊被選為擁有者的目標。 </p> <p><b>筆尖</b>

      未指派給任何團隊時，不會顯示目標。 </p> </td>
      </tr> 
       <tr> 
        <td>我的群組</td> 
        <td>您的任何群組被選為擁有者的目標。 </td> 
       </tr> 
       <tr> 
        <td>公司</td> 
        <td> <p>與貴組織相關聯的目標。 </p> <p><b>筆尖</b>
        <p>在Adobe Workfront目標中，公司篩選器會顯示您的組織被選取為擁有者的目標。 </p> <p>您無法使用此欄位來搜尋公司。 依預設，僅會選取擁有Workfront執行個體的組織。 </p> </p> </td> 
       </tr> 
      </tbody> 
     </table>

   * 將滑鼠指標暫留在篩選器名稱上，然後按一下 **編輯** 圖示 ![](assets/edit-icon.png) 在名稱旁以自訂該名稱，並新增使用者、團隊、群組的特定名稱或您的組織名稱，然後在使用者出現在清單中時加以選取。

   * 按一下 **新增篩選** 若要建立新篩選器，請選取下列選項以自訂新篩選器：

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">期間</td> 
        <td>在下拉式功能表中選取時段。 您可以選取多個時段。 </td> 
       </tr> 
       <tr> 
        <td role="rowheader">狀態</td> 
        <td> <p>從下拉式選單中選取狀態，選項如下：</p> 
         <ul> 
          <li> <p>使用中</p> </li> 
          <li> <p>草稿</p> </li> 
          <li> <p>非使用中</p> </li> 
          <li> <p>已關閉</p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">進度</td> 
        <td> <p>從下拉式選單中選取進度，選項如下： </p> 
         <ul> 
          <li> <p>陷入困境</p> </li> 
          <li> <p>有風險</p> </li> 
          <li> <p>達成目標</p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">所有者</td> 
        <td> <p>開始鍵入所有者的名稱，然後在清單中出現時選擇該名稱。 </p> <p>您可以輸入使用者、團隊、群組的名稱或組織的名稱，或從預先定義的選項中選取。 </p> <p>下列預先定義的篩選選項一律指目前登入的使用者： </p> 
         <ul> 
          <li> <p><strong>我</strong>:顯示您是擁有者的目標。</p> </li> 
          <li> <p><strong>我的家隊</strong> 和 <strong>所有我的團隊</strong>:顯示將您的主團隊或任何團隊指定為擁有者的目標。 </p> <p>提示：未指派給任何團隊時，不會顯示目標。 </p> </li> 
          <li> <p><strong>我的家庭組</strong> 和 <strong>所有我的組</strong>:顯示將您的首頁群組或任何群組指定為擁有者的目標。</p> </li> 
         </ul> </td> 
       </tr> 
      </tbody> 
     </table>

1. （選用）按一下 **重設** 在篩選器方塊的右下角，以清除您選取的所有欄位，並從頭開始建立篩選器。
1. （選用）按一下 **套用** 來套用篩選而不儲存。

   篩選器會顯示在 **未儲存** 篩選器產生器的區域為 **新增篩選**.

   無法更名未保存的篩選器。

   下次您登出Workfront並重新登入時，未儲存的篩選器會從「目標」區域中移除。

   >[!TIP]
   >
   >一次只能有一個未儲存的新篩選器。

1. 按一下 **儲存** 若要儲存篩選器以供稍後使用，請在 **新增篩選器名稱** 欄位，按一下 **完成**.

   這會將篩選器儲存在 **已儲存** 區段。 您日後可以使用此篩選器。

   下次您重新登入Workfront時，預設會顯示上次儲存和套用的篩選器

1. （選用）按一下 **向左箭頭** 下一頁 **新增篩選** 退出篩選器產生器並返回篩選器清單。
1. （選用）將滑鼠指標暫留在自訂篩選器的名稱上，按一下 **更多** ，然後按一下 **刪除**，然後 **刪除**. 這會刪除篩選器，而您無法復原。

   >[!TIP]
   >
   >您無法刪除任何預先定義的篩選器。

1. 按一下 **X圖示** 在篩選器產生器的右上角，關閉篩選器產生器。

   目前套用的篩選器名稱會顯示在目標清單的右上角的篩選器圖示右側。

   目標清單會依您的篩選條件篩選。

1. （可選和條件性）在「目標對齊」區段中檢視目標時，按一下 **顯示** 如果您想要檢視已篩選掉的目標。

   ![](assets/show-them-link-on-filtered-items-goal-list-350x109.png)

   篩選器名稱會以黃色列出，表示正在忽略該名稱。

   ![](assets/filter-yellow-outline-next-to-reapply-filter-link-350x118.png)


1. （選用和條件式）按一下 **重新套用篩選** 以套用篩選並忽略上一步中顯示的項目。


