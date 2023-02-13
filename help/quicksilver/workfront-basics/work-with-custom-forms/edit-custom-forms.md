---
product-area: projects;user-management
keywords: 編輯，表單，RTF，文本，特殊，格式，欄位，自定義，資訊，自定義，對象
navigation-topic: work-with-custom-forms
title: 在自訂表單欄位中編輯資訊
description: 表單附加至物件後，您就可以編輯自訂表單的資訊。 有關向對象添加自定義表單的資訊，請參閱向對象添加自定義表單。
author: Alina
feature: Get Started with Workfront
exl-id: c2b6afde-91a8-4e17-8e1a-3428b48e500a
source-git-commit: 6580fec18982215dbc2535d5f2ab159fc32ac3f5
workflow-type: tm+mt
source-wordcount: '982'
ht-degree: 0%

---

# 在自訂表單欄位中編輯資訊

表單附加至物件後，您就可以編輯自訂表單的資訊。 如需將自訂表單新增至物件的詳細資訊，請參閱 [將自訂表單新增至物件](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront計畫*</p> </td> 
   <td>團隊或更高</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront授權*</p> </td> 
   <td> <p>要求或更高版本</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">存取層級*</td> 
   <td> <p>編輯對要編輯自定義表單的對象的訪問</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>物件權限</p> </td> 
   <td> 
    <ul> 
     <li> <p>對要編輯自訂表單的對象貢獻或更高權限</p> </li> 
     <li>檢視您要編輯之欄位的權限。 如需自訂欄位共用權限的相關資訊，請參閱 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">配置自定義欄位和小工具的共用</a>.</li> 
     <li> <p>在您要編輯的欄位所在的表單上，編輯區段的權限</p> </li> 
    </ul> <p>有關請求對對象進行其他訪問的資訊，請參見 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

* 您的Workfront管理員或具有自訂表單管理存取權的規劃使用者，必須在您的環境中建立自訂表單。 如需詳細資訊，請參閱 [建立或編輯自訂表單](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
* 您必須將自訂表單附加至物件。

   如需如何將自訂表單套用至物件的詳細資訊，請參閱 [將自訂表單新增至物件](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## 編輯自訂表單的資訊

對於所有對象，附加到對象的自定義表單的編輯資訊都相同。 有關哪些對象可以具有自定義表單的資訊，請參見 [自訂表單概觀](../../administration-and-setup/customize-workfront/create-manage-custom-forms/custom-forms-overview.md).

1. 轉到要編輯自定義表單資訊的對象。
1. 按一下 **`<Object type>`詳細資料** 中。

   例如，在編輯專案自訂表單的資訊時，按一下 **專案詳細資料**.

1. 捲動至自訂表單。 當有自訂表單附加至物件時，表單的名稱會顯示為「詳細資訊」區段中的區域。
1. 如有必要，請按一下箭頭 ![](assets/expand-arrow-right.png) ，以展開自訂表單的名稱左側。
1. 在頁面的右上角附近，按一下「編輯」圖示 ![](assets/edit-icon.png).
1. 開始在您有權存取的任何欄位中輸入資訊。

   ![](assets/click-in-field-to-edit-info-350x132.png)

   或

   如果尚未在表單上輸入任何資訊，請按一下 **新增+** 對於您有權存取的任何欄位，請開始輸入資訊。

   ![](assets/plus-add-to-edit-info-350x180.png)

   如果將多個自訂表單附加至物件，您可以對每個表單執行此動作。

   視您正在使用的欄位類型而定，請考量下列事項：

   * 您只能為選項按鈕欄位選取一個選項。
   * 您可以在核取方塊欄位中選取一或多個選項，視表單建立者設定欄位的方式而定。
   * 根據表單建立者設定欄位的方式，您可以在多選下拉式欄位中選取一或多個選項。
   * 只有建立表單的使用者將文字欄位設定為「文字欄位」並設定「格式」欄位類型時，才能設定文字欄位的格式（粗體、斜體或底線）。 單行文本欄位和段落文本欄位不能格式化。
   * 只有在建立表單的使用者已在建立欄位時納入表單時，才可以更新「日期」欄位類型中的當天時間。

   如需所有欄位類型的相關資訊，請參閱 [建立或編輯自訂表單](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. 按一下 **儲存** 變更。

   >[!IMPORTANT]
   >
   >
   >
   ><!--   >
   ><p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">This is true in "Edit custom forms" but not in "Add a custom form to an object." This snippet is used in both articles. The whole snippet is conditioned for classic only in "Add" but not in "Edit." Don't remove the NWE conditioning in the snippet because it is needed in "Edit."</p>   >
   >-->   >
   >
   >您必須先填寫表單上的所有必填欄位，才能儲存表單。 必填欄位的名稱后面接著星號。
   ![](assets/nwe-required-custom-field.png)   >

   當某人更改另一個對象中由對象中計算的自定義欄位引用的資料時，這些更改不會自動反映在對象中。 如需手動更新物件中所有計算自訂欄位的相關資訊，請參閱 [重新計算對象的所有計算自定義欄位](#recalculate-all-calculated-custom-fields-for-an-object) 這篇文章。

   在批量編輯對象以及清單中的其他對象時，還可以手動更新對象的所有計算的自定義欄位。 如需指示，請參閱 [在編輯對象時重新計算清單中多個對象的所有計算自定義欄位](#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects) 這篇文章。

## 重新計算對象的所有計算自定義欄位  {#recalculate-all-calculated-custom-fields-for-an-object}

1. 轉到要重新計算其自定義欄位的對象的首頁。
1. 按一下 **更多** 功能表 ![](assets/more-icon.png) 在對象名稱的右側，然後按一下 **重新計算表達式**.

   這會重新計算物件表單上的所有自訂欄位。

## 在編輯對象時重新計算清單中多個對象的所有計算自定義欄位 {#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will need to be edited when the bulk edit for objects update in NW)</p>
-->

您可以從清單或報表中大量編輯多個對象的自定義欄位，以手動方式重新計算這些對象。

1. 移至包含具有計算欄位的自訂表單的物件清單。
1. 選擇要更新其計算自定義欄位的對象。
1. 按一下 **編輯圖示**.
1. 按一下 **自訂Forms** 在左側功能表中，然後選取 **重新計算自定義運算式**.
1. 按一下 **儲存** **變更**.

   Workfront會計算所有所選物件的所有自訂欄位。

>[!TIP]
根據專案的複雜度，我們建議在大量重新計算計算的自訂欄位時，不要選取大量專案，以確保最佳效能。 有些項目可能太複雜，可能是多個相依性或指派，或是大量自訂欄位。
要從項目清單中大量重新計算自定義表達式，請執行以下操作：
1. 前往專案清單或報表，然後選取一或多個專案。
1. 按一下 **更多** 功能表 ![](assets/more-icon.png)，然後按一下 **重新計算自定義運算式**.
![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)
Workfront會計算所有所選專案的所有自訂欄位。
