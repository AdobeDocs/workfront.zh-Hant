---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: API中的RTF文字欄位儲存
description: 如果專案、問題或任務等物件包含RTF文字，則會透過Workfront API將其儲存為引數值以供存取。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 2e4b18be-14bb-4d47-8e63-e2f4a5dc376f
source-git-commit: 3f7f4557c18bbb91ece850f910350d926a9e84bf
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---

# API中的RTF文字欄位儲存

如果專案、問題或任務等物件包含RTF文字，則會透過Workfront API將其儲存為引數值以供存取。

使用欄位&#x200B;**parameterValues**&#x200B;可以從包含RTF文字的專案物件要求文字資訊。

例如，簡單的HTTP請求可能類似於以下內容：

`https://your-company.workfront.com/attask/api/v11.0/project?ID=your-project-ID&fields=parameterValues:*`

如果此範例專案包含具有3個自訂欄位的自訂表單：計算欄位、段落文字和RTF 1。 接著，上述要求會傳回類似下列的回應，其中「rich 1」欄位是RTF引數欄位，而文字值為「**Hello** *World！*」：

```
{
    Data: {
        ID: "xxxxxxxxxxxxxxxxxxxxxxx",
        name: "new project with rich text",
        objCode: "PROJ",
        - parameterValues: {
            DE:rich 1: "{
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
        }",
        DE: paragraph text: "here is some paragraph text",
        DE: calc field: "here is a calc field entry",
        }
    }
}
```

如需深入瞭解RTF資訊的儲存方式，以及透過Adobe Workfront API擷取的方式，請參閱Adobe Workfront API中的[RTF欄位](../../../wf-api/general/rich-text-field-api.md)。
