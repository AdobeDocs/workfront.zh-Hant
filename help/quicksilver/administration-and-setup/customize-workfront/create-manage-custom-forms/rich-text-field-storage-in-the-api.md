---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: API中的RTF欄位儲存
description: 如果專案、問題或任務等物件包含RTF文字，則會儲存該物件，並透過Workfront API以參數值形式存取。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2e4b18be-14bb-4d47-8e63-e2f4a5dc376f
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---

# API中的RTF欄位儲存

如果專案、問題或任務等物件包含RTF文字，則會儲存該物件，並透過Workfront API以參數值形式存取。

可使用欄位，從包含RTF的專案物件要求文字資訊 **parameterValues**.

例如，簡單的HTTP要求可能類似下列：

`https://your-company.workfront.com/attask/api/v11.0/project?ID=your-project-ID&fields=parameterValues:*`

如果此範例專案包含自訂表單，且有3個自訂欄位：計算欄位、段落文本和rich 1。 然後，上述要求會傳回類似下列的回應，其中「rich 1」欄位是RTF參數欄位，而文字值是「**Hello** *世界！*&quot;:

```
{
	Data: {
		ID: “xxxxxxxxxxxxxxxxxxxxxxx”,
		name: “new project with rich text”,
		objCode: “PROJ”,
		- parameterValues: {
			DE:rich 1: “{
				"blocks":[
				{
					"key":"7eibh",
					"text":"Hello Word!",
					"type":"unstyled",
					"depth":0,
					"inlineStyleRanges":[
					{
						"offset":0,
						"length":6,
						"style":"BOLD"
					},
					{
						"offset":6,
						"length":5,
						"style":"ITALIC"
					}
					],
					"entityRanges":[
					],
				"data":{
				}
				}
				],
			"entityMap":{
			}
		}”,
		DE: paragraph text: “here is some paragraph text”,
		DE: calc field: “here is a calc field entry”,
		}
	}
}
```

如需深入了解RTF資訊的儲存方式，以及如何透過Adobe Workfront API擷取，請參閱 [Adobe Workfront API中的RTF欄位](../../../wf-api/general/rich-text-field-api.md).
