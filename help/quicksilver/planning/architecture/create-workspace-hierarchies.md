---
title: 建立Workspace階層
description: 身為工作區管理員，您可以在Adobe Workfront Planning的記錄型別之間建立多個工作區階層。 在工作區中連線記錄型別並建立階層後，記錄型別會彼此連線，其中一個記錄型別指定為父項，而最多其他6個記錄型別設定為子項。
hide: true
hidefromtoc: true
exl-id: 2f83c427-4439-499d-a0b2-fc8630552cae
source-git-commit: 3d0a6932bda338af1e6b3dcba49bfc0ac486d919
workflow-type: tm+mt
source-wordcount: '619'
ht-degree: 1%

---

<!--update the metadata with real information when making this available in TOC and in the left nav:

---
title: Create Workspace Hierarchies
description: You can create multiple workspace hierarchies between the record types in a workspace. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hide: yes 
hidefromtoc: yes 
---

-->

# 建立工作區階層

身為工作區管理員，您可以在Adobe Workfront Planning的記錄型別之間建立多個工作區階層。

在工作區中連線記錄型別並建立階層後，記錄型別會彼此連線，其中一個記錄型別指定為父項，而最多其他6個記錄型別設定為子項。<!--asking Robert how many we can have in one hierarchy; I think 7 total but not sure-->

階層會針對記錄型別產生階層連結，且記錄<!--ensure this is the case: does the breadcrumb show for both the RT and the record??-->會顯示在它們的標題中。 如此一來，使用者就能在工作流程的任何階段知道自己在階層中的位置。

如需階層與階層連結的一般資訊，請參閱[階層與階層連結概觀](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md)。

## 存取權要求

<!--check the access to see if you oversimplified???-->

<!--Update the TOC for this to publish-->

+++ 展開以檢視存取需求，以執行本文中的步驟：  

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
<ul> 
<li><p>任何Workfront和任何Planning套件</p></li>
或
<li><p>任何工作流程與任何Planning套件</p></li></ul>
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

## 建立工作區階層

{#step1-to-planning}

1. 按一下工作區卡片。
1. 按一下工作區名稱右側的&#x200B;**更多**&#x200B;功能表![更多功能表](assets/more-menu.png)，然後按一下&#x200B;**設定**。
**階層**&#x200B;區段預設會開啟。
1. 按一下&#x200B;**階層**&#x200B;頁面右上角的&#x200B;**新階層**。
1. 按一下&#x200B;**新增物件**，然後從下拉式功能表中選取物件。 這會是階層中的父物件。
您可以從目前的工作區選取記錄型別，或從Workfront選取專案。
1. 按一下&#x200B;**新增物件**以新增第二個物件，這是階層中的第一個子系，然後在下拉式選單中選取另一個物件。
   ![未選取欄位的新階層方塊](assets/new-hierarchy-modal-without-connecte-fielf-selected.png)
1. 按一下&#x200B;**選取連線的欄位**，以指出連線兩個物件的欄位。
1. （條件式）如果兩個物件型別之間有連線的欄位，請從清單中選取它。 否則，請按一下[新增連線]。****

   >[!WARNING]
   >
   >如果在建立連線的欄位時，未選取連結的記錄型別&#x200B;**上的**&#x200B;建立對應欄位，您必須先編輯欄位，然後才能繼續。

1. （視條件而定）如果您要新增連線，請執行下列動作：

   1. 在&#x200B;**名稱**&#x200B;方塊中新增連線欄位的名稱。
   1. 從下列連線型別中選取：

      * **多對多**
      * **一對多**
      * **多對一**
      * **一對一**
   1. 選取下列記錄外觀型別之一：

      * **名稱和影像**
      * **名稱**
      * **影像**
如需詳細資訊，請參閱[連線記錄型別](/help/quicksilver/planning/architecture/connect-record-types.md)。
   1. 按一下「**儲存**」。
1. （選用）依照上述步驟，繼續新增最多4種物件型別至您的階層。 您可以先新增所有物件型別，然後再新增它們之間的連線欄位。
1. （選擇性）按一下&#x200B;**移除**&#x200B;圖示![移除圖示](assets/minus-icon.png)以移除連線。
1. 按一下&#x200B;**儲存**&#x200B;以儲存您的階層。

   >[!TIP]
   >
   >如果您未設定所有連線的欄位，**儲存**&#x200B;按鈕會變暗。

   會發生下列情況：

   * 階層已新增至工作區的&#x200B;**階層**&#x200B;區段。
   * 當您前往記錄的頁面時，填入連線欄位的記錄會顯示其階層連結中的所有連線。
1. （選擇性）暫留在階層上，然後按一下&#x200B;**更多**&#x200B;功能表，然後按一下下列其中一項：

   * **編輯**：這會開啟&#x200B;**編輯階層**&#x200B;方塊，您可以在此進行變更。
   * **刪除**：這會永久刪除階層。 已刪除的階層無法復原。 不會刪除連線欄位。





