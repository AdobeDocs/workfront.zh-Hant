---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: 從系統中刪除自訂欄位或介面工具集
description: 為了改善系統效能並讓表單更方便使用者使用，您可能想要在自訂欄位和介面工具集不再使用時，從您的系統中移除這些欄位和介面工具集。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c22a7ced-da81-40b5-bb4d-69d59b855add
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 0%

---

# 從系統中刪除自訂欄位或介面工具集

為了改善系統效能並讓表單更方便使用者使用，您可能想要在自訂欄位和介面工具集不再使用時，從您的系統中移除這些欄位和介面工具集。

>[!CAUTION]
>
>刪除自訂欄位也會刪除使用者在填寫附加至物件的自訂表單時，在欄位中輸入的所有自訂資料。 已刪除的資料無法恢復。
>
>您可以檢視使用您要刪除之自訂欄位的所有自訂表單和報表，以評估可能造成的後果。 如需詳細資訊，請參閱 [檢視使用特定自訂欄位或介面工具集的所有自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-custom-forms-that-use-a-particular-custom-field.md) 和 [檢視使用特定自訂欄位或介面工具集的所有報表](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-reports-that-use-a-particular-custom-field.md).
>
>或者，如需因應措施，您可以避免在已不再使用的欄位中遺失資料，請參閱 [移除自訂欄位，但不會遺失使用者已輸入的資料](#remove-a-custom-field-without-losing-data-that-users-have-entered) 這篇文章。

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

## 從系統中刪除自訂欄位或介面工具集

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **自訂Forms。**
1. 按一下 **欄位** 標籤。
1. 選取自訂欄位或介面工具集，然後按一下 **刪除**.
1. 如果您確定要永久刪除項目，並（在自訂欄位中）在附加項目的對象上的所有關聯資料，請按一下 **是，刪除它**.

## 移除自訂欄位，但不會遺失使用者已輸入的資料 {#remove-a-custom-field-without-losing-data-that-users-have-entered}

>[!CAUTION]
>
>從具有500多個欄位和小工具的自訂表單中移除自訂欄位時，無法還原。 如果移除欄位，則在表單的欄位和小部件少於500個之前，無法重新添加該欄位。

1. 確定要從原始自定義表單中刪除的自定義欄位，但此時不刪除。
1. 建立新的自訂表單，如 [建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

   1. 將自訂欄位新增至您要從原始自訂表單中移除的新表單，如 [在自訂表單中重複使用自訂欄位或介面工具集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).
   1. 儲存新的自訂表單。

1. 將對自訂表單的存取限制為僅限具有管理存取權限的使用者，如 [共用自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).
1. 將新自定義表單應用於已應用原始自定義表單的對象，如 [將自訂表單新增至物件](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

   將新的自訂表單套用至這些物件，可確保歷史報表資料不受影響。

1. 修改原始自訂表單，並移除您新增至新表單的自訂欄位（在步驟2中）。

   您從原始自訂表單中移除的欄位現在只能在您建立的新自訂表單中使用。 使用者可以在物件上看到自訂表單，但無管理存取權的使用者無法修改自訂表單。
