---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''檢視：通過縮進任務的'
description: 通過將自定義視圖添加到任務清單中，並確保在導出該清單之前選擇了此視圖，可以保持導出任務清單中父 — 子關係的區別。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4987501f-a1d9-47cd-bfbe-83acfc225204
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 1%

---

# 查看：通過縮進任務來顯示任務中的父子關係

通過將自定義視圖添加到任務清單中，並確保在導出該清單之前選擇了此視圖，可以保持導出任務清單中父 — 子關係的區別。  

![](assets/parent-child-indented-custom-view-350x94.png)

1. 轉到包含要導出的任務清單的項目。
1. 按一下 **檢視** 下拉式功能表，然後選取 **新建視圖**.

1. 在畫面左上角為篩選器命名。
1. 按一下 **任務名稱** 欄標題。

1. 選擇 **切換到文本模式** 在右上角。
1. 按一下文本框中的任意位置可編輯文本，並刪除所有現有文本。
1. 貼上下列文字：

   ```
   displayname=<br>linkedname=direct<br>namekey=name<br>querysort=name<br>textmode=true<br>valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(" - ",{name}),IF({indent}<3,CONCAT(" - - ",{name}),IF({indent}<4,CONCAT(" - - - ",{name}),CONCAT(" - - - - ",{name})))))<br>valueformat=HTML
   ```

1. 按一下&#x200B;**儲存**。
1. 按一下 **保存視圖**.
