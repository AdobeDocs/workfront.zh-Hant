---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 「從Adobe Workfront匯出歷史資料：優點與缺點」
description: 本文說明可用來從Workfront匯出歷史資料的4個選項的優缺點。
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: ed40984f-602a-46e9-a72b-141936de8fcb
source-git-commit: 5d7ff744ed0721ffa6d793a224226f28a76c57a0
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 0%

---

# 從[!DNL Adobe Workfron]t匯出歷史資料：優點與缺點

本文說明可用來從[!DNL Workfront]匯出歷史資料的4個選項的優缺點。

## 使用我們的其中一個合作夥伴

[!DNL AtAppStore]是[!DNL Workfront]認證合作夥伴，擁有可讓您下載資料的簡單易用的應用程式。 此應用程式也包含檢視器，可讓您輕鬆檢視資料。

* **優點：**&#x200B;已匯出您的所有[!DNL Workfront]物件，包括自訂欄位。 檢視器的介面易於使用和讀取，並可輕鬆地匯入[!DNL MS Access]資料庫。

* **缺點：**&#x200B;檔案未匯出。 您必須個別下載。 如需詳細資訊，請前往[http://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx。](https://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx)

## 向我們的資料庫團隊要求[!DNL Postgres]資料傾印檔案

您的帳戶主管可以向我們的資料庫團隊提交請求，以匯出包含您資料的資料庫傾印檔案（.dmp [!DNL Postgres]檔案）。 我們的AOS團隊將收到其他請求，要求擷取您所有儲存的檔案。

* **優點**：您可獲得整個資料載入，包括自訂欄位，以及儲存在系統中的檔案。

* **缺點**：資料庫檔案難以讀取：除非您將其上載至[!DNL Postgres]資料庫並重新建立資料表之間的關係，否則無法讀取此檔案。 檔案儲存在單獨的檔案伺服器上，必須由AOS小組使用單獨的程式來分別擷取。 這樣做時，檔案沒有組織，且全部由其GUID參考。
* **成本**：此下載會產生成本，視團隊建立檔案所需的時間而定。 請洽詢您的AE/CAE以取得詳細資訊，或開始此程式。

## 透過[!UICONTROL Kick-Starts]匯出

無論您是否擁有遠端諮詢時間，您都可以使用我們的其中一位顧問，以報表或[!UICONTROL kick-starts]的形式匯出您的資料，或者您可以自行執行這些報表：

* **優點**：報告容易閱讀，而且可以在各種應用程式中匯入；您可以自訂報告，以包含您想要的任何群組和檢視。

* **問題**：檔案必須單獨下載。

* **費用**：如果您可以自行執行報告（只需要系統管理員登入即可），或可以使用剩餘的遠端諮詢時間，則完全免費。 如果您有興趣為此購買遠端諮詢，請洽詢您的AE/CAE。

  如需使用Kick-Starts匯出資料的詳細資訊，請參閱[透過[!UICONTROL Kick-Starts]](../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md)從 [!DNL Adobe Workfront] 匯出資料。

## 使用我們的開放API

如果貴組織中擁有正確的資源，這些資源可以建立自訂API，從Workfront擷取您的所有資料：

* **優點**：您控制著從系統匯出的專案。

* **缺點**：時間花在您身邊，您必須尋找資源來編寫API的程式碼並執行匯出。

* **費用**：貴組織的內部費用。
