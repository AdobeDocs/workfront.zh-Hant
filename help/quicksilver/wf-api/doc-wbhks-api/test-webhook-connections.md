---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: 測試Webhook連接
description: 測試Webhook連接
author: John
feature: Workfront API
exl-id: 7452ebfc-7c72-4fea-99ac-7f76b12404b8
source-git-commit: a62ae524f922326811423cd17d0656920b7cc9d3
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 0%

---


# 測試Webhook連接

若要驗證您的檔案WebHook實作是否正常運作，請執行本區段中的手動測試。 這些步驟會透過Adobe Workfront Web介面，間接點擊您Webhook實作的端點。

## 必要條件

執行測試需要下列必要條件：

* 已啟用進階檔案管理(ADM)的Workfront帳戶

* 具有系統管理員權限之此帳戶的Workfront使用者

* 具有可供Workfront存取之HTTP端點的Document Webhook例項

這些測試還假定已註冊Document Webhook實例。 (您可以在Workfront中的「設定>檔案>自訂整合」中註冊執行個體。)

**測試1:為用戶提供文檔Webhook服務**

測試OAuth型Webhook提供者的驗證URL和Token端點URL。

1. 在Workfront中，按一下頂部導航欄中的「文檔」連結，轉到主「文檔」頁。
1. 按一下「添加文檔」下拉清單，並在「添加服務」下選擇「文檔Webhook」服務。
1. （僅限OAuth服務）完成上一個步驟後，您會在快顯視窗中看到服務的OAuth2驗證頁面載入。 (注意：系統可能會提示您先登錄服務。) 從驗證頁面，按一下信任或允許按鈕，授予Workfront對使用者帳戶的存取權。
1. 確認服務已新增至「新增檔案」下拉式清單。 如果您一開始沒有看到，請嘗試重新整理瀏覽器。

**測試2:將檔案連結至Workfront測試下列端點：/files, /metadata**

1. 在Workfront中，按一下頂部導航欄中的「文檔」連結，轉到主「文檔」頁。
1. 在「添加文檔」下選擇「文檔Webhook」服務。
1. 在強制回應視窗中，導覽資料夾結構。
1. 確認您能夠導覽資料夾結構。
1. 選取檔案並將其連結至Workfront

**測試3:導覽至內容管理系統中的檔案**

測試下列端點：/metadata（尤其是viewLink）

1. 將檔案連結至Workfront
1. 選擇文檔，然後按一下「開啟」(Open)連結。
1. 驗證文檔是否在新頁簽中開啟。

**測試4:導覽至內容管理系統中的檔案（含登入）**

測試下列端點：/metadata（尤其是viewLink）

1. 確保您已登出內容管理系統。
1. 將檔案連結至Workfront。
1. 選擇文檔，然後按一下「開啟」(Open)連結。
1. 驗證內容管理系統的登錄螢幕是否在新頁簽中載入。
1. 登入並確認您已被帶入檔案

**測試5:從內容管理系統下載文檔**

測試下列端點（尤其是下載連結）:/metadata 

1. 將檔案連結至Workfront。
1. 選擇文檔，然後按一下「下載」連結。
1. 確認下載開始。

**測試6:搜尋內容**

測試下列端點：/search

1. 在Workfront中，按一下頂部導航欄中的「文檔」連結，轉到主「文檔」頁。
1. 在「添加文檔」下選擇「文檔Webhook」服務。
1. 在強制回應視窗中執行搜尋。
1. 驗證搜索結果是否正確。

**測試7:將檔案從Workfront傳送至內容管理系統**

測試下列端點：/files, /uploadInit, /upload

1. 在Workfront中，按一下頂部導航欄中的「文檔」連結，轉到主「文檔」頁。
1. 從電腦上傳檔案至Workfront
1. 轉到文檔詳細資訊頁
1. 在「文檔操作」下拉清單中，在「發送到……」下選擇「文檔Webhook服務」
1. 前往所需的目的地資料夾，然後按一下「儲存」按鈕。
1. 驗證文檔已上載到內容管理系統中的正確位置。

**測試8:在Workfront中檢視縮圖**

測試下列端點：/thumbnail

1. 將檔案連結至Workfront。
1. 在清單中選擇文檔。
1. 確認縮圖出現在右側面板中。

**測試9:取得內容位元組**

測試下列端點：/download

1. 將檔案連結至Workfront。
1. 轉到文檔詳細資訊頁。
1. 選擇「文檔操作」>「發送到……」>「Workfront」，將文檔發送到Workfront。 這會在Workfront中建立新的檔案版本。
1. 按一下「下載」連結，從Workfront下載檔案。

**測試10:重新整理存取權杖（僅限OAuth2網頁連結提供者）**

測試下列端點：代號端點URL

1. 為用戶提供文檔Webhook服務
1. 讓使用者的存取權杖失效，方法是1)等待它逾時，或2)在外部系統中手動使它失效。
1. 在Workfront中重新整理存取權杖。 例如，您可以將檔案連結至Workfront，即可完成此操作。 如果您能夠導覽至並連結檔案，則會知道存取權杖已成功重新整理。

>[!NOTE]
>
>目前，「發送到……」不適用於連結的文檔。 這將由Workfront新增。 您可以使用REST用戶端(例如Postman)手動點擊端點，以測試/download端點。 或者，可通過生成數字校樣來測試/download端點。 若要啟用數位校對功能，請聯絡Workfront。
