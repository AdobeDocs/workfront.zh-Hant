---
content-type: api
navigation-topic: api-navigation-topic
title: 透過API上傳檔案
description: 透過API上傳檔案
author: Becky
feature: Workfront API
role: Developer
exl-id: 4e0b73b6-0d6d-4971-a87a-dfec85fb031a
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---

# 透過API上傳檔案

您可以使用Workfront API搭配API工具(例如Postman)或簡單的cURL命令來上傳檔案。

若要上傳檔案，請參閱 **正在上傳檔案** 在Workfront中 [貼文行為](/help/quicksilver/wf-api/general/api-basics.md#post-behavior). 您也可以對cURL請求使用這些相同的指示。

**使用API工具上傳檔案時，請遵循下列准則：**

* 使用API工具選項上傳檔案。 這些通常是 **選擇檔案** 按鈕。

* 使用POSTHTTP方法提出上傳檔案的請求。

* 您的請求應該會產生一個包含其控制代碼值的回應。

* 在JSON裝載中使用物件的控制代碼值、物件型別和GUID值，進行後續呼叫。 這是用來建立檔案的物件，如下列範例所示：

```
}
"name": "TestPDF",
"handle": "7af257e64aba4a22c33ccdfc40bbb87",
"docObjCode": "PROJ",
"objID": "0398450f8345980843445534354",
"currentVersion": {"version": "v1.0", "fileName" : "TestPDF"},
}
```

您應在回應中收到物件的ID。

如需詳細資訊，請參閱您使用的特定API工具的說明。
