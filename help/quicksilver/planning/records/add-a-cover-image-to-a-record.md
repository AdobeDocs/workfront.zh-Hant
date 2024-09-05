---
title: 新增封面影像至記錄
description: 編輯記錄時，您可以在Adobe Workfront Planning中將封面影像新增至記錄頁面，以個人化記錄。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 93c6bc15-d945-4cfc-8e87-f5b4e6fac2f4
source-git-commit: bd202821687453288c96147933331c8a7a6b3acb
workflow-type: tm+mt
source-wordcount: '697'
ht-degree: 1%

---


# 新增封面影像至記錄

{{planning-important-intro}}

編輯記錄時，您可以在Adobe Workfront Planning中將封面影像新增至記錄頁面，以個人化記錄。

如需有關編輯記錄的資訊，請參閱[編輯記錄](/help/quicksilver/planning/records/edit-records.md)。

您必須先建立記錄型別，才能開始建立和編輯記錄。

如需詳細資訊，請參閱[建立記錄型別](/help/quicksilver/planning/architecture/create-record-types.md)。

## 存取需求

+++ 展開以檢視Workfront Planning的存取需求。

您必須具備下列專案才能存取Workfront Planning：

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
   <td role="rowheader"><p>Adobe Workfront規劃計畫*</p></td> 
   <td> 
<p>任何 </p> 
<p>如需每個Workfront計畫包含內容的詳細資訊，請聯絡您的Workfront客戶經理。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront平台</p></td> 
   <td> 
<p>貴組織的Workfront例項必須加入Adobe統一體驗，才能存取Workfront規劃的所有功能。</p> 
<p>如需詳細資訊，請參閱<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront的Adobe統一體驗</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權*</p></td> 
   <td><p> 標準</p>
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
   <td>   <p>管理工作區的許可權 </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>版面配置範本</p></td> 
   <td> <p>必須為所有使用者(包括Workfront管理員)指派一個版面配置範本，該範本包含主功能表中的Planning區域。 </p> </td> 
  </tr> 
</tbody> 
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


<!--

OLD: 
<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>  
   <p>Current: Plan</p>   
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access controls for Workfront Planning </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td>  <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu. </p> <p>For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For more information, see [Access requirements in Workfornt documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->

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

   從表格檢視中，按一下第一欄中的&#x200B;**開啟詳細資料**&#x200B;圖示![](assets/open-details-icon-in-table-name-field.png)。

   記錄的預覽會在檢視中開啟。

   ![](assets/details-box.png)

1. （選擇性）按一下記錄預覽右上角的&#x200B;**在新索引標籤中開啟**&#x200B;圖示![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it-->，以在新索引標籤中開啟記錄的頁面。

   記錄頁面隨即開啟。

   ![](assets/details-page.png)

1. 在記錄預覽或頁面中，按一下&#x200B;**新增封面**


   或

   將滑鼠停留在現有的封面影像上，按一下&#x200B;**更多**&#x200B;功能表![](assets/more-menu.png)，然後按一下&#x200B;**上傳**。 <!--check the casing here; I logged a bug for this-->
**唱片封面**&#x200B;方塊會在&#x200B;**上傳**&#x200B;標籤中開啟。

   ![](assets/record-cover-box-for-upload.png)

1. 按一下&#x200B;**瀏覽影像**&#x200B;並瀏覽您電腦上的圖片，以選取並新增圖片。

1. （選擇性）若要在儲存影像之前移除影像，請按一下&#x200B;**上傳新影像**&#x200B;圖示![](assets/upload-new-image-icon.png)，然後上傳新影像。

1. （選擇性）按一下&#x200B;**影像庫**&#x200B;標籤，然後按一下影像庫中的影像。 無法修改影像庫。

   ![](assets/record-cover-box-for-gallery.png)

1. 按一下&#x200B;**使用影像**。

   影像會上傳到記錄預覽或頁面頂端，而變更會自動儲存。

   ![](assets/record-page-with-cover-image.png)

1. （選擇性）將滑鼠停留在影像上，然後按一下封面影像右下角的&#x200B;**更多**&#x200B;功能表![](assets/more-menu.png)，然後執行下列任一項作業：

   * 如果您要取代封面影像，並重複步驟6以上傳並儲存新影像，請按一下&#x200B;**上傳**。
   * 按一下[重新定位]****，並使用[重新定位]工具![](assets/reposition-tool-icon.png)將封面影像置中，然後在完成時按一下[儲存]****。****
   * 按一下&#x200B;**移除**&#x200B;以移除封面影像。

   Workfront會自動儲存您的變更。
