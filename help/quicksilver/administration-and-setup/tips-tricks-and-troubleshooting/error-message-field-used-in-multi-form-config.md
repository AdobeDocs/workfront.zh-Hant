---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 錯誤訊息：發生輕微問題。 該欄位用於多表單設定
description: 當您在自訂表單的計算自訂欄位中變更計算時，出現一則錯誤訊息，告知您該欄位用於多表單設定時，您需要將該欄位取代為包含您要使用計算的新欄位。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 43668525-5572-4d82-8eed-0e320249f296
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '1241'
ht-degree: 0%

---

# 錯誤訊息：發生輕微問題。 該欄位用於多表單設定

## 問題

當您變更自訂表單上計算自訂欄位的計算時，[!DNL Adobe Workfront]可能會顯示以下警告：

出現一個小問題

[欄位]用於多表單設定，如果您想要變更此公式，您必須移除此欄位，並以包含所需計算的新欄位取代。

## 原因

至少兩個包含您嘗試變更的計算自訂欄位的自訂表單已附加至[!DNL Workfront]執行個體中的單一物件。

**範例：**&#x200B;自訂表單A和B都附加到相同工作。 兩個表單都包含名為「利潤」的計算自訂欄位。 當您嘗試在自訂表單A的利潤欄位中編輯計算時，會遇到錯誤。

您無法變更其中一個表單中自訂欄位的計算，因為這會與另一個表單中相同欄位中的公式衝突。
若要解決此衝突，您必須找到附加了具有相同計算自訂欄位的多個表單的物件，然後執行下列任一項作業：

* 從物件移除其中一個表單。
* 視需要變更計算，但在附加到物件的所有自訂表單中變更計算。
* 在附加到物件的所有自訂表單中，新增包含所需計算的新計算自訂欄位，並將舊的計算自訂欄位標籤為過時。

本文會說明如何尋找物件，然後透過以下三種方式之一解決問題。

## 尋找已附加自訂表單的物件 {#find-the-object-where-the-custom-forms-are-attached}

{{step-1-to-setup}}

1. 按一下&#x200B;**[!UICONTROL 自訂Forms]** > **[!UICONTROL 欄位]**。
1. 套用&#x200B;**[!UICONTROL 欄位清單]**&#x200B;檢視以尋找您嘗試修改的計算欄位，並記下使用它的每個自訂表單（例如，表單1、表單2、表單3） 。
1. 按一下&#x200B;**[!UICONTROL Forms]**，然後套用&#x200B;**[!UICONTROL 表單清單]**&#x200B;檢視。
1. 按一下&#x200B;**[!UICONTROL 篩選器]**&#x200B;下拉式清單，然後&#x200B;**[!UICONTROL 新增篩選器]**。

1. 按一下&#x200B;**[!UICONTROL 新增篩選規則]**，然後開始輸入「自訂表單名稱」，並在清單中顯示時選取此值。
1. 針對篩選修飾元選取&#x200B;**[!UICONTROL 等於]**，開始輸入您在步驟1中記下的每個表單的名稱，然後在其顯示時選取它。

   **範例：**&#x200B;自訂表單名稱等於Form 1、Form 2、Form 3。

1. 按一下&#x200B;**[!UICONTROL 儲存篩選器]**，然後命名新篩選器，再按一下&#x200B;**[!UICONTROL 儲存篩選器]**。

1. 在表單清單中，記下顯示在&#x200B;**[!UICONTROL 型別]**&#x200B;欄中的篩選器物件型別，例如「任務」或「問題」。
1. 在步驟1找到的每個自訂表單上，建立一個新的核取方塊自訂欄位，其單一預設值為「是」。

   **範例：**&#x200B;表單1的欄位1 =是，表單2的欄位2 =是，表單3的欄位3 =是。 這表示「計算自訂欄位存在於表單1中」或「計算自訂欄位存在於表單2中」等等。

1. 在熒幕右上角的&#x200B;**[!UICONTROL 搜尋圖示]** ![搜尋圖示](assets/search-icon.png)中，按一下&#x200B;**[!UICONTROL 進階搜尋]**。
1. 按一下自訂表單的物件（例如問題），按一下&#x200B;**[!UICONTROL 篩選結果]**，然後按一下&#x200B;**[!UICONTROL 新增篩選器]**。
1. 在&#x200B;**[!UICONTROL 開始輸入欄位名稱]**&#x200B;欄位中輸入Checkbox欄位的名稱，並在該欄位顯示在清單中時加以選取，然後選取&#x200B;**[!UICONTROL 等於]**&#x200B;並在下列方塊中輸入&#x200B;**[!UICONTROL 是]** （不含引號）。

   **範例：**&#x200B;欄位1等於（區分大小寫） Yes。

1. 按一下&#x200B;**[!UICONTROL 新增篩選器]**，並將所有核取方塊欄位新增至您的進階搜尋。

   尋找所有可能的組合。

   **範例：**&#x200B;使用您找到的組合建置多個篩選器，如下所示。 您應該會找到物件，其中包含多個包含相同計算欄位的附加自訂表單。 您可能會發現下列案例：

   * 欄位1=是+欄位2 =是+欄位3 =是（例如，沒有物件）
   * 欄位1=是+欄位2 =是（例如，沒有物件）
   * 欄位1=是+欄位3 =是（例如兩個物件）

   這表示計算欄位同時存在於表單1和表單3中，因為對應的核取方塊欄位（欄位1和欄位3）存在於這些物件中。

   欄位2 =是+欄位3 =是（例如，沒有物件）

1. 請繼續閱讀本文中下列其中一節：

   * [從物件移除其中一個自訂表單，並在其中編輯計算](#remove-one-of-the-custom-forms-from-the-object-and-edit-the-calculation-there)
   * [在所有附加的自訂表單的計算中進行相同的編輯](#make-identical-edits-in-the-calculation-in-all-of-the-attached-custom-forms)
   * [將包含已編輯計算的新計算欄位新增至一個或所有附加的自訂表單](#add-a-new-calculated-field-containing-the-edited-calculation-to-one-or-all-of-the-attached-custom-forms)

## 從物件移除其中一個自訂表單，並在其中編輯計算 {#remove-one-of-the-custom-forms-from-the-object-and-edit-the-calculation-there}

1. 尋找已附加自訂表單的物件，如[在本文章中尋找已附加自訂表單的物件](#find-the-object-where-the-custom-forms-are-attached)中所述，然後開啟該物件。
1. 從物件中移除其中一個自訂表單，然後儲存物件。

   >[!NOTE]
   >
   >若要從您從物件移除的表單新增欄位，您可能需要編輯仍附加至物件的自訂表單。 如此一來，您便可保留物件的自訂資料資訊。

1. 在您移除的自訂表單中，編輯您最初嘗試更新的自訂欄位計算，然後按一下[儲存]。****

   此時，[!DNL Workfront]不應發生衝突。

1. （選用）從自訂表單中移除核取方塊欄位，或從[!DNL Workfront]中刪除這些欄位。

## 在所有附加的自訂表單的計算中進行相同的編輯 {#make-identical-edits-in-the-calculation-in-all-of-the-attached-custom-forms}

>[!IMPORTANT]
>
>當您按照這些步驟操作時，已附加自訂表單的物件中的資料會遺失。 但是，如果計算欄位參考靜態欄位，而不是計算欄位，您可以在物件上使用[!UICONTROL 重新計算自訂運算式]選項來還原遺失的資料

1. 尋找已附加自訂表單的物件，如本文中[尋找已附加自訂表單的物件](#find-the-object-where-the-custom-forms-are-attached)中所述。
1. 從附加到物件的所有自訂表單中移除欄位，然後儲存表單。

1. 將包含新計算的自訂欄位新增回自訂表單。

   >[!IMPORTANT]
   >
   >所有附加的自訂表單中的計算內容必須相同。

1. （選用）從表單中移除核取方塊欄位，或從[!DNL Workfront]中刪除這些欄位。

## 將包含已編輯計算的新計算欄位新增至一個或所有附加的自訂表單 {#add-a-new-calculated-field-containing-the-edited-calculation-to-one-or-all-of-the-attached-custom-forms}

為避免遺失現有計算自訂欄位中的資料，或如果您只需要其中一個附加到您找到物件的自訂表單中進行編輯計算：

1. 尋找已附加自訂表單的物件，如本文中[尋找已附加自訂表單的物件](#find-the-object-where-the-custom-forms-are-attached)中所述。
1. 新增新的計算自訂欄位，其中包含您需要的計算，以新增一個或所有表單。
1. 重新命名舊的計算自訂欄位&#x200B;**過時**。

   在附加到物件的所有表單上，這個較舊的計算自訂表單會保留其歷史資料，但使用者會停止使用它。

   >[!IMPORTANT]
   >
   >舊欄位可能會在其他計算自訂欄位中參照，因此您需要在變更名稱后更新這些計算。

1. （選用）從表單中移除核取方塊欄位，或從Workfront中刪除這些欄位。

<!--
<blockquote data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Problem</h2>
<p>You get the following error while editing a calculated Custom Field on a custom form: </p>
<p><em>"<Name of custom field> field is used in a multi-form configuration, if you would like to change this formula you will need to remove this field and replace it with a new one containing the desired calculation."</em> </p>
<h2>Cause</h2>
<p>The error occurs because the following setup exists: currently you have at least one object in your system that has multiple custom forms attached. The calculated field you are editing exists on multiple forms attached to these objects.</p>
<p>You cannot have the same calculated field with different calculations on the same object. For this reason, the system does not allow you to make a change which will result in calculations being different.</p>
<p><a href="../../Resources/Images/Admin and setup/Tips, Tricks, and Troubleshooting/Calculated_field_error.png" class="MCXref xref" xrefformat="{para}"><img src="assets/calculated-field-error.png" alt="" width="542" height="272"></a> </p>
<p>For example, you have a task with custom forms A and B attached to it. Both forms contain the same calculated field, Field 1. You encounter this error when you try to edit the calculation for Field 1 on custom form A. </p>
<h2>Solution</h2>
<p>Remove the field from the custom form and replace it with a new one containing the desired calculation.  </p>
<p>To understand what custom forms are attached to objects, you can build a report for those objects and reference the Category Name field in the view of the report.<br>For more information about referencing custom forms in reports, see the "Referencing Custom Forms in a Report View (Column)" section in <a href="../../reports-and-dashboards/reports/creating-and-managing-reports/reference-custom-form-report.md" class="MCXref xref" xrefformat="{para}">Reference a custom form in a report</a>.</p>
<p>To understand what custom form contains a Custom Field, see the "Accessing Custom Forms and Fields" section in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/custom-forms-overview.md" class="MCXref xref" xrefformat="{para}">Custom forms overview</a>.</p>
</blockquote>
-->
