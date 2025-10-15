---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: 計算範例 — 從任務累加計算EAC
description: 本文提供計算專案預估完成時間(EAC)的範例，說明如何從Adobe Workfront中專案的所有任務進行統計。
author: Lisa
feature: Work Management
exl-id: 68b582c9-f72a-4000-9d28-f7dafa23541f
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '1134'
ht-degree: 2%

---

# 計算範例 — 從任務累加計算EAC

## EAC方法：從任務或子任務彙總

* [PIM=以小時為基礎](#pim-hour-based)
* [PIM=基於成本](#pim-cost-based)

### PIM=以小時為基礎 {#pim-hour-based}

* [簡單範例：專案沒有子系任務](#simple-example-project-has-no-children-tasks)
* [複雜的範例：專案具有子系任務](#complicated-example-project-has-children-tasks)

#### 簡單範例：專案沒有子系任務 {#simple-example-project-has-no-children-tasks}

PIM =以小時為基礎

EAC方法=從任務/子任務彙總

1. 建立專案A，其中三個任務（無子系任務）全部指派給成本/小時為$100.00的使用者1。
1. 根據下表將計畫/實際時數新增至每個任務，並指定完成百分比：

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
1. 工作1 **的** CPI = .04計算方式如下：\
   任務1 **的** CPI = *IF*&#x200B;實際時數> 0 *然後* CPI = TotalBudgetedCostWorkPerformed/實際時數\
       *ELSE* CPI = 1\
   任務1 **的** CPI = 1 / 25\
   工作1 **的** CPI = .04

1. 任務1 **的** EAC = 125小時計算如下：\
   **工作1**&#x200B;的EAC = *IF* CPI &lt;> 0 *則* EAC =計畫時數/ CPI\
       *ELSE*

   ```
   EAC = Planned  Hours + Actual  Hours
   ```

   任務1 **的** EAC = 5 / .04\
   任務1 **的** EAC = 125小時

1. 任務2和3的CPI / EAC為：\
   任務  2 = .12 / 83.33  小時\
   工作3 = .24 / 62.5小時

1. 專案的&#x200B;**CPI** = .13，計算方式如下：\
   專案的&#x200B;**CPI** = *IF*&#x200B;實際時數> 0 *然後*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1\
   專案的&#x200B;**CPI** = 10 / 75\
   專案的&#x200B;**CPI** = .13

1. 專案的&#x200B;**EAC** = 270.83小時，計算方式如下\
   專案的&#x200B;**EAC** = EAC任務1 + EAC任務2 + EAC任務3\
   專案的&#x200B;**EAC** = 125 + 83.33 + 62.5\
   專案的&#x200B;**EAC** = 270.83小時

#### 複雜的範例：專案具有子系任務 {#complicated-example-project-has-children-tasks}

PIM =以小時為基礎

EAC方法=從任務/子任務彙總

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

1. 將50小時直接新增至專案（「更多>小時>記錄小時」），以便有$5,000.00的實際勞力成本直接記錄至專案。
1. 執行重新計算財務
1. 工作2 **的** CPI = .1計算方式如下：\
   工作2 **的** CPI = *IF*&#x200B;實際時數> 0 *然後*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1\
   任務2 **的** CPI = 1 / 10\
   工作2 **的** CPI = .1

1. 任務2 **的** EAC = 50小時計算如下：\
   任務2 **的** EAC = *IF* CPI &lt;> 0 *則*

   ```
   EAC = Planned Hours / CPI
   ```

       *ELSE* EAC =計畫  小時+實際  小時\
   任務2 **的** EAC = 5 / .1\
   任務2 **的** EAC = 50小時

1. 工作4、工作5和工作6的CPI / EAC：\
   任務4 = .4 / 25小時\
   任務5 = .75 / 20小時\
   工作6 = 1.2 / 16.67小時

1. 工作3 **的** CPI = .38\
   工作3 **的** CPI = *IF*&#x200B;實際時數> 0 *然後*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1\
   工作3 **的** CPI = 11.5 / 30\
   工作3 **的** CPI = .38

1. 任務3的&#x200B;**EAC** = EAC任務4 + EAC任務5\
   任務3 **的** EAC = 25 + 20\
   工作3 **的** EAC = 45小時

1. 工作1 **的** CPI = .25計算方式如下：\
   工作1 **的** CPI = *IF*&#x200B;實際時數> 0 *然後*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1\
   任務1 **的** CPI = 12.5 / 50\
   工作1 **的** CPI = .25

1. **工作1**&#x200B;的EAC = EAC工作2 + EAC工作3\
   任務1 **的** EAC = 50 + 45\
   任務1 **的** EAC = 95小時

1. 專案的CPI = .22，計算方式如下：\
   專案的&#x200B;**CPI** = *IF*&#x200B;實際時數> 0 *然後*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1\
   專案的&#x200B;**CPI** = 24.5 / 110\
   專案的&#x200B;**CPI** = .22272\
   專案的&#x200B;**CPI** = .22

1. 專案的&#x200B;**EAC** = EAC任務1 + EAC任務6\
   專案的&#x200B;**EAC** = 95 + 16.67\
   專案的&#x200B;**EAC** = 111.67小時

### PIM=基於成本 {#pim-cost-based}

* [簡單範例：專案沒有子系任務](#simple-example-project-has-no-children-tasks)

#### 簡單範例：專案沒有子系任務 {#simple-example-project-has-no-children-tasks-1}

PIM =以成本為基礎

EAC方法=從任務/子任務彙總

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
   <td> <p>$2,700.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 從專案動作，執行重新計算財務
1. 工作1 **的** CPI&#x200B;**&#x200B;** = .14計算方式如下：\
   工作1 **&#x200B;**&#x200B;**&#x200B;** CPI  = *IF*&#x200B;實際勞力成本+ GeneratedActualExpenseCost  &lt;> 0 *然後*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   工作1 **&#x200B;**&#x200B;**&#x200B;** CPI  = (100+300) / (2500+400)\
   工作1 **&#x200B;**&#x200B;**&#x200B;** CPI  = 400 / 2900\
   工作1 **&#x200B;**&#x200B;**&#x200B;** CPI  = .14

1. 任務1 **的** EAC&#x200B;**&#x200B;** = $13,400.00\
   任務1 **的** CPI勞力&#x200B;**&#x200B;** =如果實際勞力成本&lt;> 0，則

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      否則CPI_Labor = 1\
   **工作1**&#x200B;**1&rbrace;的CPI人工= 100/2500**\
   **工作1**&#x200B;**1&rbrace;的CPI人力= .04**

   **工作1**&#x200B;的EAC人力&#x200B;**&#x200B;** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* EAC  勞力=計畫勞力成本+實際勞力成本\
   **工作1**&#x200B;的EAC工&#x200B;**&#x200B;**= 500.00/.04\
   **工作1**&#x200B;的EAC工&#x200B;**&#x200B;**= $12,500.00

   **任務1**&#x200B;的EAC費用&#x200B;**&#x200B;** = GeneratedActualExpenseCost + NotGeneratedPlannedExpense\
   **任務1**&#x200B;的EAC費用&#x200B;**&#x200B;** = $400.00 + $500.00\
   **任務1**&#x200B;的EAC費用&#x200B;**&#x200B;** = $900.00

   **任務1**&#x200B;的EAC&#x200B;**&#x200B;** = EAC人力+ EAC費用\
   任務1 **的** EAC&#x200B;**&#x200B;**  = $12,500.00 + $900.00\
   任務1 **的** EAC&#x200B;**&#x200B;**  = $13,400.00

1. 以下是任務2和任務3的CPI / EAC值：\
   任務2 = .19 / $8,433.33\
   作業3 = .44 / $6,950.00&#x200B;**&#x200B;**

1. 專案的CPI = .32\
   專案的&#x200B;**CPI**&#x200B;**1&rbrace; =** IF *實際勞力成本+ GeneratedActualExpenseCost  &lt;> 0*&#x200B;然後&#x200B;**

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   專案的&#x200B;**CPI**&#x200B;**&#x200B;** = (1000 + 2300) / (7500 + 2700)\
   專案的&#x200B;**CPI**&#x200B;**&#x200B;** = 3300 / 10200\
   專案的&#x200B;**CPI**&#x200B;**1&rbrace; = .32**

1. 專案的EAC為$28,783.33美元\
   專案的&#x200B;**EAC**&#x200B;**&#x200B;** = EAC任務1 + EAC任務2 + EAC任務3\
   專案的&#x200B;**EAC**&#x200B;**&#x200B;** = $13,400.00 + $8,433.33 + $6,950.00\
   專案的&#x200B;**EAC**&#x200B;**&#x200B;** = $28,783.33
