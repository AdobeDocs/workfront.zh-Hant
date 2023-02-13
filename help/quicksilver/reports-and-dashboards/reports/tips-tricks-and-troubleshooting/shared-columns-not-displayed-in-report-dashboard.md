---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 共用欄的資料不會顯示在控制面板報表中
description: 將報表置於多欄控制面板配置時，共用欄的資料不會顯示，但會顯示在單一欄配置上。 換行符也被覆蓋。
author: Nolan
feature: Reports and Dashboards
exl-id: b8307182-3ec1-4f16-8427-48ef7a65f969
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 0%

---

# 共用欄的資料不會顯示在控制面板報表中

## 問題

將報表置於多欄控制面板配置時，共用欄的資料不會顯示，但會顯示在單一欄配置上。 換行符也被覆蓋。

## 原因

僅限標示為的欄

```
shortview=true
```

當控制面板配置設定了左/右分割或左/中/右分割時，就會納入報表的控制面板檢視中。

## 解決方案

存取報表中使用的檢視並開啟文字模式。 (如需詳細資訊，請參閱 [使用文本模式編輯視圖](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md).) 為報表中的所有欄加上標籤，包括共用/合併欄中使用的欄，使用

```
shortview=true
```

.然後報表欄就會在控制面板中正確顯示。
