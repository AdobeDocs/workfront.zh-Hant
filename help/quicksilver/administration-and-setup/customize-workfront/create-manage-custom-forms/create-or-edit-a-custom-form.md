---
title: 建立或編輯自訂表單
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 您可以建立或編輯新的自訂表單。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5712e82d-bd1d-4d8a-9a2a-1e19b562b9d1
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '876'
ht-degree: 0%

---

# 建立或編輯自訂表單

您可以建立或編輯新的自訂表單。 本文將對這兩項任務進行說明。

如需從現有表單建立新自訂表單的相關資訊，請參閱 [複製自訂表單以建立新表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/copy-custom-form-to-create-a-new-one.md).

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
   <td>計劃</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>管理對自訂表單的存取</p> <p>如需Workfront管理員如何授予此存取權的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用戶對特定區域的管理訪問權限</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取層級設定，請聯絡您的Workfront管理員。

## 開始建立自訂表單

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **自訂Forms** 中。

   在顯示的檢視中，您可以檢閱為貴組織建立的所有自訂表單和自訂欄位。 您也可以查看每個表單的建立者，以及與其相關聯的欄位。

1. 按一下 **新自訂表單。**
1. 請至少選擇一個要與自定義表單關聯的對象類型，然後按一下 **繼續**.

   ![](assets/choose-object-type.jpg)

1. 在 **表單設定** 頁簽 **表單標題** 和選填 **說明** 自訂表單。

1. （可選）如果要將更多對象類型添加到窗體中，以便它可以附加到更多對象，請在「對象類型」後按一下加號，然後在顯示的菜單中選擇要選擇的對象類型。

   您可以重複此操作，以添加任意數量的對象類型。也可以按一下某個對象類型上的X以從窗體中刪除它。

   有關從已保存的自定義表單中刪除對象類型的資訊，請參見 [刪除自訂表單上的物件類型](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).

1. 按一下 **完成**.

   >[!TIP]
   >
   >您可以按一下 **套用** 在您建立自訂表單時隨時儲存變更並保持表單開啟。

1. 如果要向表單添加新的自定義欄位，請繼續到 [新增自訂欄位至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) 或 [在自訂表單中重複使用自訂欄位或介面工具集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   或

   如果您想以其他方式繼續建立自訂表單，請繼續閱讀下列其中一篇文章：

   * [在自訂表單中新增或編輯資產介面工具集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [在自訂表單中放置自訂欄位和小工具](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [為自訂表單新增區段分頁](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [將計算資料新增至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [在自訂表單中重複使用現有的計算自訂欄位](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [新增顯示邏輯並略過邏輯至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)

## 開始編輯自訂表單

自訂表單建立後，您隨時都可以編輯。

>[!CAUTION]
>
>如需如何從自訂表單中移除欄位，而又不遺失使用者在這些欄位中輸入之資料的資訊，請參閱區段 [移除自訂欄位，但不會遺失使用者已輸入的資料](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md#remove) 在文章中 [從系統中刪除自訂欄位或介面工具集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md).
>
>一般而言，建議您將編輯已使用中自訂表單的次數減到最少。 沒有通知系統可提醒使用自訂表單的使用者您所做的變更。

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **自訂Forms** 中。

   在顯示的檢視中，您可以檢閱為貴組織建立的所有自訂表單。 您也可以查看每個表單的建立者、其適用的物件類型，以及其是否使用中。

1. 選取您要編輯的自訂表單，然後按一下 **編輯**.
1. （可選）若要變更自訂表單的標題和說明，請按一下 **表單設定** 標籤，然後輸入 **表單標題** 和 **說明**.

1. （可選）如果要將更多對象類型添加到表單中，以便它可以附加到更多對象，請在後面按一下加號+ **物件類型**，然後在顯示的功能表中選取您要的類型。

   ![](assets/add-object-type-existing-form.png)

   您可以重複此操作，以新增任意數量的物件類型。

   您也可以按一下物件類型上的X，將其從表單中刪除。 如果要從已儲存的自訂表單中刪除物件類型，請小心執行此操作。 如需詳細資訊，請參閱 [刪除自訂表單上的物件類型](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).

1. 按一下 **完成**.

   >[!TIP]
   >
   >您可以按一下 **套用** 在您建立自訂表單時隨時儲存變更並保持表單開啟。

1. 如果要向表單添加新的自定義欄位，請繼續到 [新增自訂欄位至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) 或 [在自訂表單中重複使用自訂欄位或介面工具集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   或

   如果您想以其他方式繼續建立自訂表單，請繼續閱讀下列其中一篇文章：

   * [在自訂表單中新增或編輯資產介面工具集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [在自訂表單中放置自訂欄位和小工具](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [為自訂表單新增區段分頁](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [將計算資料新增至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [在自訂表單中重複使用現有的計算自訂欄位](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [新增顯示邏輯並略過邏輯至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
