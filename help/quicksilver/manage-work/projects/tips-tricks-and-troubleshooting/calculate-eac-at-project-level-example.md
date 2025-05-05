---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: 計算範例 — 在專案層級計算EAC
description: PIM =以小時為基礎
author: Alina
feature: Work Management
exl-id: ff88b7e3-2a5b-464f-bed1-6848067840b8
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '2194'
ht-degree: 0%

---

# 計算範例 — 在專案層級計算EAC

## EAC方法：在專案層級計算

* [PIM =以小時為基礎](#pim-hour-based)
* [PIM=基於成本](#pim-cost-based)

### PIM =以小時為基礎 {#pim-hour-based}

* [簡單範例：專案沒有子系任務](#simple-example-project-has-no-children-tasks)
* [複雜的範例：專案具有子系任務](#complicated-example-project-has-children-tasks)

#### 簡單範例：專案沒有子系任務 {#simple-example-project-has-no-children-tasks}

PIM =以小時為基礎

EAC方法=在專案層級計算&#x200B;**&#x200B;**

1. 建立專案A，其中三個任務（無子系任務）全部指派給成本/小時為$100.00的使用者1。
1. 根據下表將計畫和實際時數新增至每個任務並完成百分比：

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

1. 重新計算專案的財務。
1. 工作1 **的** CPI = .04計算方式如下：\
   任務1 **的** CPI = *IF*&#x200B;實際時數> 0 *然後* CPI = TotalBudgetedCostWorkPerformed/實際時數\
      *ELSE* CPI = 1\
   任務1 **的** CPI = 1 / 25\
   工作1 **的** CPI = .04

1. 任務1 **的** EAC = 125小時計算如下：\
   **工作1**&#x200B;的EAC = *IF* CPI &lt;> 0 *則* EAC =計畫時數/CPI\
       *ELSE* EAC =計畫  小時+實際  小時\
   任務1 **的** EAC = 5 / .04\
   任務1 **的** EAC = 125小時&#x200B;**&#x200B;**

1. 任務2和3的CPI / EAC為：\
   任務  2 = .12 / 83.33  小時\
   工作3 = .24 / 62.5小時

1. 專案的&#x200B;**CPI** = .13，計算方式如下：\
   專案的&#x200B;**CPI** = *IF*&#x200B;實際時數> 0 *然後* CPI = TotalBudgetedCostWorkPerformed/實際時數\
       *ELSE* CPI = 1\
   專案的&#x200B;**CPI** = 10 / 75\
   專案的&#x200B;**CPI** = .13

1. 專案的&#x200B;**EAC** = 225小時計算如下：\
   專案的&#x200B;**EAC** = *IF* CPI &lt;> 0 *則* EAC =計畫時數/CPI\
       *ELSE* EAC =計畫  小時+實際  小時\
   專案的&#x200B;**EAC** = 30 / .13333\
   專案的&#x200B;**EAC** = 225小時

#### 複雜的範例：專案具有子系任務 {#complicated-example-project-has-children-tasks}

PIM =以小時為基礎

EAC方法=在專案層級計算

1. 建立具有六個任務的專案A，其中任務3是任務4和5的父系，任務1是任務2和3的父系，如下所示：\
   任務1\
      任務2\
      任務3\
         任務4\
         任務5\
   任務6

1. 將作業2、4、5和6指定給成本/小時費率為$100.00的使用者1。
1. 根據下表新增每個任務的計畫/實際時數及完成百分比。

   >[!NOTE]
   >
   >對於任務1和3，您僅新增實際時數。

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
   <th> <p>完成<strong>%</strong> </p> </th> 
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

1. 直接新增50小時至專案（更多>小時>記錄小時）。
1. 工作2 **的** CPI = .1計算方式如下：\
   任務2 **的** CPI = *IF*&#x200B;實際時數> 0 *然後* CPI = TotalBudgetedCostWorkPerformed/實際時數\
       *ELSE* CPI = 1\
   任務2 **的** CPI = 1 / 10\
   工作2 **的** CPI = .1

1. 任務2 **的** EAC = 50小時計算如下：\
   **工作2**&#x200B;的EAC = *IF* CPI &lt;> 0 *則* EAC =計畫時數/CPI\
       *ELSE* EAC =計畫  小時+實際  小時\
   任務2 **的** EAC = 5 / .1\
   任務2 **的** EAC = 50小時

1. 任務4、5和6的CPI / EAC如下：\
   工作4：.4 / 25小時\
   任務5：.75 / 20小時\
   工作6:1.2 / 16.67小時

1. 工作3 **的** CPI = .38  計算方式如下：\
   任務3 **的** CPI = *IF*&#x200B;實際時數> 0 *然後* CPI = TotalBudgetedCostWorkPerformed/實際時數\
       *ELSE* CPI = 1\
   工作3 **的** CPI = 11.5 / 30\
   工作3 **的** CPI = .38

1. 工作3 **的** EAC = 65.22小時，計算方式如下：\
   **工作3**&#x200B;的EAC = *IF* CPI &lt;> 0 *則* EAC =計畫時數/CPI\
       *ELSE* EAC =計畫  小時+實際  小時\
   工作3 **的** EAC =  25 / .383333\
   任務3 **的** EAC = 65.22小時

1. 工作1 **的** CPI = .25計算方式如下：\
   任務1 **的** CPI = *IF*&#x200B;實際時數> 0 *然後* CPI = TotalBudgetedCostWorkPerformed/實際時數\
       *ELSE* CPI = 1\
   任務1 **的** CPI = 12.5 / 50\
   工作1 **的** CPI = .25

1. 任務1 **的** EAC = 120小時計算如下：\
   **工作1**&#x200B;的EAC = *IF* CPI &lt;> 0 *則* EAC =計畫時數/ CPI\
       *ELSE* EAC =計畫  小時+實際  小時\
   任務1 **的** EAC =  30/ .25\
   任務1 **的** EAC = 120小時

1. 專案的&#x200B;**CPI** = .22，計算方式如下：\
   專案的&#x200B;**CPI** = *IF*&#x200B;實際時數> 0 *然後* CPI = TotalBudgetedCostWorkPerformed/實際時數\
       *ELSE* CPI = 1\
   專案的&#x200B;**CPI** = 24.5 / 110\
   專案的&#x200B;**CPI** = .22272\
   專案的&#x200B;**CPI** = .22

1. 專案的&#x200B;**EAC** = 224.49  時數計算如下：\
   專案的&#x200B;**EAC** = *IF* CPI &lt;> 0 *則* EAC =計畫時數/CPI\
       *ELSE* EAC =計畫  小時+實際  小時\
   專案的&#x200B;**EAC** =  50 / .22272\
   專案的&#x200B;**EAC** = 224.49小時

### PIM=基於成本 {#pim-cost-based}

* [簡單範例：專案沒有子系任務](#simple-example-project-has-no-children-tasks)
* [複雜的範例：專案具有子系任務](#complicated-example-project-has-children-tasks)

#### 簡單範例：專案沒有子系任務 {#simple-example-project-has-no-children-tasks-1}

PIM =以成本為基礎

EAC方法=在專案層級計算

1. 建立專案A，其中三個任務（無子系任務）全部指派給成本/小時為$100.00的使用者1。
1. 根據下表將計畫/實際時數新增至每個任務，並指定完成百分比：

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
   <th> <br> <p><strong>計畫勞力成本</strong> </p> </th> 
   <th> <br> <p><strong>實際小時</strong> </p> </th> 
   <th> <br> <p><strong>實際勞力成本</strong> </p> </th> 
   <th> <p>完成<strong>%</strong> </p> </th> 
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

1. 根據下表將費用新增至每項工作：

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
   <td> <p>任務1費用1</p> </td> 
   <td> <p>300.00美元</p> </td> 
   <td> <p>400.00美元</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務1</p> </td> 
   <td> <p>任務1費用2</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務2</p> </td> 
   <td> <p>任務2費用</p> </td> 
   <td> <p>200.00美元</p> </td> 
   <td> <p>$100.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務3</p> </td> 
   <td> <p>任務3費用</p> </td> 
   <td> <p>800.00美元</p> </td> 
   <td> <p>700.00美元</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 將兩個費用新增至專案（亦即未繫結至任務），如下所示：

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
   <td> <p>專案費用1</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>$1,500.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務1費用2</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 根據上述值，已產生/未產生成本之釐定如下：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>任務</strong> </p> </th> 
   <th> <p><strong>未發生計畫費用</strong> </p> </th> 
   <th> <p><strong>已發生計畫費用</strong> </p> </th> 
   <th> <p><strong>發生實際費用</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>任務1</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>300.00美元</p> </td> 
   <td> <p>400.00美元</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務2</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>200.00美元</p> </td> 
   <td> <p>$100.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務3</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>800.00美元</p> </td> 
   <td> <p>700.00美元</p> </td> 
  </tr> 
  <tr> 
   <td> <p>專案</p> </td> 
   <td> <p>$3,000.00</p> </td> 
   <td> <p>$2,300.00</p> </td> 
   <td> <p> $2,700.00 <strong></strong></p> </td> 
  </tr> 
 </tbody> 
</table>

1. 從專案動作，執行重新計算財務
1. 工作1 **的** CPI = .14
1. 工作1 **的** CPI&#x200B;**&#x200B;** = .14計算方式如下：\
   **CPI**  任務1 **的** = *IF*&#x200B;實際勞力成本+ GeneratedActualExpenseCost  &lt;> 0 *然後*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *    ELSE* CPI = CPI_Labor\
   任務1 **的** CPI&#x200B;**&#x200B;**= (100+300) / (2500+400)\
   **CPI**  任務1 **的** = 400 / 2900\
   **CPI**  工作1 **的**  = .14&#x200B;**&#x200B;**

1. 任務1 **的** EAC&#x200B;**&#x200B;** = $13,400.00\
   **CPI人力**  任務1 **的** =如果實際勞力成本&lt;> 0，則

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

      否則CPI_Labor = 1\
   **CPI人力**  任務1 **的** = 100/2500\
   **CPI人力**  任務1的&#x200B;**&#x200B;** = .04 **&#x200B;**&#x200B;**&#x200B; EAC人力&#x200B;**&#x200B;**任務1的&#x200B;**=*IF *CPI_Labor &lt;> 0*THEN *EAC人力=計畫勞力成本/CPI_Labor\
   *    ELSE* EAC  勞力=計畫勞力成本+實際勞力成本\
   **作業1的EAC人工&#x200B;**&#x200B;**&#x200B;** = 500.00/.04\
   **工作1**&#x200B;的EAC工&#x200B;**&#x200B;**= $12,500.00\
   **任務1**&#x200B;的EAC費用&#x200B;**&#x200B;** = GeneratedActualExpenseCost + NotGeneratedPlannedExpense\
   **任務1**&#x200B;的EAC費用&#x200B;**&#x200B;** = $400.00 + $500.00\
   **任務1**&#x200B;的EAC費用&#x200B;**&#x200B;** = $900.00\
   **任務1**&#x200B;的EAC&#x200B;**&#x200B;** = EAC人力+ EAC費用\
   任務1 **的** EAC&#x200B;**&#x200B;**  = $12,500.00 + $900.00\
   任務1 **的** EAC&#x200B;**&#x200B;**  = $13,400.00

1. 以下是任務2和任務3的CPI / EAC值：\
   任務2 = .19 / $8,433.33\
   作業3 = .44 / $6,950.00

1. 專案的&#x200B;**CPI** = .32，計算方式如下：\
   專案的&#x200B;**CPI**&#x200B;**1&rbrace; = *IF*實際勞力成本+ GeneratedActualExpenseCost  &lt;> 0 *然後***

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   專案的&#x200B;**CPI**&#x200B;**&#x200B;** = (1000 + 2300) / (7500 + 2700)\
   專案的&#x200B;**CPI**&#x200B;**&#x200B;** = 3300 / 10200\
   專案的&#x200B;**CPI**&#x200B;**1&rbrace; = .32**

1. 專案的&#x200B;**EAC** = $28,200.00，計算方式如下：\
   專案&#x200B;**的** CPI勞力&#x200B;**&#x200B;**=如果實際勞力成本&lt;> 0，則

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

      否則CPI_Labor = 1\
   專案的&#x200B;**CPI勞力**&#x200B;**&#x200B;** = 1000 / 7500\
   專案的&#x200B;**CPI工**&#x200B;**&#x200B;** = .13333\
   專案的&#x200B;**CPI工**&#x200B;**&#x200B;** = .13

   專案的&#x200B;**EAC人力**&#x200B;**1&rbrace; = *IF* CPI_Labor &lt;> 0 *THEN***

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   *   ELSE* EAC  勞力=計畫勞力成本+實際勞力成本\
   **專案**&#x200B;的EAC工&#x200B;**&#x200B;**= 3000/ .13333\
   **專案**&#x200B;**EAC勞力** = $22,500.00

   **EAC費用**&#x200B;**專案** =

   ```
   IncurredActualExpenseCost + NotIncurredPlannedExpense
   ```

   **EAC費用**&#x200B;**專案** = $3000.00 + 2,700.00\
   **EAC費用**&#x200B;**專案** = $5,700.00

   **EAC**&#x200B;**專案** = EAC人力+ EAC費用\
   **EAC**&#x200B;**專案**  = $22,500.00 + $5,700.00\
   **EAC**&#x200B;**專案**  = $28,200.00

#### 複雜的範例：專案具有子系任務 {#complicated-example-project-has-children-tasks-1}

PIM =以成本為基礎

EAC方法=在專案層級計算

1. 建立具有六個任務的專案A，其中任務3是任務4和5的父系，任務1是任務2和3的父系，如下所示：\
   任務1\
      任務2\
      任務3\
         任務4\
         任務5\
   任務6

1. 將作業2、4、5和6指定給成本/小時費率為$100.00的使用者1。
1. 根據下表新增每個任務的計畫/實際時數及完成百分比。

   >[!NOTE]
   >
   >對於任務1和3，您僅新增實際時數。

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
   <th> <br> <p><strong>計畫勞力成本</strong> </p> </th> 
   <th> <br> <p><strong>實際小時</strong> </p> </th> 
   <th> <br> <p><strong>實際勞力成本</strong> </p> </th> 
   <th> <p>完成<strong>%</strong> </p> </th> 
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

1. 將50小時直接新增至專案（「更多>小時>記錄小時」），以便有$5,000.00的實際勞力成本直接記錄至專案。 **&#x200B;**
1. 根據下表新增費用至每項工作（我已在每項工作之間新增空白列，讓讀者更容易閱讀）：

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
   <td> <p>任務1費用1</p> </td> 
   <td> <p>300.00美元</p> </td> 
   <td> <p>-$400.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務1</p> </td> 
   <td> <p>任務1費用2</p> </td> 
   <td> <p>-$500.00</p> </td> 
   <td> <p>800.00美元</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務1</p> </td> 
   <td> <p>任務1費用3</p> </td> 
   <td> <p>400.00美元</p> </td> 
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
   <td> <p>任務2費用1</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>700.00美元</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務2</p> </td> 
   <td> <p>任務2費用2</p> </td> 
   <td> <p>-$400.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務2</p> </td> 
   <td> <p>任務2費用3</p> </td> 
   <td> <p>-$200.00</p> </td> 
   <td> <p>$600.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務2</p> </td> 
   <td> <p>任務2費用4</p> </td> 
   <td> <p>700.00美元</p> </td> 
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
   <td> <p>任務3費用</p> </td> 
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
   <td> <p>任務4費用1</p> </td> 
   <td> <p>800.00美元</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務4</p> </td> 
   <td> <p>任務4費用2</p> </td> 
   <td> <p>-$100.00</p> </td> 
   <td> <p>300.00美元</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務4 </p> </td> 
   <td> <p>任務4費用3</p> </td> 
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
   <td> <p>任務5費用1</p> </td> 
   <td> <p>700.00美元</p> </td> 
   <td> <p>800.00美元</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務5</p> </td> 
   <td> <p>任務5費用2</p> </td> 
   <td> <p>-$100.00</p> </td> 
   <td> <p>300.00美元</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務5</p> </td> 
   <td> <p>任務5費用3</p> </td> 
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
   <td> <p>任務6費用1</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>700.00美元</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務6</p> </td> 
   <td> <p>任務6費用2</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>-$300.0</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 將兩個費用新增至專案（亦即未繫結至任務），如下所示：

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
   <td> <p>專案費用1</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>$1,500.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務1費用2</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p> $0.00 <strong></strong></p> </td> 
  </tr> 
 </tbody> 
</table>

1. 根據上述值，「產生/未產生」成本依下列方式釐定：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>任務</strong> </p> </th> 
   <th> <p><strong>未發生計畫費用</strong> </p> </th> 
   <th> <p><strong>已發生計畫費用</strong> </p> </th> 
   <th> <p><strong>發生實際費用</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>任務1</p> </td> 
   <td> <p>400.00美元</p> </td> 
   <td> <p>-$500.00</p> </td> 
   <td> <p>800.00美元</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務2</p> </td> 
   <td> <p>-$400.00</p> </td> 
   <td> <p>300.00美元</p> </td> 
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
   <td> <p>300.00美元</p> </td> 
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
   <td> <p>700.00美元</p> </td> 
  </tr> 
  <tr> 
   <td> <p>專案</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>$1000.00</p> </td> 
   <td> <p>$1,500.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 從專案動作，執行重新計算財務
1. 工作2的&#x200B;**CPI** = .17計算方式如下：\
   **CPI工作2** = *IF*&#x200B;實際勞力成本+ GeneratedActualExpenseCost  &lt;> 0 *THEN* CPI = (TotalBudgetedCostWorkPerformed + GeneratedPlannedExpenseCost) / (ActualLaborCost + GeneratedActualExpenseCost)\
   *   ELSE* CPI = CPI_Labor\
   **CPI**&#x200B;**任務2** = (100+300) / (1000+1300)\
   **CPI**&#x200B;**工作2**  = 400 / 2300\
   **CPI**&#x200B;**工作2**  = .17

1. 任務2的&#x200B;**EAC** = $5,900.00\
   **CPI勞力**&#x200B;**任務2** =如果實際勞力成本&lt;> 0，則CPI_勞力= TotalBudgetedCostWorkPerformed /實際勞力成本\
      否則CPI_Labor = 1\
   **CPI人工**&#x200B;**工作2** = 100/1000\
   **CPI人工**&#x200B;**工作2** = .1

   **EAC Labor**&#x200B;**Task 2** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   *   ELSE* EAC  勞力=計畫勞力成本+實際勞力成本\
   **EAC人工**&#x200B;**工作2** = 500.00/.1\
   **EAC人工**&#x200B;**工作2** = $5,000.00 **&#x200B;**&#x200B;**&#x200B; EAC費用&#x200B;**&#x200B;**工作2 &#x200B;**=已發生實際費用成本+ NotGeneratedPlannedExpense\
   **EAC費用&#x200B;**&#x200B;**工作2** = $1,300.00 + -$400.00\
   **EAC費用**&#x200B;**任務2** = $900.00

   **EAC**&#x200B;**任務2** = EAC人力+ EAC費用\
   **EAC**&#x200B;**任務2**  = $5,000.00 + $900.00\
   **EAC**&#x200B;**任務2**  = $5,900.00

1. 任務4、5和6的CPI/EAC也是以相同方式決定的，因此我只提供以下這些值：\
   作業4： .23 / $3,400.00\
   任務5： .64 / $3,100.00\
   工作6:1.06 / $2,366.67

1. 作業3的CPI = .31計算方式如下：\
   **CPI**&#x200B;**任務3** = *IF*&#x200B;實際勞力成本+ GeneratedActualExpenseCost  &lt;> 0 *然後*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **CPI**&#x200B;**工作3**  = (1,150 + 500) / (3000 + 2400)\
   **CPI**&#x200B;**工作3**  =  1650 / 5400\
   **CPI**&#x200B;**工作3**  = .31 **&#x200B;**&#x200B;**&#x200B;工作3 &#x200B;** 的EAC = $9,521.74計算如下：\
   **CPI人工&#x200B;**&#x200B;**作業3** =如果實際人工成本&lt;> 0，則

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      否則CPI_Labor = 1\
   **CPI人工**&#x200B;**工作3** = 1150/3000\
   **CPI人工**&#x200B;**工作3** = .383333\
   **CPI人工**&#x200B;**工作3** = .38

   **EAC Labor**&#x200B;**Task 3** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* EAC  勞力=計畫勞力成本+實際勞力成本\
   **EAC人工**&#x200B;**工作3** = $2,500.00 / .383333\
   **EAC人工**&#x200B;**工作3** = $6,521.74

   **EAC Expense**&#x200B;**Task 3** = GeneratedActualExpenseCost + NotGeneratedPlannedExpense\
   **EAC費用**&#x200B;**工作3** = $2,400.00 + $600.00\
   **EAC費用**&#x200B;**任務3** = $3,000.00

   **EAC**&#x200B;**任務3** = EAC人力+ EAC費用\
   **EAC**&#x200B;**任務3**  = $6,521.74 + $3,000.00\
   **EAC**&#x200B;**任務3**  = $9,521.74

1. 作業1的CPI = .16計算方式如下：\
   **CPI**&#x200B;**任務1** = *IF*&#x200B;實際勞力成本+ GeneratedActualExpenseCost  &lt;> 0 *然後*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **CPI**&#x200B;**任務1**  = (1250 + 300) / (5000 + 4500)\
   **CPI**&#x200B;**任務1**  =  1550 / 9500=\
   **CPI**&#x200B;**任務1**  = .16

1. 作業1的EAC為$17,100.00，計算方式如下：\
   **CPI勞力**&#x200B;**任務1** =如果實際勞力成本&lt;> 0，則

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      否則CPI_Labor = 1\
   **CPI人工**&#x200B;**工作1** = 1250 / 5000\
   **CPI人工**&#x200B;**工作1** = .25

   **EAC勞力**&#x200B;**工作1** = *IF* CPI_Labor &lt;> 0 *THEN* EAC勞力=計畫勞力成本/ CPI_Labor\
   *   ELSE* EAC  勞力=計畫勞力成本+實際勞力成本\
   **EAC人工**&#x200B;**工作1** = $3,000.00 / .25\
   **EAC人工**&#x200B;**工作1** = $12,000.00

   **EAC Expense**&#x200B;**任務1** = GeneratedActualExpenseCost + NotGeneratedPlannedExpense\
   **EAC費用**&#x200B;**任務1** = $4500 + 600\
   **EAC費用**&#x200B;**任務1** = $5,100.00

   **EAC**&#x200B;**任務1** = EAC人力+ EAC費用\
   **EAC**&#x200B;**任務1**  = $12,000.00 + 5,100.00\
   **EAC**&#x200B;**任務1**  = $17,100.00

1. 專案的CPI是。25\
   專案的&#x200B;**CPI**&#x200B;**1&rbrace; = *IF*實際勞力成本+ GeneratedActualExpenseCost  &lt;> 0 *然後***

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor

   專案的&#x200B;**CPI**&#x200B;**&#x200B;** = (2450 + 1900) / (11000 + 6700)\
   專案的&#x200B;**CPI**&#x200B;**&#x200B;** =   4350 / 17700\
   專案的&#x200B;**CPI**&#x200B;**1&rbrace; = .25**

1. 專案的&#x200B;**EAC** = $32,248.98計算如下：\
   專案&#x200B;**的** CPI勞力&#x200B;**&#x200B;**=如果實際勞力成本&lt;> 0，則

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      否則CPI_Labor = 1\
   **專案**&#x200B;**CPI勞力** = 2450 / 11000\
   專案的&#x200B;**CPI工**&#x200B;**&#x200B;** = .22272\
   專案的&#x200B;**CPI工**&#x200B;**&#x200B;** = .22

   專案的&#x200B;**EAC人力**&#x200B;**1&rbrace; = *IF* CPI_Labor &lt;> 0 *THEN***

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* EAC  勞力=計畫勞力成本+實際勞力成本\
   **專案**&#x200B;的EAC&#x200B;**&#x200B;**&#x200B;工費用= $5,000.00 / .22272\
   **專案**&#x200B;**EAC勞力** = $22,448.97959\
   **專案**&#x200B;**EAC勞力** = $22,448.98

   **EAC Expense**&#x200B;**專案** = GeneratedActualExpenseCost + NotGeneratedPlannedExpense\
   **EAC費用**&#x200B;**專案** = $3,100.00 + $6,700.00\
   **EAC費用**&#x200B;**專案** = $9,800.00

   **EAC**&#x200B;**專案** = EAC人力+ EAC費用\
   **EAC**&#x200B;**專案**  = $22,448.98 + 9,800.00\
   **EAC**&#x200B;**專案**  = $32,248.98
