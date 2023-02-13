---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 計算計畫效能索引(SPI)
description: 計畫效能指數(SPI)描述了計畫計畫與實際計畫之間的關係。
author: Alina
feature: Work Management
exl-id: 38259774-f22b-4b69-9e22-5b541118a7de
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 1%

---

# 計算計畫效能索引(SPI)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.)</p>
-->

計畫效能指數(SPI)描述了計畫計畫與實際計畫之間的關係。 Adobe Workfront計算項目和任務層的SPI。 項目經理將查看此度量，以確定當前是否提前或延遲跟蹤任務或項目。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>審核或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>查看對項目和財務資料的訪問</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>查看項目或具有查看財務權限的項目的更高權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 計畫效能索引(SPI)概述

* [SPI值顯示什麼](#what-the-spi-value-shows)
* [Workfront如何計算SPI](#how-workfront-calculates-spi)

### SPI值顯示什麼 {#what-the-spi-value-shows}

項目經理了解，SPI值為1表示項目處於計畫狀態或按計畫狀態。  值大於1表示項目提前，值小於1表示項目晚於計畫。  距1越遠，與計畫的偏差越大。

| **SPI值** | **指示「按計畫」** |
|---|---|
| 1 | 按計畫或按計畫 |
| > 1（大於1） | 提前 |
| &lt; 1（小於1） | 後排 |

{style=&quot;table-layout:auto&quot;}

### Workfront如何計算SPI  {#how-workfront-calculates-spi}

Workfront依下列公式計算SPI:

```
SPI = (Total Planned Hours x % Complete) / Planned Hours Scheduled to Date*
```

*&#42;如果計畫小時數計畫為日期= 0,SPI = 1*.

計畫小時計畫至日期在您執行計算時計算。 它顯示截至當前日期的計畫小時數。 當您將財務資料變更為準確時，系統會自動重新計算。 Workfront中沒有指出此值的欄位。

例如，如果您的項目包含1個任務，而任務有10個計畫小時和10天持續時間，則第5天的「計畫小時計畫至日期」為5。 

## 在項目或任務中查找SPI

1. 轉到要查看SPI的項目或任務。
1. 根據您要查看項目還是任務上的SPI，執行以下操作之一：

   1. 按一下 **專案詳細資料** 在左側面板中，然後檢視 **金融** 的上界。

   1. 按一下 **任務詳細資訊** 在左側面板中，然後檢視 **金融** 的上界。

      ![](assets/spi-on-project-nwe.png)

1. 尋找 **CPI/SPI/CSI** 欄位。
