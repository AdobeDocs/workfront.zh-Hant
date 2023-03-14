---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 統一的注釋體驗
description: 新的統一注釋體驗將
author: Nolan
feature: Get Started with Workfront
source-git-commit: b2859f3d268bd947fba5bb0280677465b3039d93
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 1%

---


# 全新評論體驗

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> -->

Adobe Workfront中備注體驗的更新目前正在開發中。 此更新包含新介面、新功能，以及選取物件的「更新」區段中的效能提升。

<!--drafted for commenting experience on issues: 

>[!NOTE]
>
>The new commenting experience is not available for other areas of Workfront that displays updates. For example, the new experience is not availabe for the following areas:
>
>* Home
>* Summary panel in a list
>* Summary panel in a timesheet
>
>The new commenting experience is only available for the Updates section of select objects. 
>
>For information about what objects include the Updates section, see [Updates tab overview](../../workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md). 
-->

雖然目前僅在Adobe工作字型目標中實作，但這項新體驗將緩慢開放供Workfront中具有更新區段的所有物件使用，之後會擴展至其他Adobe Experience Cloud應用程式。

<!--when we release to Preview for issues with a toggle, we need to remove the last sentence above and replace it with this: 

The new commenting experience is currently supported for the following objects in Workfront:

By default, in the Preview and Production environments for all customers: 

* Goals

    >[!NOTE]
    >
    >You must have an additional license to Adobe Workfront Goals to be able to access this area of Workfront. For more information, see [Requirements to use Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).

    For more information about managing updates for goals, see [Manage goal comments in Adobe Workfront Goals](../../workfront-goals/goal-management/manage-goal-comments.md). 


<div class="preview">

By enabling the Beta toggle, in the Preview environment: 

* Issues

    For more information about managing updates for other objects, including issues, see [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). 

</div>

This new experience will slowly become available for all the objects with an Updates section in Workfront, and later it will expand to other Adobe Experience Cloud applications.
-->

## 功能

新的註解體驗包含對現有更新資料流的改良與變更。

>[!IMPORTANT]
>以下所列的「統一注釋體驗」功能目前僅可在Adobe Workfront Target中使用。

* **建立注釋**

   您可以建立新留言、以RTF格式設定留言，並標籤要通知的其他留言。 有關建立注釋的詳細資訊，請參閱 [管理目標備注](/help/quicksilver/workfront-goals/goal-management/manage-goal-comments.md).

* **回應留言**

   您可以使用贊回應留言，或使用新留言回覆，以通知原始留言者和物件擁有者。

* **系統活動**

   系統產生的物件更新現在會與更新標籤中的註解分開列出。 有關查看系統活動流的詳細資訊，請參閱 [管理目標備注](/help/quicksilver/workfront-goals/goal-management/manage-goal-comments.md).

<!-- When releasing this to Issues - preview with 23.2 - remove all the content above in the "Features" section and replace it with this: 

One of the main differences between the current and the new commenting experience is the separation of user-submitted comments and system activity updates with the introduction of the System Activity tab. There are no changes to the way system-generated activity updates function.

Among the improvements included in the new commenting experience are the following:

* Better, faster performance 
* Real-time updates
* Edit comments after submitting them. 

The following table illustrates the features that will be available in the new commenting experience as well as their availability now in areas where they are supported: 

<table>
  <tr>
   <td><strong>Feature </strong>
   </td>
   <td><strong>Exists in old commenting experience </strong>
   </td>
   <td><strong>Exists in Beta version of the new commenting experience </strong>
   </td>
   <td><strong>Will be introduced in the new commenting experience </strong>
   </td>
   <td><strong>When will be introduced in the new commenting experience </strong>
   </td>
   <td><strong>In research </strong>
   </td>
  </tr>
  <tr>
   <td>Create/read/reply/delete comments 
   </td>
   <td>✓ 
  </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Rich text (exludes quoting and emojis)
   </td>
   <td>✓ 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
 <tr>
   <td>Rich text (quoting and emojis)
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> ✓
   </td>
   <td> Q2, 2023
   </td>
   <td> 
   </td>
  </tr>
  <tr>

   <td>React to comments (Like) 
   </td>
   <td>✓ 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Attach images to comments 
   </td>
   <td>✓ 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Tag people in comments 
   </td>
   <td>✓ 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Remove people from the thread 
   </td>
   <td> 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Comments that are private to a company 
   </td>
   <td>✓ 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Undo posting of a comment 
   </td>
   <td>✓ 
   </td>
   <td>Replaced with edit comment 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Turn off system updates 
   </td>
   <td>✓ 
   </td>
   <td>Replaced with Activity tab 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Edit comments 
   </td>
   <td> 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Saving comment drafts when navigating away from the page 
   </td>
   <td>✓ 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>See new comments in real time 
   </td>
   <td> 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Log time 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td>✓ 
   </td>
  </tr>
  <tr>
   <td>Edit custom form 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td>✓ 
   </td>
  </tr>
  <tr>
   <td>Ability to edit status, condition, commit date while commenting 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td>✓ 
   </td>
  </tr>
  <tr>
   <td>Copy thread link 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td>✓ 
   </td>
   <td>Q2, 2023 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Copy comment link 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td>✓ 
   </td>
   <td>Q2, 2023 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Quote comment text 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td>✓ 
   </td>
   <td>Q2, 2023 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Copy body text 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td>✓ 
   </td>
   <td>Q2, 2023 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Resolve comments 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td>✓ 
   </td>
   <td>Q3, 2023 
   </td>
   <td>✓ 
   </td>
  </tr>
  <tr>
   <td>Search in comments 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td>✓ 
   </td>
   <td>Q3, 2023 
   </td>
   <td>✓ 
   </td>
  </tr>
</table>

-->
