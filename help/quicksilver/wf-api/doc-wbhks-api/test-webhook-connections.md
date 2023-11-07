---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 測試Webhook連線
description: 測試Webhook連線
author: Becky
feature: Workfront API
role: Developer
exl-id: 7452ebfc-7c72-4fea-99ac-7f76b12404b8
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 0%

---


# 測試Webhook連線

若要確認您的檔案webhook實作可正常運作，請執行本節中的手動測試。 這些步驟會透過Adobe Workfront網頁介面直接點選webhook實施的端點。

## 必要條件

執行測試需要下列先決條件：

* 已啟用進階檔案管理(ADM)的Workfront帳戶

* 此帳戶的Workfront使用者，擁有系統管理員許可權

* 具有Workfront可存取之HTTP端點的檔案Webhook例項

這些測試也假設您的Document Webhook例項已註冊。 (您可以在Workfront中的「設定>檔案>自訂整合」下註冊執行個體)。

**測試1：為使用者布建Document Webhook服務**

測試以OAuth為基礎的Webhook提供者的驗證URL和權杖端點URL。

1. 在Workfront中，按一下頂端導覽列中的「檔案」連結，前往「檔案」首頁面。
1. 按一下「新增檔案」下拉式清單，並在「新增服務」下選取您的Document Webhook服務。
1. （僅限OAuth服務）完成上一步驟後，您會在快顯視窗中看到服務的OAuth2驗證頁面載入。 （注意：系統可能會提示您先登入服務。） 在驗證頁面中，按一下「信任」或「允許」按鈕，授予Workfront使用者帳戶的存取權。
1. 確認您的服務已新增至新增檔案下拉式清單。 如果一開始沒有看見，請嘗試重新整理瀏覽器。

**測試2：將檔案連結至Workfront測試下列端點： /files、/metadata**

1. 在Workfront中，按一下頂端導覽列中的「檔案」連結，前往「檔案」首頁面。
1. 在新增檔案下選擇您的檔案Webhook服務。
1. 從強制回應視窗中，導覽至資料夾結構。
1. 確認您能夠導覽資料夾結構。
1. 選擇檔案並將其連結至Workfront

**測試3：導覽至內容管理系統中的檔案**

測試下列端點： /metadata （尤其是viewLink）

1. 將檔案連結至Workfront
1. 選取檔案並按一下「開啟」連結。
1. 確認檔案會在新標籤中開啟。

**測試4：導覽至內容管理系統中的檔案（含登入）**

測試下列端點： /metadata （尤其是viewLink）

1. 確保您已登出內容管理系統。
1. 將檔案連結至Workfront。
1. 選取檔案並按一下「開啟」連結。
1. 確認內容管理系統的登入畫面會在新標籤中載入。
1. 登入並確認您已前往檔案

**測試5：從內容管理系統下載檔案**

測試以下端點（特別是下載連結）： /metadata 

1. 將檔案連結至Workfront。
1. 選取檔案並按一下下載連結。
1. 確認下載開始。

**測試6：搜尋內容**

測試下列端點： /search

1. 在Workfront中，按一下頂端導覽列中的「檔案」連結，前往「檔案」首頁面。
1. 在新增檔案下選擇您的檔案Webhook服務。
1. 從強制回應視窗中，執行搜尋。
1. 確認搜尋結果是否正確。

**測試7：將檔案從Workfront傳送至內容管理系統**

測試下列端點： /files、/uploadInit、/upload

1. 在Workfront中，按一下頂端導覽列中的「檔案」連結，前往「檔案」首頁面。
1. 從您的電腦上傳檔案至Workfront
1. 前往檔案詳細資訊頁面
1. 從「檔案動作」下拉式清單中，選取「傳送至……」下的「檔案Webhook服務」。
1. 前往所需的目的地資料夾，然後按一下「儲存」按鈕。
1. 確認檔案已上傳至內容管理系統中的正確位置。

**測試8：在Workfront中檢視縮圖**

測試下列端點： /thumbnail

1. 將檔案連結至Workfront。
1. 在清單中選取檔案。
1. 確認縮圖出現在右側面板中。

**測試9：取得內容位元組**

測試下列端點： /download

1. 將檔案連結至Workfront。
1. 前往檔案詳細資訊頁面。
1. 透過選取檔案動作>傳送至…… > Workfront，將檔案傳送至Workfront。 這會在Workfront中建立新的檔案版本。
1. 按一下「下載」連結，從Workfront下載檔案。

**測試10：重新整理存取權杖（僅限OAuth2 Webhook提供者）**

測試下列端點：權杖端點URL

1. 為使用者布建Document Webhook服務
1. 讓使用者的存取Token失效，方法是1 )等待它逾時，或2)在外部系統中手動讓它失效。
1. 在Workfront中重新整理存取Token。 例如，您可以將檔案連結至Workfront來執行此操作。 如果您能夠導覽至並連結檔案，您將知道存取權杖已成功重新整理。

>[!NOTE]
>
>目前，傳送至……不適用於連結的檔案。 Workfront將新增此專案。 您可以使用REST使用者端(例如Postman)手動點選端點來測試/download端點。 或者，也可以透過產生數位校樣來測試/download端點。 若要啟用，數位校訂，請聯絡Workfront。
