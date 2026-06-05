---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: DOCU物件不支援連結資料夾
description: DOCU物件不支援連結資料夾
author: Becky
feature: Workfront API
role: Developer
exl-id: 33b5a998-f3e1-42a2-852e-fb862d770d50
TQID: https://experienceleague.adobe.com/iPjiffn9QLDldjWRdxMyf8RTaZaB9X6axc7UVY1B3Bg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 118
ht-degree: 0%

---

# 不支援使用API新增連結的資料夾

不支援使用API將連結資料夾新增至檔案(DOCU)物件的資料夾陣列。 請求將成功，但檔案可能會由某些外部提供者從系統中移除。 這是因為外部系統將作為最終真相來源。 因此，如果從外部提供者中移除檔案，則會將該檔案視為已不存在。 在連結（外部）資料夾中找不到任何檔案，可能會自動從[!DNL Workfront]中移除，且無法復原它們。
