---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: 透過舊版表單產生器，在自訂表單中重複使用自訂欄位或資產Widget
description: 當您建立或編輯自訂表單時，可以新增已新增至其他自訂表單的自訂欄位或Widget。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 2c617909-48cb-4ee1-b0e8-002f2e57b0f0
source-git-commit: d32f274390f6ffc5fdd01c2c9b4b2abd99d7cb10
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# 透過舊版表單產生器，在自訂表單中重複使用自訂欄位或資產Widget

{{form-designer-default}}

當您建立或編輯自訂表單時，可以新增已新增至其他自訂表單的自訂欄位或資產Widget。

您也可以重複使用自訂表單中現有的計算自訂欄位。 如需指示，請參閱[在自訂表單中重複使用現有的計算自訂欄位](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)。

如需自訂表單中自訂欄位和資產Widget的相關資訊，請參閱[新增自訂欄位至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)和[新增或編輯自訂表單中的資產Widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)。

## 存取需求

您必須具備下列專案才能執行本文所述的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront計畫*</p> </td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td>計劃</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>管理自訂表單的存取權</p> <p>如需Workfront管理員如何授予此存取權的相關資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予使用者對特定區域的管理存取權</a>。</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取層級設定，請連絡您的Workfront管理員。

## 重複使用已在其他自訂表單中使用的自訂欄位或Widget

1. 開始建立或編輯自訂表單，如[使用舊版表單產生器建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)中所述。
1. 選取&#x200B;**新增欄位**&#x200B;後，按一下&#x200B;**欄位程式庫**。

1. 將您想要的欄位或Widget拖曳至此以自訂表單顯示。
1. （可選）重複前兩個步驟以新增任何其他欄位或Widget。

   >[!NOTE]
   >
   >您最多可以在單一自訂表單中新增500個欄位和Widget。 不過，根據表單的複雜性，當表單上存在超過100個時，可能會發生效能降低。
   >
   >
   >複雜表單的範例包括含有階層式引數的表單、計算的自訂資料欄位，以及單一欄位中的多個值選項。

1. 如果您想以其他方式繼續建置自訂表單，請繼續閱讀下列其中一篇文章：

   * [使用舊版表單產生器將自訂欄位新增至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md#add2)
   * [使用舊版表單產生器將分割槽符號新增至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [使用舊版表單產生器，在自訂表單中新增或編輯資產Widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [使用舊版表單產生器將計算資料新增至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [使用舊版表單產生器，在自訂表單中放置自訂欄位和Widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [新增顯示邏輯並略過邏輯至具有舊版表單產生器的自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [使用舊版表單產生器預覽並完成自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)
