---
content-type: reference
navigation-topic: workfront-navigation
title: 字彙表 [!DNL Adobe Workfront] 術語
description: 此 [!DNL Adobe Workfront] 字彙表列出Adobe Workfront中常用的術語。
feature: Get Started with Workfront
exl-id: 758072b3-775e-4771-9ae9-da0b38580c93
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '19720'
ht-degree: 0%

---

# 字彙表 [!DNL Adobe Workfront] 術語

>[!IMPORTANT]
>
>本文可作為參考，協助您瞭解以下文章中可能會提及的術語： [!DNL Adobe Workfront] 應用程式，在 [!DNL Workfront] 說明檔案，或一般而言是關於規劃和管理工作的檔案。 我們目前正在更新此資訊，因此此表格可能不完整。 當我們認為此資訊詳盡無遺時，我們會移除此免責宣告。

下表為Adobe Workfront中的常用辭彙清單：

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
   <td>[！UICONTROL存取層級]</td> 
   <td>決定使用者如何與Workfront中的不同物件和工具互動的使用者設定檔。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL作用中任務]</td> 
   <td>目前專案中未被前置任務阻止處理的未完成任務，且沒有具有未來計劃開始日期的任務限制。 換言之，這可以在今天使用。</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[！UICONTROL活動]</td> 
   <td>在 [!DNL Workfront Goals]，活動是目標的進度指示器。 它可以是您手動更新的進度列，或與目標相關聯的專案。 您無法在報告中顯示活動，也無法透過存取這些活動 [!DNL Workfront] API。 如需活動的相關資訊，請參閱 <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">開始使用Adobe Workfront目標中的結果和活動</a>.</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL實際成本]</td> 
   <td> <p>對於任務和問題，這是與記錄的實際時數關聯的成本，與指派給任務或問題的資源的每小時成本費率相關。 對於專案，這是專案上任務和問題中所有[！UICONTROL實際成本]的總和。 如需詳細資訊，請參閱 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">追蹤成本</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL實際費用成本]</td> 
   <td> <p>針對專案或任務記錄的所有費用的[！UICONTROL實際金額]總和。</p> <b>範例 </b>
   <p>如果您為任務1建立費用，並在[！UICONTROL實際金額]欄位中輸入$600.00，則此任務的[！UICONTROL實際費用成本]為$600.00。 </p> 
   <p>若為專案， [!DNL Workfront] 使用以下公式計算[！UICONTROL實際費用成本]：</p> <p><code>Project Actual Expense Cost = SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs) + Project Fixed Cost</code> <br> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (drafting this because not sure if this is still correct)</p>
    --> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL實際時數]</td> 
   <td> <p>在專案、任務或問題報表中，[！UICONTROL實際時數]為專案、任務或問題上記錄的所有時數總和。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span> 如果從「任務1」的[！UICONTROL更新]索引標籤中，按一下「記錄時間」並輸入25小時，則任務1的實際小時= 25小時。 </p> <p>[!DNL Workfront] 使用以下公式計算父系任務或專案的[！UICONTROL實際時數]：</p> 
    <ul> 
     <li> <p><code>For parent tasks = children [!UICONTROL Actual Hours] + [!UICONTROL Actual Hours] on the parent task. </code> </p> </li> 
     <li> <p><code>For projects = [!UICONTROL Actual Hours] logged on the project + [!UICONTROL Actual Hours] logged on standalone or children tasks in the project</code> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL實際勞力成本]</td> 
   <td> <p>與投資於任務或專案的人力相關的[！UICONTROL實際成本]。 </p> <p>若為工作， [!DNL Workfront] 使用下列公式計算[！UICONTROL實際勞力成本]：</p> <p><code>Task [!UICONTROL Actual Labor Cost] = Number of [!UICONTROL Actual Hours] on the task * User or Job Role [!UICONTROL Hourly Cost Rate]</code> </p> <p>如果任務的[！UICONTROL成本型別]為[！UICONTROL使用者小時]， [!DNL Workfront] 使用使用者費率。 如果任務的[！UICONTROL成本型別]為[！UICONTROL角色小時]， [!DNL Workfront] 使用工作角色費率來計算[！UICONTROL實際勞力成本]。 </p> <p>若為專案， [!DNL Workfront] 使用以下公式計算[！UICONTROL實際勞力成本]：</p> <p><code>Project [!UICONTROL Actual Labor Cost] = SUM(All Tasks [!UICONTROL Actual Labor Cost]) </code> </p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">追蹤成本</a>.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span>例如，如果使用者以[！UICONTROL使用者每小時] [！UICONTROL成本型別]為任務記錄5小時，且每小時費率為$100，則[！UICONTROL實際勞力成本]為$500。</p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL實際收入] </td> 
   <td> <p>專案或任務的[！UICONTROL實際收入]是指與專案或任務的[！UICONTROL實際時數]相關聯的金額。 </p> <p>如需有關追蹤收入的資訊，請參閱： [!DNL Workfront]，請參閱 <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">帳單與收入概要</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL實際開始]</td> 
   <td>當使用者變更指派給他們的工作中的進行中物件時的時間戳記。</td> 
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
   <td>[！UICONTROL Agile]方法</td> 
   <td>一種基於與跨職能團隊合作開發需求和解決方案的方法型別。 它鼓勵根據固定時間表進行彈性和變更。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL敏捷團隊]</td> 
   <td>與傳統團隊不同，因為他們從待處理專案取得潛在工作，並在稱為[！UICONTROL反複專案]的設定時間內處理。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL All My Teams]</td> 
   <td> <p>在[！UICONTROL篩選器]中參考此欄位時，此欄位會顯示屬於登入使用者所屬任何團隊的使用者，或指派給登入使用者所屬任何團隊的工作專案。 </p> <p>我們建議在篩選器中使用此欄位，讓報表在與其他使用者共用時更通用。 如此一來，您只能建置一個報表，該報表會根據登入檢視者的身分顯示不同資訊，因為資訊一律會為登入使用者自訂。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL配置日期]</td> 
   <td> <p>您可以在下列型別的報表中找到此欄位：</p> 
    <ul> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates</li>
     --> 
     <li>[！UICONTROL專案] （財務資料）</li> 
     <li>[！UICONTROL預算時數]</li> 
    </ul> <p>對於<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Resource Estimates or 
      </MadCap:conditionalText>
     -->[！UICONTROL專案（財務資料）]報表： </p> 
    <ul> 
     <li>嘗試瞭解時建立此報告 <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         how resources are budgeted for work, or 
       </MadCap:conditionalText>
      --> 指派給您資源的[！UICONTROL計畫時數]數量。</li> 
     <li> <p>[！UICONTROL Allocation Date]是一週中開始向任務分配[！UICONTROL Job Role]的第一天（星期日）。 資源（[！UICONTROL工作角色]）可以具有的[！UICONTROL配置日期]與指派給它的任務在[！UICONTROL持續時間]期間的周數相同。 如果任務跨越多個月，則當月的第一天也可能成為[！UICONTROL分配日期] （如果其在任務的[！UICONTROL期間]內）。</p> <p>例如，您可以將[！UICONTROL工作角色]指派給跨越3週且有90個[！UICONTROL計畫時數的任務。 這些時數在任務期間平均分佈，因此每天都會將6個[！UICONTROL計畫時數]指派給您的工作角色：</p> <p><em> [！UICONTROL每日計畫時數] = [！UICONTROL總計畫時數]/[！UICONTROL工作天數]在任務的[！UICONTROL期間] </em> </p> <p>因此，有三個[！UICONTROL配置日期]，在任務的[！UICONTROL期間，每個星期日的每個星期日各有一個日期，每個日期都與特定數量的[！UICONTROL規劃時數]相關聯。<br>如果任務在一個月的最後一週中旬開始，並在新月份開始後兩週結束，則任務將有四個[！UICONTROL配置日期]：一個用於任務期間[！UICONTROL每週的星期日，另一個用於新月份的第一天。</p> <p>若要充分利用此資訊，建議您建置 <!--
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          Resource Estimates or a 
        </MadCap:conditionalText>
       --> 專案（財務資料）報告並新增[！UICONTROL配置日期]的矩陣群組，然後每週、每月、每季或每年群組結果，以獲得最準確的資料。<br>如需建立矩陣群組的相關資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md" class="MCXref xref">建立矩陣報表</a>.</p> </li> 
    </ul> <p>只有當與其關聯的資料存在時間少於5年時，財務資訊才會填入[！UICONTROL專案（財務資料）]報表中。 例如，如果工作角色在2015年1月被分配給任務，而今天是2021年9月，則工作角色的[！UICONTROL分配日期]等財務欄位未填入[！UICONTROL專案（財務資料）]報表中。 </p> 
    <div> 
     <p>針對[！UICONTROL預算時數]報表：</p> 
     <ul> 
      <li>嘗試瞭解在資源規劃工具中分配給您的資源或您的專案的[！UICONTROL預算時數]金額時，請建立此報告。</li> 
      <li> <p>[！UICONTROL配置日期]是您在[！UICONTROL資源規劃工具]中編列時數預算的一週的第一天（星期日）。 </p> <p>秘訣：   <p>如果一週跨越兩個月，它會在報表中產生兩列：一個對應到一週的第一天（第一個月的第一週星期日），而第二列顯示第二個月的第一天。 </p> <p>例如，如果您將使用者在6月30日（星期日）至7月6日（星期六）這週的時間預算為8小時，則兩列會顯示6月30日和7月1日的[！UICONTROL配置日期]。 </p> </p> <p>如需有關預算資源的資訊，請參閱： [!DNL Resource Planner]，請參閱文章 <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">預算資源於 [!DNL Resource Planner] 使用[！UICONTROL Project]和[！UICONTROL Role]檢視</a>.</p> <p>如需有關建立[！UICONTROL預算時數]報表的資訊，請參閱 <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">報告：預算時數</a>. </p> </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL公告]</td> 
   <td> <p>在系統中與使用者通訊資訊的方式。 此資訊通常來自 [!DNL Workfront] 指派給管理員，或從管理員指派給使用者。 </p> <p>如需詳細資訊，請參閱 <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">傳送宣告</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL應用程式整合]</td> 
   <td>應用程式最常代表軟體應用程式的聯結器，但也代表操控資料的特殊功能。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL核准者決定]</td> 
   <td> <p>在[！UICONTROL校訂核准]報告中，此欄位顯示不再有效校訂的校訂核准決定。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL核准者階段]</td> 
   <td>在[！UICONTROL校訂核准報告]中，此欄位顯示校訂目前階段的相關資訊。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL核准]</td> 
   <td> <p>指定的工作專案（例如任務、檔案或時程表）可能要求主管或其他使用者登出該工作專案。 此登出程式稱為核准。 </p> <p>如需詳細資訊，請參閱 <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">核准流程概觀</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL核准日期]</td> 
   <td>在[！UICONTROL校訂核准]報告中，此欄位顯示核准校訂的日期。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL核准者]</td> 
   <td>必須登出指定工作專案的使用者或工作角色，或核準時程表上小時專案的使用者。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL指派至]</td> 
   <td> <p>在[！UICONTROL任務或問題]報告中，此欄位顯示任務或問題的擁有者，或[！UICONTROL主要受指派人]。 您也可以依此欄位篩選或分組。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL指定任務]</td> 
   <td>指派給問題或任務的使用者、工作角色或團隊。 專案、專案組合或方案不能有指派。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL指定任務]</td> 
   <td> <p>在[！UICONTROL任務]或[！UICONTROL問題]報告中，此欄位顯示指派給任務或問題的所有實體（使用者、工作角色、團隊）清單。 您可以使用欄位[！UICONTROL指派使用者]和[！UICONTROL指派角色]依此欄位進行篩選。 您可以使用「團隊」欄位按指派給任務或問題的團隊進行篩選。 您無法依此欄位將報表分組。</p> <p>已放置在[！UICONTROL資源回收筒]中的工作專案，將繼續顯示在參照[！UICONTROL工作分派]物件的某些報告中，其中 [!DNL OR] 篩選修飾元已使用。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL指派角色]</td> 
   <td>
   <p>在[！UICONTROL任務]或[！UICONTROL問題]報告中，此欄位顯示指派給任務或問題的工作角色的相關資訊。 此欄位會顯示[！UICONTROL主要擁有者]，以及指派給任務或問題的其他職務角色。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL指派狀態]</td> 
   <td> <p>在任務指派、任務或問題報告中，[！UICONTROL任務指派狀態]會顯示指派給工作專案的使用者是否已按一下[！UICONTROL處理該工作]或[！UICONTROL完成]按鈕接受或完成工作。 存在以下[！UICONTROL指派狀態]：</p> 
    <ul> 
     <li><b>[！UICONTROL已要求]</b>：使用者已指派至任務或問題，但他們尚未按一下[！UICONTROL處理它]按鈕以開始處理。</li> 
     <li><b>[！UICONTROL運作中]</b>：使用者已按一下[！UICONTROL處理它]按鈕，且目前正在處理該專案。 </li> 
     <li><b>[！UICONTROL完成]</b>：使用者已按一下[！UICONTROL完成]按鈕，並已完成其對專案的工作。 </li> 
    </ul> <p>如需詳細資訊，請參閱 <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/work-on-it-and-done-buttons-accept-complete-work.md" class="MCXref xref">[！UICONTROL Work On It]和[！UICONTROL Done]按鈕概述</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL指派團隊]</td> 
   <td>
   <p>在[！UICONTROL任務]或[！UICONTROL問題]報告中，此欄位顯示指派給任務或問題的團隊的相關資訊。 欄位會顯示[！UICONTROL主要擁有者]，以及指派給任務或問題的其他團隊。 </p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL指派使用者]</td> 
   <td>
   <p>在[！UICONTROL任務]或[！UICONTROL問題]報告中，此欄位顯示指派給任務或問題的使用者的相關資訊。 此欄位會顯示[！UICONTROL主要擁有者]，以及指派給任務或問題的其他使用者。 </p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL屬性]</td> 
   <td>屬性是 [!DNL Workfront] 物件。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL稽核區域]</td> 
   <td> <p>稽核是記錄Workfront中發生動作的系統訊息。 會記錄下列稽核型別：</p> 
    <ul> 
     <li>[！UICONTROL範圍變更]</li> 
     <li>[！UICONTROL附件動作]</li> 
     <li>[！UICONTROL一般編輯]</li> 
     <li>[！UICONTROL狀態變更]</li> 
     <li>[！UICONTROL附註]</li> 
     <li>[！UICONTROL組合專案]</li> 
     <li>[！UICONTROL錯誤專案]</li> 
     <li>[！UICONTROL狀態變更]</li> 
     <li>[！UICONTROL訂閱變更]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL稽核軌跡]</td> 
   <td>透過記錄變更（[！UICONTROL稽核區域]）追蹤的事件，自動產生的附註集合。 每個附註都會記錄誰執行了動作、他們執行了什麼動作，以及他們何時執行。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Automatic And On Change]</td> 
   <td> <p>[！UICONTROL專案更新]型別之一。 當每晚重新計算程式執行時，以及當對專案或專案內的任務進行任何更新時，這將會重新計算專案的預計和計畫時間表。 </p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">選取專案更新型別 </a>.</p> </td> 
  </tr>

<tr> 
   <td><p>可用性</p></td> 
   <td> <p>此辭彙與「使用者可用性」或「資源可用性」相關，說明資源（使用者或工作角色）可用的工作時間。 </p> 
   <p>Workfront會使用數個欄位並根據系統中資源管理偏好設定的設定，計算使用者可用性。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">設定資源管理喜好設定</a>. </p>
   <p>如需資源可用性的詳細資訊，請參閱 <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">開始使用資源管理</a></p>
   另外，「容量」也用來表示資源可用性。 
   </td> 
  </tr>

<tr> 
   <td>[！UICONTROL Automatic Only]</td> 
   <td> <p>[！UICONTROL專案更新]型別之一。 這會在每晚重新計算程式執行時，重新計算預計和計畫時間表。</p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">選取專案更新型別</a>.</p> </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[！UICONTROL BAU]</td> 
   <td>「照常營業」工作，有助於執行日常的主要業務目標。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL待處理專案]</td> 
   <td>敏捷環境中的區域，新問題會在這裡保留，直到它們準備好處理為止。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL基準線]</td> 
   <td>在敏捷環境中測量反複專案的資料來源。</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[！UICONTROL付費記錄]</td> 
   <td> <p>記錄可記帳的收入、時數或費用。 此資訊可用於在外部會計系統中建立商業發票。</p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/projects/project-finances/create-billing-records.md">建立付費記錄</a>. </p> 
   </td> 
  </tr>

<tr> 
   <td>付費記錄狀態</td> 
   <td> <p>在「記帳記錄」或「小時」報表中，記帳記錄的狀態會指出記帳記錄是否已記帳。 您無法刪除專案或編輯與已記帳記帳記錄相關聯的時間。 如需詳細資訊，請參閱 <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >建立付費記錄</a>.</p>  
   </td> 
  </tr>


<tr> 
   <td>[！UICONTROL品牌]</td> 
   <td><p>自訂程式 [!DNL Workfront] 讓介面具有使用您的顏色和標誌來映象您公司的外觀。</p><p><strong>注意</strong><br>如果您的組織已上線 [!DNL Adobe Experience Cloud]，品牌推廣無法使用。</p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL階層連結]</td> 
   <td> <p>頁面頂端的區域，顯示使用者在應用程式中的階層位置。</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">如需詳細資訊，請參閱 <a href="../../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">階層連結概觀</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL預算狀態]</td> 
   <td> <p>這是已棄用的欄位。 此欄位可能顯示的任何資訊都與以下功能相關： [!DNL Workfront] 已移除，欄位無法更新。 </p> <p>此欄位顯示專案是否已新增至[！UICONTROL Capacity Planner]，以及是否已為其完成預算計算。 [！UICONTROL Capacity Planner]已從中移除 [!DNL Workfront]. </p> 
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
   <td>[！UICONTROL預算完成日期]</td> 
   <td> <p>這是已棄用的欄位。 此欄位可能顯示的任何資訊都與以下功能相關： [!DNL Workfront] 已移除。 無法更新此欄位。 </p>
   <p> 此欄位仍會顯示在[！UICONTROL專案]和[！UICONTROL任務]報告和清單中。</p>  </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL預算成本]</td>

<td> <p>這是與專案的預算資源相關聯的成本。 </p>
   <p>此欄位會顯示在下列區域中 [!DNL Workfront] 下列名稱底下：</p>
   <ul>
   <li><strong>[！UICONTROL預算成本]</strong>：在[！UICONTROL業務案例摘要]面板中</li>
   <li><strong>[！UICONTROL成本]</strong>：在[！UICONTROL使用率]區域中按[！UICONTROL成本]檢視資訊時</li>
   <li><strong>[！UICONTROL專案預算成本]</strong>：在清單和報告中</li>
   </ul>   
    <p>使用下列公式計算專案的[！UICONTROL預算成本]：</p> 
    <p><code>[!UICONTROL Project Budgeted Cost] (or [!UICONTROL Budgeted Cost]) = [!UICONTROL Budgeted Expense Cost] + [!UICONTROL Budgeted Labor Cost] + [!UICONTROL Fixed Cost] of the project</code> </p> 
    <p>如需有關計算[！UICONTROL預算成本]的詳細資訊，並瞭解此概念的各種名稱： [!DNL Workfront]，請參閱 <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">計算專案預算成本</a>. </p>
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL預算時數]</td> 
   <td> <p>針對專案所需完成工作的資源預算時數。 此欄位是指專案或專案資源在[！UICONTROL業務案例] （或[！UICONTROL資源規劃工具]）的[！UICONTROL資源預算]區域中預算的時數。</p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">瞭解專案的[！UICONTROL預算勞力成本]和[！UICONTROL預算時數]</a>. </p> 
    <!-- 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Hours that were formerly budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner)</p>
    <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
  -->
    <p> 如需有關預算使用者在中的資訊 [!DNL Resource Planner]，請參閱文章 <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">預算資源於 [!DNL Resource Planner] 使用[！UICONTROL Project]和[！UICONTROL Role]檢視</a>. </p> 
    <p>[！UICONTROL業務案例]或[！UICONTROL資源規劃工具]的[！UICONTROL資源預算]區域中的預算時數顯示在以下區域中 [!DNL Workfront] 和下：</p> 
     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td><strong>[！UICONTROL預算時數]顯示名稱</strong></td> 
        <td><strong>區域 [!DNL Workfront]</strong></td> 
       </tr> 
       <tr> 
        <td>[！UICONTROL小時]</td> 
        <td>[！UICONTROL Business Case]的[！UICONTROL Resource Budgeting]區域</td> 
       </tr> 
       <tr> 
        <td>[！UICONTROL BDG]</td> 
        <td>[！UICONTROL資源規劃工具]，已由[！UICONTROL小時]檢視</td> 
       </tr> 
       <tr> 
        <td>[！UICONTROL預算時數]</td> 
        <td> <p>使用報告[！UICONTROL時數]檢視</p> <p>如需[！UICONTROL使用率]報表的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md" class="MCXref xref">[！UICONTROL資源使用率]報表概觀</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[！UICONTROL預算。 時數]</td> 
        <td> <p>[！UICONTROL預算時數]報告</p><p>「預算時數」報表中的[！UICONTROL預算時數]物件會參照與已棄用資源管理工具相關的資訊。 只有「[！UICONTROL預算」。 「時數」欄位在此報告中是指專案[！UICONTROL Business Case]之[！UICONTROL資源規劃工具]或[！UICONTROL資源預算]區域中的預算時數。 </p> <p>如需建立報告的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">建立自訂報表</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[！UICONTROL資源規劃工具預算時數] </td> 
        <td> <p>可在下列報表中找到：</p>
        <ul>
        <li>[！UICONTROL專案]報告
        <li>[！UICONTROL專案（財務資料）]報表
        <li>[！UICONTROL任務]報告
        <li>[！UICONTROL問題]報告
        <li>[！UICONTROL預算時數]報告</li>
        </ul>
         <p>如需建立報告的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">建立自訂報表</a>.</p> </td> 
       </tr> 
      </tbody> 
     </table> 
    <p>中對[！UICONTROL預算時數]的任何其他提及 [!DNL Adobe Workfront] 請參閱使用已從Workfront移除之已棄用功能的預算時數。 這些是僅供檢視的欄位，當您使用目前的資源預算工具時，不會更新為目前的資訊。 </p>
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
   <td>[！UICONTROL預算勞力成本]</td> 
   <td> <p>這是與您作為資源管理員針對工作角色在專案上需要完成的工作預算的時數相關聯的成本。 </p> <p>使用下列公式計算專案報表中的[！UICONTROL預算勞力成本]：</p> <p><code style="font-style: normal;">[!UICONTROL Budgeted Labor Cost] = SUM([!UICONTROL Job Role Cost] per [!UICONTROL Hour] * [!UICONTROL Budgeted Hours] per [!UICONTROL Job Role])</code> </p> <p>此欄位可能參考以下內容：</p> 
    <ul> 
     <li> <p>顯示在[！UICONTROL Business Case]的[！UICONTROL Resource Budgeting]區域或[！UICONTROL Resource Planner]中與專案中工作角色成本相關的人工成本。 如需有關計算[！UICONTROL預算勞力成本]的資訊，請參閱文章 <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">[！UICONTROL瞭解專案的預算勞力成本]和[！UICONTROL預算時數]</a></p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>顯示在[！UICONTROL Business Case]的[！UICONTROL Resource Budgeting]區域中的勞力成本，反映了從連結至專案的方案中所估算的[！UICONTROL人員成本] [!DNL Scenario Planner] 當您使用「案例規劃工具」來預算專案資源時。 如需方案的相關資訊，請參閱 <a href="../../../scenario-planner/initiatives-overview.md" class="MCXref xref">情境規劃工具中的方案概觀</a>. </p> <p>此 [!DNL Scenario Planner] 需要額外的授權。 如需關於以下專案的資訊： [!DNL Workfront Scenario Planner]，請參閱 <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">此 [!DNL Scenario Planner] 概觀</a>. </p> </li> 
     <p>它顯示在下列名稱的下列區域：</p>
   <ul>
   <li><strong>[！UICONTROL預算勞力成本]</strong>：在[！UICONTROL Business Case]的[！UICONTROL Resource Budgeting]區域中。
   <li><strong>[！UICONTROL預算成本]</strong>：在[！UICONTROL使用率]報表[！UICONTROL成本]檢視中
   <p>如需詳細資訊，請參閱 <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">檢視資源使用率資訊 </a>.</p>
   <li><strong>[！UICONTROL BDG]</strong>：在 [!DNL Resource Planner] 專案或 [!DNL Role] 檢視，依成本檢視時
   <li><strong>[!DNL Resource Planner Budgeted Labor Cost]</strong>：在以下報表中： 
   <ul>
    <li>[！UICONTROL專案]報告</li>
    <li>[！UICONTROL專案（財務資料）]報表</li>
    <li>[！UICONTROL任務]報告</li>
    <li>[！UICONTROL問題]報告</li>
    <li>[！UICONTROL預算時數]報告</li> 
    </ul>
    <p>如需建立報告的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">建立自訂報表</a>.</p>
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
   <td>[！UICONTROL預算開始日期]</td> 
  <td> <p>這是已棄用的欄位。 此欄位可能顯示的任何資訊都與以下功能相關： [!DNL Workfront] 已移除。 無法更新此欄位。</p>
  <p>這些區域已從中移除 [!DNL Workfront]. </p> 
  <p>該欄位仍然顯示在[！UICONTROL專案]和[！UICONTROL任務]報告和清單中。</p>
   <!--
   <p>This field shows the date when the budgeting of resources starts, as defined in the Legacy Resource Estimates area of the Business Case of a project, or the Capacity Planner.</p>
   -->   
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL待執行工作圖表]</td> 
   <td>折線圖，提供已完成及剩餘工作的視覺化表示法。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL商業案例]</td> 
   <td> <p>評估專案是否應從[！UICONTROL Idea]狀態前移至[！UICONTROL Planning]狀態的工具。 換句話說，[！UICONTROL業務案例]可協助組織決定是否值得啟動及完成專案，尤其是將專案與投資組合中的其他專案進行比較時。</p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">為專案建立[！UICONTROL業務案例] </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL業務案例預算時數]</td> 
   <td> <p>這是已棄用的欄位。 此欄位可能顯示的任何資訊都與以下功能相關： [!DNL Workfront] 已移除。 無法更新此欄位。</p> <p>此欄位仍會顯示在專案和[！UICONTROL工作]清單及報告中。 </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL計算工作分派]</td> 
   <td> <p>任務[！UICONTROL工期]型別之一。 這將會根據任務的[！UICONTROL持續時間]和[！UICONTROL所需工作]計算指派給任務的使用者在8小時工作日中分配給任務的百分比。</p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任務[！UICONTROL工期]和[！UICONTROL工期型別]概觀</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL計算工時]</td> 
   <td> <p>[！UICONTROL期間型別]任務之一。 考慮到[！UICONTROL持續時間]和使用者[！UICONTROL指派]百分比（以8小時工作日為基礎），這將會計算任務的[！UICONTROL所需工時]。</p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任務[！UICONTROL工期]和[！UICONTROL工期型別]概觀</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL行事曆]</td> 
   <td> <p>中有兩種行事曆型別 [!DNL Workfront]：[！UICONTROL首頁行事曆]和行事曆報表。</p> <p>[！UICONTROL首頁行事曆]是個人行事曆，可讓使用者根據以下時間內的可用時數管理其工作量： [!DNL Workfront]. 使用者也可以將其[！UICONTROL首頁行事曆]與 [!DNL Outlook] ([!DNL Google] 和 [!DNL Microsoft] 整合即將推出)。 </p> <p>如需[！UICONTROL首頁行事曆]的詳細資訊，請參閱 <a href="../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md" class="MCXref xref">[！UICONTROL首頁行事曆]檢視</a>.</p> <p>行事曆報告是一種動態報告，使用者可以在其中檢視事件的日期和其他重要詳細資訊，包括到期日、工作狀態以及事件指派給的使用者。</p> <p> 如需行事曆報告的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md" class="MCXref xref">行事曆報表概觀</a>.</p> </td> 
  </tr> 
   <tr> 
   <td>[！UICONTROL可以開始]</td> 
   <td> <p>此欄位指出任務是否已準備好開始處理。 如果開始工作已準備就緒，可在任務的[！UICONTROL可以開始]欄位上工作，則會將設定為[！UICONTROL True]。 </p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/tasks/task-information/can-start-task-overview.md" class="MCXref xref">任務的「[！UICONTROL可以開始]」概觀</a>.</p> 
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
   <td> <p>資源可供配置進行工作的可用時間。 請參閱可用性。 </p></td> 
  </tr>

<tr> 
   <td> <p>[！UICONTROL類別]</p> </td> 
   <td> <p>類別是自訂表單。 您可以建立此物件的報表，也可以在其他物件報表中顯示。 並非所有物件都有自訂表單或類別。 下列物件可以有自訂表單： <br></p> 
    <ul> 
     <li>[！UICONTROL專案]</li> 
     <li>[！UICONTROL任務]</li> 
     <li>[！UICONTROL問題]</li> 
     <li>[！UICONTROLPortfolio]</li> 
     <li>[！UICONTROL檔案]</li> 
     <li>[！UICONTROL費用]</li> 
     <li>[！UICONTROL程式]</li> 
     <li>[！UICONTROL使用者]</li> 
     <li>[！UICONTROL公司]</li> 
     <li>[！UICONTROL反複專案]</li></ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL類別名稱]</td> 
   <td> <p>當作為欄新增到下列任何物件的檢視中時，它會顯示與這些物件相關聯的所有自訂表單清單：</p> 
    <ul> 
     <li>[！UICONTROL專案]</li> 
     <li>[！UICONTROL任務]<br></li> 
     <li>[！UICONTROL問題]<br></li> 
     <li>[！UICONTROLPortfolio]<br></li> 
     <li>[！UICONTROL檔案]<br></li> 
     <li>[！UICONTROL費用]<br></li> 
     <li>[！UICONTROL程式]<br></li> 
     <li>[！UICONTROL使用者]<br></li> 
     <li>[！UICONTROL公司]</li> 
     <li>[！UICONTROL反複專案]</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL變更管理]</td> 
   <td>練習領域專注於定義、瞭解計畫工作，並根據範圍、排程、成本和資源因素的變化進行調整。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL變更順序]</td> 
   <td>針對概述已同意範圍之變更請求的專案提出的一種問題型別。</td> 
  </tr> 
  <tr> 
   <td>僅限[！UICONTROL變更]</td> 
   <td>其中一個專案[！UICONTROL更新型別]。 它只會在對專案或任務執行任務更新或編輯時更新[！UICONTROL專案預計]和[！UICONTROL計畫]時間表。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL變更順序]</td> 
   <td> <p>[！UICONTROL Issue]型別之一，通常表示專案完成之前必須完成未計畫的工作量。</p> <p>如需[！UICONTROL Issue]型別的詳細資訊，請參閱文章中的「預設問題型別」一節 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md" class="MCXref xref">自訂預設問題型別</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL子任務]</td> 
   <td>屬於[！UICONTROL父系任務] （[！UICONTROL摘要任務]）的[！UICONTROL子任務]。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL子項]</td> 
   <td>[！UICONTROL子任務]至[！UICONTROL父任務] （[！UICONTROL摘要任務]）的集合。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Coaching]和[！UICONTROL Training]</td> 
   <td>學習模組、認證、標準或實踐社群。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL認可]</td> 
   <td>一種通訊工具，可供使用者設定對任務交付專案的期望。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL認可日期]</td> 
   <td>一種通訊工具，可供使用者設定對任務交付專案的期望。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Communication]和[！UICONTROL Reporting]</td> 
   <td>複查專案、方案或投資組合例外狀況與健康狀況的標準</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL公司]</td> 
   <td> <p>[！UICONTROL公司]是中的組織單位 [!DNL Workfront]. </p> 
   <p> 您可以將使用者或專案與一家公司建立關聯。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md">建立和編輯公司</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL完成日期]</td> 
   <td> <p>專案、任務或問題設定為完成的日期。 中有數種型別的[！UICONTROL完成日期] [!DNL Workfront]：</p> 
    <ul> 
     <li>[！UICONTROL實際完成日期]。 如需詳細資訊，請參閱 <a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">專案[！UICONTROL實際完成日期]概觀 </a>.</li> 
     <li>[！UICONTROL規劃完成日期]。 如需詳細資訊，請參閱 <a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">設定專案[！UICONTROL計畫完成日期]</a> 和 <a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">任務總覽[！UICONTROL規劃完成日期]</a>.</li> 
     <li>[！UICONTROL預計完成日期]。 如需詳細資訊，請參閱 <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">專案、任務和問題的[！UICONTROL預計完成日期]概觀</a>.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL完成日]</td> 
   <td>相對於[！UICONTROL範本]的開始日期，[！UICONTROL範本任務]或[！UICONTROL範本]應該已完成。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL完成模式]</td> 
   <td> <p>這會指出如何將專案標示為[！UICONTROL完成]。 它可以有兩個值：</p> 
    <ul> 
     <li>[！UICONTROL手冊]：使用者必須將專案狀態變更為[！UICONTROL完成]。</li> 
     <li>[！UICONTROL自動]：當專案中的所有任務完全完成且所有問題都已關閉時，專案狀態將自動變更為[！UICONTROL完成]。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL條件]</td> 
   <td> <p>這是任務、問題或專案進度的視覺化表示。</p> <p>對於專案，條件可由專案所有者手動設定，或可由自動設定 [!DNL Workfront]，根據專案的進度狀態而定。 </p> <p>專案狀態的可能值包括：</p> 
    <ul> 
     <li>[！UICONTROL On Target]</li> 
     <li>[！UICONTROL有風險]</li> 
     <li>[！UICONTROL陷入困境]</li> 
    </ul> <p>如需有關專案狀況的詳細資訊，請參閱文章 <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">[！UICONTROL專案條件]和[！UICONTROL條件型別]概觀</a>.</p>
     <p>您可以將任務和問題條件與可顯示在報告中的數字建立關聯。 以下清單顯示任務和問題條件的預設名稱和編號。 您的系統管理員可以更新條件的名稱，並且可以新增具有不同號碼的條件。 數字與條件相關聯後，即無法編輯。  </p> 
     <p>對於任務，條件由任務所有者手動設定。 工作條件的可能值包括：</p> 
    <ul> 
     <li>[！UICONTROL進展順利] (0)<br></li> 
     <li> [！UICONTROL一些問題] (1)<br></li> 
     <li>[！UICONTROL主要障礙] (2)</li> 
    </ul> <p>如需工作條件的詳細資訊，請參閱文章 <a href="../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">更新任務和問題的[！UICONTROL條件]</a>.</p> <p>對於問題，條件由問題所有者手動設定。 問題條件的可能值包括：<br></p> 
    <ul> 
     <li>[！UICONTROL進展順利] (0)<br></li> 
     <li>[！UICONTROL一些問題] (1)<br></li> 
     <li>[！UICONTROL主要障礙] (2)</li> 
    </ul> 
   <p><b>附註</b></p>
    <p>在[！UICONTROL Journal Entry]報告中追蹤[！UICONTROL Condition]欄位時，[！UICONTROL New]和[！UICONTROL Old Number Values]會顯示與條件相關的編號，而不是其名稱。 如果最初未為任務或問題定義條件，而您稍後更新了該條件，則擷取更新的日誌專案會將[！UICONTROL條件]欄位的[！UICONTROL舊編號值]顯示為 — 2,147,483,648。 另請參閱本文中的「[！UICONTROL新數字值]」、「[！UICONTROL舊數字值]」和「[！UICONTROL日誌專案]」。 </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL條件更新]</td> 
   <td> <p>此欄位顯示任務、專案或問題的目前狀況。 此選項會顯示任務、專案或問題的擁有者在[！UICONTROL更新狀態]欄位中提供的最新更新，以及新條件。</p> <p>條件更新的註解不會顯示在[！UICONTROL Condition Update]欄中；只會顯示主要更新。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL限制日期]</td> 
   <td> <p>如果您使用與特定日期繫結的[！UICONTROL任務限制]，例如[！UICONTROL必須開始於]，則該特定日期會成為任務的[！UICONTROL限制日期]。</p> <p>下列任務限制會更新[！UICONTROL限制日期]欄位：</p> 
    <ul> 
     <li>[！UICONTROL必須開始於]</li> 
     <li>[！UICONTROL必須完成日期]</li> 
     <li>[！UICONTROL開始時間不晚於]</li> 
     <li>[！UICONTROL開始時間不早於]</li> 
    </ul> <p>秘訣：   
     <ul> 
      <li> <p>[！UICONTROL條件約束]為[！UICONTROL固定日期]的任務沒有[！UICONTROL條件約束日期]。 </p> </li> 
      <li> <p> [！UICONTROL限制日期]只能在報表或自訂檢視中檢視。</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL限制日]</td> 
   <td> <p>如果您在繫結至特定日期的範本任務中使用任務限制，例如必須開始日期，則該特定日期會成為範本任務的「限制日期」。</p> <p>下列任務限制會更新[！UICONTROL限制日]欄位：</p> 
    <ul> 
     <li>[！UICONTROL必須開始於]</li> 
     <li>[！UICONTROL必須完成日期]</li> 
     <li>[！UICONTROL開始時間不晚於]</li> 
     <li>[！UICONTROL開始時間不早於]</li> 
    </ul> <p>秘訣： [！UICONTROL限制日]只能在報表或自訂檢視中檢視。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL條件約束型別]</td> 
   <td> <p>任務的排程趨勢。 例如，[！UICONTROL儘快]將排程任務以儘快開始，[！UICONTROL完成時間不晚於]將排程任務以在[！UICONTROL限制日期]之前完成，並且不晚於。</p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">[！UICONTROL任務限制]概觀</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL內容功能表]</td> 
   <td>一個選單，位於熒幕左側，專案會在該選單上變更以與活動內容相關聯。 例如，當使用者檢視專案時，[！UICONTROL內容功能表]將顯示專案相關資訊和工具的連結。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL轉換的問題建立者]</td> 
   <td>專案或任務報告中的欄位，顯示當問題轉換為專案或任務時，問題主要連絡人[！UICONTROL]使用者的相關資訊。 此欄位也會顯示在[！UICONTROL專案詳細資訊]區段中，其中顯示轉換問題之[！UICONTROL主要連絡人]的名稱。 另請參閱本文中的「[！UICONTROL主要聯絡人]」。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL成本]</td> 
   <td> <p>完成專案、任務或問題時必須花費的金額。 </p> <p>您可以針對與專案相關的人力、費用和風險追蹤各種成本型別。如需有關追蹤成本的資訊，請參閱： [!DNL Workfront] 另請參閱 <a href="../../../manage-work/projects/project-finances/track-costs.md">追蹤成本</a>.</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL成本型別]</td> 
   <td>對於任務，[！UICONTROL成本型別]會決定任務累積成本的方式。 某些範例包括[！UICONTROL固定小時]、[！UICONTROL使用者小時]和[！UICONTROL使用者小時加固定]。 </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL跨專案相依性]</td> 
   <td> <p>一個專案的任務相依於不同專案中的任務。</p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref">建立跨專案前置任務</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL自訂資料]</td> 
   <td> <p>組織特有的資料。 組織可以自訂 [!DNL Workfront] 建立自訂表單和自訂欄位。 此自訂資訊可推動KPI、稽核和需求混合的報表。 </p> <p>[！UICONTROL自訂資料]可以連結至：</p> 
    <ul> 
     <li>[！UICONTROL專案]</li> 
     <li>[！UICONTROL工作]</li> 
     <li>[！UICONTROL使用者]</li> 
     <li>[！UICONTROL公司]</li> 
     <li>[！UICONTROL問題]</li> 
     <li>[！UICONTROL檔案]</li> 
     <li>[！UICONTROL費用]</li> 
     <li>[！UICONTROLPortfolio]</li> 
     <li>[！UICONTROL程式]</li> 
     <li>[！UICONTROL反複專案]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL自訂資料型別]</td> 
   <td>用於指定[！UICONTROL自訂資料]欄位是否以文字、日期、數字或貨幣形式儲存在資料庫中的選項。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL自訂顯示型別]</td> 
   <td>自訂欄位的欄位顯示型別。 範例包括[！UICONTROL下拉式清單]、[！UICONTROL文字欄位]、[！UICONTROL文字區域]、[！UICONTROL選項按鈕]等。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL自訂欄位]</td> 
   <td>對於允許使用者從多個選項中選擇的自訂資料，這些是使用者可以從中選擇的值。 自訂選項僅在[！UICONTROL下拉式清單]、[！UICONTROL多選下拉式清單]、[！UICONTROL選項按鈕]和[！UICONTROL核取方塊]上有效。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL自訂表單標籤]</td> 
   <td>當使用具有自訂選項的自訂顯示型別時，這是將顯示在下拉選單、核取方塊或該自訂選項的單選按鈕中的使用者介面文字。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL自訂值]</td> 
   <td>搭配使用自訂欄位和自訂選項時，此值會針對特定選項儲存在資料庫中。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL自訂檢視]</td> 
   <td>針對清單中的每個物件所顯示的資料欄位或欄的定義。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL客戶]</td> 
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
   <td>[！UICONTROL儀表板]</td> 
   <td> <p> 您可以在報告或報告物件清單中新增此欄位，以顯示報告列在清單中的儀表板。 </p> <p> 您也可以使用此欄位來篩選列在特定控制面板上的報告。 </p> <p> 如需在報表物件報表中加入儀表板資訊的詳細資訊，請參閱文章中的「瞭解哪些報表列在儀表板上」一節 <a href="../../../reports-and-dashboards/reports/report-usage/access-organize-reports.md" class="MCXref xref">存取及組織報告</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL資料型別]</td> 
   <td>請參閱「[！UICONTROL自訂資料型別]」。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL延遲天數]</td> 
   <td> <p>如果缺少[！UICONTROL實際完成日期]，此欄位會顯示[！UICONTROL規劃開始]與[！UICONTROL今天]之間的日期差異。</p> <p>此外，也會在出現[！UICONTROL實際完成日期]時，顯示[！UICONTROL實際完成]與[！UICONTROL規劃完成]之間的日期差異。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[！UICONTROL預設排程]</td> 
   <td> <p>可自訂的預設工作時數，可指派給組織內的使用者和專案。 </p> <p>排程用於計算指派給使用者的任務的計畫、開始和完成日期。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[！UICONTROL交付專案]</td> 
   <td>專案完成時必須提供的可量化的商品或服務。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[！UICONTROL Demand Management]</td> 
   <td>攝入流程的評分和優先順序。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[！UICONTROL部門目標]</td> 
   <td>特定部門專屬的目標，著重於改善該部門內的營運量度。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL相依性]</td> 
   <td>兩個任務之間的連結，其中一個任務需要先變更狀態，另一個任務才能變更狀態。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL相依性型別]</td> 
   <td> <p>任務與其前置任務之間的排程關係型別。 例如[！UICONTROL Finish-Start]，它要求第一個任務必須先完成，第二個任務才能開始。</p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md" class="MCXref xref">任務相依性型別的概要</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL檔案]</td> 
   <td>任何附加到中物件的檔案 [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL檔案版本]</td> 
   <td> <p>每次將相同的檔案上傳到相同的物件時，都會為其指派一個版本編號。 使用者可以檢視和變更舊版檔案的多個選項。</p> <p>如需詳細資訊，請參閱 <a href="../../../documents/managing-documents/manage-document-versions.md" class="MCXref xref">管理檔案版本</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[！UICONTROL持續時間]</td> 
   <td> <p>分配完成任務問題或專案的時間視窗（由[！UICONTROL計劃開始]與計畫完成之間的天數決定）。</p> 
    <ul> 
     <li>對於任務，如果任務的期間型別不是簡單，則期間是可編輯的欄位。 如果任務的「工期型別」為「簡單」，或如果任務限製為「固定日期」，則「工期」是由Workfront執行的計算。</li> 
     <li>對於問題，「持續時間」始終是可編輯的欄位，應表示需要解決問題的預估天數。</li> 
     <li>對於專案而言，「持續時間」是以下人員執行的計算 [!DNL Workfront] 且代表最早任務的規劃開始與專案上最新任務的[！UICONTROL規劃完成]之間的天數差異。</li> 
    </ul> <p>如需有關任務的[！UICONTROL持續時間]與[！UICONTROL計畫持續時間]之間差異的詳細資訊，請參閱文章 <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md">[！UICONTROL計畫持續時間]與任務的[！UICONTROL持續時間]之間的差異</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[！UICONTROL持續時間（分鐘）]</td> 
   <td>此欄位顯示與[！UICONTROL Duration]欄位相同的資訊（以分鐘為單位，而非天數）。 </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc,QuicksilverOrClassic.Quicksilver"> 
   <td>[！UICONTROL每次發生的持續時間]</td> 
   <td> <p>這會顯示在遞回任務之父級的[！UICONTROL任務詳細資訊]和[！UICONTROL編輯任務]方塊中。 它會顯示每個遞回任務的持續時間。 如需建立週期性工作的相關資訊，請參閱 <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">建立週期性任務</a>. </p> <p> <span>在個別週期性任務中修改的持續時間不顯示此欄位中指示的值。</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[！UICONTROL期間型別]</td> 
   <td> <p>一個工作列位，指明完成任務所需的工作如何在整個任務期間內分配給受指派人。 它表示任務的[！UICONTROL持續時間]、[！UICONTROL所需工作]與指派的資源應花費在任務完成的時間量或[！UICONTROL配置]之間的關係。 </p> <p>此欄位會顯示在任務的[！UICONTROL詳細資訊]索引標籤上。 </p> <p>選項包括：</p> 
    <ul> 
     <li>[！UICONTROL計算工作分派]</li> 
     <li>[！UICONTROL計算工時]</li> 
     <li>[！UICONTROL投入比導向]</li> 
     <li>[！UICONTROL簡單]</li> 
    </ul> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任務[！UICONTROL工期]和[！UICONTROL工期型別]概觀</a>.</p> 
    —&gt; </td> 
   </tr> 
   <tr> 
   <td>[！UICONTROL持續時間單位]</td> 
   <td>在電源搜尋中用來測量時間的單位。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL投入比導向]</td> 
   <td>使用者人數與完成任務所需時間之間的關係。 當您新增更多使用者時，排定完成任務的總時間會減少，但任務的持續時間會維持不變。 例如，如果一項任務正在炮製一桶花生，則新增更多人員將會減少排程時間，但人日中的持續時間將保持不變。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL經過時間]</td> 
   <td> <p>[！UICONTROL經過時間]是任務的[！UICONTROL持續時間]的時間單位。 此時間介於任務的[！UICONTROL計劃開始日期]和[！UICONTROL計畫完成日期]之間，其中包含假日、週末和休假。 換言之，經過的時間就是行事曆的天數。 </p> <p>[!DNL Workfront] 支援下列任務持續時間的經過時間單位：</p> 
    <ul> 
     <li> <p>[！UICONTROL經過的分鐘數]</p> </li> 
     <li> <p>[！UICONTROL經過小時數]</p> </li> 
     <li> <p>[！UICONTROL經過的天數]</p> </li> 
     <li> <p>[！UICONTROL經過的周數]</p> </li> 
     <li> <p>[！UICONTROL經過月數]</p> </li> 
    </ul> <p>如需任務持續時間的詳細資訊，包括經過的時間，請參閱 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任務[！UICONTROL工期]和[！UICONTROL工期型別]概觀</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL結束日期]</td> 
   <td> <p> 在[！UICONTROL費率]報表中，這是專案層級工作角色的新計費率結束的日期。 在此日期之前與專案相關聯的時數，會乘以此收費率，以計算專案上的收入。 </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[！UICONTROL參與]</td> 
   <td>[！UICONTROL工作績效指標] (WPI)指出對任務、專案、團隊或組織的承諾與信賴何時減弱。 這表示您需要採取行動，以恢復該信念和承諾。 WPI的測量方式會透過以下簡單的問題來進行：「您是否瞭解期望您做什麼？ 您被指派的工作對組織是否有影響？ 你工作出色嗎？」</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[！UICONTROL企業目標]</td> 
   <td>有助於公司目標量度的跨職能目標。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL事件]</td> 
   <td>專案或任務中的任何變更。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL事件處理常式]</td> 
   <td>事件發生時發生的自動化工作。 常見的範例是自動化電子郵件通知。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL事件通知]</td> 
   <td>從事件處理常式產生的電子郵件。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[！UICONTROL費用]</td> 
   <td>任務或專案的非勞力成本。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL外部]</td> 
   <td> <p>通常是授權型別，或具有此類授權的使用者，只能檢閱系統中的資訊。</p> <p>如需詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] 授權總覽</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL外部系統]</td> 
   <td>在指定的記錄系統之外儲存和管理的任何服務或軟體。</td> 
  </tr>

<tr> 
   <td>[！UICONTROL欄位]</td> 
   <td><p>任何Workfront物件或與其相關聯的資訊（如顯示在資料庫中的資訊）。 </p>
   <p>例如，「project」、「user」、「hour」都是Workfront物件及欄位。 「名稱」、「狀態」、「擁有者」、「開始日期」是與上述物件相關聯的Workfront欄位。 </p>

<p>在參照物件時，可以互換使用「物件」和「欄位」等字詞。</p>
   <p>在報表範圍內，「欄位」是指您要在報表中擷取的物件或物件相關資訊。</p>

<p><b>附註</b></p>

<p>在文字更多報表中，欄位會參照物件或物件在資料庫中顯示的資訊。</p>
   <p>有時，您在使用者介面中看到的名稱與資料庫中欄位的名稱不同。 例如，「issue」是Workfront介面中的物件名稱，而「opTask」是Workfront資料庫中的物件（或欄位）名稱。 </p> 
   <p> 在撰寫文字模式報告、檢視、篩選或分組或建立計算欄位時，請務必使用顯示在資料庫中的欄位。</p>

<p>如需詳細資訊，請參閱 <a href="../../../wf-api/general/api-explorer.md">API總管</a> 和 <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md">文字模式概觀</a>.</p>

<p>依預設，Workfront隨附一組定義物件及其資訊的欄位。 您也可以建立自訂欄位來定義物件，但無法建立自訂物件。</p> 
   </td> 
  </tr>

<tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[！UICONTROL篩選器]</td> 
   <td> <p>定義畫面上所顯示資訊的報告或清單元素的主要建置區塊之一。 如需有關報表元素的詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">報表元素：篩選器、檢視和群組</a>.</p> <p>此篩選條件會決定要在報表或網站上顯示的結果 [!DNL Workfront] 面板清單，例如專案、任務或問題。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[！UICONTROL Financial Work Management]</td> 
   <td>管理人力成本、費用和收入資料的程式 [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL固定成本]</td> 
   <td>您可以為專案定義固定成本金額。 這是專案的[！UICONTROL計畫成本]的一部分，代表完成專案所需的金額。 如需有關成本的資訊，請參閱 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">追蹤成本</a>. </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL固定收入]</td> 
   <td>您可以定義專案的固定收入金額。 這是專案的[！UICONTROL計畫收入]的一部分，代表完成專案時可能獲得的金額。 如需收入的詳細資訊，請參閱 <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">帳單與收入概要</a>. </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL旗標]</td> 
   <td> <p> 此欄位與[！UICONTROL狀態圖示]相同，但僅適用於下列檢視： </p> 
    <ul> 
     <li> [！UICONTROL範本] </li> 
     <li> [！UICONTROL費用] </li> 
    </ul> <p> 如需詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">檢視中的內建狀態圖示</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL資料夾]</td> 
   <td>資料夾可用來組織與物件相關聯的檔案或報告。</td> </tr>
  <tr>
  <td>[！UICONTROL FTE] （全時相當的）</td> 
   <td>這是相當於全職的時間，表示資源可用於工作的時間。 
   [！UICONTROL FTE]欄位會顯示在下列區域中： 
  <ul>
   <li> 使用者設定檔（編輯或建立使用者時） </li>
   <li> [！UICONTROL資源規劃工具] </li>
   <li> [！UICONTROL Scenario Planner] (需要Workfront Scenario Planner的其他授權) </li>
   <li> 使用者清單和報告 </li> </ul>

<p>[！UICONTROL FTE]必須是十進位數字，最多為1，而且不能為0。 </p>
   <p> [！UICONTROL FTE]為1 （這是使用者的[！UICONTROL FTE]欄位的預設值，如其設定檔中所定義）表示資源（使用者或角色）會根據計算其可用性的排程進行整個小時數的作業。 </p>
   <p>您的Workfront管理員會決定使用哪個排程來判斷使用者的可用性。  </p>
   <ul>
   <li> 使用[！UICONTROL預設排程]時，Workfront會使用在其設定檔中找到的使用者的[！UICONTROL FTE]來計算可用性。 </li>
   <li> 使用使用者的排程時，Workfront會使用使用者的休假、[！UICONTROL工作時間]值和[！UICONTROL預設排程]時數，來計算使用者的[！UICONTROL FTE]。 </li> </ul>

<p>如需詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">設定資源管理喜好設定</a>.  </p>
   <p>有關在中建立排程的詳細資訊 [!DNL Workfront]，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">建立排程</a>. </p>

<p><b>附註</b></p>
   <p>對於[！UICONTROL Scenario Planner]中的所有計算，Workfront會使用以下值： 1 [！UICONTROL FTE] = 8小時。</p>
   <p>如需詳細資訊，請參閱 <a href="../../../scenario-planner/get-started-with-scenario-planning.md">開始使用[！UICONTROL Scenario Planner]</a>. </p>
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
   <td>[！UICONTROL甘特圖]</td> 
   <td> <p>行事曆檢視中專案日期的視覺時間表是根據專案任務目前排程時的計畫或預計日期。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL目標]</td> 
   <td><p>中的目標有兩個概念 [!DNL Workfront]： </p> 
    <ul> 
     <li> <p><b>專案目標</b>：專案相關利害關係人同意的一組業務目標。 專案目標為專案業務案例的一部分。 </p> <p>您無法在清單或報告中顯示專案目標，但可以透過API存取它們。 </p> <p>如需業務案例專案目標的相關資訊，請參閱 <a href="../../../manage-work/projects/define-a-business-case/create-business-case-goals.md">建立業務案例目標 </a>. </p> </li> 
     <li> <p><b>策略目標</b>：策略目標是您建立的一個目標，用來計畫特定時段的工作策略。 您可以使用以下專案建立這些型別的目標： [!DNL Workfront Goals]. 您的組織必須購買額外的授權，且您必須擁有此功能的存取權，才能建立策略目標。 [!DNL Workfront Goals] 只能透過額外的授權取得。</p> 
     <p>如需詳細資訊，請參閱 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] 概觀 </a>. </p> 
     <p>您可以在目標或專案報告中顯示策略目標，並透過API存取它們。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL目標階層]</td> 
   <td> <p>在[！UICONTROL目標]和[！UICONTROL專案]報表中，這是收集欄位，當策略目標與其他目標對齊時，會在階層中顯示其所屬的目標。 目標會以▸分界符號分隔。 </p> <p>只有目標和目標的父級會顯示在此欄位中。 子目標不顯示。 </p> <p>有關對齊目標的資訊 [!DNL Workfront Goals]，請參閱 <a href="../../../workfront-goals/goal-alignment/goal-alignment-overview.md">中的目標一致性概觀 [!DNL Workfront Goals]</a>. </p> 
   <p>此欄位僅在您的組織購買後才可見 [!DNL Workfront Goals]. 有關使用管理策略目標的資訊 [!DNL Workfront Goals]，請參閱 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] 概觀 </a>. </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL目標成功分數]</td> 
   <td> 在[！UICONTROL專案報告]中，此欄位用於引用與[！UICONTROL商業]案例相關聯的專案層級目標。 目前，此欄位已棄用，且未與任何功能建立關聯。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL目標] </td> 
   <td> <p>在[！UICONTROL專案]報表中，此集合欄位會顯示與專案相關聯的所有策略目標。 目標以逗號分隔。</p> <p>此欄位僅在您的組織購買後才可見 [!DNL Workfront Goals]. 有關使用管理策略目標的資訊 [!DNL Workfront Goals]，請參閱 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] 概觀</a>. 如需中策略目標和專案目標的詳細資訊 [!DNL Workfront]，請參閱本文章的「[！UICONTROL目標]」。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL全域介面喜好設定]</td> 
   <td>影響所有使用者的介面設定。 [！UICONTROL全域介面偏好設定]可由[！UICONTROL使用者介面偏好設定]覆寫。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[！UICONTROL群組]</td> 
   <td> <p>擁有相同物件存取權的使用者（可能來自相同部門或業務單位）集合。 除了使用者之外，群組還可以與投資組合、方案、專案相關聯<span> 專案範本、</span> 公司、團隊、時程表、版面範本和時程表設定檔。</p> <p>您也可以依群組授予物件許可權。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">群組概述</a>.</p> <p>在下列其中一種型別的物件清單或報表中，您可以使用[！UICONTROL群組]欄位來列出與特定群組相關聯的該型別物件：使用者、投資組合、方案、專案、 <span>專案範本</span>、公司、團隊、排程、版面範本或時程表設定檔。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[！UICONTROL群組管理員]</td> 
   <td> <p>管理指定使用者群組的物件、存取許可權和使用者的使用者。</p> <p> 在[！UICONTROL群組]報表中，此欄位會顯示群組中指定為[！UICONTROL群組管理員]的使用者名稱。 如需群組管理員的詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">群組管理員</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>具有管理存取權的[！UICONTROL群組]</td> 
   <td> <p> 在[！UICONTROL配置範本]、[！UICONTROL週期性時程表或[！UICONTROL排程報告]中，此欄位會顯示群組管理員有權修改範本的群組。 您也可以依此欄位篩選此報告。 </p> <p> 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">建立和管理版面範本</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[！UICONTROL群組]</td> 
   <td> <p>報表元素，用來依通用標準將清單中的資訊分類。</p> <p>如需詳細資訊，請參閱文章中的「[！UICONTROL群組]」一節 <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">報表元素：篩選器、檢視和群組</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL移交日期]</td> 
   <td> <p>任務可供工作的日期。 [！UICONTROL移交日期]是計算式，無法手動設定。 <br>如需[！UICONTROL移交日期]的詳細資訊，請參閱文章 <a href="../../../manage-work/tasks/task-information/handoff-task-date.md" class="MCXref xref">[！UICONTROL任務移交日期]概觀</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL服務檯]</td> 
   <td>部分 [!DNL Workfront] 保留所有問題佇列的屬性。 [！UICONTROL服務檯]可用於處理客戶支援票證、專案請求、服務檯票證等。 這與[！UICONTROL要求]區域相同。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL擁有者]</td> 
   <td>在[！UICONTROL Hour]報表中，[！UICONTROL Owner]是小時所屬的使用者。 這與實際記錄時間的使用者不同。 這兩個實體有時可能是兩個不同的使用者。 <br>如需其他使用者記錄時間的詳細資訊，請參閱文章 <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">記錄時間</a>.</td> 
  </tr>

<tr> 
   <td>小時狀態</td> 
   <td> <p>Workfront為使用者記錄任務、問題或專案的實際時數設定的屬性。 </p>

小時專案在Workfront中可以有下列其中一種狀態：
<ul>
   <li><b>已提交</b>：時數已記錄在專案、任務或問題上。 它們是付費記錄的一部分，或尚未新增到付費記錄。</li>
   <li><b>已核准</b>：時數已記錄且已由專案所有者核准。 它們是付費記錄的一部分，或尚未新增到付費記錄。</li> 
   <li><b>未核准</b>：專案所有者已記錄並拒絕時數。 它們是付費記錄的一部分，或尚未新增到付費記錄。</li>
   <li><b>已記帳</b>：小時已記錄，已新增到計費記錄，並且計費記錄狀態已標籤為已計費。 它們不需要專案所有者的核准。</li>
   <li><b>已記帳和已核准</b>：時數已記錄並由專案所有者核准，而計費記錄狀態已標籤為已計費。</li>
   </ul>


<p>當時數是計費記錄的一部分時，時數狀態會指出時數是否已核准或他們所屬的計費記錄是否已計費。 時數條目的時數狀態僅會顯示在時數清單或報告中。 </p>

<p>如需將時數新增至計費記錄的詳細資訊，請參閱文章中的「將時數新增至計費記錄」一節 <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >建立付費記錄</a>.</p>

<p>如需核准專案時間的詳細資訊，請參閱 <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" >專案需要核准時間</a>.</p>

<p><b>秘訣</b></p>

<p>未直接在工作專案上記錄的一般時數不會顯示時數狀態。 </p> </td> 
  </tr>



<tr> 
   <td>[！UICONTROL小時型別]</td> 
   <td> <p>可針對使用者記錄任務、問題或專案的實際時數設定的屬性。 這也是未直接連結至工作的記錄時數屬性，例如[！UICONTROL Vacation]和[！UICONTROL Time Off]。</p> <p>如需詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md" class="MCXref xref">管理小時型別</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL ID]</td> 
   <td> <p>ID是與中每個物件相關聯的英數字元指標 [!DNL Workfront]. 它可唯一識別 [!DNL Workfront] 資料庫。 您可以檢視報表中任何物件的ID或每個物件的清單。 </p> <p>秘訣：   <p>您也可以檢視物件頁面URL中的ID。 例如，當您存取[！UICONTROL專案詳細資訊]頁面時，專案的ID看起來可能類似於以下URL中概述的數字：</p> <p><code>https://&lt;your domain>.my.workfront.com/project/<b>5e29c8010027d8eb334762d4fff3ffca</b>/overview</code> </p> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[！UICONTROL個別目標]</td> 
   <td>對團隊目標量度有貢獻，但與個人或職業發展無關的個人目標。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[！UICONTROL繼承存取權]</td> 
   <td>允許存取權從物件傳播到另一個物件的共用函式。 例如，專案使用者的繼承存取權（定義在方案和投資組合記錄中）。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL方案]</td> 
   <td> <p>在 [!DNL Workfront Scenario Planner]，您可以將計劃分割為數個方案，以便更輕鬆地管理計畫。 <span>您可以建立[！UICONTROL Initiative]報表，並可存取[！UICONTROL專案]報表中的[！UICONTROL Initiative]資訊。</span></p> <p>此 [!DNL Scenario Planner] 需要額外的授權。 如需關於以下專案的資訊： [!DNL Workfront Scenario Planner]，請參閱 <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">此 [!DNL Scenario Planner] 概觀</a>. </p> <p>此 [!DNL Initiative] 報告在您的 [!DNL Workfront] 例項，除非貴公司已購買 [!DNL Workfront Scenario Planner] 授權。 您無法透過API存取[！UICONTROL Initiatives]。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[！UICONTROL行動方案工作角色]</span> </td> 
   <td> <p><span>[！UICONTROL行動方案工作角色]報告型別顯示與計畫行動方案相關之工作角色的資訊 [!DNL Workfront Scenario Planner].</span> </p> <p>此 [!DNL Scenario Planner] 需要額外的授權。 如需關於以下專案的資訊： [!DNL Workfront Scenario Planner]，請參閱 <a href="../../../scenario-planner/scenario-planner-overview.md">此 [!DNL Scenario Planner] 概觀</a>. </p> <p><span>此報告型別不會顯示在您的 [!DNL Workfront] 例項，除非貴公司已購買 [!DNL Workfront Scenario Planner] 授權。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[！UICONTROL行動方案工作角色時數]</span> </td> 
   <td> <p><span> 在[！UICONTROL行動方案工作角色]報表中，這會顯示與行動方案中工作角色相關的小時數。</span> </p> <p>此 [!DNL Scenario Planner] 需要額外的授權。 如需關於以下專案的資訊： [!DNL Workfront Scenario Planner]，請參閱 <a href="../../../scenario-planner/scenario-planner-overview.md">此 [!DNL Scenario Planner] 概觀</a>. </p> <p>此欄位和[！UICONTROL行動方案工作角色]報告型別未顯示在您的中 [!DNL Workfront] 例項，除非貴公司已購買 [!DNL Workfront Scenario Planner] 授權。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL行動方案工作角色計數]</td> 
   <td> <p>在[！UICONTROL方案工作角色]報表中，這會顯示與方案相關聯的特定工作角色數量。</p> <p>此 [!DNL Scenario Planner] 需要額外的授權。 如需關於以下專案的資訊： [!DNL Workfront Scenario Planner]，請參閱 <a href="../../../scenario-planner/scenario-planner-overview.md">此 [!DNL Scenario Planner] 概觀</a>. </p> <p>此欄位和[！UICONTROL行動方案工作角色]報告型別未顯示在您的中 [!DNL Workfront] 例項，除非貴公司已購買 [!DNL Workfront Scenario Planner] 授權。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL方案上次發佈日期]</td> 
   <td> <p>[！UICONTROL Initiative]、[！UICONTROL Initiative Job Role]和[！UICONTROL Project]報表中的欄位，顯示上次將計畫方案發佈至專案的日期。 您可以發佈方案以建立專案或更新連結至方案的專案。</p> <p>此 [!DNL Scenario Planner] 需要額外的授權。 如需關於以下專案的資訊： [!DNL Workfront Scenario Planner]，請參閱 <a href="../../../scenario-planner/scenario-planner-overview.md">此 [!DNL Scenario Planner] 概觀</a>. </p> <p><span>如需發佈行動方案的相關資訊，請參閱</span><a href="../../../scenario-planner/publish-scenarios-update-projects.md">發佈情境以在中建立和更新專案 [!DNL Workfront Scenario Planner]</a>. 此欄位不會顯示在您的 [!DNL Workfront] 例項，除非貴公司已購買 [!DNL Workfront Scenario Planner] 授權。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL內嵌搜尋]</td> 
   <td>在完成表單的過程中執行搜尋，以尋找某個特定欄位的可能專案。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL介面設定]</td> 
   <td>允許定義自訂檢視、篩選器、群組、清單控制項等的應用程式區域。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[！UICONTROL是公司目標]</p></td> 
   <td> <p>在 [!DNL goal reports]，這會為每個策略目標顯示「[！UICONTROL True]/ [！UICONTROL False]」值，以指出您的組織是否已指派給目標作為其擁有者。 </p> 
   <p>此欄位僅在您的組織購買後才可見 [!DNL Workfront Goals]. 有關使用管理策略目標的資訊 [!DNL Workfront Goals]，請參閱 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] 概觀 </a>.</p>
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[！UICONTROL問題]</td> 
   <td> <p>未計畫的工作專案，通常表示發生妨礙任務或專案完成的問題。 它會經過分類及評估，以供進一步的工作量考量</p> <p>[！UICONTROL問題]也可以是[！UICONTROL服務檯]請求。 [！UICONTROL變更單]、[！UICONTROL請求]和[！UICONTROL錯誤]也是[！UICONTROL問題]。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[！UICONTROL問題管理]</td> 
   <td> <p>管理問題型別定義的流程和規則，以及與每種型別相關聯的路由、分類或流量流程。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[！UICONTROL問題所有者]</td> 
   <td>負責分類及完成問題的團隊或使用者。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[！UICONTROL反複專案]</td> 
   <td>團隊產生預先定義之交付專案集的時間段。</td> 
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
   <td>[！UICONTROL工作角色]</td> 
   <td> <p>用於識別使用者的日常工作職能和責任。 工作角色可以指派給工作專案，以識別完成工作流程所需的技能，而不將其指派給特定使用者。 </p> <p>一個使用者可以有多個角色。 範例包括Graphic Designer或Consultant。</p> <p>如需詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">建立和管理職位角色</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[！UICONTROL日誌專案]</p> </td> 
   <td> <p>可報告物件可告訴您專案、任務、問題和其他物件的[！UICONTROL更新]區域中出現的追蹤欄位系統更新的相關資訊。</p> <p>若要深入瞭解，請參閱 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md" class="MCXref xref">[！UICONTROL更新]區域報告</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Kanban標幟]</td> 
   <td> <p>在[！UICONTROL Task]報告或[！UICONTROL Issue]報告中，[！UICONTROL Kanban Flag]欄位會顯示在[！UICONTROL Kanban Board]上的內文上設定的旗標狀態。 可能的值包括[！UICONTROL On Track]、[！UICONTROL Ready To Pull]和[！UICONTROL Is Blocked]。</p> <p>如需在[！UICONTROL Kanban劇本板上設定劇本旗標狀態的詳細資訊，請參閱文章 <a href="../../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md" class="MCXref xref">在[！UICONTROL Kanban board]上的內文上使用旗標</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>KPI</td> 
   <td>可衡量的價值，可顯示公司達成關鍵業務目標的成效。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL延遲]</td> 
   <td>前置任務的[！UICONTROL規劃完成日期]之後必須經過的時間，直到相依任務可以開始為止。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL延遲型別]</td> 
   <td> <p>計算[！UICONTROL Lag]的方法。 可以是：</p> 
    <ul> 
     <li>[！UICONTROL天數] （工作日）</li> 
     <li>[！UICONTROL行事曆日] （忽略假日）</li> 
     <li>[！UICONTROL百分比]</li> 
     <li>[！UICONTROL星期]</li> 
    </ul> <p>如需詳細資訊，請參閱以下章節中的「[！UICONTROL延遲型別概觀]」一節： <a href="../../../manage-work/tasks/use-prdcssrs/lag-types.md" class="MCXref xref">延遲型別概觀</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL大型縮圖]</td> 
   <td> <p> 在[！UICONTROL Document]清單或報表中，它會在縮圖中顯示檔案的預覽。 </p> <p>選取 <strong>[！UICONTROL大型縮圖]</strong> 在報表中檢視400畫素寬的縮圖。</p> <p>當您修改清單或報表中的欄寬時，縮圖的大小會隨之調整。</p> <p>另請參閱本文中的「[！UICONTROL縮圖]」。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL最近10個檢視者]</td> 
   <td> <p>在報告清單中，此欄位顯示最多10個最近檢視過報告的使用者名稱。<br>如需報告清單使用資訊的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">檢視報告使用量</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL上次條件備註]</td> 
   <td> <p>此欄位顯示物件擁有者上次在物件上輸入的更新。這是擁有者最近對物件進行的活動或互動。</p> <p>此 [!DNL Last Condition Note] 如果刪除了物件最後一個註記的註記文字，欄會空白。 在物件上輸入新註記時，它會變成最後一個註記，並再次顯示在欄中。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL上次財務更新日期]</td> 
   <td>在[！UICONTROL專案]報表中，此欄位會擷取上次計算及更新專案財務的日期與時間。 如需有關專案財務的資訊，請參閱 <a href="../../../manage-work/projects/project-finances/project-finances-overview-1.md" class="MCXref xref">專案財務概觀</a>. </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL上一個備註]</td> 
   <td> <p>此欄位顯示任何使用者最後在物件上輸入的更新。 這是物件上最近的活動或互動。</p> <p>如果刪除了物件最後附註的文字，則[！UICONTROL Last Note]欄為空白。 在物件上輸入新註記時，它會變成最後一個註記，並再次顯示在欄中。</p>
   <p>將此欄位新增至[！UICONTROL任務]報告時，子物件上所遺留下來的任何更新，例如問題、子任務、檔案等。  — 此欄不顯示任務的。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL上次檢視者]</td> 
   <td> <p>在報告清單中，此欄位顯示上次檢視報告之使用者的相關資訊。<br>如需報告清單使用資訊的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">檢視報告使用量</a>.<br></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL上次檢視日期]</td> 
   <td> <p>在報告清單中，此欄位顯示上次顯示報告的日期。<br>如需報告清單使用資訊的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">檢視報告使用量</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[！UICONTROL配置範本]</td> 
   <td>由系統管理員或群組管理員定義，用於識別在指定使用者的工作區中顯示的標籤和報告。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL配置型別]</td> 
   <td>[！UICONTROL配置型別]結合[！UICONTROL自訂檢視]指定[！UICONTROL自訂檢視]的型別。 目前，只有清單可用。 日後可能會提供[！UICONTROL Detail] （物件的[！UICONTROL Detail]檢視）。</td> 
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
   <td>[！UICONTROL程式庫任務]</td> 
   <td>單一工作的範本，用於跨應用程式提供一致的[！UICONTROL工作]和[！UICONTROL範本工作]命名。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL授權型別]</td> 
   <td>配置給[！UICONTROL存取層級]的授權型別。 它是[！UICONTROL Full User]、[！UICONTROL Limited User]或[！UICONTROL Requester]。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL授許可權制計畫]</td> 
   <td> <p>在[！UICONTROL群組]檢視或報表中，此欄位顯示可指派給已將個別群組指定為[！UICONTROL主群組]的使用者的[！UICONTROL計畫]授權數目上限。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL授許可權制工時]</td> 
   <td> <p>在[！UICONTROL群組]檢視或報表中，此欄位顯示可指派給已將個別群組指定為[！UICONTROL主群組]之使用者的最大[！UICONTROL工作]授權數量。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL受限使用者]</td> 
   <td>允許建立 [!DNL Access Level] 包含僅供檢視的許可權，可提交問題、輸入附註及上傳檔案。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL清單控制項]</td> 
   <td> <p>[！UICONTROL介面設定]的一部分，可將自訂篩選器、檢視和群組連結至個別使用者或全域連結至所有使用者。</p> </td> 
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
   <td>[！UICONTROL手冊]</td> 
   <td> <p>[！UICONTROL專案]的[！UICONTROL更新型別]之一。 此設定允許只有在按一下「[！UICONTROL重新計算時間表]」時，[！UICONTROL專案預計]和[！UICONTROL計畫]時間表才會更新。 在稍微重新計算過程中以及更新專案中的專案或任務時，將忽略以此方式設定的專案。</p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">選取專案[！UICONTROL更新型別] </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Me]</td> 
   <td> <p>這是指目前登入的使用者。 </p> <p>我們建議在篩選器中使用此欄位，讓報表在與其他使用者共用時更通用。 如此一來，您只能建置一個報表，該報表會根據登入檢視者的身分顯示不同資訊，因為資訊一律會為登入使用者自訂。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL最大使用者數]</td> 
   <td> <p>這是已棄用的欄位。 此欄位可能顯示的任何資訊都與以下功能相關： [!DNL Workfront] 已移除，欄位無法更新。 </p> <p>在舊版中 [!DNL Workfront]，您可在建立或編輯工作角色時更新此欄位。 它會顯示可與每個專案中的角色相關聯的使用者總數。 值為零，表示專案中可指派的使用者數量不受限制。 </p>某些報告和清單中仍可看到該欄位，但無法更新顯示的資訊。 </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[！UICONTROL里程碑]</td> 
   <td> <p>您可以與任務關聯的標籤，以表示任務完成時已達成專案中的關鍵點。 您通常可以使用里程碑來顯示重大事件，例如專案某個階段的完成或一組關鍵活動。 [！UICONTROL里程碑]通常與父級任務相關聯。 您必須先建立里程碑，然後才能將其附加至任務。 如需里程碑的相關資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md">建立里程碑路徑</a> 和 <a href="../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md">將里程碑與任務建立關聯</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL里程碑路徑]</td> 
   <td>[！UICONTROL里程碑]的集合。 [！UICONTROL里程碑路徑]用於專案，以將具有特定型別[！UICONTROL里程碑]的專案與具有一組不同[！UICONTROL里程碑]的專案區分開來。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[！UICONTROL里程碑任務]</td> 
   <td>標幟為指示要測量之可報告事件的工作。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL模組]</td> 
   <td>中的案例中的單一步驟 [!DNL Workfront Fusion] 會根據相關聯的應用程式執行某些功能。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL我的主要角色]</td> 
   <td> <p>若在篩選條件中參考此項，將顯示與登入使用者具有相同之[！UICONTROL主要角色]的使用者，或指派給登入使用者之[！UICONTROL主要角色]的工作專案。</p> <p>我們建議在篩選器中使用此欄位，讓報表在與其他使用者共用時更通用。 如此一來，您只能建置一個報表，該報表會根據登入檢視者的身分顯示不同資訊，因為資訊一律會為登入使用者自訂。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL我的主團隊]</td> 
   <td> <p>若在篩選條件中參考此欄位，此欄位會顯示屬於登入使用者的[！UICONTROL主團隊]的使用者，或指派給登入使用者的[！UICONTROL主團隊]的工作專案。 </p> <p>我們建議在篩選器中使用此欄位，讓報表在與其他使用者共用時更通用。 如此一來，您只能建置一個報表，該報表會根據登入檢視者的身分顯示不同資訊，因為資訊一律會為登入使用者自訂。 </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[！UICONTROL命名慣例]</td> 
   <td>組織範圍的一組規則，使用資料來建立專案、任務和交付專案的名稱。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[！UICONTROL原生整合]</td> 
   <td>不需要手動編碼或API設定的整合。 也稱為「立即可用」的整合。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL導覽功能表]</td> 
   <td>應用程式中央上方的面板，其中包含指向[！UICONTROL Workfront]主要區域的連結。</td> 
  </tr> 
 </tr> 
  <tr> 
   <td>[！UICONTROL新數值]</td> 
   <td>在[！UICONTROL日誌專案]報表中，這會顯示取代[！UICONTROL舊數字值]之欄位的更新值。
   如需詳細資訊，請參閱本文中的「[！UICONTROL舊數字值]」。</td> 
  </tr>
  <tr> 
   <td>[！UICONTROL非工作日]</td> 
   <td>未配置完成任何指派的日期。 這通常是假日、假期或週末。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL附註]</td> 
   <td>對進行評論或更新 [!DNL Workfront] 物件。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL附註文字]</td> 
   <td> <p>這會顯示使用者在任何物件上輸入的更新文字。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL連結目標數目]</td> 
   <td> <p>在[！UICONTROL專案]報表中，這是與專案相關聯的策略目標數目。 如需將專案與策略目標相關聯的資訊，請參閱 <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">將專案新增至中的目標  [!DNL Adobe Workfront Goals]</a>.</p> 
   <p>如需策略目標的相關資訊，另請參閱本文中的「[！UICONTROL目標]」。</p> 
   <p>此欄位僅在您的組織購買後才可見 [!DNL Workfront Goals]. 有關使用管理策略目標的資訊 [!DNL Workfront Goals]，請參閱 <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">將專案新增至[！UICONTROL Adobe Workfront目標]中的目標</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL物件]</td> 
   <td> <p>您在中顯示的資訊 [!DNL Adobe Workfront] 由儲存在 [!DNL Workfront] 資料庫。 物件會驅動Workfront中的資訊。 物件的部分範例包括：</p> 
    <ul> 
     <li>[！UICONTROLPortfolio]</li> 
     <li>[！UICONTROL程式]</li> 
     <li>[！UICONTROL專案]</li> 
     <li>[！UICONTROL工作]</li> 
     <li>[！UICONTROL問題]</li> 
     <li>[！UICONTROL檔案]</li> 
     <li>[！UICONTROL儀表板]</li> 
     <li>[！UICONTROL報表]</li> 
     <li>[！UICONTROL群組]</li> 
     <li>[！UICONTROL團隊]</li> 
     <li>[！UICONTROL使用者]</li> 
     <li>[！UICONTROL公司]</li> 
     <li>[！UICONTROL自訂表單]</li>
     <li>[！UICONTROL自訂欄位]</li>  
     <li>[！UICONTROL小時]</li> 
     <li>[！UICONTROL收費率]</li> 
     <li>[！UICONTROL範本]</li> 
     <li>[！UICONTROL範本任務]</li>

<p><b>附註</b></p>
  <p>這不是一份詳盡的清單。 </p>

</ul> <p>如需詳細資訊，請參閱 <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">瞭解[！UICONTROL Adobe Workfront]中的物件</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL物件型別]</td> 
   <td>如果您建立包含所有自訂表單的報表或清單，您可以使用此欄位作為檢視或篩選條件，以檢視與每個表單相關聯的物件型別。 </td> 
  </tr> 
 <tr> 
   <td>[！UICONTROL舊數值]</td> 
   <td>在[！UICONTROL日誌專案]報表中，這會顯示欄位在更新前的原始值。 欄位的值更新後，將在[！UICONTROL Journal Entry]報表中顯示為[！UICONTROL New Number Value]。 如需詳細資訊，另請參閱「[！UICONTROL新數值]」。</td> 
  </tr>
  <tr> 
   <td>[！UICONTROL On Change Only]</td> 
   <td> <p>其中一種[！UICONTROL專案更新]型別。 選取此專案時，[！UICONTROL專案預計]和[！UICONTROL計畫]時間表只會在專案或專案內任務進行更新或變更時更新。 它不會每晚更新專案。</p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">選取專案更新型別 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL作業任務]</td> 
   <td> <p>中的[！UICONTROL Issue]名稱 [!DNL Workfront] 資料庫，用於文字模式報表或計算的自訂資料。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL開啟]</td> 
   <td>未完成但正在處理的問題或任務。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL組織圖]</td> 
   <td>組織圖表的簡稱。 此圖表顯示組織的階層。 它也在[！UICONTROL使用者]詳細資訊熒幕上的索引標籤上，顯示並允許設定[！UICONTROL使用者]的[！UICONTROL公司]和[！UICONTROL報告]關係。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL組織設定]</td> 
   <td>這會為您的組織定義[！UICONTROL公司]、[！UICONTROL群組]和[！UICONTROL安全性設定檔]。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL其他群組]</td> 
   <td> <p>在列出使用者的報表或檢視中，此欄位會顯示每個使用者所屬的所有群組。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[！UICONTROL覆寫貨幣]</span> </td> 
   <td> 
    <div> 
     <p>在[！UICONTROL工作角色]報表中，這是與工作角色相關聯的貨幣。 此設定覆寫了[！UICONTROL基本貨幣]，如[！UICONTROL設定]區域中所建立，並由 [!DNL Workfront] 管理員。 </p> 
     <p>如需詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">建立和管理職位角色</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[！UICONTROL覆寫貨幣帳單/小時]</span> </td> 
   <td> 
    <div> 
     <p>在[！UICONTROL工作角色]報表中，這是使用工作角色所選[！UICONTROL覆寫貨幣]之工作角色的每小時收費率。</p> 
     <p> 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">建立和管理職位角色</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[！UICONTROL覆寫貨幣成本/小時]</span> </td> 
   <td> 
    <div> 
     <p>在[！UICONTROL工作角色]報表中，這是工作角色使用所選工作角色[！UICONTROL覆寫貨幣]的每小時成本率。 </p> 
     <p>如需詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">建立和管理職位角色</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[！UICONTROL擁有者]</td> 
   <td>負責完成指定物件的使用者。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[！UICONTROL擁有者型別]</span> </td> 
   <td> 
    <div> 
     <p>在[！UICONTROL目標]報表中，這會顯示指派給策略目標的擁有者型別。 以下是目標擁有者型別：</p> 
     <ul> 
      <li> <p>[！UICONTROL使用者]</p> </li> 
      <li> <p>[！UICONTROL團隊] </p> </li> 
      <li> <p>[！UICONTROL群組]</p> </li> 
     </ul> 
     <p>當目標擁有者是您的組織時，此欄位中不會顯示任何值。 </p> 
     <p>這需要額外的授權。 如需有關的資訊 [!DNL Workfront Goals]，請參閱 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">[!DNL Adobe Workfront Goals] 概觀</a>. </p> 
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
   <td>[！UICONTROL引數]</td> 
   <td> <p>[！UICONTROL引數]是自訂欄位。 您可以為系統中的所有引數或自訂欄位建立報表。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Parent]</td> 
   <td>在報表中，此欄位會顯示物件父項的相關資訊。 例如，在[！UICONTROL問題]報告中，它可能會顯示問題記錄所在之任務或專案的相關資訊；在任務報告中，它可能會顯示直接父級任務或專案的相關資訊。 有關哪些物件可能有父項的詳細資訊 [!DNL Workfront]，請參閱文章中的「物件的相依性和階層」一節 <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">瞭解中的物件 [!DNL Adobe Workfront]</a>. </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL父系延遲]</td> 
   <td>在[！UICONTROL父系任務]開始與[！UICONTROL子任務]開始之間必須經過的時間量。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL父系任務]</td> 
   <td>也稱為[！UICONTROL摘要任務]。 此任務具有子任務（也稱為[！UICONTROL子任務]）。 父系任務的[！UICONTROL工期]、[！UICONTROL所需工時]和[！UICONTROL完成百分比]是根據子任務計算的。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[！UICONTROL兼職資源]</td> 
   <td>具有少於系統中定義之預設排程的授權使用者。</td> 
  </tr> 
  <tr> 
   <td>完成百分比]</td> 
   <td> <p>顯示與任務、專案或問題相關之工作的完成百分比的專案、任務或問題欄位。</p> <p>您可以手動更新此欄位的問題和工作任務。 </p> <p>對於專案和父系任務，此欄位是從所有工作任務累計，您無法手動更新。 </p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/tasks/task-information/project-percent-complete.md" class="MCXref xref">專案[！UICONTROL完成百分比]概觀</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL許可權]</td> 
   <td> <p>授予使用者對物件的許可權，通常是為了讓使用者完成專案工作或檢視專案而提供。 您可以將許可權授予：</p> 
    <ul> 
     <li>[！UICONTROL專案]</li> 
     <li>[！UICONTROL工作]</li> 
     <li>[！UICONTROL問題]</li> 
     <li>[！UICONTROLPortfolio]</li> 
     <li>[！UICONTROL程式]</li> 
     <li>[！UICONTROL報表]</li> 
     <li>[！UICONTROL儀表板]</li> 
     <li>[！UICONTROL檔案]</li> 
     <li>[！UICONTROL自訂Forms]</li> 
     <li>[！UICONTROL檢視]</li> 
     <li>[！UICONTROL篩選器]</li> 
     <li>[！UICONTROL群組]</li> 
    </ul> <p>如需詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">共用物件許可權概觀</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL計畫]</td> 
   <td> <p>此為中的完整授權型別 [!DNL Workfront] 系統。 使用者必須具備此許可權才能存取中的所有功能 [!DNL Workfront].</p> <p>如需詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] 授權總覽</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL計畫] (在 [!DNL Scenario Planner])</td> 
   <td> <p>使用時，計畫是主要物件 [!DNL Workfront] 情境規劃工具。 您可以概述貴公司短期和長期未來的策略，找出每個高階成果並將其作為計畫新增至 [!DNL Workfront] 情境規劃工具。 </p> <p>您無法顯示 [!DNL Scenario Planner] 在報表中建立計畫，且您無法透過 [!DNL Workfront] API。 </p> <p>此 [!DNL Scenario Planner] 需要額外的授權。 如需關於以下專案的資訊： [!DNL Workfront Scenario Planner]，請參閱 <a href="../../../scenario-planner/scenario-planner-overview.md">此 [!DNL Scenario Planner] 概觀</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL計畫]</td> 
   <td> <p>某些專案排定發生的時間範圍。 當您在中建立專案、任務或問題時 [!DNL Workfront]，您可建立計畫的開始和結束日期，以及這些日期發生的計畫時間範圍。 這些值代表您的原始意圖或專案完成所需時間的預估值。 </p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL計畫權益]</td> 
   <td>這是手動輸入專案，可供專案經理估計完成專案是否能為組織帶來任何經濟利益。 為專案拼接[！UICONTROL商業案例]時，可指定此值。 您必須擁有專案的[！UICONTROL管理]許可權才能更新此值。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[！UICONTROL計畫預算時數]</td> 
   <td> <p>在[！UICONTROL預算時數]報表中，這會顯示[！UICONTROL資源規劃工具]中專案或[！UICONTROL工作角色]的預算時數。 </p> <p>如需有關在[！UICONTROL資源規劃工具]中將專案或角色編列預算的資訊，請參閱文章 <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">使用[！UICONTROL專案]和[！UICONTROL角色]檢視編列資源（在[！UICONTROL資源規劃工具]中）</a>. 如需[！UICONTROL Budgeted Hours]報表的相關資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">報告：預算時數</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL計畫完成日期]</td> 
   <td> <p>您可以手動將[！UICONTROL規劃完成日期]設定為您選擇的日期。 如果您未設定[！UICONTROL規劃完成日期]， [!DNL Workfront] 會自動設定。 自動設定時，[！UICONTROL規劃完成日期]為：[！UICONTROL規劃開始日期] + [！UICONTROL持續時間]</p> <p>如需詳細資訊，請參閱下列文章：</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">任務總覽[！UICONTROL規劃完成日期]</a> </p> </li> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">設定專案[！UICONTROL計畫完成日期]</a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL計畫成本]</td> 
   <td> <p>專案的[！UICONTROL計畫勞力成本]與[！UICONTROL計畫費用成本]的總和。 這不包括專案上的[！UICONTROL計畫風險成本]。  </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL計畫期間]</td> 
   <td> <p>任務的[！UICONTROL計畫持續時間]通常與任務的[！UICONTROL持續時間]相同。 它代表任務的[！UICONTROL計劃開始]和[！UICONTROL計畫完成日期]之間的天數差異。 </p> <p>當任務的[！UICONTROL工期]型別為[！UICONTROL投入比導向]時，根據您指派給任務的資源數量，[！UICONTROL計畫工期]可能與任務的[！UICONTROL工期]不同。 </p> <p>例如，如果[！UICONTROL工期]型別為[！UICONTROL投入比導向]的任務的[！UICONTROL工期]為3天，而您指派一個具有完整時間排程的資源給該任務，則[！UICONTROL計畫工期]也為3天。 如果您將三個具有完整時間排程的資源指派給相同的任務，[！UICONTROL期間]會維持3天，但[！UICONTROL計畫期間]會變成1天。 [！UICONTROL計畫期間]也會變更任務的[！UICONTROL計劃開始]和[！UICONTROL計畫完成]日期，以反映新的[！UICONTROL計畫期間]。 因此，專案的時間表也會受到影響。 </p> <p>如需有關任務的[！UICONTROL持續時間]與[！UICONTROL計畫持續時間]之間差異的詳細資訊，請參閱文章 <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md" class="MCXref xref">[！UICONTROL計畫持續時間]與任務的[！UICONTROL持續時間]之間的差異</a>.</p> <p>專案和問題沒有[！UICONTROL計畫期間]。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL計畫期間分鐘]</td> 
   <td> <p>專案或問題的[！UICONTROL計畫期間分鐘]是以分鐘為單位的專案或問題的[！UICONTROL期間]。 </p> <p>任務沒有[！UICONTROL計畫期間分鐘]欄位。 </p> <p>[！UICONTROL範本任務]有一個[！UICONTROL計畫期間分鐘]欄位，以分鐘為單位顯示任務的[！UICONTROL計畫期間]。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL計畫費用成本]</td> 
   <td> <p>針對專案或任務記錄的所有費用的[！UICONTROL計畫金額]總和。</p> <p><b>範例</b></p>
   <p>如果您為任務1建立費用，並在[！UICONTROL計畫金額]欄位中輸入$600.00，則此任務的[！UICONTROL計畫費用成本]為$600.00。 </p> 
   <p>若為專案， [!DNL Workfront] 使用以下公式計算[！UICONTROL計畫費用成本]：</p> <p><code>Project [!UICONTROL Planned Expense Cost] = SUM (All Project [!UICONTROL Planned Expense Costs]) + SUM (All Tasks [!UICONTROL Planned Expense Costs])</code> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (Drafting this because not sure if this is correct anymore)</p>
    --> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL計畫時數]</td> 
   <td> <p>此欄位顯示在[！UICONTROL專案]、[！UICONTROL任務]和問題區域、專案、任務或問題的報告以及資源管理工具，例如[！UICONTROL資源規劃者]、[！UICONTROL工作負載平衡器]和[！UICONTROL使用率]報告。 </p> <p>它會顯示專案所有者估計完成每個任務或問題所需的小時數。 對於專案而言，它通常是專案任務中[！UICONTROL計畫時數]的彙總。 </p> <p>根據您檢視的位置，[！UICONTROL規劃時數]欄位可能會顯示不同的資訊。 如需計畫時數的詳細資訊，請參閱 <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">計畫時數概觀</a>.</p> <p>計畫時數會以分鐘為單位儲存在 [!DNL Workfront] 資料庫。 使用此欄位編寫計算時，請確保將小時顯示為分鐘的情況納入考量。<br></p> <p>根據預設，計畫時數會平均分配給工作專案期間內的所有天數，也會平均分配給任務的所有資源。 使用者可以更新工作專案的每日計畫時數金額，或每個受指派人的個別計畫時數。</p> <p>專案、任務和問題的更新此欄位不同： </p> 
    <ul> 
     <li> <p>如有問題，您可以手動更新此欄位。 問題計畫時數未新增到專案計畫時數。 </p> <p>提示：在問題報表中，[！UICONTROL規劃時數]欄位之一已由[！UICONTROL工作]欄位取代。 欄位顯示問題的計畫時數數量。 如需詳細資訊，請參閱此表格中的「工作」或「[！UICONTROL工作]」欄位。 </p> </li> 
    </ul> 
    <ul> 
     <li> <p>對於任務，當任務的[！UICONTROL期間型別]是[！UICONTROL計算任務]或[！UICONTROL簡單]時，您可以手動更新此欄位。 此欄位的計算方式 [!DNL Workfront] 當任務的[！UICONTROL期間型別]為[！UICONTROL計算工時]或[！UICONTROL投入比導向]時。<br>如需[！UICONTROL工作期間]的相關資訊，請參閱文章 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任務[！UICONTROL工期]和[！UICONTROL工期型別]概觀</a>.</p> </li> 
    </ul> 
    <ul> 
     <li> <p>若為專案， [!DNL Workfront] 透過從專案的所有任務新增所有計畫時數來計算計畫時數。 </p> </li> 
    </ul> <p><b>秘訣</b></p> <p>您也可以使用文字模式和參考其他欄位，在[！UICONTROL專案]、[！UICONTROL任務]或[！UICONTROL問題]報告中顯示[！UICONTROL規劃時數]。 如需詳細資訊，請參閱「<code>work</code>"、"[！UICONTROL Work]"和"<code>workRequiredExpression</code>」欄位。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL計畫勞力成本]</td> 
   <td> 
    <p>對於任務，使用者或角色的每小時費率乘以指派給使用者或角色的時數。</p> <p>對於專案而言，它是所有任務的所有[！UICONTROL計畫勞力成本]的總和。</p> <p>是否使用使用者或角色的費率取決於為指定任務選取的成本型別。 </p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/projects/project-finances/track-costs.md">追蹤成本</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL計畫收入]</td> 
   <td> <p>任務和專案可以在以下位置顯示[！UICONTROL計畫收入]的值： [!DNL Workfront]. [！UICONTROL計畫收入]代表與專案上任務的[！UICONTROL計畫時數]相關聯的金額。 對於專案，它也可以包含專案的[！UICONTROL固定收入]。 </p> <p>對於任務，這是與任務的[！UICONTROL計畫時數]相關聯的收入。 所有任務的計畫時數會累計至專案的計畫時數，以參與專案[！UICONTROL計畫時數]的計算。 </p> 
   <p>[!DNL Workfront] 使用下列公式計算任務和專案的[！UICONTROL計畫收入]：</p> 
   <p><code>Task [!UICONTROL Planned Revenue] = [!UICONTROL Planned Hours] * Billing hourly rate</code> </p> <p><code>Project [!UICONTROL Planned Revenue] = SUM (All tasks [!UICONTROL Planned Revenue]) + [!UICONTROL Fixed Revenue]</code> </p> 
   <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the note below is duplicated in this article: /Content/Resource Mgmt/Resource utilization/view-utilization-information.htm and in the glossary)</p>
    --> 
    <p>顯示在[！UICONTROL專案詳細資料]區域和專案報表中的專案[！UICONTROL計畫收入]與[！UICONTROL使用率]報表中顯示的計畫收入不同。 </p> <p>[！UICONTROL專案詳細資料]區域中的[！UICONTROL計畫收入]反映了任務收入以及專案的固定收入。 [！UICONTROL使用率報表]中的[！UICONTROL計畫收入]僅顯示與專案中的任務相關聯的[！UICONTROL計畫收入]。 </p> 
     <p><b>範例</b></p>  
      <p>如果專案有1項時長為10小時的任務，指派給顧問時費為$20小時，且專案有$100的[！UICONTROL固定收入]，[！UICONTROL使用率]報表會針對[！UICONTROL計畫收入] （與任務時數相關聯的[！UICONTROL計畫收入]）顯示$200。 [！UICONTROL專案詳細資料]區段顯示$300 （來自任務的[！UICONTROL計畫收入]和專案的固定收入）。 </p> 
    <p>如需有關追蹤收入的資訊，請參閱： [!DNL Workfront] 另請參閱 <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md">帳單與收入概要</a>. </p> 
    <p>如需[！UICONTROL使用率報表]中[！UICONTROL計畫收入]計算方式的詳細資訊，請參閱 <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">檢視資源使用率資訊 </a>. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL計畫風險成本]</td> 
   <td> <p>專案上所有風險的[！UICONTROL潛在成本]總計，已計入其發生機率。 此金額不包含在專案的[！UICONTROL計畫成本]中。</p> <p>計算專案的[！UICONTROL計畫風險成本]的公式如下：</p> <p><code>Planned Risk Cost = SUM(Potential Risk Cost * Probability / 100)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL入口網站設定檔]</td> 
   <td>管理員定義的標籤和入口網站區段集合，會顯示在 [!DNL Workfront] 應用程式[！UICONTROL首頁]和其他儀表板。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL入口網站區段]</td> 
   <td>儀表板或入口網站頁面上索引標籤的一個元件。 通常是單一報告、圖表、行事曆或關鍵資訊清單。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL入口網站頁簽]</td> 
   <td>入口網站或控制面板上最多包含三個入口網站區段的標籤。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[！UICONTROLPortfolio]</td> 
   <td> <p>具有統一特性的專案集合。 這些專案通常會爭奪相同的資源、預算或時段。 您可以將Portfolio分割成方案，並在將專案新增到Portfolio之前將其與方案相關聯。</p> <p>如需投資組合的詳細資訊，請參閱 <a href="../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md">中的Portfolio概觀 [!DNL Adobe Workfront]</a>.</p> 
   </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[！UICONTROLPortfolio管理]</td> 
   <td>專注於管理集合或相關方案和專案工作的實踐領域。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[！UICONTROLPortfolio最佳化程式]</td> 
   <td>A [!DNL Workfront] 協助評估專案組合併排定其優先順序的工具。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[！UICONTROLPortfolio擁有者]</td> 
   <td>專案組合中負責優先順序和預算的利害關係人。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL潛在風險成本]</td> 
   <td>這是可在清單和報告中找到的專案欄位。 它會顯示與專案相關之風險的潛在成本（如果發生）。 如需詳細資訊，請參閱 <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">計算潛在風險成本 </a>. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[！UICONTROL前置任務]</td> 
   <td> <p>在依存性任務完成之前必須完成的工作。 亦即標示為另一個任務的[！UICONTROL相依性]的任務。 前置任務可讓供需規劃員設定順序相依性邏輯，例如在另一個任務完成後啟動任務。</p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">前置任務概觀</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL主要公司]</td> 
   <td>使用者所屬的公司，如其使用者設定中所指定。 公司也可以與專案建立關聯。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL主要連絡人]</td> 
   <td><p>[！UICONTROL主要連絡人]是問題的建立者，並由 [!DNL Workfront] 當有人建立問題時。 您可以手動更新此欄位，如果 [!DNL Manage] 問題的許可權。 一個問題只能有一個主要連絡人。</p> 
   <p>如果您變更主要連絡人，則原本指定為主要連絡人的使用者仍然擁有此問題的[！UICONTROL管理]存取權。</p>
   <p>將問題轉換為任務或專案時，指定為的[！UICONTROL主要聯絡人]的使用者會成為專案或任務的[！UICONTROL轉換的問題建立者]。 如果在問題轉換後更新問題的[！UICONTROL主要連絡人]，則轉換後的[！UICONTROL問題建立者]將保留為轉換發生時問題所在的[！UICONTROL主要連絡人]。 另請參閱本文中的「[！UICONTROL轉換的問題建立者]」。</p> 
   </td> 
  </tr>
  <tr> 
   <td>[！UICONTROL優先順序]</td> 
   <td>可指派給任務、問題或專案以指定其重要性的值。 </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Private]</td> 
   <td>在[！UICONTROL附註]或[！UICONTROL檔案]上，此選項會讓大多數檢視者隱藏該物件。 對於私人服務檯佇列，只有佇列團隊中的使用者可以透過[！UICONTROL服務檯]區域將問題提交到該佇列。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL設定檔]</td> 
   <td>有關使用者帳戶的所有資訊。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[！UICONTROL程式]</td> 
   <td> <p>投資組合的子集，其中類似的專案可以分組在一起，以實現明確界定的收益。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[！UICONTROL程式管理]</td> 
   <td>管理跨專案的相依性、風險、問題、需求和解決方案，以保持方案健康並達成定義的方案利益。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[！UICONTROL程式擁有者]</td> 
   <td>負責監督及組織活動的利害關係人，以確保專案目標與公司目標一致。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[！UICONTROL進度]</span> </td> 
   <td> <p>在[！UICONTROL目標]報表中，這會顯示策略目標接近完成的百分比。 進度百分比會以數字顯示。 如需策略目標的相關資訊，另請參閱本表中的「[！UICONTROL目標]」。</p> <p>此欄位僅在您的組織購買後才可見 [!DNL Workfront] 目標。 有關使用管理策略目標的資訊 [!DNL Workfront Goals]，請參閱 <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md"> 將專案新增至中的目標 [!DNL Adobe Workfront Goals] </a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL進度狀態]</td> 
   <td> <p>在專案、任務和目標報告中，此欄位會顯示專案、任務或策略目標的進度狀態。 如需詳細資訊，請參閱下列文章：</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-progress-status.md" class="MCXref xref">專案進度狀態概觀</a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">任務進度狀態總覽</a> </p> </li> 
     <li> <p><a href="../../../workfront-goals/goal-management/calculate-goal-progress.md">中的目標進度和條件概觀 [!DNL Adobe Workfront Goals]</a> </p>
     <p>的[！UICONTROL目標]報表和[！UICONTROL進度狀態] [!DNL goals] 欄位只有在您的組織已購買時才可見 [!DNL Workfront Goals]. 有關中策略目標的資訊 [!DNL Workfront Goals]，請參閱 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] 概觀</a>. </p> </li>
    </ul> </td> 
  </tr> 
  <td>[！UICONTROL專案]</td> 
   <td> <p>必須在特定時間範圍內完成的大量工作，且必須使用特定預算和資源數量。 為了讓專案易於管理，您可將專案分成一系列任務。 完成所有任務會導致專案完成。 如需計畫專案的詳細資訊，請參閱 <a href="../../../manage-work/projects/planning-a-project/plan-project.md">計畫專案概述</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL專案指派計畫時數]</td> 
   <td> <p>在[！UICONTROL方案工作角色]報表中，這會顯示與工作角色相關聯的[！UICONTROL規劃時數]，該工作角色會指派給專案中的任務或問題。 此欄位和[！UICONTROL行動方案工作角色]報告型別未顯示在您的中 [!DNL Workfront] 例項，除非貴公司已購買 [!DNL Workfront Scenario Planner] 授權。 如需關於以下專案的資訊： [!DNL Workfront Scenario Planner]，請參閱 <a href="../../../scenario-planner/scenario-planner-overview.md">此 [!DNL Workfront Scenario Planner] 概觀</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL專案詳細資料]</td> 
   <td>專案目前狀態的詳細資訊。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL專案預算成本]</td> 
   <td> <p> 這是專案在清單和報告中顯示的[！UICONTROL預算成本]。</p><p>另請參閱本文中的「[！UICONTROL預算成本]」。</p></td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[！UICONTROL專案管理]</td> 
   <td>一組原則，可管理專案建立、分類和命名等臨界值。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[！UICONTROL專案管理費用]</td> 
   <td>在[！UICONTROL小時]報表中，此欄位是保留給與小時型別[！UICONTROL專案時間]所記錄小時繫結的財務資訊。 專案可以有自己的計費率，如果一小時直接記錄到專案上，則這些費率將用於計算中。 根據專案設定，專案也可以有不同的貨幣，並且這些小時可以有貨幣轉換。 [！UICONTROL專案管理費用]物件允許 [!DNL Workfront] 以取得該資訊。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL專案所有者]</td> 
   <td>負責管理專案範圍、時間表和指派的使用者。 變更單、財務變更及交貨專案的預設核准者。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL專案計畫]</td> 
   <td>開發及維護專案排程的程式。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL專案贊助者]</td> 
   <td>您每個使用者的指定利害關係人設定檔，應與您相關。 在 [!DNL Workfront]，這些被指定為[！UICONTROL存取層級]</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL專案團隊]</td> 
   <td> <p>指派給專案的使用者或角色集合</p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md">專案團隊概觀</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL專案追蹤]</td> 
   <td>用來測量專案健康狀況和範圍的資料</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL專案]</td> 
   <td> <p>根據任務、問題或專案的規劃時數與完成百分比，預估工作完成的時間戳記。</p> <p>這是指任務、問題或專案的日期或[！UICONTROL期間]。 通常，它會在部分工作完成或經過一段時間後，指定更符合工作專案生平的日期和持續時間。 </p> <p>例如，任務的[！UICONTROL預計完成日期]是指 [!DNL Workfront] 會根據目前為止在該任務上完成的工作量、指派多少人員到該任務，以及自開始日期以來已過去的時間來估計任務將完成。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL校訂期限]</td> 
   <td> <p>在包含[！UICONTROL Document Version]物件的報告中（例如[！UICONTROL Document Version]報告和[！UICONTROL Proof Approval Approval]報告），此欄位會顯示校訂截止日期的星期幾、日期、時間和年份。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL校訂決定]</td> 
   <td> <p>在包含[！UICONTROL Document Version]物件的報告中（例如[！UICONTROL Document Version]報告和[！UICONTROL Proof Approval]報告），此欄位會顯示校訂的決定狀態（待處理、需要變更或已核准）</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL校訂名稱]</td> 
   <td> <p>在包含[！UICONTROL Document Version]物件的報告中（例如[！UICONTROL Document Version]報告和[！UICONTROL Proof Approval]報告），此欄位會顯示校訂名稱。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL校訂頁面]</td> 
   <td> <p>在包含[！UICONTROL Document Version]物件的報表中（例如[！UICONTROL Document Version]報表和[！UICONTROL Proof Approval]報表），此欄位會顯示校訂中包含的頁數。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL校訂進度]</td> 
   <td> <p>在包含[！UICONTROL Document Version]物件的報告中（例如[！UICONTROL Document Version]報告和[！UICONTROL Proof Approval]報告），顯示校訂的進度狀態([！UICONTROL Sent]、[！UICONTROL Open]、[！UICONTROL Commended]、[！UICONTROL Decision Made])。</p> <p>如需詳細資訊，請參閱 <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md#understanding-progress-and-status" class="MCXref xref">校訂進度概觀</a> 在 <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md" class="MCXref xref">校訂進度和狀態概觀</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL校訂]</td> 
   <td>一種稽核程式，其中一位或多位使用者在影像、文字檔案、影片或互動式網頁內容中應變更的內容上標籤和註解。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL公用]</td> 
   <td>在[！UICONTROL備註]或[！UICONTROL檔案]上，此選項可讓其他使用者或甚至外部人員存取該物件 [!DNL Workfront]. 對於[！UICONTROL服務檯佇列]，[！UICONTROL公用]表示所有可以提交問題的使用者都可以透過[！UICONTROL服務檯]區域提交問題。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[！UICONTROL品質]</td> 
   <td>組織內部對工作品質的看法。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL佇列]</td> 
   <td>也稱為[！UICONTROL服務檯佇列]。 此專案已發佈至[！UICONTROL服務檯]區域，可供使用者提交問題。 通常會為特定主題建立佇列，例如錯誤、專案請求等。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL佇列屬性]</td> 
   <td>這些設定會針對發佈至[！UICONTROL服務檯]的專案定義問題提交規則。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL佇列主題]</td> 
   <td> <p>[！UICONTROL服務檯佇列]上的屬性，可讓提交問題的使用者選取主題。 主題可以：</p> 
    <ul> 
     <li>與自訂資料表單相關聯。</li> 
     <li>透過所選主題上的路由規則集，自動將問題指派給使用者、角色或團隊。</li> 
     <li>透過所選主題上的路由規則集，將問題移至不同的專案或佇列。</li> 
    </ul> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">建立佇列主題</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL排名]</td> 
   <td> <p>在[！UICONTROL存取層級]報表中，您可以手動指出[！UICONTROL存取層級]的[！UICONTROL排名]。 這有助於 [!DNL Workfront] 管理員，以視覺化方式識別與每個存取層級相關聯的複雜性層級。 例如，您可以為較複雜的（[！UICONTROL計畫]層級）存取層級提供較低的數字，為較不複雜的（[！UICONTROL請求者]層級）存取層級提供較高的數字。 您無法將標準存取層級排名。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL就緒]</td> 
   <td> <p>任務報告上的此欄位會指出待處理專案上的[！UICONTROL Agile]任務是否已標籤為[！UICONTROL Ready]。 此旗標僅適用於[！UICONTROL Agile]任務，這些任務是指派給[！UICONTROL Agile]團隊的任務。 </p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[！UICONTROL遞回頻率]</td> 
   <td> <p>顯示於遞回任務父級的[！UICONTROL任務詳細資訊]或[！UICONTROL編輯任務]方塊的欄位。 這是工作週期性發生的頻率。 如需建立週期性工作的相關資訊，請參閱 <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">建立週期性任務</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL參考編號]</td> 
   <td> <p>專案、任務和問題在建立時自動與唯一參考編號相關聯。 您可以在專案、任務或問題的[！UICONTROL詳細資訊]頁面，或清單或報告中檢視[！UICONTROL參考編號]。 </p> <p><b>秘訣</b><p><br>當兩個專案具有相同的名稱時，您可以延遲參考編號，因為參考編號始終是唯一的。 </p> <p>[!DNL Workfront] 系統層級會自動產生循序參考編號。 每個專案、任務或問題都會取得序列中的下一個可用編號。 <br></p> <p>例如，如果使用者A建立任務， [!DNL Workfront] 可能會自動將參考編號100指派給任務。 如果使用者B在此之後建立問題， [!DNL Workfront] 將問題指派為參考編號101。 您無法手動編輯參考編號。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL拒絕問題]</td> 
   <td>在專案或任務報告中，這是當專案或任務的核准被拒絕時建立的問題。 如需拒絕問題的相關資訊，請參閱文章 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">建立工作專案的核准流程</a>. </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL剩餘風險成本]</td> 
   <td> <p>顯示專案之[！UICONTROL計畫風險成本]與專案中所有風險之[！UICONTROL實際成本]總和之間差異的專案欄位。 </p> <p>專案的[！UICONTROL剩餘風險成本]是根據下列公式計算：</p> <p><code>[!UICONTROL Remaining Risk Cost] = Project [!UICONTROL Planned Risk Cost] - SUM([!UICONTROL Actual Cost] for all risks)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL重新計畫]</td> 
   <td>變更專案的日期以修復或解決問題。 例如，已擱置幾個月的專案需要重新規劃以反映準確的日期。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL報表]</td> 
   <td>包含指定資訊的圖表或表格 [!DNL Workfront] 物件及其相關屬性。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[！UICONTROL要求]</td> 
   <td> <p>在單一集中佇列中分類的一種問題型別，與持續的工作無關。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[！UICONTROL請求佇列]</td> 
   <td>由流量和分類程式管理的問題待處理專案。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL要求速度]</td> 
   <td>攝入和完成請求的總工作週期時間。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL請求者]</td> 
   <td>通常是授權型別。 擁有請求者授權的使用者可以提交新工作請求，以便在系統中發生。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL保留時間]</td> 
   <td>在使用者個人時間中指定的天數，表示使用者將無法工作。 請參閱「[！UICONTROL非工作日]」。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL解決問題]</td> 
   <td> <p>在問題報告中，在檢視或篩選器中使用此欄位來引用可解決問題的問題。 </p> <p>有關在報告中顯示解析物件的資訊，請參閱 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">在報告中檢視可解析和解析物件資訊</a> 在 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解析與可解析物件概觀 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL解析專案]</td> 
   <td> <p>在問題報告中，在檢視或篩選器中使用此欄位來參照解決問題的專案。 </p> <p>有關在報告中顯示解析物件的資訊，請參閱 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">在報告中檢視可解析和解析物件資訊</a> 在 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解析與可解析物件概觀 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL解析任務]</td> 
   <td> <p>在問題報告中，在檢視或篩選器中使用此欄位來參照解決問題的任務。 </p> <p>有關在報告中顯示解析物件的資訊，請參閱 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">在報告中檢視可解析和解析物件資訊</a> 在 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解析與可解析物件概觀 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL資源]</td> 
   <td>存在於系統中並指派給專案團隊和任務的使用者和/或角色。</td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Resource Estimates</td> 
    <td>This report captures information about an area in&nbsp;Workfront that has been removed. The report might display legacy information but it does not update with current data. Although not recommended, you may update the information in this report using the API. For information about how you estimate resources for projects, see <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>. </td> 
   </tr>
   <td>Resource Grid</td> 
   <td>A visual table showing the allocation of resources.</td> 
  </tr> -->
  <tr> 
   <td>[！UICONTROL資源管理]</td> 
   <td> <p>[！UICONTROL Resource Management]是一組企業工具，可讓您根據資源的可用性準確預測資源的使用情況，以便必須完成的工作能按時且按預算完成。 </p> <p>使用「資源管理」工具，您可以規劃資源的長期產能與短期排程需求。 </p> <p>有關資源管理的資訊，請參閱： [!DNL Workfront]，請參閱 <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">開始使用資源管理</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL資源管理員ID]</td> 
   <td><p>在專案報告中，建立篩選器以尋找特定資源管理員時，可以使用此選項。 </p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL資源管理員]</td> 
   <td> <p>在專案報告或清單檢視中，這是一個資訊欄位，顯示指定要在專案上執行資源管理活動的使用者。  當您在報告中使用「[！UICONTROL資源管理員]」時，會顯示資源管理員清單，專案上的每個資源管理員之間會以逗號分隔。 您最多可以在指定專案上指定30名資源管理員。</p> <p>如需詳細資訊，請參閱文章 <a href="../../../manage-work/projects/planning-a-project/designate-resource-managers-for-projects-and-templates.md">為專案或範本指定資源管理員 </a>.</p> </td> 
  </tr>
  <tr> 
   <td>[！UICONTROL資源規劃工具預算時數] </td> 
   <td>[！UICONTROL資源規劃工具]中為專案編列的時數及與其關聯的資源。 另請參閱本文中的「[！UICONTROL預算時數]」。 </td> 
  </tr>  
  <tr> 
   <td>[！UICONTROL資源規劃工具] </td> 
   <td>進階 [!DNL Workfront] 此工具可讓您檢視和管理跨專案、工作角色或使用者的資源。 如需詳細資訊，請參閱 <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">資源規劃工具概觀</a>. </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL資源規劃工具預算勞力成本]</td> 
   <td> <p>這些是使用資源規劃工具之專案工作角色的預算時數相關聯的成本。 </p> <p>另請參閱本文中的「預算勞力成本」。 </p> </td>

</tr> 
  <tr> 
   <td>[！UICONTROL資源集區]</td> 
   <td> <p>資源集區是可與專案相關聯的使用者集合。相同資源集區中的使用者通常屬於相同部門、具有類似或互補的技能，或由相同預算提供資金。 您可以將多個資源集區與專案或使用者建立關聯。 資源集區可以專門指派給專案，或由多個專案共用。</p> 
   <p>如需資源集區的詳細資訊，請參閱 <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> 資源集區概觀 </a>.</p> 
   <p>在專案報表中，「資源集區」會顯示與專案相關的所有集區。 此物件無法用於群組。</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL資源使用率]</td> 
   <td>顯示特定時段內可用時數的報告，以及報告中為每個使用者排程的時數。 此數值也會計算為[！UICONTROL每日平均時數]以及配置百分比。</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[！UICONTROL結果]</td> 
   <td>在 [!DNL Workfront Goals]，結果便會是目標的進度指示器。 可以是您手動更新的數字、百分比值或貨幣金額。 您無法在報告中顯示結果，也無法透過存取這些結果 [!DNL Workfront] API。 如需活動的相關資訊，請參閱 <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">開始使用Adobe Workfront目標中的結果和活動</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL收入]</td> 
   <td>任務或專案的可記帳金額。 金額可以是每小時、固定或兩者的組合。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL收入型別]</td> 
   <td>收入型別會決定任務應計收入的方式。 某些範例包括[！UICONTROL固定小時]、[！UICONTROL角色小時]和[！UICONTROL角色小時（上限）。 如需有關追蹤收入的資訊，請參閱： [!DNL Workfront] 另請參閱 <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">帳單與收入概要</a>.</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL檢閱者]</td> 
   <td>通常是授權型別。 擁有[！UICONTROL Reviewer]授權的使用者可以檢閱和核准系統中的工作專案。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL風險]</td> 
   <td> <p>以下內容可能涉及以下概念： [!DNL Workfront]：</p> 
    <ul> 
     <li> <p>專案上指出專案風險程度的欄位。 您可以根據風險等級，排定專案執行的優先順序。 專案可能具有以下風險等級：</p> <p>- [！UICONTROL非常低]</p> <p>- [！UICONTROL低]</p> <p>- [！UICONTROL Medium]</p> <p>- [！UICONTROL高]</p> <p>- [！UICONTROL非常高]</p> <p>您為專案指定的風險層級無法自訂。 </p> <p> 如需更新專案風險的詳細資訊，請參閱文章的「專案設定」一節 <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">編輯專案</a>. 您可以在報告中顯示專案的風險欄位。 </p> </li> 
     <li> <p>在專案存留期內可能發生的事件，可識別對專案的成本、範圍或排程的潛在影響。 您定義專案的潛在風險，並在建立專案的「業務案例」時，將其發生的機率或成本建立關聯。 如需關於將風險新增至專案之業務案例的資訊，請參閱「建立及編輯專案的風險」。 </p> <p>您無法在報表中顯示[！UICONTROL業務案例]中定義的風險。 您只能在報表和清單中顯示數種風險成本。 </p> </li> 
    </ul> </td>

</tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL風險成本]</td> 
   <td> <p>與專案風險相關的成本。 以下是與您可在報表中顯示的專案相關的風險成本：</p> 
    <ul> 
     <li> <p>[！UICONTROL實際成本]：顯示已發生風險之實際成本的風險欄位。 除了報告和清單之外，在編輯或建立風險時，您還可以在[！UICONTROL編輯風險]方塊中找到它。 </p> <p>如需專案、任務或問題成本，請參閱本文中的「[！UICONTROL實際成本]」。 </p> </li> 
     <li> <p>[！UICONTROL計畫風險成本]：顯示專案所有[！UICONTROL潛在風險成本]總計的專案欄位。 另請參閱本文中的「[！UICONTROL計畫風險成本]」。 </p> <p>如需潛在風險成本的相關資訊，請參閱 <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">計算潛在風險成本 </a>. </p> </li> 
     <li> <p>[！UICONTROL剩餘風險成本]：專案上顯示所有風險的[！UICONTROL實際成本]總計與[！UICONTROL計畫風險成本]之間差額的欄位。 另請參閱本文章的「剩餘風險成本」。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL風險管理]</td> 
   <td>識別、緩解及監控風險的程式。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL角色]</td> 
   <td>請參閱本文章的「[！UICONTROL工作角色]」。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL路由]</td> 
   <td>自動指派或移動問題，通常是因為「佇列主題」或是「佇列的預設路由（路由規則）」。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL路由規則]</td> 
   <td>專案和佇列中的設定，可自動將問題指派給使用者、角色或團隊，或將問題移動到另一個專案或佇列。 路由規則通常用於服務檯佇列，以自動指派傳入的問題。</td> 
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
   <td>[！UICONTROL已儲存搜尋]</td> 
   <td>已儲存搜尋條件的搜尋。 「已儲存的搜尋」可讓您輕鬆地再次執行相同的搜尋，而不必再次輸入搜尋條件。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[！UICONTROL Scenario] (在 [!DNL Workfront Fusion]) </td> 
   <td> <p>案例由一系列步驟（模組）組成，這些步驟（模組）指出應如何在應用程式/服務之間傳輸和轉換資料。</p> <p>如需中情境的相關資訊 [!DNL Workfront Fusion]，請參閱 <a href="../../../workfront-fusion/scenarios/scenario-overview.md" class="MCXref xref">[!DNL Adobe Workfront Fusion] 案例概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Scenario] (在 [!DNL Workfront Scenario Planner]) </td> 
   <td> <p>在 [!DNL Scenario Planner]，案例是計畫的副本。 </p> <p>此 [!DNL Scenario Planner] 需要額外的授權。 如需關於以下專案的資訊： [!DNL Workfront Scenario Planner]，請參閱 <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">此 [!DNL Scenario Planner] 概觀</a>. </p> <p>如需建立情境的相關資訊，請參閱 <a href="../../../scenario-planner/create-and-compare-scenarios-for-a-plan.md">在中建立和比較計畫案例 [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL排程]</td> 
   <td>每週工作排程，包括工作時間，以及休息日（例如假日）和例外日（例如星期六工作日）。 時程表可套用至專案和使用者。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL排程劐免]</td> 
   <td>也稱為[！UICONTROL Modified Shift]。 排程的天數，與排程所定義的一般每週工作時間相反。 例如，排程工作的星期六，當排程設定為只工作星期一到星期五時，將是[！UICONTROL排程劐免]。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL排程報告]</td> 
   <td> <p>當您建立報表報表時，如果使用[！UICONTROL排程報表]欄位排程傳送報表，則可以顯示報表排程的相關資訊。 此欄位在專案符號清單中顯示多個值，每個報告的每個排程顯示一個。 如需排程報告的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md" class="MCXref xref">報告傳遞概觀</a>.</p> <p>由於此欄位顯示多個值，因此無法用於分組。 您只能在篩選或檢視中存取。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL範圍變更]</td> 
   <td>一種[！UICONTROL稽核軌跡]，如果作用中，會在任何時候變更專案或任務的範圍時產生備註，例如[！UICONTROL任務持續時間]或[！UICONTROL前置任務]已變更。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL區段]</td> 
   <td>畫面上具有自己標題的區域已建立，可用來組織自訂資料以供顯示。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL分割槽符號]</td> 
   <td>區段之間的間隙或邊框。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL安全性]</td> 
   <td>可讓使用者與系統中的特定物件互動（而非其他物件）的設定。 另請參閱本文章的「[！UICONTROL存取層級]」。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL設定]</td> 
   <td>管理員可以設定系統組態和偏好設定的區域。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL嚴重程度]</td> 
   <td> <p>[！UICONTROL Severity]表示專案影響工作完成的可能性。 例如，高[！UICONTROL嚴重性]的問題可能會完全封鎖任務的完成，但低[！UICONTROL嚴重性]的問題可能只是表面上的。</p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/issues/issue-information/update-issue-severity.md" class="MCXref xref"> 更新問題嚴重程度</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL嚴重程度]</td> 
   <td>請參閱本文章的「[！UICONTROL嚴重程度]」。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL共用]</td> 
   <td>允許其他使用者檢視或編輯中特定專案的動作 [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROLSlack日期]</td> 
   <td>在任務檢視或報告中，[！UICONTROLSlack日期]會顯示任務肯定會影響專案的[！UICONTROL完成日期]的確切日期。 如需有關任務的[！UICONTROLSlack日期]的資訊，請參閱 <a href="../../../manage-work/tasks/task-information/task-slack-date.md" class="MCXref xref">任務Slack日期總覽</a>.</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL智慧指派]</td> 
   <td> <p>將任務或問題指派給使用者時， [!DNL Workfront] 根據最佳使用者完成工作可用的時間及其與專案的關係，提供建議（[！UICONTROL智慧指派]）。</p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/tasks/assign-tasks/smart-assignments.md" class="MCXref xref">智慧指派總覽</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL來源]</td> 
   <td> <p>表示另一個物件的父物件。 例如，附加到任務的檔案具有在[！UICONTROL檔案]報告或檢視的[！UICONTROL來源]欄位中的任務名稱；在專案底下記錄的問題具有在問題報告或檢視的[！UICONTROL來源]欄位中的專案名稱。 </p> 
   <p>下列報表會顯示「來源」欄，您可以在其中檢視父物件的相關資訊：</p>
  <ul><li>問題報告</li>
    <li>小時報告</li>
    <li>檔案報告 </li>
    </ul>
   <p>如果使用者無權存取問題、小時或檔案的父物件，則報告的「來源」欄會顯示空白，即使報告已設定為顯示，或要使用其他使用者的存取許可權傳送。 </p>
   <p> 為了在報告中顯示有關父物件的資訊，我們建議為父物件新增一欄，您可以在其中顯示父物件的名稱。 </p>
    <p>例如，您可以新增下列任何專案至具有來源欄的報表： </p>
    <ul><li>檔案或時數報告的「專案名稱」、「任務名稱」或「問題名稱」欄。</li>
    <li>問題報告的「專案名稱」或「任務名稱」欄。 </li> </ul>
    如需詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md">使用其他使用者的存取許可權執行並傳遞報告</a>

</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL開始日期]</td> 
   <td> <p>專案上的工作設定為開始的日期。 中有數個開始日期 [!DNL Workfront]： </p> 
    <ul> 
     <li>[！UICONTROL計畫]</li> 
     <li>[！UICONTROL實際]</li> 
     <li>[！UICONTROL專案] </li> 
    </ul> <p>在[！UICONTROL費率報表]中，這是專案層級工作角色的新計費率開始的日期。 在此日期之後與專案相關聯的時數，會乘以此收費率，以計算專案的收入。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL狀態]</td> 
   <td> <p>用於表示工作專案或策略目標的工作流程位置的指標。</p> <p>對於專案，[！UICONTROL Status]是專案上的設定，可指出專案是否為：</p> 
    <ul> 
     <li>[！UICONTROL目前]</li> 
     <li>[！UICONTROL保留] </li> 
     <li>[！UICONTROL完成] </li> 
     <li>[！UICONTROL已廢棄]</li> 
    </ul> <p>如需專案狀態的詳細資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md">存取系統專案狀態清單</a>.</p>
    <p>對於任務，[！UICONTROL Status]是任務上的設定，指出任務是否為：</p> 
    <ul> 
     <li>[！UICONTROL新增]</li> 
     <li>[！UICONTROL進行中]</li> 
     <li>[！UICONTROL完成]</li> 
    </ul> <p>有關任務狀態的詳細資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md">存取系統任務狀態清單</a></p> <p>對於問題，[！UICONTROL Status]是問題上的設定，可指出此問題是否為：</p> 
    <ul> 
     <li>[！UICONTROL新增]</li> 
     <li>[！UICONTROL進行中]</li> 
     <li>[！UICONTROL等待回饋]</li> 
     <li>[！UICONTROL保留]</li> 
     <li>[！UICONTROL已解決]</li> 
     <li>[！UICONTROL無法解析]</li> 
     <li>[！UICONTROL無法複製]</li> 
     <li>[！UICONTROL已驗證完成]</li> 
     <li>[！UICONTROL已重新開啟]</li> 
    </ul> <p>如需問題狀態的詳細資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">存取系統問題狀態清單</a>.</p> 
    <p>對於策略目標，[！UICONTROL Status]是目標上的設定，可指出目標是否為：</p> 
     <ul> 
      <li>[！UICONTROL作用中]</li> 
      <li>[！UICONTROL草稿]</li> 
      <li>[！UICONTROL非使用中]</li> 
      <li>[！UICONTROL已關閉]</li> 
     </ul> 
     <p>如需策略目標的詳細資訊，另請參閱本文中的「[！UICONTROL目標]」或「[！UICONTROL目標]」。 </p> 
     <p>對於策略目標，此欄位僅在您的組織已購買時可見 [!DNL Workfront Goals]. 有關使用管理策略目標的資訊 [!DNL Workfront Goals]，請參閱 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] 概觀</a>. </p>
    </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL狀態變更]</td> 
   <td>[！UICONTROL稽核軌跡]。 當使用者變更專案、任務或問題的狀態時會產生附註。</td> 
  </tr> 
  <tr> 
   <td>狀態圖示</td> 
   <td> <p>您可以將內建的[！UICONTROL狀態圖示]欄位新增為檢視中的欄，以增進有關物件的關鍵點的可見度，例如：</p> 
    <ul> 
     <li>物件已附加檔案</li> 
     <li>物件與核准流程相關聯</li> 
     <li>物件具有與其相關的其他附註</li> 
     <li>費用是可記帳或可退還 </li> 
     <li>任務在關鍵路徑上</li> 
     <li>使用者屬於公司、團隊或位於不同時區 </li> 
    </ul> <p>您可以在下列物件的檢視中新增[！UICONTROL狀態圖示]欄位： </p> 
    <ul> 
     <li>[！UICONTROL工作]</li> 
     <li>[！UICONTROL問題]</li> 
     <li>[！UICONTROL專案]</li> 
     <li>[！UICONTROL範本任務]</li> 
     <li>[！UICONTROL範本]</li> 
     <li>[！UICONTROL費用]</li> 
     <li>[！UICONTROL檔案]</li> 
     <li>[！UICONTROL使用者]</li> 
    </ul> <p>如需詳細資訊，請參閱 <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">檢視中的內建狀態圖示</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL狀態更新]</td> 
   <td> <p>此欄位顯示使用者在'[！UICONTROL更新狀態]'欄位中提供的最新狀態更新。 對狀態更新所做的評論不會顯示在[！UICONTROL狀態更新]欄中。</p> <p>若要顯示'[！UICONTROL New]、' '[！UICONTROL In Process]，'和'[！UICONTROL Complete]'狀態，請使用[！UICONTROL Status]資料行。</p> <p>對狀態更新所做的評論不會顯示在[！UICONTROL狀態更新]欄中。</p> <p>如需狀態的詳細資訊，請參閱文章 <a href="../../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">更新任務狀態</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL狀態]</td> 
   <td>請參閱本文章的「[！UICONTROL狀態]」。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[！UICONTROL Storyboard]</td> 
   <td>代表劇本狀態（敏捷方法中的任務）及其完成進度的圖表。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[！UICONTROL劇本時數]</td> 
   <td>用來測量「故事」的難度或複雜性的量度。 敏捷團隊可以選擇使用小時或點。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[！UICONTROL劇本點]</td> 
   <td>用來測量「故事」的難度或複雜性的量度。 敏捷團隊可以選擇使用小時或點。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[！UICONTROL Strategic]</td> 
   <td>改變組織或組織運作方式的長期工作。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[！UICONTROL策略對齊]</td> 
   <td>衡量和調整跨投資組合和計畫的公司目標。</td> 
  </tr>

<tr> 
   <td><code>[!UICONTROL stretch]</code></td> 
   <td><p>使用「文字模式」介面時，這可用於報表欄。 </p>
   <p>此 <code>[!UICONTROL stretch]</code> 用於識別哪些欄佔用了檢視不需要的額外空間。 一般使用者的工作區使用者介面寬度約為850畫素。 這表示如果您有一個檢視包含四個欄（每個欄150畫素），則您的檢視會佔用600個（共850個畫素）。 UI中有250個額外的畫素將會新增至提供延伸百分比的欄。 </p>
   <p>當您使用其他程式碼行時，會強制實施欄的延伸： <code>[!UICONTROL usewidths=true]</code> 至少為檢視中的其中一欄。 
   </td> 
  </tr>

<tr> 
   <td>[！UICONTROL訂閱者]</td> 
   <td> <p>訂閱專案、任務或問題的使用者。</p> <p>當您在報告中使用此欄位時，會顯示訂閱者清單，每個訂閱者之間會以逗號分隔。</p> <p>如需詳細資訊，請參閱文章 <a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref">訂閱中的專案 [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL摘要任務]</td> 
   <td>請參閱本文章的「[！UICONTROL父系任務]」。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL子任務]</td> 
   <td>位於父系任務下方的子系任務。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[！UICONTROL系統管理]</td> 
   <td>一組管理系統變更和維護的原則。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[！UICONTROL系統整合]</td> 
   <td>將不同的運算系統與軟體應用程式在實體或功能上連結在一起的程式，以協調整體運作。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[！UICONTROL任務]</td> 
   <td> <p>作為達成最終目標（完成專案）的步驟而必須執行的活動。</p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/tasks/task-information/tasks-overview.md" class="MCXref xref">任務總覽</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL任務屬性]</td> 
   <td>與「任務」相關聯並指示有關「任務」之特定詳細資訊的其他欄位或物件。 例如[！UICONTROL規劃完成日期]和[！UICONTROL狀態]。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL任務限制]</td> 
   <td>請參閱「[！UICONTROL限制型別]」和「[！UICONTROL限制日期]」。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[！UICONTROL任務管理]</td> 
   <td>一組原則，用來管理任務建立、指派、關閉和可見度的臨界值。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[！UICONTROL任務所有者]</td> 
   <td>負責預估工作量和任務完成的團隊或使用者</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[！UICONTROL團隊]</td> 
   <td> <p>致力達成類似目標或業務目標的使用者集合。 透過將團隊指派給工作專案，可以將這些使用者集體指派給工作專案。</p> <p>如需有關Teams的詳細資訊，請參閱 <a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref">團隊概述</a>.</p> <p>專案可以有一個[！UICONTROL專案團隊]，其中包含與專案工作相關的所有使用者或角色。</p> <p>如需有關專案團隊的詳細資訊，請參閱 <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">專案團隊概觀</a></p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode,SnippetConitions_MaturityModel.Ad hoc"> 
    <td>Team Goals</td> 
    <td>Team goals which contribute to the metrics of enterprise or department goals.</td> 
   </tr>
  --> 
  <tr> 
   <td>[！UICONTROL範本]</td> 
   <td> <p>專案範本是您最可重複專案的一般大綱。 建立專案範本時，您可以定義任務、佇列主題、自訂表單、附加檔案或核准，以節省您必須建立新專案的時間。 </p> <p>您可以將範本附加至現有專案，也可以使用它們來建置新專案。 範本上指定的所有資訊都會傳輸到使用它建立的專案。 </p> <p>如需範本的詳細資訊，請參閱 <a href="../../../manage-work/projects/create-and-manage-templates/project-template-overview.md">專案範本概觀</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL範本任務]</td> 
   <td>屬於範本一部分的任務。 範本任務成為使用範本建立的專案中的任務。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL執行緒]</td> 
   <td>與特定主題有關的[！UICONTROL備註]及其回覆集合。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL縮圖]</td> 
   <td> <p> 在[！UICONTROL Document]清單或報表中，它會在縮圖中顯示檔案的預覽。 </p> <p> 選取 <strong>[！UICONTROL縮圖]</strong>  在報表中檢視33至66畫素寬的縮圖。 </p> <p>當您修改清單或報表中的欄寬時，縮圖的大小會隨之調整。</p> <p>另請參閱本文中的「[！UICONTROL大型縮圖]」。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL休假]</td> 
   <td>您可以建立[！UICONTROL休假]報表，以檢視使用者在其設定檔中表示休假的時間。 </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL時間表]</td> 
   <td> <p>可讓使用者輸入在專案、任務或問題上所花費的實際時數，或在與工作無關的其他活動（例如會議或訓練）上所花費的時數。 除了輸入工作所花費的時間之外，您還可以使用「小時型態」來定義您的時間專案，指出時間是否與工作相關，或相當於製造費用時間。 如需時程表的詳細資訊，請參閱 <a href="../../../timesheets/timesheets/timesheets-overview.md">時程表總覽</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL週期性時程表]</td> 
   <td> <p>[！UICONTROL週期性時程表是範本， [!DNL Workfront] 使用自動為與其相關聯的使用者建立時間表。 </p> <p>您可以設定一些設定，以便在建立每個時程表時套用至該時程表。 其中有些設定是：時程表的建立頻率（每週、每兩週、每月或每月兩次）、時程表的開始日期、時程表核准者、使用者可與記錄時數建立關聯的可用[！UICONTROL小時型別]。</p> </td> 
  </tr> 
  <tr > 
   <td>[！UICONTROL上層父系ID] </td> 
   <td> <p>此欄位可讓您識別及篩選清單或報告中頂層群組及其子群組的相關資料。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL上層父級名稱] </td> 
   <td> <p>此欄位可讓您為清單或報告識別[！UICONTROL檢視]中有關頂層群組及其子群組的資料。</p> <p>您也可以使用[！UICONTROL上層父項ID]欄位執行此操作。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL總時數]</td> 
   <td> <p>在[！UICONTROL專案報告]中，此欄位會顯示專案上所有時數的四捨五入總和（即上次計算專案財務的時間）。 [！UICONTROL實際時數]反映專案上記錄的準確時數。 通常[！UICONTROL實際時數]應與[！UICONTROL總時數]相符。 如果[！UICONTROL總時數]與[！UICONTROL實際時數]欄位顯示顯著不同，您必須重新計算專案的財務。</p> <p>如需重新計算專案財務的詳細資訊，請參閱文章 <a href="../../../manage-work/projects/project-finances/recalculate-project-finances.md" class="MCXref xref">重新計算專案財務</a>.</p> <p>在時程表[！UICONTROL標準]檢視中，此欄位是指在時程表上顯示的日期內為專案記錄的總時數。 此內建檢視中時程表的[！UICONTROL總時數]欄位會參照「[！UICONTROL hoursDuration]」欄位，動態計算時程表開始日期與結束日期之間的時數差異。 如果使用者記錄的時間超過時程表時間範圍內的可用時數，這會以紅色顯示[！UICONTROL總時數]欄。 如需詳細資訊，請參閱 <a href="../../../timesheets/create-and-manage-timesheets/view-total-hours-timesheets.md" class="MCXref xref">在時程表上檢視總時數</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL追蹤模式]</td> 
   <td> <p>任務的屬性。 這會決定如何更新「任務」的「專案」時間表，以及何時更新。 例如：</p> 
    <ul> 
     <li>[！UICONTROL使用者必須更新]要求手動更新任務。 否則，它將變成[！UICONTROL Backed Schedule]，然後[！UICONTROL Late]。</li> 
     <li>到期日[！UICONTROL規劃完成日期]過後，[！UICONTROL自動完成]將自動完成任務。</li> 
    </ul> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">任務追蹤模式概觀</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[！UICONTROL觸發程式]</td> 
   <td>啟動情境的事件。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL問題任務]</td> 
   <td>條件為[！UICONTROL Late]、[！UICONTROL落後於排程]或[！UICONTROL有風險]的未完成任務。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL未指派任務]</td> 
   <td>未指派給任何使用者、角色或團隊的任務。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL更新型別]</td> 
   <td> <p>專案上決定重新計算專案預計時間表時間的設定。 選項包括：</p> 
    <ul> 
     <li>[！UICONTROL Automatic and On Change]</li> 
     <li>[！UICONTROL Automatic Only]</li> 
     <li>[！UICONTROL手冊] </li> 
    </ul> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">選取專案更新型別 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL使用者]</td> 
   <td>在中建立的帳戶 [!DNL Workfront] 允許人員登入並與系統互動。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[！UICONTROL使用者委派]</p> </td> 
   <td> <p>可報告物件，可告訴您：</p> 
    <ul> 
     <li>哪些使用者已委派任務、問題和專案核准</li> 
     <li>哪些使用者擁有委派給他們的任務、問題和專案核准</li> 
     <li>當這些委派開始和結束時</li> 
    </ul> <p>若要深入瞭解，請參閱 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md" class="MCXref xref">建立使用者委派報告</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL使用者介面]</td> 
   <td>的所有視覺和互動層面 [!DNL Workfront] 應用程式。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL使用者介面喜好設定]</td> 
   <td>[！UICONTROL使用者介面設定]。 [!DNL Workfront] 管理員可以變更這些設定，以自訂使用者介面的各個方面。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[！UICONTROL使用率]</td> 
   <td>使用者或角色的可用性，根據指派的排程、PTO和目前的工作負載。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL使用者使用率]</td> 
   <td> <p>與顯示使用者（資源）如何配置或過度配置的報表結合的搜尋。 請參閱本文章的「[！UICONTROL資源使用率]」。</p> </td> 
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
   <td>[！UICONTROL Velocity]</td> 
   <td>測量總工作週期時間（完成一件工作需要多長時間）以及在最初認可的時間內完成工作的頻率（工作與認可的比率）。</td> 
   </tr> 
  <tr> 
   <td>[！UICONTROL檢視]</td> 
   <td> <p>檢視可用於修改報告或專案、任務或問題清單中的欄，或者可用於指示使用者僅有權檢視存取層級或許可權共用層級的資訊。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL檢檢視示]</td> 
   <td> <p> 此欄位與狀態圖示相同，但僅適用於下列檢視： </p> 
    <ul> 
     <li> [！UICONTROL檔案] </li> 
    </ul> <p> 如需詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">檢視中的內建狀態圖示</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL上個月檢視次數]</td> 
   <td> <p>在報表清單中，它會顯示上個月期間檢視報表的次數。<br>如需報告清單使用資訊的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">檢視報告使用量</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL上一季的檢視次數]</td> 
   <td>在報表清單中，它會顯示上個季度檢視報表的次數。<br>如需報告清單使用資訊的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" >檢視報告使用量</a>.</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL去年檢視次數]</td> 
   <td>在報表清單中，它會顯示去年期間檢視報表的次數。<br>如需報告清單使用資訊的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">檢視報告使用量</a>.</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL本月檢視次數]</td> 
   <td> <p>在報表清單中，它會顯示本月期間報表被檢視的次數。<br>如需報告清單使用資訊的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">檢視報告使用量</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL本季檢視次數]</td> 
   <td>在報表清單中，它會顯示本季期間報表被檢視的次數。<br>如需報告清單使用資訊的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">檢視報告使用量</a>.</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL今年檢視次數]</td> 
   <td>在報表清單中，它會顯示今年期間報表被檢視的次數。<br>如需報告清單使用資訊的詳細資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md">檢視報告使用量</a>.</td> 
  </tr>

<tr>
  <td> <code>[!UICONTROL width]</code>
  </td>
<td> 在報表中使用[！UICONTROL文字模式]介面時，您可以在其中指定每欄寬度（以畫素為單位）的程式碼行。 Workfront會提供每個欄位的建議寬度，不過根據欄位型別和格式，您可能需要進行調整。
您必須使用 <code>[!UICONTROL usewidths=true]</code> 強制使用為欄指定的寬度的程式碼行。 
  </td>

</tr>

<tr> 
   <td><code>[!UICONTROL work]</code> </td> 
   <td> <p>在專案、任務或問題報告中，在文字模式下使用以下陳述式會顯示專案、任務或問題的規劃時數：</p>
   <code><p>valuefield=work</p>
   <p>valueformat=HTML</p></code> 
   <p>如需有關使用文字模式的資訊，請參閱 <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">文字模式語法概觀</a>. </p> 
   <p><b>秘訣</b> 
   <p>在問題報告中，新增其中一個[！UICONTROL規劃時數]欄位會新增 <code>work </code>欄位至報表。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL作品]</td> 
   <td> <p>兩種主要授權型別之一。 這比[！UICONTROL Plan]的存取許可權少，但可以在系統中建立和進行更新。 這比[！UICONTROL External]、[！UICONTROL Reviewer]或[！UICONTROL Requester]授權型別更具功能。</p> <p>如需詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] 授權總覽</a>.</p> <p>工作可能指的是一個專案、任務或問題的[！UICONTROL計畫時數]。 如需詳細資訊，請參閱此表格中的「[！UICONTROL工作]」欄位。 </p> <p>提示：在問題報告中，新增其中一個[！UICONTROL規劃時數]欄位會新增 <code>work </code>欄位至報表。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL工作分解結構]</td> 
   <td>專案團隊根據父項/子項關係執行任務的階層結構。</td> 
   </tr> 
  <tr> 
   <td>[！UICONTROL工作量] </td> 
   <td> 
    <p>專案經理可能會決定使用此欄位而不是[！UICONTROL計畫時數]來預估完成任務所需的工作。 只有在符合下列條件時，才會顯示此欄位：</p> 
     <ul> 
      <li> <p>任務具有[！UICONTROL簡單期間型別]。 </p> <p>提示：如果您將任務[！UICONTROL期間型別]更新為任何其他型別，此欄位會變成隱藏。 </p> </li> 
      <li>專案經理已啟用[！UICONTROL使用工時]以自動計算專案上的任務[！UICONTROL計畫時數]欄位。 </li> 
     </ul> 
     <p>如需有關使用[！UICONTROL工作量]而非[！UICONTROL計畫時數]來預估工作量的資訊，請參閱 <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">工作投入概觀</a>. </p> 
     <p>您可以在任務報告和清單中顯示此欄位。</p> 
    </td> 
   </tr> 
  <tr> 
   <td>[！UICONTROL工作專案]</td> 
   <td> <p>此欄位是指中的任務或問題 [!DNL Workfront]. </p> <p>[！UICONTROL工作專案]報告顯示任務和問題的資訊。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL工作管理組合]</td> 
   <td>分配至業務執行與變更業務的工作比例的[！UICONTROL工作績效指標] (WPI)。 Mix WPI可協助您在組織層級瞭解您的策略是否套用任何實際的工作配置。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL工作管理資源]</td> 
   <td>系統中有資格接收工作或追蹤時間的角色指定。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL工作管理角色和職責]</td> 
   <td>定義管理指定問題、任務、專案、方案或投資組合的範圍、執行和核准的所有者和關係人。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL工作管理SLA]</td> 
   <td>所有利害關係人同意的可量化的量度。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL工作管理利害關係人]</td> 
   <td>在工作請求的結果中具有既得利益的使用者集合。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL工作管理接觸點]</td> 
   <td>利害關係人之間通訊的數位化記錄。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL工作績效指標] </td> 
   <td> <p>混合比例、容量、速度、品質和參與度。</p> <p>WPI是[！UICONTROL工作績效指標]的常見首字母縮寫。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL工作流程]</td> 
   <td> <p>接收、排定優先順序及執行工作的方法。 您執行工作的方式通常稱為「工作流程」或「專案計畫」（具有日期、前置任務關係等任務的清單）。 </p> <p>工作流程的範例可能是單一資產的製作或多資產行銷活動的傳送。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL工作流程範本]</td> 
   <td>在[！UICONTROL校訂核准]報告中，此欄位顯示附加到校訂的任何工作流程範本。 如果沒有附加範本，欄為空白。</td> 
  </tr>

<tr> 
   <td>[！UICONTROL工作時間]</td> 
   <td>

<p>代表使用者可用於實際工作（不包括額外負荷）的相當於全職([！UICONTROL FTE])時間百分比。 [！UICONTROL工作時間]必須是十進位數字，最多為1，而且不能為0。 例如，實際工作的20%可用性為0.2。</p>
   </p>該欄位的預設值為1，表示使用者將其全部[！UICONTROL FTE]花費在實際的專案相關工作上。  </p>
   <p>系統會使用此數字來計算使用者是否可以使用實際專案相關工作。 </p>
   <p> 排程例外狀況與休假也可能會影響使用者容量。 </p>
   <p>如需在Workfront中建立排程的詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">建立排程</a>. </p>
    <p>Workfront會根據[！UICONTROL設定]區域中的「資源管理」偏好設定來計算使用者的可用性。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md/">設定資源管理喜好設定</a>. </p> 
   <p>您可以在編輯或建立使用者時更新使用者的[！UICONTROL工作時間]。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">編輯使用者的設定檔</a></p> 
   <b>秘訣</b> 
   <p>將[！UICONTROL工作時間]值設為1，表示使用者可全時從事專案相關工作。</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL工作時間]</td> 
   <td>在Workfront檔案中，此辭彙用於說明根據排程分配的工作時間。</td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL workRequiredExpression]</code> </td> 
   <td> <p>在專案、任務或問題報告中，在文字模式下使用以下陳述式會顯示專案、任務或問題的計畫時數後接「時數」一詞：</p>
   <code>
   <p>valuefield=workRequiredExpression</p>
   <p>valueformat=HTML</p>
   </code>
    <p>如需有關使用文字模式的資訊，請參閱 <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">文字模式語法概觀</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>
