---
title: 在GenStudio Planning中管理Adobe Workfront Workspace
description: 當貴公司同時購買產品，且您的GenStudio for Performance Marketing執行個體已整合至貴公司的GenStudio執行個體時，Adobe Workfront Planning中即可使用Workfront工作區。 您可以從Planning檢視GenStudio工作區，並更新兩個系統中的資訊。
hide: true
hidefromtoc: true
exl-id: d6140b05-26c3-4298-a2f9-53695aa021cb
source-git-commit: 9b95b5a52576327a3df8d6955925b96c2e45848f
workflow-type: tm+mt
source-wordcount: '1337'
ht-degree: 0%

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

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

當貴公司同時購買產品，且您的Adobe GenStudio for Performance Marketing執行個體已整合至貴公司的GenStudio執行個體時，Adobe Workfront Planning中即可使用Workfront工作區。

您可以從Planning檢視GenStudio工作區，並更新兩個系統中的資訊。

如需從GenStudio效能行銷使用及管理GenStudio工作區的相關資訊，請參閱[Adobe GenStudio for Performance Marketing使用手冊](https://experienceleague.adobe.com/zh-hant/docs/genstudio-for-performance-marketing/user-guide/home)。

如需GenStudio與Workfront Planning整合的一般資訊，請參閱[開始使用Adobe Workfront Planning與Adobe GenStudio for Performance Marketing整合](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md)。

>[!IMPORTANT]
>
>本文所述的步驟說明在擁有GenStudio工作區的「管理」許可權時，如何從Workfront Planning更新工作區。
>&#x200B;> 當您擁有GenStudio工作區的貢獻許可權時，並非所有功能都可使用。
>
>如果您的公司有多個Workfront例項，則所有使用者都能在Workfront Planning中取得GenStudio工作區的貢獻許可權。

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
<p>任何Workfront套件</p>
<p>任何Planning套件</p>

</td> </tr>
   <tr> 
<td> 
   <p> 其他產品</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td><p> 標準</p>
  </td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Adobe GenStudio for Performance Marketing使用者角色</p></td> 
   <td><p><ul><li>存取行銷活動、產品和角色的任何GenStudio使用者角色</li>
   <li>GenSudio System Manager存取啟用與事件</li></ul>
   如需詳細資訊，請參閱<a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">使用者角色和許可權</a>。 
   </p>
  </td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td>  
   <p>在Workfront規劃中： </p>
   <ul>
   <li><p>管理GenStudio工作區的許可權，以新增欄位或記錄型別至GenStudio工作區</p></li>
   <li><p>為GenStudio工作區貢獻許可權，以便在GenStudio工作區中新增、更新或刪除記錄</p> </li>  
   </ul>
   <p>任何使用者都不能從Workfront Planning的GenStudio for Performance Marketing工作區中移除GenStudio記錄型別或欄位</p>
   <p>在Adobe GenStudio for Performance Marketing中： <p>
   <ul>
   <li><p> Adobe GenStudio for Performance Marketing中的任何許可權</p></li>
   <li><p> 在Adobe GenStudio for Performance Marketing中建立許可權以建立專案</p></li></ul>
   </td> 
  </tr> 
</tbody> 
</table>

如需Adobe Workfront Planning存取權的相關資訊，請參閱[Adobe Workfront Planning存取權概觀](/help/quicksilver/planning/access/access-overview.md)。

如需Adobe GenStudio for Performance Marketing的詳細資訊，請參閱[Adobe GenStudio for Performance Marketing使用手冊](https://experienceleague.adobe.com/zh-hant/docs/genstudio-for-performance-marketing/user-guide/home)。

+++   

## 在Workfront Planning中管理GenStudio工作區的考量事項

* 貴組織必須先購買Adobe GenStudio for Performance Marketing，才能在Workfront Planning中檢視GenStudio工作區。

* 根據組織擁有的Workfront例項數目，您在Planning中自動擁有GenStudio工作區的下列許可權：

  <!--this table is also in the Get started article-->

  <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
   <tbody> 
      <tr> 
      <td role="rowheader"><p>一個Workfront例項</p></td> 
      <td> 
   <p>可在您的Workfront Planning例項中看見GenStudio工作區</p>
   <p>Workfront管理員擁有在Planning中GenStudio工作區的管理許可權</p>
   <p>所有其他使用者皆擁有Planning中GenStudio工作區的「貢獻」存取權</p>
   </td> </tr>
      <tr> 
   <td> 
      <p> 多個Workfront例項</p> </td> 
      <td> 
      <p>所有Workfront例項皆顯示GenStudio工作區</p>
   <p>所有可存取GenStudio for Performance Marketing和Workfront Planning的使用者皆擁有Planning中GenStudio的「貢獻」許可權</p> </td> 
   </tr>
      </tbody> 
   </table>

* 更新GenStudio工作區的工作區設定、記錄型別、檢視和欄位，與更新Workfront Planning工作區及其元素的方式相同。

<!--
## Manage GenStudio workspace from Workfront Planning

CAN YOU DO THIS?? 
- OPTIONS FROM THE WORKSPACE CARD ??
- OPTIONS FROM THE MORE MENU ON A WORKSPACE ??
-->

## 從Workfront Planning管理GenStudio工作區

>[!NOTE]
>
>在管理GenStudio工作區之前，請參閱文章[開始使用Workfront Planning和GenStudio for Performance Marketing整合](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md)以取得詳細資訊。
>

1. 以也可存取GenStudio的使用者身分登入Workfront。
1. 按一下左上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon-left-nav.png)，然後按一下&#x200B;**[!UICONTROL 計畫]**。

   Workfront Planning首頁面隨即開啟。

1. 按一下「**其他工作區**」，然後尋找含有&#x200B;**系統**&#x200B;所建立之指示，且卡片上有&#x200B;**GenStudio**&#x200B;標籤的工作區。

   ![含標籤的GenStudio工作區卡](assets/genstudio-card-with-tag-highlighted.png)

1. 按一下&#x200B;**GenStudio工作區卡片**，在Workfront Planning中開啟GenStudio工作區。
1. 依預設，下列GenStudio記錄型別是從Workfront Planning建立並顯示：

   * 行銷活動
   * 產品
   * 人物誌
   * 啟用
   * 管道
   * 區域

   GenStudio記錄型別卡上會顯示他們原本是在GenStudio中建立的。

   <!--check screen shot-->

   ![含標籤的GenStudio記錄型別卡片](assets/genstudio-record-type-with-tag-and-tooltip-highlighted.png)

1. 按一下工作區名稱右側的&#x200B;**更多**&#x200B;功能表![更多功能表](assets/more-menu.png)，然後按一下下列其中一項：

   * **編輯**

     如需詳細資訊，請參閱[編輯工作區](/help/quicksilver/planning/architecture/edit-workspaces.md)。
     <!--* **Delete** - this will generate an error message, per Iskuhi, so don't document as an option/ possibility-->

     <!--For information, see [Delete workspaces](/help/quicksilver/planning/architecture/delete-workspaces.md). -->

1. 按一下右上角的「共用&#x200B;**」**，與其他人共用工作區。

   如需詳細資訊，請參閱[共用工作區](/help/quicksilver/planning/access/share-workspaces.md)

1. 按一下任何記錄型別卡片以檢視該型別的記錄。

   若要管理記錄型別、檢視和欄位，請參閱本文中的[從Workfront Planning管理GenStudio記錄型別](#manage-genstudio-record-types-from-workfront-planning)小節。


## 在Workfront Planning中從GenStudio工作區管理記錄型別、檢視和記錄

>[!NOTE]
>
>在管理GenStudio工作區之前，請參閱文章[開始使用Workfront Planning和GenStudio for Performance Marketing整合](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md)以取得詳細資訊。
>

1. 前往Workfront Planning中的GenStudio工作區並開啟記錄型別頁面，如本文中[從Workfront Planning管理GenStudio工作區](#manage-the-genstudio-workspace-from-workfront-planning)小節所述。

1. 按一下記錄型別名稱右側的&#x200B;**更多**&#x200B;功能表![更多功能表](assets/more-menu.png)，然後按一下下列其中一項：

   * **編輯**

     如需詳細資訊，請參閱[編輯記錄型別](/help/quicksilver/planning/architecture/edit-record-types.md)。
   * **管理自動化**

     如需詳細資訊，請參閱[設定Adobe Workfront規劃自動化](/help/quicksilver/planning/records/configure-automations-to-create-records.md)。
   * **管理請求表單**

     您可以建立多個請求表單。 Workfront的請求區域會提供請求表單，您也可以公開或透過連結共用請求表單。

     如需詳細資訊，請參閱[在Adobe Workfront Planning中建立和管理要求表單](/help/quicksilver/planning/requests/create-request-form.md)。

1. 若要共用檢視或記錄型別，請執行下列動作：

   * 按一下記錄型別頁面右上角的&#x200B;**共用**，然後按一下下列其中一項：
      * **共用記錄型別**
如需詳細資訊，請參閱[共用記錄型別](/help/quicksilver/planning/access/share-record-types.md)。
      * **共用目前的檢視**
如需詳細資訊，請參閱[共用檢視](/help/quicksilver/planning/access/share-views.md)。
      * **複製檢視連結**
檢視的連結已複製到您的剪貼簿。
      * **匯出目前的檢視**
如需詳細資訊，請參閱[從資料表檢視](/help/quicksilver/planning/records/export-records-from-the-table-view.md)匯出記錄。

1. 若要管理記錄型別檢視，請執行下列動作：

   * 按一下&#x200B;**+檢視**&#x200B;以建立GenStudio記錄型別的檢視。

     如需詳細資訊，請參閱[管理記錄檢視](/help/quicksilver/planning/views/manage-record-views.md)。

   * 按一下&#x200B;**全熒幕**&#x200B;圖示![以全熒幕模式開啟全熒幕檢檢視示](assets/open-full-screen-icon.png)，以全熒幕模式開啟任何檢視。

   * 從任何檢視管理檢視的元素。

     例如，您可以變更檢視的篩選器、群組、排序、設定（如果可用）。

     如需詳細資訊，請參閱[管理記錄檢視](/help/quicksilver/planning/views/manage-record-views.md)。

1. 若要新增記錄，請執行下列任一項作業：

   * 從任何檢視按一下&#x200B;**新增記錄**&#x200B;以從頭開始建立記錄

   * 在表格檢視中使用Excel或CSV檔案匯入記錄

   * 按一下時間軸或行事曆檢視中的任何位置，即可新增記錄。

     如需詳細資訊，請參閱[建立記錄](/help/quicksilver/planning/records/create-records.md)。

     Workfront和GenStudio皆可檢視記錄。

     >[!NOTE]
     >
     >您無法為Activations記錄型別新增記錄。

1. 若要編輯記錄，請執行下列任一項作業：

   * 從表格檢視編輯內嵌記錄

   * 從任何檢視中按一下記錄，即可開啟其詳細資訊頁面。

     如需詳細資訊，請參閱[編輯記錄](/help/quicksilver/planning/records/edit-records.md)。

     您在Planning中GenStudio工作區所做的變更會立即從GenStudio中顯示。

1. 在表格檢視中選取記錄，然後按一下[刪除]。**&#x200B;**

   如需詳細資訊，請參閱[刪除記錄](/help/quicksilver/planning/records/delete-records.md)。

   刪除的記錄會立即從GenStudio中移除。

   >[!TIP]
   >
   >已刪除的記錄可從Workfront Planning的表格檢視最近刪除的資料匣中復原。 從GenStudio中刪除的記錄也可以從Workfront Planning中最近刪除的資料匣復原。

   如需詳細資訊，請參閱[還原已刪除的記錄](/help/quicksilver/planning/records/restore-deleted-records.md)

1. 按一下表格檢視右上角的+圖示以建立下列專案：

   * 記錄欄位

     如需詳細資訊，請參閱[建立欄位](/help/quicksilver/planning/fields/create-fields.md)

   * 記錄連線

     如需詳細資訊，請參閱[連線記錄型別](/help/quicksilver/planning/architecture/connect-record-types.md)

     從GenStudio工作區建立的欄位會顯示在下列區域中：

      * Workfront Planning檢視
      * Workfront Planning記錄詳細資料
      * GenStudio記錄詳細資料

     >[!TIP]
     >
     >在Workfront Planning中建立的欄位不會顯示在GenStudio的清單檢視中。

1. 暫留在表格檢視中的欄位上，然後按一下下拉式功能表以執行下列任一項作業：

   * 依其排序
   * 隱藏它
   * 編輯其設定
     <!--* Delete it - not possible now, per Iskuhi; the link is there but it will generate an error-->

     <!--GenStudio-native fields are note removed from GenStudio. -->

     >[!NOTE]
     >
     >只有當您在GenStudio中擁有「管理」許可權時，才能編輯欄位設定並新增更多欄位。

