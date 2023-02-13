---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: 計算範例 — 從任務累計計算EAC
description: PIM =小時
author: Alina
feature: Work Management
exl-id: 68b582c9-f72a-4000-9d28-f7dafa23541f
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 8%

---

# 計算範例 — 從任務累計計算EAC

## EAC方法：從任務或子任務匯總

* [PIM=小時](#pim-hour-based)
* [PIM=基於成本](#pim-cost-based)

### PIM=小時 {#pim-hour-based}

* [簡單範例：項目沒有子任務](#simple-example-project-has-no-children-tasks)
* [複雜的範例：項目包含子任務](#complicated-example-project-has-children-tasks)

#### 簡單範例：項目沒有子任務 {#simple-example-project-has-no-children-tasks}

PIM =小時

EAC方法=從任務/子任務匯總

1. 建立項目A，其中三個任務（無子任務）均分配給成本/小時為$100.00的用戶1。
1. 將計畫/實際小時數添加到每個任務中，並根據下表完成%:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <br> <p><strong>任務</strong> </p> </th> 
   <th> <br> <p><strong>計畫小時</strong> </p> </th> 
   <th> <br> <p><strong>實際小時</strong> </p> </th> 
   <th> <p><strong>% 已完成</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>任務1</p> </td> 
   <td> <p>5小時</p> </td> 
   <td> <p>25小時</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務2</p> </td> 
   <td> <p>10小時</p> </td> 
   <td> <p>25小時</p> </td> 
   <td> <p>30%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務3</p> </td> 
   <td> <p>15小時</p> </td> 
   <td> <p>25小時</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 重新計算財務
1. **任務1的CPI** = .04計算方式如下：\
   **任務1的CPI** = *若* 實際小時數> 0 *THEN* CPI = TotalDekededCostWorkPerformed/Actual Hours\
       *ELSE* CPI = 1\
   **任務1的CPI** = 1 / 25\
   **任務1的CPI** = .04

1. **任務1的EAC** = 125小時計算如下：\
   **任務1的EAC** = *若* CPI &lt;> 0 *THEN* EAC =計畫小時數/CPI\
       *ELSE*

   ```
   EAC = Planned  Hours + Actual  Hours
   ```

   **任務1的EAC** = 5 / .04\
   **任務1的EAC** = 125小時

1. 任務2和3的CPI/EAC包括：\
   任務2 = .12 / 83.33小時\
   任務3 = .24 / 62.5小時

1. **項目CPI** = .13計算方式如下：\
   **項目CPI** = *若* 實際小時數> 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1\
   **項目CPI** = 10 / 75\
   **項目CPI** = .13

1. **專案的EAC** = 270.83小時計算如下\
   **專案的EAC** = EAC任務1 + EAC任務2 + EAC任務3\
   **專案的EAC** = 125 + 83.33 + 62.5\
   **專案的EAC** = 270.83小時

#### 複雜的範例：項目包含子任務 {#complicated-example-project-has-children-tasks}

PIM =小時

EAC方法=從任務/子任務匯總

1. 建立項目A，其中任務3是任務4和任務5的父項，任務1是任務2和任務3的父項，如下所示：\
   任務1\
      任務2\
      任務3\
         任務4\
         任務5\
   任務6

1. 將任務2、4、5和6分配給成本/人力費率為$100.00的用戶1。
1. 根據下表添加每個任務的計畫/實際小時數和完成百分比。

   >[!NOTE]
   >
   >對於任務1和任務3，您只添加實際小時數。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <br> <p><strong>任務</strong> </p> </th> 
   <th> <br> <p><strong>計畫小時</strong> </p> </th> 
   <th> <br> <p><strong>實際小時</strong> </p> </th> 
   <th> <p><strong>% 已完成</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>任務1</p> </td> 
   <td> </td> 
   <td> <p>10小時</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>任務2</p> </td> 
   <td> <p>5小時</p> </td> 
   <td> <p>10小時</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務3</p> </td> 
   <td> </td> 
   <td> <p>10小時</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>任務4</p> </td> 
   <td> <p>10小時</p> </td> 
   <td> <p>10小時</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務5</p> </td> 
   <td> <p>15小時</p> </td> 
   <td> <p>10小時</p> </td> 
   <td> <p>50%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務6</p> </td> 
   <td> <p>20小時</p> </td> 
   <td> <p>10小時</p> </td> 
   <td> <p>60%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 將50小時直接添加到項目（「更多」>「小時」>「記錄時數」），這樣就有5,000.00美元的實際人工成本直接記錄到項目中。
1. 運行重新計算財務
1. **任務2的CPI** = .1計算如下：\
   **任務2的CPI** = *若* 實際小時數> 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1\
   **任務2的CPI** = 1 / 10\
   **任務2的CPI** = .1

1. **任務2的EAC** = 50小時計算如下：\
   **任務2的EAC** = *若* CPI &lt;> 0 *THEN*

   ```
   EAC = Planned Hours / CPI
   ```

       *ELSE* EAC =計畫小時數+實際小時數\
   **任務2的EAC** = 5 / .1\
   **任務2的EAC** = 50小時

1. 任務4、任務5和任務6的CPI / EAC :\
   任務4 = .4 / 25小時\
   任務5 = .75 / 20小時\
   任務6 = 1.2 / 16.67小時

1. **任務3的CPI** = .38\
   **任務3的CPI** = *若* 實際小時數> 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1\
   **任務3的CPI** = 11.5 / 30\
   **任務3的CPI** = .38

1. **任務3的EAC** = EAC任務4 + EAC任務5\
   **任務3的EAC** = 25 + 20\
   **任務3的EAC** = 45小時

1. **任務1的CPI** = .25計算方式如下：\
   **任務1的CPI** = *若* 實際小時數> 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1\
   **任務1的CPI** = 12.5 / 50\
   **任務1的CPI** = .25

1. **任務1的EAC** = EAC任務2 + EAC任務3\
   **任務1的EAC** = 50 + 45\
   **任務1的EAC** = 95小時

1. 項目的CPI = .22，計算如下：\
   **項目CPI** = *若* 實際小時數> 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1\
   **項目CPI** = 24.5 / 110\
   **項目CPI** = .22272\
   **項目CPI** = .22

1. **專案的EAC** = EAC任務1 + EAC任務6\
   **專案的EAC** = 95 + 16.67\
   **專案的EAC** = 111.67小時

### PIM=基於成本 {#pim-cost-based}

* [簡單範例：項目沒有子任務](#simple-example-project-has-no-children-tasks)

#### 簡單範例：項目沒有子任務 {#simple-example-project-has-no-children-tasks-1}

PIM =基於成本

EAC方法=從任務/子任務匯總

1. 建立項目A，其中三個任務（無子任務）均分配給成本/小時為$100.00的用戶1。
1. 將計畫/實際小時數添加到每個任務中，並根據下表完成%:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <br> <p><strong>任務</strong> </p> </th> 
   <th> <br> <p><strong>計畫小時</strong> </p> </th> 
   <th> <br> <p><strong>Pln Lbr成本</strong> </p> </th> 
   <th> <br> <p><strong>實際小時</strong> </p> </th> 
   <th> <br> <p><strong>Act Lbr成本</strong> </p> </th> 
   <th> <p><strong>% 已完成</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>任務1</p> </td> 
   <td> <p>5小時</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>25小時</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務2</p> </td> 
   <td> <p>10小時</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>25小時</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>30%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務3</p> </td> 
   <td> <p>15小時</p> </td> 
   <td> <p>$1,500.00</p> </td> 
   <td> <p>25小時</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 根據下表為每個任務添加費用：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>任務</strong> </p> </th> 
   <th> <p><strong>費用</strong> </p> </th> 
   <th> <p><strong>計畫數量</strong> </p> </th> 
   <th> <p><strong>實際數量</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>任務1</p> </td> 
   <td> <p>任務1 Exp 1</p> </td> 
   <td> <p>$300.00</p> </td> 
   <td> <p>$400.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務1</p> </td> 
   <td> <p>任務1 Exp 2</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務2</p> </td> 
   <td> <p>任務2擴展</p> </td> 
   <td> <p>$200.00</p> </td> 
   <td> <p>$100.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務3</p> </td> 
   <td> <p>任務3擴展</p> </td> 
   <td> <p>$800.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 為項目添加兩項費用（即未與任務綁定），如下所示：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>費用</strong> </p> </th> 
   <th> <p><strong>計畫數量</strong> </p> </th> 
   <th> <p><strong>實際數量</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>專案Exp 1</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>$1,500.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務1 Exp 2</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 根據上述值，已產生/未產生成本釐定如下：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>任務</strong> </p> </th> 
   <th> <p><strong>未發生計畫費用</strong> </p> </th> 
   <th> <p><strong>已發生的計畫費用</strong> </p> </th> 
   <th> <p><strong>實際支出</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>任務1</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>$300.00</p> </td> 
   <td> <p>$400.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務2</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$200.00</p> </td> 
   <td> <p>$100.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務3</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$800.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>專案</p> </td> 
   <td> <p>$3,000.00</p> </td> 
   <td> <p>$2,300.00</p> </td> 
   <td> <p>$2,700.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 在項目活動中，運行重新計算財務
1. **任務1的CPI****** = .14計算方式如下：\
   **任務1的CPI******  = *若* 實際人工成本+已發生實際費用成本&lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **任務1的CPI******  =(100+300)/(2500+400)\
   **任務1的CPI******  = 400 / 2900\
   **任務1的CPI******  = .14

1. **任務1的EAC****** = 13,400.00美元\
   **任務1的CPI Labor****** =如果實際人工成本&lt;> 0，則

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **任務1的CPI Labor****** = 100/2500\
   **任務1的CPI Labor****** = .04

   **任務1的EAC人工****** = *若* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* EAC人工=計畫人工成本+實際人工成本\
   **任務1的EAC人工****** = 500.00/.04\
   **任務1的EAC人工****** = $12,500.00

   **任務1的EAC費用****** = ExcuredActualExpenseCost + NotExcuredPlannedExpense\
   **任務1的EAC費用****** = $400.00 + $500.00\
   **任務1的EAC費用****** = $900.00

   **任務1的EAC****** = EAC人工+ EAC費用\
   **任務1的EAC******  = $12,500.00 + $900.00\
   **任務1的EAC******  = 13,400.00美元

1. 以下是任務2和任務3的CPI/EAC值：\
   任務2 = .19 / 8,433.33美元\
   任務3 = .44 / 6,950.00美元****

1. 項目的CPI = .32\
   **項目的CPI****** = *若* 實際人工成本+已發生實際費用成本&lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **項目的CPI****** =(1000 + 2300)/(7500 + 2700)\
   **項目的CPI****** = 3300 / 10200\
   **項目的CPI****** = .32

1. 項目的EAC為28,783.33美元\
   **專案的EAC****** = EAC任務1 + EAC任務2 + EAC任務3\
   **專案的EAC****** = $13,400.00 + $8,433.33 + $6,950.00\
   **專案的EAC****** = $28,783.33
