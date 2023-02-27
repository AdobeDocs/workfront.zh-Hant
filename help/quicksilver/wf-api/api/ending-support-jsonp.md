---
content-type: api
navigation-topic: api-navigation-topic
title: 終止支援JSONP
description: 終止支援JSONP
author: Becky
feature: Workfront API
exl-id: 681336c2-2f41-4746-8cba-be077f556742
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 0%

---

# 終止支援JSONP

由於JSONP（含邊框間距的Javascript）是舊標準，具有已知的安全性弱點，自2018年11月起，Adobe Workfront將不再支援JSONP。 這一決定支援我們更大的Workfront平台現代化倡議。

JSONP是執行跨原始或跨網站要求的標準。 許多Workfront客戶和合作夥伴會透過JSONP，在自己的網域從系統存取Workfront，作為整合的一部分。 JSONP可讓Workfront應用程式處理來自非Workfront網域的請求。

如果您在任何Workfront整合中使用JSONP，則必須更新整合以使用CORS（跨原始資源共用）標準。 此更新需要您執行下列操作：

1. 向Workfront支援團隊提交請求，讓任何網域可用來向我們的允許清單提出跨來源請求。

   若要將您的網域新增至CORS允許清單，請聯絡Workfront客戶支援(電話：844-306-HELP(4357))，或線上提交支援票證。

   >[!NOTE]
   >
   >只有在2018年8月1日之前使用JSONP的客戶，才支援將網域新增至CORS的允許清單。


1. 變更您的整合程式碼以使用CORS。
