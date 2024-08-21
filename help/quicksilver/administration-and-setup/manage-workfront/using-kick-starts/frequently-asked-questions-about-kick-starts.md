---
user-type: administrator
content-type: faq
product-area: system-administration
keywords: kickstart，kick-start，kickstart，kick-start
navigation-topic: use-kick-starts
title: 關於Kick-Start的常見問題
description: 尋找有關使用Kick-Starts匯入和匯出Workfront資料的常見問題解答。
author: LIsa
feature: System Setup and Administration
role: Admin
exl-id: f286e03e-93a8-43f5-8c2d-2c36203776a8
source-git-commit: 01487bb9cb195d6fa89bbe0fbdb7678254642714
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# 關於Kick-Start的常見問題

以下是有關Kick-Start的常見問題：

## 為什麼我在嘗試匯入Kick-Start檔案時會收到此錯誤：「您的檔案正確，但未匯入任何內容？」

### 解答

Kick-Start檔案可能遺漏下列三個專案之一：

1. 對於您要匯入的所有專案，**isNew**&#x200B;資料行必須設為&#x200B;**TRUE**。 **isNew**&#x200B;必須是&#x200B;**TRUE**，因為您只能以Kick-Start匯入新資料。 您無法透過Kick-Start修改現有資料。 在試算表中可以有其他列，其中包含&#x200B;**isNew = FALSE**，但是這些列將不會匯入。

1. 檔&#x200B;案在資料標題開始之前必須有一個空白列。
1. Excel&#x200B;工作表必須具有正確的名稱。

使用Kick-Start時，我們建議先下載Kick-Start範本、手動填入正確資料，然後將其匯入Adobe Workfront。

如需使用Kick-Start在Workfront中正確匯入資料的詳細資訊，請參閱[使用Kick-Start範本將資料匯入Adobe Workfront](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md)。

## 為什麼我在嘗試使用Kick-Start檔案將時數匯入Workfront時收到此錯誤：「找不到具有主鍵值「null」的使用者？」

### 解答

錯誤是指與時數相關聯之使用者的GUID。

若要解決此問題：

1. 僅匯出&#x200B;**小時**&#x200B;物件的空白快速啟動範本。\
   如需有關匯出空白Kick-Start檔案的詳細資訊，請參閱[使用Kick-Start範本將資料匯入Adobe Workfront](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md)中的「匯出Kick-Start範本」。

1. 手動複製原始Kick-Start中的資料，並將其貼到空白檔案中。\
   對每個欄執行此動作。
1. 請再次嘗試匯入新檔案。\
   Kick-Start應該可以成功匯入。

## 為何Kick-Start匯入中的使用者設定檔中沒有填入country欄位？

### 問題

匯入欄位為&#x200B;**setCountry**&#x200B;的使用者Kick-Start時，該資料不會進入使用者設定檔上的國家/地區。

### 解答

如果使用者已啟用統一使用者管理(UUM)或AdobeIdentity Management系統(IMS)，**國家**&#x200B;欄位僅接受國家/地區代碼值（例如，US、GB、IN）。 在匯入之前，請先確認Kick-Start範本中的&#x200B;**setCountry**&#x200B;欄位正在使用國家/地區代碼值。

如需使用Kick-Start在Workfront中正確匯入資料的詳細資訊，請參閱[使用Kick-Start範本將資料匯入Adobe Workfront](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md)。
