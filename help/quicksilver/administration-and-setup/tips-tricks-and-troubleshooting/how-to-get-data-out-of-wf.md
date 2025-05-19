---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 從Adobe Workfront匯出歷史資料：優缺點
description: 本文說明可用來從Workfront匯出歷史資料的4個選項的優缺點。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: ed40984f-602a-46e9-a72b-141936de8fcb
source-git-commit: 7f0aac7c8519b1e570e29fedf1492918e8120ad2
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 0%

---

# 從[!DNL Adobe Workfront]匯出歷史資料：優點與缺點

<!-- Audited: 5/2025 -->

本文說明可用來從Adobe Workfront匯出歷史資料的4個選項的優缺點。

## 使用我們的其中一個合作夥伴

[!DNL AtAppStore] ([www.atappstore.com](https://www.atappstore.com))有一個簡單易用的應用程式(其[Workfront快照](https://store.atappstore.com/product/workfront-snapshot/)解決方案)，可讓您自行下載資料。 選用的檢視器(其[Workfront Snapshot Viewer](https://store.atappstore.com/product/workfront-snapshot-viewer/)解決方案)可讓您輕鬆離線檢視資料。

* **優點：**&#x200B;所有核心[!DNL Workfront]物件均已匯出，包括自訂欄位和備註，並儲存在容易存取的[!DNL MS Access]資料庫中。 檢視器的介面易於使用和讀取。 「擷取檔案」也可單獨作為服務使用，輸出會整理到邏輯資料夾結構中，以對應到每個檔案及其先前版本。

* **缺點：**&#x200B;技術限製為2GB的資料，但AtAppStore允許您只購買您需要的資料。

* **費用：**&#x200B;如需詳細資訊，請移至[https://store.atappstore.com/product/workfront-snapshot/](https://store.atappstore.com/product/workfront-snapshot/)。

## 向我們的資料庫團隊要求[!DNL Postgres]資料傾印檔案

您必須向我們的客戶支援團隊提交請求，然後客戶支援團隊會向我們的資料庫團隊提交請求，以匯出包含您資料的資料庫傾印檔案（.dmp [!DNL Postgres]檔案）。 我們將會向我們的NOC團隊提出其他要求，以擷取您所有儲存的檔案。

* **優點**：您可獲得整個資料載入，包括自訂欄位，以及儲存在系統中的檔案。

* **缺點**：無法讀取此檔案，除非您將其上傳至[!DNL Postgres]資料庫並重新建立資料表之間的關係。 檔案儲存在單獨的檔案伺服器上，必須由NOC小組使用單獨的程式來分別擷取。 這樣做時，檔案沒有組織，且全部由其GUID參考。

* **成本**：此下載會產生成本，視團隊建立檔案所需的時間而定。 請洽詢您的AE/CAE以取得詳細資訊，或開始此程式。

## 透過[!UICONTROL Kick-Starts]匯出

無論您是否擁有遠端諮詢時間，您都可以使用我們的其中一位顧問，以報表或[!UICONTROL kick-starts]的形式匯出您的資料，或者您可以自行執行這些報表：

* **優點**：報告容易閱讀，而且可以在各種應用程式中匯入。 這些區段可自訂為包含您想要的任何群組和檢視。

* **問題**：檔案必須單獨下載。

* **費用**：如果您可以自行執行報告（只需要系統管理員登入），或可以使用剩餘的遠端諮詢時間，則完全免費。 如果您有興趣為此購買遠端諮詢，請洽詢您的AE/CAE。

  如需使用Kick-Starts匯出資料的詳細資訊，請參閱[透過[!UICONTROL Kick-Starts]](../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md)從 [!DNL Adobe Workfront] 匯出資料。

## 使用我們的開放API

如果貴組織中擁有正確的資源，這些資源可以建立自訂API，從Workfront擷取您的所有資料：

* **優點**：您控制著從系統匯出的專案。

* **缺點**：時間花在您身邊，您必須尋找資源來編寫API的程式碼並執行匯出。

* **成本**：這是您組織的內部專案。
