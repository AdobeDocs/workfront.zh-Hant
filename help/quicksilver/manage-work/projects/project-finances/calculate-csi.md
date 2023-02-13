---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 計算成本計畫效能指數(CSI)
description: 成本計畫績效指數(CSI)是一種自動計算，它將成本績效指數(CPI)和計畫績效指數(SPI)結合為一個平衡成本和計畫的一般度量。
author: Alina
feature: Work Management
exl-id: 38a8c5e0-b812-499d-8fe7-a71ddccb3aad
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# 計算成本計畫效能指數(CSI)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.) </p>
-->

## 成本計畫績效指數(CSI)概覽

成本計畫績效指數(CSI)是一種自動計算，它將成本績效指數(CPI)和計畫績效指數(SPI)結合為一個平衡成本和計畫的一般度量。 將這些值相乘後，單一量度就能在較低預算中計入長期計畫，反之亦然。 項目經理可使用此功能來確定在成本被犧牲以推動項目中間計畫時的一般項目或任務運行狀況。

>[!TIP]
>
>Adobe Workfront會計算任務和專案的CSI。 Workfront不會計算問題的CSI值。

只有在貴組織中存在下列項目時，您才能從此量度提供的資訊中受益：

* 您的使用者正在記錄所完成工作的時間。\
   這會根據小時計算CSI。
* 您的使用者或工作角色具有與其相關聯的每小時成本率。 

   這會根據成本計算CSI。

## Workfront如何計算成本計畫效能指數(CSI)

Workfront使用以下公式計算項目或任務的成本效能指數(CSI):

```
CSI = CPI x SPI
```

有關CPI的資訊，請參見文章 [計算成本績效指數(CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md).

有關SPI的資訊，請參閱文章 [計算計畫效能索引(SPI)](../../../manage-work/projects/project-finances/calculate-spi.md).

CSI有以下三個可能值：

* 1 =遵循總體計畫   
* 
   >1 =預算計畫組合下
* &lt;1 =超出預算計畫組合

![](assets/csi-highlighted.png)

## 查找成本計畫效能指數(CSI)

>[!CAUTION]
>
>您必須具有訪問級別中查看財務資料的權限，並具有查看項目或任務的權限，才能查看項目或任務的CSI值。

您可以在下列Workfront區域找到CSI:

* 「項目詳細資訊」部分中的財務區域。
* 「任務詳細資訊」部分中的財務區域。
* 項目或任務視圖
* 項目或任務報告
