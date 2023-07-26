---
title: 表單設計工具概觀
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 您可以設計使用者可附加至Workfront物件的自訂表單。 處理物件的使用者可以填寫自訂表格，以提供物件的相關資訊。
author: Courtney / Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c2e2901b-0558-4a63-ae3c-4c3a6edf0ff0
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 0%

---

# 表單設計工具概觀

您可以使用新的表單設計工具來設計使用者可附加至Workfront物件的自訂表單。 處理物件的使用者可以填寫自訂表格，以提供物件的相關資訊。

新的表單設計工具有一個新的畫布樣式工作區，可讓您同時檢視欄位、畫布和欄位設定。 它也可讓您在設計表單時拖放區段內的欄位。

<!-- add screenshot when field settings empty state is ready -->

## 如何存取新的表單設計工具

新表單設計工具與舊版表單產生器頂端都會有一個新按鈕。 您可以使用此按鈕，在舊版產生器和新設計工具之間切換。

![切換到新的表單設計工具](assets/switch-views.png)

## 表單設計工具可用的新功能

透過新的表單設計工具，我們將

* **複製欄位**：您現在可以直接從畫布按一下欄位上的「複製」圖示，複製現有欄位。

* **變更描述性文字的大小**：您現在可以將小型、中型或大型指派給描述性文字欄位。 您也可以在相同列上與其他欄位搭配使用。

* **使用預設區段**：如果表單建立者尚未在表單頂端新增區段，畫布中現在會顯示預設區段，以便使用者調整未指派自訂區段的欄位許可權。

  >[!NOTE]
  >
  >將表單附加至物件後，物件中就不會顯示預設區段。

## 功能即將推出

下列專案目前無法在表單設計工具中使用，但很快將會新增：

* 顯示/略過邏輯

* 篩選自動提示欄位

>[!IMPORTANT]
>
>使用新表單設計工具時，邏輯和預先輸入篩選器的現有設定不受影響。

### 顯示/略過邏輯

雖然在設計新的自訂表單時您還無法新增顯示/略過邏輯，但您可以檢視在舊版表單產生器中建立的表單上的現有顯示/略過邏輯。

表單設計工具中欄位上的圖示表示邏輯已套用至欄位。

此 ![目標欄位的顯示邏輯](assets/display-logic-bottom-left.png) 圖示左下方的表示此欄位是顯示邏輯的目標欄位（如果已在表單上進行特定選取，則會顯示此欄位）。 此 ![定義顯示邏輯圖示](assets/display-logic-bottom-right.png) 圖示右下角表示此欄位用於定義顯示邏輯（此欄位上的特定選取範圍或值會顯示目標欄位）。

此 ![目標欄位的略過邏輯](assets/skip-logic-bottom-left.png) 圖示左下方的表示欄位是跳過邏輯的目標欄位（如果已在表單上做出特定選擇，則表單會向前跳過此欄位）。 此 ![定義略過邏輯圖示](assets/skip-logic-bottom-right.png) 圖示右下角表示此欄位用於定義略過邏輯（此欄位上的特定選取範圍或值會略過其他欄位，並直接移至目標欄位）。

![邏輯圖示](assets/logic-icons-3.png)

選取已套用邏輯的欄位，會顯示欄位設定中的現有邏輯規則。

![邏輯規則](assets/form-designer-view-only-logic.png)

## 從表單設計工具中移除的功能

我們已從表單設計器內部移除下列功能：


* 表單設定，表單共用，欄位共用索引標籤

   * 表單設定現在可在畫布頂端使用

   * 「表單共用」主要標籤和「欄位共用」子標籤

  >[!NOTE]
  >
  >您可以從「設定>自訂Forms > Forms」或「欄位」索引標籤控制表單和欄位共用。

* 追蹤更新摘要中的欄位變更
  >[!NOTE]
  >
  >您可以在「設定>介面>更新摘要」中找到此專案
