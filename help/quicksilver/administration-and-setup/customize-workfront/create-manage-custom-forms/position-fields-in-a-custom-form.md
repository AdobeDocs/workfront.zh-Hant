---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: 在自訂表單中使用舊版表單產生器來定位自訂欄位和Widget
description: 您可以在自訂表單中重新定位自訂欄位和Widget。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: f96425e3-8e20-43ac-8340-915538ae5886
source-git-commit: d32f274390f6ffc5fdd01c2c9b4b2abd99d7cb10
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 0%

---

# 在自訂表單中使用舊版表單產生器來定位自訂欄位和Widget

{{form-designer-default}}

您可以在自訂表單中重新定位自訂欄位和Widget。

如需自訂表單中自訂欄位和Widget的相關資訊，請參閱[新增自訂欄位至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)和[新增或編輯自訂表單中的資產Widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)。

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

## 在自訂表單中定位自訂欄位和Widget

1. 開始建立或編輯自訂表單，如[使用舊版表單產生器建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)中所述。
1. 新增自訂欄位和Widget至表單，如[使用舊版表單產生器將自訂欄位新增至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)和[使用舊版表單產生器新增或編輯自訂表單中的資產Widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)中所述。

1. （可選）若要將自訂欄位和Widget放置在同一列，請將其中一個拖曳到另一個旁邊，直到它們之間出現線條為止。

<!--
Courtney, this is a story that got postponed after I did the work. Slated for some time in 22.4 (https://hub.workfront.adobe.com/task/6220d425000140d7f7d3ea68cc9529c8/documents)
   You can drag multiple items. Press the following keys while you select the items, then drag the items together to the new row:
   * Mac: Command+Shift [Courtney, double-check these commands]
   * Windows: Ctrl+Shift

   When you drop the custom field or widget, a gray box displays around the two items to indicate that they share a row.
-->

>[!NOTE]
>
>* 您可以使用右下角的&#x200B;**預覽**&#x200B;按鈕，瞭解自訂欄位和Widget在表單中的顯示方式。
>* 描述性文字欄位無法共用列。
>* 自訂欄位和Widget不一定會在表單中以相同的方式顯示，取決於使用者檢視時可用的熒幕空間。 例如，如果水準間距受限，欄位列中的第三個欄位可能會換成下一列欄位。

1. （可選）若要將自訂欄位或Widget置於另一個欄位之上或之下，請將其拖曳至另一個欄位之上或之下，直到專案之間出現水準藍色線為止。
1. 按一下&#x200B;**套用**。
1. 如果您想以其他方式繼續建置自訂表單，請繼續閱讀下列其中一篇文章：

   * [使用舊版表單產生器將自訂欄位新增至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md#add2)
   * [使用舊版表單產生器，在自訂表單中新增或編輯資產Widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [使用舊版表單產生器將計算資料新增至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [使用舊版表單產生器將分割槽符號新增至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [新增顯示邏輯並略過邏輯至具有舊版表單產生器的自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [使用舊版表單產生器預覽並完成自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)
