---
title: 從復本設計表單
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 您可以使用表單設計工具，從副本設計自訂表單。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 578a8bd5-d93f-4327-bb4f-2c17b91b170a
source-git-commit: ecafbd693237427d727b15dd22afd485b4e59c72
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# 從復本設計表單

<!--add preview tags and see below in commet out-->

您可以根據現有表格設計新的自訂表格。 您可以將自訂表單附加至不同的Workfront物件，以擷取這些物件的相關資料。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具備下列專案才能執行本文所述的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront計畫</p> </td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>
   <p>新增：標準</p>
   <p>或</p>
   <p>目前：計畫</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>管理自訂表單的存取權</p> </td> 
  </tr>  
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 複製自訂表單以建立新表單

{{step-1-to-setup}}

1. 按一下&#x200B;**自訂Forms。**
1. 選取要作為新自訂表單基礎的自訂表單，然後按一下![復製圖示](assets/copy-icon.png)。
1. 在出現的&#x200B;**自訂表單復本**&#x200B;方塊中，輸入下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">表格名稱</td> 
      <td>輸入所複製表單的名稱。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">表單型別 </p> </td> 
      <td> <p>在<b>表單型別</b>方塊中，選取您要使用自訂表單的物件型別，然後按一下您要移除的任何型別旁的X。 已與此表單關聯的型別會在清單中停用。</p> 
      <p><img src="assets/copy-form-obj-types-040524.png"></p> 
      <p>表單必須至少與一個物件型別相關聯。</p> 
      </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**複製**。

   在原始表單中，如果計算欄位參考的欄位與您新增至新表單的物件型別不相容，則會出現一條訊息，提示您變更這些欄位中的計算。

   同樣地，如果原始表單上分割槽符號的存取選項與您新增到新表單的物件型別不相容，則會出現一則訊息，提示您調整選項。

1. 選取您剛複製的表單，然後按一下![編輯圖示](assets/edit-icon.png)。
1. 如[建立自訂表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)文章的下列章節所說明，對表單進行任何變更：

   * [重複使用已在其他自訂表單中使用的現有欄位或Widget](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#reuse-an-existing-field-or-widget-already-used-in-another-custom-form)
      * [新增文字欄位](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-text-fields)
      * [新增計算欄位](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-calculated-fields)
      * [新增選項按鈕、核取方塊群組和下拉式清單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-radio-buttons-checkboxes-and-dropdowns)
      * [新增預先輸入和日期欄位](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-typeahead-and-date-fields)
      * [新增影像、PDF和影片](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-images-pdfs-and-videos)
      * [新增Adobe XD檔案](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-adobe-xd-files)
        <!--* [Add Planning connection fields](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-planning-connection-fields)-->

1. （選擇性）按一下&#x200B;**儲存+關閉**&#x200B;之後，將表單附加至您要使用它的物件，如[將自訂表單新增至物件](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)中所述。
