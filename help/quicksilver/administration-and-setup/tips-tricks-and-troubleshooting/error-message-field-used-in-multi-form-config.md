---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '''錯誤訊息：有個小問題。 該欄位用於多表單設定中」'
description: 在自訂表單的計算自訂欄位中變更計算時，如果出現錯誤訊息指出該欄位用於多表單設定，您需要將欄位取代為包含您要使用的計算的新欄位。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 43668525-5572-4d82-8eed-0e320249f296
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '1222'
ht-degree: 0%

---

# 錯誤訊息：有個小問題。 該欄位用於多表單設定

## 問題

當您變更自訂表單上計算自訂欄位的計算時， [!DNL Adobe Workfront] 可能會顯示下列警告：

出現一個小問題

[欄位] 用於多表單配置，如果要更改此公式，則需要刪除此欄位，並將其替換為包含所需計算的新欄位。

## 原因

您嘗試變更的計算自訂欄位中，至少有兩個自訂表單會附加至您 [!DNL Workfront] 例項。

**範例：** 自訂表單A和B都附加至相同的工作。 兩個表單都包含一個名為Profit的計算自訂欄位。 嘗試在自訂表單A的「利潤」欄位中編輯計算時，您會遇到錯誤。

您無法更改其中一個表單中自定義欄位的計算，因為這將與另一個表單中同一欄位中的公式衝突。
要解決此衝突，您必須找到附加了具有相同計算自定義欄位的多個表單的對象，然後執行以下操作之一：

* 從物件中移除其中一個表單。
* 視需要變更計算，但在附加至物件的所有自訂表單中執行此操作。
* 在附加至物件的所有自訂表單中，新增包含您需要之計算的新計算自訂欄位，並將舊的計算自訂欄位標示為過時。

本文以這三種方式之一，說明如何找到對象，然後解決問題。

## 尋找自訂表單附加所在的物件 {#find-the-object-where-the-custom-forms-are-attached}

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 使用者]** ![](assets/users-icon-in-main-menu.png).

1. 按一下 **[!UICONTROL 自訂Forms]** > **[!UICONTROL 欄位]**.
1. 套用 **[!UICONTROL 欄位清單]** 查看以查找您嘗試修改的計算欄位，並記錄使用該欄位的每個自定義表單（例如表單1、表單2、表單3）。
1. 按一下 **[!UICONTROL Forms]**，然後套用 **[!UICONTROL 表單清單]** 檢視。
1. 按一下 **[!UICONTROL 篩選]** 下拉式清單，然後 **[!UICONTROL 新增篩選]**.

1. 按一下 **[!UICONTROL 新增篩選規則]**，然後開始輸入「自訂表單名稱」，並在此值顯示在清單中時加以選取。
1. 選擇 **[!UICONTROL 等於]** 對於篩選修飾詞，開始鍵入您在步驟1中記下的每個表單的名稱，然後在顯示時選取該名稱。

   **範例：** 自訂表單名稱等於表單1、表單2、表單3。

1. 按一下 **[!UICONTROL 儲存篩選]**，然後為新篩選器命名，然後按一下 **[!UICONTROL 儲存篩選]**.

1. 在表單清單中，記下顯示在 **[!UICONTROL 類型]** 欄。
1. 在步驟1找到的每個自訂表單中，建立新的「核取方塊」自訂欄位，其單一預設值為「是」。

   **範例：** 表單1上的欄位1 =是，表單2上的欄位2 =是，表單3上的欄位3 =是。 這表示「表單1上有計算自訂欄位」或「表單2上有計算自訂欄位」等。

1. 在 **[!UICONTROL 搜尋圖示]** ![](assets/search-icon.png) 在畫面的右上角，按一下 **[!UICONTROL 進階搜尋]**.
1. 按一下自訂表單的物件（例如問題），然後按一下 **[!UICONTROL 篩選結果]**，然後按一下 **[!UICONTROL 新增篩選]**.
1. 開始在 **[!UICONTROL 開始鍵入欄位名稱]** 欄位，並在其顯示於清單時加以選取，然後選取 **[!UICONTROL 等於]** 和類型 **[!UICONTROL 是]** （不含引號）。

   **範例：** 欄位1等於（區分大小寫）是。

1. 按一下 **[!UICONTROL 新增篩選器]** 並將所有核取方塊欄位新增至進階搜尋。

   尋找所有可能的組合。

   **範例：** 使用您找到的組合建立數個篩選器，如下所列。 您應該會找到具有多個附加自訂表單的物件，這些表單包含相同的計算欄位。 您可能會發現下列情況：

   * 欄位1=是+欄位2 =是+欄位3 =是（例如無物件）
   * 欄位1=是+欄位2 =是（例如，無物件）
   * 欄位1=是+欄位3 =是（例如兩個物件）

   這表示計算欄位同時存在於表單1和表單3中，因為這些對象上存在相應的複選框欄位（欄位1和欄位3）。

   欄位2 =是+欄位3 =是（例如，無物件）

1. 繼續閱讀本文的以下其中一節：

   * [從物件中移除其中一個自訂表單，並在該處編輯計算](#remove-one-of-the-custom-forms-from-the-object-and-edit-the-calculation-there)
   * [在所有附加的自訂表單中進行相同的計算編輯](#make-identical-edits-in-the-calculation-in-all-of-the-attached-custom-forms)
   * [將包含已編輯計算的新計算欄位新增至附加的一或所有自訂表單](#add-a-new-calculated-field-containing-the-edited-calculation-to-one-or-all-of-the-attached-custom-forms)

## 從物件中移除其中一個自訂表單，並在該處編輯計算 {#remove-one-of-the-custom-forms-from-the-object-and-edit-the-calculation-there}

1. 尋找自訂表單附加所在的物件，如 [尋找自訂表單附加所在的物件](#find-the-object-where-the-custom-forms-are-attached) 在本文中，然後開啟物件。
1. 從物件中移除其中一個自訂表單，然後儲存物件。

   >[!NOTE]
   >
   >若要從您從物件中移除的表單中新增欄位，您可能需要編輯仍附加至物件的自訂表單。 這樣，您就可以保留物件的自訂資料資訊。

1. 在您移除的自訂表單中，編輯您原本嘗試更新之自訂欄位的計算，然後按一下 **[!UICONTROL 儲存]**.

   這次， [!DNL Workfront] 不應遇到衝突。

1. （可選）從自訂表單中移除核取方塊欄位，或從 [!DNL Workfront].

## 在所有附加的自訂表單中進行相同的計算編輯 {#make-identical-edits-in-the-calculation-in-all-of-the-attached-custom-forms}

>[!IMPORTANT]
>
>執行這些步驟時，資料會在已附加自訂表單的物件中遺失。 不過，如果計算欄位參考靜態欄位，而非計算欄位，您可以使用 [!UICONTROL 重新計算自定義運算式] 用於恢復丟失資料的對象上的選項

1. 尋找自訂表單附加所在的物件，如 [尋找自訂表單附加所在的物件](#find-the-object-where-the-custom-forms-are-attached) 這篇文章。
1. 從附加至物件的所有自訂表單中移除欄位，然後儲存表單。

1. 將包含新計算的自訂欄位新增至自訂表單。

   >[!IMPORTANT]
   >
   >所有附加的自訂表單中的計算必須相同。

1. （可選）從表單中移除「核取方塊」欄位，或將其從 [!DNL Workfront].

## 將包含已編輯計算的新計算欄位新增至附加的一或所有自訂表單 {#add-a-new-calculated-field-containing-the-edited-calculation-to-one-or-all-of-the-attached-custom-forms}

為了避免現有計算自定義欄位中丟失資料，或者只需要在附加到您找到的對象的自定義表單中編輯計算：

1. 尋找自訂表單附加所在的物件，如 [尋找自訂表單附加所在的物件](#find-the-object-where-the-custom-forms-are-attached) 這篇文章。
1. 新增新的計算自訂欄位，其中包含您需要的計算，以填入一或所有表單。
1. 重新命名舊的計算自訂欄位 **過時**.

   在附加至物件的所有表單上，這個舊的計算自訂表單會保留其歷史資料，但使用者不會再使用它。

   >[!IMPORTANT]
   >
   >其他計算的自訂欄位可能會參考較舊的欄位，因此您必須在變更欄位名稱后更新這些計算。

1. （選用）從表單中移除「核取方塊」欄位，或從Workfront中刪除欄位。

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
<p>For more information about creating a custom form and adding or removing fields from it, see <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref" xrefformat="{para}">Create or edit a custom form</a>.</p>
</blockquote>
-->
