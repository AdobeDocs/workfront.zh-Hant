---
product-area: projects;user-management
navigation-topic: work-with-custom-forms
title: 管理附加到物件的自訂表單
description: 您可以更新附加至一個物件的自訂表單的顯示順序、移除它們，或是大量編輯自訂表單在多個物件上的顯示方式。
author: Alina
feature: Get Started with Workfront
exl-id: e5570a09-32cb-43e3-9c1d-4421db42fa24
source-git-commit: 78878fa3578e4f3a33baec3806298282d3909d8d
workflow-type: tm+mt
source-wordcount: '1109'
ht-degree: 0%

---

# 管理附加到物件的自訂表單

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

您可以更新附加至一個物件的自訂表單的顯示順序、移除它們，或是大量編輯自訂表單在多個物件上的顯示方式。

## 存取需求

您必須具有下列存取權才能執行本文所述的動作：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>要求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯您管理自訂表單之物件的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>您管理自訂表單之物件的Contribute許可權或更高版本</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 先決條件

* 您的Workfront管理員或對自訂表單具有管理存取權的計畫使用者必須在您的環境中建立自訂表單。 如需詳細資訊，請參閱[建立或編輯自訂表格](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)。
* 您必須將自訂表單附加至物件。

  如需如何將自訂表單套用至物件的詳細資訊，請參閱[新增自訂表單至物件](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)。

## 重新排序附加到物件的多個自訂表單 {#reorder-multiple-custom-forms-attached-to-an-object}

1. 前往您要變更新增自訂表單順序的物件，然後開始編輯物件。

   **範例：**&#x200B;例如，若要管理專案的自訂表單，請移至專案，按一下&#x200B;**更多**&#x200B;功能表![](assets/more-icon.png)，然後按一下&#x200B;**編輯** 。

1. 在專案、任務和問題的&#x200B;**自訂Forms**&#x200B;區段中，按一下自訂表單名稱旁的![](assets/move-icon---dots.png)圖示。 針對所有其他物件，按一下&#x200B;**管理Forms**。 只有在物件上附加了至少一個自訂表單時，才會顯示此選項。
1. 將表單![](assets/move-icon---dots.png)拖曳到清單中的新位置。
1. 針對專案、任務和問題自訂表單，按一下&#x200B;**儲存**。

   針對所有其他物件，按一下&#x200B;**我已完成管理** > **儲存變更**。

## 從物件移除自訂表單 {#remove-a-custom-form-from-an-object}

>[!IMPORTANT]
>
>當您從物件移除自訂表單時，在表單的自訂欄位中擷取的所有資訊都會遺失且無法復原。

1. 移至您要移除自訂表單的物件，並開始編輯該物件。

   例如，前往專案，按一下&#x200B;**更多**&#x200B;功能表![](assets/more-icon.png)，然後按一下&#x200B;**編輯** 。

1. 按一下&#x200B;**自訂Forms**。
1. 若是專案、任務和問題自訂表單，請按一下表單右側的&#x200B;**X**&#x200B;圖示，將其從物件中移除。

   針對所有其他物件，按一下[管理Forms] ****，然後按一下表單右側的&#x200B;**X**&#x200B;圖示，將其從物件中移除。

1. 按一下「**儲存**」。

## 管理包含相同自訂欄位的多個自訂表單

您可能會在附加到相同物件的多個自訂表單上顯示相同的欄位。 在此情況下，請考慮下列事項：

* 所有表單中的欄位值都相同。

  對於附加到相同物件的不同表單上的相同欄位，不能有不同的值。

* 如果在兩個不同的物件上有相同的計算欄位，它們的計算必須相同，以避免錯誤。 如需將計算欄位新增至包含多個表單的自訂表單的相關資訊，請參閱[將計算資料新增至自訂表單](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md) 。

## 大量編輯物件時管理多個自訂表單

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:-->

>[!NOTE]
>
>對於專案以外的所有物件，管理自訂表單至物件的方式都相同。
>
>如需大量新增自訂表單至專案的詳細資訊，請參閱文章[編輯專案](../../manage-work/projects/manage-projects/edit-projects.md)。

當您大量編輯已套用多個自訂表單的物件時，可以編輯自訂表單在這些物件上的顯示方式，以及編輯自訂表單之間的通用欄位。

只有附加到所有所選物件的自訂表單才能進行大量編輯。

若要在大量編輯物件時編輯多個自訂表單：

1. 在清單物件中，選取已附加自訂表單的物件，然後按一下&#x200B;**編輯**&#x200B;圖示![](assets/edit-icon.png)。
1. 按一下&#x200B;**自訂Forms**。

   您只能編輯附加到所有所選物件的自訂表單。

   僅附加到某些物件的自訂表單不顯示。

1. 開始編輯自訂表單上的欄位。

   編輯欄位時，視覺指示器會顯示在該欄位上，表示該欄位已編輯。

   如果欄位包含在多個自訂表單中，則當您更新其中一個表單上的欄位時，這些欄位的所有值都會更新到每個表單上。

1. 按一下&#x200B;**選取專案**&#x200B;下拉式功能表，並選取其他表單以新增至所有選取的物件。

   套用其他表單時，請考量下列事項：

   * 物件最多可以有10個自訂表單。
   * 只有當表單尚未套用至您正在編輯的任何物件時，才能套用表單。 已附加至其中一個物件的表單不會出現在下拉式功能表中。
   * 在您套用其他表單後，任何表單與其他表單相同的欄位都會顯示在&#x200B;**通用欄位**&#x200B;區段中，而且可以編輯它們。

1. （選擇性）如果您將自訂表單新增至所有物件，但尚未儲存物件，您可以變更自訂表單在物件上的顯示順序。

   如需變更表單順序的詳細資訊，請參閱本文中的[重新排序附加到物件的多個自訂表單](#reorder-multiple-custom-forms-attached-to-an-object)。

1. 按一下&#x200B;**移除表單**&#x200B;以從物件移除自訂表單。

   如需有關從物件移除自訂表單的詳細資訊，請參閱[從物件移除自訂表單](#remove-a-custom-form-from-an-object)。

   從數個物件大量移除表單時，請考量下列事項：

   * 如果您變更了表單，將其移除會導致您的變更遺失且無法復原。
   * 移除表單後，該表單中位於&#x200B;**通用欄位**&#x200B;區段中的所有欄位都將從此區段移除，並且無法在此處再編輯。

1. 按一下&#x200B;**還原表單**，將表單還原成您編輯物件之前的狀態。
1. （選擇性）按一下表單名稱旁的收合箭頭，一次收合一個表單。

   或

   按一下&#x200B;**摺疊Forms**&#x200B;以同時摺疊所有表單。

1. （可選）按一下表單名稱旁的展開箭頭，一次展開一個表單。

   或

   按一下&#x200B;**展開Forms**&#x200B;以同時展開所有表單。 

1. 按一下「**儲存變更**」。
