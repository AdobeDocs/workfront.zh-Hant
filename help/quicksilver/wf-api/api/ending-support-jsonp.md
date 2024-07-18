---
content-type: api
navigation-topic: api-navigation-topic
title: 終止支援JSONP
description: 終止支援JSONP
author: Becky
feature: Workfront API
role: Developer
exl-id: 681336c2-2f41-4746-8cba-be077f556742
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 0%

---

# 終止支援JSONP

由於JSONP (Javascript with Padding)是舊標準，具有已知的安全漏洞，因此Adobe Workfront自2018年11月起將不再支援JSONP。 此決定支援我們更新Workfront平台的大型計畫。

JSONP是可執行跨原始或跨網站要求的標準。 許多Workfront客戶和合作夥伴都會使用JSONP，從自己網域的系統存取Workfront，作為整合的一部分。 JSONP可讓Workfront應用程式處理來自非Workfront網域的請求。

如果您使用JSONP作為任何Workfront整合的一部分，您必須更新整合以使用CORS （跨原始資源共用）標準。 此更新需要您執行以下操作：

1. 向Workfront支援團隊提交請求，要求將任何用於向允許清單提出跨來源請求的網域加入。

   若要將您的網域新增至CORS允許清單，請連絡Workfront客戶支援，電話：844-306-HELP(4357)或線上提交支援票證。

   >[!NOTE]
   >
   >只有在2018年8月1日之前使用JSONP的客戶才支援將網域新增至CORS的允許清單。


1. 變更您的整合程式碼以使用CORS。
