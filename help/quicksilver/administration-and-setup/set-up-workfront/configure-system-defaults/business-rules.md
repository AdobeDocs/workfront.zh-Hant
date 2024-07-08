---
user-type: administrator
product-area: system-administration
navigation-topic: business rules
title: 建立和編輯業務規則
description: 您可以選取想要每月或每季接收新的Workfront功能。
author: Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: ff192113a73e19bf21a3e459cd793f82179dff3d
workflow-type: tm+mt
source-wordcount: '1051'
ht-degree: 0%

---

# 建立和編輯商業規則

{{highlighted-preview-article-level}}

商業規則可讓您套用驗證至Workfront物件，並防止使用者在滿足某些條件時建立、編輯或刪除物件。 商業規則可防止可能影響資料完整性的動作，有助於改善資料品質和營運效率。

一個業務規則只能分配給一個物件。 例如，如果創建“在某些情況下不編輯專案”業務規則，則不能將同一規則應用於任務。 您必須為任務創建具有相同條件的單獨業務規則。

當用戶與物件交互時，訪問級別和對象共用的優先順序高於業務規則。 例如，如果用戶具有不允許編輯專案的訪問級別或權限，則這些級別或將優先於允許在特定條件下編輯專案的業務規則。

當多個業務規則應用於一個物件時，將遵循所有規則，但不按特定順序應用。 例如，您有兩個業務規則。 一個限制在二月份創建費用。 第二種方法防止在項目狀態為完整應用程式時編輯專案。 如果使用者嘗試在六月將費用新增到完成的專案，由於費用已觸發第二個規則，因此無法新增費用。

商業規則適用於透過API以及Workfront介面建立、編輯和刪除物件。

>[!NOTE]
>
>由於商業規則會封鎖某些動作，因此您應該一律先在沙箱或預覽環境中設定商業規則，並在生產環境中啟用前對其進行徹底測試。

## 存取需求

+++ 展開以視圖本文中功能的訪問要求。

您必須具備以下各項才能執行本文中的步驟：

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

如需有關此表格的詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## 商業規則的案例

商業規則的格式為「如果符合定義的條件，則會阻止使用者對物件執行動作，且會顯示訊息。」

商業規則中屬性和其他函式的語法與自訂表單中計算欄位的語法相同。 如需有關語法的詳細資訊，請參閱 [使用表單設計工具新增計算欄位](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

有關 IF 語句的資訊，請參閱 [“IF”語句概述](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md) 和 [計算自定義欄位中](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/condition-operators-calculated-custom-expressions.md)的條件運算符。

有關基於 用戶的通配符的信息，請參閱 [使用基於 用戶的通配符通用化報表](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-user-based-wildcards-generalize-reports.md)。

有關基於日期的通配符的資訊，請參閱 [使用基於日期的通配符通用化報表](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md)。

業務規則中也有 API 通配符。 您只能用于 `$$ISAPI` 在UI或僅在 API 中觸發規則。

一些簡單的業務規則方案是：

* 使用者無法在2月的最後一週新增費用。 此公式可表示為： `IF(AND(MONTH($$TODAY) = 2, DAYOFMONTH($$TODAY) >= 22), "You cannot add new expenses during the last week of February.")`
* 使用者無法編輯處於完成狀態的專案。 此公式可表示為： `IF({status} = "CPL", "You cannot edit this project because it is in Complete status.")`

具有嵌套 IF 語句的場景為：

用戶無法編輯已完成的專案，也無法編輯計劃完成日期為 3 月的專案。 這個公式可以表述為：

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

1. 按一下 **業務規則** 在左側面板中。
1. 按一下 **新業務規則**.
1. 選取要指派商業規則的物件型別，然後按一下 **繼續**.

   ![選取物件](assets/object-for-business-rule2.png)

1. 輸入 **名稱** 適用於商業規則。
1. 在「處於活動&#x200B;**狀態」**&#x200B;欄位中，選擇儲存規則時是否應處於活動狀態。

   如果您選取 **否**，則規則會儲存為非使用中，您可稍後加以啟用。

1. 選取 **觸發** 適用於商業規則。 選項包括：

   * **建立物件時：** 此規則會在使用者嘗試建立物件時套用。
   * **在物件編輯上：** 此規則會在使用者嘗試編輯物件時套用。
   * **物件刪除時：** 此規則會在使用者嘗試刪除物件時套用。

1. （選擇性）輸入 **說明** 商業規則的，以及套用時會發生什麼事情。
1. 在商業規則對話方塊中央的公式編輯器中建立公式。

   商業規則的格式為「如果符合定義的條件，則會阻止使用者對物件執行動作，且會顯示訊息。」

   在公式區域中，您建立的商業規則部分是條件，以及在滿足條件時在Workfront中顯示的訊息。

   * 「物件」是您在建立商業規則時選取的物件型別。 它顯示在對話方塊的標題中。
   * 「動作」是您為規則選取的觸發程式：建立、編輯或刪除物件。
   * 由於物件和動作已定義，因此您不會將它們納入公式中。
   * 當使用者觸發商業規則時，就會向使用者顯示自訂錯誤訊息。 它應該提供明確的指示，說明哪裡出錯了，以及如何更正問題。

   ![新增商業規則對話方塊](assets/add-business-rule-dialog-no-ai-button.png)

   此示例是費用的業務規則。 如果當月是六月，則不允許使用者建立新費用，且訊息會說明此情況。

   如需商業規則的更多範例，請參閱 [商業規則的案例](#scenarios-for-business-rules) 本文章內容。

1. （選擇性）使用公式 **運算式** 和 **欄位** 協助建立規則。

   搜尋運算式或欄位以縮小可用專案清單的範圍。

   可用欄位清單僅限於與商業規則物件型別相關的欄位。

1. 完成業務規則建立后，按兩下儲存&#x200B;****。

>[!NOTE]
>
>添加業務規則后，應通過添加、编辑或刪除關聯的對象來測試它，以確保正確應用規則。

## 啟用業務規則

當業務規則處於非活動狀態時，業務規則清單中的〖處於活動狀態」字段將顯示為「False」。 您無法更新清單 視圖中規則的狀態。

若要啟用業務規則：

1. 在規則清單中選取商業規則，然後按一下「編輯」圖示。
1. 選取 **是** 的 **已啟用** 在商業規則對話方塊中。
1. 按一下「**儲存**」。
