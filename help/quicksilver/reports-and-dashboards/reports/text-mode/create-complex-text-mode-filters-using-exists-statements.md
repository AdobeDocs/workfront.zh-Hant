---
product-area: reporting
navigation-topic: text-mode-reporting
title: 使用EXISTS語句建立複雜文本模式篩選器
description: 使用EXISTS語句建立複雜文本模式篩選器
author: Nolan
feature: Reports and Dashboards
exl-id: 106f7c9d-46cc-46c5-ae34-93fd13a36c14
source-git-commit: 888c938e5d649557df69374a55d4e4ecc2da6f55
workflow-type: tm+mt
source-wordcount: '2799'
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
>本文要求對Adobe WorkfrontAPI和文本模式報告介面有深入的瞭解。 有關WorkfrontAPI的資訊，請參見 [API基礎](../../../wf-api/general/api-basics.md)。\
>有關使用文本模式的資訊，請參見 [文本模式概述](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)。

## Workfront對象關係概述

所有對象都連結到Workfront資料庫中的其他對象。

瞭解對象的層次結構和相互依賴關係有助於您瞭解哪些對象可以在報告中引用。

有關對象在Workfront中的資訊以及其層次結構和相互依賴性的資訊，請參見 [瞭解Adobe Workfront的對象](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)。

構建篩選器時，可以使用標準報告介面引用最多2個關係級別內連接到篩選器對象的其他對象。

例如，您可以在問題篩選器中引用PortfolioID，以便僅使用標準介面顯示與特定項目組合關聯的項目上的問題。 在這種情況下，投資組合離問題有2個級別。

但是，您不能在問題篩選器中使用標準介面來引用Portfolio所有者，以僅顯示與責任者是特定用戶的包關聯的項目中的問題。 必須使用文本模式來訪問Portfolio所有者名稱欄位，該欄位距離問題有三個級別。

![issue_to_portfolio_owner_sraight_line_icons.PNG](assets/issue-to-portfolio-owner-sraight-line-icons-350x83.png)

有關Workfront中對象的完整清單，請參見 [API資源管理器](../../../wf-api/general/api-explorer.md)。

有關如何導航API瀏覽器和查找對象的資訊，請參見 [使用API資源管理器](../../../wf-api/general/using-api-explorer.md)。

構建篩選器時，必須在文本模式介面中構建複雜語句以引用這些類型的對象。

有關構建複雜篩選器的資訊，請參見 [使用EXISTS語句的複雜文本模式篩選器概述](#overview-of-complex-text-mode-filters-that-use-exists-statements) 的子菜單。

## 使用EXISTS語句的複雜文本模式篩選器概述 {#overview-of-complex-text-mode-filters-that-use-exists-statements}

在建立跨對象層次結構中多個級別的篩選器或為缺少的對象篩選器時，請考慮以下事項：

* 當要引用未直接連接到篩選器對象的對象時，必須建立複雜的篩選器。
* 必須使用EXISTS語句執行以下操作：

   * 建立跨多個級別的篩選器。
   * 建立查找缺少的對象的篩選器。\
      例如，在生成用戶報告時，您可以篩選某段時間內沒有記錄時間的用戶。

在篩選器中使用EXISTS語句時請考慮以下規則：

* 在EXISTS篩選器中可以引用三個對象：

   * 篩選器的對象（原始對象）。
   * 要引用其欄位的對象（目標對象）。
   * 連接原始對象和目標對象的對象，以防它們不直接連接（連結對象）。

* 使用EXISTS的篩選器包含兩個由等號連結的單獨語句：

   * 等號前的語句引用您引用的對象（連結或目標對象）。
   * 等號後的語句引用您引用的對象（原始對象）。

* 必須使用連結對象的對象代碼來連接語句。\
   可以在API資源管理器中找到所有對象的對象代碼。\
   有關API瀏覽器的資訊，請參見 [API資源管理器](../../../wf-api/general/api-explorer.md)。

* 當由於原始對象和目標對象直接連接而缺少連結對象時，可以使用目標對象的對象代碼而不是連結對象。
* 您可以引用同一對象（目標對象）上的多個欄位（目標欄位），在這種情況下，您必須通過AND連接引用這些欄位的行。\
   有關篩選屬於目標對象的多個欄位的示例，請參見 [示例4:按多個欄位篩選：按Portfolio所有者名稱和Portfolio對齊記分卡ID列出的任務](#example-4-filter-by-multiple-fields-tasks-by-portfolio-owner-name-and-portfolio-alignment-scorecard-id) 的下界。

* EXISTS語句支援的唯一修飾符是NOTEXISTS。

## 訪問要求

您必須具有以下訪問權限才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront許可證*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對篩選器、視圖、分組的訪問</p> <p>編輯對報表、儀表板、日曆的訪問以編輯報表中的篩選器</p> <p>注：如果您仍然沒有訪問權限，請詢問您的Workfront管理員是否在您的訪問級別設定了其他限制。 有關Workfront管理員如何修改您的訪問級別的資訊，請參見 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自定義訪問級別</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">對象權限</td> 
   <td> <p>管理對報表的權限以編輯報表中的篩選器</p> <p>管理篩選器的權限以編輯它</p> <p>有關請求附加訪問的資訊，請參見 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求訪問對象 </a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要瞭解您擁有的計畫、許可證類型或訪問權限，請與您的Workfront管理員聯繫。

## 建立跨對象層次結構中多個級別的複雜文本模式篩選器

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***[This information is somewhat duplicated from the section below: Create Text-Mode Filters for Missing Objects])</p>
-->

您可以構建一個篩選器，該篩選器在存在篩選器對象的對象層次結構的多個級別中引用對象。 例如，您可以針對與某個Portfolio所有者不關聯的項目上的問題構建問題篩選器。

必須始終使用EXISTS語句和文本模式介面來構建此篩選器。

有關篩選器的示例，請參見 [示例1:按Portfolio所有者名稱篩選問題](#example-1-filter-for-issues-by-portfolio-owner-name) 的下界。

要建立跨對象層次結構中多個級別的篩選器：

1. 標識篩選器的對象。 我們將此對象稱為原始對象。\
   例如，Issue。
1. 標識要篩選依據的欄位。 我們將此對象稱為屬於目標對象的目標欄位。\
   例如，屬於Portfolio（目標對象）的ownerID欄位（目標欄位）。
1. （條件）如果原始對象（問題）和目標欄位(ownerID)未直接連接，則必須找到第三個對象，即連接它們的連結對象（項目）。 連結對象必須至少有一個從原始對象的「欄位」(或「引用」(References)頁籤引用的欄位(「連結」(Linking)欄位顯示在原始對象上)，並且還必須有一個與「連結對象」的「欄位」（或「引用」）頁籤中顯示的目標對象的連結欄位。 連結對象（或連結對象上顯示的連結欄位）上顯示的目標對象的連結欄位必須與目標欄位匹配。\
   例如，（項目）ID（原始對象上顯示的連結欄位）從問題（原始對象）中引用。 (Portfolio)ownerID（將欄位連結到目標對象）顯示在項目（連結對象）的「欄位」頁籤中。 PortfolioownerID也是目標對象(Portfolio)上的欄位。 連結對象上的連結欄位與目標欄位匹配。\
   ![portfolio_id_in_the_project_api_object.PNG](assets/portfolio-id-in-the-project-api-object-350x88.png)

1. 使用API資源管理器，標識 **對象代碼** 的子菜單。\
   例如，項目的對象代碼為PROJ。\
   ![project_objCode_in_the_API.PNG](assets/project-objcode-in-the-api-350x84.png)

1. 為原始對象建立篩選器。\
   例如，建立問題篩選器。\
   有關建立篩選器的資訊，請參見 [篩選器概述Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)。

1. 按一下 **切換到文本模式**。
1. 將以下公式示例貼上到新篩選器的文本模式介面，並用正確的對象和欄位替換建議的文本：

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object>
   EXISTS:A:<Linking Field on the Linking Object>=FIELD:<Linking Field displayed on the Original Object>
   EXISTS:A:<Target Object>:<Target Field>=<Your value for the Target Field>
   ```

   有關使用我們在上面標識的欄位的示例，請參見 [示例1:按Portfolio所有者名稱篩選問題](#example-1-filter-for-issues-by-portfolio-owner-name) 的下界。

1. 按一下 **保存篩選器**。

## 為缺少的對象建立複雜文本模式篩選器

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: **^[This information is somewhat duplicated from the section above: Create Text-Mode Filters that Span Multiple Levels in the Object Hierarchy])</p>
-->

可以構建引用缺少的對象的篩選器。 例如，您可以構建一個用戶篩選器，顯示哪些用戶沒有在Workfront登錄數小時。

您必須始終使用 *存在* 語句和文本模式介面來構建此篩選器。

有關缺少對象的篩選器示例，請參閱本文的以下各節：

* [示例2:篩選缺少的對象：未在任何自定義表單中顯示的自定義欄位](#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms)
* [示例3:篩選缺少的對象：未記錄某段時間的用戶](#example-3-filter-for-missing-objects-users-who-did-not-log-time-for-a-certain-period-of-time)

要建立引用缺少對象的篩選器：

1. 標識篩選器的對象。 我們將此對象稱為原始對象。\
   例如，「參數」(Parameter)或「自定義欄位」(Custom Field)。
1. 標識要篩選依據的欄位。 我們將此對象稱為屬於目標對象的目標欄位。\
   例如，屬於類別（目標對象）的categoryID欄位（目標欄位）。
1. 由於原始對象（參數）和目標欄位（類別ID）未直接連接，因此必須找到第三個對象，即連接它們的連結對象（類別參數）。 連結對象必須至少有一個從原始對象的「欄位」(或「引用」(References)頁籤引用的欄位(「連結」(Linking)欄位顯示在原始對象上)，並且還必須有一個與「連結對象」的「欄位」（或「引用」）頁籤中顯示的目標對象的連結欄位。 連結對象（或連結對象上顯示的連結欄位）上顯示的目標對象的連結欄位必須與目標欄位匹配。\
   例如，從參數（原始對象）中引用「類別參數」（顯示在原始對象上的連結欄位）的ID。 參數ID（將欄位連結到目標對象）顯示在「類別參數（連結對象）」的「欄位」頁籤中。 連結對象上顯示的目標對象的連結欄位與目標欄位匹配。
1. 使用API資源管理器，標識 **對象代碼** 的子菜單。\
   例如，類別參數的對象代碼為CTGYPA。\
   ![category_parameter_objcode_in_api.PNG](assets/category-parameter-objcode-in-api-350x79.png)

1. 為原始對象建立篩選器。\
   例如，建立「參數」過濾器。\
   有關建立篩選器的資訊，請參見 [篩選器概述Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)。

1. 按一下 **切換到文本模式**。
1. （條件）如果要篩選缺少的對象，請將以下公式示例貼上到新篩選器的文本模式介面，並用正確的對象和欄位替換建議的文本：

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object><br>
   ```

   ```
   EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

   有關未與自定義Forms關聯的自定義欄位的報告示例，請參見 [示例2:篩選缺少的對象：未在任何自定義表單中顯示的自定義欄位](#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms) 的下界。

1. 按一下 **保存篩選器**。

## 跨對象層次結構中多個級別的文本模式篩選器示例

* [示例1:按Portfolio所有者名稱篩選問題](#example-1-filter-for-issues-by-portfolio-owner-name)
* [示例2:篩選缺少的對象：未在任何自定義表單中顯示的自定義欄位](#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms)
* [示例3:篩選缺少的對象：未記錄某段時間的用戶](#example-3-filter-for-missing-objects-users-who-did-not-log-time-for-a-certain-period-of-time)
* [示例4:按多個欄位篩選：按Portfolio所有者名稱和Portfolio對齊記分卡ID列出的任務](#example-4-filter-by-multiple-fields-tasks-by-portfolio-owner-name-and-portfolio-alignment-scorecard-id)

### 示例1:按Portfolio所有者名稱篩選問題 {#example-1-filter-for-issues-by-portfolio-owner-name}

使用文本模式介面，您可以為問題清單構建篩選器，以僅顯示與其所有者為特定用戶的項目關聯的項目上的問題。

要按Portfolio所有者名稱篩選問題：

1. 建立問題篩選器。\
   有關建立篩選器的資訊，請參見 [篩選器概述Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)。

1. 按一下 **切換到文本模式**。
1. 請參閱以下通用代碼：

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object><br>
   ```

   ```
   EXISTS:A:<Linking Field on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:<Target Object>:<Target Field>=<Your value for the Target Field>
   ```

1. 將以下代碼貼上到 **設定報表的篩選器規則** 替換上述通用代碼：

   <pre>存在:A:$$OBJCODE=PROJ<br>存在:A:ID=FIELD:projectID<br>存在:A:產品組合：ownerID=4d94d7da001699b19edf50de15682221</pre>

   >[!NOTE]
   >
   >* 原始對象是報表的對象：問題
   >* 目標對象為Portfolio。
   >* 連結對象為Project。
   >* 從連結對象引用的目標欄位和指向目標對象的連結欄位為ownerID。
   >* 此處連結對象的對象代碼為PROJ。
   >* 「原始對象」(Original Object)上顯示的「連結欄位」(Linking Field)為projectID，「連結欄位」(Linking Field)為ID。


1. 將上次語句中的目標欄位(ownerID)的值替換為環境中的用戶ID。
1. 按一下 **保存篩選器**。

### 示例2:篩選缺少的對象：未在任何自定義表單中顯示的自定義欄位 {#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms}

使用文本模式介面，可以構建一個過濾器來查看與自定義Forms（類別）不關聯的自定義欄位（參數）。 此篩選器將參數連結到通過另一個對象「類別參數」(Category Parameter)連接的類別。 由於這兩個欄位之間沒有直接連接，並且由於您正在篩選缺少的資訊，因此必須使用EXISTS語句。

>[!IMPORTANT]
>
>「參數」(Parameter)是一個欄位，因為它存在於「自定義表單」中引用的「欄位庫」中。 A Category Parameter是特定窗體上顯示的欄位的版本。 例如，如果在5個窗體上顯示同一欄位，則Workfront資料庫中將有1個參數和5個類別參數。

要篩選未與自定義表單關聯的自定義欄位，請執行以下操作：

1. 建立參數或自定義欄位篩選器。\
   有關建立篩選器的資訊，請參見 [篩選器概述Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)。

1. 按一下 **切換到文本模式**。
1. 請參閱以下通用代碼：

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object>
   ```

   ```
   EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

1. 將以下代碼貼上到 **設定報表的篩選器規則** 替換上述通用代碼：

   <pre>存在:A:$$OBJCODE=CTGYPA<br>存在:A:參數ID=FIELD:ID<br>存在:A:$$EXISTSMOD=NOTEXISTS</pre>

   >[!NOTE]
   >
   >* 原始對象是報表的對象：參數。
   >* 目標對象為類別。
   >* 連結對象是類別參數。
   >* 連結對象的對象代碼為CTGYPA。
   >* 連結到目標對象的連結欄位是parameterID，因為連結對象表和目標對象表中都存在parameterID。
   >* 「原始對象」(Original Object)上顯示的「連結欄位」(Linking Field)為ID(Category Parameter)。


1. 按一下 **保存篩選器**。

### 示例3:篩選缺少的對象：未記錄某段時間的用戶 {#example-3-filter-for-missing-objects-users-who-did-not-log-time-for-a-certain-period-of-time}

使用文本模式介面，可以構建過濾器來查看某個時間段內沒有記錄時間的用戶。 此篩選器將用戶連結到彼此直接連接的小時。 但是，必須使用EXISTS語句和文本模式介面才能篩選缺失的information.information。

要篩選上週未記錄時間的用戶：

1. 建立用戶篩選器。\
   有關建立篩選器的資訊，請參見 [篩選器概述Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)。

1. 按一下 **切換到文本模式**。
1. 請參閱以下通用代碼：

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object><br>
   ```

   ```
   EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

1. 將以下代碼貼上到 **設定報表的篩選器規則** 替換上述通用代碼：

   ```
   EXISTS:A:$$OBJCODE=HOUR<br>EXISTS:A:ownerID=FIELD:ID<br>EXISTS:A:entryDate=$$TODAYb-1w<br>EXISTS:A:entryDate_Range=$$TODAYe-1w<br>EXISTS:A:entryDate_Mod=between<br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

   >[!NOTE]
   >
   >* 原始對象是報表的對象：用戶。
   >* 目標對象為小時。
   >* 在本示例中，您不需要連結對象，因為Users和Hours直接連接在Workfront資料庫中。
   >* 由於沒有連結對象，因此必須使用目標對象的對象代碼：一小時。
   >* 到目標對象的連結欄位為ownerID(顯示在原始對象上；缺少連結對象)。
   >* 原始對象上顯示的連結欄位是ID（小時）(顯示在目標對象上；缺少連結對象。)
   >* EXISTS:A:entryDate語句是指定義目標對象（小時）並使用與常規篩選器語句相同的語法的欄位。 這可確保您只顯示那些在特定時間段（本例中是前一週）內未記錄時間的用戶。
   >* NOTEXISTS修飾符表示我們正在查找報表對象（用戶）不存在的項（小時）。


1. 按一下 **保存篩選器**。

### 示例4:按多個欄位篩選：按Portfolio所有者名稱和Portfolio對齊記分卡ID列出的任務 {#example-4-filter-by-multiple-fields-tasks-by-portfolio-owner-name-and-portfolio-alignment-scorecard-id}

使用文本模式介面，可以構建一個引用目標對象上多個欄位的篩選器。 在這種情況下，引用目標欄位的篩選器語句必須通過AND連接。

例如，您可以篩選任務清單，以僅顯示滿足以下條件的任務：

* 它們位於與其所有者是特定用戶的產品組合關聯的項目中。
* 它們位於與項目組合關聯的項目上，其項目與特定的對齊記分卡未關聯。

要按Portfolio所有者名稱和Portfolio對齊記分卡ID篩選任務：

1. 建立任務篩選器。\
   有關建立篩選器的資訊，請參見 [篩選器概述Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)。

1. 按一下 **切換到文本模式**。
1. 將以下代碼貼上到 **設定報表的篩選器規則** 區域：
   <pre>存在:A:$$OBJCODE=PROJ<br>存在:A:ID=FIELD:projectID<br>存在:A:portfio:ownerID=4d80ce5200000528787d57807732a33f<br>和:A:存在:A:$$EXISTSMOD=NOTEXISTS<br>和:A:存在:A:$$OBJCODE=PROJ<br>和:A:存在:A:ID=FIELD:projectID<br>和:A:存在:A:產品組合：alignmentScoreCardID=4da387b00001cbc732b259355c33dad</pre>

   >[!NOTE]
   >
   >* 原始對象是篩選器的對象：任務。
   >* 目標對象為Portfolio。
   >* 第一個目標欄位是ownerID。
   >* 第二個目標欄位是對齊記分卡ID。
   >* 連結對象為Project。
   >* 連結對象的對象代碼為PROJ。
   >* 到目標對象的連結欄位是(Portfolio的ID)。
   >* 「原始對象」(Original Object)上顯示的「連結欄位」(Linking Field)為projectID。
   >* 將ownerID替換為環境中的用戶ID。


1. 按一下 **保存篩選器**。
