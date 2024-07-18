---
content-type: reference
navigation-topic: announcements
title: 全新Adobe Workfront管理系統，以21.1取代請求佇列的POP電子郵件
description: 我們正在將請求佇列的POP電子郵件選項取代為新的Adobe Workfront管理系統。 您仍可以透過電子郵件提交請求，但您需要在「請求佇列」區域中設定新的Workfront受管電子郵件地址。
author: Luke
feature: Product Announcements
exl-id: d7147641-ba36-422b-a9b2-3c2f4ab609d8
source-git-commit: f05b462ff596ccc19215ca684802a9820a98211a
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# 全新Adobe Workfront管理系統，以21.1取代請求佇列的POP電子郵件

我們正在將請求佇列的POP電子郵件選項取代為新的Adobe Workfront管理系統。 您仍可以透過電子郵件提交請求，但您需要在「請求佇列」區域中設定新的Workfront受管電子郵件地址。

## 為何要移除POP電子郵件選項？

POP技術是不可靠、較不安全的電子郵件選項。 此外，我們發現許多客戶對於POP電子郵件有特別的問題。 變更Workfront受管系統可提供更可靠的體驗。

## 我需要採取什麼動作？

您必須針對在生產環境中使用POP電子郵件設定的每個請求佇列，設定新的電子郵件地址，並視需要散發新的電子郵件地址。 如需詳細資訊，請參閱[讓使用者透過電子郵件將問題傳送到請求佇列專案](/help/quicksilver/manage-work/requests/create-requests/enable-email-issues-into-projects.md)。

## 什麼是轉換計畫？

從2月初的21.1版開始，您有60天的時間將使用者轉換為您建立的新&#x200B;*@intake.workfront.com*&#x200B;電子郵件地址。 在60天期間，先前使用的POP電子郵件將繼續運作。

## 如何在「預覽」中測試此專案？

若要在預覽中測試此變更，您必須在預覽環境中啟用電子郵件。 若要這麼做，請依照[啟用從預覽沙箱環境傳送電子郵件](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md)中在預覽中管理電子郵件一節中的指示進行。

>[!IMPORTANT]
>
>您在此設定的內容將不會移轉至您的生產環境。 功能發佈到生產環境後，您需要再次執行此程式。
