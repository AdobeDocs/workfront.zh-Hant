---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: API錯誤訊息400錯誤請求
description: API錯誤訊息400錯誤請求
author: Becky
feature: Workfront API
role: Developer
exl-id: ab7c76a9-16ce-41f9-b7af-5943eb2dfdff
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '90'
ht-degree: 0%

---


# API錯誤：「遠端伺服器傳回錯誤(400)錯誤請求」

## 問題

嘗試使用API將自訂欄位匯入問題時，出現以下錯誤：

`The remote server returned an error: (400) Bad Request`

## 原因

當您嘗試透過API匯入專案的自訂欄位時，此錯誤會發生，該專案沒有與佇列主題相關聯的自訂表單。

## 解決方案

將正確的自訂表單新增至佇列主題。

若要深入瞭解佇列主題，請參閱 [建立佇列主題](../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).
