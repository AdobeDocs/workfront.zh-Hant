---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 計算完工估算(EAC)
description: 作為效能量度，預估完成成本(EAC)代表專案或任務完成時的預估總成本。
author: Lisa
feature: Work Management
exl-id: 9061fa56-cff3-4fe2-866e-1fdda9d43efc
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
workflow-type: tm+mt
source-wordcount: '845'
ht-degree: 0%

---

# 計算完工估算(EAC)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link!) </p>
-->

作為效能量度，預估完成成本(EAC)代表專案或任務完成時的預估總成本。

做為設定，它可讓您定義EAC值的計算方式。 

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

## 定義如何計算EAC

作為專案系統偏好設定的一部分，Adobe Workfront管理員可以定義如何計算EAC。 EAC的計算方式為下列兩種方式之一：

* [在專案層級計算](#calculate-at-the-project-level)
* [從任務和子任務彙總](#roll-up-from-tasks-and-subtasks)

如需在Workfront中設定專案偏好設定的詳細資訊，包括如何計算預估完成值，請參閱[設定系統範圍的專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

身為專案經理，您也可以在專案的「財務」子標籤中，於專案層級變更此偏好設定。 如需有關編輯專案財務子標籤的詳細資訊，請參閱[管理專案財務區域](../../../manage-work/projects/project-finances/manage-project-finance-area.md)中的資訊。

### 在專案層級上計算 {#calculate-at-the-project-level}

在「EAC公式」中輸入實際時數/實際勞力成本，即可決定上階作業與專案的EAC。 此計算包括直接新增到父級任務或專案的實際時數/成本和費用。

### 從任務和子任務彙總 {#roll-up-from-tasks-and-subtasks}

父系任務和專案的EAC是由每個子系任務的EAC總和所決定。 此計算不包括直接新增到父級任務或專案的實際時數/成本和費用。

## 如何根據績效指數方法(PIM)計算EAC

在Workfront中，EAC的計算取決於專案的選取績效指數方法(PIM)。 如需有關為系統或專案設定PIM的詳細資訊，請參閱[設定績效指數方法(PIM)](../../../manage-work/projects/project-finances/set-pim.md)。

* [使用以小時為基礎的PIM計算EAC](#calculate-eac-using-hour-based-pim)
* [使用以成本為基礎的PIM計算EAC](#calculate-eac-using-cost-based-pim)

### 使用以小時為基礎的PIM計算EAC {#calculate-eac-using-hour-based-pim}

```
EAC = Total Planned Hours / CPI*
```

&#42;如果成本績效指數[計算成本績效指數(CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md) = 0，EAC =總計畫時數+實際時數。 當已擷取時數，但專案/任務已完成0%時，就會發生這種情況。

如需有關計算CPI的詳細資訊，請參閱[計算成本績效指數(CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md)。

### 使用以成本為基礎的PIM計算EAC {#calculate-eac-using-cost-based-pim}

專案的EAC使用下列公式計算：

```
EAC = EAC Labor + EAC Expense 
```

<pre>EAC人力=  <em>IF</em> CPI勞力&lt;&gt; 0 THEN EAC勞力=計畫勞力成本/ CPI勞力</pre><pre><em>ELSE</em> EAC  勞力=計畫勞力成本+實際勞力成本</pre><pre>CPI勞力=如果實際勞力成本&lt;&gt; 0，則CPI勞力=已執行預算成本總計/實際勞力成本</pre><pre>否則CPI人工= 1 </pre>計算EAC時，會考慮下列欄位：

* 總預算執行成本工作(BCWP) =將計畫工作的預算成本（預算成本）與目前已完成工作的百分比相乘的結果。

  如需執行的總預算成本工作(BCWP)的相關資訊，請參閱[計算執行的預算成本工作(BCWP)](../../../manage-work/projects/project-finances/calculate-bcwp.md)。

   * **針對非父系任務：**

     ```
     Total Budgeted Cost Work Performed = Planned Hours * (Percent Complete/100)
     ```

   * **對於父系任務：**
已執行預算成本工時總計=所有直接子任務之已執行預算成本工時總計欄位的總和。

   * 專案的&#x200B;**：**
已執行預算成本工時總計=所有最上層作業（父系與獨立作業）之已執行預算成本工時總計欄位的總和。 

* EAC費用=將已產生的實際費用成本新增至未產生的計畫費用成本的結果。 會透過下列公式計算：

  ```
  EAC Expense = Incurred Actual Expense Cost + Not Incurred Planned Expense
  ```

   * 已發生實際費用成本=所有費用的「計畫金額」欄位總和，其中「實際金額」欄位> 0。 例如，如果您為作業1建立費用，並在「計畫金額」欄位中輸入$500.00，並在「實際金額」欄位中輸入> 0金額（即$600.00），則此作業的「已發生計畫費用成本」為$500.00。
   * 未發生計畫費用=所有費用的「實際金額」欄位= 0的「計畫金額」欄位總和。 例如，如果您為任務1建立兩個費用，其中第一個費用的「計畫金額」欄位值為$500.00，而實際金額的值為$600.00，第二個費用的「計畫金額」欄位值為$300.00，而「實際金額」欄位的值為$0.00，則此任務的「未發生的計畫費用」值為$300.00。 

## 在專案或任務中找出EAC

1. 前往您要檢視EAC的專案或任務。
1. 根據您檢視EAC的位置，在專案或任務的左側面板中展開&#x200B;**專案詳細資料**&#x200B;或&#x200B;**任務詳細資料**。

1. 按一下&#x200B;**財務**。 

   EAC值會顯示在&#x200B;**預估完成時間**&#x200B;欄位中。

   ![](assets/eac-highlighted-on-project-350x112.png)
