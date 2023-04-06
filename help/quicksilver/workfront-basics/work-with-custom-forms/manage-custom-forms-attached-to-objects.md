---
product-area: projects;user-management
navigation-topic: work-with-custom-forms
title: 管理附加到對象的自定義表單
description: 您可以更新附加至一個物件的自訂表單顯示順序、移除它們，或大量編輯自訂表單在多個物件上的顯示方式。
author: Alina
feature: Get Started with Workfront
exl-id: e5570a09-32cb-43e3-9c1d-4421db42fa24
source-git-commit: 78878fa3578e4f3a33baec3806298282d3909d8d
workflow-type: tm+mt
source-wordcount: '1108'
ht-degree: 0%

---

# 管理附加到對象的自定義表單

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

您可以更新附加至一個物件的自訂表單顯示順序、移除它們，或大量編輯自訂表單在多個物件上的顯示方式。

## 存取需求

您必須具備下列存取權，才能執行本文所述的動作：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>要求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯您管理自訂表單之物件的存取權</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>對您管理自訂表單的物件貢獻權限或更高權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

* 您的Workfront管理員或具有自訂表單管理存取權的規劃使用者，必須在您的環境中建立自訂表單。 如需詳細資訊，請參閱 [建立或編輯自訂表單](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
* 您必須將自訂表單附加至物件。

   如需如何將自訂表單套用至物件的詳細資訊，請參閱 [將自訂表單新增至物件](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## 重新排序附加至物件的多個自訂表單 {#reorder-multiple-custom-forms-attached-to-an-object}

1. 前往您要變更新增自訂表單順序的物件，然後開始編輯物件。

   **範例：** 例如，若要管理專案的自訂表單，請前往專案，按一下 **更多** 功能表 ![](assets/more-icon.png)，然後按一下 **編輯** .

1. 在 **自訂Forms** 區段中，按一下 ![](assets/move-icon---dots.png) 表徵圖。 對於所有其他對象，按一下 **管理Forms**. 只有在至少一個自訂表單已附加至物件時，才會顯示此選項。
1. 拖曳表單 ![](assets/move-icon---dots.png) 到清單中的新位置。
1. 針對專案、工作和問題自訂表單，請按一下 **儲存**.

   對於所有其他對象，按一下 **我已經做完了** > **儲存變更**.

## 從物件中移除自訂表單 {#remove-a-custom-form-from-an-object}

>[!IMPORTANT]
>
>從對象中刪除自定義表單時，表單的自定義欄位中捕獲的所有資訊都將丟失，且無法恢復。

1. 移至您要移除自訂表單的物件，然後開始編輯物件。

   例如，前往專案，按一下 **更多** 功能表 ![](assets/more-icon.png)，然後按一下 **編輯** .

1. 按一下 **自訂Forms**.
1. 若為專案、工作和問題自訂表單，請按一下 **X** 表單右側的表徵圖，以將其從對象中刪除。

   對於所有其他對象，按一下 **管理Forms**，然後按一下 **X** 表單右側的表徵圖，以將其從對象中刪除。

1. 按一下&#x200B;**儲存**。

## 管理包含相同自訂欄位的多個自訂表單

您可能會在附加至相同物件的多個自訂表單上顯示相同欄位。 在此情況下，請考量下列事項：

* 欄位的值在所有形式中都相同。

   不同表單上的相同欄位不能有不同值附加至相同物件。

* 如果兩個不同對象上有相同的計算欄位，則其計算必須相同，以避免錯誤。 如需如何將計算欄位新增至自訂表單（包括多個表單）的資訊，請參閱 [將計算資料新增至自訂表單](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md) .

## 在大量編輯物件時管理多個自訂表單

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:-->

>[!NOTE]
>
>對於除項目外的所有對象，管理對對象的自定義表單都相同。
>
>如需將自訂表單大量新增至專案的詳細資訊，請參閱文章 [編輯專案](../../manage-work/projects/manage-projects/edit-projects.md).

當您大量編輯已套用多個自訂表單的物件時，可以編輯這些物件上自訂表單的顯示方式，以及編輯自訂表單中的常見欄位。

只有附加至所有所選對象的自定義表單可以批量編輯。

若要在大量編輯物件時編輯多個自訂表單：

1. 在清單對象中，選擇自定義表單附加的對象，然後按一下 **編輯** 圖示 ![](assets/edit-icon.png).
1. 按一下 **自訂Forms**.

   您只能編輯附加到所有選定對象的自定義表單。

   僅附加到某些對象的自定義表單不顯示。

1. 開始編輯自訂表單上的欄位。

   編輯欄位時，欄位上會顯示視覺指標，顯示已編輯欄位。

   如果一個欄位包含在多個自訂表單中，當您更新其中一個表單的欄位時，這些欄位的所有值都會在每個表單上更新。

1. 按一下 **進行選取** 下拉式選單中，並選取其他表單以新增至所有選取的物件。

   套用其他表單時，請考量下列事項：

   * 物件最多可以有10個自訂表單。
   * 僅當表單尚未應用於正在編輯的任何對象時，才可應用表單。 已附加到其中一個對象的表單不會顯示在下拉菜單中。
   * 在您套用其他表單後，表單與其他表單有共同之處的任何欄位都會顯示在 **公用欄位** 區段中填入內容，且可加以編輯。

1. （可選）如果向所有對象添加了自定義表單，但尚未保存對象，則可以更改自定義表單在對象上的顯示順序。

   如需變更表單順序的詳細資訊，請參閱 [重新排序附加至物件的多個自訂表單](#reorder-multiple-custom-forms-attached-to-an-object) 這篇文章。

1. 按一下 **移除表單** 從對象中刪除自定義表單。

   如需從物件移除自訂表單的詳細資訊，請參閱 [從物件中移除自訂表單](#remove-a-custom-form-from-an-object).

   從數個物件大量移除表單時，請考量下列事項：

   * 如果已對表單進行更改，則刪除該表單會導致您的更改丟失，且無法恢復。
   * 移除表單後，表單中任何 **公用欄位** 區段會從此區段中移除，且無法再在此編輯。

1. 按一下 **還原表單** 要將表單還原為編輯對象之前的狀態。
1. （可選）按一下表單名稱旁的折疊箭頭，一次折疊一個表單。

   或

   按一下 **折疊Forms** 同時折疊所有表單。

1. （可選）按一下表單名稱旁的展開箭頭，一次展開一個表單。

   或

   按一下 **展開Forms** 以同時展開所有表單。 

1. 按一下 **儲存變更**.
