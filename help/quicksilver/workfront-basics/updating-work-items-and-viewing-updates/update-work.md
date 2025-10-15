---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 更新工作
description: 您可以在Adobe Workfront物件（專案、任務或問題）上新增更新，以傳達物件上的進度。 指派或訂閱物件的使用者可以檢視您的更新。 您也可以標籤使用者，以吸引他們注意更新。
author: Alina
feature: Get Started with Workfront
exl-id: 0f4d6895-6326-4a83-9bbc-bb58c876e7fc
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '3201'
ht-degree: 0%

---

# 更新工作

<!-- Audited: 4/2025 -->


<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

<!--info for April 11: hide the "Important" box below-->

<!--
>[!IMPORTANT]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>
>Depending on what objects you access the commenting experience for, you might see the following functionality for the Updates section:
>* The new experience
>* The legacy experience
>* The new and the legacy experience
>
>For more information about the new commenting experience and its availability, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
><Span class="preview"> The legacy commenting experience has been removed from projects, tasks, issues, and documents in the Preview environment. </span>
>
>The new commenting experience is available only for the Updates section of Workfront objects, and it is not available when you access updates from the following areas:
>
> * Home
> * Summary panel in lists
> * Summary panel in timesheets 
> * Summary panel in the Workload Balancer
>
><span class="preview">The new commenting experience is available in the Summary panel in lists, timesheets, and the Workload Balancer in the Preview environment and in the Production environment for customers who have opted for the fast release process. </span>
-->

您可以新增註解至Adobe Workfront物件，以通知其他人物件的狀態或進度，或要求更多資訊或其他資源，藉此為物件新增更新。

如需您可以在Workfront中新增更新的物件詳細資訊，請參閱[更新區段總覽](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md)。

本文中的資訊說明如何評論專案、任務和問題。 指派給物件或訂閱物件的使用者可以檢視您的更新。 您也可以標籤使用者，以吸引他們注意更新。

將註解新增至其他Workfront物件與更新專案、任務和問題類似。

如需在Workfront Planning中評論卡片、目標和記錄的其他資訊，另請參閱下列文章：

* [在Adobe Workfront目標中管理目標註解](../../workfront-goals/goal-management/manage-goal-comments.md)。

* [新增臨機卡到展示板](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md)

* [在展示板上使用連線的卡片](/help/quicksilver/agile/get-started-with-boards/connected-cards.md)

* [管理記錄註解](/help/quicksilver/planning/records/manage-record-comments.md)

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront套件</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront授權</strong></td> 
   <td> <p>對於問題和檔案：</p>

<ul><li><p>投稿人或以上</p></li>
   <li><p>要求或更高版本</p></li></ul>

<p>對於所有其他物件：</p>
   <ul><li><p>淺色或更高</p></li>
   <li><p>評論或以上</p></li></ul>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>存取層級設定</strong></td> 
   <td> <p>檢視或編輯更新所在物件的存取權</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件許可權</strong></td> 
   <td> <p>檢視物件的存取權</p></td> 
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
   <td role="rowheader"><strong>Adobe Workfront plan</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license*</strong></td> 
   <td> 
   <p>New: Contributor or higher for issues and documents: Light or higher for all other objects</p>
   <p>Current: Request or higher for issues and documents; Review or higher for all other objects</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configurations</strong></td> 
   <td> <p>View or Edit access for the object the update is on</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Object permissions</strong></td> 
   <td> <p>View access to the object</p></td> 
  </tr> 
 </tbody> 
</table>
-->

## 關於註解物件的考量事項

* 您可以在「更新」區段中，將註解新增至Adobe Workfront中的大部分物件。 如需有關哪些物件顯示「更新」區段的詳細資訊，請參閱[更新區段概觀](../updating-work-items-and-viewing-updates/updates-tab-overview.md)。

* 您可以從與Workfront整合的其他應用程式或Workfront行動應用程式，將註解新增至Workfront物件。

  並非所有與Workfront整合的應用程式都能對Workfront物件新增註解。

  從應用程式存取Workfront物件時，並非所有其他應用程式都能使用Workfront物件更新區段中可用的所有功能。 例如，從協力廠商應用程式將評論新增至Workfront物件時，RTF功能或讓評論成為某人的公司私密可能無法使用。

* 您可以在註解物件時傳達Workfront物件（專案、任務或問題）的進度。 指派或訂閱物件的使用者可收到有關您更新的通知。 擁有物件檢視存取許可權的任何人都可以檢視您的更新。

* 您可以標籤使用者，讓他們注意更新。 標籤的使用者會收到應用程式內通知及您更新的電子郵件。

  >[!TIP]
  >
  >註解擁有者會自動加上標籤。 如需詳細資訊，請參閱[標籤其他人的更新](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md)。


* 您可以將註解新增至可以檢視的物件，也可以以Workfront或群組管理員身分登入，並代表其他使用者新增註解。 如需詳細資訊，請參閱[以其他使用者身分登入](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md)。

* 您可以從Workfront的下列區域新增更新至專案、任務和問題：

   * 從Workfront物件，在更新區段（專案、任務和問題）
   * 從首頁區域（用於任務和問題）

     如需詳細資訊，請參閱[使用「我的工作」Widget](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-work-widget.md)管理您的工作。
   * 從「摘要」面板的下列區域（針對任務、問題和檔案）：

      * 物件清單
      * 時程表
      * 首頁
      * 工作負載平衡器

     如需詳細資訊，請參閱下列文章：

      * [摘要概觀](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
      * [使用摘要更新工作負載平衡器中的工作項](/help/quicksilver/resource-mgmt/workload-balancer/update-items-in-summary-panel-in-workload-balancer.md)

<!--info for April 11: hide the section below: add an update to a work item-->

<!--
## Add an update to a work item

Adding an update to a work item differs depending on what version of the Updates section you use.

You can add updates to the following objects: 

* Projects
* Tasks
* Issues
* Programs
* Portfolios
* Templates
* Template tasks
* Users
* Timesheets
* Teams
* Goals
* Cards in the Boards area
* Iterations
-->

<!--info for April 11: hide the section below completely:-->

<!--
### Add an update to a work item in the legacy Updates section

>[!IMPORTANT]
>
>The information on this page describes how you update projects, tasks, and issues.

1. Go to the work item for which you want to provide an update (such as a project, task, or issue).
1. Click the **Updates** section.
1. (Conditional) If it is enabled, click the **New commenting** option in the upper-right corner of the Updates section to disable it and enable the legacy commenting experience.
1. Click **Start a new update,** then type your update.  
1. (Optional) Use the options in the Rich Text toolbar to format your text, add emojis, links, or images to your update, to enhance your content. For more information, see the [Use Rich Text in a Workfront update](#use-rich-text-in-a-workfront-update) section in this article.
1. (Optional) Update any of the following information about the work item:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Notify</strong></td> 
      <td>Identify users who must be notified of the update. Users assigned or subscribed to the object automatically receive notification when an update is made.<br><p>For information about how to include others on an update, see <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Tag others on updates</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Commit Date</strong></td> 
      <td>In the date picker, select the date that you commit to complete the work item. For information about Commit Date, see <a href="../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">Commit Date overview</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Condition</strong></td> 
      <td>Select a new condition for the task or issue. For information about selecting a condition, see <a href="../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">Update Condition for tasks and issues</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Status</strong></td> 
      <td>Click the arrow beside the current status, then select the desired status from the drop-down menu. For information about setting a Status, see <a href="../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Update task status</a>.<p>Updating the status of a work item does not automatically change the status of a project. Depending on how your project is set up, you might make updates to the project status separately. For more information on the various project update types, see <a href="../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a>.</p><p><b>NOTE</b>
      
      You cannot change the status of a work item while it is in a Pending Approval status.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Completion Bar</strong></td> 
      <td>(Only available on tasks) Indicate the percentage of work completed by sliding the progress bar to the desired percentage. You can also double-click the completion bar and enter the percent complete.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Private to my company</strong></td> 
      <td> <p>Disable this option to prevent users outside your company from having access to view this update.</p> 
      <p><b>NOTE</b></p>
      <p>This option displays only when the user is associated with a Company.</p>
      <p>This option is not available in all areas where you can add updates from. For example, this is not available in third-party applications where you can add updates from. </p>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Update** to add the update to the Workfront object.

   >[!NOTE]
   >
   >A small pop-up window will appear for seven seconds after clicking **Update**, allowing you to undo the update and return to the editing pane before the update is posted. The update is posted if you dismiss the undo pop-up, wait for it to disappear, or navigate away from the page. 
   >
   >If your Workfront administrator selects the "Never allow users to delete comments" setting in your access level, you cannot undo a comment. For more information, see [Create and modify custom access levels](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

1. To reply to an update, see [Reply to updates](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md).
-->

<!--info for April 11: reword the title of this section to: "Add an update to a work item"; take out the step that says you need to enable the "New commenting" toggle (I think it is step 3??)-->

## 將註解新增至工作專案

本文會介紹如何更新專案、任務或問題。 更新大多數其他物件類似。

1. 找到您要新增註解的物件，然後按一下其名稱以開啟物件的頁面。
1. 按一下左側面板中的&#x200B;**更新**。
預設會選取&#x200B;**註解**&#x200B;標籤。

1. <span class="preview">開始在&#x200B;**新註解**&#x200B;方塊中輸入註解。</span>

   <span class="preview">![新註解方塊](assets/comment-box-all-tabs.png)</span>

   >[!TIP]
   >
   >在您完成輸入並提交評論之前離開更新區段，即使您登出並重新登入，仍會將頁面上的評論保留在草稿模式中。 加入註解的任何影像也會儲存在草稿中。 草稿會儲存7天，之後便會捨棄且無法復原。 草擬的註解僅對輸入註解的使用者可見。

1. （可選）若要復原或重做變更，請使用下列快速鍵：
   * CTRL + Z (Mac為⌘+z)可復原變更
   * 按CTRL + Y (Mac為⌘+y)以重做變更

1. <span class="preview"> （選擇性）在&#x200B;**標籤人員或團隊**&#x200B;區域，開始輸入您要加入此註解的使用者或團隊的名稱或電子郵件，或在其顯示在清單中時選取它。</span>
1. （可選）使用RTF工具列中的選項來格式化文字、新增emoji、連結或影像至更新，以強化內容。 如需詳細資訊，請參閱本文中的[在Workfront更新中使用RTF文字](#use-rich-text-in-a-workfront-update)一節。

   >[!TIP]
   >
   >如果其他使用者向您更新的相同專案提交評論，則會出現一條帶有「新」指示器的紅線，以通知您較新的評論。
   >
   >指示器只會在提交專案的註解後顯示，不會在註解仍在撰寫時顯示。
   >
   >「新」指標只有在輸入新更新的使用者以及目前輸入更新的使用者都使用新註解體驗時才會顯示。
   >![即時新紅色指標](assets/real-time-new-red-indicator-unified-commenting.png)

1. 按一下&#x200B;**提交**，將更新新增至Workfront物件。
1. （選擇性）若要編輯評論，請按一下評論右上角的&#x200B;**更多**&#x200B;功能表![更多](assets/more-menu.png)，然後按一下&#x200B;**編輯**。

   >[!IMPORTANT]
   >
   >您只能在提交評論的15分鐘內編輯評論。

1. 編輯註解中的資訊、新增或移除影像，或移除任何已標籤的使用者。 「已編輯」指示器會新增至日期戳記的左側，該日期戳記會在輸入評論時顯示。

   >[!TIP]
   >
   >目前年份的評論不會在日期戳記中顯示年份。 將游標暫留在時間戳記上會顯示完整日期，包括年份。

   ![已編輯註解上的指標](assets/edited-tag-on-comment-unified-commenting.png)

   >[!TIP]
   >
   >* 系統只會在您提交原始更新時，才會產生電子郵件通知使用者您的更新。 編輯更新後不會產生電子郵件。
   >* 註解旁邊的日期戳記是原始註解的日期，而不是上次編輯的日期。
   >* 當您代表另一個使用者新增註解時(以Workfront或群組管理員身份登入時)，如果您以其他使用者身份登入，則無法編輯註解。 只有在您以使用者身分登出並以您自己的身分重新登入後，才能編輯註解。

1. （選擇性）按一下「**回覆**」或開始在「**新增回覆……**」區域輸入註解，以回覆現有的註解，然後遵循上述步驟3-7。 <!--(**************insure this stays accurate***********)-->如需回覆更新的相關資訊，請參閱[回覆更新](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md)。

1. （條件式及選擇性）若其他使用者新增的註解顯示在[更新]區段的可見區域之外，而您新增註解時，請按一下熒幕底部的藍色&#x200B;**新註解橫幅**&#x200B;中的&#x200B;**檢視**&#x200B;以顯示這些註解。

   ![帶有按鈕的藍色新評論橫幅](assets/blue-new-comments-banner-with-view-button.png)

   熒幕底部會顯示其他註解。

1. （選擇性）按一下&#x200B;**贊**&#x200B;圖示![贊](assets/like-icon.png)。 圖示會隨著喜歡的數量而更新。
1. （有條件且選擇性）如果您在註解中包含其他人員，請按一下更新中包含的成員數目，以顯示與您輸入的註解共用之實體的清單。

   已展開![個成員圖示](assets/members-icons-expanded-unshimmed.png)

   >[!TIP]
   >
   >前兩個已標籤實體的名稱會顯示在它們的頭像旁。 如果兩個以上的圖元被標籤，則只顯示第一個圖元的名稱和其他圖元的數量。

1. （選用）按一下評論者的名稱，即可在資訊方塊中檢視其名稱、角色及電子郵件地址。 在資訊方塊中再次按一下評論者的名稱以開啟其使用者設定檔。
1. （選擇性）按一下&#x200B;**系統活動**&#x200B;索引標籤，以檢視系統記錄的更新。 當物件或其任何子系更新時，Workfront會產生有關該更新的附註，並將其顯示在系統活動標籤中。

   如需詳細資訊，請參閱[更新區段總覽](../updating-work-items-and-viewing-updates/updates-tab-overview.md)。

   >[!TIP]
   >
   >您無法將註解新增至系統更新。 但是，對舊版評論體驗中系統活動記錄所做的任何回覆，都會以唯讀形式新增至「系統活動」索引標籤。 舊版評論體驗已於2024年4月11日從Workfront移除。

1. （選擇性）按一下&#x200B;**全部**&#x200B;索引標籤，以在一個位置檢視使用者註解和系統活動註解。 這是僅供檢視的標籤。

   >[!TIP]
   >
   >您無法在[全部]索引標籤的現有註解中回覆註解或標籤其他使用者。 若要在[全部]索引標籤中回複評論，請按一下[在評論中回覆]&#x200B;**&#x200B;**，在[評論]索引標籤中開啟評論。

## 在Workfront註解中使用RTF文字{#use-rich-text-in-a-workfront-comment}

您可以使用RTF或新增各種專案（例如emoji、連結或影像）來增強您的註解。

1. 前往Workfront物件的&#x200B;**更新**&#x200B;區域，開啟&#x200B;**註解**&#x200B;索引標籤並開始輸入註解。
1. （選擇性）若要將RTF格式新增至您的註解，請在輸入時使用&#x200B;**RTF**&#x200B;工具列上的任何屬性。

   ![RTF工具列](assets/rich-text-toolbar.png)

   | **屬性** | **工具列按鈕** | **Mac快速鍵** | **Windows快速鍵** |
   |---|---|---|---|
   | 粗體 | ![粗體圖示](assets/mceclip10.png) | ⌘+b | Ctrl+B |
   | 斜體 | ![斜體圖示](assets/mceclip9.png) | ⌘+i | Ctrl+I |
   | 底線 | ![加底線圖示](assets/mceclip8.png) | ⌘+u | Ctrl+U |
   | 超連結 | ![超連結圖示](assets/mceclip7.png) | <br>若要開啟[新增連結]方塊： ⌘+K</br> <br>若要在選取的文字上貼上連結： ⌘+V</br> | <br>若要開啟[新增連結]方塊： Ctrl+K</br> <br>若要在選取的文字上貼上連結： Ctrl+V</br> |
   | 項目符號清單 | ![專案符號清單圖示](assets/mceclip6.png) | ⌘+Shift+8 | Ctrl+Shift+8 |
   | 編號清單 | ![編號清單圖示](assets/mceclip5.png) | ⌘+Shift+7 | Ctrl+Shift+7 |

   <!--| Block Quote | ![](assets/block-quote-icon-large.png)|⌘+Shift+9 |<br>Ctrl+Shift+9</br> <br>This is not available in the new commenting experience. </br> |-->

   <!--remove the last row when we remove legacy from the system-->

   若要停止格式化文字，請取消選取&#x200B;**RTF格式**&#x200B;工具列上的屬性。


   <!-- in the table above: take "Create Links" verbiage from the hyperlink when the old commenting is removed and the commenting beta is the only way to comment - with October 2023-->

   >[!NOTE]
   >
   >* 使用者收到的任何包含您更新的電子郵件通知中，也會顯示格式。
   >* 在更新索引標籤中檢視時，套用至電子郵件中更新的RTF格式未顯示在更新上。
   >* 如果您的組織搭配Internet Explorer使用Workfront，則貼入更新的任何格式化文字都會遺失RTF格式，並顯示為純文字。 您可以使用RTF工具列上的屬性來重新格式化文字。
   >* RTF格式不適用於「時程表」區域中進行的更新，或報表中檢視的「附註」和「最後條件」物件。

   <!--1. (Optional and conditional) If you want to include text from previous updates or from other sources and distinguish it from your own update, you can mark it as a Block Quote. Click the **Block Quote** icon ![](assets/block-quote-small.png) and type the text you want to quote. The quoted text displays marked with a vertical gray line. Click the **Block Quote** icon again to return to normal formatting. This is not available in the new commenting experience.-->

   <!--remove this picture below and the bullet above when we remove legacy-->

   <!--![](assets/block-quote-marked-350x144.png)-->

1. （選擇性）按一下&#x200B;**表情符號**&#x200B;圖示![表情符號圖示](assets/emoji-icon.png)以將表情符號新增至您的更新。

   >[!NOTE]
   >
   >* Workfront不會以表情符號取代標點符號表情符號，例如：)。
   >* 在報表中檢視的「附註」和「最後條件」物件無法使用Emoji。
   >* Workfront中的emoji功能使用Unicode字元，因此只會在支援Unicode字碼點的瀏覽器和作業系統上顯示。 平台、瀏覽器或作業系統版本與您的使用者不同，可能無法存取相同的emoji。
   >* 不支援的emoji會以黑白方塊表示。
   >* Windows 7僅支援黑白表情符號。
   >* 在「更新」區域中檢視時，套用至透過電子郵件進行的更新的Emoji不會顯示在更新上。

1. （選用）若要新增URL連結至其他資訊來源，請執行下列動作：

   1. 在更新中按一下您要插入連結的位置。
   1. 在&#x200B;**RTF**&#x200B;工具列上，按一下&#x200B;**超連結**&#x200B;圖示![超連結圖示](assets/link-icon.png)。

   1. 在&#x200B;**建立連結**&#x200B;方塊的&#x200B;**URL**&#x200B;下，輸入或貼上您要連結之來源的URL。

   1. 在&#x200B;**要顯示的文字**&#x200B;下，輸入或貼上連結文字。
   1. 按一下「**儲存**」。

1. （選用）將影像附加至更新。

   >[!WARNING]
   >
   >您無法將影像附加到下列物件的更新區域：
   >
   >* 目標
   >* 展示板上的臨時卡片
   >* Workfront Planning中的記錄。 如需詳細資訊，請參閱[Adobe Workfront規劃總覽](/help/quicksilver/planning/general/planning-overview.md)
   >

   若要將影像附加到更新中，請執行下列任一項作業：

   * 將影像儲存在電腦上，然後將其拖放到「新增註解」區域。
   * 從電腦複製熒幕擷圖，然後貼到註解中。
   * 按一下&#x200B;**新增影像**&#x200B;圖示![新增含加號圖示的影像山](assets/add-image-mountain-with-plus-icon.png)，並瀏覽您電腦上的影像。


   >[!IMPORTANT]
   >
   >
   ><!--<span class="preview">You cannot add images to goals or ad-hoc cards on boards.</span> -->
   >
   >* 您的Workfront管理員必須先在Workfront介面區域的更新摘要偏好設定區段中啟用新增影像，您才能看到影像或新增附件圖示。 如需詳細資訊，請參閱[設定使用者更新的偏好設定](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md)。
   >* 影像檔案大小上限為7 MB。 支援的影像檔案型別為.jpg、.gif和.png。
   >* 可從物件的「更新」區段存取影像，也可從主功能表下的「檔案」區域存取影像。
   >您可以使用鍵盤組合或Print Screen功能（在Windows電腦上）從您的電腦複製熒幕擷圖。
   >* 您可以在新的註解中按一下滑鼠右鍵，然後按一下&#x200B;**貼上**，或在鍵盤上按Windows適用的CTRL + V (或Mac適用的⌘ + V )，以貼上影像。
   >* 您可以傳送包含影像且不含文字的更新。
   >* 當您刪除包含影像的註解時，該影像會從「更新」區段及「檔案」區域移除。 當您編輯註解並刪除影像時，也會從「檔案」區域刪除影像。
   >* 當有人從「檔案」區域刪除附加至註解的影像時，該影像也會從註解中移除。

   <!--remove the statement above about legacy, when we remove the legacy environment.-->

1. （選擇性）若要在現有更新中檢視影像，請執行下列任一項作業：

   * 按一下影像縮圖上的&#x200B;**預覽**&#x200B;圖示![預覽圖示](assets/previewimageicon-31x31.png)，在新的瀏覽器標籤中開啟全尺寸影像。
   * 按一下影像縮圖上的&#x200B;**下載**&#x200B;圖示![下載圖示](assets/downloadimageicon.png)來下載影像。

1. 按一下&#x200B;**提交**&#x200B;以新增您的註解。

## 搜尋更新

您可以在物件的「更新」區段中搜尋註解或回覆。

1. 移至物件的&#x200B;**更新**&#x200B;區段。
1. 開始在<!--or a user's name -->註解&#x200B;**索引標籤右上角的**&#x200B;搜尋&#x200B;**方塊中輸入關鍵字**。

   <!--Add this tip or note instead of the note below - when it'll be possible: You can search for users who have been tagged or for comment owners.-->

   >[!NOTE]
   >
   >您只能搜尋屬於註解或回覆文字的單字。 您無法搜尋在更新中標籤的使用者或團隊名稱。

   ![搜尋更新](assets/updates-all-tabs-with-search-field.png)

   您搜尋的關鍵字<!--or user-->會反白顯示，而且包含該關鍵字的註解會顯示在「更新」區段的頂端。

   Workfront會搜尋物件的整個更新流，搜尋畫面上可見的註解之外。

1. 按一下搜尋欄位中的&#x200B;**x**&#x200B;圖示以清除搜尋結果並返回所有註解。

<!-- when we release search to production, check above and make sure you don't have to add that the users tagged/ owners are also searchable-->

## 複製註解

有幾種方法可以複製註解。

您可以複製註釋的連結，或複製註釋的內容以將其用於新的更新。

<!--Copying an update differs depending on which commenting experience you use.-->

<!--info for April 11: take the sentence above out and reword the section title below to: Copy an update-->

### 複製評論

您可以執行下列任一項作業，從現有註解複製資訊：

* [引用回覆](#quote-reply)
* [複製連結](#copy-link)
* [複製本文](#copy-body-text)


![以各種方式複製註解](assets/copy-comment-ways-from-more-menu-on-comment.png)

#### 引用回覆

「報價」回複選項會將原始註解複製到新的回覆，做為區塊報價。

1. 移至您要複製的註解或回覆。
1. 按一下&#x200B;**更多**&#x200B;功能表，然後按一下&#x200B;**報價回覆**。

   新註解方塊開啟，引述的回覆會包含在新的註解中，並標示為區塊引號。

   提交前![封鎖引號標示為中間註解](assets/block-quote-highlighted-mid-comment-before-submit.png)


1. 繼續新增您的更新，然後按一下&#x200B;**提交**&#x200B;以新增註解。

#### 複製評論連結

「複製連結」選項可將註解或對話串連結複製到剪貼簿，以便與其他使用者共用註解或整個對話串。

1. 前往您要複製其連結的註解。

1. 按一下&#x200B;**更多**&#x200B;功能表，然後按一下&#x200B;**複製連結**。

1. 將您在上一步中複製的連結貼入電子郵件或其他應用程式，以便與其他人共用。 共用連結會開啟您共用連結的註解。

   >[!TIP]
   >
   >當您從較高層級的物件在子物件上共用對話連結時，該連結會在較高層級物件的「更新」區域中開啟對話串。
   >
   >例如，如果您從專案的更新區域複製任務註解的連結，註解會開啟專案頁面。

#### 複製本文

「複製內文」選項會將文字從特定註解複製到剪貼簿。

1. 移至您要複製的註解或回覆。
1. 按一下&#x200B;**更多**&#x200B;功能表，然後按一下&#x200B;**複製內文**。



<!--info for April 11: hide the entire section below - notice that there are several sub-sub sections below this main section - hide them all, all the way up to "Delete an update"-->

<!--
### Copy an update in the legacy commenting experience

* [Copy the update](#copy-the-update) 
* [Copy the thread link](#copy-the-thread-link) 
* [Copy the update link](#copy-the-update-link)
* [Quote Reply](#quote-reply)

   >[!TIP]
   >
   >When you copy and share the link of a conversation on a child object from a higher-ranking object, the link opens the thread in the child object's Updates area. 
   >
   >For example, if you copy the link of a task comment from the project's Updates area, the comment opens the task page.

#### Copy the update {#copy-the-update}

This option copies the text from a specific update to the clipboard.

1. Go to the update or reply you want to copy.
1. Click the **More** menu, then click **Copy body text**.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

#### Copy the thread link {#copy-the-thread-link}

This option copies the full thread link to the clipboard so you can share the thread with other users.

1. Go to the update thread you want to copy.

1. Click the **More** menu, then click **Copy thread link**.

   ![](assets/update-stream-comment-menu-marked-350x152.png) 

1. Paste the link you copied in the previous step in an email or another application to share it with others. The shared link opens the comment you shared the link from. 

#### Copy the update link {#copy-the-update-link}

This option copies a specific update link to the clipboard. When you share the update link, the user who follows it sees a border around the update.

1. Go to the update or reply you want to copy.
1. Click the **More** menu next to the individual update, then click **Copy update link**.

   ![](assets/copy-update-link-old-ui.png)

1. Paste the link you copied in the previous step in an email or another application to share it with others. The shared link opens the comment you shared the link from. 

#### Quote Reply  

The Quote Reply option copies the original comment to a new reply as a block quote. 

1. Go to the update or reply you want to copy.
1. Click the **More** menu, then click **Quote Reply**.

   A new comment box opens and the quoted reply is included in the new comment and marked as a block quote.

1. Continue adding your update and click **Reply** to add the comment.
-->

## 刪除評論或回覆

根據Workfront管理員賦予您的存取權，您或許可以刪除在物件的「更新」區段中新增的註解。

如需詳細資訊，請參閱文章[建立或修改自訂存取層級](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch)中的[建立或修改自訂存取層級](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

Workfront使用者(包括Workfront管理員)無法刪除其他使用者所做的更新。 但是，如果使用者的存取層級允許他們刪除自己的更新，Workfront管理員可以以該使用者的身分登入，並刪除他們所做的更新。 如需詳細資訊，請參閱[建立或修改自訂存取層級](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch)和[以其他使用者身分登入](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md)。

1. 前往您要刪除的註解或回覆。
1. 按一下您要刪除的評論或回覆旁的&#x200B;**更多**&#x200B;功能表，然後按一下&#x200B;**刪除**。

   ![更新資料流註解更多功能表](assets/update-stream-comment-menu-marked-350x152.png)

1. 在顯示的訊息中，按一下&#x200B;**刪除**。

   >[!NOTE]
   >
   >刪除具有附加影像的更新會同時刪除註解和影像。 如需詳細資訊，請參閱本文中的[在Workfront更新中使用RTF文字](#use-rich-text-in-a-workfront-update)一節。

   當您刪除的評論有關聯的回覆時，會顯示已移除評論，以及移除評論的使用者姓名。

   ![已移除評論指標](assets/removed-comment-indicator-new-experience.png)

   已刪除的評論會立即從Workfront中移除。 使用更新區段的使用者會看到另一個使用者即時刪除的評論。


## 檢閱系統更新

Workfront物件的更新區段會顯示兩種型別的資訊：

* **使用者更新：**&#x200B;使用者更新是您和您系統中的其他使用者輸入的註解。 使用者更新會顯示在「更新」區段的「註釋」和「全部」標籤中。

  ![使用者更新](assets/user-update-cl-350x277.png)

* **系統更新：**&#x200B;系統更新記錄移除任務或問題、新增或刪除檔案版本、附加或移除核准要求，以及對物件所做的任何編輯或變更。 系統更新會顯示在「系統活動」和「更新」區段的「所有」標籤中。

  ![系統更新](assets/system-updates-cl-350x277.png)

  如[系統追蹤更新](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md)所述，Workfront管理員可決定系統更新中追蹤的內容。 您也可以篩選掉系統更新或活動，以便只看到所有物件的使用者更新。

  下列物件沒有系統產生的更新：

   * 團隊
   * 範本
   * 範本任務
   * 展示板上的臨時卡片

如需有關使用者和系統更新以及它們在Workfront物件更新區段中如何顯示的詳細資訊，請參閱[更新區段概觀](../updating-work-items-and-viewing-updates/updates-tab-overview.md)。


<!--
After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>  
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>  
-->

<!-- with October 26 release: add somewhere this, and decide where we need to keep information about the legacy commenting. Should we create an article about iterations comments like we have for goals and cards?!:

>[!NOTE]
>
>Iterations display the legacy commenting experience.-->

<!--old message, before Auhust 17: 

>[!NOTE]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>
>For more information about the new commenting experience, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
>You can access the new experience for the following objects:
> * Issues, projects, tasks, and documents.
>
>     This is available when you enable the commenting Beta experience.
>
>     This functionality is available only for the Updates section, and it is not available for the following areas:
>
>     * Home
>     * Summary panel in lists
>     * Summary panel in timesheets
>
> * Goals, cards in the Boards area
>
>   The new commenting experience is the only experience for goals and cards. You must have an additional license to access Workfront Goals. For more information, see [Requirements to use Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md). 
>
>     You can add and view updates to cards in the Boards area when you enable the Comments and System Activity sections on a card. For more information, see [Add an ad hoc card to a board](../../agile/get-started-with-boards/add-card-to-board.md).
-->
