---
product-area: reporting
navigation-topic: reporting-elements
title: 修改列寬和順序
description: 請閱讀本文，瞭解列寬指南以及如何在Workfront更改列寬和順序。
author: Nolan
feature: Reports and Dashboards
exl-id: ece3f908-a0da-45d4-9f4f-0b34c69ce8fa
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '990'
ht-degree: 0%

---

# 修改列寬和順序

以下是列寬在Adobe Workfront如何工作的指南：

* Workfront預設定義清單和報表中列的寬度。
* Workfront會根據 `valueformat`清單和報表中的資訊，除非在列的文本模式中另有指定。

   >[!NOTE]
   >
   >Workfront不根據 `valueformat` 清單中的資訊。

   的 `valueformat` 值定義列中顯示的資訊類型。 例如，顯示數字的列比顯示「說明」欄位的列窄。

* 您可以根據要在列中顯示的資訊類型，自定義Workfront清單和報表中列的寬度以滿足您的需要。

   在查看清單或報表時，可以臨時修改列寬，也可以通過調整視圖生成器中列的寬度來永久修改列寬。 有關臨時修改列寬的資訊，請參見 [臨時修改列的寬度和順序時的注意事項](#considerations-when-temporarily-modifying-the-width-and-order-of-columns) 的下界。

* 在內置視圖中顯示的列具有以前由Workfront定義的硬編碼寬度。 要修改這些寬度，必須使用視圖生成器中的文本模式手動更新這些列的寬度。

   有關在文本模式下修改列的資訊，請參見 [視圖：永久編輯列的寬度](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-edit-column-width-permanently.md)。

## 訪問要求

您必須具有以下訪問權限才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront計畫</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront許可證*</strong></td> 
   <td> <p>請求或更高 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>訪問級別配置*</strong></td> 
   <td> <p>編輯對篩選器、視圖、分組的訪問</p> <p>編輯對報表、儀表板、日曆的訪問以編輯報表中的視圖</p> <p>注：如果您仍然沒有訪問權限，請詢問您的Workfront管理員是否在您的訪問級別設定了其他限制。 有關Workfront管理員如何修改您的訪問級別的資訊，請參見 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自定義訪問級別</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>對象權限</strong></td> 
   <td> <p>管理對報表的權限以編輯報表中的視圖</p> <p>管理視圖的權限以編輯它</p> <p>有關請求附加訪問的資訊，請參見 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求訪問對象 </a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要瞭解您擁有的計畫、許可證類型或訪問權限，請與您的Workfront管理員聯繫。

## 修改列寬和順序

您可以通過以下方式修改報表中列的寬度和順序：

* [臨時修改列的寬度和順序](#modify-width-and-order-of-columns-temporarily)
* [永久修改列的寬度和順序](#modify-width-and-order-of-columns-permanently)

### 臨時修改列的寬度和順序 {#modify-width-and-order-of-columns-temporarily}

您可以拖動列邊框來調整列的大小，並拖放列以臨時重新排序整個Workfront站點的大多數清單中的列。 這包括報表、視圖、儀表板上的報表和甘特圖視圖。

有關Workfront清單的詳細資訊，請參閱文章 [開始使用Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)。

* [臨時修改列的寬度和順序時的注意事項](#considerations-when-temporarily-modifying-the-width-and-order-of-columns)
* [臨時調整列大小](#resize-columns-temporarily)
* [臨時重新排序列](#reorder-columns-temporarily)

#### 臨時修改列的寬度和順序時的注意事項 {#considerations-when-temporarily-modifying-the-width-and-order-of-columns}

可以臨時修改清單中列的寬度和順序，而無需編輯其視圖。

臨時調整列大小和對列排序時，請考慮以下事項：

* 調整列大小時，新列大小將儲存在瀏覽器的本地儲存中，並預設保存。 使用其他瀏覽器或清除快取或瀏覽資料將導致列大小恢復為預設值。 刷新頁面時，將保留對列寬所做的更改。
* 重新排序列時，您選擇的順序僅會保留，直到您從清單中導航或刷新瀏覽器頁。 從清單中導航或刷新瀏覽器頁面後，列將返回其預設順序。
* 為獲得最佳效能，要重新排序的列在清單中的項數不應超過100。
* 調整列大小時，所做的更改僅應用於您當前使用的視圖，並且僅對您可見。 與其他用戶共用視圖不會共用您定義的列大小。
* 通過將列的邊框向右拖動來調整列的大小後，將保留相鄰列的寬度，以下情況除外：

   * 設定區域
   * 「報告」區域
   * 文檔清單和報表

   >[!NOTE]
   >
   >不能將列的左邊框移到任何清單中相鄰列的左邊框。

* 如果將任何清單導出到檔案，則列的臨時順序不會傳輸到導出的檔案。 導出的檔案在重新排序列之前顯示原始清單中列的順序。

有關從清單和報表導出資料的詳細資訊，請參閱文章 [導出資料](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md)。

#### 臨時調整列大小 {#resize-columns-temporarily}

1. 轉到要修改的清單。
1. 拖動列的邊框，直到列達到所需大小。\
   ![](assets/column-resize-350x124.png)

#### 臨時重新排序列 {#reorder-columns-temporarily}

1. 轉到要修改的清單。
1. 按一下要移動到其他位置的列以選擇該列。
1. 將列拖到正確的位置。
1. 將列放入位置，將其移動。

   ![](assets/column-reorder-350x118.png)

>[!TIP]
>
>當同時查看甘特圖和清單視圖時，此功能特別有用。 查看甘特圖時，列可以變為隱藏。 要在顯示甘特圖時查看列，只需拖動要查看的列，使其顯示在頁面的左側。

### 永久修改列的寬度和順序 {#modify-width-and-order-of-columns-permanently}

要永久重新排序列，請參閱一節 [建立或自定義標準視圖](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-a-standard-view) 在文章中 [Adobe Workfront視圖概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)。

只能使用文本模式永久修改列的寬度。

有關使用文本模式和永久修改列寬的詳細資訊，請參閱文章 [文本模式常用概述](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)。
