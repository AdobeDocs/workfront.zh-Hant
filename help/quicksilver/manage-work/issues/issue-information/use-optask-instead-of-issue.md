---
product-area: projects
navigation-topic: issue-information
title: 在引用問題時使用"opTask"和"issue"
description: 問題名稱在Adobe Workfront資料庫中顯示為opTask。 雖然有時需要使用問題欄位名稱來引用問題，但大多數時候在引用問題時必須使用opTask欄位名稱，而不是問題。
author: Alina
feature: Work Management
exl-id: 91107c04-616c-49b2-aa78-10e373d11f6b
source-git-commit: 813b97ee0979e29a90293d9ddaba12a33c99f64d
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---

# 在引用問題時使用&quot;opTask&quot;和&quot;issue&quot;

問題名稱顯示為 `opTask` 在Adobe Workfront資料庫里。 雖然有時你需要 `issue` 欄位名稱以引用問題，您大部分時間必須使用 `opTask` 欄位名稱 `issue` 引用問題時。

有關對象在Workfront資料庫中的顯示方式的詳細資訊，請參閱 [API資源管理器](https://developer.adobe.com/workfront/api-explorer/)。

## `opTask` 檔案名

使用 `opTask` 在以下上下文中引用問題時的欄位名稱：

* 建立問題的文本模式自定義報告時，希望引用視圖、篩選器、分組或提示中的問題。

   有關在報表中使用文本模式的詳細資訊，請參見 [文本模式概述](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)。

<!--* When you pull information about issues using our API.  
  For more information about the Workfront API, see [Adobe Workfront API](../../../wf-api/workfront-api.md)-->

* 在Kick-Start資料導入器工作表中更新問題欄位時。

   有關使用Kick-Start在Workfront導入資料的詳細資訊，請參見 [使用Kick-Start模板將資料導入Adobe Workfront](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md)。

## `issue` 欄位名稱

使用 `issue` 欄位名稱以引用以下上下文中的問題：

* 使用報表中的文本模式引用集合中的問題時。
* 使用WorkfrontAPI引用問題集合時。

有關收集報告的資訊，請參見 [報表中的引用集合](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md)。

<!--
<note type="tip">
For information about how issues appear in a collection, see the
<a href="https://developer.adobe.com/workfront/api-explorer/" target="_blank">API Explorer</a> and select the API Unsupported option from the upper-right corner of the page.
<br>(NOTE: Drafted because this might not be needed.)
</note>
-->
