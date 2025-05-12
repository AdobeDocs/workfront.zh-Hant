---
title: 自訂Forms中的進階邏輯範例
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 本文提供用來在自訂欄位上建置進階邏輯的運算式範例。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
source-git-commit: 01eeed1f73c47b79344ca60f3f6d866452cad140
workflow-type: tm+mt
source-wordcount: '758'
ht-degree: 0%

---

# 自訂表單中的進階邏輯範例

邏輯規則可讓您進一步自訂自訂表單上的欄位。

本文提供用來在自訂欄位上建置進階邏輯的運算式範例。

如需新增邏輯至自訂表單的詳細資訊，請參閱[新增邏輯規則至自訂表單和欄位](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront計畫 </td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>
   <p>新增：標準</p>
   <p>或</p>
   <p>目前：計畫</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">存取層級設定</td> 
   <td>管理自訂表單的存取權 </td> 
  </tr>  
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 驗證邏輯範例

驗證邏輯是使用公式建立的，您可以讓邏輯變得簡單或複雜。 驗證可以基於其他欄位的值或物件的狀態，並且您可以在驗證失敗時提供錯誤訊息。

如果套用了邏輯的欄位在使用者填寫自訂表單時符合定義的驗證條件，則該欄位會醒目提示並顯示錯誤訊息。

您可以將驗證邏輯套用至下列欄位型別：單行文字、段落、單選下拉式清單、多選下拉式清單、外部查閱、預先輸入、日期、核取方塊群組，以及選項按鈕。

### 僅允許專案所有者選取「Rush」SLA

在此範例中，單選下拉式欄位具有「標準SLA - 14天」、「優先順序 — 7天」和「匆忙 — 2天」選項。

驗證運算式：

```
IF({ownerID}!=$$USER&&{DE:DV - Dropdown - Control Dates}="2",CONCAT("Only ",{owner}.{name}," may select X Rush"))
```

當不是專案擁有者的任何人（包括系統管理員）嘗試選取&#x200B;**X Rush**&#x200B;時，會顯示錯誤：

![只有專案所有者Claire Stevens可以選取X Rush](assets/sla-xrush.png)

### 根據上一個欄位中的選擇進行日期驗證

繼續以SLA為例，您可以新增根據先前下拉欄位設定驗證的日期欄位。

驗證運算式：

```
IF({DE:DV - Date - Dropdown SLA}<ADDDAYS($$TODAY,{DE:DV - Dropdown - Control Dates}),CONCAT("Earliest: ",ADDDAYS($$TODAY,{DE:DV - Dropdown - Control Dates})))
```

如果使用者選取的日期早於允許的日期，則訊息會顯示他們可以選取的最早日期：

![選取的日期是3月28日，但最早的可用日期是4月3日](assets/date-validation-based-on-previous-choice.png)

### 包含要覆寫之選項的最小字元數

在此範例中，文字欄位會強制最小字元計數，並顯示字元計數。 此外，也會設定個別核取方塊以停用字元計數的驗證。

驗證運算式：

```
IF({DE:DV - Override}!="Disable Validation"&&LEN({DE:DV - Text - Min Length})<"7",CONCAT(LEN({DE:DV - Text - Min Length})," characters / ",("7"-LEN({DE:DV - Text - Min Length}))," remaining"))
```

選取下列核取方塊，即可覆寫驗證的強制執行：

![停用驗證的核取方塊](assets/disable-validation-checkbox.png)

文字欄位包含執行中的字元計數：

![字元計數為5個可用，剩餘2個](assets/running-character-count.png)

### 鎖定欄位，只有所有者才能編輯它

在此範例中，欄位只能由專案所有者編輯。 即使系統管理員也無法編輯此欄位。

驗證運算式：

```
IF({ownerID}!=$$USER,IF(ISBLANK({ownerID}),"Project Owner will provide this.",CONCAT("Only ",{owner}.{name}," can edit this.")))
```

如果非專案所有者的使用者嘗試在欄位中輸入，他們會看到一則訊息，指出只有專案所有者可以編輯欄位。

![只有Claire Stevens可以編輯此欄位](assets/only-project-owner-can-edit.png)

### 自動提示會根據其他欄位值允許或拒絕值

在此範例中，預先輸入欄位會根據表單上其他欄位中輸入的值，動態地允許或拒絕值。

驗證運算式：

```
IF({DE:DV - Text - Budget}>"10000",
   IF({DE:DV - TA User - by Budget}.{role}!="Director","Requires Director Approver")
)
```

如果預算欄位中的值超過$10,000，則即使自動提示設定上未啟用角色篩選器，也只能從自動提示中選取具有主管角色的使用者。

![預算金額需要主管核准](assets/budget-director.png)

### 不允許輸入日期起小於10天的值

在此範例中，驗證僅允許輸入日期起未來10天的值。 公式中也包含覆蓋驗證的選項（在單獨的核取方塊欄位中），並允許日期欄位留空。

驗證運算式：

```
IF({DE:DV - Override}!="Disable Validation"&&ISBLANK({DE:DV - Date - Deadline})!="true"&&{DE:DV - Date - Deadline}<ADDDAYS({entryDate},"10"),CONCAT("Earliest: ",ADDDAYS({entryDate},"10")))
```

從輸入日期起不到10天的任何值都會觸發驗證：

![選取的日期為3月28日，但最早的可用日期為4月4日](assets/earliest-deadline-date.png)

空白值不會觸發驗證訊息：

![日期](assets/blank-date-allowed.png)的空白值

### 在多重選取欄位中強制實施精確/最小/最大選取

在此範例中，核取方塊群組之類的多選欄位會要求使用者選擇特定數量的選項。

驗證運算式（剛好挑選兩個）：

```
IF({DE:DV - Override}!="Disable Validation"&&ARRAYLENGTH(ARRAY({DE:DV - Checkbox - Pick exactly 2},","))!="2","Pick Exactly 2 Options")
```

驗證運算式（至少選取兩個）：

```
IF({DE:DV - Override}!="Disable Validation"&&ARRAYLENGTH(ARRAY({DE:DV - Checkbox - Pick at least 2},","))<"2","Pick at least 2 choices")
```

驗證運算式（最多選取兩個）：

```
IF({DE:DV - Override}!="Disable Validation"&&ARRAYLENGTH(ARRAY({DE:DV - Checkbox - Pick no more than 2},","))>"2","Pick no more than 2 choices")
```

使用者如果未選取正確數量的選項，則會看到驗證錯誤。

![驗證錯誤範例](assets/min-max-selections.png)
