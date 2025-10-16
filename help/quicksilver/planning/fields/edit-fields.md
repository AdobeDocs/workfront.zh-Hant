---
title: 編輯欄位設定
description: 在Adobe Workfront Planning中，您可以編輯已建立欄位的欄位設定。 本文說明如何編輯Workfront Planning欄位的設定。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '979'
ht-degree: 0%

---


# 編輯欄位設定

<!--leave the choice value information in yellow till January 2026-->

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

您可以在Adobe Workfront Planning中編輯現有欄位的設定。

如需有關建立Adobe Workfront Planning欄位的資訊，請參閱[建立欄位](/help/quicksilver/planning/fields/create-fields.md)。

本文說明如何編輯Workfront Planning欄位的設定。 如需有關編輯記錄欄位值的資訊，請參閱[編輯記錄](/help/quicksilver/planning/records/edit-records.md)。

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
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
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
   <td><p> Standard </p>
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
   <td>   <p>Manage permissions to a workspace and record type</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p></td> 
  </tr> 
</tbody> 
</table> -->

## 編輯欄位設定的相關考量事項

在變更欄位的設定之前，您必須考慮以下事項：

* 您只能從記錄型別表中編輯欄位設定。
* 您無法在記錄頁面或表格檢視之外的任何其他檢視中編輯欄位設定。
* 儲存欄位後，您無法編輯欄位型別。
* 如果先前選取的「數字」、「百分比」或「幣別」欄位在其附加的記錄中已有負值，則無法取消選取該欄位的「允許負數」設定。
* 儲存欄位後，您可以編輯以下欄位元素的設定：

   * 任何欄位的名稱或描述
   * 單選或多選欄位的選項。
   * 公式欄位的運算式。

  >[!WARNING]
  >
  >當公式運算式變更，或從select-type欄位新增或移除選項時，已儲存資訊的記錄將遺失資料，資訊會儲存在已修改其設定的欄位中。
  >
  >當您變更欄位設定時，沒有警告或指示可能發生此資料遺失。
  >
  >不會通知其他使用者欄位設定已變更。

* 您可以從連線的記錄中編輯現有的查閱欄位。
* 除了依照本文中[編輯欄位設定](#edit-field-settings-1)一節所述編輯欄位外，當您在表格檢視中編輯記錄時，在更新欄位值時，還可以編輯單一或多重選取欄位的選擇。 如需詳細資訊，請參閱本文中在資料表檢視[區段中編輯記錄時，將](#add-new-choices-to-an-existing-select-field-when-editing-records-in-the-table-view)新選擇新增至現有的選取欄位。

<!--at production - April 10, 2025 - remove the last bullet altogether-->

<!--this is not yet true, but it might come later:
* You can deselect Allow negative numbers option from a Number, Percentage, or Currency field after you save the field. 
-->

## 編輯欄位設定

{{step1-to-planning}}

1. 按一下您要編輯其記錄欄位的工作區。

   工作區隨即開啟，且工作區中的所有記錄型別都會顯示在卡片上。

1. 按一下記錄型別的卡片。

   這會開啟記錄型別的頁面。

1. （視條件而定）按一下&#x200B;**資料表檢視**&#x200B;的索引標籤。

   與記錄型別關聯的所有現有記錄都會顯示在表格檢視的列中。
1. 暫留在您要編輯欄位的欄標題上，然後按一下欄位名稱后的向下箭頭，然後按一下&#x200B;**編輯欄位**

   或

   連按兩下欄位的欄標題。

   在表格標題中反白顯示的欄位名稱后面的![箭頭選單](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. 更新欄位相關資訊，然後按一下&#x200B;**儲存**。

   如需詳細資訊，請參閱[建立欄位](/help/quicksilver/planning/fields/create-fields.md)。

   <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >* 儲存欄位後，您無法更新欄位型別。
   >
   >* 當您修改欄位設定（欄位選項或公式運算式）時，已包含修改欄位中資訊的記錄將即時更新其值。 欄位設定變更所觸發的值變更沒有警告或稽核記錄。 所有檢視欄位的使用者都會立即看到經過修改的新值。

   欄位資訊會針對所有有權檢視工作區的人員而更新。

1. （視條件而定）對於連線的記錄欄位，按一下&#x200B;**編輯查閱欄位**，並從連線的記錄型別新增或移除任何查閱欄位。

   如需詳細資訊，請參閱[連線記錄型別](/help/quicksilver/planning/architecture/connect-record-types.md)。


## 在表格檢視中編輯記錄時，將新選擇新增至現有的選取欄位

<!--some of this information is also available in Edit records article - update both when necessary-->

在表格檢視中編輯記錄時，您可以將新選擇新增至現有的單一或多重選取欄位。

>[!IMPORTANT]
>
>本節中說明的功能只能在表格檢視中使用。 無法用於顯示單選或多選欄位的任何其他區域。

**範例**

您可能會有一個名為「狀態」的單選欄位，其選項為「新增」和「已關閉」，而且您要為「進行中」狀態新增選項。 您可以執行下列其中一項作業來新增選擇：

* 編輯欄位。 如需詳細資訊，請參閱本文中的[編輯欄位設定](#edit-field-settings-1)一節。
* 在表格檢視中編輯記錄時新增選項，如下所述。

若要在編輯記錄時新增選擇至現有的選取欄位：

1. 移至記錄型別頁面並開啟表格檢視。
1. 新增您要在表格檢視中新增選擇的單一或多重選取欄位作為新欄。 如需詳細資訊，請參閱[建立欄位](/help/quicksilver/planning/fields/create-fields.md)。
1. 連按兩下欄位的儲存格，開始內嵌編輯欄位。
1. 輸入您要新增的選擇名稱，然後按一下[新增選擇]。****

   ![在表格檢視中的單一選取欄位中新增選項](assets/add-choice-in-table-view-for-single-select-field.png)

   新選項會立即新增至單選欄位。

   <span class="preview">每個選擇也會新增一個值。 您可以在API呼叫或其他整合中使用選擇值。 如需詳細資訊，請參閱[建立欄位](/help/quicksilver/planning/fields/create-fields.md).</span>

