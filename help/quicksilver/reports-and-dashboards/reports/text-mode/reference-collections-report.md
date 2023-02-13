---
product-area: reporting
navigation-topic: text-mode-reporting
title: 在報表中參考集合
description: 在報表中參考集合
author: Nolan
feature: Reports and Dashboards
exl-id: 18ba3f4b-ae03-4694-a2fe-fdbeeb576ea9
source-git-commit: 8b6324302a70319f387d1e09d1eb92fbdabf7e32
workflow-type: tm+mt
source-wordcount: '2609'
ht-degree: 0%

---

# 在報表中參考集合

在Adobe Workfront中建立報表可讓您在清單、格線或圖表格式中顯示一組物件、其個別欄位或連結物件。

如需在Workfront中建立報表的詳細資訊，請參閱 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

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
   <td> <p>編輯對篩選器、檢視、群組的存取</p> <p>編輯對報表、控制面板、日曆的存取</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理報表權限</p> <p>管理檢視、篩選或分組的權限 </p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 了解集合

集合是連結到另一個對象的對象清單。

Workfront中的物件之間有下列兩種關係：

* **一對一關係**:一次只能將一個對象連結到另一個對象。\
   例如，一個專案一次只能連結至一個產品組合。

* **一對多關係**:一個對象一次可以連結到多個其他對象。\
   例如，一個專案可以有多個工作。 在此案例中，任務清單會形成專案的集合。

>[!IMPORTANT]
>
>您可以使用標準的報告建立工具，建立顯示物件之間一對一關係的報告。 不過，您只能使用報告建立工具中的文字模式介面，以建立顯示物件之間一對多關係的報告。

如需在標準報告建立工具中建立報告的詳細資訊，請參閱 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

如需使用文字模式介面建立報表的詳細資訊，請參閱：

* [文字模式概觀](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [文字模式常見用途概觀](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).
* [文字模式語法概觀](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)

## 在API資源管理器中查找集合對象及其欄位 {#find-collection-objects-and-their-fields-in-the-api-explorer}

並非所有集合都可以報告。

若要了解哪些物件可與其他物件的集合相關聯，您必須使用API Explorer。\
如需API總管表格的詳細資訊，請參閱 [API Explorer](../../../wf-api/general/api-explorer.md).

要了解可以報告哪些集合，請執行以下操作：

1. 前往 [API Explorer](../../../wf-api/general/api-explorer.md).
1. 尋找報表的物件。
1. 選取 **集合** 標籤。

   >[!NOTE]
   >
   >只有此標籤上列出的對象才能在所選對象的報告中以集合的形式表示。

1. 按一下集合的物件，以展開該物件。
1. 按一下顯示的連結，前往集合的物件。\
   這會開啟 **欄位** 標籤。

   >[!NOTE]
   >
   >只有此頁簽上列出的欄位在集合報表中可被引用，或與此頁簽上列出的對象關聯的欄位。

## 報表中的參考集合

您可以在下列報表元素中參照集合中的物件：

* 檢視
* 篩選器
* 提示

不能從以下報表元素中的集合引用對象：

* 群組
* 圖表

例如，您可以從項目報告中參考任務或發放集合，以顯示項目級別的任務或發放資訊。

* [在報表檢視中參考集合](#reference-a-collection-in-the-view-of-a-report)
* [在報表篩選器中參考集合](#reference-a-collection-in-the-filter-of-a-report)
* [在報表的自訂提示中參考集合](#reference-a-collection-in-the-custom-prompt-of-a-report)

### 在報表檢視中參考集合 {#reference-a-collection-in-the-view-of-a-report}

您可以在報表檢視中參考物件集合，以顯示與報表物件相關聯的物件屬性。

例如，您可以在專案報表的檢視中建立任務或問題的收集欄，借此在專案報表中顯示任務或問題資訊。

您可以在收集檢視中顯示有關工作或問題的資訊，例如名稱、日期、主要受分配者、完成百分比等。

視圖以清單格式顯示任務或問題資訊，清單的每一行代表有關任務或問題的資訊。 任務或問題清單及其欄位與任務或問題所屬項目的同一行顯示。\
![issue_and_tasks_collections_in_reports.png](assets/issue-and-tasks-collections-in-reports-350x171.png)

* [在報表檢視中新增集合欄](#add-a-collection-column-in-a-report-view)
* [了解文本模式下集合視圖的行](#understand-the-lines-of-a-collection-view-in-text-mode)
* [集合檢視的限制](#limitations-of-a-collection-view)

### 在報表檢視中新增集合欄 {#add-a-collection-column-in-a-report-view}

若要在報表檢視中新增集合欄：

1. 按一下 **主要** 功能表 ![](assets/main-menu-icon.png)，然後按一下 **報表**.
1. 按一下 **新增報表**.
1. 選取報表的物件。
1. 從報表導覽離開，並使用 [API Explorer](../../../wf-api/general/api-explorer.md)，決定您為報表選取的物件可使用的集合。

   如需選取集合物件的詳細資訊，請參閱區段 [在API資源管理器中查找集合對象及其欄位](#find-collection-objects-and-their-fields-in-the-api-explorer) 這篇文章。\
   記下集合的物件名稱。

1. 使用 [API Explorer](../../../wf-api/general/api-explorer.md)，移至您要在集合中顯示之物件的欄位清單。

   如需尋找集合物件欄位的詳細資訊，請參閱區段 [在API資源管理器中查找集合對象及其欄位](#find-collection-objects-and-their-fields-in-the-api-explorer) 這篇文章。

   記下您要在集合中顯示的欄位名稱。

1. 導覽回您的報表，並在 **欄（檢視）** 按一下 **添加列**.
1. 按一下 **切換到文本模式**.
1. 將滑鼠移到對話方塊上，然後按一下 **按一下「 」以編輯文字**.
1. 選取 **文字模式** 對話框，然後將其刪除，如果要引用集合對象的欄位，則貼上以下代碼：

   ```
   valueformat=HTML
   textmode=true
   type=iterate
   listdelimiter=<p>
   displayname=Column Name
   listmethod=nested(collection object name).lists
   valuefield=collection object field
   ```

1. 取代 **欄名稱** 欄的名稱 `displayname` 行。
1. 取代 **集合對象名稱**，且 `listmethod` 行，如 [API Explorer](../../../wf-api/general/api-explorer.md).

1. 取代 **集合對象欄位** ，且 `valuefield` 行，如 [API Explorer](../../../wf-api/general/api-explorer.md).

   您可以取代 **valuefield** with **valueexpression**，以便在檢視中建立自訂運算式。

   如需計算自訂運算式的詳細資訊，請參閱 [計算資料運算式](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

   例如，如果要在專案報表中顯示任務清單。 此集合使用 `valuefield` 行，用於引用任務的名稱。

   執行下列任一項作業：

   * 使用下列程式碼建立欄：

      ```
      valueformat=HTML
      textmode=true
      type=iterate
      listdelimiter=<p>
      displayname=Project Tasks Names
      listmethod=nested(tasks).lists
      valuefield=name
      ```

   * 使用下列程式碼來顯示報表中的問題清單：

      ```
      displayname=Project Issues Names
      listdelimiter=<p>
      listmethod=nested(issues).lists
      textmode=true
      type=iterate
      valuefield=name
      valueformat=HTML
      ```

      請注意，在集合中，您必須使用 **問題** 針對 **listmethod** 行，而非 **opTasks** 即問題的資料庫名稱。 如需使用時機的相關資訊 **問題** 和使用時機 **opTask** 當提及問題時，請參閱 [參考問題時，請使用「opTask」和「issue」](../../../manage-work/issues/issue-information/use-optask-instead-of-issue.md).

   * 如果要在項目報告中顯示任務清單及其主要受託人，請使用 **valueexpression** 用於引用與其主要任務名稱相鄰的任務名稱而不是其主要任務名稱的行 **valuefield**.

      使用下列程式碼建立欄：

      ```
      valueformat=HTML
      textmode=true
      type=iterate
      listdelimiter=<p>
      displayname=Tasks Names - Primary Assignee
      listmethod=nested(tasks).lists
      valueexpression=CONCAT({name},' - ',{assignedTo}.{name})
      ```

1. 下列欄會顯示在專案報表中，列出每個專案中的所有工作及其主要指派者：

   ![](assets/project-report-with-task-and-assignee-collection-view-nwe-350x222.png)

1. 按一下&#x200B;**儲存**。
1. （選用）繼續編輯報表。

   或

   按一下 **儲存+關閉** 以儲存報表。

#### 了解文本模式下集合視圖的行

下表列出集合的文本模式視圖中的行：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>範例行</strong> </th> 
   <th><strong>說明</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><code>valueformat=HTML</code> </td> 
   <td> <p>您可以對此行使用各種值，但建議您 <code style="font-weight: normal;">valueformat</code> 的 <strong>HTML。</strong></p>
   </td> 
  </tr> 
  <tr> 
   <td><code>textmode=true</code> </td> 
   <td> <p>此行表示該列已使用文本模式進行配置。 如果您移除此行，Workfront會依預設將其新增回。</p> </td> 
  </tr> 
  <tr> 
   <td><code>type=iterate</code> </td> 
   <td> <p>此 <code>type</code> 總是 <code>iterate</code>，建置檢視時。</p> </td> 
  </tr> 
  <tr> 
   <td><code>listdelimiter=&lt;p&gt;</code> </td> 
   <td> <p>這是用來分隔清單中值的分隔字元。<br>建議您使用 <code>&lt;p&gt;</code> 會在值之間加上分行符號。</p> <p>您也可以使用下列項目：</p> <p><code>&amp;zwj;</code> （零寬接合器）。 集合的值之間沒有分隔。<br><strong>,</strong> =逗號分隔符。 集合的值以逗號分隔，後面接著沒有空格。<br><strong>/</strong> =斜線分隔符號。 集合的值以斜線分隔。<br><strong>-</strong> =破折號分隔符號。 集合的值以破折號分隔。<br>依預設，將此行保留空白會在集合的值之間新增逗號，後面加上空格。</p> </td> 
  </tr> 
  <tr> 
   <td><code>displayname=</code><em>欄名稱</em> </td> 
   <td> <p>取代 <strong>欄名稱</strong> 新欄的實際名稱。</p> </td> 
  </tr> 
  <tr> 
   <td><code>listmethod=nested(collection object name).list</code> </td> 
   <td> <p> 此行會定義您所參考的集合。</p> <p>取代 <strong>集合對象名稱</strong> 名稱，如 <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>. 此值通常是集合物件名稱的複數形式。</p> </td> 
  </tr> 
  <tr> 
   <td><code>valuefield=collection object field</code> </td> 
   <td> <p>此行定義您要從集合物件參考的欄位。</p> <p>取代 <strong>集合對象欄位</strong> 名稱，如 <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p> <p>您可以將此行取代為：</p> <p><strong>valueexpression</strong>=計算的集合對象欄位/欄位</p> <p>使用 <strong>valueexpression</strong>，您可以在欄中顯示計算的自訂運算式。</p> <p>如需格式化的詳細資訊 <strong>valueexpression</strong> 線條，請參閱 <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">文字模式語法概觀</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### 集合檢視的限制 {#limitations-of-a-collection-view}

建立集合檢視時，請考量下列限制：

* 您無法控制收集資料的顯示順序。
* 您無法將條件式格式套用至集合檢視。
* 您無法將集合中的物件設為可點按的連結。
* 您無法建立其他集合的集合檢視。\
   例如，您無法顯示項目報告中每個任務的所有受分配者。 您只能在專案檢視的每個任務上顯示主要受託人。

### 在報表篩選器中參考集合 {#reference-a-collection-in-the-filter-of-a-report}

您可以在報表的篩選器中參考物件集合，以篩選與報表物件相關聯的物件屬性。

例如，您可以在篩選語句中使用對項目上任務或問題屬性的引用來篩選項目報告中的任務或問題資訊。

若要在報表篩選器中新增參考至集合：

1. 按一下 **主要** 功能表 ![](assets/main-menu-icon.png)，然後按一下 **報表**.
1. 按一下 **新增報表**.
1. 選取報表的物件。
1. 從報表導覽離開，並使用 [API Explorer](../../../wf-api/general/api-explorer.md)，決定您為報表選取的物件可使用的集合。

   如需選取集合物件的詳細資訊，請參閱區段 [在API資源管理器中查找集合對象及其欄位](#find-collection-objects-and-their-fields-in-the-api-explorer) 這篇文章。

   記下集合的物件名稱。

1. 使用 [API Explorer](../../../wf-api/general/api-explorer.md)，移至您要在集合中顯示之物件的欄位清單。

   如需尋找集合物件欄位的詳細資訊，請參閱區段 [在API資源管理器中查找集合對象及其欄位](#find-collection-objects-and-their-fields-in-the-api-explorer) 這篇文章。

   記下您要在集合中顯示的欄位。

1. 導覽回您的報表，並在 **篩選器** 按一下 **切換到文本模式**.

1. 在 **設定報表的篩選規則** 區域，貼上下列程式碼：

   ```
   collection object name:collection object field=collection object value
   collection object name:collection object field_Mod=value of the modifier
   ```

1. 取代 **集合對象名稱** 的名稱，如 [API Explorer](../../../wf-api/general/api-explorer.md). 此值通常是集合物件名稱的複數形式。

1. 取代 **集合對象欄位** 中集合物件的欄位名稱，如 [API Explorer](../../../wf-api/general/api-explorer.md).

1. 取代 **集合對象值** 和集合物件的值，如Workfront中顯示。
1. 取代 **修飾詞的值** 填入有效的修飾詞。

   有關修改量清單，請參閱 [篩選條件修飾元](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).\
   例如，若要建立專案報表，只顯示名稱有「行銷」之工作的專案，請使用下列程式碼：

   ```
   tasks:name=Marketing
   tasks:name_Mod=cicontains
   ```

   此報表只會顯示至少有一個任務名稱中包含「行銷」字樣的專案。

   ![](assets/marketing-only-tasks-in-project-report-nwe-350x309.png)

1. 若要篩選問題名稱，請使用下列程式碼：

   ```
   issues:name=Marketing
   issues:name_Mod=cicontains
   ```

   >[!TIP]
   >
   >請注意，您必須使用 `issues` （而非） `optask` 問題在API Explorer中的顯示方式。

1. 按一下 **完成**.
1. （選用）繼續編輯報表。

   或

   按一下 **儲存+關閉** 以儲存報表。

### 在報表的自訂提示中參考集合 {#reference-a-collection-in-the-custom-prompt-of-a-report}

您可以在報表的自定義提示中引用對象的集合，以篩選報表結果中與報表對象關聯的對象的屬性。

例如，在報表的自訂提示中，您可以使用對專案上任務屬性的參考，來提示專案報表中的任務資訊。

>[!NOTE]
>
>無法在標準提示中引用集合。

自訂提示是自訂篩選器，其中會使用&amp;符號聯結陳述式。 建議您先在篩選器中建立陳述式，然後使用&amp;符號連結陳述式的行。

有關使用集合引用建立篩選語句的詳細資訊，請參閱 [在報表篩選器中參考集合](#reference-a-collection-in-the-filter-of-a-report) 這篇文章。

若要在報表的自訂提示中新增參考至集合：

1. 按一下 **主要** 功能表 ![](assets/main-menu-icon.png)，然後按一下 **報表**.
1. 按一下 **新增報表**.
1. 選取報表的物件。
1. 使用集合參考建立篩選器，如區段所述 [在報表篩選器中參考集合](#reference-a-collection-in-the-filter-of-a-report) 這篇文章。
1. 按一下 **報表設定**.
1. 按一下 **報表提示**.
1. 按一下 **添加提示**.
1. 按一下 **自訂提示**.
1. 在 **欄位****名稱** 欄位。

1. 指定 **下拉式項目標籤**.
1. 在 **條件** 欄位：

   ```
   collection object name:collection object field_Mod=value of the modifier
   ```

1. （可選）指定此選項預設顯示在提示中。
1. 取代 **集合對象名稱** 的名稱，如 [API Explorer](../../../wf-api/general/api-explorer.md). 此值通常是集合物件名稱的複數形式。
1. 取代 **集合對象欄位** 和集合物件欄位的名稱，如 [API Explorer](../../../wf-api/general/api-explorer.md).
1. 取代 **集合對象值** 和集合物件的值，如Workfront中顯示。

   例如，如果您要篩選任務名稱包含「行銷」的專案，請取代 **集合對象值** with **行銷**.

1. 取代 **修飾詞的值** 填入有效的修飾詞。

   有關修改量清單，請參閱  [篩選條件修飾元](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   **範例：** 例如，若要建立包含自訂提示的專案報表，而您只想顯示指派給特定使用者至少一項任務的專案，請使用下列程式碼：

   ```
   tasks:assignedToID=57cf1b7a000077c9f02f66cb09c8f86c&tasks:assignedToID_Mod=in
   ```

   這會產生一個報告，列出的所有項目都至少為GUID為57cf1b7a000077c9f02f66cb09c8f86c的用戶分配了一個任務。

   >[!NOTE]
   >
   >根據 [API Explorer](../../../wf-api/general/api-explorer.md). 您只能參考主要受託人的ID。

   例如，若要篩選任何將任何專案問題指派給特定使用者的專案，請針對自訂提示使用下列程式碼：

   ```
   issues:assignedToID=57cf1b7a000077c9f02f66cb09c8f86c&issues:assignedToID_Mod=in
   ```

   這會產生一份報告，列出的所有專案至少會為GUID為57cf1b7a000077c9f02f66cb09c8f86c的使用者指派一個問題。

   >[!NOTE]
   請注意，您必須使用 **問題** （用於集合對象名稱）。 目前，API總管未針對問題提供集合物件名稱。

1. 按一下 **完成**.
1. （選用）繼續編輯報表。

   或

   按一下 **儲存+關閉** 以儲存報表。
