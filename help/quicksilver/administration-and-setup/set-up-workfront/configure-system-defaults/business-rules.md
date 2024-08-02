---
user-type: administrator
product-area: system-administration
navigation-topic: business rules
title: 建立和編輯商業規則
description: 商業規則可讓您套用驗證至Workfront物件，並防止使用者在滿足某些條件時建立、編輯或刪除物件。 商業規則可防止可能影響資料完整性的動作，有助於改善資料品質和營運效率。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 780c996c-5cf1-42fe-898d-2cc208bbae7b
source-git-commit: 634b4dc9a75b306c46168848807faff80ab2eced
workflow-type: tm+mt
source-wordcount: '1078'
ht-degree: 0%

---

# 建立和編輯商業規則

商業規則可讓您套用驗證至Workfront物件，並防止使用者在滿足某些條件時建立、編輯或刪除物件。 商業規則可防止可能影響資料完整性的動作，有助於改善資料品質和營運效率。

單一商業規則只能指派給一個物件。 例如，如果您建立在特定條件下不編輯專案的業務規則，則無法將相同的規則套用至任務。 您必須使用相同的任務條件來建立個別的商業規則。

當使用者與物件互動時，存取層級和物件共用的優先順序高於商業規則。 例如，如果使用者具有不允許編輯專案的存取層級或許可權，則這些許可權會優先於允許在特定條件下編輯專案的業務規則。

當多個商業規則套用至物件時，規則會全部遵循，但不會以特定順序套用。 例如，您有兩個業務規則。 其中一項限制在2月建立費用。 第二個可防止在專案狀態為完成時編輯專案。 如果使用者嘗試在六月將費用新增到完成的專案，由於費用已觸發第二個規則，因此無法新增費用。

商業規則適用於透過API以及Workfront介面建立、編輯和刪除物件。

>[!NOTE]
>
>由於商業規則會封鎖某些動作，因此您應該一律先在沙箱或預覽環境中設定商業規則，並在生產環境中啟用前對其進行徹底測試。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具備下列專案才能執行本文所述的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront計畫</td> 
   <td>Ultimate</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td>標準</td> 
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td>系統管理員</td> 
  </tr>  
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 商業規則的案例

商業規則的格式為「如果符合定義的條件，則會阻止使用者對物件執行動作，且會顯示訊息。」

商業規則中屬性和其他函式的語法與自訂表單中計算欄位的語法相同。 如需有關語法的詳細資訊，請參閱[使用表單設計工具新增計算欄位](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)。

如需有關IF陳述式的資訊，請參閱計算自訂欄位中的[&quot;IF&quot;陳述式概述](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md)和[條件運運算元](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/condition-operators-calculated-custom-expressions.md)。

如需使用者型萬用字元的資訊，請參閱[使用使用者型萬用字元來一般化報表](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-user-based-wildcards-generalize-reports.md)。

如需日期型萬用字元的資訊，請參閱[使用日期型萬用字元來一般化報表](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md)。

商業規則中也提供API萬用字元。 您只能在UI或API中使用`$$ISAPI`來觸發規則。

一些簡單的商業規則案例包括：

* 使用者無法在2月的最後一週新增費用。 此公式可以表示為： `IF(MONTH($$TODAY) = 2 && DAYOFMONTH($$TODAY) >= 22, "You cannot add new expenses during the last week of February.")`
* 使用者無法編輯處於完成狀態的專案。 此公式可以表示為： `IF({status} = "CPL", "You cannot edit this project because it is in Complete status.")`

含有巢狀IF陳述式的案例是：

使用者無法編輯已完成的專案，也無法編輯具有三月計畫完成日期的專案。 此公式可表示為：

```
IF(
    {status}="CPL",
    "You cannot edit a completed project",
    IF(
        MONTH({plannedCompletionDate})=3,
        "You cannot edit a project with a planned completion date in March")
)
```

## 新增商業規則

{{step-1-to-setup}}

1. 按一下左側面板中的&#x200B;**商業規則**。
1. 按一下&#x200B;**新商業規則**。
1. 選取要指派商業規則的物件型別，然後按一下[繼續]。****

   ![選取物件](assets/object-for-business-rule2.png)

1. 輸入商業規則的&#x200B;**名稱**。
1. 在&#x200B;**為使用中**&#x200B;欄位中，選取儲存規則時是否應該使用中。

   如果您選取&#x200B;**否**，規則會儲存為非使用中，您可稍後再加以啟用。

1. 選取商業規則的&#x200B;**觸發器**。 選項包括：

   * **建立物件時：**&#x200B;當使用者嘗試建立物件時，會套用規則。
   * **在物件編輯時：**&#x200B;當使用者嘗試編輯物件時，會套用規則。
   * **在物件刪除時：**&#x200B;當使用者嘗試刪除物件時，會套用規則。

1. （選擇性）輸入商業規則的&#x200B;**描述**，以及套用時會發生什麼情況。
1. 在商業規則對話方塊中央的公式編輯器中建立公式。

   商業規則的格式為「如果符合定義的條件，則會阻止使用者對物件執行動作，且會顯示訊息。」

   在公式區域中，您建立的商業規則部分是條件，以及在滿足條件時在Workfront中顯示的訊息。

   * 「物件」是您在建立商業規則時選取的物件型別。 它顯示在對話方塊的標題中。
   * 「動作」是您為規則選取的觸發程式：建立、編輯或刪除物件。
   * 由於物件和動作已定義，因此您不會將它們納入公式中。
   * 當使用者觸發商業規則時，就會向使用者顯示自訂錯誤訊息。 它應該提供明確的指示，說明哪裡出錯了，以及如何更正問題。

   ![新增商業規則對話方塊](assets/add-business-rule-dialog-no-ai-button.png)

   此範例是費用的商業規則。 如果當月是六月，則不允許使用者建立新費用，且訊息會說明此情況。

   如需商業規則的更多範例，請參閱本文中的[商業規則案例](#scenarios-for-business-rules)。

1. （選擇性）使用右側面板中的公式&#x200B;**運算式**&#x200B;和&#x200B;**欄位**&#x200B;協助建立規則。

   搜尋運算式或欄位以縮小可用專案清單的範圍。

   可用欄位清單僅限於與商業規則物件型別相關的欄位。

1. 當您完成建立商業規則時，請按一下[儲存]。****

>[!NOTE]
>
>新增商業規則後，您應該透過新增、編輯或刪除關聯的物件來測試它，以確保規則已正確套用。

## 啟用商業規則

當商業規則處於非使用中狀態時，商業規則清單中的處於使用中欄位會顯示False。 您無法在清單檢視中更新規則的狀態。

若要啟用商業規則：

1. 在規則清單中選取商業規則，然後按一下「編輯」圖示。
1. 在商業規則對話方塊中，選取&#x200B;**Is Active**&#x200B;的&#x200B;**是**。
1. 按一下「**儲存**」。
