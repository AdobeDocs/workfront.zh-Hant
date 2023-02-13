---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 完成時計算估計值(EAC)
description: 作為績效度量，完成時估計(EAC)表示項目或任務完成時的預計總成本。
author: Alina
feature: Work Management
exl-id: 9061fa56-cff3-4fe2-866e-1fdda9d43efc
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '861'
ht-degree: 0%

---

# 完成時計算估計值(EAC)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link!) </p>
-->

作為績效度量，完成時估計(EAC)表示項目或任務完成時的預計總成本。

作為設定，它可讓您定義EAC值的計算方式。 

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
   <td> <p>查看對項目和財務資料的訪問</p> <p><b>附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>查看項目或具有查看財務權限的項目的更高權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 定義EAC的計算方式

作為項目系統首選項的一部分，Adobe Workfront管理員可以定義如何計算EAC。 EAC可透過下列兩種方式之一計算：

* [在專案層級計算](#calculate-at-the-project-level)
* [從任務和子任務匯總](#roll-up-from-tasks-and-subtasks)

如需在Workfront中設定專案偏好設定的詳細資訊，包括如何在完成時計算預估，請參閱 [配置系統範圍的項目首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

作為項目經理，您還可以在項目層的「財務」子頁簽中更改此首選項。 有關編輯項目的「財務」子頁簽的詳細資訊，請參見 [管理項目財務區域中的資訊](../../../manage-work/projects/project-finances/manage-project-finance-area.md).

### 在專案層級計算 {#calculate-at-the-project-level}

父任務和項目的EAC通過在EAC公式中輸入實際小時數/實際人工成本來確定。 此計算包括直接添加到父任務或項目的實際小時數/成本和費用。

### 從任務和子任務匯總 {#roll-up-from-tasks-and-subtasks}

父任務和項目的EAC通過加總每個子任務的EAC來確定。 此計算不包括直接添加到父任務或項目的實際小時數/成本和費用。

## 基於效能指數法的EAC計算

在Workfront中，EAC的計算取決於所選項目的效能索引方法(PIM)。 有關為系統或項目設定PIM的詳細資訊，請參見 [設定效能索引方法(PIM)](../../../manage-work/projects/project-finances/set-pim.md).

* [使用基於小時的PIM計算EAC](#calculate-eac-using-hour-based-pim)
* [使用基於成本的PIM計算EAC](#calculate-eac-using-cost-based-pim)

### 使用基於小時的PIM計算EAC {#calculate-eac-using-hour-based-pim}

```
EAC = Total Planned Hours / CPI*
```

&#42;如果成本效能指數 [計算成本績效指數(CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md) = 0,EAC =總計畫小時數+實際小時數。 當已捕獲小時，但項目/任務已完成0%時，就會發生此情況。

有關計算CPI的詳細資訊，請參見 [計算成本績效指數(CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md).

### 使用基於成本的PIM計算EAC {#calculate-eac-using-cost-based-pim}

項目的EAC使用以下公式計算：

```
EAC = EAC Labor + EAC Expense 
```

<pre>EAC勞動力=  <em>若</em> CPI人工&lt;&gt; 0然後EAC人工=計畫人工成本/CPI人工</pre><pre><em>ELSE</em> EAC人工=計畫人工成本+實際人工成本</pre><pre>CPI人工= IF實際人工成本&lt;&gt; 0,CPI人工= TotalBudgetedCostWorkPerformed /實際人工成本</pre><pre>ELSE CPI勞動率= 1 </pre>計算EAC時會考慮下列欄位：

* 已執行的總預算成本工作(BCWP)=已計畫工作的預算成本（預算成本）與迄今已完成任務的百分比相乘的結果。

   有關已執行的總預算成本工作(BCWP)的資訊，請參閱 [計算已執行的預算成本工作(BCWP)](../../../manage-work/projects/project-finances/calculate-bcwp.md).

   * **對於非父任務：**

      ```
      Total Budgeted Cost Work Performed = Planned Hours * (Percent Complete/100)
      ```

   * **對於父任務：**
執行的總預算成本工作=所有直接子任務的「已執行總預算成本工作」欄位的總和。

   * **專案：**
執行的總預算成本工作=所有頂層任務（父任務和獨立任務）的「執行的總預算成本工作」欄位的總和。 

* EAC費用=將已發生的實際費用成本加到未發生的計畫費用成本的結果。 計算公式如下：

   ```
   EAC Expense = Incurred Actual Expense Cost + Not Incurred Planned Expense
   ```

   * 已發生的實際費用成本=「實際金額」欄位> 0時，所有費用的「計畫金額」欄位的總和。 例如，如果您為任務1建立費用，並在「計畫金額」欄位中輸入$500.00，並在「實際金額」欄位中輸入> 0(即$600.00)，此任務的已發生計畫費用成本為$500.00。
   * 未發生的計畫費用=「實際金額」欄位= 0時，所有費用的「計畫金額」欄位的總和。 例如，如果為任務1建立兩個費用，其中「計畫金額」欄位中的第一個費用值為$500.00，「實際金額」欄位中的值為$600.00，而第二個費用中的「計畫金額」欄位中的值為$300.00，「實際金額」欄位的值為$0.00，則此任務的「未發生的計畫費用」值為$300.00。 

## 在項目或任務中查找EAC

1. 轉到要查看EAC的項目或任務。
1. 展開 **專案詳細資料** 或 **任務詳細資訊** 視您檢視EAC的位置而定，位於專案或任務的左側面板。

1. 按一下 **金融**. 

   EAC值會顯示在 **完成時的估計** 欄位。

   ![](assets/eac-highlighted-on-project-350x112.png)
