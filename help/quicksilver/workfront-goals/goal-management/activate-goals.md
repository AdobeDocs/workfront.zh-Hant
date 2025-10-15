---
product-previous: workfront-goals
navigation-topic: goal-management
title: 在Adobe Workfront目標中啟用目標
description: 當您建立目標時，Adobe Workfront目標會以草稿狀態儲存目標。 草擬的目標不屬於目標管理。
author: Alina
feature: Workfront Goals
exl-id: fc556073-fe63-4f13-a313-505ca0ef1f9b
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 1%

---

# 在Adobe Workfront目標中啟用目標

<!--Audited for P&P only: 4/2025-->

當您建立目標時，Adobe Workfront目標會以草稿狀態儲存目標。 草擬的目標不屬於目標管理。

若要追蹤您透過更新進度達到目標的接近程度，您必須啟動目標。 這會將它的狀態變更為作用中。

如需建立目標的相關資訊，請參閱[在Adobe Workfront目標中建立目標](../../workfront-goals/goal-management/create-goals.md)。

>[!IMPORTANT]
>
>您必須先啟動目標，才能更新其結果和活動的進度。


## 存取需求

>[!NOTE]
>
>如果貴公司過去曾購買此套件，他們可能會選擇繼續使用Adobe Workfront目標。 如需詳細資訊，請洽詢客戶代表。
>
>Adobe Workfront目標不再提供購買。

+++ 展開以檢視本文中功能的存取需求。 

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
  <tr>
  <td> <p>Adobe Workfront套件</p> </td> 
   <td> 
   <p>Adobe Workfront Ultimate</p>
   </td> 
  </tr> 
  <tr>
 <td role="rowheader">存取層級設定</td>
 <td> <p>編輯目標的存取權</p> </td>
 </tr>
 <tr>
 <td role="rowheader">物件許可權</td>
 <td>
  <div>
  <p>檢視目標或更高許可權以檢視它</p>
  <p>管理目標的許可權以編輯它</p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> <p>必須為所有使用者（包括系統管理員）指派一個版面配置範本，該範本包括主功能表中的「目標」區域。 </p>  
</td>
  </tr>
</tbody>
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Old:
<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> 
   <p>For the new plan and license structure:
  <ul><li>An Ultimate plan </li></ul>
   </p>
<p>For the current plan and license structure: 
<ul><li> A Pro or higher </li>
  <li>An Adobe Workfront Goals license in addition to a Workfront license.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
  <p> New product requirement: Workfront</p>
 <p>Or</p>
  <p>Current product requirement: In addition to a Workfront license, you must purchase a license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Access level</td>
 <td> <p>Edit access to Goals</p> </td>
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
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>-->

## 先決條件

若要啟用目標，該目標必須與諸如活動、結果、專案之類的進度指示器相關聯，或它與其他使用中的目標校準。

請至少執行下列任一項作業來啟動目標：

* 將結果新增至目標

  如需詳細資訊，請參閱[在Adobe Workfront目標中新增結果](../../workfront-goals/results-and-activities/add-results-to-goals.md)。

* 將活動新增至目標

  如需詳細資訊，請參閱[在Adobe Workfront目標中新增活動](../../workfront-goals/results-and-activities/add-activities-to-goals.md)。

* 將專案連線到目標

  如需詳細資訊，請參閱[在Adobe Workfront目標中新增專案](../results-and-activities/connect-projects-to-goals-overview.md)。

* 將另一個目標與您要啟用的目標校準

  如需詳細資訊，請參閱[在Adobe Workfront目標中連線以對齊目標](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md)。

## 啟動目標

您可以啟用您建立的目標或您對其擁有管理許可權的目標。

1. 前往您要啟用的目標。 目標頁面隨即開啟。

1. 按一下目標名稱右邊的&#x200B;**更多**&#x200B;功能表![更多圖示](../goal-management/assets/more-icon.png)，然後按一下&#x200B;**啟用**。

   ![其他功能表已展開](assets/more-menu-on-goal-expanded-with-activate-unshimmed.png)

   目標狀態會變更為作用中。 您現在可以追蹤目標的進度，目標會顯示在「簽入」區段中，並在Workfront目標的圖形區段中加以考慮
