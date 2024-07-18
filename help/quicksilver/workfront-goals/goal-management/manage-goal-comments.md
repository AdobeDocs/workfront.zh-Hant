---
product-previous: workfront-goals
navigation-topic: goal-management
title: 在Adobe Workfront目標中管理目標註解
description: 您可以將註解新增至可在Adobe Workfront目標中檢視的所有目標。
author: Alina
feature: Workfront Goals
exl-id: 6cf2d2d2-5ba5-40f2-a803-01359c338541
source-git-commit: 52e8ce6dd5146d72f698583b531b3db6bc5dbf25
workflow-type: tm+mt
source-wordcount: '1092'
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
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> 
   <p>對於新計畫和授權結構：
  <ul><li>終極計畫 </li>
  或
  <li>適用於Prime或選取Adobe Workfront計畫的Adobe Workfront目標的其他授權。 </li></ul> </p>
<p>對於目前的計畫與授權結構： 
<ul><li> A Pro或更高版本 </li>
  <li>除了Adobe Workfront授權之外，還有Workfront目標授權。</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront授權</td>
 <td>
 <p>任何</td>
 </tr>
 <tr>
 <td role="rowheader">產品*</td>
 <td>
 <p> 新產品需求：如果您有Select或Prime Adobe Workfront計畫，您也必須購買額外的Adobe Workfront目標授權。 Workfront目標包含在最終Workfront計畫中。</p>
 或
 <p>目前產品需求：您必須為Adobe Workfront目標購買額外授權，才能存取本文所述功能。 </p> <p>如需詳細資訊，請參閱<a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">使用Workfront目標的需求</a>。 </p> </td>
 </tr>
 <tr>
 <td role="rowheader">存取層級設定</td>
 <td> <p>檢視或更高的目標存取權</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">物件許可權</td>
 <td>
  <div>
  <p>檢視目標的或更高許可權</p>
  <p>依預設，使用者無法存取目標 </p>
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

## 先決條件

開始之前，您必須具備下列條件：

* 包含主功能表中目標區域的版面配置範本。

## 管理目標註解

您可以在目標頁面的「更新」區段中，將註解新增至目標。

您可以回覆或喜歡您或其他人新增至此區域的註解。

1. 按一下右上角的&#x200B;**主功能表**&#x200B;圖示![](assets/main-menu-icon.png)，或左上角的&#x200B;**主功能表**&#x200B;圖示![](assets/lines-main-menu.png) （如果有的話），然後按一下&#x200B;**目標**。
如此將可開啟目標清單。
1. 找到您要新增註解的目標，然後按一下其名稱以開啟目標頁面。
1. 按一下左側面板中的&#x200B;**更新**。
1. （選擇性）若要尋找現有的註解，請在&#x200B;**註解**&#x200B;索引標籤右上角的&#x200B;**搜尋**&#x200B;方塊中開始輸入關鍵字<!--or a user's name-->。

   ![](assets/search-field-in-updates-tab-goals.png)

   您搜尋的關鍵字<!--or user-->會反白顯示，而且包含該關鍵字的註解會顯示在「更新」區段的頂端。

   <!--change the NOTE below when functionality changes-->

   >[!NOTE]
   >
   >您必須搜尋包含在註解或回覆中的單字。 您無法搜尋已標籤的使用者或團隊。

   如需詳細資訊，請參閱[更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)。

1. 按一下搜尋欄位中的&#x200B;**x**&#x200B;圖示以清除搜尋結果並返回完整更新。
1. 按一下[更新]區域左上角的&#x200B;**註解**&#x200B;標籤。
1. 開始在&#x200B;**新註解**&#x200B;方塊中輸入註解。

   ![](assets/comment-box-empty-unshimmed.png)

   >[!TIP]
   >
   >在您完成輸入並提交評論之前離開更新區段，即使您登出並重新登入，仍會將頁面上的評論保留在草稿模式中。 草稿會儲存7天，之後便會捨棄且無法復原。 草擬的註解僅對輸入註解的使用者可見。

1. （可選）若要復原或重做變更，請使用下列快速鍵：
   * CTRL + Z (Mac為⌘ + z)可復原變更
   * 按CTRL + Y (Mac則為⌘ + y)以重做變更
1. （可選）若要新增RTF格式至您的更新、超連結或Emoji，請使用RTF工具列上的任何選項或旁邊的圖示。 如需詳細資訊，請參閱[更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)。
1. （選擇性）在&#x200B;**標籤人員或團隊**&#x200B;區域，開始輸入使用者或您要加入此註解之團隊的名稱或電子郵件，然後在其顯示在清單中時選取它。
1. 選取&#x200B;**我的公司私人**&#x200B;切換按鈕，讓註解僅對您公司中的人員可見。

   >[!TIP]
   >
   >您必須在設定檔中指定公司，才能在更新區域使用此選項。

1. 按一下&#x200B;**提交**。

   >[!TIP]
   >
   >如果其他使用者向您更新的相同專案提交評論，則會有帶有「新」指示器的紅線通知您較新的評論，而畫面底部會有藍色通知，指出新評論的數量。
   >
   >指示器只會在專案上提交註解後顯示，不會在註解仍在撰寫時顯示。
   >![](assets/real-time-new-red-indicator-unified-commenting-copy.png)

1. （選擇性）若要編輯評論，請按一下[贊]圖示右側的&#x200B;**更多**&#x200B;功能表![](assets/more-icon.png)，然後按一下&#x200B;**編輯**。
1. 編輯註解中的資訊或移除任何已標籤的使用者。
您可以在提交評論後15分鐘內編輯評論。 「已編輯」指標會新增至日期戳記的左側，該日期戳記會在更新註解時顯示。

   ![](assets/edited-tag-on-comment-unified-commenting.png)

   >[!TIP]
   >
   > * 系統只會在您提交原始更新時，才會產生電子郵件通知使用者您的更新。 編輯更新後不會產生電子郵件。
   >
   > * 日期戳記是原始註解的日期，而不是最新更新的日期。

1. （選擇性）按一下&#x200B;**更多**&#x200B;功能表![](assets/more-icon.png)，然後按一下下列任一選項，將註解中的資訊複製到剪貼簿或新回覆中：

   * **複製連結**&#x200B;以複製更新的連結，而不使用回覆。
   * **複製內文**&#x200B;以複製更新的文字。
   * **引用回覆**&#x200B;開啟新註解方塊，其中原始註解會在新回覆中引用並標示為區塊引用。

     如需詳細資訊，請參閱[更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)。

1. （選擇性）按一下評論右邊的&#x200B;**更多**&#x200B;功能表![](assets/more-icon.png)，然後按一下&#x200B;**刪除**&#x200B;以刪除您新增的評論。 如需詳細資訊，請參閱[更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)。
1. （選擇性）按一下&#x200B;**回覆**&#x200B;回覆現有註解，然後依照上述步驟5-9進行。 如需回覆更新的詳細資訊，請參閱[回覆更新](../../workfront-basics/updating-work-items-and-viewing-updates/reply-to-updates.md)。<!--insure this stays accurate-->
1. （條件式及選擇性）如果其他使用者新增的註解顯示在[更新]區段的可見區域之外，請按一下畫面底部的藍色&#x200B;**新註解橫幅**&#x200B;中的&#x200B;**檢視**&#x200B;以顯示這些註解。

   ![](assets/blue-new-comments-banner-with-view-button.png)

   熒幕底部會顯示其他註解。
1. （選擇性）按一下&#x200B;**贊**&#x200B;圖示![](assets/like-icon.png)喜歡其他人新增的註解。 圖示會隨著喜歡的數量而更新。

1. （選擇性）按一下&#x200B;**系統活動**&#x200B;索引標籤，以檢視系統記錄的更新。 目標更新時，Workfront會產生該更新的相關附註，並顯示在系統活動標籤中。 將結果、活動或專案新增至目標或更新時，Workfront也會記錄系統更新。<!--ensure the casing on the tab has not changed-->


