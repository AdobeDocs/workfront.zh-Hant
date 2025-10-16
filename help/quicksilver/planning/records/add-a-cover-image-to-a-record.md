---
title: 新增封面影像至記錄
description: 編輯記錄時，您可以在Adobe Workfront Planning中將封面影像新增至記錄頁面，以個人化記錄。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 93c6bc15-d945-4cfc-8e87-f5b4e6fac2f4
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---


# 新增封面影像至記錄

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

編輯記錄時，您可以在Adobe Workfront Planning中將封面影像新增至記錄頁面，以個人化記錄。

如需有關編輯記錄的資訊，請參閱[編輯記錄](/help/quicksilver/planning/records/edit-records.md)。

您必須先建立記錄型別，才能開始建立和編輯記錄。

如需詳細資訊，請參閱[建立記錄型別](/help/quicksilver/planning/architecture/create-record-types.md)。

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
   <td><p>標準</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td>   <p>貢獻或更高的許可權到工作區和記錄型別  </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p> </td> 
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
<p>For more information about what is included in each Workfront Planning package, contact your Workfront account manager. </p> 
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
   <td><p> Standard</p>
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
   <td>   <p>Contribute or higher permissions to a workspace and record type  </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table> -->

## 關於紀錄頁封面影像的考量事項

您可以新增封面影像以個人化記錄頁面。

請考量下列事項：

* 封面影像隻適用於一筆記錄，不適用於相同型別的所有記錄。
* 您只能將影像檔案新增為封面影像。
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* 您可以從任何檢視的記錄預覽或記錄頁面，將封面影像新增至個別記錄。
* 您無法從記錄檢視中新增封面影像。
* 每次建立記錄時，Workfront都會自動上傳封面影像。 您稍後可以修改此影像。

## 新增封面影像至記錄

您可以在記錄預覽或頁面頂端新增封面影像，以個人化記錄。

{{step1-to-planning}}

1. 按一下要個人化其記錄的工作區，

   或

   從工作區中，展開現有工作區名稱右側的向下箭頭，搜尋工作區，然後在工作區顯示在清單中時選取該工作區。

   工作區隨即開啟，且記錄型別隨即顯示。

1. 按一下記錄型別卡。

   記錄型別頁面隨即開啟。

1. 從任何型別的檢視中，按一下記錄

   或

   從表格檢視中，按一下第一欄中的&#x200B;**開啟詳細資料**&#x200B;圖示![開啟詳細資料圖示](assets/open-details-icon-in-table-name-field.png)。

   記錄的預覽會在檢視中開啟。

   ![詳細資料預覽方塊](assets/details-box.png)


1. （選擇性）按一下記錄預覽右上角的&#x200B;**在新索引標籤中開啟**&#x200B;圖示![在新索引標籤中開啟](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it-->，以在新索引標籤中開啟記錄的頁面。

   記錄頁面隨即開啟。

   ![詳細資料頁面](assets/details-page.png)

1. 在記錄預覽或詳細資訊頁面中，將滑鼠暫留在記錄名稱上方的空白處，然後按一下&#x200B;**新增封面**。

   或

   將滑鼠停留在現有的封面影像上，按一下&#x200B;**更多**&#x200B;功能表![更多](assets/more-menu.png)，然後按一下&#x200B;**上傳**。 <!--check the casing here; I logged a bug for this-->
**唱片封面**&#x200B;方塊會在&#x200B;**上傳**&#x200B;標籤中開啟。

   ![用於上載的錄製封面盒](assets/record-cover-box-for-upload.png)

1. 按一下&#x200B;**瀏覽影像**&#x200B;並瀏覽您電腦上的圖片，以選取並新增圖片。

1. （選擇性）若要在儲存影像之前移除影像，請按一下&#x200B;**上傳新影像**&#x200B;圖示![上傳新影像圖示](assets/upload-new-image-icon.png)，然後上傳新影像。

1. （選擇性）按一下&#x200B;**影像庫**&#x200B;標籤，然後按一下影像庫中的影像。 無法修改影像庫。

   ![影像中心](assets/record-cover-box-for-gallery.png)的唱片封面盒

1. 按一下&#x200B;**使用影像**。

   影像會上傳到記錄預覽或詳細資訊頁面的頂端，且變更會自動儲存。

   ![含有封面影像的錄製頁面](assets/record-page-with-cover-image.png)

1. （選擇性）將滑鼠停留在影像上，然後按一下封面影像右下角的&#x200B;**更多**&#x200B;功能表![更多](assets/more-menu.png)，然後執行下列任一項作業：

   * 如果您要取代封面影像，並重複步驟6以上傳並儲存新影像，請按一下&#x200B;**上傳**。
   * 按一下&#x200B;**重新定位**，並使用&#x200B;**重新定位**&#x200B;工具![重新定位工具圖示](assets/reposition-tool-icon.png)將封面影像置中，然後在完成時按一下&#x200B;**儲存**。
   * 按一下&#x200B;**移除**&#x200B;以移除封面影像。

   Workfront會自動儲存您的變更。
