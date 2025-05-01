---
title: 管理記錄註解
description: 您可以在記錄的右側面板中新增評論或回覆，對Adobe Workfront Planning記錄進行共同作業。 您也可以在此區域中檢視系統記錄的其它變更。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 215883a4-e882-438e-9c21-954c0b1d741b
source-git-commit: e25f6ac3fb4ffc114d59bf5cceecfe718ae914ec
workflow-type: tm+mt
source-wordcount: '1063'
ht-degree: 0%

---

# 管理記錄註解

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

您可以在記錄的右側面板中新增評論或回覆，對Adobe Workfront Planning記錄進行共同作業。 您也可以在此區域中檢視系統記錄的其它變更。

記錄的右側面板會顯示下列區段：

* **註解**：顯示註解及使用者新增至記錄的回覆。
* **歷程記錄**：顯示使用者對記錄欄位所做的系統記錄變更。 如需詳細資訊，請參閱[歷程記錄區段總覽](/help/quicksilver/planning/records/history-section-overview.md)。

## 存取需求

+++ 展開以檢視存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> 產品</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront規劃<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront計畫*</p></td> 
   <td> 
<p>下列任一Workfront計畫：</p> 
<ul><li>選取</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>舊版Workfront計畫不提供Workfront計畫</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront規劃套件*</p></td> 
   <td> 
<p>任何 </p> 
<p>如需每個Workfront計畫包含內容的詳細資訊，請聯絡您的Workfront客戶經理。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront平台</p></td> 
   <td> 
<p>貴組織的Workfront例項必須上線至Adobe Unified Experience，才能存取Workfront Planning的所有功能。</p> 
<p>如需詳細資訊，請參閱<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">適用於Workfront的Adobe Unified Experience</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權*</p></td> 
   <td><p> 投稿人或更高授權</p>
   <p>Workfront計畫不適用於舊版Workfront授權</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>存取層級設定</p></td> 
   <td> <p>Adobe Workfront Planning沒有存取層級控制</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td>   <p>檢視工作區<span class="preview">和記錄型別</span> </a>的或更高許可權 </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>版面配置範本</p></td> 
   <td> <p>在「生產」環境中，所有使用者（包括系統管理員）都必須指派給包含Planning區域的版面配置範本。</p>
   <div class="preview">
<p> 在「預覽」環境中，必須為具有輕度或貢獻者授權的使用者指派包含Planning的版面配置範本。</p>

<p>標準使用者和系統管理員預設啟用Planning。</p></div>

<p>如需詳細資訊，請參閱<a href="/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md">建立及管理配置範本</a>。</p> </td> 
  </tr> 
</tbody> 
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++



## 在記錄上加上註解的考量事項

* 您可以在Workfront Planning中，於記錄的「註解」區段中，新增註解及回覆至記錄。

* 新增至連結記錄的註解不會顯示在您連結的記錄上。 例如，如果您對連結至促銷活動記錄的Workfront Planning產品記錄加上註解，該註解只會顯示在Workfront Planning的產品記錄上，而不會顯示在您連結的促銷活動記錄上。

* 您可以將註解新增至由於記錄與其他應用程式物件之間的連線而建立的Workfront Planning記錄。

  例如，將Workfront專案與Workfront Planning記錄連線後，您就可以對Workfront Planning專案記錄加上註解。 如需詳細資訊，請參閱[連線記錄](/help/quicksilver/planning/records/connect-records.md)。

* 新增至其他應用程式中連結物件的註解不會顯示在Workfront Planning中，而新增至Workfront Planning中連結物件的註解不會顯示在其他應用程式中。

  例如，在Workfront中新增至專案的評論不會顯示在連結至Workfront Planning中行銷活動的相同專案上，而新增至專案Workfront Planning記錄的評論不會顯示在Workfront中。

* 您可以標籤使用者，以提醒他們注意更新。 標籤的使用者不會收到應用程式內通知或有關您更新的電子郵件。<!--this might change??-->

* 您可以標籤使用者，以提醒他們注意更新。 標籤的使用者會收到應用程式內通知或您更新的電子郵件通知。

  >[!NOTE]
  >
  >   只有已加入Adobe Unified Experience的客戶之使用者，才會同時收到應用程式內通知和電子郵件通知。 若要判斷您的公司是否使用Adobe Unified Experience，請參閱[Workfront的Adobe Unified Experience ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md)。

* 您可以新增更新至記錄，並從Workfront Planning的下列區域複查變更歷史記錄：

   * 從記錄詳細資訊頁面。
   * 從檢視，在記錄詳細資訊方塊中。

### 管理記錄的評論

{{step1-to-planning}}

1. 按一下工作區的卡片。

   工作區隨即開啟，且記錄型別會顯示在卡片上。

1. 按一下記錄型別卡。
記錄型別頁面隨即開啟，並顯示該型別的所有記錄。

1. 從&#x200B;**檢視**&#x200B;下拉式功能表中選擇表格檢視。
1. 按一下表格檢視中的記錄名稱。

   記錄的&#x200B;**詳細資料**&#x200B;頁面隨即開啟。 「註解」區域預設會在右側面板中開啟。

1. （視條件而定）如果右面板預設未開啟，請按一下右上角的&#x200B;**顯示註解** ![顯示註解圖示](assets/show-comments-icon.png)圖示以開啟「註解」區段。

1. 開始在&#x200B;**新註解**&#x200B;方塊中輸入註解。

   ![記錄上有空白的註解方塊](assets/empty-comment-box-on-record.png)

   >[!TIP]
   >
   >在您完成輸入和提交評論之前瀏覽離開評論區段，即使您登出並重新登入，仍會將頁面上的評論保留在草稿模式。<!--this is no longer possible for records: Any images that are added to the comment are also saved in the draft. Drafts are saved for 7 days after which they are discarded and cannot be recovered. Drafted comments are only visible to the user entering them.-->

1. （可選）若要復原或重做變更，請使用下列快速鍵：
   * CTRL + Z (Mac為⌘ + z)可復原變更
   * 按CTRL + Y (Mac則為⌘ + y)以重做變更
1. （選擇性和條件性）如果您的Workfront執行個體是Adobe統一體驗的一部分，請新增&#x200B;**@**，後跟使用者名稱，以在更新中標籤某人。 如需詳細資訊，請參閱本文中關於評論記錄](#considerations-about-commenting-on-a-record)的[考量事項。

1. （可選）使用RTF工具列中的選項來格式化文字、新增emoji或連結至更新，以強化內容。

   >[!TIP]
   >
   >您無法將影像新增至錄製註解。


1. 繼續新增註解至記錄。

   如需有關更新物件的詳細資訊，包括Workfront Planning記錄，請參閱[更新工作](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md)。

1. （選擇性）按一下評論右上角的&#x200B;**更多**&#x200B;圖示![更多功能表](assets/more-menu.png)，然後按一下&#x200B;**刪除**&#x200B;以刪除評論。
1. （選擇性）按一下&#x200B;**隱藏註解**&#x200B;圖示![隱藏註解圖示](assets/hide-comments-icon.png)以關閉右側面板。

<!--
      >[!TIP]
      >
      >If another user submits a comment to the same item you are updating, there is a red line with a "New" indicator to inform you of the newer comments. 
      >
      >The indicator displays only after the comment was submitted on the item, and not when the comment is still composed. 
      >
      >![New line indicator in comments](assets/new-line-indicator-comments.png)
1. Click **Submit** to add the update to the record. 
1. (Optional) To edit a comment, click the **More** menu ![More menu](assets/more-menu.png) in the upper-right corner of the comment, then click **Edit**.
   >[!IMPORTANT]
   >
   >You can edit your comment only within 15 minutes from submitting it.  
1. Edit the information in the comment, add or remove images or remove any of the tagged users. An "edited" indicator is added to the left of the comment.
      >[!TIP]
      >
      >Comments from the current year do not display the year in the date stamp. Hovering over a timestamp displays the full date, including the year.
1. (Optional and conditional) To search for an existing comment, start typing a keyword in the search box in the upper-right corner of the **Comments** area.     
   ![Search box for comments](assets/search-box-for-comments-area.png)
1. (Optional) Click **Reply** or start typing a comment in the **Add reply ..** area, to reply to an existing comment, then follow steps 4-8 above. (**************accurate??***********)
1. (Conditional and optional) If other users have added comments that display outside of the visible area in the Comments section while you were adding your comments, click **View** inside the **new comments banner** at the bottom of the screen  to display these comments.
   ![New comments banner on record](assets/new-comments-banner-on-record.png)

    Additional comments display at the bottom of the screen.
1. (Optional) Click the **Like** icon to like an update or acknowledge that you read it. The icon updates with the number of likes.
1. (Conditional and optional) If you included additional people in your comment, click the avatars of the users included in the update to display a list of users that the comment is shared with. 
1. (Optional) Click the **More** icon ![More menu](assets/more-menu.png) in the upper-right corner of the comment and click one of the following options, to copy a information from a comment: 
    * **Copy link**: This copies a link to the comment to your clipboard.
    * **Copy body text**: This copies the text of the comment to your clipboard.
    * **Quote reply**: This copies the content of your comment into a new reply. Images are not included in the copied reply. 

    For more information, see [Update work](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md). -->

## 歷史記錄區段總覽

您可以在記錄的右側面板的「歷史記錄」區段中，檢閱對記錄所做的變更。

如需詳細資訊，請參閱[歷程記錄區段總覽](/help/quicksilver/planning/records/history-section-overview.md)。
