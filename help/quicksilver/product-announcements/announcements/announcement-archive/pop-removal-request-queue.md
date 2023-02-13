---
content-type: reference
navigation-topic: announcements
title: 新Adobe Workfront管理系統以21.1取代請求佇列的POP電子郵件
description: 我們正在將請求隊列的POP電子郵件選項替換為新的Adobe Workfront管理系統。 您仍可以透過電子郵件提交請求，但您需要在「請求佇列」區域中設定新的Workfront管理電子郵件地址。
author: Luke
feature: Product Announcements
exl-id: d7147641-ba36-422b-a9b2-3c2f4ab609d8
source-git-commit: f05b462ff596ccc19215ca684802a9820a98211a
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---

# 新Adobe Workfront管理系統以21.1取代請求佇列的POP電子郵件

我們正在將請求隊列的POP電子郵件選項替換為新的Adobe Workfront管理系統。 您仍可以透過電子郵件提交請求，但您需要在「請求佇列」區域中設定新的Workfront管理電子郵件地址。

## 為何刪除POP電子郵件選項？

POP技術是一種不可靠、安全性較差的電子郵件選項。 此外，我們還看到許多與POP電子郵件相關的客戶問題。 對Workfront管理的系統進行變更將帶來更可靠的體驗。

## 我需要採取什麼行動？

您需要為已在生產環境中透過POP電子郵件設定的每個請求佇列設定新電子郵件地址，並視需要分發新電子郵件地址。 如需詳細資訊，請參閱 [讓使用者將問題透過電子郵件傳送至「請求佇列」專案](/help/quicksilver/manage-work/requests/create-requests/enable-email-issues-into-projects.md).

## 什麼是轉換計畫？

從2月初的21.1版開始，您有60天的時間可將使用者轉變為新 *@intake.workfront.com* 您建立的電子郵件地址。 在60天期間，以前使用的POP電子郵件將繼續工作。

## 如何在預覽中測試？

若要在預覽中測試此變更，您必須在預覽環境中啟用電子郵件。 若要這麼做，請依照 [啟用從預覽沙箱環境傳送電子郵件](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!IMPORTANT]
>
>您在此設定的內容不會傳遞至您的生產環境。 在功能發行至生產環境後，您需要再次執行此程式。
