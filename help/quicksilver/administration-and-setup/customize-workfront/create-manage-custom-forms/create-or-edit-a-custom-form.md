---
title: 使用舊版表單產生器建立或編輯自訂表單
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 您可以建立或編輯新的自訂表格。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 5712e82d-bd1d-4d8a-9a2a-1e19b562b9d1
source-git-commit: 6b2a2160b5daaa94374707bad4b026daa13edf06
workflow-type: tm+mt
source-wordcount: '908'
ht-degree: 0%

---

# 使用舊版表單產生器建立或編輯自訂表單

<!--Audited: 01/2024-->

{{form-designer-default}}

您可以建立新的自訂表單或編輯現有表單。 本文會說明這兩項工作。

如需從現有表單建立新自訂表單的相關資訊，請參閱 [複製自訂表單，使用舊版表單產生器建立新表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/copy-custom-form-to-create-a-new-one.md).

本文說明如何使用舊版表單產生器建立自訂表單。 如需有關使用表單設計工具建立自訂表單的資訊，請參閱 [使用表單設計工具設計表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

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
   <td><p>新增：標準</p>
   <p>或</p>
   <p>目前：計畫</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>管理自訂表單的存取權</p> </td> 
  </tr>  
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## 開始建立自訂表單

{{step-1-to-setup}}

1. 按一下 **自訂Forms** 在左側面板中。

   自訂表單會顯示在清單中。 您可以檢閱為您的組織建立的所有自訂表單和自訂欄位。 您也可以檢視每個表單的建立者、與其相關聯的物件，以及表單是否處於作用中狀態。

1. 按一下 **新增自訂表格。**
1. 請至少選取一個要與自訂表單關聯的物件型別，然後按一下 **繼續**.

   ![](assets/choose-object-type.jpg)

1. 在 **表單設定** 開啟的標籤，鍵入 **表單標題** 和選填 **說明** 用於自訂表格。

1. （選擇性）如果要將更多物件型別加入表單，以便將其附加到更多物件，請按一下 **加** 於以下時間後簽署： **物件型別**，然後在顯示的功能表中選取您想要的物件型別。

   您可以重複此步驟，新增任意數目的物件型別。

1. （可選）按一下 **X** 物件型別，以將其從表單中刪除。

   如需有關從已儲存的自訂表單中刪除物件型別的資訊，請參閱 [刪除自訂表單上的物件型別](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).

1. 按一下 **完成** 在熒幕的左下角。

   >[!TIP]
   >
   >您可以按一下 **套用** 建立自訂表單時，隨時儲存變更並保持表單開啟。

1. 如果您想要將新的自訂欄位新增到表單中，請繼續 [新增自訂欄位至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) 或 [在自訂表單中重複使用自訂欄位或Widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   或

   如果您想以其他方式繼續建置自訂表單，請繼續閱讀下列其中一篇文章：

   * [在自訂表單中新增或編輯資產Widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [在自訂表單中定位自訂欄位和Widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [新增分割槽符號至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [新增計算資料至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [在自訂表單中重複使用現有的計算自訂欄位](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [新增顯示邏輯和略過邏輯至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)

## 開始編輯自訂表單

您可以在自訂表單建立後隨時加以編輯。

>[!CAUTION]
>
>如需關於從自訂表單中移除欄位而不遺失使用者在這些欄位中輸入的資料的資訊，請參閱區段 [移除自訂欄位而不會遺失使用者輸入的資料](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md#remove) 在文章中 [從系統中刪除自訂欄位或Widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md).
>
>一般而言，建議您儘可能減少編輯已使用中的自訂表單的次數。 沒有通知系統可提醒使用自訂表單的人員您的變更。

{{step-1-to-setup}}

1. 按一下 **自訂Forms** 在左側面板中。

   自訂表單會顯示在清單中。 您可以檢閱為您的組織建立的所有自訂表單和自訂欄位。 您也可以檢視每個表單的建立者、與其相關聯的物件，以及表單是否處於作用中狀態。

1. 選取您要編輯的自訂表單，然後按一下 ![編輯圖示](assets/edit-icon.png).
1. （可選）若要變更自訂表單的標題和說明，請按一下 **表單設定** 標籤，然後輸入 **表單標題** 和 **說明**.

1. （選擇性）如果您想要將更多物件型別新增至表單，以便將其附加至更多物件，請按一下加號+之後 **物件型別**，然後在顯示的功能表中選取您想要的型別。

   ![](assets/add-object-type-existing-form.png)

   您可以重複此步驟，新增任意數目的物件型別。

   您也可以按一下物件型別上的X，將其從表單中刪除。 當您想要從已儲存的自訂表單中刪除物件型別時，應謹慎執行此操作。 如需詳細資訊，請參閱 [刪除自訂表單上的物件型別](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).

1. 按一下 **完成**.

   >[!TIP]
   >
   >您可以按一下 **套用** 建立自訂表單時，隨時儲存變更並保持表單開啟。

1. 如果您想要將新的自訂欄位新增到表單中，請繼續 [新增自訂欄位至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) 或 [在自訂表單中重複使用自訂欄位或Widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   或

   如果您想以其他方式繼續建置自訂表單，請繼續閱讀下列其中一篇文章：

   * [在自訂表單中新增或編輯資產Widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [在自訂表單中定位自訂欄位和Widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [新增分割槽符號至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [新增計算資料至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [在自訂表單中重複使用現有的計算自訂欄位](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [新增顯示邏輯和略過邏輯至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
