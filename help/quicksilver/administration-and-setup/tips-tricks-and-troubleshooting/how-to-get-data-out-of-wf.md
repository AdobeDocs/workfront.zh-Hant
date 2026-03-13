---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 從Adobe Workfront導出歷史資料：利弊
description: 本文說明了可用於導出Workfront歷史資料的4個選項的利弊。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: ed40984f-602a-46e9-a72b-141936de8fcb
source-git-commit: bbd00374a6b291582cd03b9d0471d8547eb6ab7f
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# 從[!DNL Adobe Workfront]導出歷史資料：利弊

<!-- Audited: 5/2025 -->

本文說明了可用於導出Adobe Workfront歷史資料的4個選項的利弊。

## 使用我們的合作夥伴之一

[!DNL AtAppStore]&#x200B;([www.atappstore.com](https://www.atappstore.com))有一個易於使用的應用(其[Workfront快照](https://store.atappstore.com/product/workfront-snapshot/)解決方案)，允許您自己下載資料。 可選查看器(其[Workfront快照查看器](https://store.atappstore.com/product/workfront-snapshot-viewer/)解決方案)允許您輕鬆離線查看資料。

* **Pros:**&#x200B;所有核心[!DNL Workfront]對象都已導出，包括自定義欄位和注釋，並儲存在易於訪問的[!DNL MS Access]資料庫中。 查看器的介面易於使用和閱讀。 「提取文檔」也可單獨作為服務使用，其輸出將組織為邏輯資料夾結構，該結構映射到每個文檔及其早期版本。

* **缺點：**&#x200B;有2GB資料的技術限制，但AtAppStore允許您僅購買所需的資料。

* **成本：**&#x200B;有關詳細資訊，請訪問[https://store.atappstore.com/product/workfront-snapshot/](https://store.atappstore.com/product/workfront-snapshot/)。



## 通過[!UICONTROL 啟動]導出

無論您是否有遠程咨詢小時數，您都可以使用我們的顧問之一以報告或[!UICONTROL 啟動]的形式導出資料，或者您可以自己運行這些報告：

* **Pros**：報告易於讀取，可以在多種應用程式中導入。 可以定制它們，以包括您想要的任何分組和視圖。

* **Cons**：文檔必須單獨下載。

* **成本**：如果您可以自行運行報告（您只需要系統管理員登錄），或者您可以使用剩餘的遠程咨詢時間，則免費。 如果您對購買遠程咨詢感興趣，請與您的AE/CAE聯繫。

  有關使用Kick-Starts導出資料的詳細資訊，請參閱[通過 [!DNL Adobe Workfront] Kick-Starts[!UICONTROL 從]](../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md)導出資料。

## 使用我們的開放API

如果您在組織中擁有適當的資源，則他們可以構建自定義API以從Workfront檢索您的所有資料：

* **Pros**：您控制從系統導出的內容。

* **Cons**：時間花在您身邊，您將必須查找資源來編碼API並執行導出。

* **成本**：它是您的組織的內部。
