---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '''從Adobe Workfront匯出歷史資料：優點與缺點'
description: 本文說明從Workfront匯出歷史資料時，可使用的4個選項的優點和缺點。
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: ed40984f-602a-46e9-a72b-141936de8fcb
source-git-commit: f3af39e760b2b407cda5ab78497cdc775defdcf6
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# 匯出歷史資料 [!DNL Adobe Workfron]t:優點與缺點

本文說明4個選項的優點和缺點，這些選項可用來從 [!DNL Workfront].

## 使用我們的合作夥伴

[!DNL AtAppStore], [!DNL Workfront] 認證合作夥伴，有一款易於使用的應用程式，允許您下載資料。 此應用程式也包含檢視器，可讓您輕鬆檢視資料。

* **優點：** 所有 [!DNL Workfront] 會匯出物件，包括自訂欄位。 檢視器的介面易於使用和閱讀，且可在 [!DNL MS Access] 資料庫。

* **缺點：** 未導出文檔。 您必須另行下載。 如需詳細資訊，請前往 [http://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx。](http://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx)

## 要求 [!DNL Postgres] 資料轉儲檔案

您的客戶經理可以向我們的資料庫團隊提交導出資料庫轉儲檔案(.dmp [!DNL Postgres] 檔案)。 另外一個請求將發送給我們的AOS團隊，以檢索所有儲存的文檔。

* **優點**:您會獲得整個資料載入，包括自訂欄位，以及儲存在系統中的檔案。

* **缺點**:資料庫檔案很難讀：除非將此檔案上傳至 [!DNL Postgres] 資料庫，並重新建立表之間的關係。 文檔儲存在單獨的檔案伺服器上，並且必須由AOS團隊使用單獨的進程單獨提取。 這樣做時，檔案沒有任何組織，而且GUID都會參照這些檔案。
* **成本**:此下載會產生相關成本，具體取決於團隊建立檔案所花的時間。 請向您的AE/CAE了解詳細資訊或開始此程式。

## 透過 [!UICONTROL 開始]

無論您是否擁有遠程咨詢小時數，都可以使用我們的顧問之一以報告或 [!UICONTROL 開始]，或者您可以自行執行這些報表：

* **優點**:這些報告易於讀取，可以在多種應用程式中導入；您可以自訂這些群組，以包含您想要的任何群組和檢視。

* **缺點**:檔案必須另外下載。

* **成本**:如果您可以自行執行報表（您只需要系統管理員登入），或您可以使用剩餘的遠端諮詢時間，則此功能即可免費使用。 如果您有興趣為此購買遠程咨詢，請與您的AE/CAE聯繫。

   如需使用Kick-Starts匯出資料的詳細資訊，請參閱 [從匯出資料 [!DNL Adobe Workfront] via [!UICONTROL 開始]](../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

## 使用我們的開放API

如果貴組織中有正確的資源，他們可以建置自訂API，從Workfront擷取您的所有資料：

* **優點**:您可以控制從系統匯出的內容。

* **缺點**:此時間會花在您身邊，您必須尋找資源來編寫API程式碼並執行匯出。

* **成本**:組織內部。
