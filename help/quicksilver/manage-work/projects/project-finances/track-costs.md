---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: financials
title: 追蹤成本
description: 您可以在Adobe Workfront中追蹤專案、工作和問題的成本。
author: Alina
feature: Work Management
exl-id: df3090ae-9721-4e9b-84b4-315890619801
source-git-commit: b4bb6306b7fa088823fba8ef5614aae8551ce02c
workflow-type: tm+mt
source-wordcount: '2372'
ht-degree: 1%

---

# 追蹤成本

您可以在Adobe Workfront中追蹤專案、工作和問題的成本。

## Workfront如何計算成本

為了跟蹤成本，您必須將用戶和職務角色與每小時成本率相關聯。

每小時成本比率是與職務或用戶關聯的每個工作單位的成本金額。 將比率乘以工作所花費的小時數，可生成項目、任務或問題的成本。

存在下列情況：

* 如果任務的「成本類型」為「每小時用戶」，則用戶每小時費率將計算任務和項目成本。

   有關將用戶與成本率關聯的資訊，請參閱 [編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* 如果任務的「成本類型」為「每小時職責」，則任務職責每小時費率將計算任務和項目成本。

   有關將任務職責與成本費率關聯的資訊，請參閱 [建立和管理作業角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Workfront只計算問題的實際成本，而問題沒有成本類型。 如需詳細資訊，請參閱 [Workfront如何追蹤問題成本](#how-workfront-tracks-costs-for-issues) 這篇文章。

>[!TIP]
>
>您不能改寫項目的成本比率。 一旦您建立了用戶或任務職責的每小時成本費率，該費率就會計算系統中的所有成本。

## Workfront成本績效索引

Workfront會計算專案的多項成本效益索引，以便追蹤專案以提高成本效益。\
有關計算成本 — 效能索引的詳細資訊，請參閱：

* [計算成本績效指數(CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md)
* [計算成本計畫效能指數(CSI)](../../../manage-work/projects/project-finances/calculate-csi.md)
* [計算計畫效能索引(SPI)](../../../manage-work/projects/project-finances/calculate-spi.md)

## Workfront如何追蹤任務和專案的成本

* [Workfront如何追蹤成本](#how-workfront-tracks-costs)
* [Workfront如何計算計畫、預算和實際成本](#how-workfront-calculates-planned-budgeted-and-actual-costs)
* [Workfront如何計算任務的成本類型](#how-workfront-calculates-cost-types-for-tasks)

### Workfront如何追蹤成本  {#how-workfront-tracks-costs}

您可以追蹤Workfront中任務和專案的數種成本類型。 整體成本按以下公式計算：

```
Costs = Labor Costs + Expense Costs
```

* **人工成本** 與任務和項目的小時數以及與任務關聯的資源的每小時成本率相關聯。 一般而言，Workfront會計算下列人工成本：

   <table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td>計畫人工成本</td> 
     <td> <p>計算公式如下：</p><pre>計畫人工成本=計畫小時數*每小時成本費率</pre> </td> 
    </tr> 
    <tr> 
     <td>預算人工成本</td> 
     <td> <p>計算公式如下：</p><pre>預算人工成本=預算小時數*每小時成本率</pre> </td> 
    </tr> 
    <tr> 
     <td>實際人工成本</td> 
     <td> <p>計算公式如下：</p><pre>實際人工成本=實際小時數*每小時成本費率</pre> </td> 
    </tr> 
   </tbody> 
  </table>

   如需詳細資訊，請參閱 [Workfront如何計算計畫、預算和實際成本](#how-workfront-calculates-planned-budgeted-and-actual-costs) 一節。

* **費用成本** 與項目和任務的費用相關聯。\
   建立項目時，您可以為整個項目設定計畫費用。 此外，您可以將費用與新任務或現有任務關聯。 如需詳細資訊，請參閱 [管理項目費用](../../../manage-work/projects/project-finances/manage-project-expenses.md).

* **固定成本** 定義為項目的固定成本金額。 這是項目計畫成本的一部分，它表示完成項目所需的資金額。

   >[!TIP]
   >
   >將模板附加到項目時，模板的固定成本將添加到項目的固定成本中。 如需詳細資訊，請參閱 [將範本附加至專案的概觀](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md).

### Workfront如何計算計畫、預算和實際成本 {#how-workfront-calculates-planned-budgeted-and-actual-costs}

Workfront會計算項目中每個任務的計畫成本和實際成本。 Workfront將這些計算用於單個任務，以計算項目的計畫成本和實際成本。

* [計畫成本](#planned-cost)
* [預算成本](#budgeted-cost)
* [實際成本](#actual-cost)

#### 計畫成本 {#planned-cost}

項目的計畫成本是與項目上的計畫工作（計畫小時數）相關的成本。

項目的計畫成本按以下公式計算：

```
Planned Project Cost = Planned Labor Cost of all tasks + Planned Expense cost of all tasks + Planned Expense Cost of the project + Fixed Cost of the project
```

例如，任務的「費用」標籤中包含以下費用：$100的行銷費用和$50的管理費用。 在「財務」標籤中，選擇「用戶每小時成本」類型。 系統會為用戶分配任務，用戶的每小時費率為$15。 已將用戶分配給5小時執行此任務。 在項目的「費用」標籤中，名為「咨詢」的費用有$100的計畫成本。 此外，該項目還有$200的固定成本。

項目的計畫成本計算如下：

```
$100 (Consulting Expense) + $100 (Marketing Expense) + $50 (Administrative Expense)+$15(Hourly Rate)*5(Planned Hours Logged) + $200 (Fixed Cost)= $525
```

#### 預算成本 {#budgeted-cost}

項目預算成本是與項目預算工作（預算小時數）相關的成本。

如果滿足以下兩個條件，則項目的預算成本與項目的計畫成本相同：

* 項目上任務的計畫小時數與預算小時數（在Oracle Resource Planner中）相符
* 任務開單類型為每小時角色。

如果滿足以下條件，則使用以下公式計算項目的預算成本：

* 項目上任務的計畫小時數與預算小時數不匹配（在Oracle Resource Planner中）
* 任務的計費類型為「角色每小時」。

當滿足上述條件時，Workfront會使用以下公式計算項目的預算成本：
<pre>預算項目成本=預算人工成本+預算費用所有任務的成本+預算費用項目成本</pre>

#### 實際成本 {#actual-cost}

項目的實際成本是與項目上的實際工作（記錄的小時數）相關的成本。

實際成本使用以下公式計算：

```
Actual Project Cost = Actual Labor Cost of all tasks + Actual Expense Cost of all tasks + Actual Labor Cost of the project + Actual Expense Cost of the project + Fixed Cost of the project
```

例如，任務的「費用」標籤中包含以下費用：a實際成本為$110的市場營銷費用和實際成本為$40的管理費用。 選擇「角色每小時」成本類型，並將「顧問」作業角色分配給該任務。 顧問職務角色的費率為每小時$15，並且顧問職務角色的任務有6小時記錄。 與項目關聯的咨詢費用（在「費用」頁簽中），「實際成本」為$100，「每小時成本」為$20的用戶配置檔案記錄在項目的10小時內。 此外，該項目還有$200的固定成本。

項目的實際成本計算如下：

```
$100 (Consulting Expense) + $110 (Marketing Expense) + $40 (Administrative Expense) +$15 (Hourly Rate)*6 (Actual Hours Logged) + $20 (Cost per Hour rate for the user logging time on the project)*10 (hours the user logs on the project) + $200 (Fixed Cost)= $740
```

>[!NOTE]
>
>在項目上記錄時間時，計算項目的實際人工成本時存在以下情況：
>
>* 預設情況下，Workfront使用用戶的「每小時成本」比率來計算實際人工成本。
>* 如果記錄時間的使用者未與任何成本相關聯，則Workfront會使用使用者主要角色的每小時成本比率。
>* 如果您的Workfront管理員已啟用 **手動將作業角色分配給小時條目** 在「時間表和小時數首選項」區域中設定，並且項目上的用戶登錄時間選擇與此時間關聯的不同角色，則項目的實際成本將根據記錄小時數時指定的角色計算。 有關為特定作業角色啟用記錄時間的資訊，請參閱文章 [配置工時單和小時首選項](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
>


### Workfront如何計算任務的成本類型 {#how-workfront-calculates-cost-types-for-tasks}

任務的計畫成本和實際成本及其人工成本由每項任務的成本類型確定。

您可以為專案內的個別任務配置成本類型。 每個成本類型都會影響計畫成本值和實際成本值。

有關如何修改任務的成本類型的資訊，請參閱 [更新任務成本類型](../../../manage-work/tasks/task-information/update-task-cost-type.md).

下表介紹了Workfront中可用的任務成本類型：

<table border="1" cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>任務成本類型</strong> </p> </th> 
   <th> <p><strong>說明</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>使用者小時</p> </td> 
   <td> <p>這是建立任務時的預設成本類型。</p> <p><strong>計畫成本</strong> 是以下公式計算： </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>如果計畫人工成本的計算方式為：<br><code>Planned Labor Cost = Planned Hours * Cost per Hour Rate of the User assigned to the task</code></p> <p>備註:   <p>請考慮使用用戶每小時成本類型和計算計畫成本的以下影響：</p> 
     <ul> 
      <li>如果為任務分配了多個資源，Workfront將根據分配給每個資源的任務的百分比調整計畫成本的計算。</li> 
      <li>「計畫成本」欄位的值可能會因您從任務本身查看計畫成本還是從「利用率」報表查看計畫成本而有所不同。<br><strong>從任務本身查看計畫成本時：</strong> 「計畫成本」欄位考慮在任務職責層設定的「成本/人力」欄位（當未在用戶層設定「成本/人力」欄位時）。<br><strong>從項目的「利用率」報表中查看計畫成本時：</strong> 「計畫成本」欄位不考慮在「任務職責」層設定的「成本/人力」欄位。 相反，如果希望「利用率」報表考慮在「任務職責」層設定的「成本/人力」欄位，則必須將任務上的「成本類型」設定為「每小時」。 </li> 
     </ul> </p> <p><strong>實際成本</strong> 是以下公式計算： </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>如果按以下方式計算實際人工成本：</p> <p><code>Actual Labor Cost = Actual Hours * Cost per Hour Rate of the User logging the hours</code> </p> <p>例如，使用者的設定檔中的「每小時成本」比率為$20。 當他們為任務記錄5小時時，該任務的實際人工成本為$100。 如果用戶沒有與其關聯的每小時成本費率，則實際成本將根據其主要任務職責的每小時成本費率計算。 如果它們沒有職務職責，或未定義其職務職責的「每小時成本」比率，則任務的「實際成本」為零。 </p> <p>注意：實際成本是根據記錄時間的用戶的每小時成本比率計算的，而不管誰被分配給任務。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>角色小時</p> </td> 
   <td> <p><strong>計畫成本</strong> 是以下公式計算： </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost+ Task Planned Expense Cost</code> </p> <p>如果按以下方式計算任務計畫人工成本：</p> <p><code>Task Planned Labor Cost = Planned Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>注意：如果為任務分配多個資源，Workfront將根據分配給每個資源的任務的百分比調整計畫小時數的計算。</p> <p><strong>實際成本</strong> 是以下公式計算： </p> <p><code style="font-style: normal;">Task Actual Cost = Task Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>如果按以下方式計算任務實際人工成本：</p> <p><code>Task Actual Labor Cost = Actual Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>例如，任務被分配給某個職務角色或具有職務角色的用戶，其每小時成本費率為$20。 當用戶記錄某項任務的5小時時，該任務的實際人工成本為$100。 如果分配給任務的用戶在任務上沒有與他們關聯的任務職責，則實際成本將根據其主要任務職責的每小時成本比率計算。 如果它們沒有職務職責，或未定義其職務職責的「每小時成本」比率，則任務的「實際成本」為零。 </p> <p>備註:   <p> 「角色的實際小時數」任務根據與任務關聯的用戶的作業角色計算，而不是根據與正在記錄時間的用戶關聯的角色計算。</p> <p>如果您的Workfront管理員已啟用 <strong>手動將作業角色分配給小時條目</strong> 在「時間表和小時首選項」區域中設定，並且任務上的用戶登錄時間選擇與此時間關聯的不同角色，則「角色的實際成本」每小時任務將根據記錄小時時指定的角色計算。 有關為特定作業角色啟用記錄時間的資訊，請參閱文章 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">配置工時單和小時首選項</a>.</p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>固定小時</p> </td> 
   <td> <p><strong>計畫成本</strong> 是以下公式計算：</p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>其中任務人工成本的計算方式為：</p> <p><code>Task Planned Labor Cost = Planned Hours * Fixed Hourly Cost of the Task</code> </p> <p><strong>實際成本</strong> 是以下公式計算： </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Task Labor Cost + Task Planned Expense Cost</code> </p> <p>如果按以下方式計算實際任務人工成本：</p> <p><code>Task Actual Labor Cost = Actual Hours * Fixed Hourly Cost of the Task</code> </p> <p>此成本類型不考慮個別使用者或工作角色。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>無成本</p> </td> 
   <td> <p>此成本類型不影響成本。 如果父任務具有此成本類型，則具有另一個成本類型的子任務將根據其各自的成本類型進行計算，並相應地影響父任務的成本。 </p> <p>當沒有金融資料訪問權限的用戶或對模板沒有財務權限的用戶從該模板建立項目時，這是項目任務的預設成本類型。</p> <p>如需存取金融資料的相關資訊，請參閱文章 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">授予金融資料的存取權</a>.</p> <p>有關對象的財務權限的資訊，請參見文章 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">共用物件的財務權限</a>.</p> <p>如需從範本建立專案的相關資訊，請參閱文章 <a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">使用範本建立專案</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted because this was moved to its own how-to article linked above. Could be removed after some time.) </p>
<p>To configure the Cost Type of an individual task:</p>
<ol>
<li value="1">Go to the task where you want to configure the Cost Type. </li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then expand the <strong>Finance</strong> area. </p> </li>
<li value="3"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Double click <strong>Cost Type</strong> and select the cost type that you want to apply to the task. </p> </li>
<li value="4">Click <strong>Save.</strong></li>
</ol>
</div>
-->

## Workfront如何追蹤問題成本 {#how-workfront-tracks-costs-for-issues}

問題不存在，也不影響項目的以下成本類型：

* 計畫成本
* 預算成本

不過，問題可以 **實際成本** 也會影響項目的實際成本。

下表說明了根據問題的分配類型計算問題的實際成本的方法：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th colspan="4">發放實際成本</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>用戶分配</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>實際成本</strong> 是以下公式計算：</p> <p><code style="font-style: normal;">Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>記錄該時間的使用者的每小時成本率會在此考慮，無論指派給問題的人員為何。 </p> <p>如果記錄時間的用戶在其配置檔案中沒有每小時成本費率，則其主要任務職責的每小時成本費率將計算問題的實際成本。 如果正在記錄時間的用戶在其配置檔案中沒有角色，或者沒有與其關聯的費率，則實際小時數將使用主要受託人的主要職務角色在問題上的「成本小時數」比率來計算。 如果該角色未定義費率，則問題的實際成本為零。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>角色分配</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>實際成本</strong> 是以下公式計算：</p><code>Issue Actual Cost = Actual Hours * Cost per Hour Rate of user logging the hours</code> <p>在此處會考慮記錄問題時間的使用者每小時成本比率，而不論指派給問題的角色為何。 </p> <p>如果記錄時間的用戶沒有與其相關聯的每小時成本費率，則其主要職責的每小時成本費率將計算問題的實際成本。<br>如果正在記錄時間的使用者在其設定檔中沒有角色，或沒有與其相關聯的比率，則問題的實際成本為零。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>無指派</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>實際成本</strong> 是以下公式計算：</p> <p><code>Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>如果記錄時間的用戶沒有與其配置檔案關聯的每小時成本率，則其主要任務職責的每小時成本率將計算問題的實際成本。 </p> <p>如果正在記錄時間的用戶沒有與其配置檔案相關聯的作業角色，或者其主要作業角色沒有定義「每小時成本」比率，則問題的實際成本為零。 </p> </td> 
  </tr> 
  <!--<tr data-mc-conditions=""> 
   <td colspan="4"> 
    <div> <MadCap:conditionalText data-mc-conditions="">
       If your Workfront administrator enabled the 
      <strong>Assign Job Roles to hour entries manually</strong> setting in the Timesheets &amp; Hours Preferences area, and the user logging time on the issue selects a different role to associate with this time, the Actual Cost of the issue calculates based on the role specified when the hours were logged. For information about enabling logging time for a specific job role, see the article 
      <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">Configure timesheet and hour preferences</a>. 
     </MadCap:conditionalText> 
    </div> </td> 
  </tr> 
  -->
 </tbody> 
</table>
