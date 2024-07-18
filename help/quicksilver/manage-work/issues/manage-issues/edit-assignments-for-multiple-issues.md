---
product-area: projects
navigation-topic: manage-issues
title: 修改清單中多個問題的使用者指派
description: 修改清單中多個問題的使用者指派
author: Alina
feature: Work Management
exl-id: e1e75027-1847-44cf-afeb-b19394dc3ea5
source-git-commit: daba001c28df268721c87df7d2516ffb76e535d9
workflow-type: tm+mt
source-wordcount: '773'
ht-degree: 1%

---

# 修改清單中多個問題的使用者指派

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: similar article exists for tasks)</p>
-->

您可以同時修改多個問題的使用者指派。 如需有關編輯問題或一次指派一個問題的資訊，另請參閱下列文章：

* [編輯問題](../../../manage-work/issues/manage-issues/edit-issues.md)
* [指派問題](../../../manage-work/issues/manage-issues/assign-issues.md)

如需指派問題的一般資訊，請參閱[修改問題指派的概觀](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md)。

>[!NOTE]
>
>您必須至少擁有Contribute許可權才能指派問題。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>要求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯問題的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理問題的許可權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>When to modify user assignments on issues</h2>
<p>(NOTE:&nbsp;drafted and moved to the overview article: Modify issue assignments overview)</p>
<p>You might want to modify the user assignments for multiple issues for a variety of&nbsp;reasons, including the following:</p>
<ul>
<li>Users join or leave&nbsp;your team</li>
<li>A user takes a vacation that extends beyond the issue&nbsp;due dates</li>
<li>A specific role or user is set as the assignee for multiple issues and you want to quickly modify all items to be assigned to a different user or role</li>
</ul>
</div>
-->

## 修改多個問題的指派

1. 前往問題清單，其中包含您要修改其指派的問題。
1. （選用）建立篩選器，只顯示指派給您要修改之受指派人的問題。

   例如，您可以建立篩選器，以僅顯示與作為受託人的特定角色有關的問題。 然後，您可以使用特定使用者來取代角色。 執行下列動作：

   1. 按一下&#x200B;**篩選器**&#x200B;下拉式清單，然後按一下&#x200B;**新增篩選器**。

      「新增篩選器」對話方塊隨即顯示。

   1. 按一下&#x200B;**新增篩選規則。**
   1. 若要篩選特定角色，請展開&#x200B;**指派角色，**，然後按一下&#x200B;**識別碼。**

      或

      若要篩選特定使用者，請展開&#x200B;**指派使用者，**，然後按一下&#x200B;**識別碼。**

      >[!TIP]
      >
      >請勿使用&#x200B;**指派給**，因為此欄位僅參考問題擁有者，而非所有受指派人。

   1. 在下拉式清單中，選取&#x200B;**等於**&#x200B;作為篩選限定詞。
   1. 開始輸入您要篩選的使用者或角色名稱，然後按一下該名稱（當它出現在下拉式清單中時）。
   1. 按一下&#x200B;**儲存篩選器。**

1. 選取您要修改指派的問題，然後按一下&#x200B;**編輯**&#x200B;圖示![](assets/qs-edit-icon.png)。

   **編輯問題**&#x200B;隨即顯示。 已編輯的專案會顯示在頁面的左上角。

1. 移至&#x200B;**工作分派**&#x200B;區段，然後選取&#x200B;**受指派人**。

   ![](assets/classic-assignmens-area-on-edit-box-350x119.png)

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

         （視條件而定）如果您要移除的受指派人未顯示在「工作分派」區段中，因為受指派人僅被指派給您選取的某些問題，請按一下&#x200B;**移除受指派人**&#x200B;並開始輸入您要移除的受指派人名稱，然後在其出現在下拉式清單中時按一下該名稱。

      1. 再按一下&#x200B;**移除被指定者**&#x200B;以新增另一個要移除的被指定者。

   1. 若要移除所有現有的被指定者：

      1. 按一下&#x200B;**移除所有現有的受指派人**，然後按一下&#x200B;**是，刪除所有受指派人**。

         這不僅會移除常見的受指派人（顯示在「編輯」對話方塊中的受指派人），也會移除所有選定問題中的所有受指派人。

1. （選擇性）針對您選取要與問題關聯的受指派人，修改下列任一選項：

   * **問題擁有者：**&#x200B;選取選項按鈕，以指出已將哪個受指派人指定為問題擁有者。 如果保持未選取，Adobe Workfront會將第一個受指派人指定為問題所有者。 這不適用於團隊指派。
   * **受指派人的角色**：從下拉式清單中選取一個角色。 如果保持未選取，Workfront會自動選取使用者的主要角色。

1. 按一下「**儲存變更**」。
