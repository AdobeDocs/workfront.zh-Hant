---
title: 使用表單設計工具新增顯示邏輯和略過邏輯
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 您可以根據使用者在填寫自訂表單時所做的選擇，決定應顯示或略過哪些區段。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 5f5dbeb5-b974-489c-8f4d-ebaa00f5e5ba
source-git-commit: df6b1e4b362807025f3edb5298e8445c0d44ec69
workflow-type: tm+mt
source-wordcount: '1270'
ht-degree: 0%

---

# 使用表單設計工具新增顯示邏輯和略過邏輯

您可以根據使用者在填寫自訂表單時所做的選擇，決定應顯示或略過哪些區段。

>[!NOTE]
>
>邏輯僅適用於一個表單，且不能以來自不同表單的選擇為基礎。

## 存取需求

您必須具備下列專案才能執行本文所述的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront計畫 </td> 
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
   <td>管理自訂表單的存取權 </td> 
  </tr>  
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 顯示和略過邏輯圖示

自訂表單會顯示圖示，指出要套用至特定欄位的邏輯。 表單設計工具中欄位上的圖示表示邏輯已套用至欄位。

| 圖示 | 表單設計工具中欄位的位置 | 定義 |
|--- |--- |--- |
| ![目標欄位的顯示邏輯](assets/display-logic-bottom-left.png) | 左下方 | 欄位是顯示邏輯的目標欄位。 如果在表單上做了特定選擇，則會顯示此欄位。 |
| ![定義顯示邏輯圖示](assets/display-logic-bottom-right.png) | 右下方 | 欄位會定義顯示邏輯。 此欄位中的特定選取範圍或值會顯示目標欄位。 |
| ![目標欄位的略過邏輯](assets/skip-logic-bottom-left.png) | 左下方 | 欄位是略過邏輯的目標欄位。 如果對表單進行了特定選擇，則表單會前進到此欄位，並且之間的欄位會隱藏。 |
| ![定義略過邏輯圖示](assets/skip-logic-bottom-right.png) | 右下方 | 此欄位會定義略過邏輯。 此欄位上的特定選取範圍或值會略過其他欄位，並直接移至目標欄位。 |

![邏輯圖示](assets/logic-icons-3.png)

選取已套用邏輯的欄位，以在欄位設定中顯示現有的邏輯規則。

![邏輯規則](assets/form-designer-view-only-logic.png)

## 使用顯示邏輯和略過邏輯的考量事項

* 若要在自訂欄位、Widget或分割槽符號上新增顯示邏輯，表單上必須至少有一個多選欄位（選項按鈕、下拉清單或核取方塊）位於該欄位之前。
如需自訂表單中自訂欄位和Widget的相關資訊，請參閱 [使用表單設計工具設計表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
* 您無法將跳過邏輯新增至Widget或分割槽符號。 您只能將其新增至多選欄位（選項按鈕、下拉式清單或核取方塊）。
* 如果自訂欄位符合以下所有條件，則您可以將顯示邏輯和略過邏輯新增到自訂欄位：

   * 它是一個多選欄位（單選按鈕、下拉清單或覈取方塊）
   * 它前面有複選欄位
   * 後面接著另一個自訂欄位

* 複製具有顯示邏輯或跳過邏輯的表單時，邏輯會複製到新的自訂表單。
* 大量編輯物件時，所有自訂欄位都會顯示在「編輯物件」方塊中，包括略過或隱藏的欄位。
* 為自訂表單建立顯示邏輯規則時，請記住下列事項：

   * 預設情況下，顯示邏輯陳述式中未包含的自訂欄位會顯示在自訂表單上。
   * 您可以建立多欄位顯示邏輯陳述式。
   * 如果分割槽符號下的所有欄位都套用了顯示邏輯，並且它們都因該邏輯而隱藏，則整個分割槽將在自訂表單上隱藏。

## 新增顯示邏輯至自訂表單

顯示邏輯定義當使用者在多重選擇欄位中選擇特定值時，要在表單上顯示的自訂欄位。 此邏輯會新增至目標欄位，並僅在選取值時顯示。

{{step-1-to-setup}}

1. 按一下 **自訂Forms**.
1. 建立新的自訂表單或開啟現有的表單。 另請參閱 [使用表單設計工具設計表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) 以取得詳細資訊。
1. 視需要新增欄位至表單。 至少一個多選欄位（單選按鈕、下拉清單或核取方塊）必須放在將顯示的目標欄位之前。
1. 選取目標欄位並按一下 **新增邏輯** 在熒幕左下角。
1. 選取 **顯示邏輯** 標籤。
1. 按一下 **新增顯示規則** 在邏輯產生器上。

   ![顯示邏輯產生器](assets/custom-form-logic-builder-display-blank.png)

1. 請依照下列在產生器中的步驟建立邏輯陳述式。

   1. 第一個選項是選擇定義欄位。 此欄位具有顯示目標的選取值。 它必須是多選欄位。
   1. 第二個選項是選擇選取值。 只有已為該欄位定義的值才可使用。
   1. 第三個選項是 **已選取** 或 **未選取**. 選擇 **已選取** 表示選取值時，會顯示目標欄位。 選擇 **未選取** 表示在定義欄位中選取任何其他值時，會顯示目標欄位。
   1. 若要新增 **與** 將規則新增至邏輯陳述式，按一下 **新增規則** 直接位於您剛建立的規則底下。 依照相同的提示來建置規則。 必須符合所有的And規則，目標欄位才會顯示。

      ![顯示邏輯產生器](assets/custom-form-logic-builder-display1.png)

   1. 若要新增 **或** 將規則新增至邏輯陳述式，按一下 **新增規則** 靠近邏輯產生器底部。 然後，按一下 **新增規則** 在「或」區域中，依照相同的提示來建置規則。 當滿足一個Or規則時，將顯示目標欄位。

1. 按一下 **儲存** 完成邏輯陳述式的建置後。

   顯示邏輯圖示會新增至表單設計工具的目標欄位和定義欄位。

## 將跳過邏輯新增至自訂表單

跳過邏輯定義自訂表單欄位，當使用者在多重選擇欄位中選擇特定值時，將跳過這些欄位。 略過的欄位會隱藏在表單上。 邏輯會套用至進行選取的定義欄位，而非跳過的欄位。

{{step-1-to-setup}}

1. 按一下 **自訂Forms**.
1. 建立新的自訂表單或開啟現有的表單。 另請參閱 [使用表單設計工具設計表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) 以取得詳細資訊。
1. 視需要新增欄位至表單。 略過邏輯的定義欄位必須是多選欄位（選項按鈕、下拉式清單或核取方塊）。
1. 選取定義欄位並按一下 **新增邏輯** 在熒幕左下角。
1. 選取 **跳過邏輯** 標籤。
1. 按一下 **新增略過規則** 在邏輯產生器上。

   ![略過邏輯產生器](assets/custom-form-logic-builder-skip-blank.png)

1. 請依照下列在產生器中的步驟建立邏輯陳述式。

   1. 定義欄位會顯示在產生器中。 這是您選取要套用略過邏輯的欄位。
   1. 第一個選項是選擇選取值。 只有已為該欄位定義的值才可使用。
   1. 第二個選項是 **已選取** 或 **未選取**. 選擇 **已選取** 表示選取值時，會顯示目標欄位，並略過兩者之間的欄位。 選擇 **未選取** 表示在定義欄位中選取任何其他值時，會顯示目標欄位，並略過兩者之間的欄位。
   1. 第三個選項是目標欄位，或跳至的位置。 選取欄位名稱或 **表單結尾**. 您可能需要先按一下「空白」這個字，才能選取選項。

      ![略過邏輯產生器](assets/custom-form-logic-builder-skip1.png)

   1. 若要新增 **或** 將規則新增至邏輯陳述式，按一下 **新增規則** 靠近邏輯產生器底部。 然後，在相同的提示下選取選項以建置規則。 當一個 **或** 符合規則，則會顯示目標欄位。

1. 按一下 **儲存** 完成邏輯陳述式的建置後。

   略過邏輯圖示會新增至表單設計工具中的目標欄位和定義欄位。


