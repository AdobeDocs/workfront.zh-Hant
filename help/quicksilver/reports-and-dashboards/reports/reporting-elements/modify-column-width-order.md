---
product-area: reporting
navigation-topic: reporting-elements
title: 修改欄寬和順序
description: 請參閱本文章，瞭解欄寬指引，以及如何在Workfront中變更欄寬和順序。
author: Nolan
feature: Reports and Dashboards
exl-id: ece3f908-a0da-45d4-9f4f-0b34c69ce8fa
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '1010'
ht-degree: 0%

---

# 修改欄寬和順序

<!-- Audited: 11/2024 -->

以下是有關Adobe Workfront中欄寬如何運作的准則：

* Workfront預設會定義清單和報告中的欄寬。
* 除非在欄的文字模式中另外指定，否則Workfront會根據所有清單和報告中的`valueformat`資訊自動調整欄的寬度。

  >[!NOTE]
  >
  >Workfront不會根據「設定」和「報告」區域中可用清單中的`valueformat`資訊調整欄寬。

  `valueformat`值定義資料行中顯示的資訊型別。 例如，顯示數字的欄比顯示「說明」欄位的欄窄。

* 您可以根據自己的需求，自訂Workfront清單和報告中的欄寬。

  您可以在檢視清單或報表時暫時修改欄的寬度，或是透過在檢視產生器中調整欄的寬度來永久修改。 如需暫時修改欄寬的相關資訊，請參閱本文中暫時修改欄寬和順序時的[考量事項](#considerations-when-temporarily-modifying-the-width-and-order-of-columns)一節。

* 內建檢視中顯示的欄具有先前由Workfront定義並以硬式編碼撰寫的寬度。 若要修改這些寬度，您必須使用檢視產生器中的文字模式，手動更新這些欄的寬度。

  如需有關在文字模式中修改欄的資訊，請參閱[檢視：永久編輯欄寬](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-edit-column-width-permanently.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront計畫*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront授權*</strong></td> 
   <td> 
      <p>新增：</p>
         <ul>
         <li><p>投稿人或以上</p></li>
         </ul>
      <p>目前：</p>
         <ul>
         <li><p>要求或更高版本</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>存取層級設定*</strong></td> 
   <td> <p>編輯對篩選器、檢視、群組的存取權</p> <p>編輯報告、儀表板、行事曆的存取權，以編輯報告中的檢視</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件許可權</strong></td> 
   <td> <p>管理報表的許可權，以編輯報表中的檢視</p> <p>管理檢視的許可權以進行編輯</p></td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 修改欄寬和順序

您可以透過下列方式，修改報表中的欄寬和順序：

* [暫時修改資料行的寬度和順序](#modify-width-and-order-of-columns-temporarily)
* [永久修改欄寬和順序](#modify-width-and-order-of-columns-permanently)

### 暫時修改欄寬和順序 {#modify-width-and-order-of-columns-temporarily}

您可以拖曳欄框線來調整欄大小，拖放欄暫時在整個Workfront網站的大部分清單中重新排序。 這包括報告、檢視、控制面板的報告和甘特圖。

如需Workfront清單的詳細資訊，請參閱文章[開始使用Adobe Workfront中的清單](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)。

* [暫時修改資料行寬度和順序時的考量事項](#considerations-when-temporarily-modifying-the-width-and-order-of-columns)
* [暫時調整資料行大小](#resize-columns-temporarily)
* [暫時重新排序欄](#reorder-columns-temporarily)

#### 暫時修改欄寬和順序時的注意事項 {#considerations-when-temporarily-modifying-the-width-and-order-of-columns}

您可以暫時修改清單中欄的寬度和順序，而無需編輯其檢視。

暫時調整欄大小和排序欄時，請注意下列事項：

* 在調整欄大小時新的欄大小會儲存在瀏覽器的本機儲存體中，並依預設儲存。 使用不同的瀏覽器、清除快取或瀏覽資料會導致欄大小恢復為預設值。 重新整理頁面可保留您對欄寬所做的變更。

>[!NOTE]
> 
>欄寬受到瀏覽器視窗大小的限制；如果重新整理頁面，欄寬將會減少，直到所有欄都能符合視窗大小，而沒有水準捲動。 若要強制欄位保持比瀏覽器可容納的寬度還寬，您必須在文字模式中設定欄位寬度，如[永久修改欄位寬度和順序](#modify-width-and-order-of-columns-permanently)中所述，並避免透過拖曳欄位寬度來手動調整欄位寬度。
>

* 重新排序欄時，只會維持您選擇的順序，直到您離開清單或重新整理瀏覽器頁面為止。 離開清單或重新整理瀏覽器頁面後，欄會恢復其預設順序。
* 為獲得最佳效能，您重新排序的欄在清單中不應超過100個專案。
* 當您調整欄大小時，您的變更只會套用至您目前使用的檢視，而且只有您能看見。 與其他使用者共用檢視時，不會共用您已定義的欄大小。
* 在透過向右拖曳欄框來調整欄大小之後，除了下列情況外，會保留相鄰欄的寬度：

   * 設定區域
   * 報告區域
   * 檔案清單與報告

  >[!NOTE]
  >
  >您無法將欄的左邊框移動到任何清單中相鄰欄的左邊框之外。

* 如果將任何清單匯出到檔案，則欄的暫時順序不會轉移到匯出的檔案。 匯出的檔案會顯示原始清單中欄的順序，然後才重新排序欄。

如需有關從清單和報告匯出資料的詳細資訊，請參閱文章[匯出資料](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md)。

#### 暫時調整欄大小 {#resize-columns-temporarily}

1. 移至您要修改的清單。
1. 拖曳欄標題的框線，直到欄達到所需大小。\
   ![](assets/column-resize-350x124.png)

#### 暫時重新排序欄 {#reorder-columns-temporarily}

1. 移至您要修改的清單。
1. 按一下並拖曳您要移動至所需位置的欄標題。

>[!TIP]
>
>這在同時檢視甘特圖和清單檢視時特別有用。 檢視甘特圖時，欄可能會變成隱藏。 若要在顯示甘特圖時檢視欄，只要拖曳您要檢視的欄，使其顯示在頁面左側即可。

### 永久修改欄寬和順序 {#modify-width-and-order-of-columns-permanently}

若要永久重新排序欄，請參閱文章[在Adobe Workfront中的檢視總覽](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)中的[建立或自訂標準檢視](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-a-standard-view)一節。

您只能使用文字模式來永久修改欄寬。

如需有關使用文字模式和永久修改欄寬的詳細資訊，請參閱文章[文字模式的常見使用概述](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)。
