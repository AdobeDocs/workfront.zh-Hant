---
content-type: overview;reference
navigation-topic: workfront-navigation
title: 了解 [!DNL Adobe Workfront]
description: 了解 [!DNL Adobe Workfront]
feature: Get Started with Workfront
exl-id: f324f198-5472-4cf2-a46e-7fc24605ca90
source-git-commit: 9c78d8e08e62c86a4e1340644ed76c61ce7f2674
workflow-type: tm+mt
source-wordcount: '2308'
ht-degree: 6%

---

# 了解 [!DNL Adobe Workfront]

<!--
<***Linked to several articles, do not remove/ change. 
-->

顯示在 [!DNL Adobe Workfront] 由儲存在 [!DNL Workfront] 資料庫。 物件是 [!DNL Workfront].

了解物件在 [!DNL Workfront] 非常重要，這樣您才能根據組織中的必要需求使用正確的物件。

例如，當您計畫大量工作時，需要使用 [!UICONTROL 專案] 物件來定義該工作。 若要將此工作劃分為較小的計畫增量，您可以使用 [!UICONTROL 任務] 物件。 對於未計畫且可能意外發生的較小工作量，您可以使用「問題」對象。 如果您想要追蹤一組專案的進度及遵守預算和時間表的情況，可以在 [!UICONTROL Portfolio] 和 [!UICONTROL 方案]. 要定義幫助您解析工作的其他元素，需要使用儲存在 [!UICONTROL 專案], [!UICONTROL 工作], [!UICONTROL 問題]，或 [!UICONTROL Portfolio]，如 [!UICONTROL 檔案], [!UICONTROL 附註], [!UICONTROL 小時], [!UICONTROL 使用者]，或 [!UICONTROL 作業角色].

[!UICONTROL 報表] 和 [!UICONTROL 控制面板] 是物件的另一個範例，可協助您組織中的資料量 [!DNL Workfront] 視覺化，讓所有使用者都能輕鬆存取。

若要取得中的物件完整清單 [!DNL Workfront]，請參閱 [API Explorer](../../../wf-api/general/api-explorer.md).

## 對象的相互依存和層次

對象在 [!UICONTROL Workfront]. 例如，任務或問題在專案之外不可能獨立存在。 [!UICONTROL 工作] 和 [!UICONTROL 問題] 是儲存在中的物件的範例 [!UICONTROL 專案] 物件。 [!UICONTROL 工作] 和 [!UICONTROL 問題] 被視為項目的子對象。

以下是 [!DNL Workfront] 及其各自的父項和子項對象：

| **物件** | **父對象** | **子對象** |
|---|---|---|
| [!UICONTROL 專案組合] |  | [!UICONTROL 方案], [!UICONTROL 專案], [!UICONTROL 檔案], [!DNL Notes], [!UICONTROL 使用者] |
| [!UICONTROL 計劃] | [!UICONTROL 專案組合] | [!UICONTROL 專案], [!UICONTROL 檔案], [!UICONTROL 附註], [!UICONTROL 使用者] |
| [!UICONTROL 專案] | [!UICONTROL Portfolio], [!UICONTROL 方案] | [!UICONTROL 工作], [!UICONTROL 問題], [!UICONTROL 檔案], [!UICONTROL 附註], [!UICONTROL 小時], [!UICONTROL 使用者] |
| [!UICONTROL 任務] | [!UICONTROL 專案] | [!UICONTROL 問題], [!UICONTROL 子任務], [!UICONTROL 檔案], [!UICONTROL 附註], [!UICONTROL 小時], [!UICONTROL 使用者] |
| [!UICONTROL 問題] | [!UICONTROL 工作], [!UICONTROL 專案] | [!UICONTROL 檔案], [!UICONTROL 附註], [!UICONTROL 小時], [!UICONTROL 使用者] |
| [!UICONTROL 儀表板] |  | [!UICONTROL 報表]，外部頁面 |
| [!UICONTROL 報告] | [!UICONTROL 儀表板] |  |
| [!UICONTROL 群組] |  | [!UICONTROL 使用者] |
| [!UICONTROL 團隊] |  | [!UICONTROL 使用者] |
| [!UICONTROL 使用者] | [!UICONTROL 群組], [!UICONTROL 團隊], [!UICONTROL 公司] | [!UICONTROL 職務角色] |
| [!UICONTROL 公司] |  | [!UICONTROL 使用者] |
| [!UICONTROL 文件] | [!UICONTROL 工作], [!UICONTROL 問題], [!UICONTROL 專案], [!UICONTROL Portfolio], [!UICONTROL 方案], [!UICONTROL 使用者] |  |
| [!UICONTROL 計畫]* |  | [!UICONTROL 方案] |
| [!DNL Goals]* |  | [!UICONTROL 結果], [!UICONTROL 活動] |

若要取得中的物件完整清單 [!DNL Workfront]，請參閱 [API Explorer](../../../wf-api/general/api-explorer.md).

*計畫是 [!DNL Workfront Scenario Planner]. 如需 [!DNL Scenario Planner]，請參閱 [此 [!UICONTROL 方案計畫員] 概述](../../../scenario-planner/scenario-planner-overview.md).

*[!UICONTROL 目標] 是 [!DNL Workfront Goals]. 如需有關 [!DNL Workfront Goals]，請參閱 [[!DNL Adobe Workfront Goals] 概述](../../../workfront-goals/goal-management/wf-goals-overview.md).


## 自訂物件名稱

As a [!DNL Workfront] 管理員，可以在 [!DNL Workfront] 使用  [!UICONTROL 版面範本].

如需如何使用自訂物件名稱的詳細資訊，  [!UICONTROL 版面範本]，請參閱 [建立和管理版面範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

自訂版面範本並將其指派給使用者後，這些使用者會看到物件的自訂名稱。 已指派給版面範本的使用者，在Web應用程式中的任何位置都看不到物件的預設名稱。

>[!NOTE]
>
>要讓用戶看到對象的新名稱，它們必須註銷並重新登錄 [!DNL Workfront] 在您儲存  [!UICONTROL 版面範本].

>[!IMPORTANT]
>
>此 [!DNL Workfront] 文檔始終指對象的預設名稱。 As a [!DNL Workfront] 管理員，請確定您通知使用者物件名稱的變更，以便他們了解如何使用 [!DNL Workfront] 文檔，以及不反映對象名稱更改的應用程式區域。

* [可使用  [!UICONTROL 版面範本]](#object-names-that-can-be-customized-using-a-layout-template)
* [區域 [!DNL Workfront] 會反映自訂物件名稱](#areas-of-workfront-that-reflect-the-customized-object-names)
* [區域 [!DNL Workfront] 不反映自定義對象名稱](#areas-of-workfront-that-do-not-reflect-the-customized-object-names)

### 可使用 [!UICONTROL 版面範本]

As a [!DNL Workfront] 管理員，您可以自訂下列物件的名稱，以符合組織中的術語：

* [!UICONTROL 專案組合]
* [!UICONTROL 方案]
* [!UICONTROL 專案]
* [!UICONTROL 任務]
* [!UICONTROL 問題]
* [!UICONTROL 目標]*
* [!UICONTROL 結果]*
* [!UICONTROL 活動]*

   *[!UICONTROL 目標], [!UICONTROL 結果]，和 [!UICONTROL 活動] 只有在您的公司已購買時才可用 [!DNL Workfront Goals]. 如需有關 [!DNL Workfront Goals]，請參閱 [[!DNL Adobe Workfront Goals] 概述](../../../workfront-goals/goal-management/wf-goals-overview.md).

* [!UICONTROL 行動方案]**
* [!UICONTROL 情境]**
* [!UICONTROL 計劃]**

   **[!UICONTROL 舉措], [!UICONTROL 藍本]，和 [!UICONTROL 計畫] 只有在貴公司已購買 [!DNL Workfront Scenario Planner]. 如需 [!DNL Scenario Planner]，請參閱 [開始使用 [!DNL Scenario Planner]](../../../scenario-planner/get-started-with-scenario-planning.md).


例如，如果貴組織中較大的工作量稱為「參與」，則可以取代名稱「[!UICONTROL 專案]&#39;與&#39;Engagement&#39;。 您的 [!DNL Workfront] 介面顯示「參與」而非「[!UICONTROL 專案]名稱為「[!UICONTROL 專案]&#39;。

有關如何使用  [!UICONTROL 版面範本]，請參閱 [建立和管理版面範本](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

您無法自訂Workfront中任何其他物件的名稱。 若要取得中的物件完整清單 [!DNL Workfront]，請參閱 [API Explorer](../../../wf-api/general/api-explorer.md).

當您自訂物件的名稱時，該物件的新名稱會顯示在 [!DNL Workfront] 顯示該物件名稱的應用程式。

### 區域 [!DNL Workfront] 會反映自訂物件名稱

以下區域顯示對象的更新名稱：

* 上方巡覽
* 左側面板導覽中的所有區段
* 所有菜單
* 應用程式內通知
* 報告建立工具和報告元素（檢視、篩選和群組）
* [!UICONTROL 儲存] 按鈕
* 匯出的檔案
* 電子郵件
* 行動應用程式

### 區域 [!DNL Workfront] 不反映自定義對象名稱

以下區域不顯示對象的更新名稱：

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Referenced Object Type selection for a Typeahead field in a Custom Form </p> <p>(NOTE: drafting this because I don't think this is true)</p> </li>
  -->

* [!DNL Outlook] 附加元件

## 自定義對象名稱的意義

自訂物件名稱時，請注意下列事項： [!DNL Workfront]:

* 在系統顯示中，您可能會遇到文體或語法錯誤。 例如，如果更名「[!UICONTROL 問題]「到「Request」，而您在系統的任何位置都看到片語「An request」，此功能如預期運作，不應視為錯誤。
* 對象的自定義名稱不可翻譯。 僅 [!DNL Workfront] 預設名稱可翻譯成支援的語言。 如需支援語言的詳細資訊，請參閱 [!DNL Workfront]，請參閱 [支援的語言 [!DNL Adobe Workfront]](../../../workfront-basics/supported-languages-in-workfront.md). 自訂物件名稱欄位支援外文字元，因此您可以輸入任何語言的術語。
* 使用  [!UICONTROL 版面範本]，建議您將  [!UICONTROL 版面範本] （團隊或群組）。\
   建議您使用這些業務單位使用者清楚了解的名稱，以避免混淆。
* 電子郵件通知和傳送的報表一律包含由  [!UICONTROL 版面範本] 產生電子郵件的使用者。 如果您的使用者收到其他團隊和群組使用者的電子郵件通知，應準備好在其電子郵件中看見與其群組或團隊無關的物件名稱。\
   As a [!DNL Workfront] 管理員建議用戶注意與每個對象關聯的表徵圖。 各個對象名稱之間的表徵圖保持一致，並且與預設對象一致，如資料庫中所示。 要獲取所有 [!DNL Workfront] 與對象關聯的表徵圖，請參閱 [對象表徵圖](#object-icons).

   >[!TIP]
   >
   >若為貴組織的常見工作，請考慮建立自訂檔案以反映您的術語。

## 對象表徵圖

此 [!DNL Workfront] 檔案一律指物件的預設名稱。 如果對象已自定義其名稱，則可以依靠與其關聯的表徵圖來了解哪些自定義對象與哪些對象相對應 [!DNL Workfront] 預設對象。

有關哪些對象可以在 [!DNL Workfront]，請參閱 [可使用  [!UICONTROL 版面範本]](#object-names-that-can-be-customized-using-a-layout-template).

以下是Workfront中物件及其對應圖示的清單。

| **物件** | **圖示** | **可自訂的物件名稱** |
|---|---|---|
| [!UICONTROL 公司] | ![](assets/company-icon-nwe.png)  , ![](assets/nwe-company-icon-54x54.png) |  |
| [!UICONTROL 儀表板] | ![](assets/dashboard-icon-nwe.png)  , ![](assets/nwe-dashboards-icon.png) |  |
| [!UICONTROL 目標] | ![](assets/nwe-goal-icon.png) | ✔ |
| [!UICONTROL 群組] | ![](assets/groups-icon-nwe.png)  , ![](assets/nwe-group-icon.png) |  |
| [!UICONTROL 問題] | ![](assets/issue-icon-nwe.png)  , ![](assets/nwe-issues-icon.png) | ✔ |
| [!UICONTROL 職務角色] | ![job_role_icon.png](assets/job-role-icon-52x50.png), ![job_role_icon__1_.png](assets/job-role-icon--1--53x44.png), ![](assets/job-role-nwe-no-color.png), ![](assets/job-role-icon-nwe-color.png) |  |
| [!UICONTROL 計劃] | ![](assets/plan-icon.png), ![](assets/nwe-plan-icon-60x57.png) |  |
| [!UICONTROL 專案組合] | ![](assets/portfolio-icon-nwe.png)  , ![](assets/nwe-portfolios-icon.png) | ✔ |
| [!UICONTROL 方案] | ![](assets/program-icon-nwe.png)  , ![](assets/nwe-programs-icon.png) | ✔ |
| [!UICONTROL 專案] | ![](assets/project-icon-nwe.png)  , ![](assets/nwe-projects-icon.png) | ✔ |
| [!UICONTROL 報告] | ![](assets/report-icon-nwe.png) , ![](assets/nwe-reports-icon.png) |  |
| [!UICONTROL 任務] | ![](assets/task-icon-new.png)  , ![](assets/nwe-tasks-icon.png) | ✔ |
| [!UICONTROL 團隊] | ![](assets/team-icon-nwe.png), ![](assets/team-icon-nwe-color.png) , ![](assets/nwe-teams-icon.png) |  |
| [!UICONTROL 範本] | ![](assets/template-icon-nwe.png)  , ![](assets/nwe-templates-icon.png) |  |

## 對象的參考編號

在中建立的每個物件 [!DNL Workfront] 被分配一個唯一的引用編號。 在區分兩個其他類似對象時（例如具有相同名稱的任務），參考編號很有用。 您可以使用對象的參考編號來搜索對象，也可以在報告中包括參考編號。

有關如何按參考編號搜索對象的資訊，請參見 [使用對象的參考編號](../../../workfront-basics/navigate-workfront/search/reference-number-of-objects.md).

## 物件專屬搜尋

您可以搜尋 [!DNL Workfront]，或者，您可以在基本和進階搜尋中選取要搜尋的特定物件。

並非所有物件都可在 [!DNL Workfront]. 您可以在 [!DNL Workfront]:

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

有關運行基本和高級搜索的詳細資訊，請參閱 [!DNL Workfront]，請參閱 [搜尋 [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

## 對象報告

在開始在中建立報表之前，了解物件的階層和互依關係非常重要 [!DNL Workfront]. 報表是物件專屬的。 您必須為報表選取正確的物件，才能顯示您想要的資料。

根據您為報表選取的物件，您只能存取直接連結至報表物件的物件。

>[!IMPORTANT]
>
>只能報告所選對象以及同一報告中的父對象。 父對象報表中不能有子對象的相關資訊。 例如，您可以在任務報表中顯示項目資訊，但在項目報表中不顯示任務資訊。

您可以使用開啟的API來報告資料庫中的所有對象。 有關資料庫中所有對象的完整清單，請參見 [API Explorer](../../../wf-api/general/api-explorer.md).

>[!NOTE]
>
>如果您已使用版面範本自訂物件的名稱，報表建立工具中物件的名稱也已自訂。 請確定您知道哪些物件已自訂，並在Report Builder中尋找自訂名稱。 有關哪些對象可以在 [!DNL Workfront]，請參閱 *[可使用  [!UICONTROL 版面範本]](#object-names-that-can-be-customized-using-a-layout-template).*
>在報表中使用文字模式時，文字模式運算式中的物件名稱是 [!DNL Workfront]，而非自訂物件名稱。 如需在報表中使用文字模式的詳細資訊，請參閱 [文字模式概觀](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

如需建立報表的詳細資訊，請參閱 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).\
如需API的詳細資訊，請參閱 [API Explorer](../../../wf-api/general/api-explorer.md).

使用Report Builder時，您可以報告下列物件： [!DNL Workfront] 網頁應用程式：

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
   顯示敏捷積壓的工作或問題。 有關敏捷積壓的詳細資訊，請參閱 [管理敏捷積壓](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

* [!UICONTROL 基準線]
* [!UICONTROL 基準線任務]
* [!UICONTROL 付費記錄]
* [!UICONTROL 已編列預算時數]

   這是 [!UICONTROL 預算小時數]，如舊版、過時的資源管理工具中所示。

   &quot;巴德&quot; 小時」欄位 [!UICONTROL 預算小時數] 報表是指 [!UICONTROL 資源計畫員]. 如需詳細資訊，請參閱 [了解 [!UICONTROL 預算人工成本] 和 [!UICONTROL 預算小時數] 針對專案](../../../manage-work/projects/project-finances/budgeted-labor-cost.md).

* [!UICONTROL 行事曆事件]
* [!UICONTROL 類別] (或 [!UICONTROL 自訂表單])
* [!UICONTROL 公司]
* [!UICONTROL 儀表板]
* [!UICONTROL 文件]
* [!UICONTROL 文件核准]
* [!UICONTROL 文件版本]\
   使您可以查看有關文檔版本、版本關聯的文檔、建立版本的人員以及在文檔版本上建立校樣（如果存在）的用戶的各種資訊（校樣建立器）。
* [!UICONTROL 電子郵件範本]
* [!UICONTROL 費用]
* [!UICONTROL 費用類型]
* [!UICONTROL 外部頁面]
* [!UICONTROL 加入最愛]
* [!UICONTROL 篩選器]
* [!UICONTROL 目標]

   您可以建立策略目標的報表，或當項目與目標關聯為目標活動時，您可以在專案報表中顯示與目標相關的資訊。 只有在貴組織已購買 [!DNL Workfront Goals] 授權。 如需有關 [!DNL Workfront Goals]，請參閱 [[!DNL Workfront Goals] 概述](https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FWorkfront_Goals%2FGoal_management%2Fwf-goals-overview.htm&amp;_LANG=en). 如需將專案連結至策略目標的相關資訊，請參閱 [將專案新增至Adobe Workfront目標中的目標](https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FWorkfront_Goals%2FResults_and_activities%2Fconnect-projects-to-goals-overview.htm&amp;_LANG=en).

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: hardcoded links in this paragraph)
  </MadCap:conditionalText>
  -->

   >[!TIP]
   >
   >您無法報告與 [!UICONTROL 業務案例]. 如需有關專案目標與策略目標的資訊，請參閱 [辭匯表 [!DNL Adobe Workfront] 術語](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* [!UICONTROL 群組]
* [!UICONTROL 分組]
* [!UICONTROL 時數類型]
* [!UICONTROL 行動方案]

   只有在貴公司已購買 [!DNL Workfront Scenario Planner] 授權。 有關計畫的資訊，請參閱 [計畫概覽 [!DNL Workfront Scenario Planner]](https://one.workfront.com/s/csh?context=2066&amp;pubname=the-new-workfront-experience).

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this link is hardcoded)
  </MadCap:conditionalText>
  -->

* 計畫工作角色

   只有在貴公司已購買 [!DNL Workfront Scenario Planner] 授權。 有關建立方案以及將其與職務關聯的資訊，請參閱 [在 [!DNL Workfront Scenario Planner]](https://one.workfront.com/s/csh?context=2061&amp;pubname=the-new-workfront-experience).

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this link is hardcoded)
  </MadCap:conditionalText>
  -->

* [!UICONTROL 反覆項目]
* [!UICONTROL 職務角色]
* [!UICONTROL 日誌輸入項目]

   您可以在 [!UICONTROL 更新] 對象區域，如任務、項目、問題等。 若要進一步了解，請參閱 [報告 [!UICONTROL 更新] 區域](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

* [!UICONTROL 配置範本]
* [!UICONTROL 里程碑]
* [!UICONTROL 里程碑路徑]
* [!UICONTROL 備註]

   >[!NOTE]
   >
   >您可以報告個別使用者新增的留言。

* [!UICONTROL 參數] (或 [!UICONTROL 自訂欄位])
* [!UICONTROL 參陣列] (或 [!UICONTROL 區段分隔])
* [!UICONTROL 入口網站設定檔] （這會顯示已過時的資訊）
* [!UICONTROL 專案組合]
* [!UICONTROL 方案]
* [!UICONTROL 專案] ([!UICONTROL 財務資料])

   >[!NOTE]
   >
   >財務資訊填入 [!UICONTROL 專案] ([!UICONTROL 財務資料])僅在與其相關聯的資料少於5年時報告。 例如，如果在2015年1月將工作角色分配給任務，而今天是2021年9月，則會有類似 [!UICONTROL 分配日期] 作業角色的不會填入 [!UICONTROL 項目（財務資料）] 報表。

* [!UICONTROL 校訂核准]\
   可讓您檢視校樣核准的各種資訊，包括：提交以供核准的證明， [!UICONTROL 核准者]，請求者的相關資訊(如果請求者是 [!DNL Workfront] 使用者)、版本資訊、校樣ID和校樣建立日期。\
   [!UICONTROL 證明核准] 報表僅包含使用者「我的工作」區域中可用的校樣，而尚未做出決策。\
   校樣核准已指派至 [!DNL Workfront] 說明 [新增使用者至校樣](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) in [在內共用校樣 [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

* [!UICONTROL 佇列]
* [!UICONTROL 佇列主題]
* [!UICONTROL 比率] (這表示作業角色 [!UICONTROL 計費率] 資訊)
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

   您可以依照使用者設定檔中的使用者指示，來報告使用者的休假時間。

* [!UICONTROL 時程表]
* [!UICONTROL 時間表設定檔]
* [!UICONTROL 主題群組]
* [!UICONTROL 使用者委派]

   您可以報告已委派在他人不在辦公室時執行其任務和問題的用戶。 此報表顯示不在辦公室的使用者，以及在離開時履行其職責的使用者。

* [!UICONTROL 檢視]
* [!UICONTROL 工作項] （這是指任務和問題）
