---
title: 總覽
description: 總覽
author: Becky
draft: Probably
feature: Workfront API, Workfront Proof
exl-id: 882b657a-1bde-4efd-93e8-1de80c065b2d
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 1%

---

# 總覽

**歡迎使用Workfront Proof API**

Workfront Proof API是使用SSL保護的簡單HTTP服務。 API旨在提供您在我們自己的應用程式中使用的所有功能。

## 支援的格式

公共介面與WSDL支援相容，SOAP 1.1。 因此，所有要求都會透過HTTPS使用XML執行。

## API版本設定

為了保留與現有用戶端整合的相容性，我們在12.1版中導入了API版本設定。 請參閱  [API更新](http://api.proofhq.com/new-updates) 頁面以取得詳細資訊。 如果方法或參數沒有版本資訊，表示您會將此資訊視為標準API的一部分，請參閱下方的「API快速入門」一節。

## API快速入門

API入口點：

`https://soap.proofhq.com/soap` （請注意使用HTTPS）

可以在以下位置找到WSDL:

`https://soap.proofhq.com/soap?wsdl`

>[!NOTE]
>
>**此WSDL包含截至12.1版之前的所有變更，之後我們推出了API版本設定。 有關各種WSDL版本和即將進行的更改的詳細資訊，請參閱「API更新」頁**

每個API請求都需要工作階段金鑰。 此工作階段金鑰可識別執行動作的Workfront Proof使用者，並透過呼叫doLogin()方法並傳入使用者的電子郵件地址和密碼來取得。 只需在API請求序列之前呼叫doLogin()方法一次。 工作階段金鑰在短時間內保持作用中狀態，並會在每次方法呼叫時續約。 *我們很快將新增對權杖式驗證的支援。*

所有請求都使用下列信封、標題和內文格式：

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
