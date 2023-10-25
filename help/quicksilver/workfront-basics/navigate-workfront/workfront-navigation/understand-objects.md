---
content-type: overview;reference
navigation-topic: workfront-navigation
title: 瞭解中的物件 [!DNL Adobe Workfront]
description: 瞭解中的物件 [!DNL Adobe Workfront]
feature: Get Started with Workfront
exl-id: f324f198-5472-4cf2-a46e-7fc24605ca90
source-git-commit: a2650ccc3deffd841a7b497e6ff1b5eed6145211
workflow-type: tm+mt
source-wordcount: '2255'
ht-degree: 7%

---

# 瞭解中的物件 [!DNL Adobe Workfront]

<!--
<***Linked to several articles, do not remove/ change. 
-->

您在中顯示的資訊 [!DNL Adobe Workfront] 由儲存在 [!DNL Workfront] 資料庫。 物件是用來驅動資訊的 [!DNL Workfront].

瞭解在中如何定義物件 [!DNL Workfront] 重要，因此您可以使用正確的物件來滿足組織必要的需求。

例如，當您計畫大量工作時，您需要使用 [!UICONTROL 專案] 物件以定義該工作。 若要將此工作分成較小的計畫增量，您可以使用 [!UICONTROL 任務] 物件。 對於較少量未計畫且可能意外發生的工作，您可以使用Issue物件。 如果您想要追蹤一組專案的進度以及預算與時間表遵守情況，您可以將其組織在 [!UICONTROL Portfolio] 和 [!UICONTROL 計畫]. 若要定義可協助您解決工作的其他元素，您想使用其他儲存在下的物件 [!UICONTROL 專案]， [!UICONTROL 任務]， [!UICONTROL 問題]，或 [!UICONTROL Portfolio]，按一下 [!UICONTROL 檔案]， [!UICONTROL 更新]， [!UICONTROL 小時]， [!UICONTROL 使用者]，或 [!UICONTROL 職位角色].

[!UICONTROL 報表] 和 [!UICONTROL 儀表板] 是另一個物件範例，可協助您組織擁有的資料量 [!DNL Workfront] 視覺化，方便所有使用者存取。

如需中物件的完整清單 [!DNL Workfront]，請參閱 [API總管](../../../wf-api/general/api-explorer.md).

## 物件的相依性和階層

物件會在中相互連結 [!UICONTROL Workfront]. 例如，一個任務或問題不可能在專案之外獨立存在。 [!UICONTROL 任務] 和 [!UICONTROL 問題] 是儲存在 [!UICONTROL 專案] 物件。 [!UICONTROL 任務] 和 [!UICONTROL 問題] 會視為專案的子物件。

以下是一些最常用的物件： [!DNL Workfront] 以及它們各自的父物件和子物件：

| **物件** | **父物件** | **子物件** |
|---|---|---|
| [!UICONTROL 專案組合] |  | [!UICONTROL 計畫]， [!UICONTROL 專案]， [!UICONTROL 檔案]， [!DNL Notes]， [!UICONTROL 使用者] |
| [!UICONTROL 計劃] | [!UICONTROL 專案組合] | [!UICONTROL 專案]， [!UICONTROL 檔案]， [!UICONTROL 附註]， [!UICONTROL 使用者] |
| [!UICONTROL 專案] | [!UICONTROL Portfolio]， [!UICONTROL 計畫] | [!UICONTROL 任務]， [!UICONTROL 問題]， [!UICONTROL 檔案]， [!UICONTROL 附註]， [!UICONTROL 小時]， [!UICONTROL 使用者] |
| [!UICONTROL 任務] | [!UICONTROL 專案] | [!UICONTROL 問題]， [!UICONTROL 子系任務]， [!UICONTROL 檔案]， [!UICONTROL 附註]， [!UICONTROL 小時]， [!UICONTROL 使用者] |
| [!UICONTROL 問題] | [!UICONTROL 任務]， [!UICONTROL 專案] | [!UICONTROL 檔案]， [!UICONTROL 附註]， [!UICONTROL 小時]， [!UICONTROL 使用者] |
| [!UICONTROL 儀表板] |  | [!UICONTROL 報表]，外部頁面 |
| [!UICONTROL 報告] | [!UICONTROL 儀表板] |  |
| [!UICONTROL 群組] |  | [!UICONTROL 使用者] |
| [!UICONTROL 團隊] |  | [!UICONTROL 使用者] |
| [!UICONTROL 使用者] | [!UICONTROL 群組]， [!UICONTROL 團隊]， [!UICONTROL 公司] | [!UICONTROL 職務角色] |
| [!UICONTROL 公司] |  | [!UICONTROL 使用者] |
| [!UICONTROL 文件] | [!UICONTROL 任務]， [!UICONTROL 問題]， [!UICONTROL 專案]， [!UICONTROL Portfolio]， [!UICONTROL 計畫]， [!UICONTROL 使用者] |  |
| [!UICONTROL 計畫]* |  | [!UICONTROL 方案] |
| [!DNL Goals]* |  | [!UICONTROL 結果]， [!UICONTROL 活動] |

如需中物件的完整清單 [!DNL Workfront]，請參閱 [API總管](../../../wf-api/general/api-explorer.md).

*計畫是 [!DNL Adobe Workfront Scenario Planner]. 如需關於的資訊， [!DNL Scenario Planner]，請參閱 [此 [!UICONTROL 情境規劃工具] 概述](../../../scenario-planner/scenario-planner-overview.md).

*[!UICONTROL 目標] 的物件 [!DNL Adobe Workfront Goals]. 如需的相關資訊 [!DNL Workfront Goals]，請參閱 [[!DNL Adobe Workfront Goals] 概述](../../../workfront-goals/goal-management/wf-goals-overview.md).


## 自訂物件名稱

作為 [!DNL Workfront] 管理員，您可以自訂物件名稱於 [!DNL Workfront] 藉由使用  [!UICONTROL 版面配置範本].

如需有關如何使用自訂物件名稱的詳細資訊  [!UICONTROL 版面配置範本]，請參閱 [建立及管理版面範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

自訂版面範本並將其指派給使用者後，這些使用者可以看到物件的自訂名稱。 已指派給版面配置範本的使用者不會再看到Web應用程式中任何位置的物件預設名稱。

>[!NOTE]
>
>為了讓使用者看到物件的新名稱，使用者必須登出並重新登入 [!DNL Workfront] 在您儲存  [!UICONTROL 版面配置範本].

>[!IMPORTANT]
>
>此 [!DNL Workfront] 檔案一律參照物件的預設名稱。 作為 [!DNL Workfront] 管理員，請務必通知使用者物件名稱的變更，以便他們瞭解如何使用 [!DNL Workfront] 檔案以及未反映物件名稱變更的應用程式區域。

* [可使用自訂的物件名稱  [!UICONTROL 版面配置範本]](#object-names-that-can-be-customized-using-a-layout-template)
* [區域 [!DNL Workfront] 反映自訂物件名稱的](#areas-of-workfront-that-reflect-the-customized-object-names)
* [區域 [!DNL Workfront] 無法反映自訂物件名稱的](#areas-of-workfront-that-do-not-reflect-the-customized-object-names)

### 可使用自訂的物件名稱 [!UICONTROL 版面配置範本]

作為 [!DNL Workfront] 管理員，您可以自訂下列物件的名稱，以符合組織中的術語：

* [!UICONTROL 專案組合]
* [!UICONTROL 方案]
* [!UICONTROL 專案]
* [!UICONTROL 任務]
* [!UICONTROL 問題]
* [!UICONTROL 目標]*
* [!UICONTROL 結果]*
* [!UICONTROL 活動]*

  *[!UICONTROL 目標]， [!UICONTROL 個結果]、和 [!UICONTROL 活動] 僅適用於貴公司已購買的 [!DNL Workfront Goals]. 如需的相關資訊 [!DNL Workfront Goals]，請參閱 [[!DNL Adobe Workfront Goals] 概述](../../../workfront-goals/goal-management/wf-goals-overview.md).

* [!UICONTROL 行動方案]**
* [!UICONTROL 情境]**
* [!UICONTROL 計劃]**

  **[!UICONTROL 行動方案]， [!UICONTROL 情境]、和 [!UICONTROL 計畫] 只有在貴公司購買 [!DNL Workfront Scenario Planner]. 如需關於的資訊， [!DNL Scenario Planner]，請參閱 [開始使用 [!DNL Scenario Planner]](../../../scenario-planner/get-started-with-scenario-planning.md).


例如，如果貴組織中較大量的工作稱為「參與」，您可以取代名稱「[!UICONTROL 專案]&#39;具有&#39;Engagement&#39;。 您的 [!DNL Workfront] 介面會顯示「參與」而非「[!UICONTROL 專案]&#39;只要有名稱&#39;[!UICONTROL 專案]「 」會出現。

有關如何使用自訂物件名稱的詳細資訊  [!UICONTROL 版面配置範本]，請參閱 [建立及管理版面範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

您無法在Workfront中自訂任何其他物件的名稱。 如需中物件的完整清單 [!DNL Workfront]，請參閱 [API總管](../../../wf-api/general/api-explorer.md).

當您自訂物件的名稱時，該物件的新名稱會出現在大部分割槽域 [!DNL Workfront] 顯示物件名稱的應用程式。

### 區域 [!DNL Workfront] 反映自訂物件名稱的

下列區域顯示物件的更新名稱：

* 上方巡覽
* 左側面板導覽中的所有區段
* 所有功能表
* 應用程式內通知
* Report Builder和報告元素（檢視、篩選器和群組）
* [!UICONTROL 儲存] 按鈕
* 匯出的檔案
* 電子郵件
* 行動應用程式

### 區域 [!DNL Workfront] 無法反映自訂物件名稱的

下列區域不會顯示物件的更新名稱：

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Referenced Object Type selection for a Typeahead field in a Custom Form </p> <p>(NOTE: drafting this because I don't think this is true)</p> </li>
  -->

* [!DNL Outlook] 增益集

### 自訂物件名稱的影響

在中自訂物件名稱時，請注意下列事項 [!DNL Workfront]：

* 您可能在系統顯示中遇到文體或文法錯誤。 例如，如果您重新命名「[!UICONTROL 問題]&#39;變成&#39;Request&#39;，而您在系統中的任何位置看到&#39;An request&#39;這個片語，就如預期般運作，不應視為錯誤。
* 您物件的自訂名稱無法翻譯。 僅限 [!DNL Workfront] 預設名稱可以翻譯成支援的語言。 如需支援的語言詳細資訊，請參閱 [!DNL Workfront]，請參閱 [中支援的語言 [!DNL Adobe Workfront]](../../../workfront-basics/supported-languages-in-workfront.md). 自訂物件名稱欄位支援外來字元，因此您可以用任何語言輸入術語。
* 當您使用自訂物件名稱時  [!UICONTROL 版面配置範本]，建議您將  [!UICONTROL 版面配置範本] 在您的業務單位（團隊或群組）周圍。\
   建議您使用這些業務單位使用者清楚理解的名稱，以避免混淆。
* 電子郵件通知與傳送的報表一律會包含由定義的物件名稱。  [!UICONTROL 版面配置範本] 產生電子郵件的使用者的檔案。 如果您的使用者收到其他團隊和群組使用者的電子郵件通知，則您使用者應該準備好在其電子郵件中看到與群組或團隊無關的物件名稱。\
   作為 [!DNL Workfront] 管理員，建議使用者注意與每個物件相關聯的圖示。 各種物件名稱之間的圖示會維持一致，與預設物件一致，如顯示在資料庫中的圖示一樣。 針對所有清單 [!DNL Workfront] 與物件關聯的圖示，請參閱 [物件圖示](#object-icons).

  >[!TIP]
  >
  >對於組織中的常見工作，請考慮建立自訂檔案以反映您的術語。

## 物件圖示

此 [!DNL Workfront] 檔案一律參照物件的預設名稱。 如果您的物件已自訂其名稱，您可以依賴與其關聯的圖示來瞭解哪個自訂物件對應到哪個物件 [!DNL Workfront] 預設物件。

如需哪些物件可以有自訂名稱的詳細資訊， [!DNL Workfront]，請參閱 [可使用自訂的物件名稱  [!UICONTROL 版面配置範本]](#object-names-that-can-be-customized-using-a-layout-template).

以下是Workfront中的物件清單及其對應的圖示。

| **物件** | **圖示** | **可自訂的物件名稱** |
|---|---|---|
| [!UICONTROL 公司] | ![](assets/company-icon-nwe.png)  , ![](assets/nwe-company-icon-54x54.png) |  |
| [!UICONTROL 儀表板] | ![](assets/dashboard-icon-nwe.png)  , ![](assets/nwe-dashboards-icon.png) |  |
| [!UICONTROL 目標] | ![](assets/nwe-goal-icon.png) | ✔ |
| [!UICONTROL 群組] | ![](assets/groups-icon-nwe.png)  , ![](assets/nwe-group-icon.png) |  |
| [!UICONTROL 問題] | ![](assets/issue-icon-nwe.png)  , ![](assets/nwe-issues-icon.png) | ✔ |
| [!UICONTROL 職務角色] | ![job_role_icon.png](assets/job-role-icon-52x50.png)， ![job_role_icon__1_.png](assets/job-role-icon--1--53x44.png)， ![](assets/job-role-nwe-no-color.png)， ![](assets/job-role-icon-nwe-color.png) |  |
| [!UICONTROL 計劃] | ![](assets/plan-icon.png), ![](assets/nwe-plan-icon-60x57.png) |  |
| [!UICONTROL 專案組合] | ![](assets/portfolio-icon-nwe.png)  , ![](assets/nwe-portfolios-icon.png) | ✔ |
| [!UICONTROL 方案] | ![](assets/program-icon-nwe.png)  , ![](assets/nwe-programs-icon.png) | ✔ |
| [!UICONTROL 專案] | ![](assets/project-icon-nwe.png)  , ![](assets/nwe-projects-icon.png) | ✔ |
| [!UICONTROL 報告] | ![](assets/report-icon-nwe.png) , ![](assets/nwe-reports-icon.png) |  |
| [!UICONTROL 任務] | ![](assets/task-icon-new.png)  , ![](assets/nwe-tasks-icon.png) | ✔ |
| [!UICONTROL 團隊] | ![](assets/team-icon-nwe.png), ![](assets/team-icon-nwe-color.png) , ![](assets/nwe-teams-icon.png) |  |
| [!UICONTROL 範本] | ![](assets/template-icon-nwe.png)  , ![](assets/nwe-templates-icon.png) |  |

## 物件的參考編號

在中建立的每個物件 [!DNL Workfront] 會指定一個唯一的參考號碼。 在區分兩個在其他方面相似的物件（例如具有相同名稱的工作）時，參考編號非常有用。 您可以使用物件的參考編號來搜尋物件，也可以在報表中包含參考編號。

如需有關如何按參考編號搜尋物件的資訊，請參閱 [使用物件的參考編號](../../../workfront-basics/navigate-workfront/search/reference-number-of-objects.md).

## 物件特定搜尋

您可以搜尋所有可在中搜尋的物件 [!DNL Workfront]，或者您可以在基本和進階搜尋中選取要搜尋的特定物件。

並非所有物件都可在中搜尋 [!DNL Workfront]. 您可以對下列物件執行基本和進階搜尋： [!DNL Workfront]：

| **物件** | **基本搜尋** | **高級搜尋** |
|---|---|---|
| [!UICONTROL 專案] | ✓ | ✓ |
| [!UICONTROL 任務] | ✓ | ✓ |
| [!UICONTROL 問題] | ✓ | ✓ |
| [!UICONTROL 報告] | ✓ | ✓ |
| [!UICONTROL 使用者] | ✓ | ✓ |
| [!UICONTROL 範本] | ✓ | ✓ |
| [!UICONTROL 文件] | ✓ | ✓ |
| [!UICONTROL 專案組合] | ✓ | ✓ |
| [!UICONTROL 計劃] | ✓ | ✓ |
| [!UICONTROL 儀表板] | ✓ | ✓ |
| [!UICONTROL 公司] | ✓ | ✓ |
| [!UICONTROL 附註] (或 [!UICONTROL 更新]) | ✓ |  |

有關執行基本和進階搜尋的詳細資訊，請參閱 [!DNL Workfront]，請參閱 [搜尋 [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

## 物件報表

在您開始在中建立報表之前，瞭解物件的階層與相依性是極為重要的 [!DNL Workfront]. 報表是物件專屬的。 您必須先為報表選取正確的物件，才能顯示您想要的資料。

根據您為報表選取的物件，您只能存取直接連結至報表物件的物件。

>[!IMPORTANT]
>
>您只能在同一個報表中報告您選取的物件以及父物件。 父物件報表中不能有子物件的相關資訊。 例如，您可以在任務報告中顯示專案資訊，但不能在專案報告中顯示任務資訊。

您可以使用我們的開放API來報告資料庫中的所有物件。 如需資料庫中所有物件的完整清單，請參閱 [API總管](../../../wf-api/general/api-explorer.md).

>[!NOTE]
>
>如果您已使用版面配置範本自訂物件名稱，則也會自訂Report Builder中的物件名稱。 確保您知道哪些物件已自訂，並在Report Builder中尋找自訂名稱。 如需哪些物件可以有自訂名稱的詳細資訊， [!DNL Workfront]，請參閱 *[可使用自訂的物件名稱  [!UICONTROL 版面配置範本]](#object-names-that-can-be-customized-using-a-layout-template).*
>在報表中使用文字模式時，文字模式運算式中的物件名稱為中的標準名稱。 [!DNL Workfront]，而非自訂物件名稱。 如需有關在報表中使用文字模式的詳細資訊，請參閱 [文字模式概觀](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

如需建立報表的詳細資訊，請參閱 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).\
如需關於我們API的詳細資訊，請參閱 [API總管](../../../wf-api/general/api-explorer.md).

在中使用Report Builder時，您可以報告下列物件 [!DNL Workfront] 網頁應用程式：

* [!UICONTROL 專案]
* [!UICONTROL 任務]
* [!UICONTROL 小時]
* [!UICONTROL 問題]
* [!UICONTROL 使用者]
* [!UICONTROL 存取層級]
* [!UICONTROL 核准]
* [!UICONTROL 核准流程]
* [!UICONTROL 指派]
<!--this is no longer available: * [!UICONTROL Backlog Work Item]\
   Displays tasks or issues on the agile backlog. For more information about the agile backlog, see [Manage the agile backlog](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).-->

* [!UICONTROL 基準線]
* [!UICONTROL 基準線任務]
* [!UICONTROL 付費記錄]
* [!UICONTROL 已編列預算時數]

  這是 [!UICONTROL 已編列預算時數]，如舊版已棄用的資源管理工具中的所示。

  「Bud. 「小時」欄位 [!UICONTROL 已編列預算小時] 報告指標對工作角色預算的時數 [!UICONTROL 資源規劃工具]. 如需詳細資訊，請參閱 [瞭解 [!UICONTROL 預算勞力成本] 和 [!UICONTROL 已編列預算時數] 針對專案](../../../manage-work/projects/project-finances/budgeted-labor-cost.md).

* [!UICONTROL 行事曆事件]
* [!UICONTROL 公司]
* [!UICONTROL 自訂表單]
* [!UICONTROL 儀表板]
* [!UICONTROL 文件]
* [!UICONTROL 文件核准]
* [!UICONTROL 文件版本]\
   您可以檢視檔案版本的相關資訊、與版本相關聯的檔案、建立版本的使用者，以及在檔案版本上建立校訂的使用者（校訂建立者）（如果存在）。
* [!UICONTROL 電子郵件範本]
* [!UICONTROL 費用]
* [!UICONTROL 費用類型]
* [!UICONTROL 外部頁面]
* [!UICONTROL 加入最愛]
* [!UICONTROL 篩選器]
* [!UICONTROL 目標]

  您可以為策略目標建立報告，或在專案與目標關聯作為目標活動時，可在專案報告中顯示目標相關的資訊。 只有貴組織已購買策略目標並連線專案，您才能建立策略目標並連線專案 [!DNL Workfront Goals] 授權。 如需的相關資訊 [!DNL Workfront Goals]，請參閱 [[!DNL Workfront Goals] 概述](../../../workfront-goals/goal-management/wf-goals-overview.md). 如需有關將專案連線至策略目標的資訊，請參閱 [在Adobe Workfront目標中新增專案](../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

  >[!TIP]
  >
  >您無法報告與關聯的專案目標 [!UICONTROL 業務案例]. 如需專案目標與策略目標的相關資訊，請參閱 [字彙表 [!DNL Adobe Workfront] 術語](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* [!UICONTROL 群組]
* [!UICONTROL 分組]
* [!UICONTROL 時數類型]
* [!UICONTROL 行動方案]

  如果行動方案是計畫的子物件，且貴公司已購買，您才可以為這些行動方案建立報表。 [!DNL Workfront Scenario Planner] 授權。 如需方案的相關資訊，請參閱 [中的方案概觀 [!DNL Workfront Scenario Planner]](../../../scenario-planner/initiatives-overview.md).


* 計畫工作角色

  只有貴公司已購買，您才能為計畫中方案相關的工作角色建立報告 [!DNL Workfront Scenario Planner] 授權。 如需建立方案並將其與工作角色建立關聯的資訊，請參閱 [在中建立和編輯方案 [!DNL Workfront Scenario Planner]](../../../scenario-planner/create-and-edit-initiatives.md).


* [!UICONTROL 反覆項目]
* [!UICONTROL 職務角色]
* [!UICONTROL 日誌輸入項目]

  您可在以下位置報告追蹤的系統更新： [!UICONTROL 更新] 任務、專案、問題等物件區域。 若要深入瞭解，請參閱 [報告 [!UICONTROL 更新] 區域](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

* [!UICONTROL 版面配置範本]
* [!UICONTROL 里程碑]
* [!UICONTROL 里程碑路徑]
* [!UICONTROL 注意] 或 [!UICONTROL 更新]

  >[!NOTE]
  >
  >您可以報告個別使用者新增的註解。

* [!UICONTROL 引數] (或 [!UICONTROL 自訂欄位])
* [!UICONTROL 引數群組] (或 [!UICONTROL 分割槽符號])
  <!--this is no longer in the UI: * [!UICONTROL Portal Profile] (this displays information that has been deprecated)-->
* [!UICONTROL 專案組合]
* [!UICONTROL 方案]
* [!UICONTROL 專案] ([!UICONTROL 財務資料])

  >[!NOTE]
  >
  >財務資訊填入 [!UICONTROL 專案] ([!UICONTROL 財務資料])僅會在與其關聯的資料存在時間少於5年時報告。 例如，如果某個工作角色在2015年1月被分配給某個任務，而今天是2021年9月，則財務歸檔如下 [!UICONTROL 分配日期] （表示工作角色未填入） [!UICONTROL 專案（財務資料）] 報告。

* [!UICONTROL 校訂核准]\
   可讓您檢視關於校訂核准的各種資訊，包括：已提交核准的校訂、關於核准的資訊 [!UICONTROL 核准者]，要求者的相關資訊（如果要求者已獲授權） [!DNL Workfront] 使用者)、版本資訊、校訂ID和校訂建立日期。\
   [!UICONTROL 校訂核准] 報表僅包含可在使用者的「我的工作」區域中使用的校訂，這些區域尚未做出決定。\
   校訂核准指派於 [!DNL Workfront] 如說明 [將使用者新增到校訂](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) 在 [在中共用校訂 [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

* [!UICONTROL 佇列]
* [!UICONTROL 佇列主題]
* [!UICONTROL 評等] (這會顯示工作角色 [!UICONTROL 收費率] 資訊)
* [!UICONTROL 提醒通知]
* [!UICONTROL 報告]
* [!UICONTROL 資源集區]
* [!UICONTROL 風險]
* [!UICONTROL 風險類型]
* [!UICONTROL 排程]
* [!UICONTROL 計分卡]
* [!UICONTROL 團隊]
* [!UICONTROL 範本]
* [!UICONTROL 範本任務]
* [!UICONTROL 休假]

  您可以根據使用者在其設定檔中的指示，報告使用者的休假。

* [!UICONTROL 時程表]
* [!UICONTROL 時間表設定檔]
* [!UICONTROL 主題群組]
* [!UICONTROL 使用者核准]
* [!UICONTROL 使用者委派]

  您可以報告受委派執行外出時其他人之任務和問題的使用者。 此報表顯示不在辦公室的使用者以及在外出期間履行職責的使用者。

* [!UICONTROL 使用者決策]

  您可以報告當月使用者對校樣和檔案做了多少決策。

* [!UICONTROL 檢視]
* [!UICONTROL 工作專案] （這會產生任務和問題報告）
