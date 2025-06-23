---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 計算成本排程績效指數(CSI)
description: 成本排程績效指數(CSI)是一種自動計算，它將「成本績效指數(CPI)」與「排程績效指數(SPI)」結合為一個一般度量，以平衡成本與排程。
author: Lisa
feature: Work Management
exl-id: 38a8c5e0-b812-499d-8fe7-a71ddccb3aad
source-git-commit: abf5f21281b05dedfecbe71c6ffbf54ee69e2460
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# 計算成本排程績效指數(CSI)

<!-- Audited: 6/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.) </p>
-->

## 成本排程績效指數(CSI)概要

成本排程績效指數(CSI)是一種自動計算，它將「成本績效指數(CPI)」與「排程績效指數(SPI)」結合為一個一般度量，以平衡成本與排程。 將這些值相乘，單一量度就能以較低預算處理較長的排程，反之亦然。 當犧牲成本以推動專案中間的排程時，專案經理可以使用此項來判斷一般專案或任務狀況。

>[!TIP]
>
>Adobe Workfront會計算任務和專案的CSI，但不會計算問題。

只有當您的組織中存在以下情況時，您才能從此量度提供的資訊中獲益：

* 您的使用者正在記錄完成工作的時間。 這會根據時數計算CSI。
* 您的使用者或工作角色具有與其關聯的每小時成本費率。 這會根據成本計算CSI。

## Workfront如何計算成本排程績效指數(CSI)

Workfront會使用下列公式計算專案或作業的成本績效指數(CSI)：

`CSI = CPI x SPI`

如需有關CPI的資訊，請參閱文章[計算成本績效指數(CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md)。

如需SPI的相關資訊，請參閱文章[計算排程績效指數(SPI)](../../../manage-work/projects/project-finances/calculate-spi.md)。

CSI有下列三個可能的值：

* 1 =遵循整體計畫
* \>1 =在預算排程組合之下
* &lt;1 =超出預算排程組合

![CSI](assets/csi-highlighted.png)

## 找出成本排程績效指數(CSI)

>[!CAUTION]
>
>您必須擁有存取層級中「檢視財務資料」的存取權，以及檢視專案或任務的許可權，才能檢視專案或任務的CSI值。

您可以在Workfront的下列區域中找到CSI：

* 「專案詳細資訊」區段中的「財務」區域。
* 「工作詳細資訊」區段中的「財務」區域。
* 專案或任務檢視。
* 專案或任務報告。
