---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Workfront校樣SPF記錄
description: Workfront Proof會以Workfront Proof電子郵件地址(例如notification@proofing.yourdomain.com)傳送電子郵件通知給審核者。 為確保收件者的郵件伺服器信任所有Workfront Proof電子郵件通知，您需要設定 [!DNL Sender Policy] 連接到的自定義域的框架(SPF)記錄 [!DNL Workfront Proof] 帳戶（例如pooking.yourdomain.com）。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 5295d451-2ad2-4835-9200-f10d4e6286a2
source-git-commit: c989687e9adaf12a31a920921bf8fb69425ca1c5
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---

# Workfront校樣SPF記錄

>[!IMPORTANT]
>
>本文說明獨立產品中的功能 [!DNL Workfront Proof]. 有關內部校對的資訊 [!DNL Adobe Workfront]，請參閱 [校對](../../../review-and-approve-work/proofing/proofing.md).

[!DNL Workfront Proof] 會透過 [!DNL Workfront Proof] 電子郵件地址，例如notification@proofing.yourdomain.com。 為了確保收件者的郵件伺服器信任所有 [!DNL Workfront Proof] 電子郵件通知，您需要 [!UICONTROL 發件人策略框架] (SPF)記錄，用於連接到 [!DNL Workfront Proof] 帳戶(例如 **pooking.yourdomain.com**)。

要設定SPF記錄，您需要包含用於主域的SPF記錄。

1. 新增 **[!UICONTROL DNS TXT]** 填入以下值：

   `v=spf1 a:mx.proofhq.com -all`

   您的電子郵件管理員或IT人員可協助您進行此設定。

   >[!TIP]
   >
   >您可以在 [[!DNL https://mxtoolbox.com/spf.aspx]](https://mxtoolbox.com/spf.aspx) 查看 [!DNL Workfront] SPF記錄。
