---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: 從系統中刪除自訂欄位或Widget
description: 為了改善系統效能並使表單更易於使用者使用，您可能想要在不再使用自訂欄位和Widget時從系統中將其移除。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c22a7ced-da81-40b5-bb4d-69d59b855add
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 0%

---

# 從系統中刪除自訂欄位或Widget

為了改善系統效能並使表單更易於使用者使用，您可能想要在不再使用自訂欄位和Widget時從系統中將其移除。

>[!CAUTION]
>
>刪除自訂欄位也會在填寫附加到物件的自訂表單時刪除使用者在欄位中輸入的所有自訂資料。 已刪除的資料無法復原。
>
>您可以檢視使用您要刪除之自訂欄位的所有自訂表單和報表，以評估可能造成的影響。 如需詳細資訊，請參閱[檢視使用特定自訂欄位或Widget的所有自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-custom-forms-that-use-a-particular-custom-field.md)和[檢視使用特定自訂欄位或Widget的所有報表](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-reports-that-use-a-particular-custom-field.md)。
>
>或者，為了因應措施，您可以避免遺失不再使用的欄位中的資料，請參閱[移除自訂欄位，而不會遺失使用者在此文章中輸入的資料](#remove-a-custom-field-without-losing-data-that-users-have-entered)。

## 存取需求

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

## 從系統中刪除自訂欄位或Widget

{{step-1-to-setup}}

1. 按一下&#x200B;**自訂Forms。**
1. 按一下&#x200B;**欄位**&#x200B;以開啟[欄位]區域。
1. 選取自訂欄位或Widget，然後按一下&#x200B;**刪除**。
1. 如果您確定想要永久刪除專案，以及（如果是自訂欄位）附加物件上所有相關的資料，請按一下[是，刪除] ****。

## 移除自訂欄位而不會遺失使用者輸入的資料 {#remove-a-custom-field-without-losing-data-that-users-have-entered}

>[!CAUTION]
>
>從包含超過500個欄位和Widget的自訂表單中移除自訂欄位無法復原。 如果移除欄位，則在表單具有少於500個欄位和Widget之前，無法重新新增該欄位。

1. 決定您要從原始自訂表單中移除哪些自訂欄位，但此時不要移除它們。
1. 建立新的自訂表格：

   1. 新增自訂欄位至您要從原始自訂表單中移除的新表單。

      如需詳細資訊，請參閱[使用表單設計工具](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)設計表單中[新增或現有欄位至自訂表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-new-or-existing-fields-to-your-custom-form)一節。

   1. 儲存新的自訂表格。

1. 將自訂表單的存取許可權製為只有具有管理存取權的使用者，如[共用自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md)中所述。
1. 將新的自訂表單套用至已套用原始自訂表單的物件，如[新增自訂表單至物件](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)中所述。

   套用新的自訂表單至這些物件可確保不會影響歷史報表資料。

1. 修改原始自訂表單，並移除您新增至新表單的自訂欄位（在步驟2中）。

   您從原始自訂表單中移除的欄位現在只能用於您建立的新自訂表單。 使用者可以看到物件上的自訂表單，但無權管理存取權的使用者無法修改自訂表單。
