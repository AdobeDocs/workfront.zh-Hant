---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: 計算示例 — 在項目級別計算EAC
description: PIM =小時
author: Alina
feature: Work Management
exl-id: ff88b7e3-2a5b-464f-bed1-6848067840b8
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1768'
ht-degree: 9%

---

# 計算示例 — 在項目級別計算EAC

## EAC方法：在專案層級計算

* [PIM =小時](#pim-hour-based)
* [PIM=基於成本](#pim-cost-based)

### PIM =小時 {#pim-hour-based}

* [簡單範例：項目沒有子任務](#simple-example-project-has-no-children-tasks)
* [複雜的範例：項目包含子任務](#complicated-example-project-has-children-tasks)

#### 簡單範例：項目沒有子任務 {#simple-example-project-has-no-children-tasks}

PIM =小時

EAC方法=在專案層級計算****

1. 建立項目A，其中三個任務（無子任務）均分配給成本/小時為$100.00的用戶1。
1. 將計畫小時數和實際小時數添加到每個任務中，並根據下表完成%:

   <table style="table-layout:auto">
    <col>
    <col>
    <col>
    <col>
    <thead>
     <tr>
      <th><br><p><strong>任務</strong></p></th>
      <th><br><p><strong>計畫小時</strong></p></th>
      <th><br><p><strong>實際小時</strong></p></th>
      <th><p><strong>完成百分比</strong></p></th>
     </tr>
    </thead>
    <tbody>
     <tr>
      <td><p>任務1</p></td>
      <td><p>5小時</p></td>
      <td><p>25小時</p></td>
      <td><p>20%</p></td>
     </tr>
     <tr>
      <td><p>任務2</p></td>
      <td><p>10小時</p></td>
      <td><p>25小時</p></td>
      <td><p>30%</p></td>
     </tr>
     <tr>
      <td><p>任務3</p></td>
      <td><p>15小時</p></td>
      <td><p>25小時</p></td>
      <td><p>40%</p></td>
     </tr>
    </tbody>
   </table>

1. 重新計算項目上的財務。
1. **任務1的CPI** = .04計算方式如下：\
   **任務1的CPI** = *若* 實際小時數> 0 *THEN* CPI = TotalDekededCostWorkPerformed/Actual Hours\
      *ELSE* CPI = 1\
   **任務1的CPI** = 1 / 25\
   **任務1的CPI** = .04

1. **任務1的EAC** = 125小時計算如下：\
   **任務1的EAC** = *若* CPI &lt;> 0 *THEN* EAC =計畫時數/CPI\
       *ELSE* EAC =計畫小時數+實際小時數\
   **任務1的EAC** = 5 / .04\
   **任務1的EAC** = 125小時****

1. 任務2和3的CPI/EAC包括：\
   任務2 = .12 / 83.33小時\
   任務3 = .24 / 62.5小時

1. **項目CPI** = .13計算方式如下：\
   **項目CPI** = *若* 實際小時數> 0 *THEN* CPI = TotalDekededCostWorkPerformed/Actual Hours\
       *ELSE* CPI = 1\
   **項目CPI** = 10 / 75\
   **項目CPI** = .13

1. **專案的EAC** = 225小時計算如下：\
   **專案的EAC** = *若* CPI &lt;> 0 *THEN* EAC =計畫時數/CPI\
       *ELSE* EAC =計畫小時數+實際小時數\
   **專案的EAC** = 30 / .13333\
   **專案的EAC** = 225小時

#### 複雜的範例：項目包含子任務 {#complicated-example-project-has-children-tasks}

PIM =小時

EAC方法=在專案層級計算

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

1. 將50小時直接新增至專案（「更多>小時>記錄時數」）。
1. **任務2的CPI** = .1計算如下：\
   **任務2的CPI** = *若* 實際小時數> 0 *THEN* CPI = TotalDekededCostWorkPerformed/Actual Hours\
       *ELSE* CPI = 1\
   **任務2的CPI** = 1 / 10\
   **任務2的CPI** = .1

1. **任務2的EAC** = 50小時計算如下：\
   **任務2的EAC** = *若* CPI &lt;> 0 *THEN* EAC =計畫時數/CPI\
       *ELSE* EAC =計畫小時數+實際小時數\
   **任務2的EAC** = 5 / .1\
   **任務2的EAC** = 50小時

1. 任務4、5和6的CPI/EAC如下：\
   任務4:.4 / 25小時\
   任務5:.75 / 20小時\
   任務6:1.2 / 16.67小時

1. **任務3的CPI** = .38計算方式如下：\
   **任務3的CPI** = *若* 實際小時數> 0 *THEN* CPI = TotalDekededCostWorkPerformed/Actual Hours\
       *ELSE* CPI = 1\
   **任務3的CPI** = 11.5 / 30\
   **任務3的CPI** = .38

1. **任務3的EAC** = 65.22小時計算如下：\
   **任務3的EAC** = *若* CPI &lt;> 0 *THEN* EAC =計畫時數/CPI\
       *ELSE* EAC =計畫小時數+實際小時數\
   **任務3的EAC** = 25 / .383333\
   **任務3的EAC** = 65.22小時

1. **任務1的CPI** = .25計算方式如下：\
   **任務1的CPI** = *若* 實際小時數> 0 *THEN* CPI = TotalDekededCostWorkPerformed/Actual Hours\
       *ELSE* CPI = 1\
   **任務1的CPI** = 12.5 / 50\
   **任務1的CPI** = .25

1. **任務1的EAC** = 120小時計算如下：\
   **任務1的EAC** = *若* CPI &lt;> 0 *THEN* EAC =計畫小時數/CPI\
       *ELSE* EAC =計畫小時數+實際小時數\
   **任務1的EAC** = 30/ .25\
   **任務1的EAC** = 120小時

1. **項目CPI** = .22計算方式如下：\
   **項目CPI** = *若* 實際小時數> 0 *THEN* CPI = TotalDekededCostWorkPerformed/Actual Hours\
       *ELSE* CPI = 1\
   **項目CPI** = 24.5 / 110\
   **項目CPI** = .22272\
   **項目CPI** = .22

1. **專案的EAC** = 224.49小時計算如下：\
   **專案的EAC** = *若* CPI &lt;> 0 *THEN* EAC =計畫時數/CPI\
       *ELSE* EAC =計畫小時數+實際小時數\
   **專案的EAC** = 50 / .22272\
   **專案的EAC** = 224.49小時

### PIM=基於成本 {#pim-cost-based}

* [簡單範例：項目沒有子任務](#simple-example-project-has-no-children-tasks)
* [複雜的範例：項目包含子任務](#complicated-example-project-has-children-tasks)

#### 簡單範例：項目沒有子任務 {#simple-example-project-has-no-children-tasks-1}

PIM =基於成本

EAC方法=在專案層級計算

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
   <td> <p> $2,700.00 <strong></strong></p> </td> 
  </tr> 
 </tbody> 
</table>

1. 在項目活動中，運行重新計算財務
1. **任務1的CPI** = .14
1. **任務1的CPI****** = .14計算方式如下：\
   **CPI**  **任務1** = *若* 實際人工成本+已發生實際費用成本&lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *    ELSE* CPI = CPI_Labor\
   **任務1的CPI****** =(100+300)/(2500+400)\
   **CPI**  **任務1** = 400 / 2900\
   **CPI**  **任務1**  = .14****

1. **任務1的EAC****** = 13,400.00美元\
   **CPI勞工**  **任務1** =如果實際人工成本&lt;> 0，則

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **CPI勞工**  **任務1** = 100/2500\
   **CPI勞工**  **任務1** = .04 ****** EAC勞動力&#x200B;****任務1 **=*若&#x200B;*CPI_Labor &lt;> 0*THEN *EAC人工=計畫人工成本/CPI_人工\
   *    ELSE* EAC人工=計畫人工成本+實際人工成本\
   **EAC勞動力&#x200B;****任務1** = 500.00/.04\
   **任務1的EAC人工****** = $12,500.00\
   **任務1的EAC費用****** = ExcuredActualExpenseCost + NotExcuredPlannedExpense\
   **任務1的EAC費用****** = $400.00 + $500.00\
   **任務1的EAC費用****** = $900.00\
   **任務1的EAC****** = EAC人工+ EAC費用\
   **任務1的EAC******  = $12,500.00 + $900.00\
   **任務1的EAC******  = 13,400.00美元

1. 以下是任務2和任務3的CPI/EAC值：\
   任務2 = .19 / 8,433.33美元\
   任務3 = .44 / 6,950.00美元

1. **項目CPI** = .32計算方式如下：\
   **項目的CPI****** = *若* 實際人工成本+已發生實際費用成本&lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **項目的CPI****** =(1000 + 2300)/(7500 + 2700)\
   **項目的CPI****** = 3300 / 10200\
   **項目的CPI****** = .32

1. **專案的EAC** = $28,200.00，計算方式如下：\
   **CPI Labor**** for Project** =如果實際人工成本&lt;> 0，則

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **CPI Labor**** for Project** = 1000 / 7500\
   **CPI Labor**** for Project** = .13333\
   **CPI Labor**** for Project** = .13

   **EAC項目人工****** = *若* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   *   ELSE* EAC人工=計畫人工成本+實際人工成本\
   **EAC項目人工****** = 3000/ .13333\
   **EAC項目人工****** = $22,500.00

   **EAC費用****項目** =

   ```
   IncurredActualExpenseCost + NotIncurredPlannedExpense
   ```

   **EAC費用****項目** = $3000.00 + 2,700.00\
   **EAC費用****項目** = $5,700.00

   **EAC****項目** = EAC人工+ EAC費用\
   **EAC****項目**  = $22,500.00 + $5,700.00\
   **EAC****項目**  = $28,200.00

#### 複雜的範例：項目包含子任務 {#complicated-example-project-has-children-tasks-1}

PIM =基於成本

EAC方法=在專案層級計算

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
   <td> </td> 
   <td> </td> 
   <td> <p>10小時</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>任務2</p> </td> 
   <td> <p>5小時</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>10小時</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務3</p> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p>10小時</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>任務4</p> </td> 
   <td> <p>10小時</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>10小時</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務5</p> </td> 
   <td> <p>15小時</p> </td> 
   <td> <p>$1,500.00</p> </td> 
   <td> <p>10小時</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>50%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務6</p> </td> 
   <td> <p>20小時</p> </td> 
   <td> <p>$2,000.00</p> </td> 
   <td> <p>10小時</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>60%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 將50小時直接添加到項目（「更多」>「小時」>「記錄時數」），這樣就有5,000.00美元的實際人工成本直接記錄到項目中。 ****
1. 根據下表為每個任務添加費用（我已在每個任務之間添加一個空白行，以便更容易閱讀）:

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
   <td> <p>-$400.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務1</p> </td> 
   <td> <p>任務1 Exp 2</p> </td> 
   <td> <p>-$500.00</p> </td> 
   <td> <p>$800.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務1</p> </td> 
   <td> <p>任務1 Exp 3</p> </td> 
   <td> <p>$400.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>任務2</p> </td> 
   <td> <p>任務2 Exp 1</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務2</p> </td> 
   <td> <p>任務2 Exp 2</p> </td> 
   <td> <p>-$400.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務2</p> </td> 
   <td> <p>任務2 Exp 3</p> </td> 
   <td> <p>-$200.00</p> </td> 
   <td> <p>$600.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務2</p> </td> 
   <td> <p>任務2 Exp 4</p> </td> 
   <td> <p>$700.00</p> </td> 
   <td> <p>-$200.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>任務3</p> </td> 
   <td> <p>任務3擴展</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$1,000.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>任務4</p> </td> 
   <td> <p>任務4 Exp 1</p> </td> 
   <td> <p>$800.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務4</p> </td> 
   <td> <p>任務4 Exp 2</p> </td> 
   <td> <p>-$100.00</p> </td> 
   <td> <p>$300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務4 </p> </td> 
   <td> <p>任務4 Exp 3</p> </td> 
   <td> <p>-200.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>任務5</p> </td> 
   <td> <p>任務5 Exp 1</p> </td> 
   <td> <p>$700.00</p> </td> 
   <td> <p>$800.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務5</p> </td> 
   <td> <p>任務5 Exp 2</p> </td> 
   <td> <p>-$100.00</p> </td> 
   <td> <p>$300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務5</p> </td> 
   <td> <p>任務5擴展3</p> </td> 
   <td> <p>-$400.00</p> </td> 
   <td> <p>-$200.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>任務6</p> </td> 
   <td> <p>任務6 Exp 1</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務6</p> </td> 
   <td> <p>任務6 Exp 2</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>-$300.0</p> </td> 
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
   <td> <p> $0.00 <strong></strong></p> </td> 
  </tr> 
 </tbody> 
</table>

1. 根據上述價值，已產生/未產生成本釐定如下：

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
   <td> <p>$400.00</p> </td> 
   <td> <p>-$500.00</p> </td> 
   <td> <p>$800.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務2</p> </td> 
   <td> <p>-$400.00</p> </td> 
   <td> <p>$300.00</p> </td> 
   <td> <p>$1,300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務3</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$1,000.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務4</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>-$100.00</p> </td> 
   <td> <p>$300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務5</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>$1,100.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務6</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>專案</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>$1000.00</p> </td> 
   <td> <p>$1,500.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 在項目活動中，運行重新計算財務
1. **CPI** 對於任務2 = .17，計算如下：\
   **CPI任務2** = *若* 實際人工成本+已發生實際費用成本&lt;> 0 *THEN* CPI =(TotalDekededCostWorkPerformed + ExceedPlannedExpenseCost)/(ActualLaborCost + ExcedActualExpenseCost)\
   *   ELSE* CPI = CPI_Labor\
   **CPI****任務2** =(100+300)/(1000+1300)\
   **CPI****任務2**  = 400 / 2300\
   **CPI****任務2**  = .17

1. **EAC** 任務2 = $5,900.00\
   **CPI勞工****任務2** =如果實際人工成本&lt;> 0，則CPI_人工= TotalBudgetedCostWorkPerformed /實際人工成本\
      ELSE CPI_Labor = 1\
   **CPI勞工****任務2** = 100/1000\
   **CPI勞工****任務2** = .1

   **EAC人工****任務2** = *若* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   *   ELSE* EAC人工=計畫人工成本+實際人工成本\
   **EAC人工****任務2** = 500.00/.1\
   **EAC人工****任務2** = $5,000.00 ****** EAC費用&#x200B;****任務2 **= ExcuredActualExpenseCost + NotExcuredPlannedExpense\
   **EAC費用&#x200B;****任務2** = $1,300.00 + - $400.00\
   **EAC費用****任務2** = $900.00

   **EAC****任務2** = EAC人工+ EAC費用\
   **EAC****任務2**  = $5,000.00 + $900.00\
   **EAC****任務2**  = $5,900.00

1. 任務4、5和6的CPI/EAC是以相同的方式確定的，因此我將提供以下值：\
   任務4:.23 / 3,400.00美元\
   任務5:.64 / 3,100.00美元\
   任務6:1.06美元/2,366.67美元

1. 任務3的CPI = .31，計算如下：\
   **CPI****任務3** = *若* 實際人工成本+已發生實際費用成本&lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **CPI****任務3**  =(1,150 + 500)/(3000 + 2400)\
   **CPI****任務3**  = 1650 / 5400\
   **CPI****任務3**  = .31 ******&#x200B;任務3的EAC **= $9,521.74計算方式如下：\
   **CPI勞工&#x200B;****任務3** =實際人工成本&lt;> 0，則

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **CPI勞工****任務3** = 1150/3000\
   **CPI勞工****任務3** = .383333\
   **CPI勞工****任務3** = .38

   **EAC人工****任務3** = *若* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* EAC人工=計畫人工成本+實際人工成本\
   **EAC人工****任務3** = $2,500.00 / .383333\
   **EAC人工****任務3** = $6,521.74

   **EAC費用****任務3** = ExcuredActualExpenseCost + NotExcuredPlannedExpense\
   **EAC費用****任務3** = $2,400.00 + $600.00\
   **EAC費用****任務3** = $3,000.00

   **EAC****任務3** = EAC人工+ EAC費用\
   **EAC****任務3**  = $6,521.74 + $3,000.00\
   **EAC****任務3**  = $9,521.74

1. 任務1的CPI = .16，計算如下：\
   **CPI****任務1** = *若* 實際人工成本+已發生實際費用成本&lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **CPI****任務1**  =(1250 + 300)/(5000 + 4500)\
   **CPI****任務1**  = 1550 / 9500=\
   **CPI****任務1**  = .16

1. 任務1的EAC為$17,100.00，計算如下：\
   **CPI勞工****任務1** =如果實際人工成本&lt;> 0，則

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **CPI勞工****任務1** = 1250 / 5000\
   **CPI勞工****任務1** = .25

   **EAC人工****任務1** = *若* CPI_Labor &lt;> 0 *THEN* EAC人工=計畫人工成本/CPI_人工\
   *   ELSE* EAC人工=計畫人工成本+實際人工成本\
   **EAC人工****任務1** = $3,000.00 / .25\
   **EAC人工****任務1** = $12,000.00

   **EAC費用****任務1** = ExcuredActualExpenseCost + NotExcuredPlannedExpense\
   **EAC費用****任務1** = $4500 + 600\
   **EAC費用****任務1** = $5,100.00

   **EAC****任務1** = EAC人工+ EAC費用\
   **EAC****任務1**  = $12,000.00 + 5,100.00\
   **EAC****任務1**  = $17,100.00

1. 項目的CPI為0.25\
   **項目的CPI****** = *若* 實際人工成本+已發生實際費用成本&lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor

   **項目的CPI****** =(2450 + 1900)/(11000 + 6700)\
   **項目的CPI****** = 4350 / 17700\
   **項目的CPI****** = .25

1. **專案的EAC** = $32,248.98，計算如下：\
   **CPI Labor**** for Project** =如果實際人工成本&lt;> 0，則

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **CPI Labor**** for Project** = 2450 / 11000\
   **CPI Labor**** for Project** = .22272\
   **CPI Labor**** for Project** = .22

   **EAC項目人工****** = *若* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* EAC人工=計畫人工成本+實際人工成本\
   **EAC項目人工****** = $5,000.00 / .22272\
   **EAC項目人工****** = $22,448.97959\
   **EAC項目人工****** = $22,448.98

   **EAC費用****項目** = ExcuredActualExpenseCost + NotExcuredPlannedExpense\
   **EAC費用****項目** = $3,100.00 + $6,700.00\
   **EAC費用****項目** = $9,800.00

   **EAC****項目** = EAC人工+ EAC費用\
   **EAC****項目**  = $22,448.98 + 9,800.00\
   **EAC****項目**  = $32,248.98
