---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 將觸發程式模組新增至基本情境
description: 瞭解如何新增觸發程式模組，以允許案例定期尋找新請求並將它們轉換為專案。
author: Becky
feature: Workfront Fusion
source-git-commit: ea3f932e02ad8a9416747d4b9aefe89d087dd414
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# 將觸發程式模組新增至基本情境

觸發模組會放置在情境的開頭。 當指定服務發生變更時，這些模組會在特定條件發生變更時開始案例執行。 變更可以是建立新記錄、刪除記錄、更新記錄等。

輪詢模組會以設定的時間間隔檢查服務，並傳回在該時間間隔內發生變更的相關資訊。 如果沒有變更，則觸發器不會執行情境。

在此範例中，您將新增每15分鐘執行一次的觸發程式模組，並在有任何請求已提交至特定佇列時啟動案例。 然後此情境會將這些請求轉換為專案。

此範例修改中建立的案例 [建立基本情境](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

## 先決條件

您必須建立中所述的情境 [建立基本情境](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) 然後再執行此程式。

## 新增及設定觸發程式模組

### 新增觸發程式模組

1. 在案例編輯器中開啟案例。
1. 在第一個（搜尋）模組上按一下滑鼠右鍵，然後選取 **刪除模組**.

   模組已刪除，並保留空白預留位置。

1. 按一下空白模組，然後選擇 **Adobe Workfront** 從應用程式清單中。
1. 選取 **觀看記錄**.
1. 確認模組使用與案例中其他模組相同的連線。
1. 在「篩選」欄位中，選取 **僅限新記錄**.
1. 在「輸出」方塊中，選取 `ID`， `Name`、和 `Project ID`.
1. 按一下 **確定** 以儲存模組設定。

   「選擇開始位置」視窗會出現。

1. 選取 **從現在起**.

### 排程觸發程式模組

1. 按一下「監看紀錄」模組的時鐘。

   「排程」設定視窗會開啟。

1. 在執行案例欄位中，選取 **定期進行**.

1. 按一下 **確定**.

### 更新第二個模組

因為第一個模組已取代，第二個模組必須對應至新的第一個模組。

1. 開啟轉換物件模組。
1. 在「問題ID」欄位中，刪除黑色ID區塊。 區塊為黑色，因為其對應來源模組已無法使用。
1. 在第一個模組（觀看記錄）下方選取ID區塊，將其對應至第二個模組。
1. 按一下 **確定**.

### 測試並啟動

1. 前往Fusion所連線的Workfront環境並新增問題。
1. 按一下 **[!UICONTROL 執行一次]** 位於情境編輯器的左下角。
1. 檢查輸出，確保案例如預期般執行。
1. 當您滿意情境如預期般運作時，請按一下 **正在排程** 在熒幕左下角切換為 **開啟**.

   這會啟用情境。
1. 在 [!DNL Workfront Fusion]，按一下 **[!UICONTROL 儲存]** 靠近左下角，儲存情境的進度。

   >[!IMPORTANT]
   >
   >隨時儲存並測試情境。

## 資源

* 如需Webhook的詳細資訊，請參閱 [中的即時觸發器(webhook) [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/webhooks/instant-triggers-webhooks.md).
