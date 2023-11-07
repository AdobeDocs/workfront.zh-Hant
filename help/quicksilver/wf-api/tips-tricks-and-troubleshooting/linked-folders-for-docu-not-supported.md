---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: DOCU物件不支援連結資料夾
description: DOCU物件不支援連結資料夾
author: Becky
feature: Workfront API
role: Developer
exl-id: 33b5a998-f3e1-42a2-852e-fb862d770d50
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '118'
ht-degree: 0%

---

# 不支援使用API新增連結的資料夾

不支援使用API將連結資料夾新增至檔案(DOCU)物件的資料夾陣列。 請求將成功，但檔案可能會由某些外部提供者從系統中移除。 這是因為外部系統將作為最終真相來源。 因此，如果從外部提供者中移除檔案，則會將該檔案視為已不存在。 連結（外部）資料夾中找不到任何檔案，都會自動從中移除 [!DNL Workfront] 無法復原它們。
