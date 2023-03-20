---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 更新工作
description: 您可以在Adobe Workfront物件（專案、任務或問題）上新增更新，以傳達物件進度的相關資訊。 已指派或訂閱物件的使用者可以檢視您的更新。 您也可以標籤使用者，以吸引其注意更新。
author: Alina
feature: Get Started with Workfront
exl-id: 0f4d6895-6326-4a83-9bbc-bb58c876e7fc
source-git-commit: 4b1a82758a7e3c745e622ddbab4b0651a6b35a33
workflow-type: tm+mt
source-wordcount: '2690'
ht-degree: 1%

---

# 更新工作

<!--take "Beta" references out when we remove the beta-->

<span class="preview">本頁強調顯示的資訊指的是尚未普遍提供的功能。 它僅在預覽環境中可用。</span>

>[!NOTE]
>
>我們目前正在重新設計使用對象的「更新」(Updates)部分時更新工作的方式。
>
>您可以啟用注釋測試版，以存取新設計。
>
>目前，測試版適用於 <span class="preview">問題</span>.
>
>如需新更新體驗的詳細資訊，請參閱 [全新評論體驗](../updating-work-items-and-viewing-updates/unified-commenting-experience.md).

您可以在「更新」區段中，為Adobe Workfront中的大部分物件新增註解。 有關哪些對象顯示「更新」部分的詳細資訊，請參閱 [更新區段概觀](../updating-work-items-and-viewing-updates/updates-tab-overview.md).

您可以在對物件加上註解時，對Workfront物件（專案、任務或問題）新增更新，以傳達物件上的進度。 已指派或訂閱物件的使用者可以檢視您的更新。 您也可以標籤使用者，以吸引其注意更新。 經過標籤的使用者會收到應用程式內通知，以及您更新的相關電子郵件。

本頁的資訊說明如何對Workfront物件加上註解，以及如何更新專案、工作和問題。 如需關於評論目標的資訊，請參閱 [管理Adobe Workfront目標中的目標註解](../../workfront-goals/goal-management/manage-goal-comments.md). 您必須有額外的授權才能存取Workfront Targets。


您可以從下列Workfront區域新增專案、工作和問題的更新：

* 從Workfront物件，在「更新」區段中
* 從首頁（針對任務和問題）
* 從對象清單中的「摘要」面板（針對任務和問題）
* 從時間表（針對任務和問題）

## 存取需求

<!--
drafted for P&P release:
<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan*</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license*</strong></td> 
   <td> <p>Current license: Contributor or higher for issues and documents: Light or higher for all other objects</p> 
   Or
   <p>Legacy  license: Request or higher for issues and documents; Review or higher for all other objects</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configurations*</strong></td> 
   <td> <p>View or Edit access for the object the update is on</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Object permissions</strong></td> 
   <td> <p>View access to the object</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront計畫*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront授權*</strong></td> 
   <td> <p>要求或更高的問題和檔案；查看其他所有對象的或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>訪問級別配置*</strong></td> 
   <td> <p>查看或編輯更新所在對象的訪問</p> <p><b>附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader"><strong>物件權限</strong></td> 
   <td> <p>檢視物件的存取權</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 向工作項添加更新

<!--drafted for the commenting experience - change the NOTE at the top of the following section with every new release to other objects -->

根據「更新」部分的版本和您選擇的對象，向工作項添加更新會有所不同。

### 將更新添加到當前更新部分中的工作項

>[!NOTE]
>
>除了目標之外，所有對象都可使用以下功能。 您必須有額外的授權才能存取Workfront Targets。 如需關於評論目標的資訊，請參閱 [管理Adobe Workfront目標中的目標註解](../../workfront-goals/goal-management/manage-goal-comments.md)

1. 轉到要為其提供更新的工作項（如項目、任務或問題）。
1. 按一下 **更新** 區段。
1. 按一下 **開始新更新，** 然後輸入更新。
1. （可選）使用RTF，或在更新中新增表情符號、連結或影像，以增強您的內容。 如需詳細資訊，請參閱本文的「在Workfront更新中使用RTF」一節
1. （可選）更新有關工作項的以下任何資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>通知</strong></td> 
      <td>識別必須通知更新的使用者。 指派或訂閱物件的使用者會在進行更新時自動收到通知。<br><p>如需如何在更新中納入其他項目的相關資訊，請參閱 <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">在更新時標籤其他人</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>認可日期</strong></td> 
      <td>在日期選擇器中，選擇要完成工作項的提交日期。 有關提交日期的資訊，請參見 <a href="../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">提交日期概述</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>狀況</strong></td> 
      <td>為任務或問題選擇新條件。 如需選取條件的相關資訊，請參閱 <a href="../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">更新任務和問題的條件</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>狀態</strong></td> 
      <td>按一下目前狀態旁的箭頭，然後從下拉式功能表中選取所需的狀態。 有關設定狀態的資訊，請參閱 <a href="../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">更新任務狀態</a>.<p>更新工作項的狀態不會自動更改項目的狀態。 根據專案的設定方式，您可能必須個別更新專案狀態。 如需各種專案更新類型的詳細資訊，請參閱 <a href="../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">選擇項目更新類型 </a>.</p><p><b>附註</b>

   工作項目處於「待批准」狀態時，無法更改其狀態。</p></td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>完成欄</strong></td> 
      <td>（僅適用於任務）通過將進度條滑動到所需百分比來指示已完成工作的百分比。 您也可以按兩下完成列，然後輸入完成百分比。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>成為我公司所私有</strong></td> 
      <td> <p>停用此選項可防止公司外部的使用者存取檢視此更新。</p> 
      <p><b>附註</b></p>
      <p>只有當使用者與公司相關聯時，才會顯示此選項。</p>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **更新** 將更新新增至Workfront物件。

   >[!NOTE]
   >
   >按一下「 」後，小型快顯視窗會顯示七秒 **更新**，可讓您在發佈更新之前還原更新並返回編輯窗格。 如果您關閉還原快顯視窗、等待其消失或導覽離開頁面，則會發佈更新。
   >
   >如果您的Workfront管理員在您的存取層級中選取「絕不允許使用者刪除留言」設定，便無法還原留言。 如需詳細資訊，請參閱 [建立和修改自定義訪問級別](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

1. 若要回覆更新，請參閱 [回覆更新](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md).

### 使用註解測試版體驗將更新新增至工作項目


>[!NOTE]
>
>本節中描述的功能適用於以下對象：
>
>* <span class="preview">問題：當您啟用評論測試版體驗時。</span>
   >
   >   <span class="preview">此功能僅適用於問題的「更新」區段，不適用於下列區域：</span>
   >
   >   * <span class="preview">首頁</span>
   >   * <span class="preview">清單中的摘要面板</span>
   >   * <span class="preview">工時單中的「摘要」面板</span>
>* 目標

   >
   >   新的註解體驗是目標的預設目前體驗。
   >   您必須有額外的授權才能存取Workfront Targets。 如需詳細資訊，請參閱 [使用Workfront目標的需求](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).



1. 找出您要更新的物件，然後按一下其名稱以開啟物件的頁面。
1. 按一下  **更新** 中。
1. <span class="preview">按一下 **試用注釋測試版** 按鈕（位於「更新」區域的右下角），然後按一下 **同意** 測試版協定。 這會將「更新」區域切換為註解測試版體驗。 </span>
此 
**註解** 標籤。
1. 開始在 **新留言** 框。

   ![](assets/comment-box-empty-unshimmed.png)

   >[!TIP]
   >
   >在您完成輸入並提交注釋之前，從「更新」部分導航離開該頁面，即使您註銷並重新登錄後，該頁面上的注釋仍以草稿模式保留。 起草的注釋只對輸入它們的用戶可見。

1. （選用）在 **標籤人員或團隊** 區域中，開始鍵入用戶的名稱或電子郵件，或要包含在此注釋中的團隊，然後在清單中顯示時選擇它。
1. （可選）若要將RTF格式新增至更新，請使用 **RTF** 工具列來增強文字：

   * 粗體
   * 斜體
   * 底線
   * 連結
   * 項目符號清單
   * 編號清單
   * 添加附件 <!--(mark this parenthesis as draft: ************ this might be renamed to "Add image")-->

   如需詳細資訊，請參閱本文的「在Workfront更新中使用RTF」一節。 <!--remove this list, above, when we get to parity for Rich Text-->

   <!--not available yet in preview - should be live with production: format this as a TIP: 
      * If another user submits a comment to the same item you are updating, there will be a red line with a "New" indicator to inform you of the newer comments. 
      * The indicator only displays only after the comment was submitted on the item, and not when the comment is still composed. 
      * The "New" indicator displays only when both the user that entered a new update as well as the user who is currently entering an update are using the new commenting experience. 
      ![](assets/real-time-new-red-indicator-unified-commenting.png)-->

1. 按一下 **提交** 將更新新增至Workfront物件。
1. （選用）若要編輯留言，請按一下 **更多** 功能表 ![](assets/more-menu.png) 在「贊」圖示的右側，然後按一下 **編輯**.
1. 編輯注釋中的資訊，或刪除任何標籤的用戶。
您可以在15內編輯意見，提交後即可。 更新註解時，會在顯示的日期戳記左側新增「已編輯」指標。

   ![](assets/edited-tag-on-comment-unified-commenting.png)

   >[!TIP]
   >
   >   系統只會在您提交原始更新時，產生電子郵件，通知使用者您的更新。 編輯更新後不會產生任何電子郵件。
1. （選用）按一下 **回覆** 若要回覆現有意見，請遵循上述步驟4至7。 <!--(**************insure this stays accurate***********)-->. 如需回覆更新的相關資訊，請參閱 [回覆更新](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md).
1. （選用）按一下 **贊** 圖示![](assets/like-icon.png). 圖示會隨按贊次數更新。
1. （條件式和可選）如果注釋中包括了其他人員，請按一下更新中包括的成員數，以顯示您輸入的注釋被共用的實體清單。

   ![](assets/members-icons-expanded-unshimmed.png)
1. （選用）按一下 **系統活動** 頁簽查看系統記錄的更新。 更新對象或其任何子項時，Workfront會生成有關該更新的附註，並在「系統活動」頁簽中顯示該更新。

   如需詳細資訊，請參閱 [更新區段概觀](../updating-work-items-and-viewing-updates/updates-tab-overview.md)

   >[!TIP]
   >
   >無法向系統更新添加註釋。


## 在Workfront更新中使用RTF

<!--remove this top note when we get to parity with the current version, OR change the note to mention that some options are ONLY available in the Beta version and not the current one.-->

>[!NOTE]
>
>RTF工具列中的某些選項可能無法用於評論測試版體驗。

您可以使用RTF來增強更新，或是新增各種項目，例如表情符號、連結或影像。

1. 前往「更新」區域，開始輸入註解。
1. （可選）若要將RTF格式新增至更新，請在 **RTF** 工具欄。

   | **屬性** | **工具欄按鈕** | **Mac快捷鍵** | **PC快捷鍵** |
   |---|---|---|---|
   | 粗體 | ![mceclip10.png](assets/mceclip10.png) | ⌘+b | Ctrl+B |
   | 斜體 | ![mceclip9.png](assets/mceclip9.png) | ⌘+i | Ctrl+I |
   | 底線 | ![mceclip8.png](assets/mceclip8.png) | ⌘+u | Ctrl+U |
   | 超連結 | ![mceclip7.png](assets/mceclip7.png) | ⌘+K | Ctrl+K |
   | 項目符號清單 | ![mceclip6.png](assets/mceclip6.png) | ⌘+Shift+8 | Ctrl+Shift+8 |
   | 編號清單 | ![mceclip5.png](assets/mceclip5.png) | ⌘+Shift+7 | Ctrl+Shift+7 |
   | 封鎖報價 | ![](assets/block-quote-icon-large.png) | ⌘+Shift+9 | Ctrl+Shift+9 |

   若要停止格式化文字，請取消選取 **RTF** 工具欄。

   >[!NOTE]
   >
   >* 使用者收到的包含您更新的任何電子郵件通知中也會顯示格式設定。
   >* 在「更新」標籤中檢視時，套用至電子郵件中更新的RTF格式不會顯示在更新上。
   >* 如果貴組織使用Workfront搭配Internet Explorer，貼上至更新中的任何格式化文字都會遺失其RTF格式，並顯示為純文字。 您可以使用RTF工具列上的屬性來重新格式化文字。
   >* 在「時間表」區域中進行的更新，或在報表中查看的「注釋」和「最後一個條件」對象時，RTF格式不可用。


1. （可選）如果要包括來自先前更新或來自其他來源的文本，並將其與您自己的更新區分開來，您可以將其標籤為塊報價。 按一下 **塊報價** 圖示 ![](assets/block-quote-small.png) 並輸入要引用的文本。 引用的文本顯示為垂直灰線。 按一下 **塊報價** 表徵圖以返回到正常格式。

   ![](assets/block-quote-marked-350x144.png)

1. （選用）將表情符號新增至更新。

   >[!NOTE]
   >
   >* Workfront不會將標點符號的表情符號（例如：）取代為emoji。
   >* 在「時間表」區域中進行的更新或在報表中查看的「注釋」和「最後條件」對象不提供表情符號。
   >* Workfront中的emoji功能採用Unicode字元，因此，只會在支援Unicode代碼點的瀏覽器和作業系統上顯示。 平台、瀏覽器或作業系統版本與您不同的使用者可能無法存取相同的表情符號。
   >* 不支援的表情符號會以黑色或白色方塊表示。
   >* Windows 7僅支援黑白表情符號。
   >* 套用至透過電子郵件進行之更新的表情符號，在「更新」區域中檢視時不會顯示在更新上。


1. （選用）若要新增URL連結至其他資訊來源：

   1. 按一下您要插入連結的更新中的。
   1. 在 **RTF** 工具欄，按一下 **超連結** 表徵圖。 ![](assets/link-icon.png)

   1. 在 **建立連結** 框，位於 **URL**，輸入或貼上您要連結之來源的URL。

   1. 在 **要顯示的文字**，輸入或貼上連結文字。
   1. 按一下&#x200B;**儲存**。

1. （可選）若要將影像附加至更新，請按一下 **影像** 圖示 ![](assets/addimageicon-35x32.png) 並瀏覽到電腦上的影像。\
   或\
   將影像拖曳至更新區域。

   >[!NOTE]
   >
   >* 您的Workfront管理員必須先啟用新增影像，您才能看到影像圖示。
   >* 最大影像檔案大小為7 MB。 支援的影像檔案類型為.jpg、.gif和.png。
   >* 影像只能從對象的「更新」(Updates)頁簽中訪問，而「文檔」(Documents)頁簽中不提供影像。
   >* 您可以傳送包含影像且無文字的更新。

1. 按一下 **更新**  <span class="preview">或 **提交**</span>，即可在評論測試版體驗中取得。


## 複製更新資訊

<!--drafted for beta release toggle - remove when copying an update will be available:-->

>[!NOTE]
>
>使用測試版注釋體驗時無法複製更新。

您可以透過數種方式複製更新。 複製連結後，您可以與其他人共用連結，將他們導向更新。

* [複製更新](#copy-the-update)
* [複製線程連結](#copy-the-thread-link)
* [複製更新連結](#copy-the-update-link)

### 複製更新 {#copy-the-update}

此選項會將特定更新的文字複製到剪貼簿。

1. 前往要複製的更新或回覆。
1. 按一下 **更多** ，然後按一下 **複製正文文本**.

   ![選擇複製正文文本](assets/update-stream-copy-body-text-350x152.png)

### 複製線程連結 {#copy-the-thread-link}

此選項會將完整線程連結複製到剪貼簿，以便您可以與其他用戶共用線程。

1. 轉到要複製的更新線程。
1. 按一下 **更多** ，然後按一下 **複製線程連結**.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

### 複製更新連結 {#copy-the-update-link}

此選項會將特定更新連結複製到剪貼簿。 當您共用更新連結時，跟隨該連結的使用者會在更新周圍看到邊框。

1. 前往要複製的更新或回覆。
1. 按一下 **更多** 功能表，然後按一下 **複製更新連結**.

   ![](assets/update-stream-reply-menu-marked-350x182.png)

## 刪除更新或回覆

根據您的Workfront管理員提供的存取權，您可能可以刪除您在物件的「更新」標籤上新增的更新。 如需詳細資訊，請參閱 [建立或修改自訂存取層級](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) 在文章中 [建立或修改自訂存取層級](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

任何Workfront使用者(包括Workfront管理員)都無法刪除其他使用者進行的更新。 不過，如果使用者的存取層級允許他們刪除自己的更新，Workfront管理員可以以該使用者的身分登入，並刪除他們所做的更新。 如需詳細資訊，請參閱 [建立或修改自訂存取層級](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md#creating-a-new-access-from-scratch) 和 [以其他使用者身分登入](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

1. 前往要刪除的更新或回覆。
1. 按一下 **更多** 功能表（在您要刪除的更新或回覆旁邊），然後按一下 **刪除**.

   ![](assets/update-stream-comment-menu-marked-350x152.png)

1. 在顯示的訊息中，按一下 **確認** <span class="preview">或 **刪除**</span>，即可在評論測試版體驗中取得。

>[!NOTE]
>
>刪除含有附加影像的更新會刪除註解和影像。

## 在時間表上添加更新

1. 轉到要對其進行更新的時間表。
1. 按一下時間表以開啟它。
1. 在工時單底部，按一下 **包括注釋**.
1. 在顯示於時間表底部的框中，鍵入更新。

   ![timestee_update_stream.png](assets/timesheet-update-stream-350x50.png)

1. （條件性）要保存更新而不提交時間表進行批准，請按一下 **保存以供稍後使用**.

   或

   要保存更新並提交時間表以進行批准，請按一下 **提交以進行核准**.

   或

   如果未與批准者設定工時單，請按一下 **保存並關閉工時單** 以保存更新。

## 啟用或禁用系統更新

<!--remove the preview tag with 23.2 production, but keep the note till we remove Beta and it becomed the only exprience: -->



>[!NOTE]
>
><span class="preview">使用測試版注釋體驗時，無法停用系統更新。 </span>
><span class="preview">本節中的資訊僅指目前更新區段中提供的功能。 </span>
><span class="preview">有關測試版中系統更新的詳細資訊，請參閱 [更新區段概觀](../updating-work-items-and-viewing-updates/updates-tab-overview.md). </span>


Workfront物件的「更新」區段會顯示兩種資訊：

* **用戶更新：** 用戶更新是您和系統中的其他用戶輸入的注釋。

   ![](assets/user-update-cl-350x277.png)

* **系統更新：** 系統更新記錄刪除資產、添加或刪除版本、附加或刪除批准請求以及對對象上的文檔所做的任何編輯或更改。

   ![](assets/system-updates-cl-350x277.png)

視您的Workfront授權而定，系統更新可能會預設啟用。 Workfront管理員可判斷系統更新中追蹤的項目，如 [系統追蹤更新](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md). 您也可以篩選掉系統更新或活動，以便只看到所有對象的用戶更新。

有關用戶和系統更新之間差異的詳細資訊，請參見 [系統追蹤更新](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

要啟用或禁用系統更新，請執行以下操作：

1. 按一下 **更新** 標籤。
1. 按一下 **顯示系統更新** 左滑（禁用）或右滑（啟用）。

   ![](assets/show-system-updates-qs-350x55.png)

   此選項會持續存在於整個Workfront的所有物件中，且即使您登出Workfront，仍保留在您選取的位置。

