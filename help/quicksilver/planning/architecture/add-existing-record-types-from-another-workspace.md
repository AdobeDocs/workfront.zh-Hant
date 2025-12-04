---
title: 從其他Workspace新增現有記錄型別
description: 記錄型別是Adobe Workfront Planning的物件型別。 在Workfront Planning中，您可以新增在其他工作區中建立的現有記錄型別。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: b977d5dd-8975-42c4-9968-a7ac357972e6
source-git-commit: 0c890cc535c61c5402a334e43ed45b3ec3f9f748
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 1%

---


# 從另一個工作區新增現有記錄型別

{{planning-important-intro}}

<span class="preview">此頁面上的資訊是指尚未普遍提供的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

身為工作區管理員，您可以將存在於另一個工作區的記錄型別新增至您在Adobe Workfront Planning中管理的工作區。

工作區管理員必須先將記錄型別指定為全域記錄型別，然後才能將其新增到您作為現有記錄型別管理的工作區。 Workspace管理員可在建立或編輯記錄型別時，透過定義記錄型別的跨工作區設定，將記錄型別指定為全域。

如需詳細資訊，請參閱[設定記錄型別的跨工作區功能](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)。

本文說明如何從現有記錄型別新增記錄型別。

從全域記錄型別新增記錄至工作區之前，請先參閱文章[跨工作區記錄型別概觀](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md)。


## 存取權要求

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
   <td role="rowheader"><p>Adobe Workfront 封裝</p></td> 
   <td> 
<ul><li><p>任何Workfront套件和Planning Plus套件</p></li>
或
<li><p>任何工作流程和Planning Prime或Ultimate套件</p></p></li></ul>
<p>如需每個Workfront Planning套件所含內容的詳細資訊，請聯絡您的Workfront客戶代表。 </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront授權</p></td> 
   <td><p>標準</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td>   <p>管理工作區的許可權</p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p>  </td> 
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

  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<ul><li><p>Any Workfront package</p></li>
<p>And</p>
<li><p>Any Planning package to create connectable record types</p></li>
<li><p>A Planning Plus package to create global record types</p></li>
</ul>
Or:
<ul><li><p>A Prime or Ultimate Workflow package</p> </li>
And
<li><p>A Planning Prime or Ultimate package</p></li></ul>
<p>For more information about what is included in each Workfront Planning package, contact your Workfront account manager. </p> 
   </td> 

  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace and to the record type</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr>  
</tbody> 
</table>-->

## 從另一個工作區新增現有記錄型別，以建立記錄型別

>[!NOTE]
>
>請確定至少有一個記錄型別被指定為在至少一個其他主要工作區中的全域。
>
>如需詳細資訊，請參閱[設定記錄型別的跨工作區功能](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)。

1. 移至您要建立記錄型別的工作區（次要工作區）。
1. 開始建立記錄型別，如文章[建立記錄型別](/help/quicksilver/planning/architecture/create-record-types.md)中所述，然後按一下&#x200B;**新增現有的**。<!--check this - the option might have been renamed in the UI-->

   ![從另一個工作區新增選項以新增記錄型別的模型](assets/add-record-type-from-existing-workspace-option-when-creating-records.png)

   >[!TIP]
   >
   >當沒有記錄型別設定為要新增至系統中的其他工作區時，不會顯示&#x200B;**新增現有**&#x200B;選項。

1. 按一下「**繼續**」。
1. 在「**選擇記錄型別**」方塊中，按一下您要從現有工作區新增之記錄型別的卡片，然後按一下「**新增**」。

   記錄型別已新增至您選取的次要工作區，且&#x200B;**全域記錄型別**&#x200B;圖示![](assets/global-icon.png)會顯示在記錄型別的卡片上。

   會發生下列情況：

   * 以下資訊也會從現有的全域記錄型別中新增：

      * 所有原始欄位
      * 所有記錄連線
   * 您至少擁有這些工作區的「檢視」許可權時，才能檢視使用相同全域記錄型別之其他工作區新增的記錄。
   * 唯讀&#x200B;**Workspace**&#x200B;欄位已新增至新記錄型別資料表檢視。 欄位會顯示建立每個記錄的工作區。

     >[!NOTE]
     >
     >您無法編輯新記錄型別的外觀、其他設定或原始欄位。 您只能從原始工作區編輯記錄型別及其所有原始欄位和設定。
     >

1. （可選）按一下，然後將新新增的記錄型別拖放至工作區內的任何區段。
1. （選擇性）按一下新記錄型別卡片上的&#x200B;**更多**&#x200B;功能表，或其頁面上的記錄型別名稱右側，然後按一下&#x200B;**刪除**。

   如需詳細資訊，請參閱文章[刪除記錄型別](/help/quicksilver/planning/architecture/delete-record-types.md)中的「刪除全域記錄型別」一節。

<!--This will be released later with another epic: 
1. In the table view, click the **+** icon in the upper-right corner to add new fields. For information, see [Create fields](/help/quicksilver/planning/fields/create-fields.md).
1. (Optional) Click the **More** menu ![More menu](assets/more-menu.png) in the new record type's card, or to the right of the record type's name on its page, then click **Share** to share it with other users in the same workspace, or adjust their permissions to the record type.
-->

&lt;！ — 若我們可以新增自動化或請求表單至次要全域RT，請向Lilit核取?? — 若可以，請新增包含這些文章連結的步驟 — >







