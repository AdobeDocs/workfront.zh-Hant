---
title: 使用表單設計工具從副本設計表單
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 您可以使用表單設計工具從副本設計自訂表單。
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 4700e5650f6ef9de5291f36072db8706bade92ee
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 0%

---


# 使用表單設計工具從副本設計表單

{{highlighted-preview-article-level}}

您可以根據現有表單來設計新的自訂表單。 您可以將自訂表單附加至不同的Workfront物件，以擷取這些物件的相關資料。

## 存取需求

您必須具備下列條件才能執行本文所述步驟：

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
   <td>
   <p>當前計畫：標準</p>
   <p>或</p>
   <p>舊計畫：計畫</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>管理對自訂表單的存取</p> <p>如需Workfront管理員如何授予此存取權的詳細資訊，請參閱 <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用戶對特定區域的管理訪問權限</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取層級設定，請聯絡您的Workfront管理員。

## 複製自訂表單以建立新表單

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **自訂Forms。**
1. 選取您要作為新自訂表單基礎的自訂表單，然後按一下 **複製**.
1. 在 **自訂表單副本** 框中，鍵入以下資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">表格名稱</td> 
      <td>鍵入複製表單的名稱。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">表單類型 </p> </td> 
      <td> <p>在 <b>表單類型</b> 框中，選擇希望自定義表單使用的對象類型，然後按一下要刪除的任何類型旁邊的X。 已與表單關聯的類型在清單中被禁用。</p> 
      <p><img src="assets/copy-form-obj-types.png"></p> 
      <p>表單必須至少與一個對象類型關聯。</p> 
      </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **複製表單**.

   在原始表單中，如果計算欄位引用與添加到新表單的對象類型不相容的欄位，則會出現一條消息提示您更改這些欄位中的計算。

   同樣，如果原始表單上斷節的訪問選項與添加到新表單中的對象類型不相容，則消息會提示您調整該選項。

1. 選取您剛複製的表單，然後按一下 **編輯**.
1. 對表單進行任何變更，如 [設計表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) 文章：

* [重複使用已在其他自定義表單中使用的現有欄位或介面工具集](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#reuse-an-existing-field-or-widget-already-used-in-another-custom-form)
   * [新增文字欄位](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-text-fields)
   * [新增計算欄位](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-calculated-fields)
   * [新增選項按鈕、核取方塊群組和下拉式清單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-radio-buttons-checkboxes-and-dropdowns)
   * [新增提前類型和日期欄位](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-typeahead-and-date-fields)
   * [新增影像、PDF和影片](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-images-pdfs-and-videos)
   * [新增Adobe XD檔案](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-adobe-xd-files)

1. （選用）按一下 **儲存並關閉**，將表單附加至您要使用該表單的物件，如 [將自訂表單新增至物件](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).