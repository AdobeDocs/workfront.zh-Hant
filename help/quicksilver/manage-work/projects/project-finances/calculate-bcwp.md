---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 計算已執行工作的預算成本(BCWP)
description: 「已執行工作之預算成本(BCWP)」也稱為「盈餘值」，是一種專案績效量度，代表計算此量度時實際完成的工作量。
author: Lisa
feature: Work Management
exl-id: 203709a7-e522-4875-b3eb-40b967a938ec
source-git-commit: 23a4d055871c9138818e70fa1cd936581dbd7552
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 2%

---

# 計算已執行工作的預算成本(BCWP)

## 預算執行工作成本概要(BCWP)

「已執行工作之預算成本(BCWP)」也稱為「盈餘值」，是一種專案績效量度，代表計算此量度時實際完成的工作量。

Adobe Workfront會計算專案與任務的已執行工作預算成本(BCWP)。

檢閱任務或專案的BCWP值時，請考量下列事項：

* Workfront會根據您對專案績效指數方法(PMI)的設定，計算任務的BCWP。

  您可以設定專案以使用時數或成本計算PMI，BCWP也使用相同的值計算。

  如需有關設定BCWP計算方式的資訊，請參閱本文中的[設定BCWP計算方式](#configure-how-bcwp-is-calculated)一節。

* Workfront會將專案上所有父系任務和個別任務的所有BCWP值相加，以計算專案的BCWP。

  子系任務的值不會新增至專案的BCWP。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront套件</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td>
   <p>標準</p>
   <p>規劃</p></td> 
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td>編輯專案的存取權</td> 
  </tr> 
  <tr> 
   <td>物件許可權</td> 
   <td>管理專案的許可權</td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 設定BCWP的計算方式 {#configure-how-bcwp-is-calculated}

您可以設定如何計算專案的績效指數方法(PIM)，以設定以小時或成本計算BCWP。

1. 移至專案，並在左側面板中展開&#x200B;**專案詳細資料**。
1. 在&#x200B;**財務**&#x200B;區域中，找到&#x200B;**績效索引方法**&#x200B;欄位，然後按兩下以編輯它。

   ![PIM選項](assets/pim-options-hour-cost-based-nwe.png)

1. 從下列選項中選取：

   | 選項 | 如何執行計算 |
   |---|---|
   | 基於小時 | Workfront會使用任務的計畫時數來計算BCWP。 |
   | 基於成本 | Workfront使用任務的計畫成本來計算BCWP。 |

1. 按一下「**儲存變更**」。

專案上任務的BCWP使用時數或成本計算。

## 計算BCWP

Workfront會使用下列公式，計算任務或專案的已執行工作預算成本(BCWP)：

```
Task BCWP = Actual Percent Complete x Task Budget
```

```
Project BCWP = SUM(BCWP values of all parent and individual tasks)
```

下列值用於這些計算：

| 使用的值 | 使用值的說明 |
|---|---|
| 實際完成百分比 | 這是顯示在Workfront中的任務實際完成百分比。 |
| 任務預算 | 這是任務的計畫時數或計畫成本值。 |

例如，如果作業的實際完成百分比為25%，而「作業預算」或「計畫成本」為$10,000，則作業的BCWP為：

```
BCWP = 25% x $10,000 = $2,500
```

## 找出專案或任務的BCWP

您可以新增BCWP欄至您的檢視，以在報表或清單中檢視已執行工作的預算成本值。

1. 前往任務或專案清單。
1. 展開&#x200B;**檢視**&#x200B;功能表並選取&#x200B;**新檢視**&#x200B;或&#x200B;**自訂檢視**。

1. 按一下「**新增欄**」。
1. 在&#x200B;**顯示在此欄：**&#x200B;欄位中開始輸入&#x200B;**BCWP**，然後按一下以在清單中顯示時選取它。

   專案檢視中的![BCWP](assets/bcwp-project-view.png)

1. 按一下「**儲存視圖**」。
1. BCWP欄位會顯示在檢視中。
