---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: 修正時程表的工作週開始日期
description: 我時程表上星期的開始日期與我時程表設定檔上設定的一週開始日期不符。
author: Alina
feature: Timesheets
exl-id: 5c6c100f-2a04-4a6b-9f95-acc8de3a90f1
source-git-commit: d5d517a0c9a1292c37e66db07f7ed17d0a9a59e1
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---

# 修正時程表的工作週開始日期

## 問題

我的時程表上一週的開始日期與我時程表設定檔上設定的一週開始日期不符（如[建立、編輯和指派時程表設定檔](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)中所述）。

## 解決方案

Adobe Workfront中時程表一週的開始日期會使用瀏覽器中的語言和區域設定來決定一週的某天。 因此，您需要更新瀏覽器的語言和地區設定。

例如，瀏覽器語言設定為英文，地區設定為美國，一週從星期日開始。 或者，瀏覽器語言設定為英文，地區設定為英國，開始日期為星期一。

此設定也會影響整個系統快顯行事曆中一週的開始日期。

地區設定變更不會影響資源格線（或資源格線檢視）上的一週開始日期。 一週一律從星期日開始。

以下是Workfront支援的各種瀏覽器語言和區域設定變更的指示。

* **Chrome：**&#x200B;將下列連結複製並貼到您的Chrome瀏覽器： `chrome://settings/languages`然後移至語言。
* **Firefox：**複製下列連結並貼到您的Firefox瀏覽器： `about:preferences#content`然後移至[語言]。
* **IE 11：**&#x200B;工具 — >網際網路選項 — >一般 — >語言
* **Safari：**&#x200B;很遺憾，Safari不允許變更網頁瀏覽語言而不變更整個作業系統語言。 直接安裝其他瀏覽器(如Chrome或Firefox)可能會更容易。


