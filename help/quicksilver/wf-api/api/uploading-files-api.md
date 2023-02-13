---
content-type: api
navigation-topic: api-navigation-topic
title: 透過API上傳檔案
description: 透過API上傳檔案
author: John
feature: Workfront API
exl-id: 4e0b73b6-0d6d-4971-a87a-dfec85fb031a
source-git-commit: 03df0ad329255e86780c03bbb4541e0a0a526381
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# 透過API上傳檔案

您可以使用Workfront API搭配Postman等API工具或簡單的cURL命令來上傳檔案。

若要上傳檔案，請參閱 **上傳檔案** 在Workfront [貼文行為](https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FWF_API%2FGeneral%2Fapi-basics.html). 您也可以對cURL要求使用這些相同的指示。

**使用API工具上傳檔案時，請遵循下列准則：**

* 使用API工具選項來上傳檔案。 這通常是 **選擇檔案** 按鈕。

* 使用POSTHTTP方法來提出上傳檔案的要求。

* 您的要求應會產生包含其處理值的回應。

* 使用JSON裝載中objID的句柄值、物件類型和GUID值，進行後續呼叫。 這是用於為檔案建立物件，如下列範例所示：

```
}
"name": "TestPDF",
"handle": "7af257e64aba4a22c33ccdfc40bbb87",
"docObjCode": "PROJ",
"objID": "0398450f8345980843445534354",
"currentVersion": {"version": "v1.0", "fileName" : "TestPDF"},
}
```

您應會在回應中收到物件的ID。

如需詳細資訊，請參閱您所使用之特定API工具的說明。
