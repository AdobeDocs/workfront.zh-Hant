---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: 專案預計開始日期概要
description: 「預計開始日期」是根據專案上第一個任務的預計開始日期而預計專案開始時間的即時日期。
author: Alina
feature: Work Management
exl-id: 6277e6cf-0a73-4ba8-a3fd-c0da473dc5d4
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# 專案預計開始日期概要

## 專案與任務的預計開始日期概要

「預計開始日期」是根據專案上第一個任務的預計開始日期而預計專案開始時間的即時日期。 

當您第一次計畫專案時，任務與專案的「計劃開始日期」和「預計開始日期」相同。 由於可能發生延遲或任務可能提前完成，所以預計開始日期可能會與計劃開始日期不同。 

專案上第一項任務的「預計開始日期」變更，會觸發專案的「預計開始日期」變更。 

## 修改任務的預計開始日期

專案或任務的預計開始日期是Adobe Workfront完成的計算，無法手動修改。 

下列事件可在任務的預計開始日期中觸發修改：

* 當您開始處理任務時，任務的「實際開始日期」會變成其「預計開始日期」。
* 如果任務的「計劃開始日期」通過，則「預計開始日期」會移至未來，表示任務可以開始的最早日期。\
  計算任務開始的最早可用日期時，Workfront會考量任務上的計畫時數金額，以及專案或指派給任務的使用者的排程。 
* 執行中落後的前置任務會影響其相依任務的預計開始日期。 相依任務的「預計開始日期」會根據前置任務關係的「相依性型別」以及前置任務的「預計日期」移動。 

若其中有任何任務為專案上的第一個任務，專案的「預計開始日期」會變更，以符合此任務的「預計開始日期」。 

## 找出專案或任務的預計開始日期

您可以在Workfront的下列區域中找到專案或任務的「預計開始日期」：

* 您可以將其新增到專案、任務報告或檢視。

  如需有關建立報告的詳細資訊，請參閱文章[建立自訂報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

* 在專案的專案詳細資訊區段或任務的任務詳細資訊區段中。
