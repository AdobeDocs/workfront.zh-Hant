---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: financials
title: 追蹤成本
description: 您可以在Adobe Workfront中追蹤專案、任務和問題的成本。
author: Lisa
feature: Work Management
exl-id: df3090ae-9721-4e9b-84b4-315890619801
source-git-commit: d431ae178a157522e2b5d8d963da7b0623510d28
workflow-type: tm+mt
source-wordcount: '2480'
ht-degree: 0%

---

# 追蹤成本

<!-- Audited: 02/2024 -->

您可以在Adobe Workfront中追蹤專案、任務和問題的成本。

## Workfront如何計算成本

若要追蹤成本，您必須將使用者與職務角色與每小時成本費率產生關聯。

每小時成本率是與工作角色或使用者相關的每個工作單位的成本金額。 將費率乘以工作所花費的時數，會產生專案、任務或問題的成本。

存在下列情況：

* 如果作業的「成本型態」為「使用者小時」，則使用者小時費率會計算作業與專案成本。

  如需將使用者與成本費率建立關聯的資訊，請參閱[編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

* 如果作業的「成本型態」為「每小時角色」，則職務角色每小時費率會計算作業與專案成本。

  如需將職務角色與成本費率產生關聯的資訊，請參閱[建立和管理職務角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)。

* Workfront只會計算問題的實際成本，而問題沒有成本型別。 如需詳細資訊，請參閱本文中[Workfront如何追蹤問題成本](#how-workfront-tracks-costs-for-issues)一節。

>[!TIP]
>
>您無法覆寫專案的成本費率。 一旦您建立了使用者或職務角色的每小時成本費率，該費率就會計算系統中的所有成本。

## Workfront成本績效指數

Workfront會計算專案的許多成本績效指數，以便追蹤專案以符合成本效益。\
如需有關計算成本 — 效能指數的詳細資訊，請參閱：

* [計算成本績效指數(CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md)
* [計算成本排程績效指數(CSI)](../../../manage-work/projects/project-finances/calculate-csi.md)
* [計算排程績效指數(SPI)](../../../manage-work/projects/project-finances/calculate-spi.md)

## Workfront如何追蹤任務和專案的成本

對於任務和專案，成本型別的計算方式不同。

### Workfront如何追蹤成本 {#how-workfront-tracks-costs}

您可以在Workfront中追蹤數種型別的任務和專案成本。 總成本的計算公式如下：

`Costs = Labor Costs + Expense Costs`

* **勞力成本**&#x200B;與任務和專案的時數以及任務相關資源的每小時成本費率相關聯。 一般而言，Workfront會計算下列人工成本：

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td>計畫勞力成本</td> 
     <td> <p>會使用下列公式計算：</p><code>Planned Labor Costs = Planned Hours * Cost per Hour rate</code> </td> 
    </tr> 
    <tr> 
     <td>預算勞力成本</td> 
     <td> <p>會使用下列公式計算：</p><code>Budgeted Labor Costs = Budgeted Hours * Cost per Hour rate</code> </td> 
    </tr> 
    <tr> 
     <td>實際勞力成本</td> 
     <td> <p>會使用下列公式計算：</p><code>Actual Labor Costs = Actual Hours * Cost per Hour rate</code> </td> 
    </tr> 
   </tbody> 
  </table>

  如需詳細資訊，請參閱本文中的[Workfront如何計算計畫、預算與實際成本](#how-workfront-calculates-planned-budgeted-and-actual-costs)一節。

* **費用成本**&#x200B;與專案和工作上的費用相關聯。\
  建立專案時，您可以設定整個專案的計畫費用。 此外，您可以將費用與新任務或現有任務建立關聯。 如需詳細資訊，請參閱[管理專案費用](../../../manage-work/projects/project-finances/manage-project-expenses.md)。

* **固定成本**&#x200B;定義為專案的固定成本金額。 這是專案計畫成本的一部分，代表完成專案所需的金額。

  >[!TIP]
  >
  >將範本附加至專案時，範本的「固定成本」會新增至專案的「固定成本」。 如需詳細資訊，請參閱[將範本附加到專案的總覽](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md)。

### Workfront如何計算計畫、預算與實際成本 {#how-workfront-calculates-planned-budgeted-and-actual-costs}

Workfront會計算專案中每個個別任務的計畫成本與實際成本。 Workfront會針對個別任務使用這些計算，來計算專案的計畫成本與實際成本。

#### 規劃成本 {#planned-cost}

專案的計畫成本是與專案上的計畫工作（計畫時數）相關的成本。

專案的「計畫成本」是以下列公式計算：

`Planned Project Cost = Planned Labor Cost of all tasks + Planned Expense cost of all tasks + Planned Expense Cost of the project + Fixed Cost of the project`

例如，您在任務的「費用」標籤上有以下費用： $100的行銷費用和$50的管理費用。 在「財務」頁標中，選取「使用者每小時」成本型別。 使用者會指派給工作，而且使用者的小時費率為$15。 已指派使用者在此任務上工作5小時。 在專案的費用索引標籤中，您有一個稱為「諮詢」的費用的$100計畫成本。 您還有專案的$200固定成本。

專案的計畫成本計算方式如下：

`$100 (Consulting Expense) + $100 (Marketing Expense) + $50 (Administrative Expense) + $15(Hourly Rate)*5(Planned Hours Logged) + $200 (Fixed Cost) = $525`

公式中的每小時費率會考量費率的任何日期有效變更。

#### 預算成本 {#budgeted-cost}

專案的預算成本是與專案上的預算工作（預算時數）相關的成本。

如果符合以下兩個條件，專案的預算成本與專案的計畫成本相同：

* 專案上任務的計畫時數符合資源規劃工具中的預算時數。
* 任務的計費型別為「每小時角色」。

如果符合下列條件，則會使用下列公式計算專案的預算成本：

* 專案上任務的計畫時數不符合預算時數（在資源規劃工具中）。
* 任務的計費型別為「每小時角色」。

當上述條件符合時，Workfront會使用下列公式計算專案的預算成本：

`Budgeted Project Cost = Budgeted Labor Cost + Budgeted Expense Cost of all tasks + Budgeted Expense Cost of the project`

#### 實際成本 {#actual-cost}

專案的實際成本是與專案實際工時（記錄時數）相關的成本。

實際成本的計算公式如下：

`Actual Project Cost = Actual Labor Cost of all tasks + Actual Expense Cost of all tasks + Actual Labor Cost of the project + Actual Expense Cost of the project + Fixed Cost of the project`

例如，您在任務的「費用」標籤上有以下費用：實際成本為$110的行銷費用以及實際成本為$40的管理費用。 您選取「每小時角色」成本型態，並將「顧問」職務角色指派給作業。 顧問工作角色的費率為$15/小時，且顧問工作角色的工作會記錄6小時。 有一個與專案關聯的諮詢費用（在「費用」標籤中），其實際成本為$100，且使用者設定檔中的每小時成本費率為$20的使用者在該專案上記錄了10小時。 您還有專案的$200固定成本。

專案的實際成本計算方式如下：

`$100 (Consulting Expense) + $110 (Marketing Expense) + $40 (Administrative Expense) +$15 (Hourly Rate)*6 (Actual Hours Logged) + $20 (Cost per Hour rate for the user logging time on the project)*10 (hours the user logs on the project) + $200 (Fixed Cost) = $740`

公式中的每小時費率會考量費率的任何日期有效變更。

>[!NOTE]
>
>專案的實際費用成本計算方式如下：
>`SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs) + Project Fixed Cost`
>
>這些成本在實際成本計算中不會重複。 例如，如果固定成本是專案實際費用成本的一部分，則不會單獨新增到實際成本。

>[!NOTE]
>
>在專案上記錄時間時，計算專案的實際勞力成本時，會出現下列案例：
>
>* 依預設，Workfront會使用使用者的每小時成本費率來計算實際勞力成本。
>* 如果記錄時間的使用者未與任何成本相關聯，則Workfront會使用使用者主要角色的每小時成本費率。
>* 如果您的Workfront管理員在設定的時程表和時數偏好設定區域中手動啟用了&#x200B;**將工作角色指派到時數專案**&#x200B;設定，而且專案上的使用者記錄時間選取了其他要與此時數關聯的角色，則專案的實際成本將會根據記錄時數時指定的角色進行計算。 如需有關啟用特定工作角色的記錄時間的資訊，請參閱文章[設定時程表和小時偏好設定](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)。

### Workfront如何計算任務的成本型別 {#how-workfront-calculates-cost-types-for-tasks}

作業的「計畫成本」與「實際成本」及其人工成本是由每個作業的「成本型態」所決定。

您可以為專案中的個別任務設定「成本型別」。 每種成本型態都會影響計畫成本與實際成本值。

如需有關如何修改任務成本型別的資訊，請參閱[更新任務成本型別](../../../manage-work/tasks/task-information/update-task-cost-type.md)。

下表說明Workfront中可用的作業「成本型別」：

<table style="table-layout:auto">
 <col> 
 <col> 
<tbody> 
  <tr> 
   <td> <p><strong>任務成本型別</strong> </p> </td> 
   <td> <p><strong>說明</strong> </p> </td> 
  </tr>
  <tr> 
   <td> <p>使用者每小時</p> </td> 
   <td> <p>這是您建立作業時的預設「成本型態」。</p> <p><strong>計畫成本</strong>的計算公式如下： </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>其中計畫勞力成本的計算方式：<br><code>Planned Labor Cost = Planned Hours * Cost per Hour Rate of the User assigned to the task</code></p> <p>注意： <p>考慮使用「使用者小時成本型態」與計算計畫成本的下列影響：</p> 
     <ul> 
      <li>如果您將多個資源指定給一個任務，Workfront會根據指定給每個資源的任務百分比，調整「計畫成本」的計算。</li>
      <li>對於日期有效成本率，「計畫勞力成本」是作業所涵蓋之每個時間期間的計畫成本總和。</li>
      <li>視您是從作業本身檢視計畫成本，還是從「使用率」報表檢視「計畫成本」而定，「計畫成本」欄位的值可能會有所不同。<br><strong>從任務本身檢視計畫成本時：</strong>「計畫成本」欄位會考量在「工作角色」層次設定的「成本/小時」欄位（若尚未在使用者層次設定「成本/小時」欄位）。<br><strong>從專案的「使用率」報告檢視計畫成本時：</strong>「計畫成本」欄位未考慮在「工作角色」層次設定的「成本/小時」欄位。 反之，若您想要「使用率」報表考慮在「職務角色」層次設定的「成本/小時」欄位，則必須將作業的「成本型態」設定為「每小時角色」。 </li> 
     </ul> </p> <p><strong>實際成本</strong>的計算公式如下： </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>其中實際勞力成本的計算方式：</p> <p><code>Actual Labor Cost = Actual Hours * Cost per Hour Rate of the User logging the hours</code> </p> <p>例如，使用者在其設定檔中的每小時成本費率為$20。 當他們記錄一項任務的5小時時，該任務的「實際人工成本」為$100。 如果使用者沒有與其相關的每小時成本費率，則實際成本會根據其主要職務角色的每小時成本費率計算。 如果他們沒有工作角色，或未定義其工作角色的「每小時成本」費率，則任務的「實際成本」為零。 </p> <p>備註：實際成本是根據記錄時間之使用者的「每小時成本」費率來計算，而不論指派給任務的使用者為何。 此外，公式中的帳單小時費率會考量費率的任何日期有效變更。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>角色每小時</p> </td>
   <td> <p><strong>計畫成本</strong>的計算公式如下： </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost+ Task Planned Expense Cost</code> </p> <p>其中任務計畫勞力成本的計算方式：</p> <p><code>Task Planned Labor Cost = Planned Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>備註：如果您將多個資源指定至作業，Workfront會根據指定至各資源的作業百分比，調整「計畫時數」的計算。 此外，公式中的每小時費率會考量費率的任何日期有效變更。</p> <p><strong>實際成本</strong>的計算公式如下： </p> <p><code style="font-style: normal;">Task Actual Cost = Task Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>其中作業實際勞力成本的計算方式：</p> <p><code>Task Actual Labor Cost = Actual Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>例如，將任務指派給工作角色或具有工作角色的使用者，其「每小時成本」費率為$20。 當使用者為任務記錄5小時時，該任務的實際勞力成本為$100。 如果指派給任務的使用者沒有與他們在任務上的工作角色相關聯的工作角色，「實際成本」會根據其「主要工作角色」的「每小時成本」費率計算。 如果他們沒有工作角色，或未定義其工作角色的「每小時成本」費率，則任務的「實際成本」為零。 </p> <p>注意：「角色每小時」任務的「實際時數」是根據與任務相關聯的使用者之職務角色而計算，而非根據與記錄時間之使用者相關聯的角色而計算。 此外，公式中的帳單小時費率會考量費率的任何日期有效變更。</p> <p>如果您的Workfront管理員在設定的時程表和時數偏好設定區域中手動啟用<strong>將工作角色指派到時數專案</strong>設定，而且任務的使用者記錄時間會選取與此時數關聯的其他角色，則角色每小時工作的實際成本會根據記錄時數時數時指定的角色進行計算。 如需有關啟用特定工作角色的記錄時間的資訊，請參閱文章<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">設定時程表和小時偏好設定</a>。</p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>固定每小時</p> </td> 
   <td> <p><strong>計畫成本</strong>的計算公式如下：</p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>其中作業人工成本的計算方式：</p> <p><code>Task Planned Labor Cost = Planned Hours * Fixed Hourly Cost of the Task</code> </p> <p><strong>實際成本</strong>的計算公式如下： </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Task Labor Cost + Task Planned Expense Cost</code> </p> <p>其中實際作業人工成本的計算方式：</p> <p><code>Task Actual Labor Cost = Actual Hours * Fixed Hourly Cost of the Task</code> </p> <p>此成本型別不會將個別使用者或職位角色列入考量。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>無成本</p> </td> 
   <td> <p>此成本型別不會影響成本。 如果父系作業具有此「成本型態」，則具有其他「成本型態」的子作業會根據其個別的「成本型態」進行計算，而父系作業的成本也會相應地受到影響。 </p> <p>當沒有財務資料存取許可權的使用者或沒有範本財務許可權的使用者從該範本建立專案時，這是專案上任務的預設成本型別。</p> <p>如需有關存取財務資料的資訊，請參閱文章<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">授予財務資料的存取權</a>。</p> <p>如需物件的財務許可權相關資訊，請參閱文章<a href="../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">共用物件的財務許可權</a>。</p> <p>如需有關從範本建立專案的資訊，請參閱文章<a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">使用範本建立專案</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

## Workfront如何追蹤問題的成本 {#how-workfront-tracks-costs-for-issues}

問題沒有也不影響專案的下列成本型別：

* 規劃成本
* 預算成本

但是，問題可能有&#x200B;**實際成本**，這也會影響專案的實際成本。

下表說明如何根據問題的指定型別，計算問題的實際成本：

<table style="table-layout:auto"> 
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td> <p>使用者指派</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>實際成本</strong>的計算公式如下：</p> <p><code style="font-style: normal;">Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>在此會考量記錄時間之使用者的每小時成本費率，無論該問題指派給何人。 </p> <p>如果記錄時間的使用者在其設定檔中沒有每小時成本費率，則其主要工作角色的每小時成本費率會計算問題的實際成本。</p> <p>如果記錄時間的使用者在其設定檔中沒有任何角色或沒有關聯的比率，則實際時數是使用問題中主要受指派人之主要職務角色的每小時成本費率計算。 如果該角色未定義費率，則問題的實際成本為零。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>角色指派</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>實際成本</strong>的計算公式如下：</p><code>Issue Actual Cost = Actual Hours * Cost per Hour Rate of user logging the hours</code> <p>在此會考慮記錄問題時間的使用者的每小時成本費率，不論指派給問題的角色為何。 </p> <p>如果記錄時間的使用者沒有與其關聯的每小時成本費率，則其主要角色的每小時成本費率會計算問題的實際成本。</p><p>如果記錄時間的使用者在其設定檔中沒有角色或沒有與其關聯的費率，則問題的實際成本為零。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>無指派</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>實際成本</strong>的計算公式如下：</p> <p><code>Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>如果記錄時間的使用者沒有與其設定檔相關聯的每小時成本費率，則其主要職務角色的每小時成本費率會計算問題的實際成本。 </p> <p>如果記錄時間的使用者沒有與其設定檔關聯的工作角色，或其主要工作角色未定義每小時成本費率，則問題的實際成本為零。 </p> </td> 
  </tr> 
 </tbody> 
</table>
