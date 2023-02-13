---
product-area: reporting
navigation-topic: text-mode-reporting
title: 使用EXISTS語句建立複雜文本模式篩選器
description: 使用EXISTS語句建立複雜文本模式篩選器
author: Nolan
feature: Reports and Dashboards
exl-id: 106f7c9d-46cc-46c5-ae34-93fd13a36c14
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '2803'
ht-degree: 0%

---

# 使用EXISTS語句建立複雜文本模式篩選器

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: do not EVER&nbsp;delete this article as long as Text Mode still exists in the system.&nbsp;Google ordered this article to be written and we wrote it with the help of consultants, so the use case is very complex and very hard to understand without this. It is also very much used by many customers)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;Alina: **~ Replace screen shot of icons when list/ reporting UI changes)</p>
-->

>[!IMPORTANT]
>
>本文需要深入了解Adobe Workfront API和文字模式報表介面。 如需Workfront API的相關資訊，請參閱 [API基本介紹](../../../wf-api/general/api-basics.md).\
>如需使用文字模式的相關資訊，請參閱 [文字模式概觀](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Workfront中物件關係概觀

所有對象都連結到Workfront資料庫中的其他對象。

了解物件的階層和互依關係，有助於找出可在報表中參考的物件。

如需Workfront中物件及其階層和相依性的相關資訊，請參閱 [了解Adobe Workfront中的物件](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

建立篩選器時，您可以使用標準報表介面，參考連線至篩選器物件的其他物件，其關係層級可達2個。

例如，您可以在問題篩選器中參考PortfolioID，只顯示與使用標準介面之特定產品組合相關聯專案的問題。 在此情況下，產品組合距離問題只有2個層級。

不過，您無法使用標準介面，在問題篩選器中參考Portfolio擁有者，以僅顯示與擁有者為特定使用者之產品組合關聯之專案的問題。 您必須使用文字模式來存取「Portfolio擁有者名稱」欄位，此欄位距離問題有三個層級。

![issue_to_portfolio_owner_sraight_line_icons.PNG](assets/issue-to-portfolio-owner-sraight-line-icons-350x83.png)

如需Workfront中物件的完整清單，請參閱 [API Explorer](../../../wf-api/general/api-explorer.md).

如需如何導覽API總管和尋找物件的相關資訊，請參閱 [使用API Explorer](../../../wf-api/general/using-api-explorer.md).

建立篩選器時，必須在文本模式介面中建立複雜語句，以引用這些類型的對象。

如需建立複雜篩選器的相關資訊，請參閱 [使用EXISTS陳述式的複雜文本模式篩選器概述](#overview-of-complex-text-mode-filters-that-use-exists-statements) 區段。

## 使用EXISTS陳述式的複雜文本模式篩選器概述 {#overview-of-complex-text-mode-filters-that-use-exists-statements}

在對象層次結構中建立跨越多個級別的篩選器或為缺少的對象進行篩選時，請考慮以下事項：

* 如果要引用未直接連接到篩選器對象的對象，必須建立複雜的篩選器。
* 必須使用EXISTS語句執行以下操作：

   * 建立跨越多個層級的篩選器。
   * 建立篩選器，以查找缺少的對象。\
      例如，建立使用者報表時，您可以篩選某段時間內未記錄時間的使用者。

在篩選器中使用EXISTS陳述式時，請考量下列規則：

* 在「存在」(EXISTS)篩選器中可以引用三個對象：

   * 篩選器的對象（原始對象）。
   * 要引用其欄位的對象（目標對象）。
   * 連接原始對象和目標對象的對象（如果它們未直接連接）（連結對象）。

* 使用EXISTS的篩選器包含兩個以等號連結的獨立陳述式：

   * 等號前的陳述式會參照您所參考的物件（連結或目標物件）。
   * 等號後面的語句引用了您引用的對象（原始對象）。

* 必須使用連結對象的對象代碼來連接語句。\
   您可以在API總管中找到所有物件的物件程式碼。\
   如需API總管的相關資訊，請參閱 [API Explorer](https://one.workfront.com/s/api-explorer).

* 當連結對象因原始對象和目標對象直接連接而丟失時，可以使用目標對象的對象代碼而不是連結對象。
* 您可以參照相同物件（目標物件）上的多個欄位（目標欄位），在此情況下，您必須連結依AND引用欄位的行。\
   如需篩選屬於Target物件之多個欄位的範例，請參閱 [範例4:依多個欄位篩選：按Portfolio所有者名稱和Portfolio對齊計分卡ID列出的任務](#example-4-filter-by-multiple-fields-tasks-by-portfolio-owner-name-and-portfolio-alignment-scorecard-id) 一節。

* EXISTS語句支援的唯一修飾符是NOTEXISTS。

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
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對篩選器、檢視、群組的存取</p> <p>編輯對報表、控制面板、日曆的存取，以編輯報表中的篩選器</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理報表權限以編輯報表中的篩選器</p> <p>管理篩選器的權限以進行編輯</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 建立跨對象層次結構中多個級別的複雜文本模式篩選器

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***[This information is somewhat duplicated from the section below: Create Text-Mode Filters for Missing Objects])</p>
-->

您可以建立一個篩選器，該篩選器在存在篩選器對象的對象層次結構的多個級別上引用對象。 例如，您可以針對專案上未與特定Portfolio擁有者相關聯的問題建立問題篩選。

必須始終使用EXISTS語句和文本模式介面來構建此篩選器。

如需篩選的範例，請參閱 [範例1:依Portfolio擁有者名稱篩選問題](#example-1-filter-for-issues-by-portfolio-owner-name) 一節。

要建立跨越對象層次結構中多個級別的篩選器：

1. 識別篩選器的物件。 我們將此對象稱為原始對象。\
   例如，問題。
1. 識別要篩選依據的欄位。 我們將此物件稱為屬於某個目標物件的目標欄位。\
   例如，屬於Portfolio的ownerID欄位（目標欄位）（目標物件）。
1. （條件性）如果原始對象（問題）和目標欄位(ownerID)未直接連接，則必須找到第三個對象，即連接它們的連結對象（項目）。 連結對象必須至少有一個欄位是從原始對象的「欄位」或「引用」頁簽引用的（在原始對象上顯示的連結欄位），並且它還必須有一個連結欄位來指向目標對象，該連結欄位顯示在連結對象的「欄位」或「引用」頁簽中。 連結欄位至連結物件上顯示的目標物件（或連結物件上顯示的連結欄位）必須符合目標欄位。\
   例如，（專案）ID（原始物件上顯示的連結欄位）是從問題（原始物件）中參考。 (Portfolio)ownerID（連結欄位至目標物件）會顯示在專案（連結物件）的「欄位」標籤中。 PortfolioownerID也是目標物件(Portfolio)上的欄位。 連結物件上的連結欄位與目標欄位相符。\
   ![portfolio_id_in_the_project_api_object_PNG](assets/portfolio-id-in-the-project-api-object-350x88.png)

1. 使用API總管來識別 **物件程式碼** 連結對象（項目）的。\
   例如，項目的對象代碼為PROJ。\
   ![project_objCode_in_the_API.PNG](assets/project-objcode-in-the-api-350x84.png)

1. 為原始對象建立篩選器。\
   例如，建立「問題」篩選器。\
   如需建立篩選器的相關資訊，請參閱 [Adobe Workfront中的篩選器概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. 按一下 **切換到文本模式**.
1. 將下列公式示例貼到新篩選器的文本模式介面，並將建議的文本替換為正確的對象和欄位：

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object>
   EXISTS:A:<Linking Field on the Linking Object>=FIELD:<Linking Field displayed on the Original Object>
   EXISTS:A:<Target Object>:<Target Field>=<Your value for the Target Field>
   ```

   如需使用我們先前識別之欄位的範例，請參閱 [範例1:依Portfolio擁有者名稱篩選問題](#example-1-filter-for-issues-by-portfolio-owner-name) 一節。

1. 按一下 **儲存篩選**.

## 為缺少的對象建立複雜的文本模式篩選器

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: **^[This information is somewhat duplicated from the section above: Create Text-Mode Filters that Span Multiple Levels in the Object Hierarchy])</p>
-->

您可以建立一個篩選器，以引用缺少的對象。 例如，您可以建立使用者篩選條件，顯示哪些使用者尚未登入Workfront。

您必須一律使用 *存在* 語句和用於構建此篩選器的文本模式介面。

有關缺少對象的篩選器的示例，請參閱本文的以下部分：

* [範例2:篩選缺少的對象：未出現在任何自訂表單中的自訂欄位](#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms)
* [範例3:篩選缺少的對象：未記錄某段時間的用戶](#example-3-filter-for-missing-objects-users-who-did-not-log-time-for-a-certain-period-of-time)

要建立引用缺少對象的篩選器：

1. 識別篩選器的物件。 我們將此對象稱為原始對象。\
   例如，參數或自訂欄位。
1. 識別要篩選依據的欄位。 我們將此物件稱為屬於某個目標物件的目標欄位。\
   例如，屬於類別（目標物件）的categoryID欄位（目標欄位）。
1. 由於原始對象（參數）和目標欄位(categoryID)之間沒有直接連接，因此您必須找到第三個對象，即連結對象（類別參數），該對象將連接它們。 連結對象必須至少有一個欄位是從原始對象的「欄位」或「引用」頁簽引用的（在原始對象上顯示的連結欄位），並且它還必須有一個連結欄位來指向目標對象，該連結欄位顯示在連結對象的「欄位」或「引用」頁簽中。 連結欄位至連結物件上顯示的目標物件（或連結物件上顯示的連結欄位）必須符合目標欄位。\
   例如，從參數（原始對象）引用了類別參數（顯示在原始對象上的連結欄位）的ID。 parameterID（連結欄位至目標物件）顯示在類別參數（連結物件）的「欄位」標籤中。 顯示在連結物件上的連結欄位與目標欄位相符。
1. 使用API總管來識別 **物件程式碼** （類別參數）。\
   例如，類別參數的物件代碼為CTGYPA。\
   ![category_parameter_objcode_in_api.PNG](assets/category-parameter-objcode-in-api-350x79.png)

1. 為原始對象建立篩選器。\
   例如，建立「參數」篩選器。\
   如需建立篩選器的相關資訊，請參閱 [Adobe Workfront中的篩選器概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. 按一下 **切換到文本模式**.
1. （條件性）如果您要篩選缺少的對象，請將以下公式示例貼到新篩選器的文本模式介面中，並將建議的文本替換為正確的對象和欄位：

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object><br>
   ```

   ```
   EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

   如需未與自訂Forms關聯之自訂欄位的報表範例，請參閱 [範例2:篩選缺少的對象：未出現在任何自訂表單中的自訂欄位](#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms) 一節。

1. 按一下 **儲存篩選**.

## 在對象層次結構中跨越多個級別的文本模式篩選器示例

* [範例1:依Portfolio擁有者名稱篩選問題](#example-1-filter-for-issues-by-portfolio-owner-name)
* [範例2:篩選缺少的對象：未出現在任何自訂表單中的自訂欄位](#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms)
* [範例3:篩選缺少的對象：未記錄某段時間的用戶](#example-3-filter-for-missing-objects-users-who-did-not-log-time-for-a-certain-period-of-time)
* [範例4:依多個欄位篩選：按Portfolio所有者名稱和Portfolio對齊計分卡ID列出的任務](#example-4-filter-by-multiple-fields-tasks-by-portfolio-owner-name-and-portfolio-alignment-scorecard-id)

### 範例1:依Portfolio擁有者名稱篩選問題 {#example-1-filter-for-issues-by-portfolio-owner-name}

使用文字模式介面，您可以建立問題清單的篩選器，以僅顯示與擁有者為特定使用者之產品組合關聯之專案上的問題。

若要依Portfolio擁有者名稱篩選問題：

1. 建立問題篩選器。\
   如需建立篩選器的相關資訊，請參閱 [Adobe Workfront中的篩選器概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. 按一下 **切換到文本模式**.
1. 請參閱下列一般程式碼：

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object><br>
   ```

   ```
   EXISTS:A:<Linking Field on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:<Target Object>:<Target Field>=<Your value for the Target Field>
   ```

1. 將下列程式碼貼入 **設定報表的篩選規則** 取代上述通用代碼的區域：

   <pre>存在:A:$$OBJCODE=PROJ<br>存在:A:ID=FIELD:projectID<br>存在:A:portfolio:ownerID=4d94d7da001699b19edf50de15682221</pre>

   >[!NOTE]
   >
   >* 原始對象是報表的對象：問題
   >* 目標對象為Portfolio。
   >* 連結物件為專案。
   >* 從連結對象引用的目標欄位和指向目標對象的連結欄位是ownerID。
   >* 此處連結對象的對象代碼為PROJ。
   >* 原始對象上顯示的連結欄位為projectID，連結欄位為ID。


1. 將最後一個陳述式中目標欄位(ownerID)的值取代為您環境中的使用者ID。
1. 按一下 **儲存篩選**.

### 範例2:篩選缺少的對象：未出現在任何自訂表單中的自訂欄位 {#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms}

使用文字模式介面，您可以建立篩選器來檢視未與自訂Forms（類別）關聯的自訂欄位（參數）。 此篩選器將參數連結到類別，這些參數通過另一個對象「類別參數」(Category Parameter)連接。 因為兩個欄位之間沒有直接連接，而且由於您正在篩選缺少的資訊，因此必須使用EXISTS語句。

>[!IMPORTANT]
>
>參數是「自訂表單」中參考的欄位庫中存在的欄位。 類別參數是特定表單上顯示的欄位版本。 例如，如果相同的欄位出現在5個表單上，Workfront資料庫中就會有1個參數和5個類別參數。

要篩選未與自訂表單關聯的自訂欄位：

1. 建立參數或自訂欄位篩選。\
   如需建立篩選器的相關資訊，請參閱 [Adobe Workfront中的篩選器概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. 按一下 **切換到文本模式**.
1. 請參閱下列一般程式碼：

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object>
   ```

   ```
   EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

1. 將下列程式碼貼入 **設定報表的篩選規則** 取代上述通用代碼的區域：

   <pre>存在:A:$$OBJCODE=CTGYPA<br>存在:A:parameterID=FIELD:ID<br>存在:A:$$EXISTSMOD=NOTEXISTS</pre>

   >[!NOTE]
   >
   >* 原始對象是報表的對象：參數。
   >* 目標對象為類別。
   >* 連結物件是類別參數。
   >* 連結對象的對象代碼為CTGYPA。
   >* 指向目標對象的連結欄位是parameterID，因為parameterID存在於連結對象表和目標對象表中。
   >* 原始對象上顯示的連結欄位是ID（類別參數的）。


1. 按一下 **儲存篩選**.

### 範例3:篩選缺少的對象：未記錄某段時間的用戶 {#example-3-filter-for-missing-objects-users-who-did-not-log-time-for-a-certain-period-of-time}

使用文字模式介面，您可以建立篩選器來檢視在特定時段內未記錄時間的使用者。 此篩選器會將使用者連結至「小時」，這些小時會直接彼此連線。 但是，必須使用EXISTS語句和文本模式介面才能篩選缺少的資訊。

若要篩選上週未記錄時間的使用者：

1. 建立使用者篩選。\
   如需建立篩選器的相關資訊，請參閱 [Adobe Workfront中的篩選器概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. 按一下 **切換到文本模式**.
1. 請參閱下列一般程式碼：

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object><br>
   ```

   ```
   EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

1. 將下列程式碼貼入 **設定報表的篩選規則** 取代上述通用代碼的區域：

   ```
   EXISTS:A:$$OBJCODE=HOUR<br>EXISTS:A:ownerID=FIELD:ID<br>EXISTS:A:entryDate=$$TODAYb-1w<br>EXISTS:A:entryDate_Range=$$TODAYe-1w<br>EXISTS:A:entryDate_Mod=between<br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

   >[!NOTE]
   >
   >* 原始對象是報表的對象：使用者。
   >* 目標對象為小時。
   >* 在此示例中，您不需要連結對象，因為用戶和小時在Workfront資料庫中直接連接。
   >* 由於沒有連結對象，因此您必須使用目標對象的對象代碼：小時。
   >* 指向目標對象的連結欄位是ownerID(顯示在原始對象上；缺少連結對象)。
   >* 原始物件上顯示的連結欄位是ID（小時）（顯示在目標物件上）;缺少連結對象。)
   >* 存在:A:entryDate語句引用定義目標對象（小時）的欄位，並使用與常規篩選器語句中相同的語法。 這可確保您只顯示未記錄特定時段（在此例中為前一週）之時間的使用者。
   >* NOTEXISTS修飾符表示我們正在查找報表對象（用戶）不存在的項（小時）。


1. 按一下 **儲存篩選**.

### 範例4:依多個欄位篩選：按Portfolio所有者名稱和Portfolio對齊計分卡ID列出的任務 {#example-4-filter-by-multiple-fields-tasks-by-portfolio-owner-name-and-portfolio-alignment-scorecard-id}

使用文字模式介面，您可以建立引用目標物件上多個欄位的篩選器。 在此情況下，引用目標欄位的篩選陳述式必須以AND連結。

例如，您可以篩選任務清單，以僅顯示符合下列條件的任務：

* 它們位於與某個產品組合關聯的項目上，而該產品組合的所有者是特定用戶。
* 它們位於與產品組合關聯的項目上，其項目未與特定的對齊記分卡關聯。

要按Portfolio所有者名稱和Portfolio對齊計分卡ID篩選任務，請執行以下操作：

1. 建立任務篩選器。\
   如需建立篩選器的相關資訊，請參閱 [Adobe Workfront中的篩選器概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. 按一下 **切換到文本模式**.
1. 將下列程式碼貼入 **設定報表的篩選規則** 區域：
   <pre>存在:A:$$OBJCODE=PROJ<br>存在:A:ID=FIELD:projectID<br>存在:A:portfolio:ownerID=4d80ce5200000528787d57807732a33f<br>和:A:存在:A:$$EXISTSMOD=NOTEXISTS<br>和:A:存在:A:$$OBJCODE=PROJ<br>和:A:存在:A:ID=FIELD:projectID<br>和:A:存在:A:portfolio:alignmentScoreCardID=4da387b00001cbc732bb259355c33dad</pre>

   >[!NOTE]
   >
   >* 原始對象是篩選器的對象：任務。
   >* 目標對象為Portfolio。
   >* 第一個目標欄位是ownerID。
   >* 第二個目標欄位是「對齊計分卡ID」。
   >* 連結物件為專案。
   >* 連結對象的對象代碼為PROJ。
   >* Target物件的連結欄位是ID(Portfolio的)。
   >* 原始物件上顯示的連結欄位為projectID。
   >* 以您環境中的使用者ID取代ownerID。


1. 按一下 **儲存篩選**.
