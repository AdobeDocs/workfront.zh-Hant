---
product-previous: workfront-goals
navigation-topic: goal-management
title: 在Adobe Workfront目標中篩選資訊
description: 您可以檢視自己或其他任何新增至Adobe Workfront目標的目標。 如需建立目標的相關資訊，請參閱在Adobe Workfront目標中建立目標。 檢視目標時，您可以篩選Workfront目標中的資訊，以僅檢視對您重要的目標。
author: Alina
feature: Workfront Goals
exl-id: ec9b6789-fffe-425c-8316-eefe670ad0d6
source-git-commit: 4e1558b47f6041501aa4e4fbfa6317dec8aee571
workflow-type: tm+mt
source-wordcount: '1358'
ht-degree: 2%

---

# 在Adobe Workfront目標中篩選資訊

<!--Audited for P&P only: 4/2025-->

您可以檢視自己或其他任何新增至Adobe Workfront目標的目標。 如需建立目標的相關資訊，請參閱[在Adobe Workfront目標中建立目標](../../workfront-goals/goal-management/create-goals.md)。 檢視目標時，您可以篩選Workfront目標中的資訊，以僅檢視對您重要的目標。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具備下列條件：

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> 
   <p>對於新計畫和授權結構：
  <ul><li>Ultimate計畫 </li></ul>
   </p>
<p>對於目前的計畫與授權結構： 
<ul><li> A Pro或更高版本 </li>
  <li>除了Adobe Workfront授權之外，還有Workfront目標授權。</li></ul></p>
   </td>  
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront授權*</td>
 <td>
 <p>新授權：投稿人或以上版本</p>
 或
 <p>目前授權：要求或以上</p> <p>如需詳細資訊，請參閱<a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront授權總覽</a>。</p> </td>
 </tr>
 <tr>
 <td role="rowheader">產品*</td>
 <td>
   <p> 新產品需求：Workfront</p>
  <p>或</p>
   <p>目前產品需求：除了Workfront授權之外，您必須購買Adobe Workfront Goals的授權。 </p> <p>如需詳細資訊，請參閱<a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">使用Workfront目標的需求</a>。 </p> </td>
 </tr>
 <tr>
 <td role="rowheader">存取層級</td>
 <td> <p>編輯目標的存取權</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">物件許可權</td>
 <td>
  <div>
  <p>檢視目標或更高許可權以檢視它</p>
  <p>管理目標的許可權以編輯它</p>
  <p>如需共用目標的相關資訊，請參閱<a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">在Workfront目標中共用目標</a>。 </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> <p>必須為所有使用者(包括Workfront管理員)指派一個版面配置範本，該範本包含主功能表中的「目標」區域。 </p>  
</td>
  </tr>
</tbody>
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## Workfront目標中的篩選器概觀

>[!NOTE]
>
>若要有效率地尋找並聚焦於正確的目標，我們建議您在Workfront目標中使用篩選器。 這可讓您在開始管理對您而言重要的目標之前顯示正確的資訊。 依預設，Workfront目標會顯示系統中的所有目標。

您可以在Workfront中「目標」區域的下列區段中，尋找並篩選目標：

* 目標清單
* 圖表
* 目標校準

如需有關目標區域區段的資訊，請參閱[Adobe Workfront目標區段概覽](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md)。

>[!IMPORTANT]
>
>您可以為一個區段設定篩選器，這些篩選器在移至Workfront目標的另一個區段時仍持續存在。

在Workfront目標中使用篩選器時，請考慮下列事項：

* 您可以建立並套用篩選器而不儲存它，也可以儲存篩選器以供稍後重複使用。

  存在下列情況：

   * 當您儲存篩選器時，它會在您每次登入Workfront目標時成為您的預設篩選器。
   * 當您套用篩選器而不儲存時，可以透過重新整理頁面將其還原為原始清單。

* 您只能檢視和套用您建立的篩選器。 其他使用者建立的篩選器只會顯示給這些使用者。
* 您無法與其他使用者共用您建立的篩選器。

## 在Workfront目標中套用快速篩選

您可以在目標清單中使用快速篩選器，協助您僅找出對您而言重要的專案。 您無法儲存快速篩選，且這些篩選不是永久性的。 當您重新整理頁面時，Workfront會清除快速篩選的結果。

如需詳細資訊，請參閱[將快速篩選套用至清單](../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md)。

## 在Workfront目標中建立並套用篩選器

對於Workfront目標的任何區段，建立篩選器的程式都相同。

您可以從頭開始建立篩選器，或編輯其中一個內建篩選器。

1. 前往Workfront目標。

   如需有關存取Workfront目標的資訊，請參閱[在Adobe Workfront目標中存取和開啟目標](../../workfront-goals/goal-management/access-goals-in-wf-goals.md)

   預設情況下，目標清單區段顯示。

1. 按一下清單右上角的&#x200B;**篩選器**。

   ![篩選器圖示](assets/filter-icon-and-label.png)

   依預設，Workfront會套用&#x200B;**全部**&#x200B;篩選器，以顯示您系統中的所有目標。

   >[!TIP]
   >
   >您無法編輯或刪除「全部」篩選器。

1. 執行下列其中一項：

   * 按一下下列任何預先定義的篩選器，只顯示下列擁有者的目標：

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td>全部</td> 
        <td> <p>您系統中的所有目標，不論目標建立者、建立時間期限或擁有者為何。 這是預設篩選器，您無法進行編輯。 </p> <!--
          <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: what the ALL filter displays might change; right now, it displays all, regardless of status, period, owner, etc)</p>
         --> </td> 
       </tr> 
       <tr> 
        <td>個人</td> 
        <td>您擁有的目標。</td> 
       </tr> 
       <tr> 
        <td>我的團隊</td> 
        <td> <p>您的任何團隊被選為所有者的目標。 </p> <p><b>秘訣</b>

     未指派給任何團隊時，系統不會顯示任何目標。 </p> </td>
     </tr> 
       <tr> 
        <td>我的群組</td> 
        <td>選擇任何群組作為擁有者的目標。 </td> 
       </tr> 
       <tr> 
        <td>公司</td> 
        <td> <p>與您的組織相關聯的目標。 </p> <p><b>提示</b>
        <p>在Adobe Workfront目標中，「公司」篩選器會顯示您的組織被選為所有者的目標。 </p> <p>您無法使用此欄位來搜尋公司。 依預設，僅選取擁有Workfront執行個體的組織。 </p> </p> </td> 
       </tr> 
      </tbody> 
     </table>

   * 暫留在篩選器名稱上，然後按一下篩選器名稱旁的&#x200B;**編輯**&#x200B;圖示![編輯圖示](assets/edit-icon.png)，以自訂篩選器並新增使用者、團隊、群組的特定名稱或您組織的名稱，然後在篩選器出現在清單中時選取篩選器。

   * 按一下&#x200B;**新增篩選器**&#x200B;以建立新篩選器，然後從下列選項中選取以自訂新篩選器：

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
        <td> <p>在下拉式功能表中，從下列選項選取狀態：</p> 
         <ul> 
          <li> <p>作用中</p> </li> 
          <li> <p>草稿</p> </li> 
          <li> <p>非使用中</p> </li> 
          <li> <p>已關閉</p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">進度</td> 
        <td> <p>在下拉式功能表中，從下列選項選取進度： </p> 
         <ul> 
          <li> <p>陷入困境</p> </li> 
          <li> <p>有風險</p> </li> 
          <li> <p>達成目標</p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">所有者</td> 
        <td> <p>開始輸入擁有者的名稱，然後當它出現在清單中時選取它。 </p> <p>您可以輸入使用者、專案團隊、群組或組織名稱，也可以從預先定義的選項中選取。 </p> <p>下列預先定義的篩選選項一律會參照目前登入的使用者： </p> 
         <ul> 
          <li> <p><strong>我</strong>：顯示您是擁有者的目標。</p> </li> 
          <li> <p><strong>我的主團隊</strong>和<strong>我的所有團隊</strong>：顯示您的主團隊或任何團隊被指定為擁有者的目標。 </p> <p>提示：當您未指派給任何團隊時，不會顯示任何目標。 </p> </li> 
          <li> <p><strong>我的主群組</strong>和<strong>我的所有群組</strong>：顯示主群組或任何群組被指定為擁有者的目標。</p> </li> 
         </ul> </td> 
       </tr> 
      </tbody> 
     </table>

1. （選擇性）按一下篩選器方塊右下角的&#x200B;**重設**，以清除所有您已選取的欄位，並從頭開始建立篩選器。
1. （選擇性）按一下&#x200B;**套用**&#x200B;以套用篩選器而不儲存。

   篩選器在篩選器產生器的&#x200B;**未儲存**&#x200B;區域顯示為&#x200B;**新篩選器**。

   您無法重新命名未儲存的篩選器。

   當您下次登出Workfront並重新登入時，未儲存的篩選器會從目標區域移除。

   >[!TIP]
   >
   >您一次只能有一個未儲存的新篩選器。

1. 按一下[儲存]&#x200B;**&#x200B;**&#x200B;儲存篩選器以稍後使用，然後在[新增篩選器名稱]&#x200B;**欄位中新增篩選的名稱，然後按一下[完成]**&#x200B;**。**

   這會將篩選器儲存在篩選器產生器的&#x200B;**已儲存**&#x200B;區段中。 您日後可以使用此篩選器。

   上次儲存並套用的篩選器會在您下次登入Workfront時預設顯示

1. （選擇性）按一下&#x200B;**新篩選器**&#x200B;旁的&#x200B;**向左箭號**，結束篩選器產生器並返回篩選器清單。
1. （選擇性）將滑鼠停留在自訂篩選器的名稱上，按一下&#x200B;**更多**&#x200B;功能表，然後按一下&#x200B;**刪除**，再按一下&#x200B;**刪除**。 這樣會刪除篩選器，且您無法復原它。

   >[!TIP]
   >
   >您無法刪除任何預先定義的篩選器。

1. 按一下篩選產生器右上角的&#x200B;**X圖示**&#x200B;以關閉篩選產生器。

   目前套用的篩選器名稱會顯示在目標清單右上角的「篩選器」圖示右側。

   目標清單會依您的篩選條件篩選。

1. （選擇性和條件性）檢視「目標校準」區段中的目標時，如果您想要檢視篩選掉的目標，請按一下&#x200B;**顯示它們**。

   ![顯示篩選專案的連結](assets/show-them-link-on-filtered-items-goal-list-350x109.png)

   篩選器名稱的外框為黃色，表示它被忽略。

   ![篩選黃色外框](assets/filter-yellow-outline-next-to-reapply-filter-link-350x118.png)


1. （選擇性和條件性）按一下&#x200B;**重新套用篩選器**&#x200B;以套用篩選器，並忽略您在上一步中顯示的專案。


