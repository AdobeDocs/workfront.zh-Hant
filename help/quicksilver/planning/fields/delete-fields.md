---
title: 刪除欄位
description: 在Adobe Workfront規劃中，您可以刪除不再相關的自訂欄位。
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
author: Alina
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 1%

---



# 刪除欄位

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

在Adobe Workfront Planning中，您可以建立自訂欄位來儲存有關記錄的資訊。

如需有關在Workfront Planning中建立自訂欄位的資訊，請參閱[建立欄位](/help/quicksilver/planning/fields/create-fields.md)。

您可以刪除不再相關的Workfront規劃欄位。

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

<p><span class="preview">若要從全域記錄型別中刪除欄位，請執行下列動作：</span></p>
<ul><li><p><span class="preview">任何Workfront套件和Planning Plus套件</span></p></li>
或
<li><p><span class="preview">任何工作流程及計畫Prime和Ultimate套件</span></p></li></ul>

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
   <td>   <p>Manage permissions to a workspace and record type </a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p></td> 
  </tr> 
</tbody> 
</table> -->

## 刪除Workfront Planning欄位的相關考量事項：

* 您只能在記錄型別表格檢視中刪除欄位。
* 您無法刪除記錄的主要欄位。
* 儲存在欄位中的任何資訊都會被刪除且無法復原。
* 當您刪除連線的記錄欄位時，所有連線的查閱欄位也會從您連線的記錄型別中刪除。 您所連線之記錄型別的連線記錄欄位也會從您所連線的記錄中刪除。

  例如，當您將「行銷活動」連線至名為「產品」的另一個記錄型別，並從行銷活動刪除「已連線的產品」欄位和「產品的狀態」查詢欄位時，以下專案即會刪除：

   * 來自行銷活動的已連線產品欄位
   * 來自行銷活動的產品狀態查詢欄位
   * 來自產品的「已連線促銷活動」欄位

  如需詳細資訊，請參閱[連線記錄型別](/help/quicksilver/planning/architecture/connect-record-types.md)。

<!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

* <span class="preview">您無法從已新增至次要工作區的全域記錄刪除欄位。</span>

## 刪除欄位

<!--When they release the sharing of fields between other records, revise this section.  -->

{{step1-to-planning}}

1. 按一下要刪除其記錄欄位的工作區。

   工作區隨即開啟，且記錄型別隨即顯示。

1. 按一下記錄型別的卡片。

1. （視條件而定）如果尚未選取，請按一下記錄型別頁面上&#x200B;**資料表檢視**&#x200B;的索引標籤。

   與記錄型別關聯的所有現有記錄都會顯示在表格檢視的列中。

1. 在欄標題中尋找要刪除的欄位，並將滑鼠游標停留在欄標題上，然後按一下欄位名稱后面的向下箭頭。

   在表格標題中反白顯示的欄位名稱后面的![箭頭選單](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. 按一下&#x200B;**刪除**。<!-- check this: they might replace it with **Delete field**-->

   <!--insert screen shot when finalized-->

1. 按一下&#x200B;**刪除**&#x200B;確認。

   已刪除的欄位無法復原。

   根據您刪除的欄位型別，會發生下列情況：

   * 如果您刪除屬於所選記錄的欄位，則該欄位會遭到刪除，且無法再與任何記錄相關聯。 如果此欄位新增為其他記錄上的查閱欄位，這些欄位也會一併刪除。
   * 如果您刪除連線欄位，該欄位將會從您選取的記錄中刪除。 此外，也會刪除其原始記錄中的對應連線欄位。
   * 如果您刪除從連線記錄新增的查閱欄位，該欄位會從您選取的記錄型別中刪除，但會保留在其原始記錄型別中。
   * <span class="preview">如果您從主要工作區的全域記錄型別中刪除欄位，則會從已新增該記錄型別的所有工作區中刪除該欄位。 您無法從全域記錄型別的次要工作區中刪除欄位。</span>
