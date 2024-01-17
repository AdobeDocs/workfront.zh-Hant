---
product-previous: workfront-goals
navigation-topic: goal-management
title: 在Adobe Workfront目標中管理目標註解
description: 您可以將註解新增至可在Adobe Workfront目標中檢視的所有目標。
author: Alina
feature: Workfront Goals
exl-id: 6cf2d2d2-5ba5-40f2-a803-01359c338541
source-git-commit: 5f3d5c93c2fc721dda2dd04adac22190ef6a3f29
workflow-type: tm+mt
source-wordcount: '1095'
ht-degree: 0%

---

# 在Adobe Workfront目標中管理目標註解

<!--Audited: 01/2024-->

<!--consider retiring this article when goals and all objects are in parity and we remove the legacy commenting from the system. From then on, there is just ONE way to comment and that will be documented in the Update Work article-->

<!--take "legacy" and "new commenting" references out when we remove the legacy - April 2024???-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. </span>

<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](../../product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span>-->

<!--
After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>  
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>  
-->

您可以將註解新增至可在Adobe Workfront目標中檢視的所有目標。

## 存取需求

您必須具有下列存取權才能執行本文所述的動作：

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
 <td role="rowheader">Adobe Workfront計畫</td>
 <td>
 <p>任何</p>

</td>
 </tr>
 <tr>
 <td role="rowheader">Adobe Workfront授權*</td>
 <td>
 <p>新授權：投稿人或以上版本</p>
 或
 <p>目前授權：要求或以上</p> </td>
 </tr>
 <tr>
 <td role="rowheader">產品*</td>
 <td>
 <p> 新產品需求：如果您有Select或Prime Adobe Workfront計畫，您也必須購買額外的Adobe Workfront目標授權。 Workfront目標包含在最終Workfront計畫中。</p>
 或
 <p>目前產品需求：您必須為Adobe Workfront目標購買額外授權，才能存取本文所述功能。 </p> <p>如需詳細資訊，請參閱 <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">使用Workfront目標的需求</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">存取層級設定</td>
 <td> <p>檢視或更高的目標存取權</p> <p><b>附註</b><p>如果您沒有存取權，請洽詢Workfront管理員，瞭解他們是否在您的存取層級設定其他限制。 如需詳細資訊，請參閱 <span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">授予Adobe Workfront目標的存取權</a></span></td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">物件許可權</td>
 <td>
  <div>
  <p>檢視目標的或更高許可權</p>
  <p>依預設，使用者無法存取目標 </p>
 <p>如需關於共用目標的資訊，請參閱 <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">在Workfront目標中共用目標</a>. </p>
  </div> </td>
 </tr>
</tbody>
</table>

*若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。 如需詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 先決條件

開始之前，您必須具備下列條件：

* 包含主功能表中目標區域的版面配置範本。

## 管理目標註解

您可以在目標頁面的「更新」區段中，將註解新增至目標。

您可以回覆或喜歡您或其他人新增至此區域的註解。

1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) 位於右上角，或 **主要功能表** 圖示 ![](assets/lines-main-menu.png) （如果有的話）按一下 **目標**.
如此將可開啟目標清單。
1. 找到您要新增註解的目標，然後按一下其名稱以開啟目標頁面。
1. 按一下  **更新** 在左側面板中。
1. （選擇性）若要尋找現有註解，請開始輸入關鍵字 <!--or a user's name--> 在 **搜尋** 方塊右上角的 **註解** 標籤。

   ![](assets/search-field-in-updates-tab-goals.png)

   關鍵字 <!--or user--> 您搜尋的註釋會反白顯示，且包含該註釋的註釋會顯示在「更新」區段的頂端。

   <!--change the NOTE below when functionality changes-->

   >[!NOTE]
   >
   >   您必須搜尋包含在註解或回覆中的單字。 您無法搜尋已標籤的使用者或團隊。


   如需詳細資訊，請參閱 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)

1. 按一下 **x** 圖示來清除搜尋結果，並返回至完成狀態。
1. 按一下 **註解** 索引標籤更新區域的左上角。
1. 開始在 **新註解** 方塊。

   ![](assets/comment-box-empty-unshimmed.png)

   >[!TIP]
   >
   >在您完成輸入並提交評論之前離開更新區段，即使您登出並重新登入，仍會將頁面上的評論保留在草稿模式中。 加入註解的任何影像也會儲存在草稿中。 草稿會儲存7天，之後便會捨棄且無法復原。 草擬的註解僅對輸入註解的使用者可見。

1. （可選）若要復原或重做變更，請使用下列快速鍵：
   * CTRL + Z (Mac為⌘ + z)可復原變更
   * 按CTRL + Y (Mac則為⌘ + y)以重做變更
1. （可選）若要新增RTF格式至您的更新、超連結或影像，請使用RTF工具列上的任何選項或旁邊的圖示。 如需詳細資訊，請參閱 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. （選用）在 **標籤人員或團隊** 區域，開始輸入使用者或要納入此註解中的團隊的名稱或電子郵件，然後在其顯示在清單中時選取它。
1. 選取 **我的公司私有** 切換即可讓註解僅對您公司中的人員可見。

   >[!TIP]
   >
   >您必須在設定檔中指定公司，才能在更新區域使用此選項。

1. 按一下 **提交**.

   >[!TIP]
   >
   >如果其他使用者向您更新的相同專案提交評論，則會有帶有「新」指示器的紅線通知您較新的評論，而畫面底部會有藍色通知，指出新評論的數量。
   >
   >指示器只會在專案上提交註解後顯示，不會在註解仍在撰寫時顯示。
   >![](assets/real-time-new-red-indicator-unified-commenting.png)

1. （可選）若要編輯註解，請按一下 **更多** 功能表 ![](assets/more-icon.png) 按一下「讚」圖示右側，然後按一下 **編輯**.
1. 編輯註解中的資訊、新增或移除影像，或移除任何已標籤的使用者。
您可以在提交評論後15分鐘內編輯評論。 「已編輯」指標會新增至日期戳記的左側，該日期戳記會在更新註解時顯示。

   ![](assets/edited-tag-on-comment-unified-commenting.png)

   >[!TIP]
   >
   > * 系統只會在您提交原始更新時，才會產生電子郵件通知使用者您的更新。 編輯更新後不會產生電子郵件。
   >
   > * 日期戳記是原始註解的日期，而不是最新更新的日期。

1. （可選）按一下 **更多** 功能表 ![](assets/more-icon.png)，然後按一下下列任一選項，將註解中的資訊複製到剪貼簿或新回覆中：

   * **複製連結** 複製更新的連結，而不複製回覆。
   * **複製內文** 以複製更新的文字。
   * **引用回覆** 開啟新註解方塊，其中原始註解會在新回覆中引號，並標籤為區塊引號。

     如需詳細資訊，請參閱 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

1. （可選）按一下 **更多** 功能表 ![](assets/more-icon.png) ，然後按一下 **刪除** 以刪除您新增的註解。 如需詳細資訊，請參閱 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. （選用）按一下 **回覆** 若要回覆現有註解，請遵循上述步驟5至9。 如需有關回覆更新的詳細資訊，請參閱 [回覆更新](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md). <!--insure this stays accurate-->
1. （條件式與選擇性）如果其他使用者已新增註釋，且這些註釋顯示在「更新」區段的可見區域之外，請按一下 **檢視** 藍色內部 **新評論橫幅** 在熒幕底部顯示這些註解。

   ![](assets/blue-new-comments-banner-with-view-button.png)

   熒幕底部會顯示其他註解。
1. （可選）按一下 **按讚** 圖示![](assets/like-icon.png) 喜歡其他人新增的註解。 圖示會隨著喜歡的數量而更新。

1. （可選）按一下 **系統活動** 標籤以檢視系統記錄的更新。 目標更新時，Workfront會產生該更新的相關附註，並顯示在系統活動標籤中。 將結果、活動或專案新增至目標或更新時，Workfront也會記錄系統更新。 <!--ensure the casing on the tab has not changed-->

