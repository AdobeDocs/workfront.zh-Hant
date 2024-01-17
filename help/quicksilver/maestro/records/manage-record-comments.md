---
title: 管理記錄註解
description: 您可以在AdobeMaestro記錄上共同作業，方法是在記錄的「註解」區域中新增註解或回覆。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 5f3d5c93c2fc721dda2dd04adac22190ef6a3f29
workflow-type: tm+mt
source-wordcount: '991'
ht-degree: 0%

---


# 管理記錄註解

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. </span>

<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span> -->

您可以在AdobeMaestro記錄上共同作業，方法是在記錄的「註解」區域中新增註解或回覆。

## 在記錄上加上註解的考量事項

* 您可以在Maestro記錄的「註解」區段中，新增對作業記錄和分類的註解和回覆。

* 新增至連結記錄的註解不會顯示在您連結的記錄上。 例如，如果您對連結至Campaign記錄的Maestro產品記錄加上註解，該註解只會顯示在Maestro的產品記錄上，而不會顯示在您連結的Campaign記錄上。

* 您可以新增註解至由Maestro記錄與其他應用程式物件之間的連線所建立的Maestro記錄。

  例如，在連線Workfront專案與Maestro記錄後，您可以對Project Maestro記錄加上註解。 如需詳細資訊，請參閱 [連線記錄](/help/quicksilver/maestro/records/connect-records.md).

* 新增至其他應用程式中連結物件的註解不會顯示在Maestro中，而新增至Maestro中連結物件的註解不會顯示在其他應用程式中。

  例如，在Workfront中新增至專案的評論不會顯示在連結至Maestro中促銷活動的相同專案上，而且新增至Maestro專案記錄的評論不會顯示在Workfront中。

* 您可以標籤使用者，以提醒他們注意更新。 標籤的使用者不會收到應用程式內通知或有關您更新的電子郵件。 <!--this might change??-->

* 您可以從Maestro的下列區域新增記錄更新：

   * 從「詳細資訊」頁面。

  <!--* From the table view.-->

## 存取需求

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
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront合約</p></td>
   <td>
<p>貴組織必須註冊AdobeMaestro封閉測試版計畫。 請聯絡您的客戶代表以查詢此新產品/服務。 </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront計畫</p></td>
   <td>
<p>任何</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront授權</p></td>
   <td>
   <p>任何</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>存取層級設定</p></td>
   <td> <p>Maestro中沒有存取層級控制項。 </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>權限</p></td>
   <td> <p>檢視或更高的工作區許可權</a> </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> <p>您的Workfront或群組管理員必須在您的版面配置範本中新增Maestro區域。 如需詳細資訊，請參閱 <a href="../access/access-overview.md">存取權總覽</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

### 管理記錄的評論

{{step1-to-maestro}}

預設會開啟上次存取的工作區。
1. 從中選擇表格檢視 **檢視** 下拉式功能表。
1. 按一下表格檢視中的記錄名稱。

   記錄的 **詳細資料** 頁面隨即開啟。 「註解」區域預設會在右側面板中開啟。

1. 開始在 **新註解** 方塊。

   ![](assets/empty-comment-box-on-record.png)

   >[!TIP]
   >
   >在您完成輸入和提交評論之前瀏覽離開評論區段，即使您登出並重新登入，仍會將頁面上的評論保留在草稿模式。 加入註解的任何影像也會儲存在草稿中。 草稿會儲存7天，之後便會捨棄且無法復原。 草擬的註解僅對輸入註解的使用者可見。

1. （可選）若要復原或重做變更，請使用下列快速鍵：
   * CTRL + Z (Mac為⌘ + z)可復原變更
   * 按CTRL + Y (Mac則為⌘ + y)以重做變更
1. （可選）新增 **@** 後接在更新中標籤某人的使用者名稱。
1. （可選）使用RTF工具列中的選項來格式化文字、新增emoji、連結或影像至更新，以強化內容。 如需詳細資訊，請參閱文章中的「在Workfront更新中使用RTF文字」一節 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

   >[!TIP]
   >
   >如果其他使用者向您更新的相同專案提交評論，則會出現一條帶有「新」指示器的紅線，以通知您較新的評論。
   >
   >指示器只會在提交專案的註解後顯示，不會在註解仍在撰寫時顯示。
   >
   >![](assets/new-line-indicator-comments.png)

1. 按一下 **提交** 以將更新新增至記錄。
1. （可選）若要編輯註解，請按一下 **更多** 功能表 ![](assets/more-menu.png) 在註解的右上角，然後按一下 **編輯**.

   >[!IMPORTANT]
   >
   >您只能在提交評論的15分鐘內編輯評論。

1. 編輯註解中的資訊、新增或移除影像，或移除任何已標籤的使用者。 「已編輯」指標會新增至註解的左側。

   >[!TIP]
   >
   >目前年份的評論不會在日期戳記中顯示年份。 將游標暫留在時間戳記上會顯示完整日期，包括年份。

1. （選擇性和條件性）若要搜尋現有的註解，請在 **註解** 區域。

   ![](assets/search-box-for-comments-area.png)

1. （選用）按一下 **回覆** 或開始在 **新增回覆……** 區域，回覆現有的評論，然後遵循上述步驟4到8。 <!--(**************accurate??***********)-->

1. （條件式與選擇性）如果您在加入註解時，其他使用者已新增註解，且註解顯示在「註解」區段的可見區域之外，請按一下 **檢視** 內部 **新評論橫幅** 在熒幕底部顯示這些註解。

   ![](assets/new-comments-banner-on-record.png)

   熒幕底部會顯示其他註解。

1. （可選）按一下 **按讚** 圖示喜歡更新或確認您已閱讀該更新。 圖示會隨著喜歡的數量而更新。
1. （有條件且選用）如果您在評論中納入其他人員，請按一下更新中包含之使用者的頭像，以顯示共用評論的使用者清單。
1. （可選）按一下 **更多** 圖示 ![](assets/more-menu.png) 在註解的右上角，按一下下列其中一個選項，即可從註解中複製資訊：

   * **複製連結**：這會將註解的連結複製到剪貼簿。
   * **複製內文** t：這會將註解的文字複製到剪貼簿。
   * **引用回覆**：這會將您評論的內容複製到新回覆中。 複製的回覆中不包含影像。

   如需詳細資訊，請參閱 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. （可選）按一下 **更多** 圖示 ![](assets/more-menu.png) 在註解的右上角，然後按一下 **刪除** 以刪除註解。

