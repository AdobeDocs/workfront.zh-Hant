---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: DOCU對象不支援連結的資料夾
description: DOCU對象不支援連結的資料夾
author: Becky
feature: Workfront API
source-git-commit: 9bdc433158e471729bd27d701947d6ae41aa06e7
workflow-type: tm+mt
source-wordcount: '118'
ht-degree: 0%

---


# 不支援使用API來新增連結的資料夾

不支援使用API將連結的資料夾添加到文檔(DOCU)對象的資料夾陣列。 請求將會成功，但某些外部提供程式可能會從系統中刪除該文檔。 這是因為外部系統將被用作真相的最終來源。 因此，如果從外部提供程式中刪除文檔，則該文檔被視為已不存在。 在連結（外部）資料夾中找不到的任何文檔都可自動從 [!DNL Workfront] 卻無法復原。
