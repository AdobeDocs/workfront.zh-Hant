---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Workfront Proof SPF記錄
description: Workfront Proof會從Workfront Proof的電子郵件地址（例如notification@proofing.yourdomain.com）傳送電子郵件通知給檢閱者。 為了確保收件者的郵件伺服器信任所有Workfront Proof電子郵件通知，您必須為連線至 [!DNL Workfront Proof] 帳戶的自訂網域設定 [!DNL Sender Policy] 架構(SPF)記錄（例如，proofing.yourdomain.com）。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 5295d451-2ad2-4835-9200-f10d4e6286a2
TQID: https://experienceleague.adobe.com/LTZzs99Zzsn5dbOlu4wP1coyJAMDnnCZZ1pTTbEjT24
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 181
ht-degree: 0%

---

# Workfront Proof SPF記錄

>[!IMPORTANT]
>
>本文提及獨立產品[!DNL Workfront Proof]中的功能。 有關[!DNL Adobe Workfront]內部校訂的資訊，請參閱[校訂](../../../review-and-approve-work/proofing/proofing.md)。

[!DNL Workfront Proof]會從[!DNL Workfront Proof]電子郵件地址（例如notification@proofing.yourdomain.com）傳送電子郵件通知給您的稽核者。 為了確保收件者的郵件伺服器信任所有[!DNL Workfront Proof]電子郵件通知，您必須為連線至[!DNL Workfront Proof]帳戶的自訂網域設定[!UICONTROL 寄件者原則架構] (SPF)記錄（例如，**proofing.yourdomain.com**）。

若要設定SPF記錄，您必須包含用於我們主要網域的SPF記錄。

1. 使用下列值為您的網域新增&#x200B;**[!UICONTROL DNS TXT]**&#x200B;專案：

   `v=spf1 a:mx.proofhq.com -all`

   您的電子郵件管理員或IT人員可以協助您進行此設定。

   >[!TIP]
   >
   >您可以在[[!DNL https://mxtoolbox.com/spf.aspx]](https://mxtoolbox.com/spf.aspx)使用免費工具檢閱[!DNL Workfront]個SPF記錄。
