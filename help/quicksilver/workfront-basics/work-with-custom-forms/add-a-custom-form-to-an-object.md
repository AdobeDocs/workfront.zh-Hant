---
product-area: projects;user-management
keywords: 附加，應用
navigation-topic: work-with-custom-forms
title: 將自訂表單新增至物件
description: 您可以將現有的自訂表單新增至下列任何物件。 自訂表單包含自訂欄位，您可在其中儲存物件的相關資訊。
author: Alina
feature: Get Started with Workfront
exl-id: c06666a7-ab78-4311-8fcb-1d1a68034133
source-git-commit: 78878fa3578e4f3a33baec3806298282d3909d8d
workflow-type: tm+mt
source-wordcount: '850'
ht-degree: 1%

---

# 將自訂表單新增至物件

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

您可以將現有的自訂表單新增至下列任何物件。 自訂表單包含自訂欄位，您可在其中儲存物件的相關資訊。

* 項目（包括業務案例）
* 任務
* 問題
* 公司
* 專案組合
* 計劃
* 文件
* 使用者
* 疊代
* 費用
* 帳單記錄

您只能將自定義表單添加到為其建立表單的對象類型中。

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
   <td> <p>編輯您管理自訂表單之物件的存取權</p> <p><b>附註</b></p>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理要附加自訂表單之物件的權限。</p> <p>檢視自訂表單的或更高權限，並具有 <b>附加至自訂資料</b> 對象（項目、任務和問題）。 如需詳細資訊，請參閱 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">共用自訂表單</a>.</p> <p>重要：如果您沒有具有自訂Forms管理存取權的計畫授權，您必須擁有特定權限，才能至少檢視自訂表單，如 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">共用自訂表單</a>. 即使表單在全系統可見，也必須授予您這些權限。 </p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 先決條件

您的Workfront管理員或具有自訂表單計畫授權和管理存取權的使用者，必須先在您的環境中建立自訂表單，才能將其新增至物件。 如需詳細資訊，請參閱 [建立或編輯自訂表單](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## 將自訂表單新增至物件

您可以透過兩種方式將自訂表單新增至物件：

* [通過編輯對象向對象添加自定義表單](#add-a-custom-form-to-an-object-by-editing-the-object)
* [從「詳細資訊」區域將自訂表單新增至物件](#add-a-custom-form-to-an-object-from-the-details-area)

### 通過編輯對象向對象添加自定義表單 {#add-a-custom-form-to-an-object-by-editing-the-object}

1. 移至您要新增自訂表單的物件。
1. 按一下 **更多** 功能表 ![](assets/more-icon.png)，然後按一下 **編輯** ![](assets/edit-icon.png).
1. 按一下 **自訂Forms** > **新增Forms**，然後從下拉式功能表中選取最多10個表單。

1. （可選）更新自訂表單上可編輯欄位中的資訊。

   您必須更新所新增表單上的所有必要欄位。

1. 按一下&#x200B;**儲存**。

### 從「詳細資訊」區域將自訂表單新增至物件 {#add-a-custom-form-to-an-object-from-the-details-area}

1. 移至您要新增自訂表單的物件。
1. 按一下 **`<Object type>`詳細資料** 區段。 例如，按一下 **專案詳細資料** 將自訂表單新增至專案或 **問題詳細資訊** 將自訂表單新增至問題。
1. 按一下 **新增自訂表單** 欄位，然後從顯示的清單中選取最多10個自訂表單。

   如果表單包含任何必填欄位（標有紅色星號），您目前不需要完成這些欄位。

   所選表單會自動附加到對象。

1. （選用）更新表單自訂欄位中的資訊，然後按一下 **儲存變更**.

## 物件上的多個自訂表單

您可以在指定物件上新增最多10個自訂表單，讓某些使用者可使用欄位，而非其他使用者可使用，或讓您更符合多個專案的表單需求。

**範例：** 如果現有項目已有自定義表單，並且需要其他自定義表單上存在的自定義欄位，則您可以使用其他欄位將第二個表單添加到項目，而不是將欄位添加到現有自定義表單（如果僅需要這個項目的這些欄位）。

## 將自訂表單大量新增至多個物件

您可以在清單中選取自訂表單，將自訂表單新增至多個物件。

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:-->

>[!NOTE]
>
>對於除項目外的所有對象，將自定義表單添加到對象是相同的。
>
>如需將自訂表單大量新增至專案的詳細資訊，請參閱文章 [編輯專案](../../manage-work/projects/manage-projects/edit-projects.md).


1. 導覽至物件清單。
1. 在清單中選取多個物件。

1. 按一下 **更多** 功能表 ![](assets/more-icon.png)，然後按一下 **編輯** 圖示  ![](assets/edit-icon.png)，或按一下 **編輯** 圖示 ![](assets/edit-icon.png) 清單頂端。
1. 按一下 **自訂Forms** 中。
1. 選擇要與 **進行選取** 下拉式功能表。
   >[!NOTE]
   >
   >如果在下拉菜單中找不到表單，這意味著至少有一個對象具有已與其關聯的表單。 確定哪個對象是該對象，並在將表單添加到剩餘對象之前將其從您的選擇中刪除。


1. 按一下 **儲存變更**.

   如果表單包含任何必填欄位（標有紅色星號），您目前不需要完成這些欄位。
