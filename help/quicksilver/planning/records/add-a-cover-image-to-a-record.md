---
title: 新增封面影像至記錄
description: 編輯記錄時，您可以在Adobe Workfront Planning中將封面影像新增至記錄頁面，以個人化記錄。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 93c6bc15-d945-4cfc-8e87-f5b4e6fac2f4
source-git-commit: 1dc2791bed0dfada109ee102e09c25ae9a52e6b0
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 1%

---


# 新增封面影像至記錄

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

編輯記錄時，您可以在Adobe Workfront Planning中將封面影像新增至記錄頁面，以個人化記錄。

如需有關編輯記錄的資訊，請參閱[編輯記錄](/help/quicksilver/planning/records/edit-records.md)。

您必須先建立記錄型別，才能開始建立和編輯記錄。

如需詳細資訊，請參閱[建立記錄型別](/help/quicksilver/planning/architecture/create-record-types.md)。

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
<p>如需每個Workfront Planning套件所含專案的詳細資訊，請連絡您的Workfront客戶經理。 </p> 
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
   <td>   <p>為工作區<span class="preview">和記錄型別</span>貢獻或更高的許可權  </p>  
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

<!--replace the layout template info in the table with this at release: 


<p>In the Production environment, all users including the System Administrators must be assigned to a layout template that includes the Planning areas.</p>
<p><span class="preview">In the Preview environment, Standard users and System Administrators have the Planning area enabled by default.</span></p>

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
