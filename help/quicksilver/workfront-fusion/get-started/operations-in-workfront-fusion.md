---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adobe Workfront Fusion中的作業
description: Adobe Workfront Fusion中的操作是由模組執行的任務。 基於追蹤目的，模組所執行的任何成功動作都是操作。
author: Becky
feature: Workfront Fusion
source-git-commit: 8d82fd10a6742f13f62b5479fafa5b42e567700f
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# 中的作業 [!DNL Adobe Workfront Fusion]

中的操作 [!DNL Adobe Workfront Fusion] 是由模組執行的任務。 基於追蹤目的，模組所執行的任何成功動作都是操作。

## 計算作業數目時的注意事項

* 一般而言，任何成功的動作步驟執行都會被視為作業。

* 案例中的第一個模組只會執行一次，且一律計為一項作業，即使它未傳回套件組合亦然。

* 其餘模組執行的次數取決於它們必須處理的組合數量。  一個套件組合的一個模組執行是單一作業。 彙總模組則為例外，計算為每一組處理中的套件組合執行一項作業。

* 作業計數於 [!UICONTROL 最終處理] 案例執行的階段。

* 以下為 **not** 計為作業：

   * 任何篩選步驟。

   * 任何發生錯誤或中斷的動作。

   * 因不符合路由規則而不執行的任何路由，例如遞補或停用的路由。

   * 任何未執行的動作，可能是因為篩選條件不允許資料通過，或是因為案例因錯誤而停止。

## 作業限制

貴組織可能有每月營運限制。 這是根據 [!DNL Workfront] 貴組織購買的計畫。 此 [!UICONTROL Ultimate] [!DNL Workfront] 計畫提供不限次數的作業。

如果您的組織有每月限制，當您接近限制時，您會收到通知。 如果您超過限制， [!DNL Workfront] 將會連絡您的組織，以確保您的計畫符合您的需求。

## 檢視過去30天內執行的作業數目

您可以看到顯示已執行作業數目的圖表。 這些圖表可在下列位置使用：

* **組織儀表板**：整個組織使用的作業
* **團隊儀表板**：此團隊擁有的案例使用的操作([!DNL Adobe Experience Cloud] 僅限)
* **案例詳細資訊頁面**：此情境使用的操作([!DNL Adobe Experience Cloud] 僅限)

