---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: 更正工時單的工作周開始日
description: 我的時間表上的一週的開始日期與在時間表配置檔案上配置的一週的開始日期不匹配。
author: Alina
feature: Timesheets
exl-id: 5c6c100f-2a04-4a6b-9f95-acc8de3a90f1
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# 更正工時單的工作周開始日

## 問題

我的時間表上的一週的開始日期與在時間表配置檔案上配置的一週的開始日期不匹配(如 [建立、編輯和分配工時單配置檔案](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).)。

## 解決方案

Adobe Workfront中時間表的一週開始日使用瀏覽器中的語言和地區設定來判斷一週中的某天。 因此，您需要更新瀏覽器的語言和地區設定。 

例如，瀏覽器語言設為英文，地區設定為美國，一週從星期日開始。 或者，將瀏覽器語言設定為英文，將地區設定為英國，開始日為星期一。

此設定也會影響系統上快顯日曆中一週的開始日。

區域設定更改不會影響資源網格（或資源網格視圖）上一週的開始日。 一週一律從週日開始。

以下是Workfront支援之各種瀏覽器的語言和地區設定變更指示。

* **鉻黃：** 將下列連結複製並貼入您的Chrome瀏覽器： `chrome://settings/languages` 然後前往「語言」。
* **Firefox:**將下列連結複製並貼到您的Firefox瀏覽器中： `about:preferences#content` 然後前往「語言」。
* **IE 11:** 工具 — > Internet選項 — >常規 — >語言
* **Safari:** 很可惜，Safari不允許在變更網頁瀏覽語言的同時，變更您的整個作業系統語言。 只需安裝其他瀏覽器（例如Chrome或Firefox）可能會比較容易。

 
