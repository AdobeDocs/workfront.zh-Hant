---
title: 設定記錄型別的跨工作區功能
description: 您可以啟用記錄型別，以新增至另一個工作區，或從另一個工作區進行連線。
hidefromtoc: true
hide: true
exl-id: d36ab9fb-0275-483d-97be-0a88e170f8e0
source-git-commit: 976810c8cedc5d3c5afd8333fdbace4fe8d0ccda
workflow-type: tm+mt
source-wordcount: '1052'
ht-degree: 1%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog

-->

<!--*******************THIS TITLE MIGHT NEED TO CHANGE WHEN WE HAVE THE FINAL NAME FOR THE "GLOBAL" RECORD TYPE - NOT SURE IF WE ARE GOING TO USE "GLOBAL" OR "DYNAMIC", OR ???? ***************; also update TOC file, the miniTOC,  etc when this is finalized-->



<!--this article is linked to the UI - do not delete or change the URL-->
<!--add more info here about permissions, how users gain permissions from the original record type, per Lilit: users who add this to another space gain View permissions on that space when they add records to this imported record type - this info is in the UI - this is what she sent in figma:

Hey, Alina, Lusine. As this page contains not only the "global record types" but also cross-workspace connectivity setting, we shouldn't have this message that's highlighting only the global rt features. I think we should have explanation for each setting both in enabled and disabled states. 

So we'd have the "Allow adding this record type to other workspaces" setting in enabled or disabled state, and display an explanation text below it explaining the capability, as well as a link to help articles for more context. I'd like to include the following key points in the message:  

Once enabled, this record type can be added in other workspaces by designated people 

Members of those workspaces can create and manage records in scope of their workspace 

Any records added by other workspace members will be rolled up to this workspace with view access so members of the current workspace can create views for cross-workspace records.  

Then for the second setting for cross-workspace connections, we'll need a similar explanation text would highlight that the other workspaces can create connections and gain view access to the records in this record type, but will not see the record type in their workspace. (not sure what she means by this last bit, asking in figma also)

-->

# 設定記錄型別的跨工作區功能

<!--this is linked to the UI in the info icon when you enable a record to be either centralized or connectable-->

<span class="preview">此頁面上的資訊是指尚未普遍提供的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

以下是記錄型別的跨工作區功能：

* 您可以將記錄型別指定為集中式。 使用者可以將集中式記錄型別新增到他們可以管理的其他工作區。
* 您可以將記錄型別指定為可連線。 使用者可以從其他工作區連線到此記錄型別。

您必須先定義記錄型別的跨工作區功能，然後工作區管理員才能從其他工作區連線記錄型別或將記錄型別匯入其他工作區。

當您建立或編輯記錄型別時，可以定義記錄型別的跨工作區功能。

如需詳細資訊，請參閱下列其中一篇文章：

* [建立記錄型別](/help/quicksilver/planning/architecture/create-record-types.md)
* [編輯記錄型別](/help/quicksilver/planning/architecture/edit-record-types.md)

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
   <td role="rowheader"><p>Adobe Workfront套件*</p></td> 
   <td> 
<ul><li><p>任何Workfront套件</p></li>
與
<li><p>Planning Plus套件</p></li></ul>
或：
<ul><li><p>任何Workflow封裝</p> </li>
與
<li><p>規劃Prime或Ultimate套件</p></li></ul>
<p>如需每個Workfront計畫包含內容的詳細資訊，請聯絡您的Workfront客戶經理。 </p> 
   </td>

<tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td><p>標準</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td>   <p>管理工作區</a>的許可權 </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p>  </td> 
  </tr>  
</tbody> 
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++   

## 設定集中記錄型別

<!--this is a UI term; don't change the title of this section-->
<!--IMPORTANT: not sure if we can call these centralized yet - checking with Lilit as of Sept 2; you might need to revert this to what the screen shot shows below?????-->

身為工作區管理員，您可以將記錄型別設定為集中式記錄型別。 集中記錄型別可以新增到其他工作區。

工作區管理員可以將集中式記錄型別新增到他們管理的工作區。 也會新增記錄型別的原始欄位。

使用者可以從他們有權貢獻的任何工作區（包括其主要工作區），將記錄新增至集中記錄型別。 他們只能從他們有權檢視的工作區檢視記錄。

若要將新增記錄型別設定為集中記錄型別：

{{step1-to-planning}}

1. 按一下您要編輯其記錄型別的工作區。

   工作區頁面隨即開啟，且記錄型別隨即顯示。
1. 執行下列其中一項：

   * 暫留在記錄型別的卡片上，然後按一下記錄型別卡片右上角的&#x200B;**更多**&#x200B;功能表![更多功能表](assets/more-menu.png)
或
   * 按一下記錄型別卡片以開啟記錄型別頁面，然後按一下記錄型別名稱右側的&#x200B;**更多**&#x200B;功能表![更多](assets/more-menu.png)。
1. 按一下&#x200B;**編輯**。

   ![更多記錄型別卡片中的功能表選項](assets/more-menu-options-from-record-type-card.png)

1. 在&#x200B;**編輯記錄型別**&#x200B;方塊中，選取&#x200B;**進階設定**&#x200B;索引標籤。
1. 啟用&#x200B;**允許將此記錄型別新增到其他工作區**&#x200B;設定。

   ![編輯記錄型別使用[新增至其他工作區]的進階設定可啟用](assets/edit-record-type-advanced-settings-add-to-other-workspaces-enabled.png)

1. 在&#x200B;**選取誰可以新增此記錄型別至他們管理的工作區**&#x200B;欄位中，新增您要允許新增此記錄型別的使用者至他們管理的工作區。

   您的名稱會自動新增到欄位中。

   您可以新增個別使用者，或群組、團隊、職務角色或您想允許其使用者將此記錄型別新增到他們管理的工作區的公司。

   儲存記錄型別後，您可以編輯此欄位。
1. （選擇性）從&#x200B;**選取誰可以新增此記錄型別到他們管理的工作區**&#x200B;欄位，移除您的名稱。

1. 按一下「**儲存**」。

   會發生下列情況：

   * 記錄型別及其欄位現在可以由您指定的人員新增到另一個工作區。

   >[!NOTE]
   >
   >您只能從原始工作區編輯記錄型別及其欄位。

   * 記錄型別卡片會顯示全域圖示![全域記錄型別圖示](assets/global-icon.png)，以表示該記錄型別可新增至您在組態中指定的管理員所在的任何工作區。
   * 系統產生的&#x200B;**Workspace**&#x200B;欄位已新增至記錄型別。

     Workspace欄位會顯示建立每個記錄的工作區。

     此欄位是唯讀的，無法刪除。
1. （選擇性）移至另一個工作區，並使用現有的記錄型別來建立記錄型別。 選取您在上述步驟中啟用的記錄型別。

   如需詳細資訊，請參閱[新增現有記錄型別](/help/quicksilver/planning/architecture/add-cross-workspace-record-types.md)。

## 設定可連線的記錄型別

<!--this is a UI term; don't change the title of this section-->

當您建立或編輯記錄型別時，可以設定要從其他工作區連線的記錄型別。

若要在編輯記錄型別時，設定記錄型別以從其他工作區連線：

{{step1-to-planning}}

1. 按一下您要編輯其記錄型別的工作區，

   工作區頁面隨即開啟，且記錄型別隨即顯示。
1. 執行下列其中一項：

   * 暫留在記錄型別的卡片上，然後按一下記錄型別卡片右上角的&#x200B;**更多**&#x200B;功能表![更多功能表](assets/more-menu.png)，然後按一下&#x200B;**編輯**
或
   * 按一下記錄型別卡片以開啟記錄型別頁面，按一下記錄型別名稱右側的&#x200B;**更多**&#x200B;功能表![更多](assets/more-menu.png)，然後按一下&#x200B;**編輯**。

   ![更多記錄型別卡片中的功能表選項](assets/more-menu-options-from-record-type-card.png)

1. 在&#x200B;**編輯記錄型別**&#x200B;方塊中，選取&#x200B;**進階設定**&#x200B;索引標籤。
1. 啟用&#x200B;**允許連線到其他工作區中的這個記錄型別**&#x200B;設定。<!-- check the setting name, I sent this to Lilit to say FROM instead of IN-->

   ![編輯記錄型別[進階設定]索引標籤並啟用從其他工作區的連線](assets/edit-record-type-advanced-settings-connect-from-other-workspaces-enabled.png)

   啟用時，記錄型別可供存取，並可從其他工作區連線。

1. 選擇可存取記錄型別的工作區。 從下列選項中選擇：

   * **系統範圍**：使用者可以從他們擁有管理許可權的所有工作區連線到此記錄型別。
   * **特定工作區**：新增工作區管理員可連線至此記錄型別的工作區名稱。
1. 按一下&#x200B;**編輯**。

   會發生下列情況：

   * 記錄型別及其欄位現在可以從您指定的工作區連線。
   * 記錄型別卡片會顯示跨工作區連線圖示![跨工作區連線圖示](assets/connect-from-other-workspaces-icon.png)，表示您可以從您在組態中指定的任何工作區連線記錄型別。

   記錄型別變為可以從指定的工作區連線。
1. （可選）前往另一個工作區，並將連線新增至您在上述步驟中啟用跨工作區連線的記錄型別。

   如需詳細資訊，請參閱[連線記錄型別](/help/quicksilver/planning/architecture/connect-record-types.md)。









