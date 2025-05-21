---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 計算成本績效指數(CPI)
description: 成本績效指數(CPI)說明專案或作業層次的計畫成本與實際成本之間的關係。 專案經理會檢閱此量度，以識別目前於指定時間點追蹤成本過低或過高的任務或專案。
author: Lisa
feature: Work Management
exl-id: 7f2efe26-7292-482d-986c-2d2077a7ca52
source-git-commit: a411c1ddf0c6d19dc7f6e181cceeebba5504530c
workflow-type: tm+mt
source-wordcount: '606'
ht-degree: 0%

---

# 計算成本績效指數(CPI)

<!-- Audited: 5/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.)</p>
-->

成本績效指數(CPI)說明專案或作業層次的計畫成本與實際成本之間的關係。 專案經理會檢閱此量度，以識別目前於指定時間點追蹤成本過低或過高的任務或專案。 視您的績效指數方法(PIM)而定，成本可以用小時或美元來衡量。 如需有關設定績效指數方法的詳細資訊，請參閱[設定績效指數方法(PIM)](../../../manage-work/projects/project-finances/set-pim.md)。

只有需要輸入時間的組織才能使用CPI。 此外，以成本為基礎的PIM值只有在已定義作業受指派人（職務角色或使用者）的成本比率的組織中才正確。

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
   <p>新增：淺色或更高</p>
   <p>或</p>
   <p>目前：檢閱或以上</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td>檢視專案與財務資料的存取權</td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td>檢視專案或更高許可權，並具有檢視財務的許可權</td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 成本績效指數(CPI)概要

### CPI值 {#the-cpi-value}

專案經理瞭解CPI值為1表示專案完全符合預算。 大於1的值表示專案在預算內（記錄的時數或費用少於最初計畫），而小於1的值表示專案超出預算（記錄的時數或費用多於最初計畫）。 從1越遠，與計畫的偏差越大。

| **CPI值** | 預算&#x200B;**上的**&#x200B;指示 |
|---|---|
| 1 | 在計畫或預算內 |
| > 1 （大於1） | 低於預算 |
| &lt; 1 （小於1） | 超出預算 |


### CPI的計算方式 {#how-cpi-is-calculated}

在Adobe Workfront中，CPI的計算取決於為專案選取的績效指數方法。 如需有關設定績效指數方法的詳細資訊，請參閱[設定績效指數方法(PIM)](../../../manage-work/projects/project-finances/set-pim.md)。

* 使用以小時為基礎的PIM時進行[CPI計算](#cpi-calculations-when-using-hour-based-pim)
* [使用成本型PIM時的CPI計算](#cpi-calculations-when-using-cost-based-pim)

#### 使用以小時為基礎的PIM時的CPI計算 {#cpi-calculations-when-using-hour-based-pim}

若

```
Actual Hours > 0 THEN CPI = Total Budgeted Cost Work Performed / Actual Hours
```

否則

```
CPI = 1
```

* **針對非父系任務：**

  ```
  Total Budgeted Cost Work Performed = Planned Hours * (Percent Complete / 100)
  ```

* **對於父系任務：**
已執行預算成本工時總計=所有直接子任務之已執行預算成本工時總計欄位的總和。

* 專案的&#x200B;**：**
已執行預算成本工時總計=所有最上層作業（父系與獨立作業）之已執行預算成本工時總計欄位的總和。

如需執行的總預算成本工作(BCWP)的相關資訊，請參閱[計算執行的預算成本工作(BCWP)](../../../manage-work/projects/project-finances/calculate-bcwp.md)。

#### 使用成本型PIM時的CPI計算 {#cpi-calculations-when-using-cost-based-pim}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>CPI = (Planned Cost of Work Performed + Planned Cost of Incurred Expenses) / (Total Actual Cost + Actual Cost of Incurred Expenses) </code> </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>NOTE: this used to be here before - above - but Anna sent me the one below. I kept the other one, although she is still researching its validity - see this issue: https://hub.workfront.com/issue/5fc7b1cf00012aeebf9e822db8ea2513/overview)</code> </p>
-->

若

```
Actual Labor Cost + Incurred Actual Expense Cost <> 0 THEN CPI = (Total Budgeted Cost Work Performed + Incurred Planned Expense Cost) / (Actual Labor Cost + Incurred Actual Expense Cost)
```



否則

```
CPI = 1
```

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>(NOTE: above: this used to say: CPI = CPI Labor, but Anna had me fix it on July 21, 2021)</code> </p>
-->

此計算中的欄位說明如下：

```
Total Actual Cost = Actual (logged) Hours * Hourly Rate of assignees
```

```
Incurred Actual Expense Cost = Actual Cost
```

發生費用是實際成本> 0的費用

```
Planned Cost of Incurred Expenses = Total of Planned Cost of all incurred expenses
```



<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Old calculation - taken out by Lilit and replaced below: Planned Cost of Work Performed= (planned labor cost) * (percent complete) / 100 where planned labor cost is the planned hours allocated to assignees * their rates.)</p>
  -->

* 已執行工作之計畫成本的計算公式如下：

  ```
  Planned Cost of Work Performed = Planned cost * Percent Complete / 100
  ```

已執行的總預算成本工作針對下列專案計算：

* **針對非父系任務：**

  ```
  Total Budgeted Cost Work Performed = Planned Labor Cost * Percent Complete / 100
  ```

* **對於父系任務：**

  ```
  Total Budgeted Cost Work Performed = SUM(Total Budgeted Cost Work Performed field from all direct child tasks)
  ```

* 專案的&#x200B;**：**

  ```
  Total Budgeted Cost Work Performed = SUM(Total Budgeted Cost Work Performed field for all top-level tasks)
  ```



## 在專案或任務中尋找CPI

您可以在專案、任務清單或報告中顯示專案或任務的CPI。 此外，您還可以在專案或任務層級檢視它。

1. 前往您要檢視CPI的專案或任務。
1. 展開左側面板中的&#x200B;**專案詳細資料**&#x200B;或&#x200B;**任務詳細資料**，具體取決於您檢視的是專案還是任務的CPI。

1. 按一下&#x200B;**財務**。 CPI顯示在&#x200B;**CPI/ SPI/ CSI**&#x200B;欄位中。

   專案![&#128279;](assets/cpi-on-project-nwe.png)上的CPI
