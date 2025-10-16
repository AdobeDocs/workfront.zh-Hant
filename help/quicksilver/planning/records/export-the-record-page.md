---
title: 匯出記錄頁面
description: 您可以將記錄的預覽或詳細資訊頁面從Adobe Workfront Planning匯出至Microsoft Word檔案。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 8de68b70-dd87-4aad-9137-980ea9fc0d69
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 0%

---

# 匯出記錄的詳細資料

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>-->


若要與可能沒有Workfront帳戶的其他人更有效率地共同作業，您可以將記錄的詳細資訊頁面匯出至Microsoft Word檔案並與他們共用。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront套件</p></td> 
   <td> 
<p>任何Workfront和任何Planning套件</p> <p>任何工作流程與任何Planning套件</p>
<p>如需每個Workfront Planning套件所含內容的詳細資訊，請聯絡您的Workfront客戶代表。 </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td><p>淺色或更高</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td>   <p>檢視或更高的工作區許可權並記錄型別</a> </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p> </td> 
  </tr> 
  </tr> 
  <tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> 必須為具有輕度或貢獻者授權的使用者指派包含Planning的版面配置範本。
   <p>標準使用者和系統管理員預設會啟用Planning區域。</p></div></li></ul>
</td>
  </tr>  
</tbody> 
</table>

如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++  

<!--Old:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td> <p>Light or higher</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>View or higher permissions to a workspace and record type</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table> 

 *For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).-->


## 匯出記錄詳細資訊的考量事項：

* 您可以將記錄的詳細資訊匯出為下列檔案格式：

   * .docx Word
   * .pdf

* 您只能匯出記錄頁面或預覽區域的詳細資訊標籤。

* 匯出的檔案會保留記錄頁面的版面，包括縮圖和封面影像。

## 匯出記錄的詳細資料

{{step1-to-planning}}

1. 按一下工作區的卡片。

   工作區隨即開啟，且記錄型別會顯示在卡片上。

1. 按一下記錄型別卡。
記錄型別頁面隨即開啟，並顯示該型別的所有記錄。

1. 從任何檢視中，按一下記錄名稱。

   記錄的預覽方塊開啟。

1. （選擇性）按一下&#x200B;**在新標籤中開啟**&#x200B;圖示![在新標籤中開啟詳細資料](assets/open-details-in-a-new-tab-icon.png)以開啟紀錄的頁面。

1. 選擇&#x200B;**詳細資料**&#x200B;標籤。 詳細資訊標籤預設為開啟。

1. 在預覽或記錄頁面中，按一下&#x200B;**匯出**&#x200B;功能表![記錄詳細資料頁面中的「匯出」圖示](assets/export-icon-in-record-details-page.png)，然後按一下下列其中一項：

   * **Microsoft Word**
   * **Adobe PDF**

   Word (.docx)或PDF檔案會下載並儲存至您的電腦。

   匯出的檔案的名稱是記錄的「主要」欄位。

   ![已匯出的Word檔案](assets/exported-word-file.png)

   >[!NOTE]
   >
   >    不會顯示在頁面上，且只會在按一下記錄詳細資訊區域中的顯示更多後顯示的其他資訊，不會顯示在匯出的PDF檔案中。 匯出的檔案中只會顯示頁面上顯示的資訊。


1. （選擇性）移至下載的檔案，開啟檔案並加以編輯（如果是Word檔案），或與其他人共用。

