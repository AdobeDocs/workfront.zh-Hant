---
title: 檢視使用特定自訂欄位或Widget的所有報表
description: 您可以在「自訂Forms」區域中新增自訂檢視，以顯示哪些報表正在使用特定自訂欄位或Widget。 當您需要編輯或刪除欄位或Widget時，這個用法很有用，因為它可能已在一個或多個報告中實作。 請務必評估這些報表是否需要調整，才能繼續正常運作。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: eaafe79b-bdbc-4fb9-b449-23e5a4bc455a
source-git-commit: 35de4535970d5cd15fcd68f79bf849803f94a77e
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 0%

---

# 檢視使用特定自訂欄位或Widget的所有報表

您可以在「自訂Forms」區域中新增自訂檢視，以顯示哪些報表正在使用特定自訂欄位或Widget。 當您需要編輯或刪除欄位或Widget時，這個用法很有用，因為它可能已在一個或多個報告中實作。 請務必評估這些報表是否需要調整，才能繼續正常運作。

如需自訂表單中自訂欄位和Widget的相關資訊，請參閱 [新增自訂欄位至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) 和 [在自訂表單中新增或編輯資產Widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

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

如需有關此表格的詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 列出使用特定自訂欄位或Widget的報告

{{step-1-to-setup}}

1. 在左側面板中，按一下 **自訂Forms**.
1. 按一下 **欄位** 顯示列出您Workfront執行個體中所有自訂欄位和Widget的報告。

1. 按一下 **檢視** 功能表，然後檢查清單中是否包含任何自訂檢視 **報表** 欄（不是此索引標籤上的預設欄）。

   「報表」欄是您檢視哪些報表正在使用系統中已新增至自訂表單的每個自訂欄位和Widget。 有人可能已經建立包含 **報表** 欄。

1. 如果您沒有看到包含 **報表** 欄，建立包含它的新檢視：

   1. 按一下 **檢視** 功能表，然後按一下 **新檢視**.

   1. 在 **新檢視** 出現的頁面，在左上角附近的方塊中，取代 **新增引數檢視** 具有檢視的描述性名稱，例如 *欄位和Widget*.

   1. 按一下 **新增欄** 靠近右下角。
   1. 在 **顯示在此欄中** 左上角附近顯示的方塊，開始輸入 *報告*，然後選取 **報表** 出現在方塊下方的清單中時。

   1. （視條件而定）如果要移動 **報表** 將您剛新增至不同水平位置的欄拖曳至 **欄預覽** 頁面底部的區域。

   1. 按一下 **完成**，然後按一下 **儲存檢視**.

1. 按一下 **檢視** 下拉式功能表，然後選取您剛建立的自訂檢視名稱。
1. 在 **名稱** 欄，尋找您要編輯或刪除的自訂欄位或Widget，然後檢視 **報表** 欄檢視哪些報表使用它（如果有的話）。

   若要尋找此欄的資訊，Workfront會在所有報表篩選器、檢視、分組中搜尋自訂欄位和Widget。

   如果您看到加號，可以按一下該文字行以顯示方塊，列出使用該欄位或Widget的所有其他報表。

   >[!NOTE]
   >
   >此工具的初始載入時間可能需要10秒到2.5分鐘，視系統中的資料量而定。

   >[!TIP]
   >
   >如果您沒時間調查使用自訂欄位或Widget的報告，可以按一下「匯出」來建立列出它們的檔案。 如果任何人擁有使用欄位或Widget的報告，您可以與其共用此檔案，並討論所需的變更、變更對報告可能造成的影響，以及需要採取哪些措施來確保報告可繼續正常運作。
   >
   >此檢視也可在引數報表中使用：
   >      
   > 1. 在主功能表中，按一下 **報表**.
   > 1. 在左上角附近，按一下 **新報告**，然後按一下 **引數** 在顯示的清單中。
   > 1. 按一下 **新增欄** 靠近右下角。
   > 1. 在 **顯示在此欄中** 左上角附近顯示的方塊，開始輸入 *報告*，然後選取 **報表** 出現在方塊下方的清單中時。
   > 1. （視條件而定）如果要移動 **報表** 將您剛新增至不同水平位置的欄拖曳至 **欄預覽** 頁面底部的區域。
   > 1. 按一下 **完成**，然後按一下 **儲存+關閉**.
   > 1. 輸入報表的描述性名稱，例如 *欄位和Widget*.
