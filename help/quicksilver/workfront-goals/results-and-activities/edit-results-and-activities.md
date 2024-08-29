---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: 在Adobe Workfront目標中編輯結果和活動
description: Adobe Workfront管理員授與您對Adobe Workfront目標的正確存取權後，您就可以建立及編輯目標、結果和活動。
author: Alina
feature: Workfront Goals
exl-id: 922a05f9-2995-4401-a6d2-e5a331270fd3
source-git-commit: d7dd5ab4e3041a100b13c5bf169747f58db0ea39
workflow-type: tm+mt
source-wordcount: '763'
ht-degree: 1%

---

# 在Adobe Workfront目標中編輯結果和活動

Adobe Workfront管理員授與您對Adobe Workfront目標的正確存取權後，您就可以建立及編輯目標、結果和活動。

如需有關建立目標、結果和活動的資訊，請參閱下列文章：

* [在Adobe Workfront目標中建立目標](../../workfront-goals/goal-management/create-goals.md)
* [開始使用Adobe Workfront目標中的結果和活動](../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md)
* [將結果新增至Adobe Workfront目標中的目標](../../workfront-goals/results-and-activities/add-results-to-goals.md)
* [將活動新增至Adobe Workfront目標中的目標](../../workfront-goals/results-and-activities/add-activities-to-goals.md)

## 存取需求

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
  <ul><li>終極計畫 </li></ul>
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
 <p> 新產品需求，下列其中一項： </p>
<ul>
<li>Select或Prime Adobe Workfront計畫以及額外的Adobe Workfront目標授權。</li>
<li>預設包含Workfront目標的Ultimate Workfront計畫。 </li></ul>
 <p>或</p>
 <p>目前產品需求： Adobe Workfront Goals的Workfront計畫和額外授權。 </p> <p>如需詳細資訊，請參閱<a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">使用Workfront目標的需求</a>。 </p> </td>
 </tr>
 <tr>
 <td role="rowheader"><p>存取層級</p></td>
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

## 編輯結果和活動時的注意事項

<!--
According to Vazgen, access levels will add more considerations.)
-->

* 您可以編輯屬於您建立的目標或您擁有管理許可權之目標的結果和活動。
* 您無法從Workfront目標中編輯作為活動連線到目標的專案進度。 專案中的任務完成時，會更新專案進度。 您可以中斷專案的連線，從目標中移除專案。 如需詳細資訊，請參閱文章[從Adobe Workfront目標中的目標移除結果、活動和專案](../../workfront-goals/results-and-activities/remove-results-activities-from-goals.md)中的「中斷專案連線」一節。

  >[!NOTE]
  >
  >如果下列專案資訊在專案層級更新，Workfront目標會自動在目標層級更新：
  >
  >   
  >   
  >   * 專案所有者
  >   * 專案名稱
  >   * 專案完成百分比
  >   
  >   
  >如需有關將專案連線至目標的資訊，請參閱[在Adobe Workfront目標中新增專案](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md)。

* 當結果和活動不再與目標進度相關時，您可以從目標中刪除它們。 已刪除的結果和活動無法復原。 如需有關刪除結果和活動的資訊，請參閱[從Adobe Workfront目標中的目標移除結果、活動和專案](../../workfront-goals/results-and-activities/remove-results-activities-from-goals.md)。
* 您可以編輯任何時段（包括過去）內與目標相關聯的結果和活動。
* 編輯結果和活動會更新其設定，而不會更新其進度。 您必須更新結果和活動的進度。 如需有關更新目標、結果和活動進度的資訊，請參閱[在Adobe Workfront目標中更新目標進度](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md)。

## 編輯結果

<!--
Editing results differs depending on which environment you use.

### Edit results in the Production environment

1. Go to the goal for which you want to edit a result and click the goal name to open the **Goal Details** panel.
1. Click **Results**.
1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the result you want to edit.

   ![](assets/results-gear-icon-options-350x85.png)

1. Click **Edit** to edit the following information:

   | Field |Description|
   |---|---|
   | Name |The name of the result. |
   | Owner |The owner of result.  |
   | Value |How you measure the progress of the result. |
   | Initial |The original value of the result. |
   | Target |The desired value when the result is completed. |

1. Click **Save**.
-->


1. 按一下&#x200B;**主要功能表** ![](assets/main-menu-icon.png)，然後按一下&#x200B;**目標**。
1. 從目標清單中，按一下目標的名稱以開啟目標頁面。
1. 按一下左側面板中的&#x200B;**進度指示器**。
1. 在[進度指示器]清單中選取結果，然後按一下&#x200B;**編輯**&#x200B;圖示![](assets/edit-icon.png)。

   「編輯結果」方塊開啟。

   ![](assets/edit-result-box-unshimmed.png)

1. 編輯下列資訊：
   * **結果名稱**：結果的名稱。 使用說明性名稱，說明您需要取得什麼結果才能完成目標。
   * **結果擁有者**：結果的擁有者。 擁有者必須是使用中的Workfront使用者。
   * **值型別**：如何測量結果的進度。
   * **初始值**：結果的原始值。
   * **目標值**：結果完成時的所需值。
如需結果欄位的詳細資訊，請參閱[將結果新增至目標](../results-and-activities/add-results-to-goals.md)。
1. 按一下「**儲存**」。

## 編輯活動

<!--
Editing activities differs depending on which environment you use.

### Edit activities in the Production environment

>[!TIP]
>
>You cannot edit the Activity Type after you saved an activity on a goal.

1. Go to the goal for which you want to edit an activity and click the goal name to open the **Goal Details** panel.
1. Click **Activities**.
1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the activity you want to edit .

   ![](assets/activities-gear-icon-options-350x84.png)

1. Click **Edit** to edit the following information:

   | Field |Description |
   |---|---|
   | Name |The name of the activity. |
   | Owner |The owner of activity.  |

1. Click **Save**.
-->

1. 按一下&#x200B;**主要功能表** ![](assets/main-menu-icon.png)，然後按一下&#x200B;**目標**。
1. 從目標清單中，按一下目標的名稱以開啟目標頁面。
1. 按一下左側面板中的&#x200B;**進度指示器**。
1. 在進度指標清單中選取活動，然後按一下&#x200B;**編輯**&#x200B;圖示![](assets/edit-icon.png)。

   「編輯活動」方塊開啟。

   ![](assets/edit-activity-box-unshimmed.png)

1. 編輯下列資訊：
   * **活動名稱**：活動的名稱。 使用說明性名稱，說明您應該執行哪些活動，以指出目標已完成。
   * **活動擁有者：**&#x200B;活動擁有者。 擁有者必須是使用中的Workfront使用者。\
     如需活動欄位的詳細資訊，請參閱[將活動新增至目標](../results-and-activities/add-activities-to-goals.md)。
1. 按一下「**儲存**」。


