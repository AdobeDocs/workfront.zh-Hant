---
user-type: administrator
content-type: faq
product-area: system-administration
keywords: kickstart,kickstart,kickstarts,kickstarts
navigation-topic: use-kick-starts
title: 關於Kick-Starts的常見問題
description: 尋找有關使用Kick-Starts匯入和匯出Workfront資料的常見問題解答。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f286e03e-93a8-43f5-8c2d-2c36203776a8
source-git-commit: 1ebdb3797e30a7e06f4dfd4a7e0e5f540351c126
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---

# 關於Kick-Starts的常見問題

以下是關於Kick-Starts的常見問題：

## 嘗試匯入Kick-Start檔案時，為何收到此錯誤：「您的檔案正確，但未匯入任何內容？」

### 回答

Kick-Start檔案中可能遺漏下列三項之一：

1. 此 **isNew** 欄必須設為 **TRUE** 為所有要匯入的項目。 **isNew** 必須 **TRUE** 因為您只能以「啟動」匯入新資料。 您無法透過Kick-Start修改現有資料。 試算表中可有其他列，其包含 **isNew = FALSE** 但這些列不會匯入。

1. &#x200B;在資料的標題之前，檔案必須有一個空白列。
1. &#x200B; Excel工作表的名稱必須正確。

使用「啟動」時，我們建議先下載「啟動範本」、手動填入正確的資料，然後將其匯回Adobe Workfront。

如需使用Kick-Starts在Workfront中正確匯入資料的詳細資訊，請參閱 [使用Kick-Start範本將資料匯入Adobe Workfront](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

## 嘗試使用Kick-Start檔案將小時匯入Workfront時，為何收到此錯誤：&quot;未找到主鍵值為&quot;null&quot;的用戶？&quot;

### 回答

錯誤是指與小時關聯的用戶的GUID。

若要解決此問題：

1. 匯出空白的「啟動」範本 **小時** 僅對象。\
   如需匯出空白「啟動」檔案的詳細資訊，請參閱  [使用Kick-Start範本將資料匯入Adobe Workfront](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

1. 手動複製原始Kick-Start中的資料，並貼到空白檔案中。\
   對每欄執行此操作。
1. 請再次嘗試導入新檔案。\
   Kick-Start應成功導入。

## 為什麼Cick-Start匯入中的國家欄位沒有填入使用者設定檔？

### 問題

使用欄位匯入使用者啟動時 **setCountry**，該資料不會傳至使用者設定檔上的國家/地區。

### 回答

如果使用者已啟用統一使用者管理(UUM)或AdobeIdentity Management系統(IMS)，則 **國家/地區** 欄位僅接受國家/地區代碼值（例如US、GB、IN）。 確認 **setCountry** 「啟動」範本中的欄位在匯入前使用國家/地區代碼值。

如需使用Kick-Starts在Workfront中正確匯入資料的詳細資訊，請參閱 [使用Kick-Start範本將資料匯入Adobe Workfront](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).
