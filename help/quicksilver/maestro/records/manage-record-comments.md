---
title: 管理記錄註解
description: 您可以在AdobeMaestro記錄的「註解」區域新增更新並詢問問題或回覆，以進行共同作業。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 3ffb6fdebb54682abc737e55186850458a133f7c
workflow-type: tm+mt
source-wordcount: '957'
ht-degree: 0%

---


<!--update the metadata with real information when making this available in TOC and in the left nav-->

# 管理記錄註解

您可以在AdobeMaestro記錄上合作，方法是新增更新並在記錄的「註解」區域中詢問問題或回覆。

## 在記錄上加上註解的考量事項

* 您可以在Maestro記錄的「註解」區段中，新增對作業記錄和分類的註解和回覆。

* 新增至連結記錄的註解不會顯示在您連結的記錄上。 例如，如果您對連結至Campaign記錄的專案進行註解，該註解只會顯示在Maestro中的專案記錄上，而不會顯示在您連結的促銷活動記錄上。

* 新增至其他應用程式中連結物件的註解不會顯示在Maestro中。
新增至Maestro中連結物件的註解不會顯示在其他應用程式中。\
  例如，在Workfront中新增至專案的評論不會顯示在連結至Maestro中行銷活動的相同專案上。

* 您可以標籤使用者，以提醒他們注意更新。 標籤的使用者不會收到應用程式內通知或有關您更新的電子郵件。 您無法在Maestro註解中標籤團隊。

  >[!TIP]
  >
  >* 評論擁有者不會在更新中自動標籤。
  >
  >* 當您回覆更新時，無法從更新中移除已標籤的使用者。

* 您可以從Maestro的下列區域新增記錄更新：

   * 從「詳細資訊」頁面。

  <!--* From the table view.-->

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> Adobe產品</p> </td>
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
   <td role="rowheader">存取層級</td>
   <td> <p>任何</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">版面配置範本</td>
   <td> <p>您的系統管理員必須在您的版面配置範本中新增Maestro區域。 如需詳細資訊，請參閱 <a href="../access/grant-access.md">授與Adobe大師的存取權</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--
After permissions - replace the table with: **************CHECK ON THE VIEW PERMISSIONS TO THE WORKSPACE; RIGHT NOW, WE SAY THAT VIEW USERS CAN COMMENT BUT THE PAGE BLOWS OUT WHEN I TRY - ASKED PM TO CONFIRM*****************

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/grant-access.md">Grant access to Adobe Maestro</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>View or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

-->


<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

### 管理記錄的評論

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](assets/dots-main-menu.png) 在Adobe Workfront的右上角，或（如果有的話）按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](assets/lines-main-menu.png) 然後按一下「 」 **[!UICONTROL 大師]**.

   預設會開啟上次存取的工作區。
1. 從中選擇表格檢視 **檢視** 下拉式功能表。
1. 按一下表格檢視中的記錄名稱。

   記錄的 **詳細資料** 頁面隨即開啟。

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

