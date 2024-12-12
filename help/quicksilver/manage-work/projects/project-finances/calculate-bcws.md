---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 計算已排程工作的預算成本(BCWS)
description: 「已排程工作之預算成本(BCWS)」也稱為計畫值，是專案效能量度，代表計算此量度時應該完成的工作量。
author: Lisa
feature: Work Management
exl-id: b9a36333-9430-42bd-99dd-3ad82803b633
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 2%

---

# 計算已排程工作的預算成本(BCWS)

## 已排程工作之預算成本概要(BCWS)

「已排程工作之預算成本(BCWS)」也稱為計畫值，是專案效能量度，代表計算此量度時應該完成的工作量。

Adobe Workfront會計算專案和任務的已排程工作預算成本(BCWS)。

檢閱任務或專案的BCWS值時，請考量下列事項：

* Workfront會根據您對專案之績效指數方法(PIM)的設定，計算任務的BCWS。

  您可以設定專案以使用時數或成本計算PIM，BCWS也使用相同的值計算。

  如需設定BCWS計算方式的詳細資訊，請參閱本文中[設定BCWS計算方式](#configure-how-bcws-is-calculated)一節。

* Workfront會將專案上所有父系任務和個別任務的所有BCWS值相加，以計算專案的BCWS。

  子系任務的值不會新增至專案的BCWS。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>
   <p>新增：標準</p>
   <p>或</p>
   <p>目前：計畫</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td>編輯專案的存取權</td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td>管理專案的許可權</td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 設定BCWS的計算方式 {#configure-how-bcws-is-calculated}

您可以設定如何計算專案的績效指數方法(PIM)，以設定以小時或成本計算BCWS。

1. 移至專案，然後按一下左側面板中的&#x200B;**專案詳細資料**。
1. 在&#x200B;**財務**&#x200B;區域中，找到&#x200B;**績效索引方法**&#x200B;欄位，然後按兩下以編輯它。

   ![](assets/pim-options-hour-cost-based-nwe.png)

1. 從下列選項中選取：

   | 選項 | 如何執行計算 |
   |---|---|
   | 基於小時 | Workfront會使用任務的計畫時數來計算BCWS。 |
   | 基於成本 | Workfront會使用任務的計畫成本來計算BCWS。 |


1. 按一下「**儲存變更**」。

   專案上任務的BCWS使用時數或成本計算。

## 計算BCWS

Workfront會使用下列公式，計算任務或專案的已排程工作預算成本(BCWS)：

```
Task BCWS = Planned Percent Complete x Task Budget
```

```
Project BCWS = SUM(BCWS values of all parent and individual tasks)
```

此計算中使用下列值：

| 使用的值 | 使用值的說明 |
|---|---|
| 計畫完成百分比 | 這是任務的完成百分比，方法是檢視任務開始與今天之間經過的時間量。 |
| 任務預算 | 這是任務的計畫時數或計畫成本值。 |

例如，如果今天是2月12日，而任務排程從2月10日持續到2月20日，則任務應該會在今天完成20%。 如果作業預算（計畫成本）為$10,000，則作業的BCWS為：

```
Task BCWS = 20% x $10,000 = $2,000
```

## 找出專案或任務的BCWS

您可以新增BCWS欄到您的檢視，以檢視報表或清單中排程之預算工作成本的值。

1. 前往任務或專案清單。
1. 展開&#x200B;**檢視**&#x200B;功能表並選取&#x200B;**新檢視**&#x200B;或&#x200B;**自訂檢視**。

1. 按一下「**新增欄**」。
1. 在&#x200B;**顯示在此資料行：**&#x200B;欄位中，開始輸入&#x200B;**BCWS**，然後按一下以在清單中顯示時選取它。

   ![](assets/bcws-in-project-view.png)

1. 按一下「**儲存視圖**」。
1. **BCWS**&#x200B;欄位會顯示在檢視中。
