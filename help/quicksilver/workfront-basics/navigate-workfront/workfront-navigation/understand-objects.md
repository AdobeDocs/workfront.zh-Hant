---
content-type: overview;reference
navigation-topic: workfront-navigation
title: 瞭解中的對象 [!DNL Adobe Workfront]
description: 瞭解中的對象 [!DNL Adobe Workfront]
feature: Get Started with Workfront
exl-id: f324f198-5472-4cf2-a46e-7fc24605ca90
source-git-commit: 888c938e5d649557df69374a55d4e4ecc2da6f55
workflow-type: tm+mt
source-wordcount: '2263'
ht-degree: 6%

---

# 瞭解中的對象 [!DNL Adobe Workfront]

<!--
<***Linked to several articles, do not remove/ change. 
-->

您在中顯示的資訊 [!DNL Adobe Workfront] 由儲存在 [!DNL Workfront] 資料庫。 這些對象是驅動資訊的 [!DNL Workfront]。

瞭解對象在中的定義方式 [!DNL Workfront] 非常重要，因此您可以根據組織中的需要使用正確的對象。

例如，在計畫大量工作時，需要使用 [!UICONTROL 項目] 定義該工作的對象。 要將此工作分為較小的計畫增量，可以使用 [!UICONTROL 任務] 的雙曲餘切值。 對於未計畫且可能意外發生的較小工作量，可以使用「問題」對象。 如果要跟蹤一組項目的進度和對預算和時間表的遵守情況，可以在 [!UICONTROL Portfolio] 和 [!UICONTROL 程式]。 要定義幫助您解決工作的其他元素，您需要使用儲存在 [!UICONTROL 項目]。 [!UICONTROL 任務]。 [!UICONTROL 問題]或 [!UICONTROL Portfolio]，例如 [!UICONTROL 文檔]。 [!UICONTROL 注釋]。 [!UICONTROL 小時]。 [!UICONTROL 用戶]或 [!UICONTROL 作業角色]。

[!UICONTROL 報告] 和 [!UICONTROL 儀表板] 是可幫助您組織資料量的對象的另一個示例 [!DNL Workfront] 使所有用戶都能輕鬆訪問。

有關中對象的完整清單 [!DNL Workfront]，請參見 [API資源管理器](../../../wf-api/general/api-explorer.md)。

## 對象的相互依賴和層次

對象在 [!UICONTROL Workfront]。 例如，任務或問題在項目之外永遠不能獨立存在。 [!UICONTROL 任務] 和 [!UICONTROL 問題] 是儲存在 [!UICONTROL 項目] 的雙曲餘切值。 [!UICONTROL 任務] 和 [!UICONTROL 問題] 被視為項目的子對象。

以下是中某些最常用的對象 [!DNL Workfront] 及其各自的父子對象：

| **物件** | **父對象** | **子對象** |
|---|---|---|
| [!UICONTROL 專案組合] |  | [!UICONTROL 程式]。 [!UICONTROL 項目]。 [!UICONTROL 文檔]。 [!DNL Notes]。 [!UICONTROL 用戶] |
| [!UICONTROL 計劃] | [!UICONTROL 專案組合] | [!UICONTROL 項目]。 [!UICONTROL 文檔]。 [!UICONTROL 注釋]。 [!UICONTROL 用戶] |
| [!UICONTROL 專案] | [!UICONTROL Portfolio]。 [!UICONTROL 程式] | [!UICONTROL 任務]。 [!UICONTROL 問題]。 [!UICONTROL 文檔]。 [!UICONTROL 注釋]。 [!UICONTROL 小時]。 [!UICONTROL 用戶] |
| [!UICONTROL 任務] | [!UICONTROL 專案] | [!UICONTROL 問題]。 [!UICONTROL 子任務]。 [!UICONTROL 文檔]。 [!UICONTROL 注釋]。 [!UICONTROL 小時]。 [!UICONTROL 用戶] |
| [!UICONTROL 問題] | [!UICONTROL 任務]。 [!UICONTROL 項目] | [!UICONTROL 文檔]。 [!UICONTROL 注釋]。 [!UICONTROL 小時]。 [!UICONTROL 用戶] |
| [!UICONTROL 儀表板] |  | [!UICONTROL 報告]，外部頁面 |
| [!UICONTROL 報告] | [!UICONTROL 儀表板] |  |
| [!UICONTROL 群組] |  | [!UICONTROL 使用者] |
| [!UICONTROL 團隊] |  | [!UICONTROL 使用者] |
| [!UICONTROL 使用者] | [!UICONTROL 組]。 [!UICONTROL 團隊]。 [!UICONTROL 公司] | [!UICONTROL 職務角色] |
| [!UICONTROL 公司] |  | [!UICONTROL 使用者] |
| [!UICONTROL 文件] | [!UICONTROL 任務]。 [!UICONTROL 問題]。 [!UICONTROL 項目]。 [!UICONTROL Portfolio]。 [!UICONTROL 程式]。 [!UICONTROL 用戶] |  |
| [!UICONTROL 計畫]* |  | [!UICONTROL 方案] |
| [!DNL Goals]* |  | [!UICONTROL 結果]。 [!UICONTROL 活動] |

有關中對象的完整清單 [!DNL Workfront]，請參見 [API資源管理器](../../../wf-api/general/api-explorer.md)。

*計畫是 [!DNL Workfront Scenario Planner]。 有關 [!DNL Scenario Planner]，請參閱 [的 [!UICONTROL 方案規劃器] 概述](../../../scenario-planner/scenario-planner-overview.md)。

*[!UICONTROL 目標] 是 [!DNL Workfront Goals]。 有關 [!DNL Workfront Goals]，請參閱 [[!DNL Adobe Workfront Goals] 概述](../../../workfront-goals/goal-management/wf-goals-overview.md)。


## 自定義對象名稱

作為 [!DNL Workfront] 管理員，可以在 [!DNL Workfront] 使用  [!UICONTROL 佈局模板]。

有關如何使用  [!UICONTROL 佈局模板]，請參閱 [建立和管理佈局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)。

自定義佈局模板並將其分配給用戶後，這些用戶將看到對象的自定義名稱。 分配給佈局模板的用戶不再看到Web應用程式中任何位置的對象的預設名稱。

>[!NOTE]
>
>要讓用戶看到對象的新名稱，這些對象必須註銷並重新登錄到 [!DNL Workfront] 在你保存  [!UICONTROL 佈局模板]。

>[!IMPORTANT]
>
>的 [!DNL Workfront] 文檔始終引用對象的預設名稱。 作為 [!DNL Workfront] 管理員，確保您通知用戶對象名稱中的更改，以便他們能夠瞭解如何使用 [!DNL Workfront] 文檔，以及不反映對象名稱更改的應用程式區域。

* [可以使用  [!UICONTROL 佈局模板]](#object-names-that-can-be-customized-using-a-layout-template)
* [區域 [!DNL Workfront] 反映自定義對象名稱](#areas-of-workfront-that-reflect-the-customized-object-names)
* [區域 [!DNL Workfront] 不反映自定義對象名稱](#areas-of-workfront-that-do-not-reflect-the-customized-object-names)

### 可以使用 [!UICONTROL 佈局模板]

作為 [!DNL Workfront] 管理員，您可以自定義下列對象的名稱以與組織中的術語匹配：

* [!UICONTROL 專案組合]
* [!UICONTROL 方案]
* [!UICONTROL 專案]
* [!UICONTROL 任務]
* [!UICONTROL 問題]
* [!UICONTROL 目標]*
* [!UICONTROL 結果]*
* [!UICONTROL 活動]*

   *[!UICONTROL 目標]。 [!UICONTROL 結果], [!UICONTROL 活動] 僅當您的公司購買時 [!DNL Workfront Goals]。 有關 [!DNL Workfront Goals]，請參閱 [[!DNL Adobe Workfront Goals] 概述](../../../workfront-goals/goal-management/wf-goals-overview.md)。

* [!UICONTROL 行動方案]**
* [!UICONTROL 情境]**
* [!UICONTROL 計劃]**

   **[!UICONTROL 倡議]。 [!UICONTROL 場景], [!UICONTROL 計畫] 只有在您的公司購買了 [!DNL Workfront Scenario Planner]。 有關 [!DNL Scenario Planner]，請參閱 [開始使用 [!DNL Scenario Planner]](../../../scenario-planner/get-started-with-scenario-planning.md)。


例如，如果組織中的較大工作量稱為「項目」，則可以替換名稱「[!UICONTROL 項目]「 Engagement」。 您 [!DNL Workfront] 介面顯示「Engagement」而不是「[!UICONTROL 項目]名稱「」的位置[!UICONTROL 項目]」。

有關如何使用  [!UICONTROL 佈局模板]，請參閱 [建立和管理佈局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)。

不能自定義Workfront中任何其他對象的名稱。 有關中對象的完整清單 [!DNL Workfront]，請參見 [API資源管理器](../../../wf-api/general/api-explorer.md)。

自定義對象名稱時，該對象的新名稱將出現在 [!DNL Workfront] 顯示對象名稱的應用程式。

### 區域 [!DNL Workfront] 反映自定義對象名稱

以下區域顯示對象的更新名稱：

* 上方巡覽
* 左面板導航中的所有部分
* 所有菜單
* 應用內通知
* 報表生成器和報表元素（視圖、篩選器和分組）
* [!UICONTROL 保存] 按鈕
* 導出的檔案
* 電子郵件
* 移動應用

### 區域 [!DNL Workfront] 不反映自定義對象名稱

以下區域不顯示對象的更新名稱：

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Referenced Object Type selection for a Typeahead field in a Custom Form </p> <p>(NOTE: drafting this because I don't think this is true)</p> </li>
  -->

* [!DNL Outlook] 載入項

## 自定義對象名稱的含義

在中自定義對象名稱時，應注意以下事項 [!DNL Workfront]:

* 在系統顯示中，可能會遇到文體或語法錯誤。 例如，如果更名「[!UICONTROL 問題]「」到「請求」，您在系統中的任何位置都看到短語「An request」，它按預期運行，不應被視為Bug。
* 對象的自定義名稱不可翻譯。 僅 [!DNL Workfront] 預設名稱可以用支援的語言翻譯。 有關中支援的語言的詳細資訊 [!DNL Workfront]，請參閱 [支援的語言 [!DNL Adobe Workfront]](../../../workfront-basics/supported-languages-in-workfront.md)。 自定義對象名稱欄位支援外來字元，因此您可以以任何語言輸入術語。
* 使用  [!UICONTROL 佈局模板]，建議您  [!UICONTROL 佈局模板] 業務單元（團隊或組）。\
   我們建議您使用這些業務部門的用戶能夠清楚理解的名稱，以避免混淆。
* 電子郵件通知和已傳遞的報告始終包含由  [!UICONTROL 佈局模板] 生成電子郵件的用戶。 如果用戶收到其他團隊和組中用戶的電子郵件通知，則應準備好在其電子郵件中查看與其組或團隊無關的對象名稱。\
   作為 [!DNL Workfront] 管理員，建議用戶注意與每個對象關聯的表徵圖。 表徵圖在各種對象名稱之間保持一致，並且與預設對象一致，就像它出現在資料庫中一樣。 用於所有清單 [!DNL Workfront] 與對象關聯的表徵圖，請參閱 [對象表徵圖](#object-icons)。

   >[!TIP]
   >
   >對於組織中的常見任務，請考慮建立自定義文檔以反映您的術語。

## 對象表徵圖

的 [!DNL Workfront] 文檔始終引用對象的預設名稱。 如果對象已自定義了其名稱，則可以依靠與其關聯的表徵圖來瞭解哪些自定義對象與哪些對象對應 [!DNL Workfront] 預設對象。

有關哪些對象可以在中具有自定義名稱的詳細資訊 [!DNL Workfront]，請參閱 [可以使用  [!UICONTROL 佈局模板]](#object-names-that-can-be-customized-using-a-layout-template)。

以下是Workfront中對象及其相應表徵圖的清單。

| **物件** | **圖示** | **可自定義的對象名稱** |
|---|---|---|
| [!UICONTROL 公司] | ![](assets/company-icon-nwe.png)  , ![](assets/nwe-company-icon-54x54.png) |  |
| [!UICONTROL 儀表板] | ![](assets/dashboard-icon-nwe.png)  , ![](assets/nwe-dashboards-icon.png) |  |
| [!UICONTROL 目標] | ![](assets/nwe-goal-icon.png) | ✔ |
| [!UICONTROL 群組] | ![](assets/groups-icon-nwe.png)  , ![](assets/nwe-group-icon.png) |  |
| [!UICONTROL 問題] | ![](assets/issue-icon-nwe.png)  , ![](assets/nwe-issues-icon.png) | ✔ |
| [!UICONTROL 職務角色] | ![job_role_icon_png](assets/job-role-icon-52x50.png)。 ![job_role_icon_1_.png](assets/job-role-icon--1--53x44.png)。 ![](assets/job-role-nwe-no-color.png)。 ![](assets/job-role-icon-nwe-color.png) |  |
| [!UICONTROL 計劃] | ![](assets/plan-icon.png), ![](assets/nwe-plan-icon-60x57.png) |  |
| [!UICONTROL 專案組合] | ![](assets/portfolio-icon-nwe.png)  , ![](assets/nwe-portfolios-icon.png) | ✔ |
| [!UICONTROL 方案] | ![](assets/program-icon-nwe.png)  , ![](assets/nwe-programs-icon.png) | ✔ |
| [!UICONTROL 專案] | ![](assets/project-icon-nwe.png)  , ![](assets/nwe-projects-icon.png) | ✔ |
| [!UICONTROL 報告] | ![](assets/report-icon-nwe.png) , ![](assets/nwe-reports-icon.png) |  |
| [!UICONTROL 任務] | ![](assets/task-icon-new.png)  , ![](assets/nwe-tasks-icon.png) | ✔ |
| [!UICONTROL 團隊] | ![](assets/team-icon-nwe.png), ![](assets/team-icon-nwe-color.png) , ![](assets/nwe-teams-icon.png) |  |
| [!UICONTROL 範本] | ![](assets/template-icon-nwe.png)  , ![](assets/nwe-templates-icon.png) |  |

## 對象的引用編號

建立的每個對象 [!DNL Workfront] 為其分配了唯一的引用編號。 參考編號在區分兩個其它相似對象（如具有相同名稱的任務）時非常有用。 您可以使用對象的參考編號來搜索對象，也可以在報表中包括參考編號。

有關如何按參考編號搜索對象的資訊，請參閱 [使用對象的引用數](../../../workfront-basics/navigate-workfront/search/reference-number-of-objects.md)。

## 對象特定搜索

您可以搜索所有可在中搜索的對象 [!DNL Workfront]，或者可以選擇要在基本和高級搜索中搜索的特定對象。

並非所有對象都可在 [!DNL Workfront]。 您可以在中為以下對象運行基本和高級搜索 [!DNL Workfront]:

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
| [!UICONTROL 附註] | ✓ |  |

有關在中運行基本和高級搜索的詳細資訊 [!DNL Workfront]，請參閱 [搜索 [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/search/search-workfront.md)。

## 對象報告

在開始在中生成報告之前，瞭解對象的層次結構和相互依賴關係非常重要 [!DNL Workfront]。 報告是特定於對象的。 必須為報表選擇正確的對象，才能顯示所需的資料。

根據您為報表選擇的對象，您只能訪問直接連結到報表對象的那些對象。

>[!IMPORTANT]
>
>您只能報告所選對象和同一報告中的父對象。 父對象報表中不能包含有關子對象的資訊。 例如，可以在任務報告中顯示項目資訊，但不能在項目報告中顯示任務資訊。

可以使用我們的開啟API報告資料庫中的所有對象。 有關資料庫中所有對象的完整清單，請參見 [API資源管理器](../../../wf-api/general/api-explorer.md)。

>[!NOTE]
>
>如果已使用佈局模板自定義對象的名稱，則報表生成器中對象的名稱也已自定義。 確保您知道哪些對象已自定義，並在報表生成器中查找自定義名稱。 有關哪些對象可以在中具有自定義名稱的詳細資訊 [!DNL Workfront]，請參閱 *[可以使用  [!UICONTROL 佈局模板]](#object-names-that-can-be-customized-using-a-layout-template)。*
>在報表中使用文本模式時，文本模式表達式中對象的名稱是 [!DNL Workfront]，而不是自定義對象名。 有關在報告中使用文本模式的詳細資訊，請參見 [文本模式概述](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)。

有關生成報告的詳細資訊，請參見 [建立自定義報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。\
有關API的詳細資訊，請參見 [API資源管理器](../../../wf-api/general/api-explorer.md)。

在中使用報表生成器時，可以報告以下對象 [!DNL Workfront] web應用程式：

* [!UICONTROL 專案]
* [!UICONTROL 任務]
* [!UICONTROL 時數]
* [!UICONTROL 問題]
* [!UICONTROL 使用者]
* [!UICONTROL 存取層級]
* [!UICONTROL 核准]
* [!UICONTROL 核准流程]
* [!UICONTROL 指派]
* [!UICONTROL 積壓工作項]\
   顯示敏捷積壓工作中的任務或問題。 有關敏捷積壓的詳細資訊，請參閱 [管理敏捷積壓](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)。

* [!UICONTROL 基準線]
* [!UICONTROL 基準線任務]
* [!UICONTROL 付費記錄]
* [!UICONTROL 已編列預算時數]

   這是 [!UICONTROL 預算小時數]，如舊的、過時的資源管理工具中所示。

   巴德。 「小時」欄位 [!UICONTROL 預算工時] 報表是指為中的工作角色編入預算的小時數 [!UICONTROL 資源計畫器]。 有關詳細資訊，請參見 [瞭解 [!UICONTROL 預算人工成本] 和 [!UICONTROL 預算小時數] 為項目](../../../manage-work/projects/project-finances/budgeted-labor-cost.md)。

* [!UICONTROL 行事曆事件]
* [!UICONTROL 類別] 或 [!UICONTROL 自定義窗體])
* [!UICONTROL 公司]
* [!UICONTROL 儀表板]
* [!UICONTROL 文件]
* [!UICONTROL 文件核准]
* [!UICONTROL 文件版本]\
   允許您查看有關文檔版本、版本與之關聯的文檔、建立版本的人以及在文檔版本上建立證明（如果存在）的用戶的各種資訊（證明建立者）。
* [!UICONTROL 電子郵件範本]
* [!UICONTROL 費用]
* [!UICONTROL 費用類型]
* [!UICONTROL 外部頁面]
* [!UICONTROL 加入最愛]
* [!UICONTROL 篩選器]
* [!UICONTROL 目標]

   您可以為戰略目標生成報告，或在項目與目標關聯為目標活動時，在項目報告中顯示與目標相關的資訊。 只有在您的組織購買了 [!DNL Workfront Goals] 許可證。 有關 [!DNL Workfront Goals]，請參閱 [[!DNL Workfront Goals] 概述](../../../workfront-goals/goal-management/wf-goals-overview.md)。 有關將項目與戰略目標連接的資訊，請參見 [將項目添加到Adobe Workfront目標中的目標](../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md)。

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: hardcoded links in this paragraph)
  </MadCap:conditionalText>
  -->

   >[!TIP]
   >
   >無法報告與關聯的項目目標 [!UICONTROL 業務案例]。 有關項目目標與戰略目標的資訊，請參見 [辭彙表 [!DNL Adobe Workfront] 術語](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md)。

* [!UICONTROL 群組]
* [!UICONTROL 分組]
* [!UICONTROL 時數類型]
* [!UICONTROL 行動方案]

   只有在您的公司購買了計畫的子對象時，您才能為計畫生成報告 [!DNL Workfront Scenario Planner] 許可證。 有關方案的資訊，請參見 [中的計畫概述 [!DNL Workfront Scenario Planner]](../../../scenario-planner/initiatives-overview.md)。


* 計畫工作角色

   只有在您的公司購買了計畫中與方案關聯的職務職責時，您才可以生成報表 [!DNL Workfront Scenario Planner] 許可證。 有關建立方案並將其與職務職責關聯的資訊，請參閱 [在中建立和編輯方案 [!DNL Workfront Scenario Planner]](../../../scenario-planner/create-and-edit-initiatives.md)。


* [!UICONTROL 反覆項目]
* [!UICONTROL 職務角色]
* [!UICONTROL 日誌輸入項目]

   您可以在 [!UICONTROL 更新] 任務、項目、問題等對象的區域。 要瞭解更多資訊，請參閱 [報告 [!UICONTROL 更新] 面積](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md)。

* [!UICONTROL 配置範本]
* [!UICONTROL 里程碑]
* [!UICONTROL 里程碑路徑]
* [!UICONTROL 備註]

   >[!NOTE]
   >
   >您可以報告由單個用戶添加的注釋。

* [!UICONTROL 參數] 或 [!UICONTROL 自定義欄位])
* [!UICONTROL 參陣列] 或 [!UICONTROL 分節符])
* [!UICONTROL 門戶配置檔案] （這顯示已棄用的資訊）
* [!UICONTROL 專案組合]
* [!UICONTROL 方案]
* [!UICONTROL 項目] ([!UICONTROL 財務資料])

   >[!NOTE]
   >
   >財務資訊填入 [!UICONTROL 項目] ([!UICONTROL 財務資料])僅在與其關聯的資料的使用時間少於5年時報告。 例如，如果在2015年1月將某個職務分配給某項任務，而今天是2021年9月，則像 [!UICONTROL 分配日期] 作業角色未填充 [!UICONTROL 項目（財務資料）] 報告。

* [!UICONTROL 校訂核准]\
   使您能夠查看有關證明審批的各種資訊，包括：提交審批的證明，有關 [!UICONTROL 批准者]，有關請求者的資訊(如果請求者是許可的 [!DNL Workfront] 用戶)、版本資訊、證明ID和證明建立日期。\
   [!UICONTROL 證明批准] 報告只包含用戶「我的工作」區域中尚未做出決策的可用證據。\
   在中分配證明批准 [!DNL Workfront] 如所述 [將用戶添加到證明](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) 在 [在中共用證據 [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)。

* [!UICONTROL 佇列]
* [!UICONTROL 佇列主題]
* [!UICONTROL 比率] (顯示作業角色 [!UICONTROL 開單費率] 資訊)
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

   您可以報告用戶在其配置檔案中指示的休假時間。

* [!UICONTROL 時程表]
* [!UICONTROL 時間表設定檔]
* [!UICONTROL 主題群組]
* [!UICONTROL 使用者委派]

   您可以報告已委派用戶在外出時執行他人的任務和問題的用戶。 此報表顯示外出的用戶以及外出時履行職責的用戶。

* [!UICONTROL 檢視]
* [!UICONTROL 工作項] （指任務和問題）
