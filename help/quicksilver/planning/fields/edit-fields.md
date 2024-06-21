---
title: 編輯欄位設定
description: 在Adobe Workfront Planning中，您可以編輯已建立欄位的欄位設定。 本文說明如何編輯Workfront Planning欄位的設定。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: dc8e6f730ec88fc66c3486987e064b5f0760fb80
workflow-type: tm+mt
source-wordcount: '627'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!---
title: Edit fields
description: In Adobe Workfront Planning, you can edit the field settings for fields that are already created.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

# 編輯欄位設定

{{planning-important-intro}}

您可以編輯已在Adobe Workfront Planning中建立的欄位之欄位設定。

如需建立Adobe Workfront Planning欄位的相關資訊，請參閱 [建立欄位](/help/quicksilver/planning/fields/create-fields.md).

本文說明如何編輯Workfront Planning欄位的設定。 如需有關編輯記錄欄位值的資訊，請參閱 [編輯記錄](/help/quicksilver/planning/records/edit-records.md).

## 存取需求

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
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront合約</p></td>
   <td>
<p>您的組織必須處於Workfront Planning的早期存取階段中註冊 </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront計畫</p></td>
   <td>
<p>任何</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront授權*</p></td>
   <td>
   <p>新增：標準</p>
   <p>目前：計畫</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>存取層級設定</p></td>
   <td> <p>Workfront Planning沒有存取控制</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>權限</p></td>
   <td> <p>管理工作區的許可權</a> </p>  
   <p>系統管理員擁有所有工作區的許可權，包括他們未建立的工作區</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>版面配置範本</p></td>
   <td> <p>您的Workfront或群組管理員必須在版面配置範本中新增Planning區域。 如需詳細資訊，請參閱 <a href="/help/quicksilver/planning/access/access-overview.md">存取權總覽</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*如需詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

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

1. （視條件而定）按一下 **表格檢視**.

   與記錄型別關聯的所有現有記錄都會顯示在表格檢視的列中。
1. 將游標停留在您要編輯的欄位標題上，然後按一下欄位名稱后的向下箭頭，然後按一下 **編輯欄位**

   或

   連按兩下欄位的欄標題。

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. 更新欄位的相關資訊，然後按一下 **儲存**. <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >* 儲存欄位後，您無法更新欄位型別。
   >
   >* 當您修改欄位設定（欄位選項或公式運算式）時，已包含修改欄位中資訊的記錄將即時更新其值。 欄位設定變更所觸發的值變更沒有警告或稽核記錄。 所有檢視欄位的使用者都會立即看到經過修改的新值。

   欄位資訊會針對所有有權檢視工作區的人員而更新。

1. （視條件而定）對於連結的記錄欄位，按一下 **編輯查閱欄位** 和從連結的記錄型別新增或移除任何欄位。

   如需詳細資訊，請參閱 [連線記錄型別](/help/quicksilver/planning/architecture/connect-record-types.md).

