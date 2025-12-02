---
title: 刪除記錄型別
description: 當記錄型別不再相關時，您可以將其刪除。 刪除記錄型別也會刪除與記錄型別相關的所有資訊，例如其記錄、欄位和檢視。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 70fd3887-3871-45b5-9c21-f57da63662aa
source-git-commit: 476e10f2962f19fd17705cb5f20619d3b636aaa4
workflow-type: tm+mt
source-wordcount: '1062'
ht-degree: 1%

---


<!--keep the global record type reference in yellow till January 2026-->

# 刪除記錄型別

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

當記錄型別不再相關時，您可以將其刪除。

但是，刪除記錄型別也會刪除與記錄型別相關的所有資訊。 如需詳細資訊，請參閱本文中[刪除記錄型別](#considerations-when-deleting-record-types)時的考量事項。

如需有關記錄型別的資訊，請參閱[記錄型別概觀](/help/quicksilver/planning/architecture/overview-of-record-types.md)。

<!-- last sentence might need to be deleted when we can recover or replace deleted record types-->

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
<ul> 
<li><p>任何Workfront和任何Planning套件</p></li>
或
<li><p>任何工作流程與任何Planning套件</p></li></ul>
<div class="preview">
<p>若要刪除全域記錄型別，請執行下列動作：</p>
<ul><li><p>任何Workfront套件和Planning Plus套件</p></li>
或
<li><p>任何工作流程和Planning Prime或Ultimate套件</p></li></ul>
</div>
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
   <td><p> Standard</p>
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
   <td>   <p>Manage permissions to a workspace and record type</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p></td> 
  </tr> 
</tbody> 
</table> 
-->


## 刪除記錄型別時的注意事項

<!--check this and ensure these are still true - some things might change with / after closed beta-->

* 您只能從您擁有「管理」許可權的工作區中刪除記錄型別。
* 刪除記錄型別會移除下列與其相關的資訊：

   * 該型別的所有記錄。
   * 與記錄型別關聯的所有欄位。
   * 記錄型別的所有檢視（包括篩選器、群組和排序標準）。
* 記錄型別會從存取工作區的所有使用者中移除。
* 您無法復原已刪除的記錄型別或其資訊。
* 建議您先在其他記錄型別上重新建立與您要刪除之記錄型別相關的欄位和記錄，然後再刪除它們。

<div class="preview">

* 您無法刪除已新增至其他工作區的全域記錄型別。

  如需詳細資訊，請參閱本文中的[刪除全域記錄型別](#delete-global-record-types)一節。

</div>

## 刪除記錄型別

{{step1-to-planning}}

1. 按一下要刪除其記錄型別的工作區，

   或

   從工作區中，展開現有工作區名稱右側的向下箭頭，搜尋工作區，然後在工作區顯示在清單中時選取該工作區。

   工作區隨即開啟，且記錄型別隨即顯示。
1. 執行下列其中一項：

   * 將游標停留在記錄型別卡片上，按一下&#x200B;**更多**&#x200B;功能表，然後&#x200B;**刪除**。
   * 按一下您要刪除之記錄型別的卡片，然後在記錄型別頁面中，按一下記錄型別名稱右側的&#x200B;**更多**&#x200B;功能表![更多](assets/more-menu.png)，然後按一下&#x200B;**刪除**。

   ![永久刪除記錄型別確認](assets/permanently-delete-record-type-confirmation.png)


1. 在確認方塊中輸入&#x200B;**刪除**，然後按一下&#x200B;**永久刪除**。 不區分大小寫。

   所選的記錄型別及其欄位、關聯的記錄和檢視都會被刪除並且無法復原。

<div class="preview">

## 刪除全域記錄型別

刪除全域記錄型別時有下列情況：

* 如果設定為全域的記錄型別尚未新增到另一個工作區，您可以從它的原始工作區中刪除它。

* 如果設定為全域記錄型別的記錄型別已新增到至少一個其他工作區，則您無法從它的原始工作區中刪除它。 您必須先從新增的全域記錄型別所在的次要工作區中移除（透過刪除）全域記錄型別，然後再從原始工作區中永久刪除全域記錄型別。

### 從原始工作區中刪除全域記錄型別

如果記錄型別不再相關，您可以將其從原始工作區中刪除。

1. 移至原始工作區中的全域記錄型別。

1. （視條件而定）根據全域記錄型別是否已新增至次要工作區，執行下列其中一項作業：

   * 如果記錄型別未新增到次要工作區，請按一下記錄型別卡片上的&#x200B;**更多**&#x200B;功能表![更多](assets/more-menu.png)，或在其頁面上的記錄型別名稱右側，然後按一下&#x200B;**刪除**。
   * 如果記錄型別已新增到至少一個其他次要工作區，請先移至次要工作區，然後從該工作區中刪除全域記錄。

     如需詳細資訊，請參閱本文中的[從次要工作區刪除全域記錄型別](#delete-a-global-record-type-from-a-secondary-workspace)一節。

1. （視條件而定）繼續刪除記錄型別，如本文中[刪除記錄型別](#delete-record-types-1)一節所述。

   會發生下列情況：

   * 全域記錄型別會從原始工作區中移除，且無法復原記錄型別、其記錄和欄位。
   * 次要工作區中的所有全域記錄型別及其記錄也會被移除。

### 從次要工作區刪除全域記錄型別

如果您不再需要記錄型別，可將其從另一個工作區刪除。

請考量下列事項：

* 從次要工作區刪除全域記錄型別只會將其從次要工作區中移除， 記錄型別會保留在原始工作區中。

* 當您從次要工作區中刪除全域記錄型別時，也會刪除下列專案：

   * 從次要工作區新增的記錄。

  <!--Coming later: * The fields added from the secondary workspace.-->

* 從次要工作區中刪除的全域記錄型別無法復原。

* 原始記錄型別會保留在其原始工作區中，也會保留在其已加入的其他工作區中。

若要從次要工作區刪除全域記錄型別，請執行下列動作：

1. 移至其次要工作區中的全域記錄型別。

1. （選擇性）按一下記錄型別卡片上的&#x200B;**更多**&#x200B;功能表![更多功能表](assets/more-menu.png)，或在其頁面上的記錄型別名稱右側，然後按一下&#x200B;**刪除**。
1. （視條件而定）在提供的欄位中輸入&#x200B;**刪除**，然後按一下&#x200B;**永久刪除**。

   ![刪除次要全域記錄型別確認方塊](assets/delete-secondary-global-record-type.png)

   會發生下列情況：

   * 從全域記錄型別建立的記錄型別會從選取的工作區中移除。
   * 原始記錄型別及其欄位會保留在其原始工作區中。
   * 記錄型別會保留在已新增它的所有其他工作區中。
   * 刪除從目前工作區新增到記錄型別的記錄<!--and fields-->。 從已新增全域記錄型別的其他工作區新增的所有其他記錄都會保留在各自的工作區和原始工作區中。 &lt;！ — 欄位會保留在加入它們的工作區中。

</div>
