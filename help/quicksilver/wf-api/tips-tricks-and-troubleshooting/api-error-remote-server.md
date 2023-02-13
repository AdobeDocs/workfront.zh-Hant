---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: API錯誤訊息400錯誤請求
description: API錯誤訊息400錯誤請求
author: John
feature: Workfront API
exl-id: ab7c76a9-16ce-41f9-b7af-5943eb2dfdff
source-git-commit: 368a634b09d38a5b61c3e320f3f72e896694eeb1
workflow-type: tm+mt
source-wordcount: '90'
ht-degree: 0%

---


# API錯誤：&quot;遠程伺服器返回錯誤(400)錯誤請求&quot;

## 問題

嘗試使用API將自訂欄位匯入問題時，您會收到下列錯誤：

`The remote server returned an error: (400) Bad Request`

## 原因

當您嘗試透過API從沒有與佇列主題相關聯的自訂表單的專案匯入自訂欄位時，就會發生此錯誤。

## 解決方案

將正確的自訂表單新增至佇列主題。

若要進一步了解佇列主題，請參閱 [建立佇列主題](../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).
