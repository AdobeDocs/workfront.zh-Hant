---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 計算成本績效指數(CPI)
description: 成本績效指數(CPI)描述了計畫成本與實際成本之間在項目或任務層的關係。 項目經理複查此度量，以確定當前在指定時間按或超出成本跟蹤的任務或項目。
author: Alina
feature: Work Management
exl-id: 7f2efe26-7292-482d-986c-2d2077a7ca52
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '635'
ht-degree: 0%

---

# 計算成本績效指數(CPI)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.)</p>
-->

成本績效指數(CPI)描述了計畫成本與實際成本之間在項目或任務層的關係。 項目經理複查此度量，以確定當前在指定時間按或超出成本跟蹤的任務或項目。 成本可以按小時或美元計算，具體取決於您的效能索引方法(PIM)。 有關設定效能索引方法的詳細資訊，請參見 [設定效能索引方法(PIM)](../../../manage-work/projects/project-finances/set-pim.md).

只有需要時間輸入的組織才能使用CPI。 此外，基於成本的PIM值僅在具有為任務分配者（任務角色或用戶）定義成本率的組織中準確。

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
   <td> <p>查看對項目和財務資料的訪問</p> <p> 如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>查看項目或具有查看財務權限的項目的更高權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 成本績效指數(CPI)概覽

* [CPI值](#the-cpi-value)
* [如何計算CPI](#how-cpi-is-calculated)

### CPI值 {#the-cpi-value}

項目經理們明白，CPI值為1表示項目完全處於預算狀態。 值大於1表示項目處於預算之下（記錄的小時數或費用少於原計畫），值小於1表示項目超出預算（記錄的小時數或費用比原計畫的要多）。 距1越遠，與計畫的偏差越大。

| **CPI值** | **預算指示** |
|---|---|
| 1 | 計畫或預算 |
| > 1（大於1） | 預算不足 |
| &lt; 1（小於1） | 超預算 |


### 如何計算CPI {#how-cpi-is-calculated}

在Adobe Workfront中，CPI的計算取決於為專案選取的效能指數方法。 有關設定效能索引方法的詳細資訊，請參見 [設定效能索引方法(PIM)](../../../manage-work/projects/project-finances/set-pim.md).

* [使用小時型PIM時的CPI計算](#cpi-calculations-when-using-hour-based-pim)
* [使用基於成本的PIM時的CPI計算](#cpi-calculations-when-using-cost-based-pim)

#### 使用小時型PIM時的CPI計算 {#cpi-calculations-when-using-hour-based-pim}

如果

```
Actual Hours > 0 THEN CPI = Total Budgeted Cost Work Performed / Actual Hours
```

否則

```
CPI = 1
```

* **對於非父任務：**

   ```
   Total Budgeted Cost Work Performed = Planned Hours * (Percent Complete / 100)
   ```

* **對於父任務：**
執行的總預算成本工作=所有直接子任務的「已執行總預算成本工作」欄位的總和。

* **專案：**
執行的總預算成本工作=所有頂層任務（父任務和獨立任務）的「執行的總預算成本工作」欄位的總和。

有關已執行的總預算成本工作(BCWP)的資訊，請參閱 [計算已執行的預算成本工作(BCWP)](../../../manage-work/projects/project-finances/calculate-bcwp.md).

#### 使用基於成本的PIM時的CPI計算 {#cpi-calculations-when-using-cost-based-pim}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>CPI = (Planned Cost of Work Performed + Planned Cost of Incurred Expenses) / (Total Actual Cost + Actual Cost of Incurred Expenses) </code> </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>NOTE: this used to be here before - above - but Anna sent me the one below. I kept the other one, although she is still researching its validity - see this issue: https://hub.workfront.com/issue/5fc7b1cf00012aeebf9e822db8ea2513/overview)</code> </p>
-->

如果

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

此計算中的欄位如下所述：

```
Total Actual Cost = Actual (logged) Hours * Hourly Rate of assignees
```

```
Incurred Actual Expense Cost = Actual Cost
```

已發生費用是實際成本> 0的費用

```
Planned Cost of Incurred Expenses = Total of Planned Cost of all incurred expenses
```



<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Old calculation - taken out by Lilit and replaced below: Planned Cost of Work Performed= (planned labor cost) * (percent complete) / 100 where planned labor cost is the planned hours allocated to assignees * their rates.)</p>
  -->

* 已執行的計畫成本按以下公式計算：

   ```
   Planned Cost of Work Performed = Planned cost * Percent Complete / 100
   ```

執行的總預算成本工作計算如下：

* **對於非父任務：**

   ```
   Total Budgeted Cost Work Performed = Planned Labor Cost * Percent Complete / 100
   ```

* **對於父任務：**

   ```
   Total Budgeted Cost Work Performed = SUM(Total Budgeted Cost Work Performed field from all direct child tasks)
   ```

* **專案：**

   ```
   Total Budgeted Cost Work Performed = SUM(Total Budgeted Cost Work Performed field for all top level tasks)
   ```



## 在項目或任務中查找CPI

您可以在項目或任務清單或報表中顯示項目或任務的CPI。 此外，您也可以在專案或任務層級檢視。

1. 轉到要查看CPI的項目或任務。
1. 展開 **專案詳細資料** 或 **任務詳細資訊** 在左側面板中，根據您是查看項目還是任務的CPI。

1. 按一下 **金融**.

   CPI會顯示在 **CPI/SPI/CSI** 欄位。

   ![](assets/cpi-on-project-nwe.png)
