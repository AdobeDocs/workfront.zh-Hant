---
content-type: reference
navigation-topic: workfront-navigation
title: 辭匯表 [!DNL Adobe Workfront] 術語
description: 此 [!DNL Adobe Workfront] 字彙表列出Adobe Workfront中常用的辭彙。
feature: Get Started with Workfront
exl-id: 758072b3-775e-4771-9ae9-da0b38580c93
source-git-commit: fb538c6511514eedf81f4b9be452d5f87e3f7577
workflow-type: tm+mt
source-wordcount: '19138'
ht-degree: 0%

---

# 辭匯表 [!DNL Adobe Workfront] 術語

>[!IMPORTANT]
>
>本文應作為參考，以了解您在 [!DNL Adobe Workfront] 應用程式中 [!DNL Workfront] 說明檔案，或通常說到規劃和管理工作時。 我們目前正在更新此資訊，因此此表可能不完整。 當我們認為此資訊詳盡無遺時，我們將刪除此免責聲明。

下表為Adobe Workfront中常用辭彙的清單：

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
   <td>一種使用者設定檔，可決定使用者如何與Workfront內的不同物件和工具互動。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL活動任務]</td> 
   <td>當前項目中的未完成任務，不能被前置任務阻止，並且沒有與未來計畫起始日期一起的任務約束。 換句話說，它可以在今天起作用。</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL活動]</td> 
   <td>在 [!DNL Workfront Goals]，活動是目標的進度指標。 可以是手動更新的進度列，也可以是與目標相關聯的專案。 您無法在報表中顯示活動，也無法透過 [!DNL Workfront] API。 如需活動的相關資訊，請參閱 <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">開始使用Adobe Workfront Target中的結果和活動</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL實際成本]</td> 
   <td> <p>對於任務和問題，這是與實際記錄的小時數相關的成本，與分配給任務或問題的資源的每小時成本比率相關。 對於專案，這是來自專案任務和問題的所有[!UICONTROL實際成本]的總數。 如需詳細資訊，請參閱 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">追蹤成本</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL實際費用成本]</td> 
   <td> <p>為項目或任務記錄的所有費用的[!UICONTROL實際金額]總和。</p> <b>範例 </b>
   <p>如果為任務1建立費用，並在「[!UICONTROL實際金額]」欄位中輸入$600.00，則此任務的「[!UICONTROL實際費用成本]」為$600.00。 </p> 
   <p>對於一個項目， [!DNL Workfront] 使用以下公式計算[!UICONTROL實際費用成本]:</p> <p><code>Project Actual Expense Cost = SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs)</code> <br> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (drafting this because not sure if this is still correct)</p>
    --> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL實際小時數]</td> 
   <td> <p>在專案、任務或問題報表中，[!UICONTROL實際小時數]是記錄在專案、任務或問題上的所有小時數之和。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span> 如果從任務1的[!UICONTROL Updates]頁簽，按一下「Log Time」（日誌時間）並輸入25小時，則任務1的實際小時數= 25小時。 </p> <p>[!DNL Workfront] 使用以下公式計算父任務或項目的[!UICONTROL實際小時數]:</p> 
    <ul> 
     <li> <p><code>For parent tasks = children [!UICONTROL Actual Hours] + [!UICONTROL Actual Hours] on the parent task. </code> </p> </li> 
     <li> <p><code>For projects = [!UICONTROL Actual Hours] logged on the project + [!UICONTROL Actual Hours] logged on standalone or children tasks in the project</code> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL實際人工成本]</td> 
   <td> <p>與在任務或項目中投資的人工相關聯的[!UICONTROL實際成本]。 </p> <p>對於任務， [!DNL Workfront] 使用以下公式計算[!UICONTROL實際人工成本]:</p> <p><code>Task [!UICONTROL Actual Labor Cost] = Number of [!UICONTROL Actual Hours] on the task * User or Job Role [!UICONTROL Hourly Cost Rate]</code> </p> <p>如果任務的[!UICONTROL成本類型]為[!UICONTROL用戶每小時], [!DNL Workfront] 使用使用者率。 如果任務的[!UICONTROL成本類型]為[!UICONTROL角色每小時], [!DNL Workfront] 使用任務職責費率來計算[!UICONTROL實際人工成本]。 </p> <p>對於一個項目， [!DNL Workfront] 使用以下公式計算[!UICONTROL實際人工成本]:</p> <p><code>Project [!UICONTROL Actual Labor Cost] = SUM(All Tasks [!UICONTROL Actual Labor Cost]) </code> </p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">追蹤成本</a>.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span>例如，如果用戶以[!UICONTROL用戶每小時] [!UICONTROL成本類型]記錄某個任務的5小時，並且其每小時費率為$100，則[!UICONTROL實際人工成本]為$500。</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL實際收入] </td> 
   <td> <p>項目或任務的[!UICONTROL實際收入]是與項目或任務的[!UICONTROL實際小時數]關聯的金額。 </p> <p>如需關於在 [!DNL Workfront]，請參閱 <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">帳單和收入概觀</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL實際開始]</td> 
   <td>用戶在工作中更改被分配的正在進行的對象時的時間戳。</td> 
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
   <td>一種方法，其基礎是需求和解決方案與跨職能團隊的協作演化。 它鼓勵根據固定時間表靈活地進行更改。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Agile Team]</td> 
   <td>與傳統團隊不同，因為他們從積壓工作中提取他們的預期工作，並在一段稱為[!UICONTROL迭代]的指定時間內處理它。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL我的所有團隊]</td> 
   <td> <p>在[!UICONTROL篩選器]中引用此項時，此欄位將顯示屬於登錄用戶所屬的任何團隊的用戶，或分配給該登錄用戶所屬的任何團隊的工作項目。 </p> <p>建議您在篩選器中使用此欄位，以便在與其他使用者共用報表時讓報表更為通用。 這樣，您只能建立一個報表，根據登入者檢視該報表，而顯示不同資訊，因為資訊一律會針對登入使用者自訂。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL分配日期]</td> 
   <td> <p>您可以在下列類型的報表中找到此欄位：</p> 
    <ul> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates</li>
     --> 
     <li>[!UICONTROL項目]（財務資料）</li> 
     <li>[!UICONTROL預算小時數]</li> 
    </ul> <p>若<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Resource Estimates or 
      </MadCap:conditionalText>
     -->[!UICONTROL項目（財務資料）]報告： </p> 
    <ul> 
     <li>嘗試了解時建立此報表 <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         how resources are budgeted for work, or 
       </MadCap:conditionalText>
      --> 分配給您的資源的[!UICONTROL計畫小時數]。</li> 
     <li> <p>[!UICONTROL分配日期]是開始分配[!UICONTROL作業角色]至任務的一週的第一天（星期日）。 資源（[!UICONTROL作業角色]）在分配給它的任務的[!UICONTROL持續時間]期間，其[!UICONTROL分配日期]可以與有周相同。 如果任務跨越多個月，則如果任務落在任務的[!UICONTROL持續時間]內，則該月的第一天也可以變成[!UICONTROL分配日期]。</p> <p>例如，您可以將[!UICONTROL作業角色]指派給跨度超過3週且有90個[!UICONTROL計畫小時]的任務。 這些小時在任務期間平均分配，這使每天將6個[!UICONTROL計畫小時數]分配給您的工作角色：</p> <p><em> [!UICONTROL每日計畫小時數] = [!UICONTROL總計計畫小時數]/任務的[!UICONTROL工作日數] </em> </p> <p>因此，有三個[!UICONTROL分配日期]，在任務的[!UICONTROL持續時間]期間，每週的每個星期日各一個，每個日期都與它們關聯一定數量的[!UICONTROL計畫小時數]。<br>如果任務從一個月的最後一週的中間開始，並在新月開始後的兩週結束，則任務將有四個[!UICONTROL分配日期]:在任務的[!UICONTROL持續時間]期間，每週的每個星期日各一個，在新月的第一天各一個。</p> <p>若要充分利用此資訊，建議您建置 <!--
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          Resource Estimates or a 
        </MadCap:conditionalText>
       --> 專案（財務資料）報表，並為[!UICONTROL分配日期]新增矩陣分組，然後將結果分組為每週、每月、每季或每年，以獲得最準確的資料。<br>如需建立矩陣分組的相關資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md" class="MCXref xref">建立矩陣報表</a>.</p> </li> 
    </ul> <p>只有當與財務資訊相關聯的資料少於5年時，財務資訊才會填入[!UICONTROL專案（財務資料）]報表中。 例如，如果在2015年1月將職務角色分配給某個任務，而今天是2021年9月，則職務角色的[!UICONTROL分配日期]之類的財務欄位不會填入[!UICONTROL項目（財務資料）]報表中。 </p> 
    <div> 
     <p>對於[!UICONTROL預算小時]報表：</p> 
     <ul> 
      <li>在嘗試了解分配給資源或資源計畫員中項目的[!UICONTROL預算小時數]金額時，建立此報表。</li> 
      <li> <p>[!UICONTROL分配日期]是您在[!UICONTROL資源規劃器]中預算小時數的一週的第一天（星期日）。 </p> <p>提示：   <p>如果一週跨越兩個月，報表中會產生兩列：一個對應於一週的第一天（第一週的星期日，在第一個月期間），而第二行顯示第二個月的第一天。 </p> <p>例如，若您為某位使用者在6月30日（星期日） — 7月6日（星期六）這一週預算8小時，則兩列會顯示6月30日和7月1日的[!UICONTROL分配日期]。 </p> </p> <p>有關 [!DNL Resource Planner]，請參閱文章 <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">預算資源 [!DNL Resource Planner] 使用[!UICONTROL項目]和[!UICONTROL角色]視圖</a>.</p> <p>如需有關建立[!UICONTROL預算小時]報表的資訊，請參閱 <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">報告：預算小時數</a>. </p> </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL公告]</td> 
   <td> <p>與系統內的用戶資訊通信的方法。 這些資訊通常來自 [!DNL Workfront] 或從管理員到用戶。 </p> <p>如需詳細資訊，請參閱 <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">傳送公告</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL應用程式整合]</td> 
   <td>應用程式最常代表軟體應用程式的連接器，但也可代表處理資料的特殊功能。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL批准者決策]</td> 
   <td> <p>在[!UICONTROL校樣核准]報表中，此欄位會針對已不再使用的校樣顯示校樣核准決策。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL批准者階段]</td> 
   <td>在[!UICONTROL校樣核准報表]中，此欄位會顯示目前階段校樣的相關資訊。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL批准]</td> 
   <td> <p>給定的工作項（如任務、文檔或時間表）可能要求主管或其他用戶簽出該工作項。 此註銷過程稱為批准。 </p> <p>如需詳細資訊，請參閱 <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">核准流程概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL批准日期]</td> 
   <td>在[!UICONTROL校樣核准]報表中，此欄位會顯示校樣的核准日期。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL核准者]</td> 
   <td>必須在指定工作項上簽出的用戶或職務角色，或批准工時單上的工時條目的用戶。</td> 
  </tr> 
  <tr> 
   <td>[!Uicontrol已分配給]</td> 
   <td> <p>在[!UICONTROL任務或問題]報表中，此欄位顯示任務或問題的所有者，或[!UICONTROL主要受託人]。 您也可以依此欄位篩選或分組。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL分配]</td> 
   <td>指派給問題或任務的使用者、工作角色或團隊。 項目、產品組合或項目群不能具有分配。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL分配]</td> 
   <td> <p>在[!UICONTROL任務]或[!UICONTROL問題]報表中，此欄位顯示分配給該任務或問題的所有實體（用戶、作業角色、團隊）的清單。 您可以使用欄位[!UICONTROL分配用戶]和[!UICONTROL分配角色]按此欄位進行篩選。 您可以使用「組」欄位按分配給任務或問題的組進行篩選。 您無法依此欄位將報表分組。</p> <p>放在[!UICONTROL資源回收筒]中的工作項目將繼續顯示在一些引用[!UICONTROL分配]對象的報告中，其中 [!DNL OR] 篩選器修飾詞。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL分配角色]</td> 
   <td>
   <p>在[!UICONTROL任務]或[!UICONTROL問題]報告中，此欄位顯示有關分配給任務或問題的作業角色的資訊。 此欄位顯示[!UICONTROL主要擁有者]，以及指派給任務或問題的其他作業角色。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL分配狀態]</td> 
   <td> <p>在分配、任務或問題報告中，[!UICONTROL分配狀態]顯示分配給工作項的用戶是按一下[!UICONTROL Work On It]按鈕還是按一下[!UICONTROL Done]按鈕接受或完成該工作。 存在以下[!UICONTROL分配狀態]:</p> 
    <ul> 
     <li><b>[！已請求UICONTROL]</b>:已將用戶分配給該任務或問題，但他們尚未按一下[!UICONTROL Work On It]按鈕以開始處理該任務或問題。</li> 
     <li><b>[!UICONTROL工作]</b>:使用者已按一下[!UICONTROL Work On It]按鈕，目前正在處理該項目。 </li> 
     <li><b>[!UICONTROL完成]</b>:使用者已按一下[!UICONTROL Done]按鈕，並已完成對項目的工作。 </li> 
    </ul> <p>如需詳細資訊，請參閱 <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/work-on-it-and-done-buttons-accept-complete-work.md" class="MCXref xref">[!UICONTROL Work It]和[!UICONTROL Done]按鈕概述</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL分配團隊]</td> 
   <td>
   <p>在[!UICONTROL任務]或[!UICONTROL問題]報表中，此欄位顯示有關分配給任務或問題的團隊的資訊。 欄位會顯示[!UICONTROL主要擁有者]，以及指派給工作或問題的其他團隊。 </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL分配用戶]</td> 
   <td>
   <p>在[!UICONTROL任務]或[!UICONTROL問題]報表中，此欄位顯示有關分配給任務或問題的用戶的資訊。 此欄位顯示[!UICONTROL主要擁有者]，以及指派給工作或問題的其他使用者。 </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL屬性]</td> 
   <td>屬性是 [!DNL Workfront] 物件。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL審核區域]</td> 
   <td> <p>稽核是系統訊息，會記錄在Workfront中發生的動作。 記錄了以下審計類型：</p> 
    <ul> 
     <li>[!UICONTROL範圍更改]</li> 
     <li>[!UICONTROL附件操作]</li> 
     <li>[!UICONTROL常規編輯]</li> 
     <li>[!UICONTROL狀態更改]</li> 
     <li>[!UICONTROL注]</li> 
     <li>[!UICONTROL組合條目]</li> 
     <li>[!UICONTROL錯誤條目]</li> 
     <li>[!UICONTROL狀態更改]</li> 
     <li>[!UICONTROL訂閱更改]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL審核跟蹤]</td> 
   <td>由透過「記錄的變更」（[!UICONTROL稽核區域]）追蹤的事件自動產生的附註集合。 每張紙條都記錄了哪些人執行了操作、做了什麼，以及何時執行了操作。</td> 
  </tr> 
  <tr> 
   <td>[!Uicontrol自動更改]</td> 
   <td> <p>[!UICONTROL項目更新]類型之一。 這將在夜間重新計算流程運行時以及對項目內的項目或任務進行任何更新時重新計算項目的預計和計畫時間表。 </p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">選擇項目更新類型 </a>.</p> </td> 
  </tr>

<tr> 
   <td><p>可用性</p></td> 
   <td> <p>此術語用於「用戶可用性」或「資源可用性」，它說明資源（用戶或作業角色）可用於工作的時間量。 </p> 
   <p>Workfront使用數個欄位計算用戶可用性，具體取決於系統中「資源管理」首選項的設定。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">配置資源管理首選項</a>. </p>
   <p>有關資源可用性的詳細資訊，請參見 <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">開始使用資源管理</a></p>
   或者，「容量」也用於指資源可用性。 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL僅自動]</td> 
   <td> <p>[!UICONTROL項目更新]類型之一。 這將在夜間重新計算流程運行時重新計算預計時間軸和計畫時間軸。</p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">選擇項目更新類型</a>.</p> </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL BAU]</td> 
   <td>「一切照常」工作，有助於實現日常的主要業務目標。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL積壓]</td> 
   <td>敏捷環境中的領域，新問題會一直保留到它們準備好處理為止。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL基線]</td> 
   <td>在敏捷環境中測量反覆項目的資料來源。</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL計費記錄]</td> 
   <td> <p>記錄可開單的收入、小時或費用。 此資訊可用於在外部會計系統中建立發票。</p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/projects/project-finances/create-billing-records.md">建立計費記錄</a>. </p> 
   </td> 
  </tr>

<tr> 
   <td>開單記錄狀態</td> 
   <td> <p>在「開單記錄」或「小時」報表中，開單記錄的狀態指示開單記錄是否已開單。 您不能刪除與計費記錄關聯的項目或編輯時間。 如需詳細資訊，請參閱 <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >建立計費記錄</a>.</p>  
   </td> 
  </tr>


<tr> 
   <td>[!UICONTROL品牌推廣]</td> 
   <td>自訂程式 [!DNL Workfront] 使介面具有外觀，通過使用您的顏色和徽標來鏡像您的公司。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL階層連結]</td> 
   <td> <p>頁面頂端的區域，顯示使用者在應用程式中的階層位置。</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">如需詳細資訊，請參閱 <a href="../../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">階層連結概觀</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL預算狀態]</td> 
   <td> <p>此欄位已淘汰。 此欄位可能顯示的任何資訊都與 [!DNL Workfront] 已移除，且無法更新欄位。 </p> <p>此欄位顯示項目是否已添加到[!UICONTROL能力規劃器]中，以及是否已完成其預算計算。 已從 [!DNL Workfront]. </p> 
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
   <td> <p>此欄位已淘汰。 此欄位可能顯示的任何資訊都與 [!DNL Workfront] 已移除。 無法更新此欄位。 </p>
   <p> 此欄位仍顯示在[!UICONTROL專案]和[!UICONTROL任務]報表和清單中。</p>  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL預算成本]</td>

<td> <p>這是與項目預算資源關聯的成本。 </p>
   <p>欄位會顯示在 [!DNL Workfront] 名稱下：</p>
   <ul>
   <li><strong>[!UICONTROL預算成本]</strong>:在[!UICONTROL業務案例摘要]面板中</li>
   <li><strong>[!UICONTROL成本]</strong>:在[!UICONTROL成本]查看資訊時顯示在[!UICONTROL利用率]區域中</li>
   <li><strong>[!UICONTROL項目預算成本]</strong>:在清單和報表中</li>
   </ul>   
    <p>項目的[!UICONTROL預算成本]使用以下公式計算：</p> 
    <p><code>[!UICONTROL Project Budgeted Cost] (or [!UICONTROL Budgeted Cost]) = [!UICONTROL Budgeted Expense Cost] + [!UICONTROL Budgeted Labor Cost] + [!UICONTROL Fixed Cost] of the project</code> </p> 
    <p>有關計算[!UICONTROL預算成本]的詳細資訊，以及了解此概念的各種名稱(在 [!DNL Workfront]，請參閱 <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">計算項目預算成本</a>. </p>
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL預算小時數]</td> 
   <td> <p>為完成項目所需工作的資源編入預算的時數。 此欄位指的是在[!UICONTROL Business Case]（或在[!UICONTROL Resource Planner]）的[!UICONTROL Resource Budgeting]區域中為項目或項目資源預算的小時數。</p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">了解項目的[!UICONTROL預算人工成本]和[!UICONTROL預算工時]</a>. </p> 
    <!-- 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Hours that were formerly budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner)</p>
    <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
  -->
    <p> 有關在 [!DNL Resource Planner]，請參閱文章 <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">預算資源 [!DNL Resource Planner] 使用[!UICONTROL項目]和[!UICONTROL角色]視圖</a>. </p> 
    <p>在[!UICONTROL Business Case]或[!UICONTROL Resource Planner]的[!UICONTROL Resource Budgeting]區域中預算的小時數顯示在以下區域： [!DNL Workfront] 並以下列名稱：</p> 
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
        <td>[!UICONTROL Business Case]的[!UICONTROL資源預算]區</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL BDG]</td> 
        <td>由[!UICONTROL小時數]查看的[!UICONTROL資源規劃器]</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL預算小時數]</td> 
        <td> <p>利用率報告[!UICONTROL小時]視圖</p> <p>如需[!UICONTROL使用率]報表的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md" class="MCXref xref">[!UICONTROL資源利用率]報表概述</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Bud。 時數]</td> 
        <td> <p>[!UICONTROL預算小時]報告</p><p>「預算小時」報告中的[!UICONTROL預算小時]對象引用與已廢止的資源管理工具相關的資訊。 僅"[!UICONTROL Bud. 此報表中的「小時」欄位是指在項目的[!UICONTROL Business Case]的[!UICONTROL Resource Planner]或[!UICONTROL Resource Budgeting]區域中預算的小時數。 </p> <p>如需建立報表的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">建立自訂報表</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL資源計畫員預算小時數] </td> 
        <td> <p>可在下列報表中找到：</p>
        <ul>
        <li>[!UICONTROL專案]報表
        <li>[!UICONTROL項目（財務資料）]報告
        <li>[!UICONTROL任務]報告
        <li>[!UICONTROL問題]報告
        <li>[!UICONTROL預算小時]報告</li>
        </ul>
         <p>如需建立報表的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">建立自訂報表</a>.</p> </td> 
       </tr> 
      </tbody> 
     </table> 
    <p>在 [!DNL Adobe Workfront] 是指使用已從Workfront移除的已棄用功能編入預算的時數。 這些欄位僅供檢視，當您使用目前的資源預算工具時，不會更新為目前的資訊。 </p>
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
   <td>[!UICONTROL預算的人工成本]</td> 
   <td> <p>這是與您作為資源管理器完成項目所需工作的任務職責預算時數關聯的成本。 </p> <p>項目報表中的[!UICONTROL預算人工成本]使用以下公式計算：</p> <p><code style="font-style: normal;">[!UICONTROL Budgeted Labor Cost] = SUM([!UICONTROL Job Role Cost] per [!UICONTROL Hour] * [!UICONTROL Budgeted Hours] per [!UICONTROL Job Role])</code> </p> <p>此欄位可參考下列項目：</p> 
    <ul> 
     <li> <p>顯示在[!UICONTROL Business Case]的[!UICONTROL Resource Budgeting]區域中或與項目上職務成本關聯的[!UICONTROL Resource Planner]中的人工成本。 有關計算[!UICONTROL預算人工成本]的資訊，請參閱文章 <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">項目的[!UICONTROL了解預算人工成本]和[!UICONTROL預算小時數]</a></p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>在[!UICONTROL業務案例]的[!UICONTROL資源預算]區域中顯示的人工成本，反映了與項目連結的計畫中的[!UICONTROL人員成本]估計值，該計畫包含 [!DNL Scenario Planner] 當您使用方案計畫程式來預算項目資源時。 有關計畫的資訊，請參閱 <a href="../../../scenario-planner/initiatives-overview.md" class="MCXref xref">方案計畫器中的方案概覽</a>. </p> <p>此 [!DNL Scenario Planner] 需要額外的授權。 如需 [!DNL Workfront Scenario Planner]，請參閱 <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">此 [!DNL Scenario Planner] 概述</a>. </p> </li> 
     <p>會以下列名稱顯示於的下列區域：</p>
   <ul>
   <li><strong>[!UICONTROL預算的人工成本]</strong>:在[!UICONTROL Business Case]的[!UICONTROL Resource Budgeting]區域中。
   <li><strong>[!UICONTROL預算成本]</strong>:在[!UICONTROL利用率]報表[!UICONTROL成本]視圖中
   <p>如需詳細資訊，請參閱 <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">查看資源利用資訊 </a>.</p>
   <li><strong>[!UICONTROL BDG]</strong>:在 [!DNL Resource Planner] 專案或 [!DNL Role] 視圖，按成本查看時
   <li><strong>[!DNL Resource Planner Budgeted Labor Cost]</strong>:（在以下報告中）: 
   <ul>
    <li>[!UICONTROL專案]報表</li>
    <li>[!UICONTROL項目（財務資料）]報告</li>
    <li>[!UICONTROL任務]報告</li>
    <li>[!UICONTROL問題]報告</li>
    <li>[!UICONTROL預算小時]報告</li> 
    </ul>
    <p>如需建立報表的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">建立自訂報表</a>.</p>
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
  <td> <p>此欄位已淘汰。 此欄位可能顯示的任何資訊都與 [!DNL Workfront] 已移除。 無法更新此欄位。</p>
  <p>這些區域已從 [!DNL Workfront]. </p> 
  <p>此欄位仍顯示在[!UICONTROL專案]和[!UICONTROL任務]報表和清單中。</p>
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
   <td> <p>用於評估項目是否應從[!UICONTROL Idea]狀態轉移到[!UICONTROL Planning]狀態的工具。 換言之，[!UICONTROL業務案例]可協助組織判斷是否值得啟動及完成專案，尤其是在比較專案與產品組合中的其他項目時。</p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">為專案建立[!UICONTROL商業案例] </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL業務案例預算小時數]</td> 
   <td> <p>此欄位已淘汰。 此欄位可能顯示的任何資訊都與 [!DNL Workfront] 已移除。 無法更新此欄位。</p> <p>此欄位仍顯示在專案和[!UICONTROL任務]清單和報表中。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL計算分配]</td> 
   <td> <p>任務[!UICONTROL持續時間]類型之一。 這將根據任務的[!UICONTROL持續時間]和[!UICONTROL所需工作]計算分配給任務的用戶的8小時工作日的百分比。</p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任務[!UICONTROL持續時間]和[!UICONTROL持續時間類型]的概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL計算工作]</td> 
   <td> <p>任務[!UICONTROL持續時間類型]之一。 這將計算任務的[!UICONTROL所需工作]，給定[!UICONTROL持續時間]和用戶[!UICONTROL分配]百分比（以8小時工作日為基礎）。</p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任務[!UICONTROL持續時間]和[!UICONTROL持續時間類型]的概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL日曆]</td> 
   <td> <p>中有兩種日曆 [!DNL Workfront]:[!UICONTROL首頁日曆]和日曆報告。</p> <p>[!UICONTROL首頁日曆]是個人日曆，允許用戶根據其可用小時管理其工作負載 [!DNL Workfront]. 使用者也可以將其[!UICONTROL首頁行事歷]與 [!DNL Outlook] ([!DNL Google] 和 [!DNL Microsoft] 整合即將推出)。 </p> <p>如需[!UICONTROL首頁日曆]的詳細資訊，請參閱 <a href="../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md" class="MCXref xref">[!UICONTROL首頁日曆]視圖</a>.</p> <p>日曆報表是一種動態報表，使用者可在其中檢視事件的日期和其他重要詳細資訊，包括到期日、工作狀態以及指派事件給的使用者。</p> <p> 如需日曆報表的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md" class="MCXref xref">日曆報表概觀</a>.</p> </td> 
  </tr> 
   <tr> 
   <td>[!UICONTROL可以開始]</td> 
   <td> <p>此欄位指示任務是否已準備好開始工作。 如果開始已準備好在任務的[!UICONTROL可以開始]欄位上工作，則此欄位設定為[!UICONTROL True]。 </p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/tasks/task-information/can-start-task-overview.md" class="MCXref xref">任務的「[!UICONTROL Can Start]」概述</a>.</p> 
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
   <td> <p>資源可用的時間，當它們可被分配到工作時。 請參閱「可用性」。 </p></td> 
  </tr>

<tr> 
   <td> <p>[!UICONTROL類別]</p> </td> 
   <td> <p>類別是自訂表單。 您可以建立此物件的報表，也可以在其他物件報表中顯示。 並非所有對象都可以有自定義表單或類別。 下列物件可以有自訂表單： <br></p> 
    <ul> 
     <li>[!UICONTROL項目]</li> 
     <li>[!UICONTROL任務]</li> 
     <li>[!UICONTROL問題]</li> 
     <li>[!UICONTROLPortfolio]</li> 
     <li>[!UICONTROL文檔]</li> 
     <li>[!UICONTROL費用]</li> 
     <li>[!UICONTROL程式]</li> 
     <li>[!UICONTROL用戶]</li> 
     <li>[!UICONTROL公司]</li> 
     <li>[!UICONTROL迭代]</li></ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL類別名稱]</td> 
   <td> <p>將作為列添加到以下任何對象的視圖中時，它將顯示與這些對象關聯的所有自定義表單的清單：</p> 
    <ul> 
     <li>[!UICONTROL項目]</li> 
     <li>[!UICONTROL任務]<br></li> 
     <li>[!UICONTROL問題]<br></li> 
     <li>[!UICONTROLPortfolio]<br></li> 
     <li>[!UICONTROL文檔]<br></li> 
     <li>[!UICONTROL費用]<br></li> 
     <li>[!UICONTROL程式]<br></li> 
     <li>[!UICONTROL用戶]<br></li> 
     <li>[!UICONTROL公司]</li> 
     <li>[!UICONTROL迭代]</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL更改管理]</td> 
   <td>一個實踐領域，重點是定義、理解和調整計畫內工作以適應範圍、時間表、成本和資源因素的變化。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL更改順序]</td> 
   <td>針對項目提出的一種問題，概述對商定範圍所要求的更改。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL僅更改]</td> 
   <td>其中一個項目[!UICONTROL更新類型]。 它只會在對任務進行更新或在項目或任務上執行編輯時更新[!UICONTROL Project Projected]和[!UICONTROL Planeded]時間表。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL更改順序]</td> 
   <td> <p>[!UICONTROL問題]類型之一，通常表示在項目完成之前必須完成計畫外的工作量。</p> <p>如需[!UICONTROL問題]類型的詳細資訊，請參閱文章中的「預設問題類型」一節 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md" class="MCXref xref">自訂預設問題類型</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL子任務]</td> 
   <td>是[!UICONTROL父任務]（[!UICONTROL摘要任務]）的[!UICONTROL子任務]的任務。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL子項]</td> 
   <td>[!UICONTROL子任務]到[!UICONTROL父任務]（[!UICONTROL摘要任務]）的集合。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL指導]和[!UICONTROL培訓]</td> 
   <td>學習模組、認證、標準或實踐社群。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL提交]</td> 
   <td>一種通信工具，用於用戶對任務交付件設定期望。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL提交日期]</td> 
   <td>一種通信工具，用於為任務交付項設定期望值。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Communication]和[!UICONTROL Reporting]</td> 
   <td>用於審核項目、項目群或產品組合的例外和運行狀況的標準</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL公司]</td> 
   <td> <p>[!UICONTROL公司]是 [!DNL Workfront]. </p> 
   <p> 您可以將使用者或專案與一個公司建立關聯。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md">建立和編輯公司</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL完成日期]</td> 
   <td> <p>項目、任務或問題的設定完成日期。 中有數種類型的[!UICONTROL完成日期] [!DNL Workfront]:</p> 
    <ul> 
     <li>[!UICONTROL實際完成日期]。 如需詳細資訊，請參閱 <a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">項目[!UICONTROL實際完成日期]概覽 </a>.</li> 
     <li>[!UICONTROL計畫完成日期]。 如需詳細資訊，請參閱 <a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">設定項目[!UICONTROL計畫完成日期]</a> 和 <a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">任務[!UICONTROL計畫完成日期]概覽</a>.</li> 
     <li>[!UICONTROL預計完成日期]。 如需詳細資訊，請參閱 <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">項目、任務和問題的[!UICONTROL預計完成日期]概覽</a>.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL完成日]</td> 
   <td>相對於[!UICONTROL模板]的開頭，[!UICONTROL模板任務]或[!UICONTROL模板]應該完成的日子。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL完成模式]</td> 
   <td> <p>這表示專案將如何標示為[!UICONTROL完成]。 它可以有兩個值：</p> 
    <ul> 
     <li>[!UICONTROL手冊]:使用者必須將專案狀態變更為[!UICONTROL完成]。</li> 
     <li>[!UICONTROL自動]:當項目中的所有任務100%完成且所有問題都已結束時，項目狀態將自動更改為[!UICONTROL Complete]。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL條件]</td> 
   <td> <p>這是任務、問題或專案進度的視覺表示。</p> <p>對於專案，條件可由專案擁有者手動設定，或由 [!DNL Workfront]，根據專案的進度狀態。 </p> <p>專案條件的可能值為：</p> 
    <ul> 
     <li>目標上的[!UICONTROL]</li> 
     <li>[!UICONTROL面臨風險]</li> 
     <li>[!UICONTROL遇到問題]</li> 
    </ul> <p>如需專案條件的詳細資訊，請參閱文章 <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">[!UICONTROL項目條件]和[!UICONTROL條件類型]的概述</a>.</p>
     <p>您可以將任務和問題條件與可顯示在報表中的數字相關聯。 以下清單顯示任務和問題條件的預設名稱和編號。 您的系統管理員可以更新條件的名稱，而且他們可以以不同的數字新增條件。 數字與條件關聯後，便無法編輯。  </p> 
     <p>對於任務，條件由任務所有者手動設定。 任務條件的可能值為：</p> 
    <ul> 
     <li>[!UICONTROL順利進行](0)<br></li> 
     <li> [!UICONTROL某些顧慮](1)<br></li> 
     <li>[!UICONTROL主要路障](2)</li> 
    </ul> <p>如需工作條件的詳細資訊，請參閱文章 <a href="../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">更新[!UICONTROL條件]以了解任務和問題</a>.</p> <p>對於問題，條件是由問題擁有者手動設定。 問題條件的可能值為：<br></p> 
    <ul> 
     <li>[!UICONTROL順利進行](0)<br></li> 
     <li>[!UICONTROL某些顧慮](1)<br></li> 
     <li>[!UICONTROL主要路障](2)</li> 
    </ul> 
   <p><b>附註</b></p>
    <p>在[!UICONTROL日誌條目]報表中跟蹤[!UICONTROL條件]欄位時，[!UICONTROL新]和[!UICONTROL舊編號值]將顯示與條件相關聯的編號，而不是其名稱。 如果最初沒有為任務或問題定義條件，而您稍後更新了該條件，則捕獲更新的日記帳分錄將將[!UICONTROL條件]欄位的[!UICONTROL舊編號值]顯示為–2,147,483,648。 另請參閱本文中的「[!UICONTROL新編號值]」、「[!UICONTROL舊編號值]」和「[!UICONTROL日記帳分錄]」。 </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL條件更新]</td> 
   <td> <p>此欄位顯示任務、項目或問題的當前狀態。 此選項顯示[!UICONTROL更新狀態]欄位中任務、項目或問題的所有者提供的最新更新，以及新條件。</p> <p>在條件更新時所做的註解不會顯示在[!UICONTROL條件更新]欄中；僅顯示主要更新。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL約束日期]</td> 
   <td> <p>如果您使用與特定日期（如[!UICONTROL必須從開始]）綁定的[!UICONTROL任務約束]，則該特定日期將成為任務的[!UICONTROL約束日期]。</p> <p>以下任務約束更新了[!UICONTROL約束日期]欄位：</p> 
    <ul> 
     <li>[!UICONTROL必須開始]</li> 
     <li>[!UICONTROL必須在完成]</li> 
     <li>[!UICONTROL不晚於]</li> 
     <li>[!UICONTROL開始時間早於]</li> 
    </ul> <p>提示：   
     <ul> 
      <li> <p>具有[!UICONTROL固定日期]的[!UICONTROL約束]的任務沒有[!UICONTROL約束日期]。 </p> </li> 
      <li> <p> [!UICONTROL約束日期]只能在報表或自定義視圖中查看。</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL約束日]</td> 
   <td> <p>如果在與特定日（如「必須開始」）綁定的模板任務中使用「任務約束」，則該特定日將成為模板任務的「約束日」。</p> <p>以下任務約束更新了[!UICONTROL約束日]欄位：</p> 
    <ul> 
     <li>[!UICONTROL必須開始]</li> 
     <li>[!UICONTROL必須在完成]</li> 
     <li>[!UICONTROL不晚於]</li> 
     <li>[!UICONTROL開始時間早於]</li> 
    </ul> <p>提示：[!UICONTROL約束日]只能在報告或自定義視圖中查看。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL約束類型]</td> 
   <td> <p>任務的計畫趨勢。 例如，[!UICONTROL Soo Phose Op Possible]將安排一個任務盡快開始，而[!UICONTROL Finish No Than]將安排一個任務以在[!UICONTROL Constraint Date]之前完成，而不是以後完成。</p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">[!UICONTROL任務約束]概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL上下文菜單]</td> 
   <td>位於畫面左側的功能表，項目會在其上變更，以與作用中內容產生關聯。 例如，當使用者檢視專案時，[!UICONTROL內容功能表]會顯示與專案相關的資訊和工具的連結。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL轉換的問題創作者]</td> 
   <td>項目或任務報表中的欄位，顯示當問題轉換為項目或任務時，作為問題[!UICONTROL主要聯繫人]的用戶的相關資訊。 欄位也會顯示在[!UICONTROL專案詳細資料]區段中，其中顯示轉換問題的[!UICONTROL主要連絡人]的名稱。 另請參閱本文中的「[!UICONTROL主要連絡人]」。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL成本]</td> 
   <td> <p>完成項目、任務或問題時必須花費的金額。 </p> <p>您可以跟蹤與項目相關的各種成本類型。有關跟蹤成本的資訊，請參閱 [!DNL Workfront] 請參閱 <a href="../../../manage-work/projects/project-finances/track-costs.md">追蹤成本</a>.</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL成本類型]</td> 
   <td>對於任務，[!UICONTROL成本類型]確定任務如何應計成本。 有些範例包括[!UICONTROL固定每小時]、[!UICONTROL使用者每小時]和[!UICONTROL使用者每小時加固定]。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL跨項目依賴項]</td> 
   <td> <p>一個項目的任務取決於來自不同項目的任務。</p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref">建立跨專案的前置項目</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL自訂資料]</td> 
   <td> <p>組織專屬的資料。 組織可以自訂 [!DNL Workfront] 建立自訂表單和自訂欄位以應用程式。 此自訂資訊可促進KPI、稽核和需求組合的報告。 </p> <p>[!UICONTROL自訂資料]可連結至：</p> 
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
   <td>[!UICONTROL自訂資料類型]</td> 
   <td>用於指定[!UICONTROL自定義資料]欄位是否以文本、日期、數字或貨幣形式儲存在資料庫中的選項。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL自定義顯示類型]</td> 
   <td>自訂欄位的欄位顯示類型。 例如： [!UICONTROL下拉式清單]、[!UICONTROL文本欄位]、[!UICONTROL文本區域]、[!UICONTROL單選按鈕]等。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL自定義欄位]</td> 
   <td>對於允許使用者從數個選項中選取的自訂資料，這些是使用者可以選取的值。 自訂選項僅對[!UICONTROL下拉式清單]、[!UICONTROL多選下拉式清單]、[!UICONTROL選項按鈕]和[!UICONTROL複選框]有效。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL自定義表單標籤]</td> 
   <td>使用具有自訂選項的自訂顯示類型時，這是將顯示在下拉式選單、核取方塊或該自訂選項的選項按鈕中的使用者介面文字。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL自定義值]</td> 
   <td>使用「自定義」欄位和「自定義選項」時，這是將儲存在特定選項的資料庫中的值。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL自定義視圖]</td> 
   <td>針對清單中每個對象顯示的資料欄位或列的定義。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL客戶]</td> 
   <td>使用Workfront例項的組織。</td> 
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
   <td>[!UICONTROL控制面板]</td> 
   <td> <p> 您可以在報表或報表物件清單中新增此欄位，以顯示清單中列出報表的控制面板。 </p> <p> 您也可以使用此欄位來篩選列在特定控制面板上的報表。 </p> <p> 如需關於在報表物件報表上納入控制面板資訊的詳細資訊，請參閱文章中的「了解控制面板上列出的報表」一節 <a href="../../../reports-and-dashboards/reports/report-usage/access-organize-reports.md" class="MCXref xref">存取及組織報表</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資料類型]</td> 
   <td>請參閱「[!UICONTROL自訂資料類型]」。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL延遲天數]</td> 
   <td> <p>如果缺少[!UICONTROL實際完成日期]，此欄位將顯示[!UICONTROL計劃開始]和[!UICONTROL今天]之間的日期差異。</p> <p>還顯示[!UICONTROL實際完成]和[!UICONTROL計畫完成]之間的日期差，當存在[!UICONTROL實際完成日期]時。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL預設計畫]</td> 
   <td> <p>可自訂預設工作時間，以指派給組織內的使用者和專案。 </p> <p>計畫用於計算分配給用戶的任務的計畫日期、開始日期和完成日期。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL交付件]</td> 
   <td>在項目完成時必須提供的可量化貨物或服務。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Demand Management]</td> 
   <td>對進氣過程進行評分和確定優先順序。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL部門目標]</td> 
   <td>特定部門特有的目標，該部門專注於改進部門內的操作指標。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL依賴項]</td> 
   <td>需要一個任務在另一個任務之前更改狀態的兩個任務之間的連結也可以更改狀態。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL依賴項類型]</td> 
   <td> <p>任務與其前身之間的調度關係的類型。 一個示例是[!UICONTROL Finish-Start]，它要求第一個任務必須「完成」，然後第二個任務才能「啟動」。</p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md" class="MCXref xref">任務相關性類型概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文檔]</td> 
   <td>附加到內對象的任何檔案 [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文檔版本]</td> 
   <td> <p>每次將同一文檔上載到同一對象時，都會為其分配版本號。 用戶可以查看和更改文檔的以前版本的多個選項。</p> <p>如需詳細資訊，請參閱 <a href="../../../documents/managing-documents/manage-document-versions.md" class="MCXref xref">管理文檔版本</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL持續時間]</td> 
   <td> <p>為完成任務問題或項目分配的時間窗口（由[!UICONTROL計劃開始]和計畫完成之間的天數確定）。</p> 
    <ul> 
     <li>對於任務，如果任務的「持續時間類型」不是「簡單」，則「持續時間」是可編輯的欄位。 如果任務的「持續時間類型」為「簡單」，或者「任務約束」為「固定日期」，則「持續時間」是由Workfront執行的計算。</li> 
     <li>對於問題，「持續時間」一律是可編輯的欄位，它應代表需要解決問題的預估天數。</li> 
     <li>對於專案，持續時間是由 [!DNL Workfront] 它表示最早任務的「計劃開始」與項目上最新任務的[!UICONTROL計畫完成]之間的天數差異。</li> 
    </ul> <p>有關任務的[!UICONTROL持續時間]和[!UICONTROL計畫持續時間]之間差異的詳細資訊，請參閱文章 <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md">任務的[!UICONTROL計畫持續時間]和[!UICONTROL持續時間]之間的差異</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL持續時間（以分鐘為單位）]</td> 
   <td>此欄位以分鐘為單位顯示與[!UICONTROL持續時間]欄位相同的資訊，而非天。 </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc,QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL每次發生的持續時間]</td> 
   <td> <p>這將顯示在循環任務父項的[!UICONTROL任務詳細資訊]和[!UICONTROL編輯任務]框中。 它顯示每個循環任務的持續時間。 有關建立循環任務的資訊，請參閱 <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">建立循環任務</a>. </p> <p> <span>在個別循環任務中修改的持續時間不會顯示此欄位中指出的值。</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL持續時間類型]</td> 
   <td> <p>一個任務欄位，指明完成任務所需的工作如何在任務期間分配給受分配者。 它表示任務的[!UICONTROL持續時間]、[!UICONTROL所需工作]與時間量（或[!UICONTROL分配]）之間的關係，分配的資源應花費在任務上以完成它。 </p> <p>此欄位將顯示在任務的[!UICONTROL詳細資訊]頁簽上。 </p> <p>選項為：</p> 
    <ul> 
     <li>[!UICONTROL計算分配]</li> 
     <li>[!UICONTROL計算工作]</li> 
     <li>[!UICONTROL工作驅動]</li> 
     <li>[!UICONTROL簡單]</li> 
    </ul> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任務[!UICONTROL持續時間]和[!UICONTROL持續時間類型]的概述</a>.</p> 
    —&gt; </td> 
   </tr> 
   <tr> 
   <td>[!UICONTROL持續時間單位]</td> 
   <td>用於測量電源搜索中時間的單位。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作驅動]</td> 
   <td>用戶數與任務完成所需時間之間的關係。 隨著添加更多用戶，任務完成的計畫總時間會減少，但任務的持續時間保持不變。 例如，如果一項任務在炮擊一桶花生，增加更多人將減少計畫的時間，但人日的持續時間將保持不變。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL已用時間]</td> 
   <td> <p>[!UICONTROL Elapped time]是任務的[!UICONTROL Duration]的時間單位。 這是任務的[!UICONTROL計畫起始日期]和[!UICONTROL計畫完成日期]之間的時間，該任務包括節假日、週末和休息時間。 換句話說，經過的時間是日曆天數的過去。 </p> <p>[!DNL Workfront] 支援任務持續時間的以下已用時間單位：</p> 
    <ul> 
     <li> <p>[!UICONTROL已用分鐘數]</p> </li> 
     <li> <p>[!UICONTROL已用小時數]</p> </li> 
     <li> <p>[!UICONTROL已用天數]</p> </li> 
     <li> <p>[!UICONTROL已用周數]</p> </li> 
     <li> <p>[!UICONTROL已用月數]</p> </li> 
    </ul> <p>有關任務持續時間（包括已用時間）的詳細資訊，請參見 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任務[!UICONTROL持續時間]和[!UICONTROL持續時間類型]的概述</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL結束日期]</td> 
   <td> <p> 在[!UICONTROL比率]報表中，這是項目層職務角色的新計費比率結束的日期。 在此日期之前與項目關聯的小時數乘以此開單比率，以計算項目收入。 </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL參與]</td> 
   <td>指出任務、項目、團隊或組織的承諾和信念何時減弱的[!UICONTROL工作績效指標](WPI)。 這表明你需要採取行動來恢復這種信念和承諾。 WPI會通過問一些簡單的問題來衡量， 「你明白你的期望嗎？ 您指派的工作對組織有影響嗎？ 你做得很棒嗎？」</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL企業目標]</td> 
   <td>貢獻公司目標量度的跨功能目標。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL事件]</td> 
   <td>項目或任務中的任何更改。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL事件處理程式]</td> 
   <td>發生事件時發生的自動化任務。 自動電子郵件通知是常見的範例。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL事件通知]</td> 
   <td>從事件處理常式產生的電子郵件。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL費用]</td> 
   <td>任務或項目的非人工成本。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL外部]</td> 
   <td> <p>通常是許可證類型，或具有此類許可證的用戶，它只能查看系統中的資訊。</p> <p>如需詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] 授權概述</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL外部系統]</td> 
   <td>儲存和管理在指定記錄系統之外的任何服務或軟體。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL篩選器]</td> 
   <td> <p>定義螢幕上顯示之資訊之報表或清單元素的其中一個主要組成要素。 如需報表元素的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">報表元素：篩選器、檢視和群組</a>.</p> <p>篩選器會決定報表或 [!DNL Workfront] 面板清單，例如專案、工作或問題。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Financial Work Management]</td> 
   <td>管理人工成本、費用和收入資料的流程 [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL固定成本]</td> 
   <td>您可以定義項目的固定成本金額。 這是項目的[!UICONTROL計畫成本]的一部分，它表示完成項目所需的資金額。 有關成本的資訊，請參閱 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">追蹤成本</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL固定收入]</td> 
   <td>您可以定義專案的固定收入金額。 這是專案的[!UICONTROL計畫收入]的一部分，代表完成專案後您可能獲得的金額。 如需收入的相關資訊，請參閱 <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">帳單和收入概觀</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL標誌]</td> 
   <td> <p> 此欄位與[!UICONTROL狀態表徵圖]相同，但僅適用於以下視圖： </p> 
    <ul> 
     <li> [!UICONTROL模板] </li> 
     <li> [!UICONTROL費用] </li> 
    </ul> <p> 如需詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">檢視中的內建狀態圖示</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資料夾]</td> 
   <td>資料夾用於組織與對象關聯的文檔或報告。</td> </tr>
  <tr>
  <td>[!UICONTROL FTE]（等於全職）</td> 
   <td>這是「全時等價物」，它指示資源可用於工作的時間量。 
   [!UICONTROL FTE]欄位將顯示在以下區域： 
  <ul>
   <li> 編輯或建立使用者時的使用者設定檔 </li>
   <li> [!UICONTROL資源規劃器] </li>
   <li> [!UICONTROL方案規劃器](需要Workfront方案規劃器的附加許可) </li>
   <li> 使用者清單和報表 </li> </ul>

<p>[!UICONTROL FTE]必須是十進位數，最多1，不能是0。 </p>
   <p> 1的[!UICONTROL FTE]（如其配置檔案中所定義，是用戶的[!UICONTROL FTE]欄位的預設值）表示資源（用戶或角色）根據計算可用性的計畫工作整個小時數。 </p>
   <p>您的Workfront管理員會決定要使用哪個排程來判斷使用者的可用性。  </p>
   <ul>
   <li> 使用[!UICONTROL預設計畫]時，Workfront會使用在其設定檔中找到之使用者的[!UICONTROL FTE]來計算可用性。 </li>
   <li> 使用使用者排程時，Workfront會使用使用者的休息時間， <span class="preview">[!UICONTROL工作時間]值</span>，和[!UICONTROL預設計畫]的小時數來計算用戶的[!UICONTROL FTE]。 </li> </ul>

<p>如需詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">配置資源管理首選項</a>.  </p>
   <p>如需在 [!DNL Workfront]，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">建立排程</a>. </p>

<p><b>附註</b></p>
   <p>對於[!UICONTROL方案規劃器]中的所有計算，Workfront使用以下值：1 [!UICONTROL FTE] = 8小時。</p>
   <p>如需詳細資訊，請參閱 <a href="../../../scenario-planner/get-started-with-scenario-planning.md">開始使用[!UICONTROL方案規劃器]</a>. </p>
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
   <td> <p>根據當前計畫項目任務時的計畫日期或預計日期，在日曆視圖中顯示項目日期的可視時間表。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL目標]</td> 
   <td><p>中有兩個目標概念 [!DNL Workfront]: </p> 
    <ul> 
     <li> <p><b>專案目標</b>:由項目相關利益相關方同意的一組業務目標。 專案目標是專案商業案例的一部分。 </p> <p>您無法在清單或報表中顯示專案目標，但可透過API存取。 </p> <p>有關業務案例項目目標的資訊，請參閱 <a href="../../../manage-work/projects/define-a-business-case/create-business-case-goals.md">建立業務案例目標 </a>. </p> </li> 
     <li> <p><b>戰略目標</b>:策略目標是您建立的目標，用於為特定時段規劃工作策略。 您可以使用 [!DNL Workfront Goals]. 您的組織必須購買額外的授權，且您必須擁有此功能的存取權，才能建立策略目標。 [!DNL Workfront Goals] 只能使用額外的授權。</p> 
     <p>如需詳細資訊，請參閱 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] 概述 </a>. </p> 
     <p>您可以在目標或專案報表中顯示策略目標，並透過API存取。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL目標層次結構]</td> 
   <td> <p>在[!UICONTROL目標]和[!UICONTROL項目]報表中，此集合欄位顯示策略目標與其他目標一致時，在層次結構中所屬的目標。 目標以▸分隔字元分隔。 </p> <p>此欄位中只會顯示目標和目標的父項。 子項目標不會顯示。 </p> <p>如需在 [!DNL Workfront Goals]，請參閱 <a href="../../../workfront-goals/goal-alignment/goal-alignment-overview.md">目標對齊概觀 [!DNL Workfront Goals]</a>. </p> 
   <p>只有在貴組織已購買時，此欄位才會顯示 [!DNL Workfront Goals]. 如需使用管理策略目標的相關資訊 [!DNL Workfront Goals]，請參閱 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] 概述 </a>. </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL目標成功分數]</td> 
   <td> 在[!UICONTROL專案報表]中，此欄位用來指與[!UICONTROL商業]案例相關聯的專案層級目標。 目前，此欄位已淘汰，且未與任何功能建立關聯。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL目標] </td> 
   <td> <p>在[!UICONTROL專案]報表中，此為收集欄位，可顯示與專案相關聯的所有策略目標。 目標以逗號分隔。</p> <p>只有在貴組織已購買時，此欄位才會顯示 [!DNL Workfront Goals]. 如需使用管理策略目標的相關資訊 [!DNL Workfront Goals]，請參閱 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] 概述</a>. 如需有關 [!DNL Workfront]，請參閱本文中的「[!UICONTROL目標]」。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL全局介面首選項]</td> 
   <td>影響所有用戶的介面設定。 [!UICONTROL全局介面首選項]可被[!UICONTROL用戶介面首選項]覆蓋。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL組]</td> 
   <td> <p>具有相同對象訪問權限的用戶（可能來自同一部門或業務單位）的集合。 除了使用者外，群組也可與產品組合、方案、專案、<span> 專案範本，</span> 公司、團隊、排程、佈局模板和時間表配置檔案。</p> <p>您也可以按群組授予物件的權限。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">群組概觀</a>.</p> <p>在以下類型之一的對象清單或報告中，可以使用[!UICONTROL組]欄位列出與特定組關聯的該類型的對象：用戶，產品組合，方案，項目， <span>專案範本</span>、公司、團隊、排程、配置模板或時間表配置檔案。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL組管理員]</td> 
   <td> <p>管理指定用戶組的對象、訪問權和用戶的用戶。</p> <p> 在[!UICONTROL組]報表中，此欄位顯示組中指定為[!UICONTROL組管理員]的用戶的名稱。 如需群組管理員的詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">群組管理員</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！具有管理訪問權限的UICONTROL組]</td> 
   <td> <p> 在[!UICONTROL佈局模板]、[!UICONTROL時間表配置檔案]或[!UICONTROL時間表報告]中，此欄位顯示組管理員有權修改模板的組。 您也可以依此欄位篩選此報表。 </p> <p> 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">建立和管理版面範本</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL分組]</td> 
   <td> <p>一種報告元素，用於根據通用標準對清單中的資訊進行分類。</p> <p>如需詳細資訊，請參閱文章中的「[!UICONTROL群組]」一節 <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">報表元素：篩選器、檢視和群組</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL切換日期]</td> 
   <td> <p>任務可用於工作的日期。 [!UICONTROL切換日期]是計算，無法手動設定。 <br>如需[!UICONTROL切換日期]的詳細資訊，請參閱文章 <a href="../../../manage-work/tasks/task-information/handoff-task-date.md" class="MCXref xref">[!UICONTROL任務切換日期]概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL服務台]</td> 
   <td>部分 [!DNL Workfront] 它包含所有問題隊列。 [!UICONTROL Help Desk]可用於處理客戶支援票證、項目請求、幫助台票證等。 這與[!UICONTROL請求]區域相同。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL所有者]</td> 
   <td>在[!UICONTROL小時]報表中，將小時歸因於[!UICONTROL所有者]的用戶。 這與實際記錄時間的使用者不同。 這兩個實體有時可能是兩個不同的使用者。 <br>如需其他使用者記錄時間的詳細資訊，請參閱文章 <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">記錄時間</a>.</td> 
  </tr>

<tr> 
   <td>小時狀態</td> 
   <td> <p>由Workfront針對使用者記錄任務、問題或專案的實際小時數所設定的屬性。 </p>

在Workfront中，小時項目可能具有下列其中一種狀態：
<ul>
   <li><b>已提交</b>:已記錄項目、任務或問題的小時數。 它們是計費記錄的一部分，或尚未添加到計費記錄中。</li>
   <li><b>已核准</b>:這些小時已記錄，並且已獲得項目所有者的批准。 它們是計費記錄的一部分，或尚未添加到計費記錄中。</li> 
   <li><b>未批准</b>:該小時已被項目所有者記錄並拒絕。 它們是計費記錄的一部分，或尚未添加到計費記錄中。</li>
   <li><b>已計費</b>:已記錄小時，並將其添加到計費記錄中，並且計費記錄狀態已標籤為「已計費」。 它們不需要獲得項目所有者的批准。</li>
   <li><b>計費和批准</b>:小時已記錄，已經由項目所有者批准，並且計費記錄狀態已標籤為「已開單」。</li>
   </ul>


<p>當小時數是計費記錄的一部分時，「小時狀態」指示小時數是否已獲得批准，或其所屬的計費記錄是否已開單。 小時條目的「小時狀態」僅顯示在小時清單或報告中。 </p>

<p>有關向計費記錄添加小時的詳細資訊，請參閱文章中的「向計費記錄添加小時」部分 <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >建立計費記錄</a>.</p>

<p>如需核准專案時間的詳細資訊，請參閱 <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" >需要為項目批准的時間</a>.</p>

<p><b>筆尖</b></p>

<p>未直接記錄在工作項目上的一般小時數不會顯示「小時」狀態。 </p> </td> 
  </tr>



<tr> 
   <td>[!UICONTROL小時類型]</td> 
   <td> <p>可針對使用者記錄任務、問題或專案的實際小時數設定的屬性。 這也是未直接連結至工作的記錄小時數的屬性，例如[!UICONTROL Vacation]和[!UICONTROL Time Off]。</p> <p>如需詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md" class="MCXref xref">管理小時類型</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>ID是與中每個物件相關聯的英數字元指標 [!DNL Workfront]. 它會唯一識別 [!DNL Workfront] 資料庫。 您可以檢視報表中任何物件的ID，或檢視每個物件的清單。 </p> <p>提示：   <p>您也可以在物件頁面的URL中檢視ID。 例如，當您存取[!UICONTROL專案詳細資料]頁面時，專案的ID可能看起來像下列URL中概述的數字：</p> <p><code>https://&lt;your domain>.my.workfront.com/project/<b>5e29c8010027d8eb334762d4fff3ffca</b>/overview</code> </p> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL個別目標]</td> 
   <td>貢獻團隊目標量度，但與個人或職業發展無關的個別目標。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL繼承的訪問]</td> 
   <td>允許訪問從對象傳播到另一個對象的共用功能。 例如，項目用戶在方案和產品組合記錄中定義的繼承訪問權限。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL計畫]</td> 
   <td> <p>在 [!DNL Workfront Scenario Planner]，您可以將計畫劃分為幾個計畫，以便更輕鬆地管理計畫。 <span>您可以建置[!UICONTROL計畫]報表，並且可以在[!UICONTROL項目]報表中訪問[!UICONTROL計畫]資訊。</span></p> <p>此 [!DNL Scenario Planner] 需要額外的授權。 如需 [!DNL Workfront Scenario Planner]，請參閱 <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">此 [!DNL Scenario Planner] 概述</a>. </p> <p>此 [!DNL Initiative] 報表不會顯示在您的 [!DNL Workfront] 例項，除非您的公司已購買 [!DNL Workfront Scenario Planner] 授權。 您無法透過API存取[!UICONTROL方案]。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL計畫作業角色]</span> </td> 
   <td> <p><span>[!UICONTROL方案作業角色]報表類型顯示與計畫方案關聯的作業角色的相關資訊，位於 [!DNL Workfront Scenario Planner].</span> </p> <p>此 [!DNL Scenario Planner] 需要額外的授權。 如需 [!DNL Workfront Scenario Planner]，請參閱 <a href="../../../scenario-planner/scenario-planner-overview.md">此 [!DNL Scenario Planner] 概述</a>. </p> <p><span>此報表類型不會顯示在 [!DNL Workfront] 例項，除非您的公司已購買 [!DNL Workfront Scenario Planner] 授權。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL計畫作業角色小時數]</span> </td> 
   <td> <p><span> 在[!UICONTROL計畫作業角色]報表中，它顯示與計畫中的作業角色相關聯的小時數。</span> </p> <p>此 [!DNL Scenario Planner] 需要額外的授權。 如需 [!DNL Workfront Scenario Planner]，請參閱 <a href="../../../scenario-planner/scenario-planner-overview.md">此 [!DNL Scenario Planner] 概述</a>. </p> <p>您的 [!DNL Workfront] 例項，除非您的公司已購買 [!DNL Workfront Scenario Planner] 授權。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL計畫作業角色計數]</td> 
   <td> <p>在[!UICONTROL計畫作業角色]報表中，它顯示與計畫關聯的特定作業角色的數量。</p> <p>此 [!DNL Scenario Planner] 需要額外的授權。 如需 [!DNL Workfront Scenario Planner]，請參閱 <a href="../../../scenario-planner/scenario-planner-overview.md">此 [!DNL Scenario Planner] 概述</a>. </p> <p>您的 [!DNL Workfront] 例項，除非您的公司已購買 [!DNL Workfront Scenario Planner] 授權。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL計畫上次發佈日期]</td> 
   <td> <p>[!UICONTROL計畫]、[!UICONTROL計畫作業角色]和[!UICONTROL項目]報表中的欄位，顯示計畫計畫上次發佈到項目的日期。 您可以發佈活動以建立項目或更新連結到活動的項目。</p> <p>此 [!DNL Scenario Planner] 需要額外的授權。 如需 [!DNL Workfront Scenario Planner]，請參閱 <a href="../../../scenario-planner/scenario-planner-overview.md">此 [!DNL Scenario Planner] 概述</a>. </p> <p><span>如需發佈活動的相關資訊，請參閱</span><a href="../../../scenario-planner/publish-scenarios-update-projects.md">發佈藍本以在中建立和更新專案 [!DNL Workfront Scenario Planner]</a>. 您的 [!DNL Workfront] 例項，除非您的公司已購買 [!DNL Workfront Scenario Planner] 授權。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL內聯搜索]</td> 
   <td>在填寫表單過程中執行的搜索，以查找特定欄位的可能條目。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL介面設定]</td> 
   <td>允許定義自訂檢視、篩選器、群組、清單控制項等的應用程式區域。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL是公司目標]</p></td> 
   <td> <p>在 [!DNL goal reports]，則會為每個策略目標顯示「[!UICONTROL True]/ [!UICONTROL False]」值，以指示是否將您的組織指派給目標作為其擁有者。 </p> 
   <p>只有在貴組織已購買時，此欄位才會顯示 [!DNL Workfront Goals]. 如需使用管理策略目標的相關資訊 [!DNL Workfront Goals]，請參閱 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] 概述 </a>.</p>
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL問題]</td> 
   <td> <p>計畫外工作項，通常表示有問題阻止完成任務或項目。 它被分類和評估，以供進一步的工作考慮</p> <p>[!UICONTROL問題]也可以是[!UICONTROL幫助台]請求。 [!UICONTROL更改順序]、[!UICONTROL請求]和[!UICONTROL錯誤]也是[!UICONTROL問題]。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL問題管理]</td> 
   <td> <p>管理問題類型定義的流程和規則，以及與每種類型關聯的路由、分類或流量流程。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL問題所有者]</td> 
   <td>負責分類及完成問題的團隊或使用者。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL迭代]</td> 
   <td>一個團隊生成預定義的一組交付件的時間段。</td> 
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
   <td> <p>用來識別使用者的日常工作功能和責任。 可以為工作項分配任務角色，以確定完成工作流程所需的技能，而不將其分配給特定用戶。 </p> <p>使用者可以有多個角色。 例如，圖形設計員或顧問。</p> <p>如需詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">建立和管理作業角色</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL日記帳分錄]</p> </td> 
   <td> <p>一個可報告對象，它告訴您項目、任務、問題和其他對象的[!UICONTROL更新]區域中所顯示的跟蹤欄位的系統更新資訊。</p> <p>若要進一步了解，請參閱 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md" class="MCXref xref">[!UICONTROL更新]區域報告</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL看板標籤]</td> 
   <td> <p>在[!UICONTROL任務]報告或[!UICONTROL問題]報告中，[!UICONTROL看板標誌]欄位顯示在[!UICONTROL看板板]的文章上設定的標誌狀態。 可能的值有：[!UICONTROL On Track]、[!UICONTROL Ready To Pull]和[!UICONTROL Is Blocked]。</p> <p>有關在[!UICONTROL看板看板看板看板看板看板看板看板看板上設定動態標誌狀態的詳細資訊，請參閱文章 <a href="../../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md" class="MCXref xref">在[!UICONTROL看板板]上的文章上使用標籤</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>KPI</td> 
   <td>一個可衡量的價值，表明公司如何有效地實現關鍵業務目標。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL滯後]</td> 
   <td>在前置任務的[!UICONTROL計畫完成日期]過後必須經過的時間量，直到相依任務開始為止。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL延遲類型]</td> 
   <td> <p>計算[!UICONTROL Lag]的方法。 可以是：</p> 
    <ul> 
     <li>[!UICONTROL天數]（工作天數）</li> 
     <li>[!UICONTROL日曆天數]（忽略假日）</li> 
     <li>[!UICONTROL百分比]</li> 
     <li>[!UICONTROL一週中的第幾天]</li> 
    </ul> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/tasks/use-prdcssrs/lag-types.md" class="MCXref xref">延遲類型概觀</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL大縮略圖]</td> 
   <td> <p> 在[!UICONTROL文檔]清單或報告中，它會在縮略圖中顯示文檔的預覽。 </p> <p>選擇 <strong>[!UICONTROL大縮略圖]</strong> 以在報表中檢視400像素寬的縮圖。</p> <p>當您修改清單或報表中的欄寬時，縮圖的大小會隨之調整。</p> <p>另請參閱本文中的「[!UICONTROL縮圖]」。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL最近10個檢視器]</td> 
   <td> <p>在報表清單中，此欄位會顯示最多10位最近檢視過報表的使用者的名稱。<br>如需報表清單中使用資訊的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">檢視報表使用量</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL最後一個條件注釋]</td> 
   <td> <p>此欄位顯示對象的所有者上次在對象上輸入的更新。這是對象的所有者最近的活動或交互。</p> <p>此 [!DNL Last Condition Note] 欄是空的（如果已刪除對象的最後一個備注的備注文本）。 在對象上輸入新注釋時，它將成為最後一個注釋，並在列中再次顯示。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL上次財務更新日期]</td> 
   <td>在[!UICONTROL專案]報表中，此欄位會擷取上次計算和更新專案財務的日期和時間。 有關項目財務的資訊，請參閱 <a href="../../../manage-work/projects/project-finances/project-finances-overview-1.md" class="MCXref xref">項目財務概覽</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL最後一條注]</td> 
   <td> <p>此欄位顯示任何使用者上次在物件上輸入的更新。 這是物件上最近的活動或互動。</p> <p>如果已刪除對象最後一個注釋的文本，則[!UICONTROL最後一個注釋]列為空。 在對象上輸入新注釋時，它將成為最後一個注釋，並在列中再次顯示。</p>
   <p>將此欄位添加到[!UICONTROL任務]報表時，子對象上剩餘的任何更新，如問題、子任務、文檔等。  — 此列中不顯示任務的。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL上次查看者]</td> 
   <td> <p>在報表清單中，此欄位會顯示上次檢視報表之使用者的相關資訊。<br>如需報表清單中使用資訊的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">檢視報表使用量</a>.<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL上次檢視日期]</td> 
   <td> <p>在報表清單中，此欄位會顯示上次顯示報表的日期。<br>如需報表清單中使用資訊的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">檢視報表使用量</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL佈局模板]</td> 
   <td>由「系統管理員」或「群組管理員」定義，以識別指定使用者工作區中顯示的標籤和報表。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL佈局類型]</td> 
   <td>結合[!UICONTROL自定義視圖],[!UICONTROL佈局類型]指定[!UICONTROL自定義視圖]的類型。 目前，只有清單可用。 將來，對象的[!UICONTROL詳細資訊]（[!UICONTROL詳細資訊]視圖）可能可用。</td> 
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
   <td>單個任務的模板，用於在應用程式中提供[!UICONTROL任務]和[!UICONTROL模板任務]的一致命名。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL許可證類型]</td> 
   <td>分配給[!UICONTROL訪問級別]的許可證類型。 它可以是[!UICONTROL Full User]、[!UICONTROL Limited User]或[!UICONTROL Requester]。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL許可限制計畫]</td> 
   <td> <p>在[!UICONTROL組]視圖或報表中，此欄位顯示可分配給將相應組指定為其[!UICONTROL主組]的用戶的[!UICONTROL計畫]許可證的最大數量。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL許可限制工作]</td> 
   <td> <p>在[!UICONTROL組]視圖或報表中，此欄位顯示可分配給將相應組指定為其[!UICONTROL主組]的用戶的[!UICONTROL工作]許可證的最大數量。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL有限用戶]</td> 
   <td>允許建立 [!DNL Access Level] 包含僅供檢視的權限，可提交問題、輸入附註及上傳檔案。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL清單控制項]</td> 
   <td> <p>[!UICONTROL介面設定]的一部分，它允許將自訂篩選器、檢視和群組連結至個別使用者或全域連結至所有使用者。</p> </td> 
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
   <td>[！僅手動]</td> 
   <td> <p>[!UICONTROL項目]的[!UICONTROL更新類型]之一。 此設定允許僅在按一下「[!UICONTROL重新計算的時間軸]」時更新[!UICONTROL項目預計]和[!UICONTROL計畫的]時間軸。 在輕度重新計算過程和更新項目中的項目或任務期間，將忽略此方式設定的項目。</p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">選擇項目[!UICONTROL更新類型] </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Me]</td> 
   <td> <p>這是指目前登入的使用者。 </p> <p>建議您在篩選器中使用此欄位，以便在與其他使用者共用報表時讓報表更為通用。 這樣，您只能建立一個報表，根據登入者檢視該報表，而顯示不同資訊，因為資訊一律會針對登入使用者自訂。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL最大用戶數]</td> 
   <td> <p>此欄位已淘汰。 此欄位可能顯示的任何資訊都與 [!DNL Workfront] 已移除，且無法更新欄位。 </p> <p>在舊版 [!DNL Workfront]，您可以在建立或編輯工作角色時更新此欄位。 它顯示可與每個專案中的角色相關聯的使用者總數。 專案上可指派的不限數量使用者允許值為零。 </p>某些報表和清單中仍會顯示欄位，但顯示的資訊無法更新。 </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL里程碑]</td> 
   <td> <p>可與任務關聯的標籤，用於指示任務完成時項目中的關鍵點已實現。 通常，您可以使用里程碑來顯示重要事件，例如項目的某一階段或一組關鍵活動的完成。 [!UICONTROL里程碑]通常與父任務關聯。 您必須先建立里程碑，才能將它們附加至任務。 如需里程碑的資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md">建立里程碑路徑</a> 和 <a href="../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md">將里程碑與任務關聯</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL里程碑路徑]</td> 
   <td>[!UICONTROL里程碑]的集合。 [!UICONTROL里程碑路徑]用於專案，以區分具有特定類型[!UICONTROL里程碑]的專案與具有不同集合[!UICONTROL里程碑]的專案。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL里程碑任務]</td> 
   <td>標籤為指示要測量的可報告事件的任務。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL模組]</td> 
   <td>在以下情形中的單一步驟： [!DNL Workfront Fusion] 可根據關聯的應用程式執行某些功能。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL我的主要角色]</td> 
   <td> <p>當篩選器中引用此名稱時，將顯示與登入使用者具有相同[!UICONTROL主要角色]的使用者，或指派給登入使用者之[!UICONTROL主要角色]的工作項目。</p> <p>建議您在篩選器中使用此欄位，以便在與其他使用者共用報表時讓報表更為通用。 這樣，您只能建立一個報表，根據登入者檢視該報表，而顯示不同資訊，因為資訊一律會針對登入使用者自訂。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL我的首頁團隊]</td> 
   <td> <p>在篩選器中引用此選項時，此欄位會顯示屬於登入使用者的[!UICONTROL首頁團隊]的使用者，或指派給登入使用者的[!UICONTROL首頁團隊]的工作項目。 </p> <p>建議您在篩選器中使用此欄位，以便在與其他使用者共用報表時讓報表更為通用。 這樣，您只能建立一個報表，根據登入者檢視該報表，而顯示不同資訊，因為資訊一律會針對登入使用者自訂。 </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL命名慣例]</td> 
   <td>組織範圍的一組規則，使用資料建立項目、任務和交付項的名稱。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL本機整合]</td> 
   <td>不需要手動編碼或API設定的整合。 也稱為「現成可用」整合。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL導航菜單]</td> 
   <td>應用程式的中上方面板，其中包含[!UICONTROL Workfront]主要區域的連結。</td> 
  </tr> 
 </tr> 
  <tr> 
   <td>[!UICONTROL新數字值]</td> 
   <td>在[!UICONTROL日記帳分錄]報表中，此欄位將顯示更新的值，該欄位將替換[!UICONTROL舊數字值]。
   如需詳細資訊，請參閱本文中的「[!UICONTROL舊數字值]」。</td> 
  </tr>
  <tr> 
   <td>[!UICONTROL非工作日]</td> 
   <td>未分配給完成任何分配的日。 這通常是度假日、假期或週末。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL注]</td> 
   <td>對 [!DNL Workfront] 物件。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL注釋文本]</td> 
   <td> <p>這會顯示使用者在任何物件上輸入的更新文字。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL連結目標數]</td> 
   <td> <p>在[!UICONTROL專案]報表中，這是與專案相關聯的策略目標數目。 如需將專案與策略目標關聯的詳細資訊，請參閱 <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">將專案新增至中的目標  [!DNL Adobe Workfront Goals]</a>.</p> 
   <p>如需有關戰略目標的資訊，另請參閱本文中的「[!UICONTROL目標]」。</p> 
   <p>只有在貴組織已購買時，此欄位才會顯示 [!DNL Workfront Goals]. 如需使用管理策略目標的相關資訊 [!DNL Workfront Goals]，請參閱 <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">將專案新增至[!UICONTROL Adobe Workfront Goals]中的目標</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL對象]</td> 
   <td> <p>組織的工作項目和報表，以及在[!UICONTROL Workfront]中管理這些項目和報表的使用者群組。 對象可以是：</p> 
    <ul> 
     <li>[!UICONTROLPortfolio]</li> 
     <li>[!UICONTROL程式]</li> 
     <li>[!UICONTROL項目]</li> 
     <li>[!UICONTROL任務]</li> 
     <li>[!UICONTROL問題]</li> 
     <li>[!UICONTROL文檔]</li> 
     <li>[!UICONTROL控制面板]</li> 
     <li>[!UICONTROL報表]</li> 
     <li>[!UICONTROL組]</li> 
     <li>[!UICONTROL團隊]</li> 
     <li>[!UICONTROL用戶]</li> 
     <li>[!UICONTROL公司]</li> 
    </ul> <p>如需詳細資訊，請參閱 <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">了解[!UICONTROL Adobe Workfront]中的對象</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL對象類型]</td> 
   <td>如果您建立包含所有自訂表單的報表或清單，則可將此欄位用作檢視或篩選，以查看哪些物件類型與每個表單相關聯。 </td> 
  </tr> 
 <tr> 
   <td>[!UICONTROL舊數字值]</td> 
   <td>在[!UICONTROL日記帳分錄]報表中，這將顯示欄位在更新之前的原始值。 更新欄位的值後，它將在[!UICONTROL日記帳分錄]報表中顯示為[!UICONTROL新編號值]。 如需詳細資訊，另請參閱「[!UICONTROL新編號值]」。</td> 
  </tr>
  <tr> 
   <td>[！僅更改時UICONTROL]</td> 
   <td> <p>[!UICONTROL項目更新]類型之一。 選中此選項時，只有對項目或項目內的任務進行更新或更改時，才會更新[!UICONTROL項目預計]和[!UICONTROL計畫]時間軸。 它不會每晚更新專案。</p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">選擇項目更新類型 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Op Task]</td> 
   <td> <p>在 [!DNL Workfront] 資料庫，用於文本模式報告或計算的自定義資料。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL開啟]</td> 
   <td>問題或任務尚未完成，但正在處理。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL組織圖]</td> 
   <td>組織圖的簡稱。 此圖表顯示組織的階層。 它也位於[!UICONTROL用戶]詳細資訊螢幕上的「頁簽」上，該頁簽顯示並允許設定[!UICONTROL用戶]的[!UICONTROL公司]和[!UICONTROL報告]關係。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL組織設定]</td> 
   <td>這會定義貴組織的[!UICONTROL公司]、[!UICONTROL群組]和[!UICONTROL安全性設定檔]。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL其他組]</td> 
   <td> <p>在列出使用者的報表或檢視中，此欄位會顯示每位使用者所屬的所有群組。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL覆蓋貨幣]</span> </td> 
   <td> 
    <div> 
     <p>在[!UICONTROL作業角色]報表中，這是與作業角色關聯的貨幣。 它是[!UICONTROL設定]區域中所建立的[!UICONTROL基本貨幣]的覆蓋，由 [!DNL Workfront] 管理員。 </p> 
     <p>如需詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">建立和管理作業角色</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL覆蓋貨幣帳單/小時]</span> </td> 
   <td> 
    <div> 
     <p>在[!UICONTROL作業角色]報表中，這是使用作業角色的選定[!UICONTROL覆蓋貨幣]的作業角色的每小時費率。</p> 
     <p> 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">建立和管理作業角色</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL覆蓋貨幣成本/小時]</span> </td> 
   <td> 
    <div> 
     <p>在[!UICONTROL作業角色]報表中，這是使用作業角色的選定[!UICONTROL覆蓋貨幣]的作業角色的每小時成本比率。 </p> 
     <p>如需詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">建立和管理作業角色</a>.</p> 
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
     <p>在[!UICONTROL目標]報表中，這會顯示指派給策略目標的擁有者類型。 以下是目標擁有者類型：</p> 
     <ul> 
      <li> <p>[!UICONTROL用戶]</p> </li> 
      <li> <p>[!UICONTROL團隊] </p> </li> 
      <li> <p>[!UICONTROL組]</p> </li> 
     </ul> 
     <p>目標擁有者為您的組織時，此欄位中不會顯示任何值。 </p> 
     <p>這需要額外的授權。 如需有關 [!DNL Workfront Goals]，請參閱 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">[!DNL Adobe Workfront Goals] 概述</a>. </p> 
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
   <td> <p>[!UICONTROL參數]是自訂欄位。 您可以為所有參數或系統中的自訂欄位建立報表。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL父級]</td> 
   <td>在報表中，此欄位會顯示物件上層的相關資訊。 例如，在[!UICONTROL問題]報表中，它可能會顯示有關問題記錄在下的任務或專案的資訊；在任務報表中，它可能會顯示有關直接父任務或項目的資訊。 有關中可能具有父項的對象的詳細資訊 [!DNL Workfront]，請參閱文章中的「物件的相依性和階層」一節 <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">了解 [!DNL Adobe Workfront]</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL父級延遲]</td> 
   <td>在[!UICONTROL父任務]開始和[!UICONTROL子任務]開始之間必須經過的時間量。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL父任務]</td> 
   <td>也稱為[!UICONTROL摘要任務]。 這是具有子任務（也稱為[!UICONTROL子任務]）的任務。 父任務的[!UICONTROL持續時間]、[!UICONTROL需要工作]和[!UICONTROL完成百分比]是從子任務中計算的。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL兼職資源]</td> 
   <td>容量小於系統中定義的預設計畫的授權用戶。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL百分比完成]</td> 
   <td> <p>項目、任務或問題欄位，顯示與任務、項目或問題相關聯的工作完成百分比。</p> <p>您可以手動更新此欄位以解決問題和執行工作。 </p> <p>對於項目和父任務，此欄位是所有工作任務的匯總，您無法手動更新它。 </p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/tasks/task-information/project-percent-complete.md" class="MCXref xref">專案[!UICONTROL百分比完成]概觀</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL權限]</td> 
   <td> <p>授予物件上使用者的權限，通常是為了讓使用者能夠完成項目上的工作或檢視項目。 您可以將權限授予：</p> 
    <ul> 
     <li>[!UICONTROL項目]</li> 
     <li>[!UICONTROL任務]</li> 
     <li>[!UICONTROL問題]</li> 
     <li>[!UICONTROLPortfolio]</li> 
     <li>[!UICONTROL程式]</li> 
     <li>[!UICONTROL報表]</li> 
     <li>[!UICONTROL控制面板]</li> 
     <li>[!UICONTROL文檔]</li> 
     <li>[!UICONTROL自訂Forms]</li> 
     <li>[!UICONTROL視圖]</li> 
     <li>[!UICONTROL篩選器]</li> 
     <li>[!UICONTROL分組]</li> 
    </ul> <p>如需詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">對象共用權限概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL計畫]</td> 
   <td> <p>這是 [!DNL Workfront] 系統。 使用者必須擁有此權限才能存取 [!DNL Workfront].</p> <p>如需詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] 授權概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL計畫](在 [!DNL Scenario Planner])</td> 
   <td> <p>使用 [!DNL Workfront] 方案規劃器。 您可以概述貴公司近期和長期未來的策略，並確定每個高級別結果，並將其作為計畫添加到 [!DNL Workfront] 方案規劃器。 </p> <p>您無法顯示 [!DNL Scenario Planner] 報表中的計畫，您無法透過 [!DNL Workfront] API。 </p> <p>此 [!DNL Scenario Planner] 需要額外的授權。 如需 [!DNL Workfront Scenario Planner]，請參閱 <a href="../../../scenario-planner/scenario-planner-overview.md">此 [!DNL Scenario Planner] 概述</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL已計畫]</td> 
   <td> <p>排程發生某件事的時間範圍。 當您在 [!DNL Workfront]，您可以建立計畫的開始和結束日期，以及發生時間範圍。 這些值代表您的原始意圖，或項目完成所需時間的估計。 </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL計畫福利]</td> 
   <td>這是項目經理用於估計完成項目是否會給組織帶來任何金錢利益的人工輸入。 指定此值可以是為專案建立[!UICONTROL商業案例]的一部分。 您必須擁有專案的[!UICONTROL管理]權限，才能更新此值。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL預算小時數]</td> 
   <td> <p>在[!UICONTROL預算小時]報表中，此報表顯示為項目或[!UICONTROL資源規劃器]中的[!UICONTROL任務角色]編入預算的小時數。 </p> <p>有關[!UICONTROL資源計畫器]中的項目或職責預算的資訊，請參閱文章 <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">使用[!UICONTROL項目]和[!UICONTROL角色]視圖在[!UICONTROL資源規劃器]中的預算資源</a>. 如需[!UICONTROL預算小時數]報表的相關資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">報告：預算小時數</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL計畫完成日期]</td> 
   <td> <p>您可以手動將[!UICONTROL計畫完成日期]設定為您選擇的日期。 如果您未設定[!UICONTROL計畫完成日期], [!DNL Workfront] 自動設定。 自動設定後，[!UICONTROL計畫完成日期]為： [!UICONTROL計劃開始日期] + [!UICONTROL持續時間]</p> <p>如需詳細資訊，請參閱下列文章：</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">任務[!UICONTROL計畫完成日期]概覽</a> </p> </li> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">設定項目[!UICONTROL計畫完成日期]</a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL計畫成本]</td> 
   <td> <p>項目的[!UICONTROL計畫人工成本]和[!UICONTROL計畫支出成本]的合計。 這不包括項目上的[!UICONTROL計畫風險成本]。  </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL計畫持續時間]</td> 
   <td> <p>任務的[!UICONTROL計畫持續時間]通常與任務的[!UICONTROL持續時間]相同。 它表示任務的[!UICONTROL計劃開始]和[!UICONTROL計畫完成日期]之間的天數差異。 </p> <p>當任務的[!UICONTROL持續時間]類型為[!UICONTROL工作驅動]時，根據您分配給任務的資源數，[!UICONTROL計畫持續時間]可能與任務的[!UICONTROL持續時間]不同。 </p> <p>例如，如果[!UICONTROL持續時間]類型為[!UICONTROL工作驅動]的任務的[!UICONTROL持續時間]為3天，並且您為任務分配了一個具有全時計畫的資源，則[!UICONTROL計畫持續時間]也為3天。 如果為同一任務分配了三個具有全時計畫的資源，則[!UICONTROL持續時間]會保持3天，但[!UICONTROL計畫持續時間]會變為1天。 [!UICONTROL計畫持續時間]還更改了任務的[!UICONTROL計劃開始]和[!UICONTROL計畫完成日期]，以反映新的[!UICONTROL計畫持續時間]。 因此，也會影響專案的時間軸。 </p> <p>有關任務的[!UICONTROL持續時間]和[!UICONTROL計畫持續時間]之間差異的詳細資訊，請參閱文章 <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md" class="MCXref xref">任務的[!UICONTROL計畫持續時間]和[!UICONTROL持續時間]之間的差異</a>.</p> <p>專案和問題沒有[!UICONTROL計畫持續時間]。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL計畫持續時間分鐘]</td> 
   <td> <p>專案或問題的[!UICONTROL計畫持續時間分鐘]是專案或問題的[!UICONTROL持續時間]（以分鐘為單位）。 </p> <p>任務沒有[!UICONTROL計畫持續時間分鐘]欄位。 </p> <p>[!UICONTROL模板任務]有一個[!UICONTROL計畫持續時間分鐘]欄位，該欄位以分鐘顯示任務的[!UICONTROL計畫持續時間]。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL計畫費用成本]</td> 
   <td> <p>為項目或任務記錄的所有費用的[!UICONTROL計畫金額]總和。</p> <p><b>範例</b></p>
   <p>如果為任務1建立費用，並在「[!UICONTROL計畫金額]」欄位中輸入$600.00，則此任務的「[!UICONTROL計畫費用成本]」為$600.00。 </p> 
   <p>對於一個項目， [!DNL Workfront] 使用以下公式計算[!UICONTROL計畫費用成本]:</p> <p><code>Project [!UICONTROL Planned Expense Cost] = SUM (All Project [!UICONTROL Planned Expense Costs]) + SUM (All Tasks [!UICONTROL Planned Expense Costs])</code> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (Drafting this because not sure if this is correct anymore)</p>
    --> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL計畫小時數]</td> 
   <td> <p>此欄位將顯示在[!UICONTROL項目]、[!UICONTROL任務]中，並顯示問題區域、項目報表、任務或問題以及資源管理工具，如[!UICONTROL資源規劃器]、[!UICONTROL工作負載平衡器]和[!UICONTROL利用率]報表。 </p> <p>它顯示項目所有者估計完成每個任務或問題所需的小時數。 對於專案，通常是來自專案工作的[!UICONTROL計畫小時數]匯總。 </p> <p>根據您從何處查看，[!UICONTROL計畫小時數]欄位可能會顯示不同的資訊。 如需「計畫小時數」的相關資訊，請參閱 <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">計畫小時數概觀</a>.</p> <p>計畫小時數會以分鐘為單位儲存在 [!DNL Workfront] 資料庫。 使用此欄位撰寫計算時，請務必說明小時數顯示為分鐘的事實。<br></p> <p>預設情況下，計畫小時數平均分配給工作項目期間內的所有天數，也平均分配給任務的所有資源。 用戶可以更新工作項的每日計畫小時數，或每個受託人的單個計畫小時數。</p> <p>針對專案、工作和問題，更新此欄位的方式有所不同： </p> 
    <ul> 
     <li> <p>如有問題，您可以手動更新此欄位。 「發放計畫小時數」不會添加到「項目計畫小時數」中。 </p> <p>提示：在問題報告中，[!UICONTROL計畫小時數]欄位中的一個將替換為[!UICONTROL工作]欄位。 欄位會顯示問題的「計畫小時數」。 如需詳細資訊，請參閱此表中的「work」或「[!UICONTROL Work]」欄位。 </p> </li> 
    </ul> 
    <ul> 
     <li> <p>對於任務，當任務的[!UICONTROL持續時間類型]為[!UICONTROL計算分配]或[!UICONTROL簡單]時，可以手動更新此欄位。 此欄位的計算方式為 [!DNL Workfront] 當任務的[!UICONTROL持續時間類型]為[!UICONTROL計算工作]或[!UICONTROL工作驅動]時。<br>有關[!UICONTROL任務持續時間]的資訊，請參閱文章 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任務[!UICONTROL持續時間]和[!UICONTROL持續時間類型]的概述</a>.</p> </li> 
    </ul> 
    <ul> 
     <li> <p>若為專案， [!DNL Workfront] 通過添加項目上所有任務中的所有計畫小時數來計算計畫小時數。 </p> </li> 
    </ul> <p><b>筆尖</b></p> <p>您也可以使用文字模式並參考其他欄位，在[!UICONTROL專案]、[!UICONTROL任務]或[!UICONTROL問題]報表中顯示[!UICONTROL計畫時數]。 如需詳細資訊，請參閱<code>work</code>", "[!UICONTROL工作]"和"<code>workRequiredExpression</code>」欄位。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL計畫人工成本]</td> 
   <td> 
    <p>對於任務，用戶或角色的小時費率乘以分配給用戶或角色的小時數。</p> <p>對於項目，它是所有任務的所有[!UICONTROL計畫人工成本]的合計。</p> <p>是否使用用戶或角色的比率取決於為給定任務選擇的成本類型。 </p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/projects/project-finances/track-costs.md">追蹤成本</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL計畫收入]</td> 
   <td> <p>任務和專案可顯示[!UICONTROL計畫收入]的值，位於 [!DNL Workfront]. [!UICONTROL計畫收入]表示與項目上任務的[!UICONTROL計畫小時數]關聯的金額。 對於專案，也可以包含專案的[!UICONTROL固定收入]。 </p> <p>對於任務，這是與任務的[!UICONTROL計畫小時數]關聯的收入。 所有任務的「計畫小時數」累計到項目的「計畫小時數」，用於計算項目[!UICONTROL計畫小時數]。 </p> 
   <p>[!DNL Workfront] 使用下列公式計算任務和項目的[!UICONTROL計畫收入]:</p> 
   <p><code>Task [!UICONTROL Planned Revenue] = [!UICONTROL Planned Hours] * Billing hourly rate</code> </p> <p><code>Project [!UICONTROL Planned Revenue] = SUM (All tasks [!UICONTROL Planned Revenue]) + [!UICONTROL Fixed Revenue]</code> </p> 
   <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the note below is duplicated in this article: /Content/Resource Mgmt/Resource utilization/view-utilization-information.htm and in the glossary)</p>
    --> 
    <p>在[!UICONTROL項目詳細資訊]區域和項目報表中顯示的項目[!UICONTROL計畫收入]與[!UICONTROL利用率]報表中顯示的計畫收入不同。 </p> <p>[!UICONTROL項目詳細資訊]區域中的[!UICONTROL計畫收入]反映任務收入以及項目的固定收入。 [!UICONTROL利用率報告]中的[!UICONTROL計畫收入]將顯示僅與項目中的任務關聯的[!UICONTROL計畫收入]。 </p> 
     <p><b>範例</b></p>  
      <p>如果項目有1個10小時的任務，分配給一個顧問，每小時費率為$20，而項目有$100 [!UICONTROL固定收入]，則[!UICONTROL利用率]報表會顯示與任務小時數關聯的[!UICONTROL計畫收入]為$200的[!UICONTROL計畫收入]。 「 [!UICONTROL項目詳細資訊]」部分顯示$300（來自任務的[!UICONTROL計畫收入]和項目的固定收入）。 </p> 
    <p>如需關於在 [!DNL Workfront] 請參閱 <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md">帳單和收入概觀</a>. </p> 
    <p>如需[!UICONTROL使用率報表]中[!UICONTROL計畫收入]計算的相關資訊，請參閱 <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">查看資源利用資訊 </a>. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL計畫風險成本]</td> 
   <td> <p>項目所有風險的[!UICONTROL潛在成本]合計，考慮其發生的可能性。 此金額不包含在項目的[!UICONTROL計畫成本]中。</p> <p>項目的[!UICONTROL計畫風險成本]按以下公式計算：</p> <p><code>Planned Risk Cost = SUM(Potential Risk Cost * Probability / 100)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL門戶配置檔案]</td> 
   <td>管理員定義的標籤和入口區段集合，會顯示在 [!DNL Workfront] 應用程式[!UICONTROL首頁]和其他控制面板。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL門戶節]</td> 
   <td>控制面板或入口網頁上Tab的一個元件。 通常是單一報表、圖表、日曆或關鍵資訊清單。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL門戶頁簽]</td> 
   <td>入口網站或控制面板上的索引標籤，最多包含三個入口網站區段。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROLPortfolio]</td> 
   <td> <p>具有統一特徵的項目集合。 這些專案通常會爭用相同的資源、預算或時段。 您可以將Portfolio分為方案，並在項目添加到Portfolio之前將其與方案關聯。</p> <p>如需產品組合的詳細資訊，請參閱 <a href="../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md">Portfolio概觀，於 [!DNL Adobe Workfront]</a>.</p> 
   </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROLPortfolio管理]</td> 
   <td>一個側重於管理收集或相關方案和項目工作的實踐領域。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROLPortfolio優化程式]</td> 
   <td>A [!DNL Workfront] 協助評估和排定項目組合優先順序的工具。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROLPortfolio所有者]</td> 
   <td>負責確定投資組合的優先順序和預算的利益攸關方。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL潛在風險成本]</td> 
   <td>這是您可在清單和報表中找到的專案欄位。 它顯示與項目相關的風險的潛在成本（如果發生）。 如需詳細資訊，請參閱 <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">計算潛在風險成本 </a>. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL前身]</td> 
   <td> <p>在完成相依任務之前必須完成的任務。 另一個任務標籤為[!UICONTROL依賴項]的任務。 前置任務允許規劃器設定序列相依性邏輯，例如在完成另一個任務後啟動任務。</p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">任務前置任務概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL主要公司]</td> 
   <td>使用者所屬的公司，如其使用者設定中所指定。 公司也可以與專案相關聯。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL主要聯繫人]</td> 
   <td><p>[!UICONTROL Primary Contact]是問題的建立者，它由 [!DNL Workfront] 當某人建立問題時。 如果您有 [!DNL Manage] 問題的權限。 問題只能有一個主要聯繫人。</p> 
   <p>如果您變更主要連絡人，原本指定為主要連絡人的使用者仍可存取問題的[!UICONTROL管理]存取權。</p>
   <p>將問題轉換為任務或項目時，指定為的[!UICONTROL主聯繫人]的用戶將成為項目或任務的[!UICONTROL已轉換的問題創作者]。 如果問題的[!UICONTROL主要聯繫人]在轉換問題後更新，則在轉換發生時，[!UICONTROL已轉換的問題創作者]將保留為問題的[!UICONTROL主要聯繫人]。 另請參閱本文中的「[!UICONTROL轉換的問題創作者]」。</p> 
   </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL優先順序]</td> 
   <td>可指派給任務、問題或專案的值，以指定其重要性。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL專用]</td> 
   <td>在[!UICONTROL Note]或[!UICONTROL Document]上，此選項使大多數查看器都隱藏該對象。 對於專用幫助台隊列，只有隊列團隊中的用戶可以通過[!UICONTROL幫助台]區域向該隊列提交問題。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL配置檔案]</td> 
   <td>使用者帳戶的所有相關資訊。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL程式]</td> 
   <td> <p>組合內的子集，可將類似的項目組合在一起，以獲得明確的好處。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL程式管理]</td> 
   <td>管理跨項目依賴關係、風險、問題、要求和解決方案，以保持計畫的健康並實現既定計畫收益。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL程式所有者]</td> 
   <td>負責監督和組織活動的利益相關方，確保項目目標與公司目標一致。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL進度]</span> </td> 
   <td> <p>在[!UICONTROL目標]報表中，這會顯示完成策略目標的百分比。 進度百分比顯示為數字。 如需有關策略目標的資訊，另請參閱下表中的「[!UICONTROL目標]」。</p> <p>只有在貴組織已購買時，此欄位才會顯示 [!DNL Workfront] 目標。 如需使用管理策略目標的相關資訊 [!DNL Workfront Goals]，請參閱 <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md"> 將專案新增至中的目標 [!DNL Adobe Workfront Goals] </a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL進度狀態]</td> 
   <td> <p>在「項目」、「任務」和「目標」報表中，此欄位顯示項目、任務或戰略目標的「進度狀態」。 如需詳細資訊，請參閱下列文章：</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-progress-status.md" class="MCXref xref">項目進度狀態概觀</a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">任務進度狀態概述</a> </p> </li> 
     <li> <p><a href="../../../workfront-goals/goal-management/calculate-goal-progress.md">中的目標進度和條件概觀 [!DNL Adobe Workfront Goals]</a> </p>
     <p>[!UICONTROL目標]報表和 [!DNL goals] 欄位只有在貴組織已購買時才會顯示 [!DNL Workfront Goals]. 如需有關 [!DNL Workfront Goals]，請參閱 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] 概述</a>. </p> </li>
    </ul> </td> 
  </tr> 
  <td>[!UICONTROL項目]</td> 
   <td> <p>必須在特定時間範圍內完成並且必須使用特定預算和資源數量的大量工作。 為使其易於管理，您將項目分成一系列任務。 完成所有任務將完成項目。 如需規劃專案的相關資訊，請參閱 <a href="../../../manage-work/projects/planning-a-project/plan-project.md">規劃專案概觀</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL項目分配計畫小時數]</td> 
   <td> <p>在[!UICONTROL計畫作業角色]報表中，它顯示與分配給項目中的任務或問題的作業角色相關聯的[!UICONTROL計畫小時數]。 您的 [!DNL Workfront] 例項，除非您的公司已購買 [!DNL Workfront Scenario Planner] 授權。 如需 [!DNL Workfront Scenario Planner]，請參閱 <a href="../../../scenario-planner/scenario-planner-overview.md">此 [!DNL Workfront Scenario Planner] 概述</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL項目詳細資訊]</td> 
   <td>項目當前狀態的詳細資訊。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL項目預算成本]</td> 
   <td> <p> 這是項目在清單和報表中顯示的[!UICONTROL預算成本]。</p><p>另請參閱本文中的「[!UICONTROL預算成本]」。</p></td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Project Management]</td> 
   <td>管理項目建立、分類和命名閾值的一組策略。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL項目開銷]</td> 
   <td>在[!UICONTROL小時]報表中，此欄位專為與小時類型為[!UICONTROL專案時間]記錄的小時數相關聯的財務資訊而保留。 專案可以有自己的計費率，如果專案直接記錄一小時，系統便會在計算時使用這些費率。 根據專案設定，專案也可以有不同的貨幣，而且這些小時內可能會有貨幣轉換。 [!UICONTROL項目開銷]對象允許 [!DNL Workfront] 才能得到這些資訊。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL項目所有者]</td> 
   <td>負責管理項目的範圍、時間表和分配的用戶。 更改單、財務更改和可交付項的預設批准者。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL項目規劃]</td> 
   <td>開發和維護項目計畫的流程。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL項目贊助商]</td> 
   <td>每個使用者都應與之相關的指定利害關係人設定檔。 在 [!DNL Workfront]，則這些欄會被指定為[!UICONTROL存取層級]</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL項目團隊]</td> 
   <td> <p>指派給專案的使用者或角色的集合</p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md">專案團隊概觀</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL專案追蹤]</td> 
   <td>用於測量項目運行狀況和範圍的資料</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL投影]</td> 
   <td> <p>根據任務、問題或項目的計畫小時數和完成百分比，估計完成工作的時間時間。</p> <p>這是指工作、問題或專案的日期或[!UICONTROL持續時間]。 通常，它會指定在某些工作已經完成或一段時間過後，對工作項目的生命週期更真實的日期和持續時間。 </p> <p>例如，任務的[!UICONTROL預計完成日期]是 [!DNL Workfront] 根據迄今為止已完成的工作量、分配給該任務的人員數量以及自開始日期以來已經過的時間，估計任務將完成。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL校樣截止日期]</td> 
   <td> <p>在包含[!UICONTROL文檔版本]對象的報表中（如[!UICONTROL文檔版本]報表和[!UICONTROL校樣批准]報表），此欄位顯示一週中的某天、日期、一天中的某天和校樣截止日期的年份。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL證明決策]</td> 
   <td> <p>在包含[!UICONTROL文檔版本]對象的報表中（如[!UICONTROL文檔版本]報表和[!UICONTROL校樣批准]報表），此欄位顯示校樣的決策狀態（待定、需要更改或已批准）</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL校樣名稱]</td> 
   <td> <p>在包含[!UICONTROL文檔版本]對象的報表中（如[!UICONTROL文檔版本]報表和[!UICONTROL校樣批准]報表），此欄位將顯示校樣名稱。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL校樣頁面]</td> 
   <td> <p>在包含[!UICONTROL文檔版本]對象的報表中（如[!UICONTROL文檔版本]報表和[!UICONTROL校樣批准]報表），此欄位將顯示校樣中包含的頁數。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL校樣進度]</td> 
   <td> <p>在包含[!UICONTROL文檔版本]對象的報表中（如[!UICONTROL文檔版本]報表和[!UICONTROL校樣批准]報表），顯示校樣（[!UICONTROL已發送]、[!UICONTROL已開啟]、[!UICONTROL已注釋]、[!UICONTROL已做出決策]）的進度狀態。</p> <p>如需詳細資訊，請參閱 <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md#understanding-progress-and-status" class="MCXref xref">校樣進度概觀</a> in <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md" class="MCXref xref">校樣進度與狀態概觀</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL校對]</td> 
   <td>一個審閱過程，其中一個或多個用戶對應在影像、文本文檔、視頻或互動式Web內容中更改的內容進行標籤和注釋。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL公用]</td> 
   <td>在[!UICONTROL Note]或[!UICONTROL Document]上，此選項使其他用戶甚至外部人員可以訪問該對象 [!DNL Workfront]. 對於[!UICONTROL服務台隊列],[!UICONTROL公用]表示所有可提交問題的用戶都可以通過[!UICONTROL服務台]區域提交問題。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL質量]</td> 
   <td>組織內對工作品質的認知。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL隊列]</td> 
   <td>也稱為[!UICONTROL服務台隊列]。 這是已發佈到[!UICONTROL幫助台]區域的項目，允許用戶向其提交問題。 通常會為特定主題（如錯誤、專案要求等）建立佇列。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL隊列屬性]</td> 
   <td>這些設定定義了要發佈到[!UICONTROL服務台]的項目的「問題」提交規則。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL隊列主題]</td> 
   <td> <p>[!UICONTROL服務台隊列]上的屬性，允許提交問題的用戶選擇主題。 主題可以：</p> 
    <ul> 
     <li>與自訂資料表單相關聯。</li> 
     <li>通過選定主題上的路由規則集自動將問題分配給用戶、角色或團隊。</li> 
     <li>通過選定主題上的路由規則集將問題移到其他項目或隊列。</li> 
    </ul> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">建立佇列主題</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL排名]</td> 
   <td> <p>在[!UICONTROL存取層級]報表中，您可以手動指出[!UICONTROL存取層級]的[!UICONTROL排名]。 這可協助您，因為 [!DNL Workfront] 管理員，以直觀地識別與每個訪問級別相關的複雜程度。 例如，您可以為較複雜（[!UICONTROL Plan]級）的訪問級別提供較低的數字，為較不複雜（[!UICONTROL Requesters]級）的訪問級別提供較高的數字。 您無法對標準存取層級進行排名。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL就緒]</td> 
   <td> <p>任務報告上的此欄位指示積壓工作上的[!UICONTROL Agile]任務是否已標籤為[!UICONTROL Ready]。 此標幟僅適用於[!UICONTROL Agile]任務，這些任務是指派給[!UICONTROL Agile]團隊的任務。 </p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL週期頻率]</td> 
   <td> <p>顯示在循環任務父項的[!UICONTROL任務詳細資訊]或[!UICONTROL編輯任務]框中的欄位。 這是重複執行中的任務發生的頻率。 有關建立循環任務的資訊，請參閱 <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">建立循環任務</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL參考編號]</td> 
   <td> <p>項目、任務和問題在建立時會自動與唯一的參考編號關聯。 您可以在專案、任務或問題的[!UICONTROL詳細資訊]頁面或清單或報表中檢視[!UICONTROL參考編號]。 </p> <p><b>筆尖</b><p><br>當兩個項目具有相同名稱時，可以推遲到參考編號，因為參考編號始終是唯一的。 </p> <p>[!DNL Workfront] 自動在系統級別生成循序參考編號。 每個項目、任務或問題都會獲得序列中的下一個可用編號。 <br></p> <p>例如，如果用戶A建立了任務， [!DNL Workfront] 可以自動將任務分配為「參考編號100」。 如果使用者B在此之後立即建立問題， [!DNL Workfront] 將問題分配為「Reference Number 101」。 不能手動編輯引用編號。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL拒絕問題]</td> 
   <td>在項目或任務報表中，這是在項目或任務的批准被拒絕時建立的問題。 如需拒絕問題的相關資訊，請參閱文章 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">建立工作項的審批流程</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL剩餘風險成本]</td> 
   <td> <p>顯示項目的[!UICONTROL計畫風險成本]與項目上所有風險的所有[!UICONTROL實際成本]合計之差的項目欄位。 </p> <p>項目的[!UICONTROL剩餘風險成本]使用以下公式計算：</p> <p><code>[!UICONTROL Remaining Risk Cost] = Project [!UICONTROL Planned Risk Cost] - SUM([!UICONTROL Actual Cost] for all risks)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL重新規劃]</td> 
   <td>更改項目日期以修復或解決問題。 例如，已暫停數個月的專案需要重新規劃，以反映正確的日期。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL報告]</td> 
   <td>包含有關給定資訊的圖表或表 [!DNL Workfront] 物件及其相關屬性。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL請求]</td> 
   <td> <p>在單個集中隊列中進行分類的問題類型，與持續的工作無關。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL請求隊列]</td> 
   <td>由流量和分類程式管理的積壓問題。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL要求速度]</td> 
   <td>接收和完成請求的總工作週期時間。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL請求者]</td> 
   <td>通常是授權類型。 具有請求者許可證的用戶可以提交對系統中將要發生的新作品的請求。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL保留時間]</td> 
   <td>用戶的「個人時間」上指定的天數，表示用戶將無法工作。 請參閱「[!UICONTROL非工作日]」。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL解決問題]</td> 
   <td> <p>在問題報表中，在檢視或篩選器中使用此欄位，即可參照解決問題的問題。 </p> <p>有關在報表中顯示解析對象的資訊，請參閱 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">在報表中查看可解析和可解析的對象資訊</a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解析和可解析對象概述 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL解析項目]</td> 
   <td> <p>在問題報表中，在檢視或篩選器中使用此欄位，即可參照解決問題的專案。 </p> <p>有關在報表中顯示解析對象的資訊，請參閱 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">在報表中查看可解析和可解析的對象資訊</a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解析和可解析對象概述 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL解析任務]</td> 
   <td> <p>在問題報表中，在檢視或篩選器中使用此欄位，以參照解決問題的任務。 </p> <p>有關在報表中顯示解析對象的資訊，請參閱 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">在報表中查看可解析和可解析的對象資訊</a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解析和可解析對象概述 </a>.</p> </td> 
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
   <td> <p>[!UICONTROL Resource Management]是一組企業工具，允許您根據資源的可用性準確預測資源的使用情況，以便必須完成的工作按時和按預算完成。 </p> <p>使用資源管理工具，您可以規劃資源的長期容量和短期計畫需求。 </p> <p>有關 [!DNL Workfront]，請參閱 <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">開始使用資源管理</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資源管理器ID]</td> 
   <td><p>在項目報告中，建立篩選器以查找特定資源管理器時可以使用此選項。 </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資源管理器]</td> 
   <td> <p>在項目報告或清單視圖中，此欄位是資訊欄位，顯示指定用於在項目上執行資源管理活動的用戶。  在報表中使用「[!UICONTROL資源管理器]」時，將顯示資源管理器清單，項目上的每個資源管理器以逗號分隔。 您最多可以在指定的項目中指定30名資源管理器。</p> <p>如需詳細資訊，請參閱文章 <a href="../../../manage-work/projects/planning-a-project/designate-resource-managers-for-projects-and-templates.md">為項目或模板指定資源管理器 </a>.</p> </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL資源計畫員預算小時數] </td> 
   <td>在[!UICONTROL資源規劃器]中為項目和與其關聯的資源編入預算的小時數。 另請參閱本文中的「[!UICONTROL預算小時數]」。 </td> 
  </tr>  
  <tr> 
   <td>[!UICONTROL資源規劃器] </td> 
   <td>進階 [!DNL Workfront] 可讓您檢視及管理專案、工作角色或使用者之間的資源的工具。 如需詳細資訊，請參閱 <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">資源計畫員概覽</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資源計畫員預算人工成本]</td> 
   <td> <p>這些是與使用資源計畫員的項目任務職責的預算小時數關聯的成本。 </p> <p>另請參閱本文中的「預算人工成本」。 </p> </td>

</tr> 
  <tr> 
   <td>[!UICONTROL資源池]</td> 
   <td> <p>資源池是可以與項目關聯的用戶的集合。同一資源池中的用戶通常屬於同一部門，具有類似或互補的技能，或由相同預算供資。 您可以將多個資源池關聯到項目或用戶。 資源池可以專門分配給項目或由多個項目共用。</p> 
   <p>有關資源池的詳細資訊，請參見 <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> 資源池概述 </a>.</p> 
   <p>在項目報表中，資源池顯示與項目關聯的所有池。 此對象不能用於分組。</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資源利用率]</td> 
   <td>顯示特定時段內可用小時數的報表，以及報表中每位使用者排程的小時數。 這也會計算為[!UICONTROL每日平均小時數]和分配百分比。</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL結果]</td> 
   <td>在 [!DNL Workfront Goals]，結果是目標的進度指標。 可以是您手動更新的數字、百分比值或貨幣金額。 您無法在報表中顯示結果，也無法透過 [!DNL Workfront] API。 如需活動的相關資訊，請參閱 <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">開始使用Adobe Workfront Target中的結果和活動</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL收入]</td> 
   <td>任務或項目的可開單金額。 金額可以是每小時、固定，或兩者的組合。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL收入類型]</td> 
   <td>收入類型決定任務如何應計收入。 有些範例包括[!UICONTROL固定每小時]、[!UICONTROL角色每小時]和[!UICONTROL角色每小時（含上限）]。 如需關於在 [!DNL Workfront] 請參閱 <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">帳單和收入概觀</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL審核者]</td> 
   <td>通常是授權類型。 具有[!UICONTROL Reviewer]許可的用戶能夠審閱和批准系統中的工作項目。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL風險]</td> 
   <td> <p>這可能是指 [!DNL Workfront]:</p> 
    <ul> 
     <li> <p>專案上的欄位，指出專案的風險程度。 您可以根據風險等級排定執行專案的優先順序。 項目可能具有以下風險級別：</p> <p>- [!UICONTROL極低]</p> <p>- [!UICONTROL低]</p> <p>- [!UICONTROL中]</p> <p>- [!UICONTROL高]</p> <p>- [!UICONTROL非常高]</p> <p>您為項目指定的風險級別無法自定義。 </p> <p> 如需更新專案風險的相關資訊，請參閱文章的「專案設定」一節 <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">編輯專案</a>. 您可以在報表中顯示專案的風險欄位。 </p> </li> 
     <li> <p>在項目生命週期中可能發生的事件，可確定對項目的成本、範圍或計畫的潛在影響。 您可以定義項目的潛在風險，並在構建項目的業務案例時將發生風險的可能性或成本關聯起來。 有關為項目的業務案例添加風險的資訊，請參閱「建立和編輯項目風險」。 </p> <p>您無法在報表中顯示[!UICONTROL業務案例]中定義的風險。 您只能在報表和清單中顯示幾種類型的風險成本。 </p> </li> 
    </ul> </td>

</tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL風險成本]</td> 
   <td> <p>與項目風險相關的成本。 以下是可在報表中顯示的與項目相關的風險成本：</p> 
    <ul> 
     <li> <p>[!UICONTROL實際成本]:一個風險欄位，顯示已發生的風險的實際成本。 除了報告和清單之外，在編輯或建立風險時，您還可以在[!UICONTROL編輯風險]框中找到它。 </p> <p>有關項目、任務或問題成本，請參閱本文中的「[!UICONTROL實際成本]」。 </p> </li> 
     <li> <p>[!UICONTROL計畫風險成本]:項目上的欄位，顯示項目的所有[!UICONTROL潛在風險成本]。 另請參閱本文中的「[!UICONTROL計畫風險成本]」。 </p> <p>有關潛在風險成本的資訊，請參見 <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">計算潛在風險成本 </a>. </p> </li> 
     <li> <p>[!UICONTROL剩餘風險成本]:項目上的欄位，顯示所有風險的[!UICONTROL實際成本]合計與[!UICONTROL計畫風險成本]之間的差值。 另請參閱本文的「剩餘風險成本」。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL風險管理]</td> 
   <td>識別、減輕和監控風險的程式。</td> 
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
   <td>「項目」和「隊列」上的設定，可自動將問題分配給用戶、角色或團隊，或將問題移動到其他項目或隊列。 路由規則通常與服務台隊列一起使用，以自動分配傳入的問題。</td> 
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
   <td>[!UICONTROL保存的搜索]</td> 
   <td>已保存搜索條件的搜索。 「已儲存的搜尋」可讓您輕鬆執行相同的搜尋，而無須再次輸入搜尋准則。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL方案](在 [!DNL Workfront Fusion]) </td> 
   <td> <p>案例由一系列步驟（模組）組成，這些步驟（模組）指示應如何在應用程式/服務之間傳輸和轉換資料。</p> <p>若要了解 [!DNL Workfront Fusion]，請參閱 <a href="../../../workfront-fusion/scenarios/scenario-overview.md" class="MCXref xref">[!DNL Adobe Workfront Fusion] 方案概觀</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL案例](在 [!DNL Workfront Scenario Planner]) </td> 
   <td> <p>在 [!DNL Scenario Planner]，案例是計畫的復本。 </p> <p>此 [!DNL Scenario Planner] 需要額外的授權。 如需 [!DNL Workfront Scenario Planner]，請參閱 <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">此 [!DNL Scenario Planner] 概述</a>. </p> <p>如需建立藍本的詳細資訊，請參閱 <a href="../../../scenario-planner/create-and-compare-scenarios-for-a-plan.md">在 [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL計畫]</td> 
   <td>每週工作計畫，包括工作時間，加上休假天數（如節假日）和例外天數（如星期六工作日）。 排程可套用至「專案」和「使用者」。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL計畫免除]</td> 
   <td>也稱為[!UICONTROL修改的Shift]。 排程的天數，與排程所定義的一般每週工作時間不同。 例如，排程在星期一到星期五設為僅工作時，排程將是[!UICONTROL排程例外]。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL計畫報表]</td> 
   <td> <p>當您建立報表報表報表時，如果報表已排程要傳送，則可使用[!UICONTROL排程報表]欄位來顯示報表排程的相關資訊。 此欄位在項目符號清單中顯示多個值，每個報表的每個排程各一個。 如需排程報表的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md" class="MCXref xref">報表傳送概觀</a>.</p> <p>由於此欄位顯示多個值，因此無法在分組中使用。 您只能在篩選器或檢視中存取。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL範圍更改]</td> 
   <td>[!UICONTROL審核跟蹤]，如果活動，則每當對項目或任務的範圍進行更改時都會生成注釋，例如，[!UICONTROL任務持續時間]或[!UICONTROL前置任務]被更改時。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL節]</td> 
   <td>畫面上的區域，以及其專屬的標題，用來組織自訂資料以供顯示。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL節分符]</td> 
   <td>截面之間的間隙或邊框。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL安全性]</td> 
   <td>允許用戶與系統中的特定對象（而非其他對象）交互的設定。 另請參閱本文中的「[!UICONTROL存取層級]」。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL設定]</td> 
   <td>管理員可以設定系統配置和首選項的區域。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL嚴重性]</td> 
   <td> <p>[!UICONTROL嚴重性]表示項目對完成工作的影響程度。 例如，[!UICONTROL嚴重性]高的問題可能完全阻止任務的完成，但[!UICONTROL嚴重性]低的問題可能只是外觀上的問題。</p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/issues/issue-information/update-issue-severity.md" class="MCXref xref"> 更新問題嚴重性</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL嚴重性]</td> 
   <td>請參閱本文中的「[!UICONTROL嚴重性]」。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL共用]</td> 
   <td>允許其他使用者在 [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROLSlack日期]</td> 
   <td>在任務視圖或報表中，[!UICONTROLSlack日期]顯示任務肯定會影響項目的[!UICONTROL完成日期]的確切日期。 有關任務的[!UICONTROLSlack日期]的資訊，請參見 <a href="../../../manage-work/tasks/task-information/task-slack-date.md" class="MCXref xref">任務Slack日期概觀</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL智慧分配]</td> 
   <td> <p>將任務或問題分配給用戶時， [!DNL Workfront] 根據最佳使用者完成工作的時間及其與專案的關係，提出建議（[!UICONTROL智慧指派]），以了解最佳使用者要完成工作的人。</p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/tasks/assign-tasks/smart-assignments.md" class="MCXref xref">智慧分配概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL源]</td> 
   <td> <p>指示另一個對象的父對象。 例如，附加到任務的文檔在[!UICONTROL文檔]報表或視圖的[!UICONTROL源]欄位中具有任務的名稱；在「問題」報表或檢視的[!UICONTROL來源]欄位中，專案下記錄的問題會包含專案名稱。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL開始日期]</td> 
   <td> <p>項目上的工作設定為開始的日期。 中有數個開始日期 [!DNL Workfront]: </p> 
    <ul> 
     <li>[!UICONTROL已計畫]</li> 
     <li>[!UICONTROL實際]</li> 
     <li>[!UICONTROL投影] </li> 
    </ul> <p>在[!UICONTROL比率報表]中，這是項目層職務角色的新開單率開始的日期。 在此日期之後與項目關聯的小時數乘以此開單比率，以計算項目收入。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL狀態]</td> 
   <td> <p>用於指示工作項目或戰略目標的工作流位置的指示器。</p> <p>對於項目，[!UICONTROL狀態]是項目上的設定，它指示項目是否為：</p> 
    <ul> 
     <li>[!UICONTROL當前]</li> 
     <li>[!UICONTROL保留] </li> 
     <li>[!UICONTROL完成] </li> 
     <li>[!UICONTROL死亡]</li> 
    </ul> <p>如需「專案狀態」的詳細資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md">訪問系統項目狀態清單</a>.</p>
    <p>對於任務，[!UICONTROL狀態]是任務上的設定，它指示任務是否為：</p> 
    <ul> 
     <li>[!UICONTROL新]</li> 
     <li>[!UICONTROL正在進行中]</li> 
     <li>[!UICONTROL完成]</li> 
    </ul> <p>有關「任務狀態」的詳細資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md">訪問系統任務狀態清單</a></p> <p>對於「問題」，[!UICONTROL狀態]是「問題」上的設定，指示此問題是否為：</p> 
    <ul> 
     <li>[!UICONTROL新]</li> 
     <li>[!UICONTROL正在進行中]</li> 
     <li>[!UICONTROL等待反饋]</li> 
     <li>[!UICONTROL保留]</li> 
     <li>[!UICONTROL已解析]</li> 
     <li>[!UICONTROL無法解決]</li> 
     <li>[!UICONTROL不能重複]</li> 
     <li>[!UICONTROL已驗證完成]</li> 
     <li>[!UICONTROL重新開啟]</li> 
    </ul> <p>如需問題狀態的詳細資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">訪問系統問題狀態清單</a>.</p> 
    <p>對於策略目標，[!UICONTROL狀態]是指明目標是否為：</p> 
     <ul> 
      <li>[!UICONTROL活動]</li> 
      <li>[!UICONTROL草稿]</li> 
      <li>[!UICONTROL非活動]</li> 
      <li>[!UICONTROL已關閉]</li> 
     </ul> 
     <p>如需有關戰略目標的詳細資訊，另請參閱本文中的「[!UICONTROL目標]」或「[!UICONTROL目標]」。 </p> 
     <p>對於策略目標，只有在您的組織已購買時，才會顯示此欄位 [!DNL Workfront Goals]. 如需使用管理策略目標的相關資訊 [!DNL Workfront Goals]，請參閱 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] 概述</a>. </p>
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL狀態更改]</td> 
   <td>[!UICONTROL稽核軌跡]。 當用戶更改項目、任務或問題的狀態時，將生成注釋。</td> 
  </tr> 
  <tr> 
   <td>狀態圖示</td> 
   <td> <p>您可以將內建的[!UICONTROL狀態表徵圖]欄位添加為視圖中的列，以增強對對象關鍵點的可見性，例如：</p> 
    <ul> 
     <li>對象附加了文檔</li> 
     <li>對象與批准過程相關聯</li> 
     <li>對象具有與其關聯的附加註釋</li> 
     <li>費用是可計費或可償還的 </li> 
     <li>任務位於關鍵路徑上</li> 
     <li>使用者屬於公司、團隊，或位於不同時區 </li> 
    </ul> <p>您可以在下列對象的視圖中添加[!UICONTROL狀態表徵圖]欄位： </p> 
    <ul> 
     <li>[!UICONTROL任務]</li> 
     <li>[!UICONTROL問題]</li> 
     <li>[!UICONTROL項目]</li> 
     <li>[!UICONTROL模板任務]</li> 
     <li>[!UICONTROL模板]</li> 
     <li>[!UICONTROL費用]</li> 
     <li>[!UICONTROL文檔]</li> 
     <li>[!UICONTROL用戶]</li> 
    </ul> <p>如需詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">檢視中的內建狀態圖示</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL狀態更新]</td> 
   <td> <p>此欄位顯示用戶在「[!UICONTROL更新狀態]」欄位中提供的最新狀態更新。 對狀態更新所做的注釋不會顯示在[!UICONTROL狀態更新]列中。</p> <p>要顯示「[!UICONTROL New]，」「[!UICONTROL In Process]，」和「[!UICONTROL Complete]」狀態，請使用[!UICONTROL Status]列。</p> <p>對狀態更新所做的注釋不會顯示在[!UICONTROL狀態更新]列中。</p> <p>如需狀態的詳細資訊，請參閱文章 <a href="../../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">更新任務狀態</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL狀態]</td> 
   <td>請參閱本文中的「[!UICONTROL狀態]」。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL情節提要]</td> 
   <td>代表故事狀態（敏捷方法中的任務）及其走向完成的圖表。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL營業時間]</td> 
   <td>用來測量動態的難度或複雜度的量度。 敏捷團隊可以選擇使用小時或點。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL故事點]</td> 
   <td>用來測量動態的難度或複雜度的量度。 敏捷團隊可以選擇使用小時或點。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Strategic]</td> 
   <td>改變組織或組織運作方式的長期工作。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL戰略協調]</td> 
   <td>衡量並協調不同產品組合和計畫的公司目標。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL訂閱者]</td> 
   <td> <p>訂閱專案、工作或問題的使用者。</p> <p>在報表中使用此欄位時，會顯示訂閱者清單，每個訂閱者以逗號分隔。</p> <p>如需詳細資訊，請參閱文章 <a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref">訂閱 [!DNL Adobe Workfront]</a>.</p> </td> 
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
   <td>[!UICONTROL系統控管]</td> 
   <td>一組管理系統更改和維護的策略。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL系統整合]</td> 
   <td>將不同的計算系統和軟體應用程式物理或功能連接在一起，以便作為一個協調的整體。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL任務]</td> 
   <td> <p>必須執行的活動，以達到最終目標（完成專案）。</p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/tasks/task-information/tasks-overview.md" class="MCXref xref">任務概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL任務屬性]</td> 
   <td>與任務關聯並指明任務某些詳細資訊的其他欄位或對象。 有些範例是[!UICONTROL計畫完成日期]和[!UICONTROL狀態]。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL任務約束]</td> 
   <td>請參閱「[!UICONTROL約束類型]」和「[!UICONTROL約束日期]」。</td> 
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
   <td> <p>致力於類似目標或業務目標的使用者集合。 通過將團隊分配給工作項目，這些用戶可以集體分配給工作項目。</p> <p>如需團隊的詳細資訊，請參閱 <a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref">團隊概觀</a>.</p> <p>專案可以有[!UICONTROL專案團隊]，其中包含與專案工作相關聯的所有使用者或角色。</p> <p>如需專案團隊的詳細資訊，請參閱 <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">專案團隊概觀</a></p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode,SnippetConitions_MaturityModel.Ad hoc"> 
    <td>Team Goals</td> 
    <td>Team goals which contribute to the metrics of enterprise or department goals.</td> 
   </tr>
  --> 
  <tr> 
   <td>[!UICONTROL模板]</td> 
   <td> <p>專案範本是最可重複專案的一般大綱。 建立項目模板時，您可以定義任務、隊列主題、自定義表單、附加文檔或批准，以在必須建立新項目時節省時間。 </p> <p>您可以將範本附加至現有專案，或使用範本建立新專案。 所有在範本上指定的資訊都會傳送給使用它建立的專案。 </p> <p>如需範本的詳細資訊，請參閱 <a href="../../../manage-work/projects/create-and-manage-templates/project-template-overview.md">專案範本概觀</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL模板任務]</td> 
   <td>屬於模板的任務。 模板任務成為使用模板建立的項目中的任務。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL線程]</td> 
   <td>[!UICONTROL注釋]及其與特定主題相關的答復集合。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL縮圖]</td> 
   <td> <p> 在[!UICONTROL文檔]清單或報告中，它會在縮略圖中顯示文檔的預覽。 </p> <p> 選擇 <strong>[!UICONTROL縮圖]</strong>  在報表中檢視33-66像素寬的縮圖。 </p> <p>當您修改清單或報表中的欄寬時，縮圖的大小會隨之調整。</p> <p>另請參閱本文中的「[!UICONTROL大縮圖]」。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL關閉時間]</td> 
   <td>您可以建立[!UICONTROL關閉時間]報表，以在使用者的設定檔中指出關閉時間時檢視。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL時間表]</td> 
   <td> <p>一種工時記錄卡，允許用戶輸入實際花費在項目、任務或問題上的小時數，或他們花費在與工作無關的其他活動（如會議或培訓）上的小時數。 除了輸入您花費在工作上的時間量外，您還可以使用「小時類型」來定義時間條目，以指明時間是與工作相關的時間，還是與間接費用時間相等。 有關工時單的資訊，請參見 <a href="../../../timesheets/timesheets/timesheets-overview.md">工時單概觀</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL時間表配置檔案]</td> 
   <td> <p>[!UICONTROL時間表配置檔案]是一個模板， [!DNL Workfront] 用於為與其關聯的用戶自動建立工時單。 </p> <p>您可以配置多個設定，這些設定將在建立時應用於每個時間表。 其中一些設定為：建立工時單的頻率（每週、每兩週、每月兩次或每月）、工時單的開始日、工時單批准者、可用的[!UICONTROL小時類型]（用戶可以與記錄的小時建立關聯）。</p> </td> 
  </tr> 
  <tr > 
   <td>[!UICONTROL上層父ID] </td> 
   <td> <p>此欄位可讓您識別和篩選清單或報表中頂層群組及其子群組的相關資料。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL頂級父代名稱] </td> 
   <td> <p>此欄位可讓您識別清單或報表中[!UICONTROL檢視]中頂級群組及其子群組的相關資料。</p> <p>您也可以使用[!UICONTROL上層父項ID]欄位來執行此操作。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL總小時數]</td> 
   <td> <p>在[!UICONTROL項目報表]中，此欄位顯示項目上所有小時的四捨五入總和，即上次計算項目財務的時間。 [!UICONTROL實際小時數]反映專案上記錄的確切小時數。 通常， [!UICONTROL實際小時數]應與[!UICONTROL總小時數]相符。 如果[!UICONTROL總小時數]與[!UICONTROL實際小時數]欄位顯著不同，則必須重新計算項目上的財務。</p> <p>有關重新計算項目財務的詳細資訊，請參閱文章 <a href="../../../manage-work/projects/project-finances/recalculate-project-finances.md" class="MCXref xref">重新計算項目財務</a>.</p> <p>在工時單[!UICONTROL Standard]視圖中，此欄位表示在工時單上顯示的日期中記錄物料的總小時數。 此內置視圖中時間表的[!UICONTROL總小時數]欄位引用「[!UICONTROL hoursDuration]」欄位，該欄位動態計算工時單起始日期和終止日期之間的小時數差異。 如果用戶記錄的時間超過時間表時間範圍內的可用時間，則此選項用於以紅色顯示[!UICONTROL總時數]列。 如需詳細資訊，請參閱 <a href="../../../timesheets/create-and-manage-timesheets/view-total-hours-timesheets.md" class="MCXref xref">查看工時單上的總小時數</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL追蹤模式]</td> 
   <td> <p>任務的屬性。 這決定了如何更新「任務」的「預計時間表」。 例如：</p> 
    <ul> 
     <li>[!UICONTROL用戶必須更新]要求手動更新任務。 否則，它將變成[!UICONTROL Bed Schedule]，然後變成[!UICONTROL Late]。</li> 
     <li>[!UICONTROL自動完成]將在到期日或[!UICONTROL計畫完成日期]過後自動完成任務。</li> 
    </ul> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">任務追蹤模式概觀</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL觸發器]</td> 
   <td>啟動情境的事件。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL故障任務]</td> 
   <td>條件為[!UICONTROL延遲]、[!UICONTROL延遲計畫]或[!UICONTROL面臨風險]的不完整任務。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL未分配的任務]</td> 
   <td>未分配給任何用戶、角色或團隊的任務。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL更新類型]</td> 
   <td> <p>項目上的設定，確定何時將重新計算項目的預計時間表。 選項包括：</p> 
    <ul> 
     <li>[!UICONTROL自動和更改時]</li> 
     <li>[!UICONTROL僅自動]</li> 
     <li>[！僅手動] </li> 
    </ul> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">選擇項目更新類型 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL用戶]</td> 
   <td>在 [!DNL Workfront] 允許人員登入並與系統互動。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL用戶委派]</p> </td> 
   <td> <p>可報告的對象，告訴您：</p> 
    <ul> 
     <li>哪些用戶已委派任務、問題和項目批准</li> 
     <li>哪些用戶具有委派給他們的任務、問題和項目批准</li> 
     <li>當這些代表團開始和結束時</li> 
    </ul> <p>若要進一步了解，請參閱 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md" class="MCXref xref">建立使用者委派報表</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL用戶介面]</td> 
   <td>的所有視覺和互動方面 [!DNL Workfront] 應用程式。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL用戶介面首選項]</td> 
   <td>[!UICONTROL用戶介面設定]。 [!DNL Workfront] 管理員可以變更這些設定以自訂使用者介面的各個方面。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL利用率]</td> 
   <td>根據分配的計畫、PTO和當前工作量的用戶或角色的可用性。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL用戶利用率]</td> 
   <td> <p>與報表結合的搜尋，可顯示如何分配或過度分配使用者（資源）。 請參閱本文中的「[!UICONTROL資源利用率]」。</p> </td> 
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
   <td>[!UICONTROL Velocity]</td> 
   <td>衡量工作週期總時間（完成工作所需時間）以及在最初承諾的時間內完成工作的頻率（工作與承諾的比率）。</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL視圖]</td> 
   <td> <p>檢視可用來修改報表或專案、工作或問題清單中的欄，或用來指出使用者僅有權檢視存取層級或權限共用層級的資訊。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL視圖表徵圖]</td> 
   <td> <p> 此欄位與「狀態圖示」相同，但僅適用於下列檢視： </p> 
    <ul> 
     <li> [!UICONTROL文檔] </li> 
    </ul> <p> 如需詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">檢視中的內建狀態圖示</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL上個月的視圖]</td> 
   <td> <p>在報表清單中，它會顯示上個月內檢視報表的次數。<br>如需報表清單中使用資訊的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">檢視報表使用量</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL上一季度的視圖]</td> 
   <td>在報表清單中，它顯示上一季度內檢視報表的次數。<br>如需報表清單中使用資訊的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" >檢視報表使用量</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL去年的查看次數]</td> 
   <td>在報表清單中，它會顯示去年內檢視報表的次數。<br>如需報表清單中使用資訊的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">檢視報表使用量</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL本月檢視]</td> 
   <td> <p>在報表清單中，它顯示該報表在本月被檢視的次數。<br>如需報表清單中使用資訊的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">檢視報表使用量</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL本季度查看]</td> 
   <td>在報表清單中，它顯示該季度內檢視報表的次數。<br>如需報表清單中使用資訊的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">檢視報表使用量</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL今年的觀看次數]</td> 
   <td>在報表清單中，它顯示今年內檢視報表的次數。<br>如需報表清單中使用資訊的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md">檢視報表使用量</a>.</td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL work]</code> </td> 
   <td> <p>在項目、任務或問題報表中，在文本模式下使用以下語句顯示項目、任務或問題的計畫時數：</p>
   <p></p><p></p> 
   <p>如需使用文字模式的相關資訊，請參閱 <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">文字模式語法概觀</a>. </p> 
   <p><b>筆尖</b> 
   <p>在問題報表中，新增[!UICONTROL計畫小時數]欄位中的一個，會新增 <code>work </code>欄位。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作]</td> 
   <td> <p>兩種主要許可證類型之一。 這比[!UICONTROL計畫]的訪問量小，但可以在系統中建立和更新。 這比[!UICONTROL External]、[!UICONTROL Reviewer]或[!UICONTROL Requesters]許可證類型更多。</p> <p>如需詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] 授權概述</a>.</p> <p>工作可能指專案、任務或問題的[!UICONTROL計畫小時數]。 有關詳細資訊，請參閱此表中的「[!UICONTROL工作]」欄位。 </p> <p>提示：在問題報表中，新增[!UICONTROL計畫小時數]欄位中的一個，會新增 <code>work </code>欄位。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作劃分結構]</td> 
   <td>要由項目團隊根據父/子關係執行的任務的層次結構。</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL工作] </td> 
   <td> 
    <p>項目經理可能決定使用此欄位，而不是[!UICONTROL計畫小時數]來估計完成任務所需的工作量。 只有在符合下列條件時，此欄位才會顯示：</p> 
     <ul> 
      <li> <p>該任務具有[!UICONTROL簡單持續時間類型]。 </p> <p>提示：如果將任務[!UICONTROL持續時間類型]更新為任何其他類型，則此欄位將變為隱藏。 </p> </li> 
      <li>項目經理已啟用[!UICONTROL使用工作]以自動計算項目上的任務[!UICONTROL計畫小時數]欄位。 </li> 
     </ul> 
     <p>有關使用[!UICONTROL工作成果]（而非[!UICONTROL計畫小時數]）來估計任務工作成果的資訊，請參閱 <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">工作成果概觀</a>. </p> 
     <p>您可以在任務報告和清單中顯示此欄位。</p> 
    </td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL工作項]</td> 
   <td> <p>此欄位是指 [!DNL Workfront]. </p> <p>[!UICONTROL工作項目]報表同時顯示任務和問題的資訊。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作管理組合]</td> 
   <td>[!UICONTROL工作績效指標](WPI)，指用於運行您的業務和更改您的業務的工作比例。 Mix WPI可協助您了解組織層級的策略是否套用了任何實際工作配置。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作管理資源]</td> 
   <td>系統中有資格接收工作或跟蹤時間的角色的指定。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作管理角色和責任]</td> 
   <td>定義所有者和利益相關方，以管理指定問題、任務、項目、計畫或產品組合的範圍、執行和批准。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作管理SLA]</td> 
   <td>所有利害關係人同意的可量化量度。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作管理利害關係人]</td> 
   <td>對工作請求結果具有既得利益的用戶集合。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作管理接觸點]</td> 
   <td>利害關係方之間溝通的數字化記錄。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作績效指標] </td> 
   <td> <p>混合比例、容量、速度、品質和參與。</p> <p>WPI是[!UICONTROL工作績效指標]的常見縮寫。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作流程]</td> 
   <td> <p>接收、排定優先順序和執行工作的方法。 您執行工作的方式通常稱為「工作流程」或「專案計畫」（含日期、前身關係等的任務清單）。 </p> <p>例如，生產單一資產或傳送多資產促銷活動。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作流模板]</td> 
   <td>在[!UICONTROL校樣核准]報表中，此欄位會顯示附加至校樣的任何工作流程範本。 如果沒有附加任何模板，則列為空。</td> 
  </tr>

<tr> 
   <td>[!UICONTROL工作時間]</td> 
   <td>

<p><span class="preview">表示用戶可用於實際工作（不包括間接費用）的等效全職時間([!UICONTROL FTE])的百分比。 [!UICONTROL工作時間]必須是十進位數字，最多1，不能是0。 例如，實際工作20%的可用性為0.2。</span>  </p>
   </p><span class="preview">欄位的預設值為1，表示使用者花費其整個[!UICONTROL FTE]在實際的專案相關工作上。</span>   </p>
   <p><span class="preview">系統使用此編號來計算用戶在實際項目相關工作中的可用性。 </span></p>
   <p> <span class="preview">排程例外和休假時間也可能影響使用者容量。</span> </p>
   <p><span class="preview">如需在Workfront中建立排程的詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">建立排程</a>.</span> </p>
    <p>Workfront會根據您的[!UICONTROL設定]區域中的「資源管理」首選項計算用戶的可用性。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md/">配置資源管理首選項</a>. </p> 
   <p><span class="preview">您可以在編輯或建立使用者時更新使用者的[!UICONTROL工作時間]。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">編輯使用者的設定檔</a></span></p> 
   <b>筆尖</b> 
   <p><span class="preview">將[!UICONTROL工作時間]值設為1，表示該用戶可用於與項目相關的整個全職工作。</span></p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作時間]</td> 
   <td>在Workfront檔案中，此辭彙用於根據排程說明分配給工作的時間。</td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL workRequiredExpression]</code> </td> 
   <td> <p>在項目、任務或問題報表中，在文本模式下使用以下語句顯示項目、任務或問題的計畫小時數，後跟「小時」一詞：</p>
   <p></p><p></p>
    <p>如需使用文字模式的相關資訊，請參閱 <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">文字模式語法概觀</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>
