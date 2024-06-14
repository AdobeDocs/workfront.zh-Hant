---
product-area: projects;user-management
keywords: 附加，套用
navigation-topic: work-with-custom-forms
title: 新增自訂表單至物件
description: 您可以將現有的自訂表單新增至下列任何物件。 自訂表單包含自訂欄位，您可以在其中儲存物件的相關資訊。
author: Alina
feature: Get Started with Workfront
exl-id: c06666a7-ab78-4311-8fcb-1d1a68034133
source-git-commit: 43afa8136e51332a0970b01fff36113d5bf42294
workflow-type: tm+mt
source-wordcount: '822'
ht-degree: 2%

---

# 新增自訂表單至物件

<!--Audited: 12/2023-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

您可以將現有的自訂表單新增至下列任何物件。 自訂表單包含自訂欄位，您可以在其中儲存物件的相關資訊。

* 專案（包括業務案例）
* 任務
* 問題
* 公司
* 專案組合
* 計劃
* 文件
* 使用者
* 疊代
* 費用
* 計費記錄

您只能將自訂表單新增至已建立表單的物件型別。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文所述的動作：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
<tr> 
  <td role="rowheader">Adobe Workfront授權</td> 
  <td> <p>新增：投稿人或更高版本 </p>
 <p>或</p> 
<p>目前：要求或以上 </p> 
</td> 
 </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯您管理自訂表單之物件的存取權</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理您要附加自訂表單之物件的許可權。</p> <p>檢視自訂表單或更高許可權，並具有以下許可權： <b>附加至自訂資料</b> 物件（專案、任務和問題）。 如需詳細資訊，請參閱 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">共用自訂表格</a>.</p> <p>重要：如果您沒有可管理存取自訂Forms的計畫授權，則您必須至少擁有檢視自訂表單的特定許可權，如所述 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">共用自訂表格</a>. 即使表單在整個系統內可見，也必須將這些許可權授予您。 </p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## 先決條件

您的Workfront管理員或具有自訂表單計畫授權和管理存取權的使用者必須在您的環境中建立自訂表單，然後才能將其新增到物件。 如需詳細資訊，請參閱 [建立或編輯自訂表單](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## 新增自訂表單至物件

您可以透過兩種方式將自訂表單新增到物件：

* [透過編輯物件來新增自訂表單至物件](#add-a-custom-form-to-an-object-by-editing-the-object)
* [從詳細資訊區域新增自訂表單到物件](#add-a-custom-form-to-an-object-from-the-details-area)

### 透過編輯物件來新增自訂表單至物件 {#add-a-custom-form-to-an-object-by-editing-the-object}

1. 前往您要新增自訂表單的物件。
1. 按一下 **更多** 功能表 ![](assets/more-icon.png)，然後按一下 **編輯** ![](assets/edit-icon.png).
1. 按一下 **自訂Forms** > **新增Forms**，然後從下拉式選單中選取最多10個表單。

1. （選用）更新自訂表單上可編輯欄位中的資訊。

   您必須更新新增的表單上的所有必填欄位。

1. 按一下「**儲存**」。

### 從詳細資訊區域新增自訂表單到物件 {#add-a-custom-form-to-an-object-from-the-details-area}

1. 前往您要新增自訂表單的物件。
1. 按一下 **`<Object type>`詳細資料** 區段。 例如，按一下 **專案詳細資訊** 若要將自訂表單新增至專案或 **問題詳細資訊** 將自訂表單新增至問題。
1. 按一下 **新增自訂表格** 欄位中輸入資訊，然後從顯示的清單中選取最多10個自訂表單。

   如果表單包含任何必要欄位（以紅色星號標示），您目前不必填寫。

   選取的表單會自動附加至物件。

1. （選用）更新表單自訂欄位中的資訊，然後按一下 **儲存變更**.

## 物件上的多個自訂表單

您可以在指定物件上新增最多10個自訂表單，讓部分使用者可以使用欄位，其他人則無法使用，或讓您更符合多個專案的表單要求。

**範例：** 如果現有專案已有自訂表單，而且此專案需要更多自訂欄位（存在於另一個自訂表單中），您可以新增第二個表單到具有其他欄位的專案，而不是將欄位新增到現有自訂表單。

## 大量新增自訂表單至多個物件

您可以在清單中選取自訂表單，將其新增至多個物件。

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:-->

>[!NOTE]
>
>對於專案以外的所有物件，新增自訂表單至物件是相同的。
>
>如需大量新增自訂表單至專案的詳細資訊，請參閱文章 [編輯專案](../../manage-work/projects/manage-projects/edit-projects.md).


1. 瀏覽至物件清單。
1. 在清單中選取多個物件。

1. 按一下 **更多** 功能表 ![](assets/more-icon.png)，然後按一下 **編輯** 圖示  ![](assets/edit-icon.png).

   或

   按一下 **編輯** 圖示 ![](assets/edit-icon.png) 在清單頂端。
1. 按一下 **自訂Forms** 在左側面板中。
1. 在 **進行選取** 下拉式功能表，選取要與所有選取物件關聯的表單。

   >[!NOTE]
   >
   >如果您在下拉式功能表中找不到表單，這表示至少有一個物件具有已與其關聯的表單。 在將表單新增至剩餘物件之前，請先決定是哪個物件，並將它從您的選取範圍中移除。


1. 按一下「**儲存變更**」。

   如果表單包含任何必要欄位（以紅色星號標示），您目前不必填寫。
