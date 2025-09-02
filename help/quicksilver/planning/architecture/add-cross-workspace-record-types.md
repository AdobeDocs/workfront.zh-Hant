---
title: 新增現有記錄型別
description: 記錄型別是Adobe Workfront Planning的物件型別。 在Workfront Planning中，您可以從另一個工作區匯入現有的記錄型別。
hidefromtoc: true
hide: true
exl-id: b977d5dd-8975-42c4-9968-a7ac357972e6
source-git-commit: 976810c8cedc5d3c5afd8333fdbace4fe8d0ccda
workflow-type: tm+mt
source-wordcount: '584'
ht-degree: 1%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# 新增現有記錄型別

<span class="preview">此頁面上的資訊是指尚未普遍提供的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

身為工作區管理員，您可以匯入現有記錄型別或將其新增至另一個工作區。

必須先將記錄型別指定為集中型別，工作區管理員才能將其匯入其他工作區。

當您在定義記錄型別的跨工作區設定時，可以在建立或編輯記錄型別時將其指定為集中型別。

如需詳細資訊，請參閱[設定記錄型別的跨工作區功能](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)。

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

## 集中記錄型別概觀

從另一個工作區新增現有記錄型別時的注意事項

* 當沒有記錄型別設定為要新增到另一個工作區時，建立記錄型別時不會顯示從另一個工作區匯入它們的選項。<!--add this a tip in the steps below, and/ or add a Conditional step that this is possible only when these record types are first enabled-->
* 從另一個工作區新增記錄型別之後，也會從現有記錄型別新增以下資訊：

   * 欄位
   * 記錄連線

* 只有在您擁有其他工作區的許可權時，才能檢視從這些工作區新增的記錄。

* 您只能在其原始工作區中編輯記錄型別，包括其欄位。 您無法從新增它的工作區中編輯它。
* 從所有工作區新增的記錄將對從所有工作區存取它們的所有使用者可見，即使這些記錄是在沒有許可權的工作區中建立的。

## 從現有記錄型別建立記錄型別

1. 開始建立記錄型別，如文章[建立記錄型別](/help/quicksilver/planning/architecture/create-record-types.md)中所述，然後按一下&#x200B;**新增現有的**。<!--check this - the option might have been renamed in the UI-->

   ![模式以新增記錄型別，並附上從其他工作區匯入的選項](assets/add-record-type-from-existing-workspace-option-when-creating-records.png)

1. 按一下&#x200B;**繼續**。
1. 在&#x200B;**選擇記錄型別**&#x200B;方塊中，按一下您要從現有工作區新增的記錄型別的卡片，然後按一下&#x200B;**新增**。

   記錄型別會新增至您選取的工作區，且會發生下列情況：

   * **跨工作區記錄型別**&#x200B;圖示![跨工作區連線圖示](assets/global-icon.png)已新增至匯入記錄型別的卡片。
   * 唯讀&#x200B;**Workspace**&#x200B;欄位已新增至匯入的記錄型別。 欄位會顯示每個記錄建立時所在的工作區。

     >[!NOTE]
     >
     >* 您無法編輯匯入的記錄型別或其欄位。 您可以從原始工作區中編輯記錄型別及其欄位。

1. （選擇性）在匯入的記錄型別卡片中按一下&#x200B;**更多**&#x200B;功能表![更多功能表](assets/more-menu.png)，或在其頁面上的記錄型別名稱右側，然後按一下&#x200B;**刪除**。
1. （視條件而定）在提供的欄位中輸入&#x200B;**刪除**，然後按一下&#x200B;**永久刪除**。

   這會從選取的工作區移除匯入的記錄型別。 原始記錄型別及其欄位會保留在其原始工作區中。

   <!--**************************ASK LILIT ON THIS ONE, NOT SURE IF THIS IS TRUE: Any records added in the current workspace are saved in the original workspace.**********-->



