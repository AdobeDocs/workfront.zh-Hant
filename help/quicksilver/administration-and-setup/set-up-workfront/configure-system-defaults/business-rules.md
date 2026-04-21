---
user-type: administrator
product-area: system-administration
navigation-topic: business rules
title: 建立和編輯商業規則
description: 商業規則可讓您套用驗證至Workfront物件，並防止使用者在滿足某些條件時建立、編輯或刪除物件。 商業規則可防止可能影響資料完整性的動作，有助於改善資料品質和營運效率。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 780c996c-5cf1-42fe-898d-2cc208bbae7b
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 8ee1cda376b51a5f5b7b4af44e6d34bf70ee9600
workflow-type: tm+mt
source-wordcount: '1803'
ht-degree: 3%

---

# 建立和編輯業務規則

商業規則可讓您套用驗證至Workfront物件，並防止使用者在滿足某些條件時建立、編輯或刪除物件。 商業規則驗證可防止可能影響資料完整性的動作，有助於改善資料品質和營運效率。

擁有Workflow Ultimate套件的組織也可以設定商業規則，以在符合某些條件時，為已建立、已編輯或已修改的物件自動執行動作。 可用的動作包括共用物件或將自訂表單附加到物件。


單一商業規則只能指派給一個物件。 例如，如果您建立在特定條件下不編輯專案的業務規則，則無法將相同的規則套用至任務。 您必須使用相同的任務條件來建立個別的商業規則。

當使用者與物件互動時，存取層級和物件共用的優先順序高於商業規則。 例如，如果使用者具有不允許編輯專案的存取層級或許可權，則這些許可權會優先於允許在特定條件下編輯專案的業務規則。

當多個商業規則套用至物件時，規則會全部遵循，但不會以特定順序套用。 例如，您有兩個業務規則。 其中一項限制在2月建立費用。 第二個可防止在專案狀態為完成時編輯專案。 如果使用者嘗試在六月將費用新增到完成的專案，由於費用已觸發第二個規則，因此無法新增費用。

商業規則適用於透過API以及Workfront介面建立、編輯和刪除物件。

>[!NOTE]
>
>由於商業規則會封鎖某些動作，因此您應該一律先在沙箱或預覽環境中設定商業規則，並在生產環境中啟用前對其進行徹底測試。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr>
   <td>Adobe Workfront 封裝
   </td>
   <td> <p>商業規則驗證：<ul><li><p>Ultimate</p></li><li>
    <p>Workflow Ultimate</p></li></ul></p><p>商業規則自動化：<ul><li>
    <p>Workflow Ultimate</p></li><ul></p>
   </td>
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

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 商業規則的案例

* [商業規則驗證的案例](#scenarios-for-business-rule-validation)
* [商業規則自動化的案例](#scenarios-for-business-rule-automation)

### 商業規則驗證的案例

商業規則驗證的格式為「如果符合定義的條件，則會阻止使用者對物件執行動作，且會顯示訊息。」

商業規則中屬性和其他函式的語法與自訂表單中計算欄位的語法相同。 如需有關語法的詳細資訊，請參閱[使用表單設計工具新增計算欄位](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)。

如需有關IF陳述式的資訊，請參閱計算自訂欄位中的[&quot;IF&quot;陳述式概述](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md)和[條件運運算元](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/condition-operators-calculated-custom-expressions.md)。

如需使用者型萬用字元的資訊，請參閱[使用使用者型萬用字元來一般化報表](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-user-based-wildcards-generalize-reports.md)。

如需日期型萬用字元的資訊，請參閱[使用日期型萬用字元來一般化報表](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md)。

商業規則中也提供API萬用字元。 僅在API中使用`$$ISAPI`觸發規則。 使用`!$$ISAPI`只會在使用者介面中強制執行規則，並允許使用者透過API略過規則。

* 例如，此規則禁止使用者透過API編輯完成的專案。 如果未使用萬用字元，則規則會同時封鎖使用者介面和API中的動作。

  ```
  IF({status} = "CPL" && $$ISAPI, "You cannot edit completed projects through the API.")
  ```

在運算式中使用`$$BEFORE_STATE`和`$$AFTER_STATE`萬用字元來存取任何編輯前後物件的欄位值。

* 這兩個萬用字元都可用於編輯觸發器。 編輯觸發器的預設狀態（如果運算式中未包含任何狀態）為`$$AFTER_STATE`。
* 物件建立觸發程式只允許`$$AFTER_STATE`，因為之前狀態不存在。
* 物件刪除觸發程式只允許`$$BEFORE_STATE`，因為after狀態不存在。

一些簡單的商業規則案例包括：

* 使用者無法在2月的最後一週新增費用。 此公式可表示為：

  ```
  IF(MONTH($$TODAY) = 2 && DAYOFMONTH($$TODAY) >= 22, "You cannot add new expenses during the last week of February.")
  ```

* 使用者無法編輯處於完成狀態的專案名稱。 此公式可表示為：

  ```
  IF({status} = "CPL" && {name} != $$BEFORE_STATE.{name}, "You cannot edit the project name.")
  ```

系統允許每個觸發器的每個物件擁有一個商業規則。 例如，一個編輯觸發規則可用於問題。 不過，您可以在含有巢狀IF陳述式的公式中加入多個規則。

含有巢狀IF陳述式的案例是：

使用者無法編輯已完成的專案，也無法編輯具有三月計畫完成日期的專案。 此公式可表示為：

```
IF(
    $$AFTER_STATE.{status}="CPL",
    "You cannot edit a completed project",
    IF(
        MONTH({plannedCompletionDate})=3,
        "You cannot edit a project with a planned completion date in March")
)
```

### 在商業規則中啟用本地化

如果您的組織使用自訂本地化，則必須在商業規則中啟用商業規則訊息的翻譯。 如果未啟用翻譯，即使訊息文字在本地化清單中，且使用者的瀏覽器設定為適當的語言，訊息仍會以英文顯示給讀者。

設定規則時，請在訊息前插入TRANSLATE這個字，並將訊息括在括弧中。

>[!BEGINSHADEBOX]

範例：

此範例假設訊息「您無法編輯已完成的專案」包含在「設定」的本地化區域中，且使用者的瀏覽器設定為當地語系化語言。

* `IF({status} = "CPL", "You cannot edit completed projects.") `
訊息會以英文顯示。
* `IF({status} = "CPL", TRANSLATE("You cannot edit completed projects."))`
訊息會以當地語系化語言顯示。

>[!ENDSHADEBOX]

如需自訂本地化的詳細資訊，請參閱[設定自訂本地化](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-custom-localization.md)。

## 商業規則自動化的案例

>[!NOTE]
>
>貴組織必須擁有Workflow Ultimate套件才能使用商業規則自動化。

商業規則自動化的格式為「如果符合定義的條件，則會觸發所選的自動化」。

商業規則自動化公式不需要錯誤訊息

若要確保每當選取的物件與動作（例如建立專案時）發生時，自動化都會執行，請使用下列公式：

```
IF(true, true)
```

若要在專案已核准後才共用該專案，請使用如下的公式：

```
IF({status} = "APR", true)
```

您可以在商業規則動作中使用萬用字元，如[商業規則驗證的案例](#scenarios-for-business-rule-validation)一節中所述。


## 新增商業規則

{{step-1-to-setup}}

1. 按一下左側面板中的&#x200B;**商業規則**。
1. 按一下&#x200B;**新商業規則**。

1. 在規則產生器對話方塊中輸入商業規則的&#x200B;**名稱**。
1. 在&#x200B;**為使用中**&#x200B;欄位中，選取儲存規則時是否應該使用中。

   如果您選取&#x200B;**否**，規則會儲存為非使用中，您可稍後再加以啟用。

1. （選擇性）輸入商業規則的&#x200B;**描述**，以及套用時會發生什麼情況。


1. 選取要指派商業規則的物件型別。

   ![選取物件](assets/object-for-business-rule4.png)

   您可以將商業規則套用至下列物件：

   * 專案
   * 任務
   * 問題/請求
   * 專案組合
   * 文件
   * 方案
   * 費用
   * 使用者
   * 公司
   * 疊代
   * 計費記錄
   * 群組
   * 風險
   * 費率卡
   * 指派
   * 職務角色
   * 資源集區
   * 休假
   * 時數
   * 範本
   <!--
   * Non-labor resource
   * Non-labor resource category
   * Staffing Plan
   * Staffing Plan Resource
   * Team
   -->

1. 選取商業規則的&#x200B;**觸發器**。 選項包括：

   * **已建立**&#x200B;當使用者嘗試建立物件時，會套用規則。
   * **已編輯**&#x200B;當使用者嘗試編輯物件時，會套用規則。
   * **已刪除**&#x200B;當使用者嘗試刪除物件時，會套用規則。

1. 在商業規則對話方塊中央的公式編輯器中建立公式。

   商業規則的格式為「如果符合定義的條件，則會阻止使用者對物件執行動作，且會顯示訊息。」

   在公式區域中，您建立的商業規則部分是條件，以及在滿足條件時在Workfront中顯示的訊息。

   * 「物件」是您在建立商業規則時選取的物件型別。 它顯示在對話方塊的標題中。
   * 「動作」是您為規則選取的觸發程式：建立、編輯或刪除物件。
   * 由於物件和動作已定義，因此您不會將它們納入公式中。
   * 只有在規則用於驗證時才會包含自訂錯誤訊息，並在使用者觸發商業規則時顯示給使用者。 它應該提供明確的指示，說明哪裡出錯了，以及如何更正問題。

     您可以在錯誤訊息中加入靜態URL，以連結至檔案或其他實用頁面，引導使用者如何在規則的限制內修改其動作。

     在此範例中，「瞭解更多」將連結至URL。 `"You are not allowed to add a new project in November.[Learn more](http://url)"` URL必須位於括弧中，但不需要括弧中的連結文字。 您可以顯示完整URL，它將是可點按的連結。

   ![新增商業規則對話方塊](assets/add-business-rule-new.png)

   此範例是專案的業務規則。 如果目前月份是11月，則不允許使用者建立新專案，且訊息會說明此情況。

   如需商業規則的更多範例，請參閱本文中的[商業規則案例](#scenarios-for-business-rules)。

1. （選擇性）使用右側面板中的公式&#x200B;**運算式**&#x200B;和&#x200B;**欄位**&#x200B;協助建立規則。

   搜尋運算式或欄位以縮小可用專案清單的範圍。

   可用欄位清單僅限於與商業規則物件型別相關的欄位。

1. （視條件而定）如果您要驗證動作，如果您的組織位於Workfront Ultimate套件上，請在「然後」區域中，選取&#x200B;**驗證物件**。

   對於其他套件，會預先選取此選項。

1. （視條件而定）若要自動執行其他動作，請選取動作。

   如需這些動作的詳細資訊，請參閱本文中的[商業規則自動化選項](#business-rule-automation-options)一節。

   >[!NOTE]
   >
   >您的組織必須在工作流程Ultimate套件上，才能使用驗證以外的動作。 如果您沒有看到這些其他選項，表示您的組織不在Workflow Ultimate套件中。

1. 當您完成建立商業規則時，請按一下[儲存]。****

>[!NOTE]
>
>新增商業規則後，您應該透過新增、編輯或刪除關聯的物件來測試它，以確保規則已正確套用。

### 商業規則自動化選項

>[!NOTE]
>
>您的組織必須在工作流程Ultimate套件上，才能使用驗證以外的動作。 如果您沒有看到這些其他選項，表示您的組織不在Workflow Ultimate套件中。

您可以設定這些動作，以便在觸發商業規則時自動執行。 可用的動作取決於選取的物件型別。

| 自動完成 | 進一步設定 |
|---|---|
| 附加自訂表單 | 選取您要新增的自訂表單 |
| 共用此物件 | 選取您要共用物件的使用者、角色、群組、公司或存取層級。 |

## 啟用商業規則

當商業規則處於非使用中狀態時，商業規則清單中的處於使用中欄位會顯示False。 您無法在清單檢視中更新規則的狀態。

若要啟用商業規則：

1. 在規則清單中選取商業規則，然後按一下「編輯」圖示。
1. 在商業規則對話方塊中，選取&#x200B;**Is Active**&#x200B;的&#x200B;**是**。
1. 按一下「**儲存**」。
