---
content-type: reference
navigation-topic: workfront-navigation
title: 辭彙表 [!DNL Adobe Workfront] 術語
description: 的 [!DNL Adobe Workfront] 辭彙表列出了Adobe Workfront常用術語。
feature: Get Started with Workfront
exl-id: 758072b3-775e-4771-9ae9-da0b38580c93
source-git-commit: 888c938e5d649557df69374a55d4e4ecc2da6f55
workflow-type: tm+mt
source-wordcount: '19551'
ht-degree: 0%

---

# 辭彙表 [!DNL Adobe Workfront] 術語

>[!IMPORTANT]
>
>本文應用作參考，以瞭解在 [!DNL Adobe Workfront] 應用程式，在 [!DNL Workfront] 文檔，或通常說到規劃和管理工作時。 我們當前正在更新此資訊，因此此表可能不完整。 當我們考慮完整的資訊時，我們將刪除此免責聲明。

下表是Adobe Workfront常用術語的清單：

## A - C

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>物件名稱</strong></th> 
   <th><strong>說明</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL訪問級別]</td> 
   <td>確定用戶如何與Workfront內的不同對象和工具交互的用戶配置檔案。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL活動任務]</td> 
   <td>當前項目中未完成的任務，該任務不會被前置任務所阻止，並且沒有具有將來計畫起始日期的任務約束。 換句話說，它可以在今天進行。</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL活動]</td> 
   <td>在 [!DNL Workfront Goals]，活動是目標的進度指標。 它可以是手動更新的進度欄，也可以是與目標關聯的項目。 您不能在報表中顯示活動，也不能通過 [!DNL Workfront] API。 有關活動的資訊，請參見 <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">開始Adobe Workfront目標中的結果和活動</a>。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL實際成本]</td> 
   <td> <p>對於任務和問題，這是與實際記錄的小時數相關的成本，與分配給任務或問題的資源的每小時成本率有關。 對於項目，這是項目任務和問題中所有[!UICONTROL實際成本]的總和。 有關資訊，請參見 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">跟蹤成本</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL實際費用成本]</td> 
   <td> <p>為項目或任務記錄的所有支出的[!UICONTROL實際金額]總和。</p> <b>示例 </b>
   <p>如果為任務1建立費用並在[!UICONTROL實際金額]欄位中輸入$600.00，則此任務的[!UICONTROL實際費用成本]為$600.00。 </p> 
   <p>對於一個項目， [!DNL Workfront] 使用以下公式計算[!UICONTROL實際費用成本]:</p> <p><code>Project Actual Expense Cost = SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs) + Project Fixed Cost</code> <br> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (drafting this because not sure if this is still correct)</p>
    --> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL實際小時數]</td> 
   <td> <p>在項目、任務或發佈報告中，[!UICONTROL實際小時數]是記錄在項目、任務或問題上的所有小時數之和。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span> 如果從任務1的[!UICONTROL更新]頁籤中，按一下「記錄時間」，然後輸入25小時，則任務1的實際小時數= 25小時。 </p> <p>[!DNL Workfront] 使用以下公式計算父任務或項目的[!UICONTROL實際小時數]:</p> 
    <ul> 
     <li> <p><code>For parent tasks = children [!UICONTROL Actual Hours] + [!UICONTROL Actual Hours] on the parent task. </code> </p> </li> 
     <li> <p><code>For projects = [!UICONTROL Actual Hours] logged on the project + [!UICONTROL Actual Hours] logged on standalone or children tasks in the project</code> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL實際人工成本]</td> 
   <td> <p>與在任務或項目中投資的人工關聯的[!UICONTROL實際成本]。 </p> <p>對於任務， [!DNL Workfront] 使用以下公式計算[!UICONTROL實際人工成本]:</p> <p><code>Task [!UICONTROL Actual Labor Cost] = Number of [!UICONTROL Actual Hours] on the task * User or Job Role [!UICONTROL Hourly Cost Rate]</code> </p> <p>如果任務的[!UICONTROL成本類型]為[!UICONTROL用戶小時], [!DNL Workfront] 使用用戶費率。 如果任務的[!UICONTROL成本類型]為[!UICONTROL角色小時], [!DNL Workfront] 使用任務職責費率計算[!UICONTROL實際人工成本]。 </p> <p>對於一個項目， [!DNL Workfront] 使用以下公式計算[!UICONTROL實際人工成本]:</p> <p><code>Project [!UICONTROL Actual Labor Cost] = SUM(All Tasks [!UICONTROL Actual Labor Cost]) </code> </p> <p>有關詳細資訊，請參見 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">跟蹤成本</a>。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span>例如，如果用戶使用[!UICONTROL用戶小時] [!UICONTROL成本類型]記錄任務的5小時，並且其小時費率為$100，則[!UICONTROL實際人工成本]為$500。</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL實際收入] </td> 
   <td> <p>項目或任務的[!UICONTROL實際收入]是與項目或任務的[!UICONTROL實際小時數]關聯的金額。 </p> <p>有關跟蹤收入的資訊 [!DNL Workfront]，請參閱 <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">開單和收入概覽</a>。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL實際開始]</td> 
   <td>用戶更改指定給他們的正在進行的工作對象時的時間戳。</td> 
  </tr> 
  <!--<tr> 
 <td>A type of work process that is unplanned.</td> 
 -->
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Additional Schedules</td> 
    <td>An additional preset to be used for a new user group.</td> 
   </tr>
  --> 
  <tr> 
   <td>[!UICONTROL Agile]方法</td> 
   <td>一種基於需求和解決方案與跨職能團隊協作演變的方法。 它鼓勵基於固定時間表的靈活性和變化。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL敏捷團隊]</td> 
   <td>與傳統團隊不同，因為他們從積壓工作中提取他們的預期工作，並在一段稱為[!UICONTROL迭代]的設定時間內對其進行處理。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL我的所有團隊]</td> 
   <td> <p>在[!UICONTROL篩選器]中引用此選項時，此欄位顯示屬於登錄用戶所屬任何團隊的用戶，或分配給登錄用戶所屬任何團隊的工作項。 </p> <p>建議在與其他用戶共用報告時在篩選器中使用此欄位使報告更一般。 這樣，您只能生成一個報告，該報告將根據登錄者來查看該報告的不同資訊，因為該資訊始終是為登錄用戶自定義的。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL分配日期]</td> 
   <td> <p>您可以在以下類型的報告中找到此欄位：</p> 
    <ul> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates</li>
     --> 
     <li>[!UICONTROL項目]（財務資料）</li> 
     <li>[!UICONTROL預算小時]</li> 
    </ul> <p>對於<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Resource Estimates or 
      </MadCap:conditionalText>
     -->[!UICONTROL項目（財務資料）]報告： </p> 
    <ul> 
     <li>嘗試瞭解時生成此報告 <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         how resources are budgeted for work, or 
       </MadCap:conditionalText>
      --> 分配給您的資源的[!UICONTROL計畫小時數]的量。</li> 
     <li> <p>[!UICONTROL分配日期]是一週的第一天（星期日），此時將開始向任務分配[!UICONTROL作業角色]。 資源（[!UICONTROL作業角色]）在分配給它的任務的[!UICONTROL持續時間]中具有的[!UICONTROL分配日期]可以與它具有的周數相同。 如果任務跨過多個月，則一個月的第一天也可以變成[!UICONTROL分配日期]，如果它在任務的[!UICONTROL持續時間]內。</p> <p>例如，您可以將[!UICONTROL作業角色]分配給跨3週且具有90 [!UICONTROL計畫小時數]的任務。 這些小時數在任務期間平均分佈，這使每天將6 [!UICONTROL計畫小時數]分配給您的工作角色：</p> <p><em> [!UICONTROL每日計畫小時數] = [!UICONTROL總計計畫小時數]/任務[!UICONTROL工作日數]期間的[!UICONTROL工作日數] </em> </p> <p>因此，有三個[!UICONTROL分配日期]，在任務的[!UICONTROL持續時間]期間，每週的每個星期日都有一個，每個日期與它們關聯的[!UICONTROL計畫小時數]一定數目。<br>如果任務在一個月的最後一週的中間開始，並在新月開始後兩週結束，則任務將具有四個[!UICONTROL分配日期]:在任務的[!UICONTROL持續時間]期間，每週的每個星期日都有一個，在新月的第一天有一個。</p> <p>為充分利用此資訊，我們建議您 <!--
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          Resource Estimates or a 
        </MadCap:conditionalText>
       --> 項目（財務資料）報告並為[!UICONTROL分配日期]添加矩陣分組，然後對結果按周、每月、季度或每年分組以獲得最準確的資料。<br>有關構建矩陣分組的資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md" class="MCXref xref">建立矩陣報表</a>。</p> </li> 
    </ul> <p>財務資訊僅在與[!UICONTROL項目（財務資料）]關聯的資料不到5年時才填充到報表中。 例如，如果作業角色在2015年1月分配給任務，而今天是2021年9月，則像作業角色的[!UICONTROL分配日期]這樣的財務欄位不會填充在[!UICONTROL項目（財務資料）]報告中。 </p> 
    <div> 
     <p>對於[!UICONTROL預算小時]報告：</p> 
     <ul> 
      <li>在嘗試瞭解分配給您的資源或資源計畫器中的項目的[!UICONTROL預算小時數]金額時，生成此報表。</li> 
      <li> <p>[!UICONTROL分配日期]是您在[!UICONTROL資源規劃器]中預算小時數的星期初（星期日）。 </p> <p>提示：   <p>如果一週跨度為兩個月，它將在報告中生成兩行：一個對應於周的第一天（第一週的星期日，即第一個月），第二行顯示第二個月的第一天。 </p> <p>例如，如果您為用戶預算6月30日（星期日） — 7月6日（星期六）這一週的8小時，則兩行將顯示6月30日和7月1日的[!UICONTROL分配日期]。 </p> </p> <p>有關中預算資源的資訊 [!DNL Resource Planner]，請參閱文章 <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">預算資源 [!DNL Resource Planner] 使用[!UICONTROL項目]和[!UICONTROL角色]視圖</a>。</p> <p>有關生成[!UICONTROL預算小時數]報告的資訊，請參見 <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">報告：預算工時</a>。 </p> </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL公告]</td> 
   <td> <p>一種與系統內的用戶資訊通信的方法。 這些資訊通常來自 [!DNL Workfront] 從管理員到用戶。 </p> <p>有關詳細資訊，請參見 <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">發送通知</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL應用整合]</td> 
   <td>應用最常代表軟體應用程式的連接器，但也可以代表處理資料的特殊功能。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL批准者決定]</td> 
   <td> <p>在[!UICONTROL校樣批准]報告中，此欄位顯示不再有效校樣的校樣批准決定。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL批准者階段]</td> 
   <td>在[!UICONTROL校樣批准報告]中，此欄位顯示有關當前階段校樣的資訊。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL批准]</td> 
   <td> <p>給定工作項（如任務、文檔或時間表）可能要求主管或其他用戶在工作項上簽名。 此註銷過程稱為批准。 </p> <p>有關詳細資訊，請參見 <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">審批流程概述</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL批准日期]</td> 
   <td>在[!UICONTROL證明批准]報告中，此欄位顯示批准證明的日期。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL批准者]</td> 
   <td>必須在給定工作項上註銷的用戶或作業角色，或批准工時單上的工時條目的用戶。</td> 
  </tr> 
  <tr> 
   <td>[！分配給的UICONTROL]</td> 
   <td> <p>在[!UICONTROL任務或問題]報告中，此欄位顯示任務或問題的所有者或[!UICONTROL主要受分配者]。 您也可以按此欄位進行篩選或分組。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL賦值]</td> 
   <td>分配給問題或任務的用戶、作業角色或團隊。 項目、項目組或項目群不能有分配。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL分配]</td> 
   <td> <p>在[!UICONTROL任務]或[!UICONTROL問題]報告中，此欄位顯示分配給該任務或問題的所有實體（用戶、作業角色、團隊）的清單。 可以使用欄位[!UICONTROL分配用戶]和[!UICONTROL分配角色]按此欄位進行篩選。 您可以使用「團隊」(Team)欄位按分配給任務或問題的團隊進行篩選。 不能按此欄位對報表進行分組。</p> <p>已放在[!UICONTROL資源回收筒]中的工作項將繼續顯示在引用[!UICONTROL分配]對象的某些報告中，其中 [!DNL OR] 篩選器修飾符被使用。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL分配角色]</td> 
   <td>
   <p>在[!UICONTROL任務]或[!UICONTROL問題]報告中，此欄位顯示有關分配給任務或問題的作業角色的資訊。 此欄位顯示[!UICONTROL主要所有者]以及分配給任務或問題的其他作業角色。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL分配狀態]</td> 
   <td> <p>在分配、任務或發佈報告中，[!UICONTROL分配狀態]顯示分配給工作項的用戶是按一下了[!UICONTROL Work On It]按鈕還是按一下[!UICONTROL Done]按鈕來接受或完成該工作。 存在以下[!UICONTROL分配狀態]:</p> 
    <ul> 
     <li><b>[！請求的UICONTROL]</b>:用戶已分配給該任務或問題，但他們尚未按一下[!UICONTROL Work On It]按鈕開始處理它。</li> 
     <li><b>[!UICONTROL工作]</b>:用戶已按一下[!UICONTROL Work On It]按鈕，當前正在處理該項。 </li> 
     <li><b>[!UICONTROL完成]</b>:用戶已按一下[!UICONTROL Done]按鈕，並已完成對該項的工作。 </li> 
    </ul> <p>有關詳細資訊，請參見 <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/work-on-it-and-done-buttons-accept-complete-work.md" class="MCXref xref">[!UICONTROL Work On It]和[!UICONTROL Done]按鈕概述</a>。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL分配團隊]</td> 
   <td>
   <p>在[!UICONTROL任務]或[!UICONTROL問題]報告中，此欄位顯示有關分配給任務或問題的團隊的資訊。 該欄位顯示[!UICONTROL主要所有者]以及分配給任務或問題的其他團隊。 </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL分配用戶]</td> 
   <td>
   <p>在[!UICONTROL任務]或[!UICONTROL問題]報告中，此欄位顯示有關分配給任務或問題的用戶的資訊。 此欄位顯示[!UICONTROL主要所有者]以及分配給任務或問題的其他用戶。 </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL屬性]</td> 
   <td>屬性是 [!DNL Workfront] 的雙曲餘切值。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL審核區域]</td> 
   <td> <p>審計是記錄在Workfront發生的操作的系統消息。 記錄了以下審計類型：</p> 
    <ul> 
     <li>[!UICONTROL範圍更改]</li> 
     <li>[!UICONTROL附件操作]</li> 
     <li>[!UICONTROL常規編輯]</li> 
     <li>[!UICONTROL狀態更改]</li> 
     <li>[!UICONTROL注釋]</li> 
     <li>[!UICONTROL組合項]</li> 
     <li>[!UICONTROL錯誤條目]</li> 
     <li>[!UICONTROL狀態更改]</li> 
     <li>[!UICONTROL訂閱更改]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL審核跟蹤]</td> 
   <td>通過記錄的更改（[!UICONTROL審計區域]）跟蹤的事件自動生成的注釋的集合。 每張紙條都記錄了誰做了這件事，他們做了什麼，以及他們做了什麼。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL自動和更改時]</td> 
   <td> <p>[!UICONTROL項目更新]類型之一。 這將在夜間重新計算流程運行時以及對項目內的項目或任務進行任何更新時重新計算項目的預計時間表和計畫時間表。 </p> <p>有關詳細資訊，請參見 <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">選擇項目更新類型 </a>。</p> </td> 
  </tr>

<tr> 
   <td><p>可用性</p></td> 
   <td> <p>此術語用於「用戶可用性」或「資源可用性」，它說明了資源（用戶或作業角色）可用於工作的時間量。 </p> 
   <p>Workfront使用多個欄位計算用戶可用性，具體取決於系統中資源管理首選項的設定。 有關詳細資訊，請參見 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">配置資源管理首選項</a>。 </p>
   <p>有關資源可用性的詳細資訊，請參見 <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">資源管理入門</a></p>
   或者，「容量」也用於指資源可用性。 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL僅自動]</td> 
   <td> <p>[!UICONTROL項目更新]類型之一。 此操作將在夜間重新計算流程運行時重新計算預計時間線和計畫時間線。</p> <p>有關詳細資訊，請參見 <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">選擇項目更新類型</a>。</p> </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL BAU]</td> 
   <td>「一切照常」工作，有助於實現日常主要業務目標。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL積壓工作]</td> 
   <td>在敏捷環境中，新問題會一直保留到準備解決。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL基線]</td> 
   <td>在靈活環境中度量迭代的資料源。</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL計費記錄]</td> 
   <td> <p>記錄可開單的收入、小時數或費用。 此資訊可用於在外部會計系統中建立發票。</p> <p>有關詳細資訊，請參見 <a href="../../../manage-work/projects/project-finances/create-billing-records.md">建立開單記錄</a>。 </p> 
   </td> 
  </tr>

<tr> 
   <td>開單記錄狀態</td> 
   <td> <p>在「開單記錄」或「小時」報表中，開單記錄的狀態指明開單記錄是否已開單或未開單。 您不能刪除與開單記錄關聯的項目或編輯時間。 有關詳細資訊，請參見 <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >建立開單記錄</a>。</p>  
   </td> 
  </tr>


<tr> 
   <td>[!UICONTROL品牌推廣]</td> 
   <td><p>定制過程 [!DNL Workfront] 使介面具有通過使用顏色和徽標來鏡像貴公司的外觀。</p><p><strong>注釋</strong><br>如果您的組織已連接到 [!DNL Adobe Experience Cloud]，品牌推廣不可用。</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Breadcrumbs]</td> 
   <td> <p>頁面頂部顯示用戶在應用程式中的分層位置的區域。</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">有關詳細資訊，請參見 <a href="../../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">Breadcrumbs概述</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL預算狀態]</td> 
   <td> <p>這是一個已棄用的欄位。 此欄位可能顯示的任何資訊都與某個功能相關 [!DNL Workfront] 已刪除，無法更新該欄位。 </p> <p>此欄位顯示項目是否已添加到[!UICONTROL能力規劃器]，以及是否已為其完成預算計算。 已從中刪除[!UICONTROL容量規劃器] [!DNL Workfront]。 </p> 
    <ul> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">If the project is&nbsp;not added to the capacity planner, its value is <i>Not Included</i>.&nbsp;</li>
     --> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">If the project is&nbsp;added to the Capacity Planner but is excluded from the budget calculation,&nbsp;the value is <i>Included but not Calculated</i>.&nbsp;</li>
     --> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> If the project is&nbsp;added to the Capacity Planner and included in the budget calculation, the value is <i>Included and Calculated</i>. </li>
     --> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL預算完成日期]</td> 
   <td> <p>這是一個已棄用的欄位。 此欄位可能顯示的任何資訊都與某個功能相關 [!DNL Workfront] 已刪除。 無法更新此欄位。 </p>
   <p> 此欄位在[!UICONTROL項目]和[!UICONTROL任務]報告和清單中仍可見。</p>  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL預算成本]</td>

<td> <p>這是與項目預算資源關聯的成本。 </p>
   <p>該欄位顯示在以下區域 [!DNL Workfront] 的下界：</p>
   <ul>
   <li><strong>[!UICONTROL預算成本]</strong>:在[!UICONTROL業務案例摘要]面板中</li>
   <li><strong>[!UICONTROL成本]</strong>:在[!UICONTROL成本]查看資訊時在[!UICONTROL利用率]區域中</li>
   <li><strong>[!UICONTROL項目預算成本]</strong>:清單和報表</li>
   </ul>   
    <p>項目的[!UICONTROL預算成本]使用以下公式計算：</p> 
    <p><code>[!UICONTROL Project Budgeted Cost] (or [!UICONTROL Budgeted Cost]) = [!UICONTROL Budgeted Expense Cost] + [!UICONTROL Budgeted Labor Cost] + [!UICONTROL Fixed Cost] of the project</code> </p> 
    <p>有關計算[!UICONTROL預算成本]的詳細資訊，以及瞭解中此概念的各種名稱 [!DNL Workfront]，請參閱 <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">計算項目預算成本</a>。 </p>
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL預算小時數]</td> 
   <td> <p>為項目上需要完成的工作的資源編入預算的小時數。 此欄位指在項目或項目資源的[!UICONTROL業務案例]（或在[!UICONTROL資源規劃器]）的[!UICONTROL資源預算]區域中預算的小時數。</p> <p>有關詳細資訊，請參見 <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">瞭解項目的[!UICONTROL預算人工成本]和[!UICONTROL預算工時]</a>。 </p> 
    <!-- 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Hours that were formerly budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner)</p>
    <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
  -->
    <p> 有關預算中用戶的資訊 [!DNL Resource Planner]，請參閱文章 <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">預算資源 [!DNL Resource Planner] 使用[!UICONTROL項目]和[!UICONTROL角色]視圖</a>。 </p> 
    <p>[!UICONTROL業務案例]或[!UICONTROL資源規劃器]的[!UICONTROL資源預算]區域中預算的小時數顯示在以下區域中 [!DNL Workfront] 名稱：</p> 
     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td><strong>[!UICONTROL預算小時數]顯示名稱</strong></td> 
        <td><strong>區域 [!DNL Workfront]</strong></td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL小時]</td> 
        <td>[!UICONTROL業務案例]的[!UICONTROL資源預算]區域</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL BDG]</td> 
        <td>[!UICONTROL資源規劃器]已通過[!UICONTROL小時數]查看</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL預算小時數]</td> 
        <td> <p>利用率報告[!UICONTROL小時數]視圖</p> <p>有關[!UICONTROL利用率]報告的詳細資訊，請參見文章 <a href="../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md" class="MCXref xref">[!UICONTROL資源利用率]報告概述</a>。</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Bud。 時數]</td> 
        <td> <p>[!UICONTROL預算小時]報告</p><p>「預算工時」報告中的[!UICONTROL預算工時]對象引用與已過時的資源管理工具相關的資訊。 僅"[!UICONTROL Bud。 此報表中的「小時數」欄位指在項目[!UICONTROL Resource Planner]或[!UICONTROL Resource Budgeting]區域中預算的小時數。 </p> <p>有關建立報告的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">建立自定義報告</a>。</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL資源規劃器預算小時數] </td> 
        <td> <p>在以下報告中找到：</p>
        <ul>
        <li>[!UICONTROL項目]報告
        <li>[!UICONTROL項目（財務資料）]報告
        <li>[!UICONTROL任務]報告
        <li>[!UICONTROL問題]報告
        <li>[!UICONTROL預算小時]報告</li>
        </ul>
         <p>有關建立報告的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">建立自定義報告</a>。</p> </td> 
       </tr> 
      </tbody> 
     </table> 
    <p>在中提到的[!UICONTROL預算小時數] [!DNL Adobe Workfront] 指使用已從Workfront刪除的過時功能編入預算的小時數。 這些欄位是僅查看欄位，在使用當前資源預算工具時不會使用當前資訊進行更新。 </p>
    <!--<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Hours from theResource Planner in the areas and reports listed below. </p>
     <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Planner Hours view (in the BDG column)</li>
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Utilization report Hours view</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Budgeting area of the Business Case (in the Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report (the Bud. Hours field refers to hours budgeted for users; the Pln. Bud. Hours field refers to hours budgeted for roles or projects)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (in the Project: Budgeted Hours field) </li>
        </ul>
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The fields listed below display in the reports listed and are hours formerly budgeted in the&nbsp;Capacity Planner or the Legacy Resource Estimates area of the Business Case.</p>
         <p>Important: The Capacity Planner and Legacy&nbsp;Resource Estimates have been removed from Workfront. You cannot update any information that might display in these fields.</p>
        <ul>
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Capacity Planner</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Legacy&nbsp;Resource Estimates area of the Business Case (in the Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (in the Bud. Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report (in the Budgeted Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report (in the Budgeted Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project (Financial&nbsp;Data) report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task&nbsp;report (in the Project: Budgeted Hours field)</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report (in the Project: Budgeted Hours field)</li>
      </ul> --> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL預算人工成本]</td> 
   <td> <p>這是與您作為資源經理完成項目所需工作的職務職責預算的小時數關聯的成本。 </p> <p>項目報表中的[!UICONTROL預算人工成本]使用以下公式計算：</p> <p><code style="font-style: normal;">[!UICONTROL Budgeted Labor Cost] = SUM([!UICONTROL Job Role Cost] per [!UICONTROL Hour] * [!UICONTROL Budgeted Hours] per [!UICONTROL Job Role])</code> </p> <p>此欄位可以引用以下內容：</p> 
    <ul> 
     <li> <p>在[!UICONTROL業務案例]的[!UICONTROL資源預算]區域或與項目上任務職責成本關聯的[!UICONTROL資源計畫器]中顯示的人工成本。 有關計算[!UICONTROL預算人工成本]的資訊，請參閱文章 <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">[!UICONTROL瞭解項目的預算人工成本]和[!UICONTROL預算工時]</a></p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>在[!UICONTROL業務案例]的[!UICONTROL資源預算]區域中顯示的人工成本，反映與項目連結的方案中的[!UICONTROL人員成本]估計的人工成本 [!DNL Scenario Planner] 使用方案計畫器來預算項目資源時。 有關方案的資訊，請參見 <a href="../../../scenario-planner/initiatives-overview.md" class="MCXref xref">方案規劃器中的方案概覽</a>。 </p> <p>的 [!DNL Scenario Planner] 需要額外的許可證。 有關 [!DNL Workfront Scenario Planner]，請參閱 <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">的 [!DNL Scenario Planner] 概述</a>。 </p> </li> 
     <p>它顯示在以下名稱下的以下區域：</p>
   <ul>
   <li><strong>[!UICONTROL預算人工成本]</strong>:在[!UICONTROL業務案例]的[!UICONTROL資源預算]區域中。
   <li><strong>[!UICONTROL預算成本]</strong>:在[!UICONTROL利用率]報告[!UICONTROL成本]視圖中
   <p>有關詳細資訊，請參見 <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">查看資源利用率資訊 </a>。</p>
   <li><strong>[!UICONTROL BDG]</strong>:的 [!DNL Resource Planner] 項目或 [!DNL Role] 視圖，按成本查看時
   <li><strong>[!DNL Resource Planner Budgeted Labor Cost]</strong>:在以下報告中： 
   <ul>
    <li>[!UICONTROL項目]報告</li>
    <li>[!UICONTROL項目（財務資料）]報告</li>
    <li>[!UICONTROL任務]報告</li>
    <li>[!UICONTROL問題]報告</li>
    <li>[!UICONTROL預算小時]報告</li> 
    </ul>
    <p>有關建立報告的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">建立自定義報告</a>。</p>
    <!--
          <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Labor costs for hours budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner). This was available only in Adobe Workfront Classic. </p>
           <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
       </li> 
    </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Labor Cost field based on the hours budgeted in the Resource Planner in the following areas and reports in&nbsp;Workfront: </p>
        <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Planner Cost view (in the BDG column)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Utilization report Cost view (in the Budgeted Cost column)</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Budgeting area of the Business Case </li>
         </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Labor Cost associated with resources budgeted in the Resource Planner in the Resource Planner Resource Budgeted Cost field in the following reports: </p>
       <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report </li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task&nbsp;report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report</li>
         </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate a Budgeted Labor Cost field that contains information from a tool that has been deprecated in the reports listed below. You can no longer update the fields displayed in these reports and budgeting your resources on the projects does not update them: </p>
        <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report </li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task&nbsp;report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report</li>
         </ul>      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about calculating the Budgeted Labor Cost, see the article <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a>&nbsp;.&nbsp;</p>
    --> 
    </td> 
   </tr> 
   <tr> 
   <td>[!UICONTROL預算開始日期]</td> 
  <td> <p>這是一個已棄用的欄位。 此欄位可能顯示的任何資訊都與某個功能相關 [!DNL Workfront] 已刪除。 無法更新此欄位。</p>
  <p>這些區域已從 [!DNL Workfront]。 </p> 
  <p>該欄位在[!UICONTROL項目]和[!UICONTROL任務]報告和清單中仍可見。</p>
   <!--
   <p>This field shows the date when the budgeting of resources starts, as defined in the Legacy Resource Estimates area of the Business Case of a project, or the Capacity Planner.</p>
   -->   
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL燃耗圖]</td> 
   <td>提供已完成和剩餘工作的可視表示的折線圖。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL業務案例]</td> 
   <td> <p>用於評估項目是否應從[!UICONTROL Idea]狀態前移到[!UICONTROL Planning]狀態的工具。 換句話說，[!UICONTROL業務案例]可幫助組織確定啟動和完成項目是否值得，尤其是在將項目與產品組合中的其他項目進行比較時。</p> <p>有關詳細資訊，請參見 <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">為項目建立[!UICONTROL業務案例] </a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL業務案例預算小時數]</td> 
   <td> <p>這是一個已棄用的欄位。 此欄位可能顯示的任何資訊都與某個功能相關 [!DNL Workfront] 已刪除。 無法更新此欄位。</p> <p>此欄位在項目和[!UICONTROL任務]清單和報表中仍可見。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL計算分配]</td> 
   <td> <p>任務[!UICONTROL持續時間]類型之一。 這將根據任務的[!UICONTROL持續時間]和[!UICONTROL需要的工時]計算分配給任務的用戶將分配給任務的8小時工作日的百分比。</p> <p>有關詳細資訊，請參見 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任務[!UICONTROL持續時間]和[!UICONTROL持續時間類型]概覽</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL計算工作]</td> 
   <td> <p>任務[!UICONTROL持續時間類型]之一。 這將計算任務的[!UICONTROL需要的工作]，給定[!UICONTROL持續時間]和用戶[!UICONTROL分配]百分比（基於8小時工作日）。</p> <p>有關詳細資訊，請參見 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任務[!UICONTROL持續時間]和[!UICONTROL持續時間類型]概覽</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL日曆]</td> 
   <td> <p>中有兩種日曆 [!DNL Workfront]:[!UICONTROL主日曆]和日曆報表。</p> <p>[!UICONTROL主日曆]是個人日曆，允許用戶根據其可用時間管理其工作負載 [!DNL Workfront]。 用戶還可以將其[!UICONTROL主日曆]與 [!DNL Outlook] ([!DNL Google] 和 [!DNL Microsoft] 整合即將到來)。 </p> <p>有關[!UICONTROL主日曆]的詳細資訊，請參見 <a href="../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md" class="MCXref xref">[!UICONTROL主日曆]視圖</a>。</p> <p>日曆報表是動態報表，用戶可以在其中查看事件的日期和其他重要詳細資訊，包括到期日期、工作狀態以及事件分配給的用戶。</p> <p> 有關日曆報表的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md" class="MCXref xref">日曆報表概述</a>。</p> </td> 
  </tr> 
   <tr> 
   <td>[!UICONTROL可以啟動]</td> 
   <td> <p>此欄位指示任務是否準備開始處理。 如果開始已準備好在任務的[!UICONTROL Can Start]欄位上工作，則將其設定為[!UICONTROL True]。 </p> <p>有關詳細資訊，請參見 <a href="../../../manage-work/tasks/task-information/can-start-task-overview.md" class="MCXref xref">"[!UICONTROL可以啟動]"任務概述</a>。</p> 
   <!--
     <p>(NOTE: everything below is drafted because I created a new article linked above with all this information - it was getting kind of too big for just a table cell)</p>
    --> <!--
     <p>Workfront checks for the following things before it marks a task as True for the Can Start field:<br></p>
    --> 
    <!--
     <ul> 
      <li> If the task has a parent, it checks to see if the value of Can Start for the parent it set to True. If the value for the parent is False, then all the subtasks have the value of Can Start set to False, as well.&nbsp;</li> 
      <li> It also checks to see if the predecessors of the task as well as the predecessors of their parents are complete. If they are complete, the Can Start value for the task is set to True. If any of the task predecessors or their parents' predecessors are not complete, or have a status of Complete-Pending Approval, then the Can Start value for the task is set to False.&nbsp;</li> 
     </ul>
    --> 
    <!--
     <p>For information about task predecessors, see <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Overview of task predecessors</a>.</p>
    --> <!--
     <p>Tip: If the Dependency Type between a task and its predecessors is Start-Start, the predecessor must start before the predecessor relationship is considered resolved and the successor tasks can start. For information about dependency types, see <a href="../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md" class="MCXref xref">Overview of task dependency types</a>. </p>
    --> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Capacity</td> 
    <td>The total availability (measure in either hours or FTE) of a designated user, resource pool, team, rob role, or company.</td> 
   </tr>
  -->

<tr> 
   <td> <p>能力</p> </td> 
   <td> <p>資源可分配給工作的可用時間。 請參閱「可用性」。 </p></td> 
  </tr>

<tr> 
   <td> <p>[!UICONTROL類別]</p> </td> 
   <td> <p>類別是自定義窗體。 您可以生成此對象的報告，也可以在其他對象報告中顯示它。 並非所有對象都可以具有自定義窗體或類別。 以下對象可以具有自定義窗體： <br></p> 
    <ul> 
     <li>[!UICONTROL項目]</li> 
     <li>[!UICONTROL任務]</li> 
     <li>[!UICONTROL問題]</li> 
     <li>[!UICONTROLPortfolio]</li> 
     <li>[!UICONTROL文檔]</li> 
     <li>[!UICONTROL支出]</li> 
     <li>[!UICONTROL程式]</li> 
     <li>[!UICONTROL用戶]</li> 
     <li>[!UICONTROL公司]</li> 
     <li>[!UICONTROL迭代]</li></ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL類別名稱]</td> 
   <td> <p>當作為列添加到以下任意對象的視圖中時，它將顯示與這些對象關聯的所有自定義表單的清單：</p> 
    <ul> 
     <li>[!UICONTROL項目]</li> 
     <li>[!UICONTROL任務]<br></li> 
     <li>[!UICONTROL問題]<br></li> 
     <li>[!UICONTROLPortfolio]<br></li> 
     <li>[!UICONTROL文檔]<br></li> 
     <li>[!UICONTROL支出]<br></li> 
     <li>[!UICONTROL程式]<br></li> 
     <li>[!UICONTROL用戶]<br></li> 
     <li>[!UICONTROL公司]</li> 
     <li>[!UICONTROL迭代]</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL更改管理]</td> 
   <td>實踐領域側重於定義、理解和調整計畫工作以適應範圍、計畫、成本和資源因素的變化。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL更改順序]</td> 
   <td>針對概述對商定範圍所要求的更改的項目提出的問題類型。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL僅更改]</td> 
   <td>項目[!UICONTROL更新類型]之一。 在對「任務」進行更新或對「項目」或「任務」執行編輯時，它只更新[!UICONTROL項目投影]和[!UICONTROL計畫]時間表。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL更改順序]</td> 
   <td> <p>[!UICONTROL問題]類型之一，通常表示必須在項目完成之前完成計畫外的工作量。</p> <p>有關[!UICONTROL問題]類型的詳細資訊，請參閱文章中的「預設問題類型」一節 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md" class="MCXref xref">自定義預設問題類型</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL子任務]</td> 
   <td>作為[!UICONTROL父任務]（[!UICONTROL摘要任務]）的[!UICONTROL子任務]的任務。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL子級]</td> 
   <td>[!UICONTROL子任務]到[!UICONTROL父任務]（[!UICONTROL摘要任務]）的集合。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Coaching]和[!UICONTROL Training]</td> 
   <td>學習模組、認證、標準或實踐團體。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL提交]</td> 
   <td>一種通信工具，用於用戶設定對任務交付件的期望。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL提交日期]</td> 
   <td>一種通信工具，用於用戶圍繞任務交付項設定期望值。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL通信]和[!UICONTROL報告]</td> 
   <td>審查項目、項目群或項目組合的例外和運行狀況的標準</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL公司]</td> 
   <td> <p>[!UICONTROL公司]是中的組織單位 [!DNL Workfront]。 </p> 
   <p> 您可以將用戶或項目與一家公司關聯。 有關詳細資訊，請參見 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md">建立和編輯公司</a>。</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL完成日期]</td> 
   <td> <p>項目、任務或發放設定為完成的日期。 中有幾種類型的[!UICONTROL完成日期] [!DNL Workfront]:</p> 
    <ul> 
     <li>[!UICONTROL實際完成日期]。 有關詳細資訊，請參見 <a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">項目[!UICONTROL實際完成日期]概覽 </a>。</li> 
     <li>[!UICONTROL計畫完成日期]。 有關詳細資訊，請參見 <a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">設定項目[!UICONTROL計畫完成日期]</a> 和 <a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">任務[!UICONTROL計畫完成日期]概覽</a>。</li> 
     <li>[!UICONTROL投影完成日期]。 有關詳細資訊，請參見 <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">項目、任務和問題的[!UICONTROL預計完成日期]概覽</a>。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL完成日]</td> 
   <td>相對於[!UICONTROL模板]的開頭，[!UICONTROL模板任務]或[!UICONTROL模板]應該完成的日期。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL完成模式]</td> 
   <td> <p>這表示項目將如何標籤為[!UICONTROL完成]。 它可以有兩個值：</p> 
    <ul> 
     <li>[!UICONTROL手冊]:用戶必須將項目狀態更改為[!UICONTROL完成]。</li> 
     <li>[!UICONTROL自動]:當項目中的所有任務全部完成且所有問題都已結束時，項目狀態將自動更改為[!UICONTROL完成]。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL條件]</td> 
   <td> <p>這是任務、問題或項目進度的直觀表示。</p> <p>對於項目，條件可由項目所有者手動設定，也可由 [!DNL Workfront]，根據項目進度狀態。 </p> <p>項目條件的可能值為：</p> 
    <ul> 
     <li>[！目標上的UICONTROL]</li> 
     <li>[!UICONTROL面臨風險]</li> 
     <li>[!UICONTROL遇到故障]</li> 
    </ul> <p>有關項目條件的詳細資訊，請參閱文章 <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">[!UICONTROL項目條件]和[!UICONTROL條件類型]概述</a>。</p>
     <p>您可以將任務和發放條件與可在報表中顯示的數字相關聯。 下面的清單顯示任務和問題條件的預設名稱和編號。 系統管理員可以更新條件的名稱，並且他們可以添加具有不同編號的新條件。 將數字與條件關聯後，無法編輯該數字。  </p> 
     <p>對於任務，條件由任務所有者手動設定。 任務條件的可能值為：</p> 
    <ul> 
     <li>[!UICONTROL正平滑前進](0)<br></li> 
     <li> [!UICONTROL某些關注點](1)<br></li> 
     <li>[!UICONTROL主要路障](2)</li> 
    </ul> <p>有關任務條件的詳細資訊，請參閱文章 <a href="../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">更新[!UICONTROL條件]以瞭解任務和問題</a>。</p> <p>對於問題，條件由問題所有者手動設定。 問題條件的可能值為：<br></p> 
    <ul> 
     <li>[!UICONTROL正平滑前進](0)<br></li> 
     <li>[!UICONTROL某些關注點](1)<br></li> 
     <li>[!UICONTROL主要路障](2)</li> 
    </ul> 
   <p><b>附註</b></p>
    <p>在[!UICONTROL日誌條目]報告中跟蹤[!UICONTROL條件]欄位時，[!UICONTROL New]和[!UICONTROL舊數值值]將顯示與該條件關聯的數字，而不是其名稱。 如果最初沒有為任務或問題定義條件，而您稍後會更新它，則捕獲更新的日誌條目將將[!UICONTROL條件]欄位的[!UICONTROL舊數值]顯示為–2,147,483,648。 另請參見本文中的「[!UICONTROL新編號值]」、「[!UICONTROL舊編號值]」和「[!UICONTROL日誌條目]」。 </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL條件更新]</td> 
   <td> <p>此欄位顯示任務、項目或問題的當前狀態。 此選項顯示任務、項目或問題的所有者在[!UICONTROL更新狀態]欄位中提供的最新更新以及新條件。</p> <p>在[!UICONTROL條件更新]列中不顯示對條件更新所做的注釋；只顯示主更新。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL約束日期]</td> 
   <td> <p>如果您使用與特定日期（如[!UICONTROL必須開始]）相關的[!UICONTROL任務約束]，則該特定日期將成為任務的[!UICONTROL約束日期]。</p> <p>以下任務約束更新[!UICONTROL約束日期]欄位：</p> 
    <ul> 
     <li>[!UICONTROL必須在開始]</li> 
     <li>[!UICONTROL必須在完成時完成]</li> 
     <li>[!UICONTROL開始時間不晚於]</li> 
     <li>[!UICONTROL開始時間不早於]</li> 
    </ul> <p>提示：   
     <ul> 
      <li> <p>具有[!UICONTROL約束]的[!UICONTROL固定日期]的任務沒有[!UICONTROL約束日期]。 </p> </li> 
      <li> <p> [!UICONTROL約束日期]只能在報表或自定義視圖中查看。</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL約束日]</td> 
   <td> <p>如果在與特定日期（如必須開始日期）關聯的模板任務中使用任務約束，則該特定日期將成為模板任務的約束日。</p> <p>以下任務約束更新[!UICONTROL約束日]欄位：</p> 
    <ul> 
     <li>[!UICONTROL必須在開始]</li> 
     <li>[!UICONTROL必須在完成時完成]</li> 
     <li>[!UICONTROL開始時間不晚於]</li> 
     <li>[!UICONTROL開始時間不早於]</li> 
    </ul> <p>提示：[!UICONTROL約束日]只能在報表或自定義視圖中查看。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL約束類型]</td> 
   <td> <p>任務的計畫趨勢。 例如，[!UICONTROL Op Op Op Op Op Op Op Op Op Op Op Op Op Op Op Op Op Tan]將安排一個任務盡快開始，並且[!UICONTROL Finish Op Op Op Op Th]將一個任務安排在[! OP OP OP OP OP OP ON OP OP OP OP OP OP OP OP OP ON OP O O ON OP ON OP OP O O O O O O O O O O OP O O O O O O O O O O O O O O O O O O O O</p> <p>有關詳細資訊，請參見 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">[!UICONTROL任務約束]概述</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL上下文菜單]</td> 
   <td>位於螢幕左側的菜單，其上的項目將更改為與活動內容相關聯。 例如，當用戶查看項目時，[!UICONTROL上下文菜單]將顯示指向與項目相關的資訊和工具的連結。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL已轉換問題發起方]</td> 
   <td>項目或任務報告中的欄位，顯示有關將問題轉換為項目或任務時屬於問題[!UICONTROL主要聯繫人]的用戶的資訊。 該欄位還顯示在[!UICONTROL項目詳細資訊]節中，其中顯示已轉換問題的[!UICONTROL主要聯繫人]的名稱。 另請參見本文中的「[!UICONTROL主聯繫人]」。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL成本]</td> 
   <td> <p>完成項目、任務或發放時必須花費的貨幣金額。 </p> <p>您可以跟蹤與項目相關的人工、費用和風險的各種成本類型。有關跟蹤中成本的資訊 [!DNL Workfront] 見 <a href="../../../manage-work/projects/project-finances/track-costs.md">跟蹤成本</a>。</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL成本類型]</td> 
   <td>對於任務，[!UICONTROL成本類型]確定任務將如何應計成本。 一些示例包括[!UICONTROL固定小時]、[!UICONTROL用戶小時]和[!UICONTROL用戶小時加固定]。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL跨項目依賴項]</td> 
   <td> <p>一個項目的任務依賴於來自另一個項目的任務。</p> <p>有關詳細資訊，請參見 <a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref">建立跨項目前置任務</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL自定義資料]</td> 
   <td> <p>組織獨有的資料。 組織可以自定義 [!DNL Workfront] 建立自定義表單和自定義域。 此自定義資訊可推動KPI 、審核和需求組合的報告。 </p> <p>[!UICONTROL自定義資料]可以連結到：</p> 
    <ul> 
     <li>[!UICONTROL項目]</li> 
     <li>[!UICONTROL任務]</li> 
     <li>[!UICONTROL用戶]</li> 
     <li>[!UICONTROL公司]</li> 
     <li>[!UICONTROL問題]</li> 
     <li>[!UICONTROL文檔]</li> 
     <li>[!UICONTROL費用]</li> 
     <li>[!UICONTROLPortfolio]</li> 
     <li>[!UICONTROL程式]</li> 
     <li>[!UICONTROL迭代]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL自定義資料類型]</td> 
   <td>指定[!UICONTROL自定義資料]欄位是否以文本、日期、數字或貨幣形式儲存在資料庫中的選項。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL自定義顯示類型]</td> 
   <td>自定義欄位的欄位顯示類型。 示例包括[!UICONTROL下拉清單]、[!UICONTROL文本欄位]、[!UICONTROL文本區域]、[!UICONTROL單選按鈕]等。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL自定義欄位]</td> 
   <td>對於允許用戶從多個選項中選擇的自定義資料，這些值是用戶可以從中選擇的值。 自定義選項僅在[!UICONTROL下拉清單]、[!UICONTROL多選項下拉清單]、[!UICONTROL單選按鈕]和[!UICONTROL複選框]上有效。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL自定義窗體標籤]</td> 
   <td>使用帶有自定義選項的自定義顯示類型時，這是用戶介面文本，將在該自定義選項的下拉菜單、複選框或單選按鈕中顯示。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL自定義值]</td> 
   <td>使用帶有自定義選項的自定義欄位時，這是將儲存在特定選項的資料庫中的值。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL自定義視圖]</td> 
   <td>為清單中的每個對象顯示的資料欄位或列的定義。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL客戶]</td> 
   <td>使用Workfront實例的組織。</td> 
  </tr> 
 </tbody> 
</table>

## D - F

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>物件名稱</th> 
   <th>說明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL儀表板]</td> 
   <td> <p> 您可以將此欄位添加到報表或報表對象清單中，以顯示清單中列出報表的儀表板。 </p> <p> 您也可以使用此欄位過濾特定儀表板上列出的報告。 </p> <p> 有關在報表對象報表中包括儀表板資訊的詳細資訊，請參閱文章中的「瞭解哪些報表在儀表板上列出」部分 <a href="../../../reports-and-dashboards/reports/report-usage/access-organize-reports.md" class="MCXref xref">訪問和組織報告</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資料類型]</td> 
   <td>請參閱「[!UICONTROL自定義資料類型]」。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL延遲天數]</td> 
   <td> <p>如果缺少[!UICONTROL實際完成日期]，此欄位將顯示[!UICONTROL計劃開始]和[!UICONTROL今天]之間的日期差。</p> <p>還顯示[!UICONTROL實際完成]和[!UICONTROL計畫完成]之間的日期差，當存在[!UICONTROL實際完成日期]時。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL預設計畫]</td> 
   <td> <p>可自定義的預設工作時間，以分配給組織內的用戶和項目。 </p> <p>計畫用於計算分配給用戶的任務的計畫日期、開始日期和完成日期。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL交付項]</td> 
   <td>在項目完成後必須提供的可量化的貨物或服務。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL需求管理]</td> 
   <td>對進氣過程進行評分和排定優先順序。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL部門目標]</td> 
   <td>特定部門所獨有的目標，重點是改善部門內的運營指標。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL依賴項]</td> 
   <td>兩個任務之間的連結需要一個任務更改狀態，然後另一個任務也可以更改狀態。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL依賴項類型]</td> 
   <td> <p>任務與其前置任務之間調度關係的類型。 一個示例是[!UICONTROL完成 — 開始]，它要求第一個任務必須完成，然後第二個任務才能開始。</p> <p>有關詳細資訊，請參見 <a href="../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md" class="MCXref xref">任務依賴關係類型概述</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文檔]</td> 
   <td>附加到內部對象的任何檔案 [!DNL Workfront]。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文檔版本]</td> 
   <td> <p>每次將同一文檔上載到同一對象時，都會為其分配版本號。 用戶可以查看和更改文檔早期版本的多個選項。</p> <p>有關詳細資訊，請參見 <a href="../../../documents/managing-documents/manage-document-versions.md" class="MCXref xref">管理文檔版本</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL持續時間]</td> 
   <td> <p>為完成任務問題或項目分配的時間窗口（由[!UICONTROL計劃開始]和計畫完成之間的天數確定）。</p> 
    <ul> 
     <li>對於任務，如果任務的「工期類型」不是「簡單」，則「工期」是可編輯欄位。 如果任務的持續時間類型為「簡單」，或者如果任務約束為「固定日期」，則持續時間是由Workfront執行的計算。</li> 
     <li>對於問題，「持續時間」始終是可編輯欄位，它應表示需要解決問題的估計天數。</li> 
     <li>對於項目，「工期」是由 [!DNL Workfront] 它表示最早任務的「計劃開始」與項目上最新任務的[!UICONTROL計畫完成]之間的天數差異。</li> 
    </ul> <p>有關任務的[!UICONTROL持續時間]和[!UICONTROL計畫持續時間]之間差異的詳細資訊，請參閱文章 <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md">任務的[!UICONTROL計畫持續時間]和[!UICONTROL持續時間]之間的差異</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL持續時間（分鐘）]</td> 
   <td>此欄位顯示的資訊與[!UICONTROL持續時間]欄位（以分鐘為單位）相同，而不是以天為單位。 </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc,QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL每個事件的持續時間]</td> 
   <td> <p>此操作將顯示在循環任務父項的[!UICONTROL任務詳細資訊]和[!UICONTROL編輯任務]框中。 它顯示每個循環任務的持續時間。 有關建立循環任務的資訊，請參閱 <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">建立循環任務</a>。 </p> <p> <span>在單個循環任務中修改的持續時間不會顯示此欄位中指示的值。</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL持續時間類型]</td> 
   <td> <p>一個任務欄位，指明完成任務所需的工作如何在任務持續時間內分配給任務受分配人。 它表示任務的[!UICONTROL工期]、[!UICONTROL需要的工時]與時間量（或[!UICONTROL分配]）之間的關係，分配的資源應花費在任務上以完成它。 </p> <p>此欄位顯示在任務的[!UICONTROL詳細資訊]頁籤上。 </p> <p>選項為：</p> 
    <ul> 
     <li>[!UICONTROL計算分配]</li> 
     <li>[!UICONTROL計算工作]</li> 
     <li>[!UICONTROL工作驅動]</li> 
     <li>[!UICONTROL簡單]</li> 
    </ul> <p>有關詳細資訊，請參見 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任務[!UICONTROL持續時間]和[!UICONTROL持續時間類型]概覽</a>。</p> 
    —&gt; </td> 
   </tr> 
   <tr> 
   <td>[!UICONTROL持續時間單位]</td> 
   <td>用於測量電源搜索中時間的單位。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作驅動]</td> 
   <td>用戶數與任務完成所花時間之間的關係。 添加更多用戶後，為任務計畫的完成總時間會減少，但任務的持續時間保持不變。 例如，如果一項任務是去掉一桶花生，增加更多人會減少計畫的時間，但人日的持續時間將保持不變。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL已用時間]</td> 
   <td> <p>[!UICONTROL已用時間]是任務的[!UICONTROL持續時間]的時間單位。 它是任務的[!UICONTROL計畫起始日期]和[!UICONTROL計畫完成日期]之間的時間，該任務包括節假日、週末和休假時間。 換句話說，已用時間是日曆天數的過去。 </p> <p>[!DNL Workfront] 支援任務持續時間的以下已用時間單位：</p> 
    <ul> 
     <li> <p>[!UICONTROL已用分鐘]</p> </li> 
     <li> <p>[!UICONTROL已用小時數]</p> </li> 
     <li> <p>[!UICONTROL已用天數]</p> </li> 
     <li> <p>[!UICONTROL已用周]</p> </li> 
     <li> <p>[!UICONTROL已用月]</p> </li> 
    </ul> <p>有關任務持續時間（包括已用時間）的詳細資訊，請參見 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任務[!UICONTROL持續時間]和[!UICONTROL持續時間類型]概覽</a>。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL結束日期]</td> 
   <td> <p> 在[!UICONTROL比率]報表中，這是項目層職務角色的新開單比率結束的日期。 與此日期之前與項目關聯的小時數乘以此開單費率計算項目收入。 </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL項目]</td> 
   <td>指示任務、項目、團隊或組織中的承諾和信念何時減弱的[!UICONTROL工作績效指標](WPI)。 這表明你需要採取行動來恢復這種信念和承諾。 WPI會通過問一些簡單的問題來衡量， "你明白你期望的是什麼嗎？ 您分配的工作對組織有影響嗎？ 你做得好嗎？」</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL企業目標]</td> 
   <td>跨職能目標，這些目標有助於衡量公司目標。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL事件]</td> 
   <td>項目或任務中的任何更改。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL事件處理程式]</td> 
   <td>發生事件時發生的自動任務。 一個常見的示例是自動電子郵件通知。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL事件通知]</td> 
   <td>從事件處理程式生成的電子郵件。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL費用]</td> 
   <td>任務或項目的非人工成本。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL外部]</td> 
   <td> <p>通常是許可證類型或具有此許可證的用戶，它只能查看系統中的資訊。</p> <p>有關詳細資訊，請參見 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] 許可證概述</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL外部系統]</td> 
   <td>儲存和管理在指定記錄系統之外的任何服務或軟體。</td> 
  </tr>

<tr> 
   <td>[!UICONTROL欄位]</td> 
   <td><p>任何Workfront對象或與其關聯的資訊，如資料庫中所示。 </p>
   <p>例如，"project"、"user"、"hour"既是Workfront對象，也是欄位。 "Name"、"status"、"owner"、"start date"是與上述對象關聯的Workfront欄位。 </p>

<p>在引用對象時，項目"objects"和"fields"可互換使用。</p>
   <p>在報告範圍中，「欄位」是指要在報告中捕獲的對象或有關對象的資訊。</p>

<p><b>附註</b></p>

<p>在文本更多報告中，欄位是指對象或其資訊在資料庫中顯示時的資訊。</p>
   <p>有時，您在用戶介面中看到的名稱與資料庫中欄位的名稱不同。 例如，"issue"是Workfront介面中對象的名稱，而"opTask"是Workfront資料庫中對象（或欄位）的名稱。 </p> 
   <p> 在編寫文本模式報告、視圖、篩選器或分組時，或在建立計算欄位時，必須使用該欄位在資料庫中顯示。</p>

<p>有關詳細資訊，請參見 <a href="../../../wf-api/general/api-explorer.md">API資源管理器</a> 和 <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md">文本模式概述</a>。</p>

<p>預設情況下，Workfront附帶一組欄位，可定義對象及其資訊。 您也可以建立自定義欄位來定義對象，但無法建立自定義對象。</p> 
   </td> 
  </tr>

<tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL篩選器]</td> 
   <td> <p>報告或清單元素的主要構建塊之一，用於定義螢幕上顯示的資訊。 有關報告元素的詳細資訊，請參見 <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">報告元素：篩選器、視圖和分組</a>。</p> <p>篩選器確定在報表或報表上顯示的結果 [!DNL Workfront] 面板清單，如項目、任務或問題。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL財務工作管理]</td> 
   <td>管理人工成本、費用和收入資料的流程 [!DNL Workfront]。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL固定成本]</td> 
   <td>您可以為項目定義固定成本金額。 這是項目的[!UICONTROL計畫成本]的一部分，它表示完成項目所需的資金量。 有關成本的資訊，請參閱 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">跟蹤成本</a>。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL固定收入]</td> 
   <td>您可以為項目定義固定收入金額。 這是項目的[!UICONTROL計畫收入]的一部分，它表示在完成項目時可能獲得的金額。 有關收入的資訊，請參閱 <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">開單和收入概覽</a>。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL標誌]</td> 
   <td> <p> 此欄位與[!UICONTROL狀態表徵圖]相同，但它僅可用於以下視圖： </p> 
    <ul> 
     <li> [!UICONTROL模板] </li> 
     <li> [!UICONTROL費用] </li> 
    </ul> <p> 有關詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">視圖中的內置狀態表徵圖</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資料夾]</td> 
   <td>資料夾用於組織與對象關聯的文檔或報告。</td> </tr>
  <tr>
  <td>[!UICONTROL FTE]（全時等效）</td> 
   <td>這是「全時對等」，它指示資源可用於工作的時間量。 
   [!UICONTROL FTE]欄位顯示在以下區域： 
  <ul>
   <li> 編輯或建立用戶時的用戶配置檔案 </li>
   <li> [!UICONTROL資源規劃器] </li>
   <li> [!UICONTROL方案規劃器](需要Workfront方案規劃器的附加許可) </li>
   <li> 用戶清單和報告 </li> </ul>

<p>[!UICONTROL FTE]必須是最多1的十進位數，並且不能是0。 </p>
   <p> 1的[!UICONTROL FTE]（如其配置檔案中所定義，是用戶的[!UICONTROL FTE]欄位的預設值）表示資源（用戶或角色）根據計算其可用性的計畫工作整個小時數。 </p>
   <p>您的Workfront管理員決定在確定用戶可用性時使用哪個計畫。  </p>
   <ul>
   <li> 使用[!UICONTROL預設計畫]時，Workfront使用其配置檔案中找到的用戶的[!UICONTROL FTE]計算可用性。 </li>
   <li> 使用用戶調度時，Workfront會使用用戶的休息時間、[!UICONTROL工作時間]值和[!UICONTROL預設調度]小時數來計算用戶的[!UICONTROL FTE]。 </li> </ul>

<p>有關詳細資訊，請參見 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">配置資源管理首選項</a>。  </p>
   <p>有關在中建立計畫的詳細資訊 [!DNL Workfront]，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">建立計畫</a>。 </p>

<p><b>附註</b></p>
   <p>對於[!UICONTROL方案規劃器]中的所有計算，Workfront使用以下值：1 [!UICONTROL FTE] = 8小時。</p>
   <p>有關詳細資訊，請參見 <a href="../../../scenario-planner/get-started-with-scenario-planning.md">開始使用[!UICONTROL方案規劃器]</a>。 </p>
   </td> </tr> 
   </tbody> 
   </table>

<!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Task field used by the planner to set how the work required is allocated to the assignees across the duration.</p>
<!--
FTE
The designated full time equivalency for users. A full-time user should have 100% FTE and part-time user should have a percentage that equals their working hours. 
-->

## G - I

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>物件名稱</th> 
   <th>說明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL甘特圖]</td> 
   <td> <p>在當前計畫項目任務時，基於計畫日期或預計日期的日曆視圖中項目日期的可視日程表。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL目標]</td> 
   <td><p>在 [!DNL Workfront]: </p> 
    <ul> 
     <li> <p><b>項目目標</b>:項目相關利益相關方同意的一組業務目標。 項目目標是項目業務案例的一部分。 </p> <p>不能在清單或報表中顯示項目目標，但可以通過API訪問它們。 </p> <p>有關業務案例項目目標的資訊，請參閱 <a href="../../../manage-work/projects/define-a-business-case/create-business-case-goals.md">建立業務案例目標 </a>。 </p> </li> 
     <li> <p><b>戰略目標</b>:戰略目標是您建立的目標，用於為特定時間段規劃工作策略。 可以使用 [!DNL Workfront Goals]。 您的組織必須購買額外的許可證，並且您必須擁有此功能的訪問權限才能建立戰略目標。 [!DNL Workfront Goals] 只有附加許可證才可用。</p> 
     <p>有關詳細資訊，請參見 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] 概述 </a>。 </p> 
     <p>您可以在目標或項目報告中顯示戰略目標，並通過API訪問這些目標。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL目標層次]</td> 
   <td> <p>在[!UICONTROL Goal]和[!UICONTROL Project]報告中，這是一個集合欄位，它顯示策略目標與其他目標對齊時所屬層次結構中的目標。 目標由分隔符▸開。 </p> <p>此欄位中只顯示目標和目標的父級。 不顯示子項目標。 </p> <p>有關在中調整目標的資訊 [!DNL Workfront Goals]，請參閱 <a href="../../../workfront-goals/goal-alignment/goal-alignment-overview.md">目標對齊概述 [!DNL Workfront Goals]</a>。 </p> 
   <p>僅當您的組織已購買時，此欄位才可見 [!DNL Workfront Goals]。 有關使用 [!DNL Workfront Goals]，請參閱 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] 概述 </a>。 </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL目標成功分數]</td> 
   <td> 在[!UICONTROL項目報告]中，此欄位用於引用與[!UICONTROL業務]案例關聯的項目級目標。 當前，此欄位已過時，未與任何功能關聯。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL目標] </td> 
   <td> <p>在[!UICONTROL項目]報告中，這是一個集合欄位，顯示與項目關聯的所有戰略目標。 目標用逗號分隔。</p> <p>僅當您的組織已購買時，此欄位才可見 [!DNL Workfront Goals]。 有關使用 [!DNL Workfront Goals]，請參閱 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] 概述</a>。 有關中的戰略目標和項目目標的詳細資訊 [!DNL Workfront]，請參見本文中的「[!UICONTROL目標]」。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL全局介面首選項]</td> 
   <td>影響所有用戶的介面設定。 [!UICONTROL全局介面首選項]可被[!UICONTROL用戶介面首選項]覆蓋。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL組]</td> 
   <td> <p>有權訪問相同對象的用戶（可能來自同一部門或業務部門）的集合。 除用戶外，組還可以與包、程式、項目、<span> 項目模板，</span> 公司、團隊、時間表、佈局模板和時間表配置檔案。</p> <p>也可以按組向對象授予權限。 有關詳細資訊，請參見 <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">組概述</a>。</p> <p>在以下類型之一的對象的清單或報告中，可以使用[!UICONTROL組]欄位列出與特定組關聯的該類型的對象：用戶，項目組，項目， <span>項目模板</span>、公司、團隊、時間表、佈局模板或時間表配置檔案。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL組管理員]</td> 
   <td> <p>管理指定用戶組的對象、訪問權和用戶的用戶。</p> <p> 在[!UICONTROL組]報告中，此欄位顯示組中指定為[!UICONTROL組管理員]的用戶的名稱。 有關組管理員的詳細資訊，請參見 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">組管理員</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！具有管理訪問權限的UICONTROL組]</td> 
   <td> <p> 在[!UICONTROL佈局模板]、[!UICONTROL時間表配置檔案]或[!UICONTROL時間表報告]中，此欄位顯示組管理員有權修改模板的組。 您也可以按此欄位篩選此報告。 </p> <p> 有關詳細資訊，請參見 <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">建立和管理佈局模板</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL分組]</td> 
   <td> <p>一種報告元素，用於按通用標準對清單中的資訊進行分類。</p> <p>有關詳細資訊，請參閱文章中的「[!UICONTROL分組]」部分 <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">報告元素：篩選器、視圖和分組</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL切換日期]</td> 
   <td> <p>任務可用於工作的日期。 [!UICONTROL切換日期]是計算，無法手動設定。 <br>有關[!UICONTROL切換日期]的詳細資訊，請參閱文章 <a href="../../../manage-work/tasks/task-information/handoff-task-date.md" class="MCXref xref">[!UICONTROL任務切換日期]概述</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL幫助台]</td> 
   <td>部分 [!DNL Workfront] 包含所有問題隊列。 [!UICONTROL幫助台]可用於處理客戶支援票證、項目請求、幫助台票證等。 這與[!UICONTROL請求]區域相同。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL所有者]</td> 
   <td>在[!UICONTROL Hour]報告中，[!UICONTROL Owner]是將小時分配給的用戶。 這與實際記錄時間的用戶不同。 這兩個實體有時可以是兩個不同的用戶。 <br>有關其他用戶記錄時間的詳細資訊，請參閱文章 <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">日誌時間</a>。</td> 
  </tr>

<tr> 
   <td>小時狀態</td> 
   <td> <p>由Workfront為用戶記錄任務、問題或項目的實際小時數設定的屬性。 </p>

工時條目在Workfront可具有以下狀態之一：
<ul>
   <li><b>已提交</b>:已記錄項目、任務或問題的小時數。 它們是計費記錄的一部分或尚未添加到計費記錄。</li>
   <li><b>已批准</b>:這些小時數已記錄，並且已經獲得項目所有者的批准。 它們是計費記錄的一部分或尚未添加到計費記錄。</li> 
   <li><b>未批准</b>:這些小時已被項目所有者記錄和拒絕。 它們是計費記錄的一部分或尚未添加到計費記錄。</li>
   <li><b>已計費</b>:已記錄小時，並將其添加到開單記錄，並且開單記錄狀態已標籤為已開單。 它們不需要獲得項目所有者的批准。</li>
   <li><b>已開單和已批准</b>:小時已記錄，並且項目責任人已批准，並且開單記錄狀態已標籤為已開單。</li>
   </ul>


<p>如果小時數是開單記錄的一部分，則「小時狀態」將指明是否已批准小時數，或是否已對其所屬的開單記錄開單。 小時條目的「小時狀態」僅在小時清單或報告中可見。 </p>

<p>有關將小時數添加到開單記錄的詳細資訊，請參閱文章中的「將小時數添加到開單記錄」一節 <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >建立開單記錄</a>。</p>

<p>有關批准項目時間的詳細資訊，請參閱 <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" >需要為項目批准時間</a>。</p>

<p><b>提示</b></p>

<p>未直接登錄工作項的一般小時數不顯示小時狀態。 </p> </td> 
  </tr>



<tr> 
   <td>[!UICONTROL小時類型]</td> 
   <td> <p>可為用戶記錄任務、問題或項目的實際小時數設定的屬性。 這也是未直接連結到工作的已記錄小時數的屬性，如[!UICONTROL Vacation]和[!UICONTROL Time Off]。</p> <p>有關詳細資訊，請參見 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md" class="MCXref xref">管理工時類型</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>ID是與中的每個對象關聯的字母數字指示符 [!DNL Workfront]。 它唯一地標識 [!DNL Workfront] 資料庫。 您可以查看報表中任何對象的ID或每個對象的清單。 </p> <p>提示：   <p>您也可以在對象頁面的URL中查看ID。 例如，訪問[!UICONTROL項目詳細資訊]頁時，項目的ID可能與以下URL中概述的數字類似：</p> <p><code>https://&lt;your domain>.my.workfront.com/project/<b>5e29c8010027d8eb334762d4fff3ffca</b>/overview</code> </p> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL個人目標]</td> 
   <td>個人目標，這些目標有助於團隊目標的指標，但與個人或職業發展無關。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL繼承的訪問]</td> 
   <td>允許訪問從對象傳播到另一個對象的共用函式。 例如，項目用戶在方案和項目組合記錄中定義的繼承訪問權限。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL計畫]</td> 
   <td> <p>在 [!DNL Workfront Scenario Planner]，您可以將計劃分為多個計畫，以便更易於管理計畫。 <span>您可以生成[!UICONTROL Initiative]報告，並且可以訪問[!UICONTROL Project]報告中的[!UICONTROL Initiative]資訊。</span></p> <p>的 [!DNL Scenario Planner] 需要額外的許可證。 有關 [!DNL Workfront Scenario Planner]，請參閱 <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">的 [!DNL Scenario Planner] 概述</a>。 </p> <p>的 [!DNL Initiative] 報表在您的 [!DNL Workfront] 例如，除非您的公司購買了 [!DNL Workfront Scenario Planner] 許可證。 無法通過API訪問[!UICONTROL倡議]。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL計畫作業角色]</span> </td> 
   <td> <p><span>[!UICONTROL方案作業角色]報告類型顯示與計畫方案關聯的作業角色的資訊 [!DNL Workfront Scenario Planner]。</span> </p> <p>的 [!DNL Scenario Planner] 需要額外的許可證。 有關 [!DNL Workfront Scenario Planner]，請參閱 <a href="../../../scenario-planner/scenario-planner-overview.md">的 [!DNL Scenario Planner] 概述</a>。 </p> <p><span>此報告類型在您的 [!DNL Workfront] 例如，除非您的公司購買了 [!DNL Workfront Scenario Planner] 許可證。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL計畫作業角色小時數]</span> </td> 
   <td> <p><span> 在[!UICONTROL方案作業角色]報告中，顯示與方案中的作業角色關聯的小時數。</span> </p> <p>的 [!DNL Scenario Planner] 需要額外的許可證。 有關 [!DNL Workfront Scenario Planner]，請參閱 <a href="../../../scenario-planner/scenario-planner-overview.md">的 [!DNL Scenario Planner] 概述</a>。 </p> <p>此欄位和[!UICONTROL計畫作業角色]報告類型在您的 [!DNL Workfront] 例如，除非您的公司購買了 [!DNL Workfront Scenario Planner] 許可證。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL計畫作業角色計數]</td> 
   <td> <p>在[!UICONTROL方案作業角色]報告中，顯示與方案關聯的特定作業角色的數量。</p> <p>的 [!DNL Scenario Planner] 需要額外的許可證。 有關 [!DNL Workfront Scenario Planner]，請參閱 <a href="../../../scenario-planner/scenario-planner-overview.md">的 [!DNL Scenario Planner] 概述</a>。 </p> <p>此欄位和[!UICONTROL計畫作業角色]報告類型在您的 [!DNL Workfront] 例如，除非您的公司購買了 [!DNL Workfront Scenario Planner] 許可證。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL計畫上次發佈日期]</td> 
   <td> <p>[!UICONTROL方案]、[!UICONTROL方案作業角色]和[!UICONTROL項目]報告中的欄位，顯示計畫方案上次發佈到項目的日期。 您可以發佈方案以建立項目或更新連結到方案的項目。</p> <p>的 [!DNL Scenario Planner] 需要額外的許可證。 有關 [!DNL Workfront Scenario Planner]，請參閱 <a href="../../../scenario-planner/scenario-planner-overview.md">的 [!DNL Scenario Planner] 概述</a>。 </p> <p><span>有關發佈方案的資訊，請參見</span><a href="../../../scenario-planner/publish-scenarios-update-projects.md">發佈方案以在 [!DNL Workfront Scenario Planner]</a>。 此欄位在您的 [!DNL Workfront] 例如，除非您的公司購買了 [!DNL Workfront Scenario Planner] 許可證。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL內聯搜索]</td> 
   <td>在完成表單的過程中執行搜索以查找一個特定欄位的可能條目。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL介面設定]</td> 
   <td>允許定義自定義視圖、篩選器、分組、清單控制項等的應用程式區域。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL是公司目標]</p></td> 
   <td> <p>在 [!DNL goal reports]，這將為每個策略目標顯示「[!UICONTROL True]/ [!UICONTROL False]」值，以指示您的組織是否已分配給目標作為其所有者。 </p> 
   <p>僅當您的組織已購買時，此欄位才可見 [!DNL Workfront Goals]。 有關使用 [!DNL Workfront Goals]，請參閱 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] 概述 </a>。</p>
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL問題]</td> 
   <td> <p>計畫外工作項，通常指示存在妨礙完成任務或項目的問題。 對其進行篩選和評估，以供進一步的工作努力考慮</p> <p>[!UICONTROL問題]也可以是[!UICONTROL幫助台]請求。 [!UICONTROL更改順序]、[!UICONTROL請求]和[!UICONTROL錯誤]也是[!UICONTROL問題]。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL問題管理]</td> 
   <td> <p>用於定義問題類型和與每種類型關聯的路由、篩選或通信流程的流程和規則。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL問題所有者]</td> 
   <td>負責篩選和完成問題的團隊或用戶。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL迭代]</td> 
   <td>團隊生成預定義的交付項集的時間段。</td> 
  </tr> 
 </tbody> 
</table>

## J - L

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>物件名稱</th> 
   <th>說明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL作業角色]</td> 
   <td> <p>用於標識用戶的日常工作職能和職責。 可以將作業角色分配給工作項目，以確定完成工作過程所需的技能，而不將其分配給特定用戶。 </p> <p>用戶可以具有多個角色。 示例包括圖形設計器或顧問。</p> <p>有關詳細資訊，請參見 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">建立和管理作業角色</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL日記帳分錄]</p> </td> 
   <td> <p>一個可報告對象，它告訴您有關項目、任務、問題和其他對象的[!UICONTROL更新]區域中顯示的跟蹤欄位的系統更新的資訊。</p> <p>要瞭解更多資訊，請參閱 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md" class="MCXref xref">[!UICONTROL更新]區域的報告</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL看板標誌]</td> 
   <td> <p>在[!UICONTROL任務]報表或[!UICONTROL問題]報表中，[!UICONTROL看板標誌]欄位顯示在[!UICONTROL看板板]上文章上設定的標誌狀態。 可能的值為[!UICONTROL On Track]、[!UICONTROL Ready to Pull]和[!UICONTROL被阻止]。</p> <p>有關在[!UICONTROL看板文章板]上設定文章標誌狀態的詳細資訊，請參閱文章 <a href="../../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md" class="MCXref xref">在[!UICONTROL看板板]上的文章上使用標誌</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>關鍵績效指標</td> 
   <td>一個可衡量的價值，它展示了公司如何有效地實現關鍵業務目標。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lag]</td> 
   <td>在前置任務的[!UICONTROL計畫完成日期]過後必須經過的時間量，直到從屬任務開始為止。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL滯後類型]</td> 
   <td> <p>計算[!UICONTROL Lag]的方法。 可以是：</p> 
    <ul> 
     <li>[!UICONTROL天數]（工作日）</li> 
     <li>[!UICONTROL日曆天數]（忽略節假日）</li> 
     <li>[!UICONTROL百分比]</li> 
     <li>[!UICONTROL週日]</li> 
    </ul> <p>有關詳細資訊，請參閱中的「[!UICONTROL Lag Types overview]」一節 <a href="../../../manage-work/tasks/use-prdcssrs/lag-types.md" class="MCXref xref">延遲類型概覽</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL大縮略圖]</td> 
   <td> <p> 在[!UICONTROL文檔]清單或報告中，它會在縮略圖中顯示文檔的預覽。 </p> <p>選擇 <strong>[!UICONTROL大縮略圖]</strong> 查看報告中400像素範圍的縮略圖。</p> <p>修改清單或報表中列的寬度時，縮覽圖的大小會調整。</p> <p>另請參見本文中的「[!UICONTROL縮略圖]」。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL最後10個查看器]</td> 
   <td> <p>在報告清單中，此欄位顯示最近查看了報告的最多10個用戶的名稱。<br>有關報表清單中使用資訊的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">查看報表使用情況</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL最後條件注釋]</td> 
   <td> <p>此欄位顯示對象所有者上次在對象上輸入的更新。這是所有者在對象上最近的活動或交互。</p> <p>的 [!DNL Last Condition Note] 如果刪除了對象最後一個注釋的注釋文本，則列為空。 當在對象上輸入新附註時，它將成為最後一個附註，並在列中再次顯示。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL上次財務更新日期]</td> 
   <td>在[!UICONTROL項目]報告中，此欄位將捕獲上次計算和更新項目財務的日期和時間。 有關項目財務的資訊，請參見 <a href="../../../manage-work/projects/project-finances/project-finances-overview-1.md" class="MCXref xref">項目財務概覽</a>。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL最後一個注釋]</td> 
   <td> <p>此欄位顯示任何用戶上次在對象上輸入的更新。 這是對象上最近的活動或交互。</p> <p>如果刪除了對象最後一個注釋的文本，則[!UICONTROL最後一個注釋]列為空。 當在對象上輸入新附註時，它將成為最後一個附註，並在列中再次顯示。</p>
   <p>將此欄位添加到[!UICONTROL任務]報表時，子對象（如問題、子任務、文檔等）上剩餘的任何更新。  — 此列中不顯示任務。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL上次查看者]</td> 
   <td> <p>在報告清單中，此欄位顯示有關上次查看報告的用戶的資訊。<br>有關報表清單中使用資訊的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">查看報表使用情況</a>。<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL上次查看日期]</td> 
   <td> <p>在報表清單中，此欄位顯示上次顯示報表的日期。<br>有關報表清單中使用資訊的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">查看報表使用情況</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL佈局模板]</td> 
   <td>由系統管理員或組管理員定義，用於標識在給定用戶工作區中顯示的頁籤和報告。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL佈局類型]</td> 
   <td>與[!UICONTROL自定義視圖]結合使用，[!UICONTROL佈局類型]指定[!UICONTROL自定義視圖]的類型。 當前，只有清單可用。 將來，[!UICONTROL詳細資訊]（對象的[!UICONTROL詳細資訊]視圖）可能會變為可用。</td> 
  </tr> 
  <!--<tr data-mc-conditions=""> 
   <td>Legacy Budgeted Cost</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p> <p>The field is still visible in some reports and lists, but the information displayed cannot be updated. </p> <p>See <i>Budgeted Cost</i>. </p> </td> 
  </tr>
  --> 
  <!--<tr data-mc-conditions=""> 
   <td>Legacy Budgeted Hours</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p> <p>The field is still visible in some reports and lists, but the information displayed cannot be updated. </p> <p>See <i>Budgeted Hours</i>. </p> <p>
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        This field shows the number of hours budgeted for the project in the Legacy Resource Estimates area of the Business Case or in the Capacity Planner. 
       <br>If there&nbsp;are multiple job roles, this is a summary of the budgeted hours for all job roles. The Legacy Budgeted Hours are calculated after you have used the "Set budget to schedule" feature, or after you have defined how many of the Planned Hours should be budgeted, in the Resource Estimates area of the Business Case of the project or in the Capacity Planner.&nbsp; 
     </p> </td> </tr> -->
  <!--<tr data-mc-conditions=""> 
   <td>Legacy Budgeted Labor Cost</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed. This field cannot be updated. </p> <p>The field is still visible in some reports and lists. </p> <p>See <i>Budgeted Labor Cost</i>. </p> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In a project report, this field shows the labor cost associated with the project, taking into account the Cost per Hour rate of every job role and the amount of Legacy Budgeted Hours estimated in the Legacy Resource Estimates area of the Business Case that is needed for each role to complete the project.&nbsp;</p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Legacy Budgeted Labor Cost in a project report is calculated using the following formula:</p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code style="font-style: normal;">Legacy Budgeted Labor Cost = SUM(Job Role Cost per Hour * Legacy Budgeted Hours per Job Role)</code> </p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about calculating Legacy Budgeted Labor Cost, see the article <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a>&nbsp;&nbsp;</p>
    --> </td> 
  </tr> 
  <tr> 
   <!-- <td>Legacy Resource Pool</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed. This field cannot be updated. </p> 
   <p>Although not recommended, you may update the information in this report using the API.</p> 
   <p>See <i>Resource Pools</i> for updated fields. </p> 
   <p>The Legacy Resource Pool is a collection&nbsp;of job roles associated with a project or a user. The functionality of the Legacy Resource Pools is displayed in the tools available in the Legacy Resource Planning tab of the People area. This is a deprecated field.</p>
    --> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL庫任務]</td> 
   <td>單個任務的模板，用於跨應用程式提供[!UICONTROL Tasks]和[!UICONTROL Template Tasks]的一致命名。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL許可證類型]</td> 
   <td>分配給[!UICONTROL訪問級別]的許可證類型。 它為[!UICONTROL完整用戶]、[!UICONTROL有限用戶]或[!UICONTROL請求者]。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL許可證限制計畫]</td> 
   <td> <p>在[!UICONTROL組]視圖或報表中，此欄位顯示可分配給將相應組指定為其[!UICONTROL主組]的用戶的最大[!UICONTROL計畫]許可證數。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL許可證限制工作]</td> 
   <td> <p>在[!UICONTROL組]視圖或報表中，此欄位顯示可分配給將相應組指定為其[!UICONTROL主組]的用戶的最大[!UICONTROL工作]許可證數。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL受限用戶]</td> 
   <td>允許建立 [!DNL Access Level] 包含僅查看權限，可提交問題、輸入附註和上載文檔。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL清單控制項]</td> 
   <td> <p>[!UICONTROL介面設定]的一部分，它允許將自定義篩選器、視圖和分組連結到單個用戶或全局連結到所有用戶。</p> </td> 
  </tr> 
 </tbody> 
</table>

## M - O

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>物件名稱</th> 
   <th>說明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[！僅UICONTROL手動]</td> 
   <td> <p>[!UICONTROL項目]的[!UICONTROL更新類型]之一。 此設定允許僅在按一下「[!UICONTROL重新計算的時間軸]」時更新[!UICONTROL項目投影]和[!UICONTROL計畫的]時間軸。 在輕量重新計算流程中以及更新項目中的項目或任務時，將忽略以這種方式設定的項目。</p> <p>有關詳細資訊，請參見 <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">選擇項目[!UICONTROL更新類型] </a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Me]</td> 
   <td> <p>這是指當前登錄的用戶。 </p> <p>建議在與其他用戶共用報告時在篩選器中使用此欄位使報告更一般。 這樣，您只能生成一個報告，該報告將根據登錄者來查看該報告的不同資訊，因為該資訊始終是為登錄用戶自定義的。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL最大用戶數]</td> 
   <td> <p>這是一個已棄用的欄位。 此欄位可能顯示的任何資訊都與某個功能相關 [!DNL Workfront] 已刪除，無法更新該欄位。 </p> <p>在以前版本中 [!DNL Workfront]，可以在建立或編輯作業角色時更新此欄位。 它顯示了可以與每個項目上的角色關聯的用戶總數。 對於可以在項目上分配的無限數量用戶，允許值為零。 </p>該欄位在某些報告和清單中仍然可見，但顯示的資訊無法更新。 </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL里程碑]</td> 
   <td> <p>可以與任務關聯的標籤，用於指示任務完成後項目中的關鍵點已實現。 通常，您可以使用里程碑來顯示重要事件，例如項目的某一階段或一組關鍵活動的完成。 [!UICONTROL Milestones]通常與父任務關聯。 必須先建立里程碑，然後才能將它們附加到任務。 有關裡程碑的資訊，請參見 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md">建立里程碑路徑</a> 和 <a href="../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md">將里程碑與任務關聯</a>。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL里程碑路徑]</td> 
   <td>[!UICONTROL里程碑]的集合。 [!UICONTROL里程碑路徑]用於項目，以區分具有某些類型的[!UICONTROL里程碑]的項目和具有不同組的[!UICONTROL里程碑]的項目。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL里程碑任務]</td> 
   <td>標籤為指示要衡量的可報告事件的任務。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL模組]</td> 
   <td>中方案中的單個步驟 [!DNL Workfront Fusion] 基於關聯的應用執行某些功能。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL我的主角色]</td> 
   <td> <p>在篩選器中引用此項時，將顯示與登錄用戶具有相同[!UICONTROL主角色]的用戶，或分配給登錄用戶的[!UICONTROL主角色]的工作項。</p> <p>建議在與其他用戶共用報告時在篩選器中使用此欄位使報告更一般。 這樣，您只能生成一個報告，該報告將根據登錄者來查看該報告的不同資訊，因為該資訊始終是為登錄用戶自定義的。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL我的主團隊]</td> 
   <td> <p>在篩選器中引用此項時，此欄位顯示屬於已登錄用戶的[!UICONTROL主團隊]的用戶，或分配給已登錄用戶的[!UICONTROL主團隊]的工作項。 </p> <p>建議在與其他用戶共用報告時在篩選器中使用此欄位使報告更一般。 這樣，您只能生成一個報告，該報告將根據登錄者來查看該報告的不同資訊，因為該資訊始終是為登錄用戶自定義的。 </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL命名約定]</td> 
   <td>組織範圍的一組規則，使用資料建立項目、任務和交付項的名稱。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL本機整合]</td> 
   <td>不需要手動編碼或API配置的整合。 也稱為「現成」整合。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL導航菜單]</td> 
   <td>具有到[!UICONTROLWorkfront]主區域連結的應用程式的頂中心面板。</td> 
  </tr> 
 </tr> 
  <tr> 
   <td>[!UICONTROL新數字值]</td> 
   <td>在[!UICONTROL日記帳條目]報告中，將顯示替換[!UICONTROL舊數值]的欄位的更新值。
   有關詳細資訊，請參閱本文中的「[!UICONTROL舊數值]」。</td> 
  </tr>
  <tr> 
   <td>[!UICONTROL非工作日]</td> 
   <td>未分配給完成任何分配的日。 這通常是假日、假日或週末。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL注釋]</td> 
   <td>對 [!DNL Workfront] 的雙曲餘切值。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL注釋文本]</td> 
   <td> <p>這顯示用戶在任何對象上輸入的更新文本。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL連結目標數]</td> 
   <td> <p>在[!UICONTROL項目]報告中，這是與項目關聯的戰略目標數。 有關將項目與戰略目標關聯的資訊，請參閱 <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">將項目添加到  [!DNL Adobe Workfront Goals]</a>。</p> 
   <p>有關戰略目標的資訊，另請參見本文中的「[!UICONTROL目標]」。</p> 
   <p>僅當您的組織已購買時，此欄位才可見 [!DNL Workfront Goals]。 有關使用 [!DNL Workfront Goals]，請參閱 <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">將項目添加到[!UICONTROLAdobe Workfront目標]中的目標</a>。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL對象]</td> 
   <td> <p>您在中顯示的資訊 [!DNL Adobe Workfront] 由儲存在 [!DNL Workfront] 資料庫。 這些物體是Workfront資訊的驅動因素。 對象的一些示例包括：</p> 
    <ul> 
     <li>[!UICONTROLPortfolio]</li> 
     <li>[!UICONTROL程式]</li> 
     <li>[!UICONTROL項目]</li> 
     <li>[!UICONTROL任務]</li> 
     <li>[!UICONTROL問題]</li> 
     <li>[!UICONTROL文檔]</li> 
     <li>[!UICONTROL儀表板]</li> 
     <li>[!UICONTROL報告]</li> 
     <li>[!UICONTROL組]</li> 
     <li>[!UICONTROL團隊]</li> 
     <li>[!UICONTROL用戶]</li> 
     <li>[!UICONTROL公司]</li> 
     <li>[!UICONTROL自定義表單]</li>
     <li>[!UICONTROL自定義欄位]</li>  
     <li>[!UICONTROL小時]</li> 
     <li>[!UICONTROL開單費率]</li> 
     <li>[!UICONTROL模板]</li> 
     <li>[!UICONTROL模板任務]</li>

<p><b>附註</b></p>
  <p>這不是一份詳盡的清單。 </p>

</ul> <p>有關詳細資訊，請參見 <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">瞭解[!UICONTROLAdobe Workfront]中的對象</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL對象類型]</td> 
   <td>如果建立包含所有自定義表單的報表或清單，則可以將此欄位用作視圖或篩選器，以查看哪些對象類型與每個表單相關聯。 </td> 
  </tr> 
 <tr> 
   <td>[!UICONTROL舊數值]</td> 
   <td>在[!UICONTROL日記帳分錄]報表中，這將顯示更新前欄位的原始值。 更新欄位的值後，它將顯示為[!UICONTROL日記帳條目]報表中的[!UICONTROL新編號值]。 有關詳細資訊，另請參見「[!UICONTROL新數字值]」。</td> 
  </tr>
  <tr> 
   <td>[！僅更改時的UICONTROL]</td> 
   <td> <p>[!UICONTROL項目更新]類型之一。 選中此選項時，[!UICONTROL項目投影]和[!UICONTROL計畫]時間線僅在對項目或項目內的任務進行更新或更改時更新。 它不會每晚更新項目。</p> <p>有關詳細資訊，請參見 <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">選擇項目更新類型 </a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL操作任務]</td> 
   <td> <p>中[!UICONTROL問題]的名稱 [!DNL Workfront] 資料庫，用於文本模式報表或計算的自定義資料。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL開啟]</td> 
   <td>未完成但正在處理的問題或任務。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL組織圖]</td> 
   <td>組織圖的縮寫。 這是一個圖表，顯示組織的層次結構。 它也位於[!UICONTROL User]詳細資訊螢幕的「頁籤」上，顯示並允許設定[!UICONTROL User]的[!UICONTROL Company]和[!UICONTROL Reporting]關係。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL組織設定]</td> 
   <td>這為您的組織定義[!UICONTROL公司]、[!UICONTROL組]和[!UICONTROL安全配置檔案]。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL其他組]</td> 
   <td> <p>在列出用戶的報表或視圖中，此欄位顯示每個用戶是成員的所有組。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL覆蓋貨幣]</span> </td> 
   <td> 
    <div> 
     <p>在[!UICONTROL作業角色]報告中，這是與作業角色關聯的貨幣。 它是[!UICONTROL基本貨幣]的重寫，如在[!UICONTROL設定]區域中所建立，由 [!DNL Workfront] 管理員。 </p> 
     <p>有關詳細資訊，請參見 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">建立和管理作業角色</a>。</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL覆蓋幣種開單/小時]</span> </td> 
   <td> 
    <div> 
     <p>在[!UICONTROL作業角色]報告中，這是使用作業角色的選定[!UICONTROL覆蓋幣種]的作業角色每小時計費率。</p> 
     <p> 有關詳細資訊，請參見 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">建立和管理作業角色</a>。</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL覆蓋貨幣成本/小時]</span> </td> 
   <td> 
    <div> 
     <p>在[!UICONTROL作業角色]報告中，這是使用作業角色的選定[!UICONTROL覆蓋幣種]的作業角色每小時的成本率。 </p> 
     <p>有關詳細資訊，請參見 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">建立和管理作業角色</a>。</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL所有者]</td> 
   <td>負責完成指定對象的用戶。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL所有者類型]</span> </td> 
   <td> 
    <div> 
     <p>在[!UICONTROL目標]報告中，將顯示分配給策略目標的所有者類型。 以下是目標所有者類型：</p> 
     <ul> 
      <li> <p>[!UICONTROL用戶]</p> </li> 
      <li> <p>[!UICONTROL團隊] </p> </li> 
      <li> <p>[!UICONTROL組]</p> </li> 
     </ul> 
     <p>當目標所有者是您的組織時，此欄位中不顯示任何值。 </p> 
     <p>這需要額外的許可證。 有關 [!DNL Workfront Goals]，請參閱 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">[!DNL Adobe Workfront Goals] 概述</a>。 </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## P - R

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>物件名稱</th> 
   <th>說明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL參數]</td> 
   <td> <p>[!UICONTROL參數]是自定義欄位。 您可以為系統中的所有參數或自定義欄位生成報告。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL父級]</td> 
   <td>在報告中，此欄位顯示有關對象父級的資訊。 例如，在[!UICONTROL問題]報告中，它可能顯示有關該問題所記錄的任務或項目的資訊；在任務報告中，它可能顯示有關直接父任務或項目的資訊。 有關哪些對象可能包含父項的詳細資訊 [!DNL Workfront]，請參閱文章中的「對象的相互依賴和層次」部分 <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">瞭解中的對象 [!DNL Adobe Workfront]</a>。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL父級延遲]</td> 
   <td>[!UICONTROL父任務]啟動和[!UICONTROL子任務]啟動之間必須傳遞的時間量。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL父任務]</td> 
   <td>也稱為[!UICONTROL摘要任務]。 這是一個具有子任務（也稱為[!UICONTROL子任務]）的任務。 父任務的[!UICONTROL持續時間]、[!UICONTROL需要工作]和[!UICONTROL完成百分比]是從子任務計算的。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL兼職資源]</td> 
   <td>容量小於系統中定義的預設計畫的許可用戶。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL完成百分比]</td> 
   <td> <p>顯示與任務、項目或問題關聯的工作百分比的項目、任務或問題欄位已完成。</p> <p>您可以手動更新此欄位以處理問題和工作任務。 </p> <p>對於項目和父任務，此欄位是所有工作任務的匯總，您不能手動更新它。 </p> <p>有關詳細資訊，請參見 <a href="../../../manage-work/tasks/task-information/project-percent-complete.md" class="MCXref xref">項目[!UICONTROL完成百分比]概述</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL權限]</td> 
   <td> <p>授予對象上用戶的權限，通常指定為這樣用戶就可以完成項目或查看項目。 您可以授予以下權限：</p> 
    <ul> 
     <li>[!UICONTROL項目]</li> 
     <li>[!UICONTROL任務]</li> 
     <li>[!UICONTROL問題]</li> 
     <li>[!UICONTROLPortfolio]</li> 
     <li>[!UICONTROL程式]</li> 
     <li>[!UICONTROL報告]</li> 
     <li>[!UICONTROL儀表板]</li> 
     <li>[!UICONTROL文檔]</li> 
     <li>[!UICONTROL自定義Forms]</li> 
     <li>[!UICONTROL視圖]</li> 
     <li>[!UICONTROL篩選器]</li> 
     <li>[!UICONTROL分組]</li> 
    </ul> <p>有關詳細資訊，請參見 <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">對象共用權限概述</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL計畫]</td> 
   <td> <p>這是中的完整許可證類型 [!DNL Workfront] 系統。 用戶必須具有此功能才能訪問 [!DNL Workfront]。</p> <p>有關詳細資訊，請參見 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] 許可證概述</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL計畫](在 [!DNL Scenario Planner])</td> 
   <td> <p>計畫是使用 [!DNL Workfront] 方案規劃器。 您可以概述貴公司近期和長期未來的戰略，並確定每個高級別結果，並將其作為計畫添加到 [!DNL Workfront] 方案規劃器。 </p> <p>無法顯示 [!DNL Scenario Planner] 報表中的計畫，您無法通過 [!DNL Workfront] API。 </p> <p>的 [!DNL Scenario Planner] 需要額外的許可證。 有關 [!DNL Workfront Scenario Planner]，請參閱 <a href="../../../scenario-planner/scenario-planner-overview.md">的 [!DNL Scenario Planner] 概述</a>。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL已計畫]</td> 
   <td> <p>計畫發生事件的時間範圍。 建立項目、任務或問題時 [!DNL Workfront]，您可以建立計畫起始日期和終止日期，以及發生這些日期的計畫時間範圍。 這些值表示您對項目完成所需時間的原始意圖或估計。 </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL計畫的益處]</td> 
   <td>這是項目經理的人工錄入，用於評估完成項目是否會給組織帶來任何金錢利益。 指定此值可以是為項目集合[!UICONTROL業務案例]的一部分。 必須對項目具有[!UICONTROL管理]權限才能更新此值。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL計畫預算小時數]</td> 
   <td> <p>在[!UICONTROL預算小時數]報表中，它顯示為[!UICONTROL資源規劃器]中的項目或[!UICONTROL作業角色]編入預算的小時數。 </p> <p>有關[!UICONTROL資源規劃器]中項目或角色預算的資訊，請參閱文章 <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">使用[!UICONTROL項目]和[!UICONTROL角色]視圖在[!UICONTROL資源規劃器]中預算資源</a>。 有關[!UICONTROL預算小時數]報告的資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">報告：預算工時</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL計畫完成日期]</td> 
   <td> <p>您可以手動將[!UICONTROL計畫完成日期]設定為您選擇的日期。 如果未設定[!UICONTROL計畫完成日期], [!DNL Workfront] 自動設定。 自動設定時，[!UICONTROL計畫完成日期]為：[!UICONTROL計劃開始日期] + [!UICONTROL持續時間]</p> <p>有關詳細資訊，請參閱以下文章：</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">任務[!UICONTROL計畫完成日期]概覽</a> </p> </li> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">設定項目[!UICONTROL計畫完成日期]</a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL計畫成本]</td> 
   <td> <p>項目的[!UICONTROL計畫人工成本]和[!UICONTROL計畫支出成本]的合計。 這不包括項目中的[!UICONTROL計畫風險成本]。  </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL計畫持續時間]</td> 
   <td> <p>任務的[!UICONTROL計畫持續時間]通常與任務的[!UICONTROL持續時間]相同。 它表示任務的[!UICONTROL計劃開始]和[!UICONTROL計畫完成日期]之間的天數差異。 </p> <p>當任務的[!UICONTROL持續時間]類型為[!UICONTROL工作驅動]時，[!UICONTROL計畫持續時間]可能與任務的[!UICONTROL持續時間]不同，具體取決於您為任務分配的資源數。 </p> <p>例如，如果[!UICONTROL Duration]類型為[!UICONTROL工作驅動]的任務的[!UICONTROL持續時間]為3天，並且您為任務分配了一個具有全職計畫的資源，則[!UICONTROL計畫持續時間]也為3天。 如果為同一任務分配了三個具有全職計畫的資源，則[!UICONTROL工期]將保持3天，但[!UICONTROL計畫工期]將變為1天。 [!UICONTROL計畫持續時間]還更改任務的[!UICONTROL計劃開始]和[!UICONTROL計畫完成]日期，以反映新的[!UICONTROL計畫持續時間]。 因此，項目的時間表也受到影響。 </p> <p>有關任務的[!UICONTROL持續時間]和[!UICONTROL計畫持續時間]之間差異的詳細資訊，請參閱文章 <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md" class="MCXref xref">任務的[!UICONTROL計畫持續時間]和[!UICONTROL持續時間]之間的差異</a>。</p> <p>項目和問題沒有[!UICONTROL計畫工期]。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL計畫持續時間分鐘]</td> 
   <td> <p>項目或問題的[!UICONTROL計畫持續時間分鐘數]是項目或問題的[!UICONTROL持續時間]（以分鐘為單位）。 </p> <p>任務沒有[!UICONTROL計畫持續時間分鐘]欄位。 </p> <p>[!UICONTROL模板任務]有一個[!UICONTROL計畫持續時間分鐘]欄位，該欄位以分鐘為單位顯示任務的[!UICONTROL計畫持續時間]。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL計畫費用成本]</td> 
   <td> <p>為項目或任務記錄的所有支出的[!UICONTROL計畫金額]總和。</p> <p><b>示例</b></p>
   <p>如果為任務1建立費用，並在[!UICONTROL計畫金額]欄位中輸入$600.00，則此任務的[!UICONTROL計畫費用成本]為$600.00。 </p> 
   <p>對於一個項目， [!DNL Workfront] 使用以下公式計算[!UICONTROL計畫費用成本]:</p> <p><code>Project [!UICONTROL Planned Expense Cost] = SUM (All Project [!UICONTROL Planned Expense Costs]) + SUM (All Tasks [!UICONTROL Planned Expense Costs])</code> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (Drafting this because not sure if this is correct anymore)</p>
    --> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL計畫小時數]</td> 
   <td> <p>此欄位顯示在[!UICONTROL項目]、[!UICONTROL任務]中，以及[!UICONTROL資源規劃器]、[!UICONTROL工作負載平衡器]和[!UICONTROL利用率]報表等項目、任務或問題以及資源管理工具的發佈區域、報告。 </p> <p>它顯示項目所有者估計每個任務或問題完成所需的小時數。 對於項目，通常是項目任務中[!UICONTROL計畫小時數]的匯總。 </p> <p>[!UICONTROL計畫小時數]欄位可能顯示不同的資訊，具體取決於您從何處查看它。 有關計畫工時的資訊，請參閱 <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">計畫工時概覽</a>。</p> <p>計畫小時數以分鐘為單位儲存在 [!DNL Workfront] 資料庫。 使用此欄位寫入計算時，請確保考慮小時數以分鐘為單位顯示的事實。<br></p> <p>預設情況下，計畫小時數將平均分配給工作項目持續時間內的所有天數，並且對分配給任務的所有資源也平均分配。 用戶可以更新工作項的每日計畫小時數金額或每個受分配人的單個計畫小時數。</p> <p>對於項目、任務和問題，更新此欄位時有所不同： </p> 
    <ul> 
     <li> <p>對於問題，您可以手動更新此欄位。 未將發放計畫小時數添加到項目計畫小時數。 </p> <p>提示：在問題報告中，[!UICONTROL計畫小時數]欄位之一將替換為[!UICONTROL工作]欄位。 此欄位顯示該問題的計畫小時數。 有關詳細資訊，請參閱此表中的「work」或「[!UICONTROL Work]」欄位。 </p> </li> 
    </ul> 
    <ul> 
     <li> <p>對於任務，當任務的[!UICONTROL持續時間類型]為[!UICONTROL計算分配]或[!UICONTROL簡單]時，可以手動更新此欄位。 此欄位由 [!DNL Workfront] 當任務的[!UICONTROL持續時間類型]為[!UICONTROL計算工作]或[!UICONTROL工作驅動]時。<br>有關[!UICONTROL任務持續時間]的資訊，請參見文章 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任務[!UICONTROL持續時間]和[!UICONTROL持續時間類型]概覽</a>。</p> </li> 
    </ul> 
    <ul> 
     <li> <p>對於項目， [!DNL Workfront] 通過添加項目上所有任務的所有計畫小時數計算計畫小時數。 </p> </li> 
    </ul> <p><b>提示</b></p> <p>也可以使用文本模式和引用其他欄位，在[!UICONTROL項目]、[!UICONTROL任務]或[!UICONTROL問題]報告中顯示[!UICONTROL計畫小時數]。 有關詳細資訊，請參閱「<code>work</code>", "[!UICONTROL工作]"和"<code>workRequiredExpression</code>」欄位。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL計畫人工成本]</td> 
   <td> 
    <p>對於任務，用戶或角色的小時費率乘以分配給用戶或角色的小時數。</p> <p>對於項目，它是所有任務的所有[!UICONTROL計畫人工成本]的總和。</p> <p>是否使用用戶或角色的比率取決於為給定任務選擇的成本類型。 </p> <p>有關詳細資訊，請參見 <a href="../../../manage-work/projects/project-finances/track-costs.md">跟蹤成本</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL計畫收入]</td> 
   <td> <p>任務和項目可以在中顯示[!UICONTROL計畫收入]的值 [!DNL Workfront]。 [!UICONTROL計畫收入]表示與項目上任務的[!UICONTROL計畫小時數]關聯的金額。 對於項目，它還可以包括項目的[!UICONTROL固定收入]。 </p> <p>對於任務，這是與任務的[!UICONTROL計畫小時數]關聯的收入。 所有任務中的計畫小時數累計到項目的計畫小時數，以幫助計算項目[!UICONTROL計畫小時數]。 </p> 
   <p>[!DNL Workfront] 使用以下公式計算任務和項目的[!UICONTROL計畫收入]:</p> 
   <p><code>Task [!UICONTROL Planned Revenue] = [!UICONTROL Planned Hours] * Billing hourly rate</code> </p> <p><code>Project [!UICONTROL Planned Revenue] = SUM (All tasks [!UICONTROL Planned Revenue]) + [!UICONTROL Fixed Revenue]</code> </p> 
   <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the note below is duplicated in this article: /Content/Resource Mgmt/Resource utilization/view-utilization-information.htm and in the glossary)</p>
    --> 
    <p>在[!UICONTROL項目詳細資訊]區域和項目報告中顯示的項目[!UICONTROL計畫收入]與在[!UICONTROL利用率]報告中顯示的計畫收入不同。 </p> <p>[!UICONTROL項目詳細資訊]區域中的[!UICONTROL計畫收入]反映任務收入以及項目的固定收入。 [!UICONTROL利用率報表]中的[!UICONTROL計畫收入]顯示僅與項目中的任務關聯的[!UICONTROL計畫收入]。 </p> 
     <p><b>示例</b></p>  
      <p>如果項目有1個任務，10小時，分配給顧問，每小時費率為$20，而項目有$100 [!UICONTROL固定收入]，則[!UICONTROL利用率]報表將顯示$200的[!UICONTROL計畫收入]（與小時數關聯的[!UICONTROL計畫收入]）任務)。 [!UICONTROL項目詳細資訊]部分顯示$300（任務中的[!UICONTROL計畫收入]和項目的固定收入）。 </p> 
    <p>有關跟蹤收入的資訊 [!DNL Workfront] 見 <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md">開單和收入概覽</a>。 </p> 
    <p>有關[!UICONTROL利用率報告]中[!UICONTROL計畫收入]計算的資訊，請參見 <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">查看資源利用率資訊 </a>。 </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL計畫風險成本]</td> 
   <td> <p>項目上所有風險的[!UICONTROL潛在成本]的總和，考慮其發生概率。 此金額未包括在項目的[!UICONTROL計畫成本]中。</p> <p>項目的[!UICONTROL計畫風險成本]按以下公式計算：</p> <p><code>Planned Risk Cost = SUM(Potential Risk Cost * Probability / 100)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL門戶配置檔案]</td> 
   <td>管理員定義的頁籤和門戶節集合，顯示在 [!DNL Workfront] 應用程式[!UICONTROL主目錄]和其他儀表板。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL門戶節]</td> 
   <td>儀表板或門戶頁面上頁籤的一個元件。 通常是單個報表、圖表、日曆或關鍵資訊清單。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL門戶頁籤]</td> 
   <td>門戶或儀表板上最多包含三個門戶節的頁籤。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROLPortfolio]</td> 
   <td> <p>具有統一特徵的項目集合。 這些項目通常爭奪相同的資源、預算或時段。 在將Portfolio添加到Portfolio之前，可以將項目分為「項目群」，並將項目與「項目群」關聯。</p> <p>有關包的詳細資訊，請參見 <a href="../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md">Portfolio概述 [!DNL Adobe Workfront]</a>。</p> 
   </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROLPortfolio管理]</td> 
   <td>一個實踐領域側重於管理收集或相關方案和項目工作。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROLPortfolio優化程式]</td> 
   <td>A [!DNL Workfront] 幫助評估和排定項目組合中項目的優先順序的工具。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROLPortfolio所有者]</td> 
   <td>負責確定投資組合的優先次序和預算的利益攸關方。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL潛在風險成本]</td> 
   <td>這是一個可以在清單和報告中找到的項目欄位。 它顯示與項目相關的風險的潛在成本（如果發生）。 有關詳細資訊，請參閱 <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">計算潛在風險成本 </a>。 </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL前置任務]</td> 
   <td> <p>在完成從屬任務之前必須完成的任務。 另外一個標籤為[!UICONTROL依賴項]的任務。 前置任務允許規劃器設定序列相關性邏輯，例如在其他任務完成後啟動任務。</p> <p>有關詳細資訊，請參見 <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">任務前置任務概覽</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL主公司]</td> 
   <td>用戶所屬的公司，在用戶設定中指定。 公司也可以與項目關聯。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL主聯繫人]</td> 
   <td><p>[!UICONTROL主要聯繫人]是問題的建立者，它由 [!DNL Workfront] 當有人製造問題時。 如果具有 [!DNL Manage] 權限。 問題只能有一個主要聯繫人。</p> 
   <p>如果更改主要聯繫人，最初指定為主要聯繫人的用戶仍具有[!UICONTROL管理]權限。</p>
   <p>將問題轉換為任務或項目時，指定為項目的[!UICONTROL主聯繫人]的用戶將成為項目或任務的[!UICONTROL已轉換的問題發起方]。 如果問題的[!UICONTROL主聯繫人]在問題轉換後更新，則在轉換發生時，[!UICONTROL已轉換的問題發起人]將保留為問題的[!UICONTROL主聯繫人]。 另請參見本文中的「[!UICONTROL已轉換問題發起方]」。</p> 
   </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL優先順序]</td> 
   <td>可分配給任務、問題或項目以指定其重要性的值。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL專用]</td> 
   <td>在[!UICONTROL Note]或[!UICONTROL Document]上，此選項使該對象對大多數查看者處於隱藏狀態。 對於專用幫助台隊列，只有隊列團隊中的用戶才能通過[!UICONTROL幫助台]區域將問題提交到該隊列。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL配置檔案]</td> 
   <td>有關用戶帳戶的所有資訊。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL程式]</td> 
   <td> <p>組合中的子集，其中類似項目可以組合在一起以實現明確定義的好處。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL程式管理]</td> 
   <td>管理跨項目依賴性、風險、問題、要求和解決方案，以保持計畫的健康並實現既定的計畫利益。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL程式所有者]</td> 
   <td>負責監督和組織活動的利益相關方確保項目目標與公司目標保持一致。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL進度]</span> </td> 
   <td> <p>在[!UICONTROL目標]報告中，它顯示完成戰略目標的百分比。 進度百分比顯示為數字。 有關戰略目標的資訊，另請參見此表中的「[!UICONTROL目標]」。</p> <p>僅當您的組織已購買時，此欄位才可見 [!DNL Workfront] 目標。 有關使用 [!DNL Workfront Goals]，請參閱 <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md"> 將項目添加到 [!DNL Adobe Workfront Goals] </a>。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL進度狀態]</td> 
   <td> <p>在「項目」、「任務」和「目標」報告中，此欄位顯示項目、任務或戰略目標的「進度狀態」。 有關詳細資訊，請參閱以下文章：</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-progress-status.md" class="MCXref xref">項目進度狀態概述</a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">任務進度狀態概述</a> </p> </li> 
     <li> <p><a href="../../../workfront-goals/goal-management/calculate-goal-progress.md">目標進度和條件概述 [!DNL Adobe Workfront Goals]</a> </p>
     <p>[!UICONTROL目標]報告和[!UICONTROL進度狀態] [!DNL goals] 欄位僅在您的組織已購買時可見 [!DNL Workfront Goals]。 有關中的戰略目標的資訊 [!DNL Workfront Goals]，請參閱 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] 概述</a>。 </p> </li>
    </ul> </td> 
  </tr> 
  <td>[!UICONTROL項目]</td> 
   <td> <p>必須在特定時間範圍內完成並必須使用特定預算和資源數量的大量工作。 要使其易於管理，您可以將項目分為一系列任務。 完成所有任務將導致項目完成。 有關計畫項目的資訊，請參閱 <a href="../../../manage-work/projects/planning-a-project/plan-project.md">計畫項目概述</a>。</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL項目分配計畫小時數]</td> 
   <td> <p>在[!UICONTROL計畫作業角色]報告中，將顯示與分配給項目中任務或問題的作業角色關聯的[!UICONTROL計畫小時數]。 此欄位和[!UICONTROL計畫作業角色]報告類型未顯示在 [!DNL Workfront] 例如，除非您的公司購買了 [!DNL Workfront Scenario Planner] 許可證。 有關 [!DNL Workfront Scenario Planner]，請參閱 <a href="../../../scenario-planner/scenario-planner-overview.md">的 [!DNL Workfront Scenario Planner] 概述</a>。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL項目詳細資訊]</td> 
   <td>項目當前狀態的詳細資訊。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL項目預算成本]</td> 
   <td> <p> 這是項目在清單和報表中顯示的[!UICONTROL預算成本]。</p><p>另請參見本文中的「[!UICONTROL預算成本]」。</p></td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL項目管理]</td> 
   <td>一組策略，用於管理項目建立、分類和命名的閾值。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL項目開銷]</td> 
   <td>在[!UICONTROL Hour]報表中，此欄位保留為與小時類型為[!UICONTROL項目時間]記錄的小時相關的財務資訊。 項目可以有自己的開單費率，如果直接在項目上記錄一小時，則這些費率將用於計算。 根據項目設定，項目也可以有不同的幣種，並且這些小時可以進行貨幣兌換。 [!UICONTROL項目開銷]對象允許 [!DNL Workfront] 來獲取資訊。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL項目所有者]</td> 
   <td>負責管理項目的範圍、時間線和分配的用戶。 更改單、財務更改和交付項的預設審批人。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL項目規劃]</td> 
   <td>開發和維護項目計畫的流程。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL項目發起人]</td> 
   <td>每個用戶都應與的指定利益相關方配置檔案相關。 在 [!DNL Workfront]，這些被指定為[!UICONTROL訪問級別]</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL項目團隊]</td> 
   <td> <p>分配給項目的用戶或角色的集合</p> <p>有關詳細資訊，請參見 <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md">項目團隊概述</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL項目跟蹤]</td> 
   <td>用於測量項目運行狀況和範圍的資料</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL投影]</td> 
   <td> <p>根據任務、問題或項目的計畫小時數和完成百分比估計工作完成時間的時間戳。</p> <p>這是指任務、問題或項目的日期或[!UICONTROL持續時間]。 通常，它指定在某些工作已經完成或已經過一段時間後，對工作項的壽命更真實的日期和持續時間。 </p> <p>例如，任務的[!UICONTROL預計完成日期]是 [!DNL Workfront] 根據迄今為止已經完成多少工作、分配了多少人以及自開始日期以來已經過多少時間，估計任務將完成。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL證明截止時間]</td> 
   <td> <p>在包含[!UICONTROL文檔版本]對象（如[!UICONTROL文檔版本]報表和[!UICONTROL校樣批准]報表）的報告中，此欄位顯示證明截止日期的週日、日期、時間和年份。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL證明決定]</td> 
   <td> <p>在包含[!UICONTROL文檔版本]對象（如[!UICONTROL文檔版本]報告和[!UICONTROL校樣批准]報告）的報告中，此欄位顯示證明的決策狀態（待定、需要更改或批准）</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL校樣名稱]</td> 
   <td> <p>在包含[!UICONTROL文檔版本]對象（如[!UICONTROL文檔版本]報告和[!UICONTROL校樣批准]報告）的報告中，此欄位顯示校樣名稱。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL校樣頁]</td> 
   <td> <p>在包含[!UICONTROL文檔版本]對象（如[!UICONTROL文檔版本]報告和[!UICONTROL校樣批准]報告）的報告中，此欄位顯示校樣中包括的頁數。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL證明進度]</td> 
   <td> <p>在包含[!UICONTROL文檔版本]對象（如[!UICONTROL文檔版本]報告和[!UICONTROL校樣批准]報告）的報告中，顯示校樣（[!UICONTROL已發送]、[!UICONTROL已開啟]、[!UICONTROL已注釋]、[!UICONTROLcontrol決定）。</p> <p>有關詳細資訊，請參見 <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md#understanding-progress-and-status" class="MCXref xref">證明進度概述</a> 在 <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md" class="MCXref xref">證明進度和狀態概述</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL校對]</td> 
   <td>一種審閱過程，其中一個或多個用戶對應在影像、文本文檔、視頻或互動式Web內容中更改的內容進行標籤和評論。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL公共]</td> 
   <td>在[!UICONTROL Note]或[!UICONTROL Document]上，此選項使其他用戶甚至外部人員都可以訪問該對象 [!DNL Workfront]。 對於[!UICONTROL幫助台隊列],[!UICONTROL公共]表示所有可提交問題的用戶都可以通過[!UICONTROL幫助台]區域提交問題。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL質量]</td> 
   <td>對組織內工作質量的認識。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL隊列]</td> 
   <td>也稱為[!UICONTROL幫助台隊列]。 這是已發佈到[!UICONTROL幫助台]區域的項目，允許用戶向其提交問題。 通常為特定主題（如Bug、Project Requests等）建立隊列。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL隊列屬性]</td> 
   <td>這些設定定義要發佈到[!UICONTROL幫助台]的項目的「發佈提交規則」。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL隊列主題]</td> 
   <td> <p>[!UICONTROL幫助台隊列]上的屬性，允許用戶提交問題以選擇主題。 主題可以：</p> 
    <ul> 
     <li>與自定義資料表單關聯。</li> 
     <li>通過選定主題上的路由規則集，將問題自動分配給用戶、角色或團隊。</li> 
     <li>通過選定主題上的路由規則集將問題移動到其他項目或隊列。</li> 
    </ul> <p>有關詳細資訊，請參見 <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">建立隊列主題</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL秩]</td> 
   <td> <p>在[!UICONTROL訪問級別]報告中，可以手動指示[!UICONTROL訪問級別]的[!UICONTROL級別]。 這對你有幫助，因為 [!DNL Workfront] 管理員，以直觀地確定與每個訪問級別關聯的複雜性級別。 例如，您可以為較複雜（[!UICONTROL Plan]級別）的訪問級別提供較低的數字，而為較不複雜（[!UICONTROL Requester]級別）的訪問級別提供較高的數字。 您無法對標準訪問級別進行排序。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL就緒]</td> 
   <td> <p>任務報告上的此欄位指示積壓工作上的[!UICONTROL Agile]任務是否標籤為[!UICONTROL Ready]。 此標誌僅適用於[!UICONTROL Agile]任務，這些任務是分配給[!UICONTROL Agile]團隊的任務。 </p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL循環頻率]</td> 
   <td> <p>顯示在循環任務父項的[!UICONTROL任務詳細資訊]或[!UICONTROL編輯任務]框中的欄位。 它是重複執行中任務的頻率。 有關建立循環任務的資訊，請參閱 <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">建立循環任務</a>。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL引用編號]</td> 
   <td> <p>項目、任務和問題在建立時自動與唯一的參考編號關聯。 您可以在項目、任務或問題的[!UICONTROL詳細資訊]頁或清單或報表中查看[!UICONTROL參考編號]。 </p> <p><b>提示</b><p><br>當兩個項目具有相同名稱時，可以順從於引用編號，因為引用編號始終唯一。 </p> <p>[!DNL Workfront] 在系統級別自動生成順序參考編號。 每個項目、任務或問題都獲取序列中的下一個可用編號。 <br></p> <p>例如，如果用戶A建立任務， [!DNL Workfront] 可能會自動將任務分配為「參考編號100」。 如果用戶B在此之後立即建立問題， [!DNL Workfront] 將問題指定為「參考編號101」。 不能手動編輯引用編號。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL拒絕問題]</td> 
   <td>在項目或任務報表中，這是在項目或任務審批被拒絕時建立的問題。 有關拒絕問題的資訊，請參閱文章 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">為工作項建立審批流程</a>。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL剩餘風險成本]</td> 
   <td> <p>顯示項目的[!UICONTROL計畫風險成本]與項目上所有風險的所有[!UICONTROL實際成本]總和之間差異的項目欄位。 </p> <p>項目的[!UICONTROL剩餘風險成本]使用以下公式計算：</p> <p><code>[!UICONTROL Remaining Risk Cost] = Project [!UICONTROL Planned Risk Cost] - SUM([!UICONTROL Actual Cost] for all risks)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL重新規劃]</td> 
   <td>更改項目日期以修復或克服問題。 例如，需要重新計劃一個已暫停數月的項目，以反映準確的日期。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL報告]</td> 
   <td>包含給定資訊的圖表或表 [!DNL Workfront] 對象及其相關屬性。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL請求]</td> 
   <td> <p>在單個集中隊列中篩選且與正在進行的工作無關的問題類型。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL請求隊列]</td> 
   <td>由流量和篩選流程管理的問題積壓。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL請求速度]</td> 
   <td>接收和完成請求的工作週期總時間。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL請求者]</td> 
   <td>通常為許可證類型。 具有請求者許可證的用戶可以提交對系統中將要進行的新工作的請求。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL保留時間]</td> 
   <td>在用戶的個人時間上指定的天數，表示用戶將無法工作。 請參閱「[!UICONTROL非工作日]」。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL解決問題]</td> 
   <td> <p>在問題報告中，在視圖或篩選器中使用此欄位來引用解決問題的問題。 </p> <p>有關在報表中顯示解析對象的資訊，請參見 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">查看報表中可解析和解析對象資訊</a> 在 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解析和可解析對象概述 </a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL解析項目]</td> 
   <td> <p>在問題報告中，在視圖或篩選器中使用此欄位來引用解決問題的項目。 </p> <p>有關在報表中顯示解析對象的資訊，請參見 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">查看報表中可解析和解析對象資訊</a> 在 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解析和可解析對象概述 </a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL解決任務]</td> 
   <td> <p>在問題報告中，在視圖或篩選器中使用此欄位來引用解決問題的任務。 </p> <p>有關在報表中顯示解析對象的資訊，請參見 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">查看報表中可解析和解析對象資訊</a> 在 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解析和可解析對象概述 </a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資源]</td> 
   <td>系統中現有並分配給項目團隊和任務的用戶和/或角色。</td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Resource Estimates</td> 
    <td>This report captures information about an area in&nbsp;Workfront that has been removed. The report might display legacy information but it does not update with current data. Although not recommended, you may update the information in this report using the API. For information about how you estimate resources for projects, see <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>. </td> 
   </tr>
   <td>Resource Grid</td> 
   <td>A visual table showing the allocation of resources.</td> 
  </tr> -->
  <tr> 
   <td>[!UICONTROL資源管理]</td> 
   <td> <p>[!UICONTROL Resource Management]是一組企業工具，允許您根據資源的可用性準確預測資源的使用情況，以便必須完成的工作按時和按預算完成。 </p> <p>使用資源管理工具，您可以計畫資源的長期能力和短期計畫需求。 </p> <p>有關中的資源管理的資訊 [!DNL Workfront]，請參閱 <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">資源管理入門</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資源管理器ID]</td> 
   <td><p>在項目報告中，在建立篩選器以查找特定資源管理器時可以使用此選項。 </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資源管理器]</td> 
   <td> <p>在項目報告或清單視圖中，這是一個資訊欄位，顯示指定在項目上執行資源管理活動的用戶。  在報表中使用「[!UICONTROL資源管理器]」時，將顯示資源管理器清單，項目上的每個資源管理器都用逗號分隔。 在給定項目上最多可指定30名資源經理。</p> <p>有關詳細資訊，請參閱文章 <a href="../../../manage-work/projects/planning-a-project/designate-resource-managers-for-projects-and-templates.md">為項目或模板指定資源經理 </a>。</p> </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL資源規劃器預算小時數] </td> 
   <td>在[!UICONTROL資源規劃器]中為項目和與項目關聯的資源編入預算的小時數。 另請參見本文中的「[!UICONTROL預算小時數]」。 </td> 
  </tr>  
  <tr> 
   <td>[!UICONTROL資源規劃器] </td> 
   <td>高級 [!DNL Workfront] 工具，用於查看和管理跨項目、作業角色或用戶的資源。 有關資訊，請參見 <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">資源計畫器概覽</a>。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資源規劃器預算人工成本]</td> 
   <td> <p>這些是與使用資源計畫器為項目任務職責編製預算的小時數關聯的成本。 </p> <p>另請參閱本文中的「預算人工成本」。 </p> </td>

</tr> 
  <tr> 
   <td>[!UICONTROL資源池]</td> 
   <td> <p>資源池是可以與項目關聯的用戶的集合。同一資源池中的用戶通常屬於同一部門，具有相似或互補的技能，或由同一預算提供資金。 您可以將多個資源池與項目或用戶相關聯。 資源池可以專門分配給項目或由多個項目共用。</p> 
   <p>有關資源池的詳細資訊，請參見 <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> 資源池概述 </a>。</p> 
   <p>在項目報告中，資源池顯示與項目關聯的所有池。 此對象不能用於分組。</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資源利用率]</td> 
   <td>一個報告，顯示在某個時間段內可用的小時數以及報告中每個用戶計畫的小時數。 此值也計算為[!UICONTROL Average Hours Per Day]和分配百分比。</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL結果]</td> 
   <td>在 [!DNL Workfront Goals]，結果是目標的進度指標。 它可以是數字、百分比值或您手動更新的幣種金額。 您不能在報表中顯示結果，並且無法通過 [!DNL Workfront] API。 有關活動的資訊，請參見 <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">開始Adobe Workfront目標中的結果和活動</a>。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL收入]</td> 
   <td>任務或項目的可開單金額。 金額可以是小時、固定或兩者的組合。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL收入類型]</td> 
   <td>收入類型確定任務如何應計收入。 一些示例包括[!UICONTROL固定小時]、[!UICONTROL角色小時]和[!UICONTROL角色小時/小時（帶上限）]。 有關跟蹤收入的資訊 [!DNL Workfront] 見 <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">開單和收入概覽</a>。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL審閱者]</td> 
   <td>通常為許可證類型。 具有[!UICONTROL Reviewer]許可證的用戶能夠審閱和批准系統中的工作項。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL風險]</td> 
   <td> <p>這可參考以下概念： [!DNL Workfront]:</p> 
    <ul> 
     <li> <p>項目上的一個欄位，它指示項目的風險。 您可以根據風險級別確定項目執行的優先順序。 項目可能具有以下風險級別：</p> <p>- [!UICONTROL非常低]</p> <p>- [!UICONTROL低]</p> <p>- [!UICONTROL介質]</p> <p>- [!UICONTROL高]</p> <p>- [!UICONTROL非常高]</p> <p>無法自定義您為項目指明的風險級別。 </p> <p> 有關更新項目風險的資訊，請參閱文章的「項目設定」部分 <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">編輯項目</a>。 您可以在報表中顯示項目的風險欄位。 </p> </li> 
     <li> <p>在項目生命期內可能發生的事件，它標識了對項目成本、範圍或計畫的潛在影響。 您可以定義項目的潛在風險，並在構建項目業務案例時將其發生的可能性或成本關聯起來。 有關將風險添加到項目業務案例的資訊，請參閱「建立和編輯項目風險」。 </p> <p>不能在報告中顯示[!UICONTROL業務案例]中定義的風險。 您只能在報表和清單中顯示幾種類型的風險成本。 </p> </li> 
    </ul> </td>

</tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL風險成本]</td> 
   <td> <p>與項目風險相關的成本。 以下是與可在報表中顯示的項目關聯的風險成本：</p> 
    <ul> 
     <li> <p>[!UICONTROL實際成本]:一個關於風險的欄位，該欄位顯示已發生風險的實際成本。 除了報告和清單外，在編輯或建立風險時，還可以在[!UICONTROL編輯風險]框中找到它。 </p> <p>有關項目、任務或發放成本，請參閱本文中的「[!UICONTROL實際成本]」。 </p> </li> 
     <li> <p>[!UICONTROL計畫風險成本]:項目上的一個欄位，其中顯示項目的所有[!UICONTROL潛在風險成本]。 另請參見本文中的「[!UICONTROL計畫風險成本]」。 </p> <p>有關潛在風險成本的資訊，請參閱 <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">計算潛在風險成本 </a>。 </p> </li> 
     <li> <p>[!UICONTROL剩餘風險成本]:項目上的一個欄位，顯示所有風險的[!UICONTROL實際成本]總和與[!UICONTROL計畫風險成本]之間的差。 另請參閱本文中的「剩餘風險成本」。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL風險管理]</td> 
   <td>識別、減輕和監控風險的流程。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL角色]</td> 
   <td>請參閱本文中的「[!UICONTROL作業角色]」。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL路由]</td> 
   <td>自動分配或移動問題，通常是由於隊列主題或作為隊列的預設路由（路由規則）。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL路由規則]</td> 
   <td>「項目」和「隊列」上的設定，可自動將問題分配給用戶、角色或團隊，或將問題移至其他項目或隊列。 路由規則通常與幫助台隊列一起使用，以自動分配傳入的問題。</td> 
  </tr> 
 </tbody> 
</table>

## S - U

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>物件名稱</th> 
   <th>說明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL已保存的搜索]</td> 
   <td>已保存搜索條件的搜索。 「保存的搜索」(Saved Searches)使每個搜索都可以輕鬆運行，而無需再次輸入搜索標準。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL方案](在 [!DNL Workfront Fusion]) </td> 
   <td> <p>方案由一系列步驟（模組）組成，這些步驟（模組）指示應如何在應用/服務之間傳輸和轉換資料。</p> <p>有關中的方案的資訊 [!DNL Workfront Fusion]，請參閱 <a href="../../../workfront-fusion/scenarios/scenario-overview.md" class="MCXref xref">[!DNL Adobe Workfront Fusion] 方案概述</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL方案](在 [!DNL Workfront Scenario Planner]) </td> 
   <td> <p>在 [!DNL Scenario Planner]，方案是計畫的副本。 </p> <p>的 [!DNL Scenario Planner] 需要額外的許可證。 有關 [!DNL Workfront Scenario Planner]，請參閱 <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">的 [!DNL Scenario Planner] 概述</a>。 </p> <p>有關建立方案的資訊，請參閱 <a href="../../../scenario-planner/create-and-compare-scenarios-for-a-plan.md">在中建立和比較計畫方案 [!DNL Scenario Planner]</a>。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL計畫]</td> 
   <td>每週工作計畫，包括工作時間，與休假日（如節假日）和例外日（如星期六工作日）相結合。 計畫可應用於項目和用戶。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL計畫例外]</td> 
   <td>也稱為[!UICONTROL Modified Shift]。 計畫的天數與計畫定義的常規每週工作時間不同。 例如，計畫工作的星期六（如果計畫設定為只在星期一到星期五工作）將是[!UICONTROL計畫例外]。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL計畫報告]</td> 
   <td> <p>在生成報告報告時，如果報告已使用[!UICONTROL計畫報告]欄位計畫交付，則可以顯示有關報告計畫的資訊。 此欄位在項目符號清單中顯示多個值，每個報表的每個計畫都顯示一個值。 有關計畫報告的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md" class="MCXref xref">報告交付概述</a>。</p> <p>由於此欄位顯示多個值，因此不能在分組中使用。 您只能在篩選器或視圖中訪問它。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL範圍更改]</td> 
   <td>[!UICONTROL審核跟蹤]，如果處於活動狀態，則每當對項目或任務的範圍進行更改時都會生成注釋，例如[!UICONTROL任務持續時間]或[!UICONTROL前置任務]已更改。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL節]</td> 
   <td>螢幕上的一個區域，帶有自己的標題，用於組織自定義資料以用於顯示目的。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL節分隔符]</td> 
   <td>截面之間的間隙或邊框。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL安全性]</td> 
   <td>允許用戶與系統中的某些對象而不是其他對象交互的設定。 另請參見本文中的「[!UICONTROL訪問級別]」。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL安裝程式]</td> 
   <td>管理員可以設定系統配置和首選項的區域。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL嚴重性]</td> 
   <td> <p>[!UICONTROL嚴重性]表示項目對完成工作的影響。 例如，高[!UICONTROL嚴重性]的問題可能會完全阻止任務的完成，但低[!UICONTROL嚴重性]的問題可能只是表面問題。</p> <p>有關詳細資訊，請參見 <a href="../../../manage-work/issues/issue-information/update-issue-severity.md" class="MCXref xref"> 更新問題嚴重性</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL嚴重性]</td> 
   <td>請參閱本文中的「[!UICONTROL嚴重性]」。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL共用]</td> 
   <td>允許其他用戶查看或編輯中的特定項目的操作 [!DNL Workfront]。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROLSlack日期]</td> 
   <td>在任務視圖或報表中，[!UICONTROLSlack日期]顯示任務肯定會影響項目的[!UICONTROL完成日期]的確切日期。 有關任務的[!UICONTROLSlack日期]的資訊，請參見 <a href="../../../manage-work/tasks/task-information/task-slack-date.md" class="MCXref xref">任務Slack日期概述</a>。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL智慧分配]</td> 
   <td> <p>將任務或問題分配給用戶時， [!DNL Workfront] 根據最佳用戶完成工作的時間以及他們與項目的關係，提出建議([!UICONTROL Smart Assignments])。</p> <p>有關詳細資訊，請參見 <a href="../../../manage-work/tasks/assign-tasks/smart-assignments.md" class="MCXref xref">智慧分配概述</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL源]</td> 
   <td> <p>指示另一個對象的父對象。 例如，附加到任務的文檔在[!UICONTROL Document]報表或視圖的[!UICONTROL Source]欄位中具有任務的名稱；在項目下記錄的問題在「問題」報告或視圖的[!UICONTROL源]欄位中具有項目名稱。 </p> 
   <p>以下報表顯示「源」列，在該列中可以查看有關父對象的資訊：</p>
  <ul><li>發佈報告</li>
    <li>工時報告</li>
    <li>文檔報表 </li>
    </ul>
   <p>如果用戶對問題、小時或文檔的父對象沒有權限，則即使將報告配置為顯示或以其他用戶的訪問權限傳遞，報告的「源」列也將顯示為空。 </p>
   <p> 為了在報告中顯示有關父對象的資訊，我們建議為父對象添加一列，在列中可以顯示父對象的名稱。 </p>
    <p>例如，可以將下列任何一項添加到具有「源」列的報表中： </p>
    <ul><li>文檔或小時報表的「項目名稱」(Project Name)、「任務名稱」(Task Name)或「發行名稱」(Issue Name)列。</li>
    <li>發佈報告的「項目名稱」或「任務名稱」列。 </li> </ul>
    有關詳細資訊，請參見 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md">運行並提交具有其他用戶訪問權限的報告</a>

</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL開始日期]</td> 
   <td> <p>項目工作設定為開始的日期。 中有幾個開始日期 [!DNL Workfront]: </p> 
    <ul> 
     <li>[!UICONTROL已計畫]</li> 
     <li>[!UICONTROL實際]</li> 
     <li>[!UICONTROL投影] </li> 
    </ul> <p>在[!UICONTROL比率報表]中，這是項目層職務角色的新開單比率開始的日期。 與此日期之後與項目關聯的小時數乘以此開單費率計算項目收入。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL狀態]</td> 
   <td> <p>用於指示工作項或戰略目標的工作流位置的指示符。</p> <p>對於項目，[!UICONTROL狀態]是項目上的一個設定，指示項目是否為：</p> 
    <ul> 
     <li>[!UICONTROL當前]</li> 
     <li>[!UICONTROL保持] </li> 
     <li>[!UICONTROL完成] </li> 
     <li>[!UICONTROL死]</li> 
    </ul> <p>有關項目狀態的詳細資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md">訪問系統項目狀態清單</a>。</p>
    <p>對於任務，[!UICONTROL狀態]是任務上的一個設定，它指示任務是否為：</p> 
    <ul> 
     <li>[!UICONTROL新建]</li> 
     <li>[!UICONTROL正在進行]</li> 
     <li>[!UICONTROL完成]</li> 
    </ul> <p>有關任務狀態的詳細資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md">訪問系統任務狀態清單</a></p> <p>對於問題，[!UICONTROL狀態]是問題上的一個設定，指示此問題是否為：</p> 
    <ul> 
     <li>[!UICONTROL新建]</li> 
     <li>[!UICONTROL正在進行]</li> 
     <li>[!UICONTROL正在等待反饋]</li> 
     <li>[!UICONTROL保持]</li> 
     <li>[!UICONTROL已解析]</li> 
     <li>[!UICONTROL將不解決]</li> 
     <li>[!UICONTROL不能重複]</li> 
     <li>[!UICONTROL已驗證完成]</li> 
     <li>[!UICONTROL已重新開啟]</li> 
    </ul> <p>有關發行狀態的詳細資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">訪問系統發佈狀態清單</a>。</p> 
    <p>對於戰略目標，[!UICONTROL狀態]是目標上的一個設定，用於指示目標是否為：</p> 
     <ul> 
      <li>[!UICONTROL活動]</li> 
      <li>[!UICONTROL草稿]</li> 
      <li>[!UICONTROL非活動]</li> 
      <li>[!UICONTROL已關閉]</li> 
     </ul> 
     <p>有關戰略目標的詳細資訊，請參閱本文中的「[!UICONTROL目標]」或「[!UICONTROL目標]」。 </p> 
     <p>對於戰略目標，僅當您的組織已購買時，此欄位才可見 [!DNL Workfront Goals]。 有關使用 [!DNL Workfront Goals]，請參閱 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] 概述</a>。 </p>
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL狀態更改]</td> 
   <td>[!UICONTROL審計跟蹤]。 當用戶更改項目、任務或問題的狀態時，將生成附註。</td> 
  </tr> 
  <tr> 
   <td>狀態圖示</td> 
   <td> <p>您可以將內置的[!UICONTROL狀態表徵圖]欄位添加為視圖中的列，以增強對對象關鍵點的可見性，例如：</p> 
    <ul> 
     <li>對象附加了文檔</li> 
     <li>對象與批准進程關聯</li> 
     <li>對象具有與其關聯的附加註釋</li> 
     <li>費用可開單或可報銷 </li> 
     <li>任務在關鍵路徑上</li> 
     <li>用戶屬於公司、團隊或位於其他時區 </li> 
    </ul> <p>可以在以下對象的視圖中添加[!UICONTROL狀態表徵圖]欄位： </p> 
    <ul> 
     <li>[!UICONTROL任務]</li> 
     <li>[!UICONTROL問題]</li> 
     <li>[!UICONTROL項目]</li> 
     <li>[!UICONTROL模板任務]</li> 
     <li>[!UICONTROL模板]</li> 
     <li>[!UICONTROL費用]</li> 
     <li>[!UICONTROL文檔]</li> 
     <li>[!UICONTROL用戶]</li> 
    </ul> <p>有關詳細資訊，請參見 <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">視圖中的內置狀態表徵圖</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL狀態更新]</td> 
   <td> <p>此欄位顯示用戶在「[!UICONTROL更新狀態]」欄位中提供的最新狀態更新。 在[!UICONTROL狀態更新]列中不顯示對狀態更新所做的注釋。</p> <p>要顯示「[!UICONTROL New]，」「[!UICONTROL In Process]」和「[!UICONTROL Complete]」狀態，請使用[!UICONTROL Status]列。</p> <p>在[!UICONTROL狀態更新]列中不顯示對狀態更新所做的注釋。</p> <p>有關狀態的詳細資訊，請參閱文章 <a href="../../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">更新任務狀態</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL狀態]</td> 
   <td>請參閱本文中的「[!UICONTROL狀態]」。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL情節提要]</td> 
   <td>一個圖表，它表示故事的狀態（敏捷方法中的任務）以及它們在完成過程中的進展。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL故事小時數]</td> 
   <td>用於衡量故事的難度或複雜性的度量。 敏捷團隊可以選擇是使用「小時」還是「分」。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL故事點]</td> 
   <td>用於衡量故事的難度或複雜性的度量。 敏捷團隊可以選擇是使用「小時」還是「分」。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Strategic]</td> 
   <td>更改組織或組織工作方式的長期工作。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL戰略協調]</td> 
   <td>衡量和調整公司在投資組合和計畫中的目標。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL訂閱伺服器]</td> 
   <td> <p>訂閱項目、任務或問題的用戶。</p> <p>在報表中使用此欄位時，將顯示訂閱伺服器清單，每個訂閱伺服器用逗號分隔。</p> <p>有關詳細資訊，請參閱文章 <a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref">訂閱中的項目 [!DNL Adobe Workfront]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL摘要任務]</td> 
   <td>請參閱本文中的「[!UICONTROL父任務]」。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL子任務]</td> 
   <td>子任務，位於父任務下。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL系統治理]</td> 
   <td>一組控制系統更改和維護的策略。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL系統整合]</td> 
   <td>將不同的計算系統和軟體應用程式物理或功能連接在一起以作為一個協調的整體。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL任務]</td> 
   <td> <p>作為實現最終目標（完成項目）的步驟必須執行的活動。</p> <p>有關詳細資訊，請參見 <a href="../../../manage-work/tasks/task-information/tasks-overview.md" class="MCXref xref">任務概述</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL任務屬性]</td> 
   <td>與Task關聯並指明Task某些詳細資訊的其他欄位或對象。 一些示例包括[!UICONTROL計畫完成日期]和[!UICONTROL狀態]。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL任務約束]</td> 
   <td>請參見「[!UICONTROL約束類型]」和「[!UICONTROL約束日期]」。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL任務管理]</td> 
   <td>一組策略，用於管理任務建立、分配、關閉和可見性的閾值。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL任務所有者]</td> 
   <td>負責估計工作量和完成任務的團隊或用戶</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL團隊]</td> 
   <td> <p>向類似目標或業務目標努力的用戶集合。 通過將團隊分配給工作項目，可以將這些用戶集體分配給工作項目。</p> <p>有關團隊的詳細資訊，請參見 <a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref">團隊概述</a>。</p> <p>項目可以具有[!UICONTROL項目團隊]，其中包含與項目上的工作相關聯的所有用戶或角色。</p> <p>有關項目團隊的詳細資訊，請參見 <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">項目團隊概述</a></p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode,SnippetConitions_MaturityModel.Ad hoc"> 
    <td>Team Goals</td> 
    <td>Team goals which contribute to the metrics of enterprise or department goals.</td> 
   </tr>
  --> 
  <tr> 
   <td>[!UICONTROL模板]</td> 
   <td> <p>項目模板是最可重複項目的一般大綱。 在建立項目模板時，您可以定義任務、隊列主題、自定義表單、附加文檔或審批，以節省您必須建立新項目的時間。 </p> <p>您可以將模板附加到現有項目，也可以使用它們來構建新項目。 在模板上指定的所有資訊都會傳輸到使用它建立的項目。 </p> <p>有關模板的詳細資訊，請參見 <a href="../../../manage-work/projects/create-and-manage-templates/project-template-overview.md">項目模板概述</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL模板任務]</td> 
   <td>屬於模板的任務。 模板任務將成為使用模板建立的項目中的任務。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL線程]</td> 
   <td>[!UICONTROL Note]及其與特定主題相關的答復集合。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL縮略圖]</td> 
   <td> <p> 在[!UICONTROL文檔]清單或報告中，它會在縮略圖中顯示文檔的預覽。 </p> <p> 選擇 <strong>[!UICONTROL縮略圖]</strong>  查看報告中33-66像素寬的縮略圖。 </p> <p>修改清單或報表中列的寬度時，縮覽圖的大小會調整。</p> <p>另請參見本文中的「[!UICONTROL大縮略圖]」。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL關閉時間]</td> 
   <td>當用戶在其配置檔案中指示休息時間時，可以生成[!UICONTROL Time Off]報告來查看。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL時間表]</td> 
   <td> <p>一種工時記錄卡，允許用戶輸入他們在項目、任務或問題上所花的實際小時數，或他們在與工作無關的其他活動（如會議或培訓）上所花的小時數。 除了輸入您所花費的工作時間外，您還可以使用「工時類型」定義時間條目來指明該時間是與工作相關還是與間接費用時間有關。 有關工時單的資訊，請參見 <a href="../../../timesheets/timesheets/timesheets-overview.md">工時單概述</a>。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL時間表配置檔案]</td> 
   <td> <p>[!UICONTROL時間表配置檔案]是一個模板 [!DNL Workfront] 用於為與其關聯的用戶自動建立工時單。 </p> <p>您可以配置多個設定，這些設定將在建立時應用於每個時間表。 其中一些設定是：建立時間表的頻率（每週、每隔一週、每月兩次或每月一次）、時間表的開始日、時間表批准者、用戶可與記錄小時數關聯的可用[!UICONTROL小時類型]。</p> </td> 
  </tr> 
  <tr > 
   <td>[!UICONTROL上父ID] </td> 
   <td> <p>此欄位允許您識別和篩選有關清單或報告中頂級組及其子組的資料。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL頂層父名稱] </td> 
   <td> <p>此欄位允許您標識清單或報表的[!UICONTROL視圖]中有關頂級組及其子組的資料。</p> <p>也可以使用[!UICONTROL頂級父ID]欄位執行此操作。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL總小時數]</td> 
   <td> <p>在[!UICONTROL項目報表]中，此欄位顯示項目上所有小時的捨入和，即上次計算項目財務的時間。 [!UICONTROL實際小時數]反映了在項目上記錄的確切小時數。 通常，[!UICONTROL實際小時數]應與[!UICONTROL總小時數]匹配。 如果[!UICONTROL總小時數]顯示與[!UICONTROL實際小時數]欄位明顯不同，則必須重新計算項目上的財務。</p> <p>有關重新計算項目財務的詳細資訊，請參閱文章 <a href="../../../manage-work/projects/project-finances/recalculate-project-finances.md" class="MCXref xref">重新計算項目財務</a>。</p> <p>在時間表[!UICONTROL標準]視圖中，此欄位引用為時間表上顯示日期的項目記錄的總小時數。 此內置視圖中時間表的[!UICONTROL Total Hours]欄位引用「[!UICONTROL hoursDuration]」欄位，該欄位動態計算時間表「開始」和「結束」日期之間的小時數差。 如果用戶在時間表的時間範圍內記錄的時間超過可用小時數，則此列將用紅色顯示[!UICONTROL Total Hours]列。 有關詳細資訊，請參見 <a href="../../../timesheets/create-and-manage-timesheets/view-total-hours-timesheets.md" class="MCXref xref">查看工時單上的總工時</a>。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL跟蹤模式]</td> 
   <td> <p>任務的屬性。 這確定了如何更新任務的預計時間表，然後更新任務。 例如：</p> 
    <ul> 
     <li>[!UICONTROL用戶必須更新]要求手動更新任務。 否則，它將變為[!UICONTROL Bethind Schedule]，然後變為[!UICONTROL Late]。</li> 
     <li>[!UICONTROL自動完成]將在到期日（或[!UICONTROL計畫完成日期]）已過時自動完成任務。</li> 
    </ul> <p>有關詳細資訊，請參見 <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">任務跟蹤模式概述</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL觸發器]</td> 
   <td>啟動方案的事件。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL故障任務]</td> 
   <td>條件為[!UICONTROL Late]、[!UICONTROL Bet Schedule]或[!UICONTROL At Risk]的不完整任務。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL未分配任務]</td> 
   <td>未分配給任何用戶、角色或團隊的任務。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL更新類型]</td> 
   <td> <p>項目上的一個設定，用於確定何時重新計算項目的預計時間線。 選項包括：</p> 
    <ul> 
     <li>[!UICONTROL自動和更改時]</li> 
     <li>[!UICONTROL僅自動]</li> 
     <li>[！僅UICONTROL手動] </li> 
    </ul> <p>有關詳細資訊，請參見 <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">選擇項目更新類型 </a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL用戶]</td> 
   <td>在中建立的帳戶 [!DNL Workfront] 允許用戶登錄並與系統交互。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL用戶委派]</p> </td> 
   <td> <p>可報告對象，它告訴您：</p> 
    <ul> 
     <li>哪些用戶已委託任務、發放和項目審批</li> 
     <li>哪些用戶已將任務、發放和項目批准委託給他們</li> 
     <li>當這些委託開始和結束時</li> 
    </ul> <p>要瞭解更多資訊，請參閱 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md" class="MCXref xref">建立用戶委派報告</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL用戶介面]</td> 
   <td>所有視覺和交互方面 [!DNL Workfront] 的子菜單。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL用戶介面首選項]</td> 
   <td>[!UICONTROL用戶介面設定]。 [!DNL Workfront] 管理員可以更改這些設定以自定義用戶介面的各個方面。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL利用率]</td> 
   <td>根據分配的計畫、PTO和當前工作量確定用戶或角色的可用性。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL用戶利用率]</td> 
   <td> <p>與報告相結合的搜索，該報告顯示如何分配或過度分配用戶（資源）。 請參閱本文中的「[!UICONTROL資源利用率]」。</p> </td> 
  </tr> 
 </tbody> 
</table>

## V - Z

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>物件名稱</th> 
   <th>說明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UCONTROL速度]</td> 
   <td>衡量工作週期總時間（完成某項工作需要多長時間）以及在最初承諾時間內完成工作的頻率（工作與承諾比率）。</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL視圖]</td> 
   <td> <p>視圖可用於修改報表或項目、任務或問題清單中的列，也可用於指示用戶僅有權查看訪問級別或權限共用級別的資訊。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL視圖表徵圖]</td> 
   <td> <p> 此欄位與「狀態表徵圖」(Status Icons)欄位相同，但僅適用於以下視圖： </p> 
    <ul> 
     <li> [!UICONTROL文檔] </li> 
    </ul> <p> 有關詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">視圖中的內置狀態表徵圖</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！上個月的UICONTROL視圖]</td> 
   <td> <p>在報告清單中，它顯示報告在上個月被查看的次數。<br>有關報表清單中使用資訊的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">查看報表使用情況</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL視圖上季度]</td> 
   <td>在報告清單中，它顯示報告在上一季度中被查看的次數。<br>有關報表清單中使用資訊的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" >查看報表使用情況</a>。</td> 
  </tr> 
  <tr> 
   <td>[！去年的UICONTROL視圖]</td> 
   <td>在報告清單中，它顯示報告在過去一年中被查看的次數。<br>有關報表清單中使用資訊的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">查看報表使用情況</a>。</td> 
  </tr> 
  <tr> 
   <td>[！本月的UICONTROL視圖]</td> 
   <td> <p>在報告清單中，它顯示本月查看報告的次數。<br>有關報表清單中使用資訊的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">查看報表使用情況</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！本季度的UICONTROL視圖]</td> 
   <td>在報告清單中，它顯示該報告在本季度內被查看的次數。<br>有關報表清單中使用資訊的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">查看報表使用情況</a>。</td> 
  </tr> 
  <tr> 
   <td>[！今年的UICONTROL視圖]</td> 
   <td>在報告清單中，它顯示報告在今年內被查看的次數。<br>有關報表清單中使用資訊的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md">查看報表使用情況</a>。</td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL work]</code> </td> 
   <td> <p>在項目、任務或發放報表中，在文本模式下使用以下語句顯示項目、任務或發放的計畫小時數：</p>
   <p></p><p></p> 
   <p>有關使用文本模式的資訊，請參見 <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">文本模式語法概述</a>。 </p> 
   <p><b>提示</b> 
   <p>在問題報告中，添加[!UICONTROL計畫小時數]欄位之一將添加 <code>work </code>的子菜單。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作]</td> 
   <td> <p>兩種主要許可證類型之一。 此訪問權限比[!UICONTROL Plan]少，但可以在系統中建立和更新。 這比[!UICONTROL External]、[!UICONTROL Reviewer]或[!UICONTROL Requester]許可證類型的能力要多。</p> <p>有關詳細資訊，請參見 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] 許可證概述</a>。</p> <p>工作可能指項目、任務或問題的[!UICONTROL計畫小時數]。 有關詳細資訊，請參閱此表中的「[!UICONTROL工作]」欄位。 </p> <p>提示：在問題報告中，添加[!UICONTROL計畫小時數]欄位之一將添加 <code>work </code>的子菜單。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作細分結構]</td> 
   <td>項目團隊基於父/子關係要執行的任務的層次結構。</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL工作量] </td> 
   <td> 
    <p>項目經理可能決定使用此欄位而不是[!UICONTROL計畫小時數]來估計完成任務所需的工作量。 僅當滿足以下條件時，此欄位才可見：</p> 
     <ul> 
      <li> <p>任務具有[!UICONTROL簡單持續時間類型]。 </p> <p>提示：如果將任務[!UICONTROL持續時間類型]更新為任何其他類型，則此欄位將變為隱藏。 </p> </li> 
      <li>項目經理已啟用[!UICONTROL使用工作]以自動計算項目上的任務[!UICONTROL計畫小時數]欄位。 </li> 
     </ul> 
     <p>有關使用[!UICONTROL工作量]而不是[!UICONTROL計畫小時數]來估計任務工作量的資訊，請參見 <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">工作概述</a>。 </p> 
     <p>可以在任務報告和清單中顯示此欄位。</p> 
    </td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL工作項]</td> 
   <td> <p>此欄位指的是任務或問題 [!DNL Workfront]。 </p> <p>[!UICONTROL工作項]報告顯示任務和問題的資訊。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作管理組合]</td> 
   <td>[!UICONTROL工作績效指標](WPI)，它分配用於運行業務的工作與更改業務的比例。 「混合WPI」可幫助您在組織級別瞭解您的策略是否應用了任何實際工作分配。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作管理資源]</td> 
   <td>系統中有資格接收工作或跟蹤時間的人物的指定。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作管理角色和責任]</td> 
   <td>定義負責管理指定問題、任務、項目、項目或項目組合的範圍、執行和批准的所有者和利益相關方。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作管理SLA]</td> 
   <td>所有利益相關方商定的可量化指標。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作管理利益相關方]</td> 
   <td>對工作請求結果具有既得利益的用戶集合。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作管理觸點]</td> 
   <td>利益攸關方之間交流的數字化記錄。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作績效指標] </td> 
   <td> <p>混合比、容量、速度、質量和接合。</p> <p>WPI是[!UICONTROL工作效能指示器]的常用縮寫。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作進程]</td> 
   <td> <p>接收、排定優先順序和執行工作的方法。 執行工作的方式通常稱為「工作流」或「項目計畫」（包含日期、前置任務關係等的任務清單）。 </p> <p>工作流程的示例可能是生產單個資產或交付多資產市場活動。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作流模板]</td> 
   <td>在[!UICONTROL證明批准]報告中，此欄位顯示附加到證明的所有工作流模板。 如果沒有附加模板，則列為空。</td> 
  </tr>

<tr> 
   <td>[!UICONTROL工作時間]</td> 
   <td>

<p>表示用戶可用於實際工作（不包括開銷）的全職等效時間([!UICONTROL FTE])的百分比。 [!UICONTROL工作時間]必須是最多1的十進位數，並且不能是0。 例如，實際工作20%的可用性為0.2。</p>
   </p>該欄位的預設值是1，表示用戶將其整個[!UICONTROL FTE]用於實際的項目相關工作。  </p>
   <p>系統使用此數字計算用戶在實際項目相關工作中的可用性。 </p>
   <p> 計畫例外和休息時間也可能影響用戶容量。 </p>
   <p>有關在Workfront建立計畫的詳細資訊，請參見 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">建立計畫</a>。 </p>
    <p>Workfront根據[!UICONTROL設定]區域中的「資源管理」首選項計算用戶的可用性。 有關詳細資訊，請參見 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md/">配置資源管理首選項</a>。 </p> 
   <p>在編輯或建立用戶時，可以更新用戶的[!UICONTROL工作時間]。 有關資訊，請參見 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">編輯用戶的配置檔案</a></p> 
   <b>提示</b> 
   <p>將[!UICONTROL工作時間]值設定為1，以指示用戶可用於與項目相關的工作，且其整個全時對等。</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作時間]</td> 
   <td>在Workfront檔案中，該術語用於描述根據時間表分配給工作的時間。</td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL workRequiredExpression]</code> </td> 
   <td> <p>在項目、任務或發放報表中，在文本模式下使用以下語句顯示項目、任務或發放的計畫小時數，後跟「小時數」一詞：</p>
   <p></p><p></p>
    <p>有關使用文本模式的資訊，請參見 <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">文本模式語法概述</a>。 </p> </td> 
  </tr> 
 </tbody> 
</table>
