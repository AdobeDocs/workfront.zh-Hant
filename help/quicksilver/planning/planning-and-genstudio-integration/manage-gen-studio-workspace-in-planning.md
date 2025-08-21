---
title: 在GenStudio Planning中管理Adobe Workfront Workspace
description: 當貴公司同時購買產品，且您的GenStudio for Performance Marketing執行個體已整合至貴公司的GenStudio執行個體時，Adobe Workfront Planning中即可使用Workfront工作區。 您可以從Planning檢視GenStudio工作區，並更新兩個系統中的資訊。
hide: true
hidefromtoc: true
exl-id: d6140b05-26c3-4298-a2f9-53695aa021cb
source-git-commit: 4569b5bd004a93396257f3f1f8964831f69399dc
workflow-type: tm+mt
source-wordcount: '931'
ht-degree: 1%

---


<!--Better metadata, at publishing:
---
title: Manage the GenStudio Workspace in Adobe Workfront Planning
description: The GenStudio for Performance Marketing workspace is available in Adobe Workfront Planning when your company has purchased both products and your instance of Workfront is integrated with your company's instance of GenStudio. You can view the GenStudio workspace from Planning and update information in both systems.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
---
-->

<!--MUST update the access requirements below - not complete!!!!!!!!!-->

# 在Adobe Workfront Planning中管理GenStudio工作區

<span class="preview">此頁面上的資訊是指尚未普遍提供的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

當貴公司同時購買產品，且您的Adobe GenStudio for Performance Marketing執行個體已整合至貴公司的GenStudio執行個體時，Adobe Workfront Planning中即可使用Workfront工作區。

您可以從Planning檢視GenStudio工作區，並更新兩個系統中的資訊。

如需從GenStudio效能行銷使用及管理GenStudio工作區的相關資訊，請參閱[Adobe GenStudio for Performance Marketing使用手冊](https://experienceleague.adobe.com/zh-hant/docs/genstudio-for-performance-marketing/user-guide/home)。

如需GenStudio與Workfront Planning整合的一般資訊，請參閱[開始使用Adobe Workfront Planning與Adobe GenStudio for Performance Marketing整合](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
    <td role="rowheader"><p>Adobe Workfront套件</p></td> 
   <td> 
<p>任何Adobe Workfront Workflow套件</p>
<p>任何Adobe Workfront Planning套件</p>

</td> </tr>
<tr> 
   <td role="rowheader"><p>Adobe GenStudio套件</p></td> 
   <td> 
<p>???GEN STUDIO是否有支援此功能的套件???</p>

</td> </tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront平台</p></td> 
   <td> 
<p>貴組織的Workfront例項必須上線至Adobe Unified Experience，才能存取Workfront Planning。</p> 
<p>如需詳細資訊，請參閱<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">適用於Workfront的Adobe Unified Experience</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td><p> 標準</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe GenStudio授權</p></td> 
   <td><p> ???GEN STUDIO是否需要支援此的特定授權???</p>
  </td> 
  </tr> 
  <tr> 
<td> 
   <p> 其他產品</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>   
  <tr> 
   <td role="rowheader"><p>存取層級設定</p></td> 
   <td> <p>Adobe Workfront Planning沒有存取層級控制</p>  
   <p>GenStudio的設定：???GENS的存取層級需求為何???</p> 
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>物件許可權*</p></td> 
   <td>  
   <p>在Workfront規劃中： </p>
   <ul>
   <li><p>貢獻或更高的許可權到工作區和記錄型別  </p> </li> 
   <li><p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p></li>
   </ul>
   <p>在Adobe GenStudio for Performance Marketing中： <p>
   <ul>
   <li><p> Adobe GenStudio for Performance Marketing中的任何許可權</p></li>
   <li><p> 在Adobe GenStudio for Performance Marketing中建立許可權以建立專案</p></li></ul>
   </td> 
  </tr> 
</tbody> 
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。
*如需Adobe GenStudio for Performance Marketing的詳細資訊，請參閱[Adobe GenStudio for Performance Marketing使用手冊](https://experienceleague.adobe.com/zh-hant/docs/genstudio-for-performance-marketing/user-guide/home)。

+++   

## 在Workfront Planning中管理GenStudio工作區的考量事項

* 貴組織必須先購買Adobe GenStudio for Performance Marketing，才能在Workfront Planning中檢視GenStudio工作區。

* Workfront使用者必須擁有GenStudio的存取權，才能在Workfront Planning中檢視GenStudio工作區。

* 您可以從Workfront Planning更新GenStudio工作區的下列資訊：

   * 編輯工作區設定<!--check to see if this is correct? is this editable or read only from Planning??-->
   * 編輯記錄型別及其欄位<!--check on this-->
   * 共用、編輯和新增檢視
   * 新增記錄型別
   * 編輯、新增或刪除記錄

* 更新GenStudio工作區的工作區設定、記錄型別、檢視和欄位，與更新Workfront Planning工作區及其元素的方式相同。

<!--
## Manage GenStudio workspace from Workfront Planning

CAN YOU DO THIS?? 
- OPTIONS FROM THE WORKSPACE CARD ??
- OPTIONS FROM THE MORE MENU ON A WORKSPACE ??
-->

## 從Workfront Planning管理GenStudio記錄型別

>[!NOTE]
>
>在管理GenStudio工作區之前，請參閱文章[開始使用Workfront規劃和GenStudio for Performance Marketing整合](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md)。

1. 以也可存取GenStudio的使用者身分登入Workfront。
1. 按一下左上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon-left-nav.png)，然後按一下&#x200B;**[!UICONTROL 計畫]**。

   Workfront Planning首頁面隨即開啟。

1. 按一下「**其他工作區**」，然後尋找含有&#x200B;**系統**&#x200B;所建立之指示，且卡片上有&#x200B;**GenStudio**&#x200B;標籤的工作區。

   ![含標籤的GenStudio工作區卡](assets/genstudio-card-with-tag-highlighted.png)

1. 按一下&#x200B;**GenStudio工作區卡片**，在Workfront Planning中開啟GenStudio工作區。
1. 依預設，下列GenStudio記錄型別是從Workfront Planning建立並顯示：

   * 行銷活動
   * 產品
   * 啟用
   * 管道
   * 區域

   GenStudio記錄型別卡上會顯示他們原本是在GenStudio中建立的。

   <!--check screen shot-->

   ![含標籤的GenStudio記錄型別卡片](assets/genstudio-record-type-with-tag-and-tooltip-highlighted.png)

1. 按一下任何記錄型別卡片以檢視該型別的記錄。

1. 執行下列其中一項：

   * 按一下記錄型別頁面右上角的&#x200B;**共用**，然後按一下下列其中一項：
      * **複製檢視連結**&#x200B;以共用記錄型別的連結
      * **匯出目前的檢視**&#x200B;以將其匯出為CSV或Excel檔案。
您只能匯出表格檢視。<!--check on this later; is this true or are there more options in the Share button-->

   * 按一下&#x200B;**+檢視**&#x200B;以建立GenStudio記錄型別的檢視。

     如需詳細資訊，請參閱[管理記錄檢視](/help/quicksilver/planning/views/manage-record-views.md)。

   * 按一下&#x200B;**全熒幕**&#x200B;圖示![以全熒幕模式開啟全熒幕檢檢視示](assets/open-full-screen-icon.png)，以全熒幕模式開啟任何檢視。

   * 從任何檢視管理檢視的元素。

     例如，您可以變更檢視的篩選器、群組、排序、設定（如果可用）。

     如需詳細資訊，請參閱[管理記錄檢視](/help/quicksilver/planning/views/manage-record-views.md)。

   * 在表格或時間表檢視中新增記錄。

     您只能從頭開始建立記錄，或是匯入CSV或Excel檔案。

     如需詳細資訊，請參閱[建立記錄](/help/quicksilver/planning/records/create-records.md)。

     Workfront和GenStudio皆可檢視記錄。

   * 從表格檢視中編輯內嵌記錄，或按一下記錄以開啟其詳細資訊頁面。

     如需詳細資訊，請參閱[編輯記錄](/help/quicksilver/planning/records/edit-records.md)。

   * 刪除表格檢視中的記錄。

     如需詳細資訊，請參閱[刪除記錄](/help/quicksilver/planning/records/delete-records.md)。

     如果從Workfront中刪除已刪除的記錄，則可以從Workfront Planning的表格檢視資源回收筒復原這些記錄。

     如需詳細資訊，請參閱[還原已刪除的記錄](/help/quicksilver/planning/records/restore-deleted-records.md)

   * 暫留在表格檢視中的欄位上可排序或隱藏欄位。

     >[!NOTE]
     >
     >只有當您在GenStudio中擁有「管理」許可權時，才能編輯欄位設定並新增更多欄位。<!--check to see if this is true??-->
