---
product-area: projects
navigation-topic: issue-information
title: 參考問題時使用「opTask」和「issue」
description: 問題的名稱會在Adobe Workfront資料庫中顯示為opTask 。 雖然有時您需要使用問題欄位名稱來參考問題，但大多數時候您在參考問題時都必須使用opTask欄位名稱而非問題。
author: Alina
feature: Work Management
exl-id: 91107c04-616c-49b2-aa78-10e373d11f6b
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/jrNMdSfyMO3MgzcxxKSNtrgzuY3e4ZNJpJ-JdvylJN4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 257
ht-degree: 1%

---

# 參考問題時使用「opTask」和「issue」

<!--Audited: 08/2025-->

問題名稱在Adobe Workfront資料庫中顯示為`opTask`。 雖然有時您需要使用`issue`欄位名稱來參考問題，但大多數時候您在參考問題時必須使用`opTask`欄位名稱，而非`issue`。

如需物件在Workfront資料庫中出現的詳細資訊，請參閱[API總管](https://developer.adobe.com/workfront/api-explorer/)。

## `opTask`欄位名稱

在參考下列內容中的問題時使用`opTask`欄位名稱：

* 當您建立問題的文字模式自訂報告，並且您想在檢視、篩選器、分組或提示中參考問題時。

  如需有關在報表中使用文字模式的詳細資訊，請參閱[文字模式概觀](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)。

<!--
* When you pull information about issues using our API.  
  For more information about the Workfront API, see [Adobe Workfront API](../../../wf-api/workfront-api.md)
  -->

* 當您更新Kick-Start資料匯入工具表中的問題欄位時。

  如需使用Kick-Start在Workfront中匯入資料的詳細資訊，請參閱[使用Kick-Start範本將資料匯入Adobe Workfront](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md)。

## `issue`欄位名稱

使用`issue`欄位名稱來參考下列內容中的問題：

* 當您在報告中使用文字模式參考集合中的問題時。
* 當您使用Workfront API參考問題集合時。

如需關於集合報表的資訊，請參閱報表中的[參考集合](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md)。

<!--
<note type="tip">
For information about how issues appear in a collection, see the
<a href="https://developer.adobe.com/workfront/api-explorer/" target="_blank">API Explorer</a> and select the API Unsupported option from the upper-right corner of the page.
<br>(NOTE: Drafted because this might not be needed.)
</note>
-->
