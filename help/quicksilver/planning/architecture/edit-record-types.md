---
title: 編輯記錄型別
description: 記錄型別儲存後，您可以編輯記錄型別。 記錄型別是Adobe Workfront Planning的物件型別。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: 7d37481fc5b468f6f8ea1fce6ccd7ae064f00251
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 2%

---


# 編輯記錄型別

<span class="preview">此頁面上的資訊是指尚未普遍提供的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

記錄型別是Adobe Workfront Planning的物件型別。 您可以編輯您或其他人建立的記錄型別外觀。 如需建立Workfront Planning記錄型別的相關資訊，請參閱[建立記錄型別](/help/quicksilver/planning/architecture/create-record-types.md)。

## 存取需求

+++ 展開以檢視存取需求。 

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
<ul><li>選擇</li> 
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
<p>貴組織的Workfront例項必須上線至Adobe Unified Experience，才能存取Workfront Planning。</p> 
<p>如需詳細資訊，請參閱<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">適用於Workfront的Adobe Unified Experience</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權*</p></td> 
   <td><p> 標準 </p>
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
   <td>   <p>管理工作區和記錄型別的許可權 </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p>
   <p>只有系統管理員可以啟用記錄型別以從其他工作區連線</p> </td> 
  </tr>

</tbody> 
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++   

## 編輯記錄型別

{{step1-to-planning}}

1. 按一下您要編輯其記錄型別的工作區。

   工作區頁面隨即開啟，且記錄型別隨即顯示。
1. 執行下列其中一項：

   * 暫留在記錄型別的卡片上，然後按一下記錄型別卡片右上角的&#x200B;**更多**&#x200B;功能表![更多功能表](assets/more-menu.png)，然後按一下&#x200B;**編輯**
     <!--<span class="preview">or **Settings**</span>-->
或
   * <span class="preview">按一下記錄型別卡片以開啟記錄型別頁面，按一下記錄型別名稱右邊的&#x200B;**更多**&#x200B;功能表![更多](assets/more-menu.png)，然後按一下&#x200B;**編輯**<!--<span class="preview">or **Settings**</span>. </span>-->

   <!--<span class="preview">![More menu options from record type card](assets/more-menu-options-from-record-type-card.png)</span>-->

1. 在&#x200B;**編輯記錄型別**&#x200B;方塊中，**外觀**&#x200B;索引標籤預設為開啟。<!--update screen shot below at preview-->

   ![編輯記錄型別方塊外觀索引標籤](assets/edit-record-type-box-appearance-tab.png)

   更新&#x200B;**外觀**&#x200B;索引標籤中的下列資訊：

   * 視需要編輯記錄型別名稱。<!--did they add a field label for this?-->
   * **描述**：編輯或新增記錄型別的描述，其中包含更多相關資訊。
   * 編輯與記錄型別關聯的圖示的顏色和形狀。 請執行下列動作：
      * 選取顏色以識別記錄型別。 這是記錄型別圖示的顏色。
      * 從清單中選取圖示，或開始輸入圖示名稱以說明其代表內容，然後在顯示時選取它。 這是記錄型別的圖示。 依預設，會選取檔案圖示。


1. （選擇性和條件性）如果您是系統管理員，請按一下&#x200B;**進階設定**，並更新&#x200B;**跨工作區功能**&#x200B;區段中的下列資訊： <!--the info here is duplicated in the Create record types article-->
   * 啟用&#x200B;**允許連線到其他工作區中的這個記錄型別**&#x200B;設定：這可讓工作區管理員從其他工作區連線到這個記錄型別。\
     您可以指定此記錄型別可以連線哪些工作區。 您可以使其可用於所有工作區，或指定可匯入其的特定工作區。
如需詳細資訊，請參閱[設定記錄型別的跨工作區功能](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)。


   ![在進階設定索引標籤上建立記錄型別方塊](assets/create-record-type-box-advanced-settings-tab.png)

   <!--replace last point with this when we release global record types; the preview tags might need to be edited, too:
    1. <span class="preview">(Optional and conditional) If you are a system administrator, update the information in the **Cross-workspace settings** tab.</span>
    <span class="preview">For more information, see [Configure cross-workspace capabilities for record types](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).</span>
    ***********Add screenshot***********
    -->

1. 按一下「**儲存**」。

   工作區上的記錄型別卡片會在右上角顯示連線圖示![從其他工作區連線圖示](assets/connect-from-other-workspaces-icon.png)，表示現在可以從其他工作區存取記錄。

   <!--replace the blurb above after "Save" with this: <span class="preview">If you configured the cross-workspace capabilities for the record, the **connectable record type** icon ![Connectable record type icon](assets/connect-from-other-workspaces-icon.png) and the **global record type** icon ![Global record type icon](assets/global-icon.png) also display on the card. </span>-->

1. （可選）從工作區區域按一下記錄型別卡以開啟記錄型別的頁面，然後重新命名標題中的記錄型別。

1. （選擇性）若要編輯其他記錄型別，請從記錄型別頁面中，展開記錄型別名稱右側的向下箭頭，搜尋記錄型別，然後在其顯示在清單中時選取該記錄型別。

   ![具有搜尋方塊的記錄型別頁面上的記錄型別下拉式清單](assets/record-type-drop-down-on-record-type-page-with-search-box.png)
