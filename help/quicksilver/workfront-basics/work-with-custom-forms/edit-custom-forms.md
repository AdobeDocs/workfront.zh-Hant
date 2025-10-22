---
product-area: projects;user-management
keywords: 編輯，表單，rtf，文字，特殊，格式，欄位，自訂，資訊，自訂，物件
navigation-topic: work-with-custom-forms
title: 編輯自訂表單欄位中的資訊
description: 將表單附加到物件後，您可以編輯自訂表單上的資訊。 如需有關將自訂表單新增至物件的資訊，請參閱將自訂表單新增至物件。
author: Alina
feature: Get Started with Workfront
exl-id: c2b6afde-91a8-4e17-8e1a-3428b48e500a
source-git-commit: 6ded38ef130fbcdde8d680f77f6db38fbd81efb4
workflow-type: tm+mt
source-wordcount: '1039'
ht-degree: 0%

---

# 編輯自訂表單欄位中的資訊

<!--Audited: 10/2025-->

將表單附加到物件後，您可以編輯自訂表單上的資訊。 如需將自訂表單新增至物件的相關資訊，請參閱[將自訂表單新增至物件](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront套件</p> </td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront授權</p> </td> 
   <td> <p>投稿人或以上</p> 
   <p>要求或更高版本</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯您要編輯自訂表單之物件的存取權</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>物件許可權</p> </td> 
   <td> 
    <ul> 
     <li> <p>針對您要編輯自訂表單的物件，提供Contribute或更高的許可權</p> </li> 
     <li><p>檢視您要編輯之欄位的許可權。</p></li> 
     <li><p>編輯表單上要編輯的欄位所在區段的許可權</p></li> 
    </ul></td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront plan*</p> </td> 
   <td>Team or higher</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront licenses*</p> </td> 
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to the object for which you want to edit the custom form</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Object permissions</p> </td> 
   <td> 
    <ul> 
     <li> <p>Contribute or higher permissions on the object for which you want to edit the custom form</p> </li> 
     <li>View permissions on the fields you want to edit. For information about sharing permissions for custom fields, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/manage-a-form/share-custom-fields.md" class="MCXref xref">Configure sharing for custom fields and widgets</a>.</li> 
     <li> <p>Edit permissions for the sections on the form where the fields you want to edit are located</p> </li> 
    </ul> <p>For information on requesting additional access for objects, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 先決條件

* 您的Workfront管理員或對自訂表單具有管理存取權的計畫使用者必須在您的環境中建立自訂表單。 如需詳細資訊，請參閱[建立自訂表格](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。
* 您必須將自訂表單附加至物件。

  如需如何將自訂表單套用至物件的詳細資訊，請參閱[新增自訂表單至物件](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)。

## 編輯自訂表單上的資訊

針對所有物件，編輯附加到物件的自訂表單上的資訊都是相同的。 如需哪些物件可以有自訂表單的詳細資訊，請參閱[自訂表單概觀](../../administration-and-setup/customize-workfront/create-manage-custom-forms/custom-forms-overview.md)。

1. 移至您想要編輯自訂表單資訊的物件。
1. 按一下左側面板中的&#x200B;**`<Object type>`詳細資料**。

   例如，編輯專案自訂表單的資訊時，請按一下&#x200B;**專案詳細資料**。

1. 捲動至自訂表單。 當有自訂表單附加至物件時，表單的名稱會顯示為詳細資訊區段中的區域。
1. 如有必要，請按一下自訂表單名稱左側的箭頭![](assets/expand-arrow-right.png)以展開它。
1. 在頁面的右上角附近，按一下「編輯」圖示![](assets/edit-icon.png)。
1. 開始在您有權存取的任何欄位中輸入資訊。

   ![](assets/click-in-field-to-edit-info-350x132.png)

   或

   如果表單上尚未輸入任何資訊，請按一下任何您有權存取的欄位的[新增+**]，開始輸入資訊。**

   ![](assets/plus-add-to-edit-info-350x180.png)

   如果將多個自訂表單附加到物件，您可以對每個表單執行此操作。

   根據您使用的欄位型別，請考慮下列事項：

   * 您只能為選項按鈕欄位選取一個選項。
   * 您可以在核取方塊欄位中選取一或多個選項，視表單建立者如何設定欄位而定。
   * 您可以根據表單建立者設定欄位的方式，在多選下拉欄位中選取一個或多個選項。
   * 只有當建立表單的使用者將文字欄位設定為「文字欄位」並輸入格式欄位時，您才能設定文字欄位的格式（粗體、斜體或底線）。 無法格式化單行文字欄位和段落文字欄位。
   * 只有在建立表單的使用者在建立欄位時已包含日期欄位型別中的時間，您才能更新該時間。

   如需有關所有欄位型別的資訊，請參閱[建立自訂表格](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

1. 按一下「**儲存變更**」。

   >[!IMPORTANT]
   >
   >您必須先完成表單上的所有必填欄位，然後才能儲存表單。 必要欄位的名稱后面會加上星號。
   >
   >![](assets/nwe-required-custom-field.png)

   當有人變更物件中由計算自訂欄位參考的其他物件資料時，變更不會自動反映在您的物件中。 如需有關手動更新物件中所有計算自訂欄位的資訊，請參閱本文中的[重新計算物件的所有計算自訂欄位](#recalculate-all-calculated-custom-fields-for-an-object)。

   修改頁面上的相依欄位時，會即時動態重新計算自訂表單上的計算欄位。 您可以在不儲存表單的情況下看到新的計算欄位值，但在您儲存變更之前，該值不會實際套用至表單和物件。 這適用於預設表單以及自訂表單的計算欄位。

   當您與清單中的其他物件一起大量編輯物件時，也可以手動更新物件的所有計算自訂欄位。 如需指示，請參閱編輯本文中的物件時[重新計算清單中多個物件的所有已計算自訂欄位](#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects)。

## 重新計算物件的所有已計算自訂欄位  {#recalculate-all-calculated-custom-fields-for-an-object}

>[!IMPORTANT]
>
>您必須有包含附加到物件之計算欄位的自訂表單，然後才能遵循本節中的步驟。


1. 移至要重新計算其自訂欄位的物件首頁面。
1. 按一下物件名稱右邊的&#x200B;**更多**&#x200B;功能表![](assets/more-icon.png)，然後按一下&#x200B;**重新計算運算式**。

   這會重新計算物件表單上的所有自訂欄位。

## 編輯物件時，重新計算清單中多個物件的所有計算自訂欄位 {#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will need to be edited when the bulk edit for objects update in NW)</p>
-->

根據您要重新計算自訂運算式的物件，您可以在下列區域這樣做：

* 在物件清單中，從清單頂端的「更多」選單。
* 在「編輯」方塊中，大量選取和編輯多個物件時。

若要從清單或報表大量編輯數個物件的自訂欄位，以手動方式重新計算這些物件：

1. 移至物件清單，其中包含具有計算欄位的自訂表單。
1. 選取要更新其計算自訂欄位的物件。
1. 按一下&#x200B;**編輯圖示**。
1. 按一下左側功能表中的[自訂Forms]&#x200B;**&#x200B;**，然後選取[重新計算自訂運算式]&#x200B;**&#x200B;**。
1. 按一下&#x200B;**儲存** **變更**。

   Workfront會為所有選取的物件計算所有自訂欄位。

若要從物件清單重新計算自訂運算式：

1. 前往專案清單或報告，然後選取一或多個專案。
1. 按一下&#x200B;**更多**&#x200B;功能表![](assets/more-icon.png)，然後按一下&#x200B;**重新計算自訂運算式**。

![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

Workfront會立即計算所有選定專案的所有自訂欄位。
並非所有物件的清單都有此功能。

>[!NOTE]
>
>根據您專案的複雜性，我們建議不要在大量重新計算已計算的自訂欄位時選取大量專案以確保最佳效能。 有些因素會導致專案過於複雜，包括多重相依性或指派，或大量自訂欄位。

