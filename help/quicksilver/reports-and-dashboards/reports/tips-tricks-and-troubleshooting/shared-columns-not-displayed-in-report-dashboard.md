---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 來自共用欄的資料不會顯示在儀表板報表中
description: 將報表置於多欄控制面板配置時，不會顯示共用欄的資料，但會顯示於單一欄配置中。 也會覆寫分行符號。
author: Courtney
feature: Reports and Dashboards
exl-id: b8307182-3ec1-4f16-8427-48ef7a65f969
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/OEFlwkdPf98g4-rC1tzaTmmEwb5-BXHx-j8XGrRR8sE
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 162
ht-degree: 1%

---

# 來自共用欄的資料不會顯示在儀表板報表中

## 問題

將報表置於多欄控制面板配置時，不會顯示共用欄的資料，但會顯示於單一欄配置中。 也會覆寫分行符號。

## 原因

僅限標籤為的欄

```
shortview=true
```

當儀表板配置設定為左/右分割或左/中/右分割時，報告儀表板檢視中會包含儀表板檢視。

## 解決方案

存取報告中使用的檢視，並開啟文字模式。 （如需詳細資訊，請參閱[使用文字模式編輯檢視](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md)。） 為報表中的所有欄加上標籤，包括共用/合併欄中所使用的欄，使用

```
shortview=true
```

. 之後，報告欄即可在控制面板中正確顯示。
