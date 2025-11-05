---
product-area: projects
navigation-topic: manage-issues
title: 修改清單中多個問題的使用者指派
description: 修改清單中多個問題的使用者指派
author: Lisa
feature: Work Management
exl-id: e1e75027-1847-44cf-afeb-b19394dc3ea5
source-git-commit: ac24b2486b9fc5a0b8c2944a6ec240140238b908
workflow-type: tm+mt
source-wordcount: '968'
ht-degree: 1%

---

# 修改清單中多個問題的使用者指派

<!--Audited: 07/2024-->
<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: similar article exists for tasks)</p>
-->

<div class="preview">

本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在預覽環境中可供所有客戶使用。 從預覽版開始的一週起，生產環境中也將提供相同功能給所有客戶。

如需詳細資訊，請參閱[介面現代化](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md)。

</div>

您可以同時修改多個問題的使用者指派。 如需有關編輯問題或一次指派一個問題的資訊，另請參閱下列文章：

* [編輯問題](../../../manage-work/issues/manage-issues/edit-issues.md)
* [指派問題](../../../manage-work/issues/manage-issues/assign-issues.md)

如需指派問題的一般資訊，請參閱[修改問題指派的概觀](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md)。

>[!NOTE]
>
>您必須至少擁有問題的「貢獻者」許可權，才能為問題指派作業。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td> <p>標準</p>
   <p>要求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td> <p>編輯問題的存取權</p> <p>檢視專案和任務的或更高存取權以指派一個問題</p> </td> 
  </tr> 
  <tr> 
   <td>物件許可權</td> 
   <td> <p>管理問題的許可權</p> <p>指派多個問題時，為問題所在的專案或任務貢獻許可權或以上。</p>  </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>When to modify user assignments on issues</h2>
<p>(NOTE:  drafted and moved to the overview article: Modify issue assignments overview)</p>
<p>You might want to modify the user assignments for multiple issues for a variety of  reasons, including the following:</p>
<ul>
<li>Users join or leave  your team</li>
<li>A user takes a vacation that extends beyond the issue  due dates</li>
<li>A specific role or user is set as the assignee for multiple issues and you want to quickly modify all items to be assigned to a different user or role</li>
</ul>
</div>
-->

## 修改多個問題的指派

1. 前往問題清單，其中包含您要修改其指派的問題。
1. （選用）建立篩選器，只顯示指派給您要修改之受指派人的問題。

   例如，您可以建立篩選器，以僅顯示與作為受託人的特定角色有關的問題。  然後，您可以使用特定使用者來取代角色。 請執行下列動作：

   1. 按一下&#x200B;**篩選器**&#x200B;下拉式清單，然後按一下&#x200B;**新增篩選器**。

   1. 在第一個欄位中，開始輸入&#x200B;**指派角色**，然後從清單中選擇&#x200B;**指派角色：名稱**。
   1. 從修飾元下拉式功能表中選取&#x200B;**是**&#x200B;的任一項，然後開始輸入角色的名稱，並在角色顯示在清單中時選取角色。 您可以輸入多個角色。

      >[!TIP]
      >
      >請勿使用&#x200B;**指派給**，因為此欄位僅參考問題擁有者，而非所有受指派人。

      問題清單會自動根據您的篩選條件進行篩選。
   1. （選擇性）按一下&#x200B;**另存新檔**，然後按&#x200B;**儲存**。

1. 選取您要修改指派的問題，然後按一下&#x200B;**編輯**&#x200B;圖示![編輯圖示](assets/qs-edit-icon.png)。

   **編輯問題**&#x200B;隨即顯示。 所選的專案數會顯示在頁面的左上角。

1. （視條件而定）在生產環境中，執行下列作業：

   1. 移至&#x200B;**工作分派**&#x200B;區段，然後選取&#x200B;**受指派人**。

      ![工作分派區域](assets/classic-assignmens-area-on-edit-box-350x119.png)

   1. 執行下列其中一項：

      1. 若要新增受指派人：

         1. 開始輸入使用者、角色或團隊的名稱，然後在其顯示在清單中時選取它。 指派已新增，不會取代所選問題上的目前指派。

         >[!TIP]
         >
         >您可以指派多個使用者、工作角色或團隊。 您只能指派作用中的使用者、工作角色和團隊。
         >
         >如果使用者、工作角色或團隊在停用之前已被指派，則他們仍被指派給工作專案。 在此情況下，我們建議採取下列步驟：
         >
         >* 將工作專案重新指派給作用中的資源。
         >* 將已停用團隊中的使用者與作用中團隊建立關聯，並將工作專案重新指派給作用中團隊。

         所有選定問題的共同資訊隨即顯示。 例如，如果將同一個使用者指派給所有問題，則該使用者會顯示在&#x200B;**受託人**&#x200B;欄中。 如果所選問題的資訊不常見，則不會顯示任何資訊。

      1. 若要移除個別受指派人，請執行下列動作：

         1. 如果受指派人顯示在「工作總攬」清單中，則按一下您要移除之受指派人名稱旁的&#x200B;**X圖示**。

            或

            如果您要移除的被指定者未顯示在「工作總攬」區段中，因為被指定者僅被指定給您選取的某些問題，請按一下&#x200B;**移除被指定者**&#x200B;並開始輸入您要移除的被指定者名稱，然後在其出現在下拉式清單中時按一下該名稱。

         1. 再按一下&#x200B;**移除被指定者**&#x200B;以新增另一個要移除的被指定者。

      1. 若要移除所有現有的被指定者：

         1. 按一下&#x200B;**移除所有現有的受指派人**，然後按一下&#x200B;**是，刪除所有受指派人**。

            這不僅會移除常見的受指派人（顯示在「編輯」對話方塊中的受指派人），也會移除所有選定問題中的所有受指派人。

         1. （選擇性）針對您選取要與問題關聯的受指派人，修改下列任一選項：

            * **問題擁有者：**&#x200B;選取選項按鈕，以指出已將哪個受指派人指定為問題擁有者。 如果保持未選取，Adobe Workfront會將第一個受指派人指定為問題所有者。 這不適用於團隊指派。
            * **受指派人的角色**：從下拉式清單中選取一個角色。 如果保持未選取，Workfront會自動選取使用者的主要角色。

      1. 按一下「**儲存變更**」。

1. <span class="preview">在預覽環境中，執行下列動作：</span>

   1. <span class="preview">按一下左側面板中的&#x200B;**工作**，然後按一下您要移除的工作負責人旁的&#x200B;**x**&#x200B;圖示。</span>

      >[!TIP]
      >
      ><span class="preview">只有指派給所有選定問題的受指派人才會顯示在&#x200B;**指派**&#x200B;區域中。</span>

      ![大量編輯問題中的指派區域](assets/assignments-area-on-bulk-edit-issues.png)

   1. <span class="preview">開始輸入使用者、角色或團隊的名稱，以將受指派人新增至所有選取的問題。</span>

      >[!TIP]
      >
      >您可以指派多個使用者、工作角色或團隊。 您只能指派作用中的使用者、工作角色和團隊。
      >
      >如果使用者、工作角色或團隊在停用之前已被指派，則他們仍被指派給工作專案。 在此情況下，我們建議採取下列步驟：
      >
      >* 將工作專案重新指派給作用中的資源。
      >* 將已停用團隊中的使用者與作用中團隊建立關聯，並將工作專案重新指派給作用中團隊。

      <span class="preview">新增的受指派人已新增至現有受指派人。 它們不會取代每個所選問題的現有問題。</span>
   1. <span class="preview">（選擇性）按一下&#x200B;**指派給我**&#x200B;以指派所有問題給您自己。</span>
   1. <span class="preview">按一下&#x200B;**儲存**。</span>




