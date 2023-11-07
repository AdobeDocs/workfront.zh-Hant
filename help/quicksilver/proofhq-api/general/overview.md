---
title: 總覽
description: 總覽
author: Becky
draft: Probably
feature: Workfront API, Workfront Proof
role: Developer
exl-id: 882b657a-1bde-4efd-93e8-1de80c065b2d
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 1%

---

# 總覽

**歡迎使用Workfront Proof API**

Workfront Proof API是使用SSL保護的簡單HTTP服務。 此API旨在為您提供我們自己的應用程式中使用的所有功能。

## 支援的格式

公用介面與WSDL支援相容，與SOAP 1.1相容。 因此，所有要求都會透過HTTPS使用XML執行。

## API版本設定

為了保持與現有使用者端整合的相容性，我們從12.1版開始匯入API版本設定。 請參閱  [API更新](http://api.proofhq.com/new-updates) 頁面以取得詳細資訊。 如果方法或引數沒有版本資訊，表示您會在標準API中找到此專案，請參閱下方的「API快速入門」一節。

## 開始使用API

API進入點：

`https://soap.proofhq.com/soap` （請注意HTTPS的使用）

您可在下列位置找到WSDL：

`https://soap.proofhq.com/soap?wsdl`

>[!NOTE]
>
>**此WSDL包含12.1版之前的所有變更，之後我們引入了API版本設定。 請參閱API更新頁面，以取得各種WSDL版本和即將進行的變更的詳細資訊**

每個API要求都需要工作階段金鑰。 此工作階段金鑰可識別執行動作的Workfront Proof使用者，並透過呼叫doLogin()方法並傳入使用者的電子郵件地址和密碼來取得。 在一系列API要求之前，只需要呼叫一次doLogin()方法。 工作階段金鑰會維持作用中一小段時間，並在每次方法呼叫時更新。 *我們很快將新增對權杖型驗證的支援。*

所有要求都使用下列信封、標頭和正文格式：

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:urn="urn:proofhqapi">`
   <soapenv:Header/>
   <soapenv:Body>
       ... API function and data inserted here ...
    </soapenv:Body>
    </soapenv:Envelope>
```

## 常見問題集

如需常見問題的集合，請造訪 [此](http://api.proofhq.com/faqs) 頁面。
