---
user-type: administrator
product-area: system-administration
keywords: 建立，自訂，表單，複製，基礎，其他
navigation-topic: create-and-manage-custom-forms
title: 複製自訂表單，使用舊版產生器建立新表單
description: 您可以建立以現有表單為基礎的新自訂表單。
author: Caroline
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 946a726e-af88-413c-abe3-55fbc7486380
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# 複製自訂表單，使用舊版產生器建立新表單

您可以建立以現有表單為基礎的新自訂表單。

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
   <td> <p>管理自訂表單的存取權</p> <p>如需Workfront管理員如何授予此存取許可權的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予使用者管理特定區域的存取權</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取層級設定，請聯絡Workfront管理員。

## 複製自訂表單以建立新表單

1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) (位於Adobe Workfront的右上角)，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **自訂Forms。**
1. 選取要作為新自訂表單基礎的自訂表單，然後按一下 **複製**.
1. 在 **自訂表格複製** 在出現的方塊中，輸入下列資訊：

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
      <td> <p>在 <b>表單型別</b> 方塊中，選取您要使用自訂表單的物件型別，然後按一下您要移除的任何型別旁的X。 已與此表單關聯的型別會在清單中停用。</p> 
      <p><img src="assets/copy-form-obj-types.png"></p> 
      <p>表單必須至少與一個物件型別相關聯。</p> 
      </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **複製表單**.

   在原始表單中，如果計算欄位參考的欄位與您新增至新表單的物件型別不相容，則會出現一條訊息，提示您變更這些欄位中的計算。

   同樣地，如果原始表單上分割槽符號的存取選項與您新增到新表單的物件型別不相容，則會出現一則訊息，提示您調整選項。

1. 選取您剛複製的表單，然後按一下 **編輯**.
1. 變更表單，如下列文章所述：

   * [複製自訂表單，使用舊版表單產生器建立新表單](#Add2)
   * [使用舊版表單產生器將計算資料新增至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [在自訂表單中使用舊版表單產生器來定位自訂欄位和Widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [使用舊版表單產生器，在自訂表單中新增或編輯資產小工具](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [使用舊版表單產生器重複使用自訂表單中現有的計算自訂欄位](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [使用舊版表單產生器新增顯示邏輯和略過邏輯至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [使用舊版表單產生器預覽並完成自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

1. （選擇性）按一下 **儲存+關閉**，將表單附加至您要使用的物件，如所述 [新增自訂表單至物件](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
