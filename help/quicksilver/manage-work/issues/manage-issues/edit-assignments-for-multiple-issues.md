---
product-area: projects
navigation-topic: manage-issues
title: 修改清單中多個問題的用戶分配
description: 修改清單中多個問題的用戶分配
author: Alina
feature: Work Management
exl-id: e1e75027-1847-44cf-afeb-b19394dc3ea5
source-git-commit: 7e77223595d3c9cf0d6592a09e893142439adb2c
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 1%

---

# 修改清單中多個問題的用戶分配

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: similar article exists for tasks)</p>
-->

您可以同時修改多個問題的使用者指派。 如需編輯問題或一次指派問題的相關資訊，另請參閱下列文章：

* [編輯問題](../../../manage-work/issues/manage-issues/edit-issues.md)
* [指派問題](../../../manage-work/issues/manage-issues/assign-issues.md)

如需指派問題的一般資訊，請參閱 [修改問題分配概覽](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!NOTE]
>
>您至少必須擁有問題的Contribute權限，才能指派給問題。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯問題的存取權</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理問題的權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

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

## 修改多個問題的分配

1. 轉到包含要修改其分配的問題的問題清單。
1. （選用）建立篩選器，僅顯示指派給您要修改之受託人的問題。

   例如，您可以建立篩選器，以僅顯示特定角色作為受託人的問題。 然後，您可以將角色取代為特定使用者。 執行下列動作：

   1. 按一下 **篩選** 下拉式清單，然後按一下 **新增篩選**.

      隨即顯示「新建篩選器」對話框。

   1. 按一下 **新增篩選規則。**
   1. 若要篩選特定角色，請展開 **分配角色，** 然後按一下 **ID.**

      或

      若要篩選特定使用者，請展開 **分配用戶，** 然後按一下 **ID.**

      >[!TIP]
      >
      >請勿使用 **指派給** 因為此欄位僅指問題所有者，而非所有受分配者。

   1. 在下拉式清單中，選取 **等於** 作為篩選限定符。
   1. 開始鍵入要篩選的用戶或角色的名稱，然後在下拉清單中出現時按一下該名稱。
   1. 按一下 **儲存篩選器。**

1. 選擇要修改分配的問題，然後按一下 **編輯** 圖示 ![](assets/qs-edit-icon.png).

   此 **編輯問題** 顯示。 編輯的項目會顯示在頁面的左上角。

1. 前往 **分配** 區段，然後選取 **受託人**.

   ![](assets/classic-assignmens-area-on-edit-box-350x119.png)

1. 執行下列任一項作業：

   1. 要添加新的受託人，請執行以下操作：

      1. 開始鍵入用戶、角色或團隊的名稱，然後在清單中顯示時選擇它。 將添加分配，不會替換所選問題上的當前分配。

         >[!TIP]
         您可以指派多個使用者、工作角色或團隊。 您只能指派作用中的使用者、工作角色和團隊。
         如果在停用前已指派使用者、工作角色或團隊，則他們仍會指派給工作項目。 在此情況下，我們建議：
         * 將工作項重新分配給活動資源。
         * 將已停用團隊中的用戶與活動團隊關聯，並將工作項重新分配給活動團隊。


         所有選取的問題中都很常見的資訊會隨即顯示。 例如，如果將相同的使用者指派給所有問題，該使用者會顯示在 **受託人** 欄。 如果資訊在所選問題中不常見，則不會顯示任何資訊。
   1. 要刪除單個受分配者，請執行以下操作：

      1. 按一下 **X圖示** 如果「分配」清單中顯示了受分配人，則您要刪除的受分配人的名稱旁邊。

         或

         （條件性）如果要刪除的受託人不會顯示在「分配」部分，因為受託人僅分配給您選擇的某些問題，請按一下 **刪除受託人** 然後開始鍵入要刪除的受託人的名稱，然後在下拉清單中出現名稱時按一下該名稱。

      1. 按一下 **刪除受託人** 再次添加另一個要刪除的受託人。
   1. 要刪除所有現有受分配者：

      1. 按一下 **刪除所有現有受分配者**，然後按一下 **是，刪除所有受分配者**.

         這不僅會刪除常見的受分配者（在編輯對話框中顯示的受分配者），而且還會刪除所有選定問題上的所有受分配者。



1. （可選）為您選擇與問題關聯的受分配者修改以下任何選項：

   * **問題所有者：** 選擇單選按鈕，以指明將哪個受託人指定為「問題責任人」。 如果未選取，Adobe Workfront會指定第一個受託人為問題擁有者。 這不適用於團隊分配。
   * **受託人的角色**:從下拉式清單中選取角色。 如果未選取，Workfront會自動選取使用者的主要角色。

1. 按一下 **儲存變更**.
