---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 將觸發程式模組新增至基本情境
description: 瞭解如何新增觸發程式模組，以允許案例定期尋找新請求並將它們轉換為專案。
author: Becky
feature: Workfront Fusion
exl-id: 067ee6a1-f4c1-4602-ac39-0283255cced8
source-git-commit: 1196e2d7a6d6750944a7c6209222f07382abfee7
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# 將觸發程式模組新增至基本情境

觸發模組會放置在情境的開頭。 當指定服務發生變更時，這些模組會在特定條件發生變更時開始案例執行。 變更可以是建立新記錄、刪除記錄、更新記錄等。

輪詢模組會以設定的時間間隔檢查服務，並傳回在該時間間隔內發生變更的相關資訊。 如果沒有變更，則觸發器不會執行情境。

在此範例中，您將新增每15分鐘執行一次的觸發程式模組，並在有任何請求已提交至特定佇列時啟動案例。 然後此情境會將這些請求轉換為專案。

此範例修改在[建立基本案例](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md)中建立的案例。

## 先決條件

在執行此程式之前，您必須先建立[建立基本案例](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md)中所述的案例。

## 新增及設定觸發程式模組

### 新增觸發程式模組

1. 在案例編輯器中開啟案例。
1. 在第一個（搜尋）模組上按一下滑鼠右鍵，然後選取&#x200B;**刪除模組**。

   模組已刪除，並保留空白預留位置。

1. 按一下空白模組，然後從應用程式清單中選取&#x200B;**Adobe Workfront**。
1. 選取&#x200B;**觀看記錄**。
1. 確認模組使用與案例中其他模組相同的連線。
1. 在篩選欄位中，選取&#x200B;**僅新增記錄**。
1. 在[輸出]方塊中，選取`ID`、`Name`和`Project ID`。
1. 按一下&#x200B;**確定**&#x200B;以儲存模組設定。

   「選擇開始位置」視窗會出現。

1. 從&#x200B;**開始選取**。

### 排程觸發程式模組

1. 按一下「監看紀錄」模組的時鐘。

   「排程」設定視窗會開啟。

1. 在[執行]案例欄位中，選取&#x200B;**定期間隔**。

1. 按一下&#x200B;**確定**。

### 更新第二個模組

因為第一個模組已取代，第二個模組必須對應至新的第一個模組。

1. 開啟轉換物件模組。
1. 在「問題ID」欄位中，刪除黑色ID區塊。 區塊為黑色，因為其對應來源模組已無法使用。
1. 在第一個模組（觀看記錄）下方選取ID區塊，將其對應至第二個模組。
1. 按一下&#x200B;**確定**。

### 測試並啟動

1. 前往Fusion所連線的Workfront環境並新增問題。
1. 按一下案例編輯器左下角的&#x200B;**[!UICONTROL 執行一次]**。
1. 檢查輸出，確保案例如預期般執行。
1. 當您滿意情境如預期般運作時，請按一下畫面左下角的&#x200B;**排程**&#x200B;切換開關至&#x200B;**開啟**。

   這會啟用情境。
1. 在[!DNL Workfront Fusion]中，按一下左下角附近的&#x200B;**[!UICONTROL 儲存]**，以儲存您的情境進度。

   >[!IMPORTANT]
   >
   >隨時儲存並測試情境。

## 資源

* 如需Webhook的詳細資訊，請參閱 [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/webhooks/instant-triggers-webhooks.md)中的[即時觸發器(Webhook)。
