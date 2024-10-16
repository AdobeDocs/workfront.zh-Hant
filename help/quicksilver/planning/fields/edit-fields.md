---
title: 編輯欄位設定
description: 在Adobe Workfront Planning中，您可以編輯已建立欄位的欄位設定。 本文說明如何編輯Workfront Planning欄位的設定。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: 9debb7c6d9df0f9f4962f3e66f146e5f605d20f0
workflow-type: tm+mt
source-wordcount: '711'
ht-degree: 1%

---


# 編輯欄位設定

{{planning-important-intro}}

您可以編輯已在Adobe Workfront Planning中建立的欄位之欄位設定。

如需有關建立Adobe Workfront Planning欄位的資訊，請參閱[建立欄位](/help/quicksilver/planning/fields/create-fields.md)。

本文說明如何編輯Workfront Planning欄位的設定。 如需有關編輯記錄欄位值的資訊，請參閱[編輯記錄](/help/quicksilver/planning/records/edit-records.md)。

## 存取需求

+++ 展開以檢視Workfront Planning的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

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
<ul><li>選取</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>舊版Workfront計畫不提供Workfront計畫</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront規劃計畫*</p></td> 
   <td> 
<p>任何 </p> 
<p>如需每個Workfront計畫包含內容的詳細資訊，請聯絡您的Workfront客戶經理。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront平台</p></td> 
   <td> 
<p>貴組織的Workfront例項必須加入Adobe統一體驗，才能存取Workfront規劃的所有功能。</p> 
<p>如需詳細資訊，請參閱<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront的Adobe統一體驗</a>。 </p> 
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
   <td>   <p>管理工作區</a>的許可權 </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>版面配置範本</p></td> 
   <td> <p>必須為所有使用者(包括Workfront管理員)指派一個版面配置範本，該範本包含主功能表中的Planning區域。 </p> </td> 
  </tr> 
</tbody> 
</table>

*如需Workfront存取需求的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


<!--
OLD

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   <p>Current: Plan</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access controls for Workfront Planning</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->

## 編輯欄位設定的相關考量事項

在變更欄位的設定之前，您必須考慮以下事項：

* 如果您擁有該欄位所屬工作區的管理許可權，您可以編輯您建立的欄位或其他使用者建立的欄位。
* 您可以在記錄型別表格中編輯欄位。
* 您無法在記錄頁面或表格檢視之外的任何其他檢視中編輯欄位。
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

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. 更新欄位相關資訊，然後按一下&#x200B;**儲存**。<!--insert screen shot when finalized-->

   >[!TIP]
   >
   >* 儲存欄位後，您無法更新欄位型別。
   >
   >* 當您修改欄位設定（欄位選項或公式運算式）時，已包含修改欄位中資訊的記錄將即時更新其值。 欄位設定變更所觸發的值變更沒有警告或稽核記錄。 所有檢視欄位的使用者都會立即看到經過修改的新值。

   欄位資訊會針對所有有權檢視工作區的人員而更新。

1. （視條件而定）對於連結的記錄欄位，按一下&#x200B;**編輯查閱欄位**&#x200B;並從連結的記錄型別新增或移除任何欄位。

   如需詳細資訊，請參閱[連線記錄型別](/help/quicksilver/planning/architecture/connect-record-types.md)。

