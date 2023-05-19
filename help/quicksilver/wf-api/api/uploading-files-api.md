---
content-type: api
navigation-topic: api-navigation-topic
title: 通過API上載檔案
description: 通過API上載檔案
author: Becky
feature: Workfront API
exl-id: 4e0b73b6-0d6d-4971-a87a-dfec85fb031a
source-git-commit: 3db01c329c005570b782ae3445f83b7c44ced676
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---

# 通過API上載檔案

您可以使用API工具(如Postman)或簡單的cURL命令使用WorkfrontAPI上載檔案。

要上載文檔，請參閱 **正在上載文檔** 在Workfront [帖子行為](/help/quicksilver/wf-api/general/api-basics.md#post-behavior)。 您也可以對cURL請求使用這些相同的說明。

**使用API工具上載檔案時，請遵循以下准則：**

* 使用API工具選項上載檔案。 這通常是 **選擇檔案** 按鈕。

* 使用POSTHTTP方法來請求上載檔案。

* 您的請求應生成包含其句柄值的響應。

* 使用JSON負載中objID的句柄值、對象類型和GUID值進行後續調用。 這用於為檔案建立對象，如下例所示：

```
}
"name": "TestPDF",
"handle": "7af257e64aba4a22c33ccdfc40bbb87",
"docObjCode": "PROJ",
"objID": "0398450f8345980843445534354",
"currentVersion": {"version": "v1.0", "fileName" : "TestPDF"},
}
```

您應在響應中接收對象的ID。

有關詳細資訊，請參閱所使用的特定API工具的幫助。
