---
content-type: overview
product-area: projects
navigation-topic: financials
title: 帳單和收入概觀
description: 身為專案經理，您可以使用計費率來擷取專案的收入。
author: Alina
feature: Work Management
exl-id: 400abcde-e368-4a70-89a9-05027900ab81
source-git-commit: 518a552845598a30fd547d432aa9d22dfef6ec8e
workflow-type: tm+mt
source-wordcount: '3313'
ht-degree: 0%

---

# 帳單和收入概觀

身為專案經理，您可以使用計費率來擷取專案的收入。

本文說明如何追蹤專案的收入。 收入在「利用率報表」中的計算方式不同。 有關「利用率」報表中收入計算的資訊，請參閱 [查看資源利用資訊](../../../resource-mgmt/resource-utilization/view-utilization-information.md).

## 計費率概觀

使用計費率時，請考量下列事項：

* 您需要具有編輯金融資料存取權的計畫授權，才能管理計費率。\
   有關授予對金融資料的訪問權限的詳細資訊，請參見 [授予金融資料的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

* 開單費率是與職務角色或用戶關聯的每個工作單位的收入額。

   將比率乘以工作所花費的小時數，可為您的專案產生收入。

* 建立計費費率後，您就可以建立計費記錄來追蹤收入，以記錄已開具和未開具的費用。

   >[!TIP]
   >
   >當您將帳單記錄標示為已計費時，將無法編輯該記錄。 當您的費率不同，而且您想要鎖定專案的收入和費用資訊時，這點很重要。 將其添加到計費記錄中並標籤為「已計費」，會在費率在您的系統中更新時阻止其更新。

   有關建立計費記錄的詳細資訊，請參閱文章 [建立計費記錄](../../../manage-work/projects/project-finances/create-billing-records.md).

* 您可以為用戶、職務角色建立開單費率，也可以為項目或任務建立一次性開單費率。

>[!IMPORTANT]
>
>計算收入的比率屬於記錄時間的使用者或其工作角色。

* [用戶計費率](#user-billing-rates)
* [任務職責開單費率](#job-role-billing-rates)
* [項目或任務的固定計費率](#fixed-billing-rates-for-projects-or-tasks)
* [改寫開單費率](#override-billing-rates)

### 用戶計費率 {#user-billing-rates}

作為用戶管理員，在建立用戶時，可以通過在用戶配置檔案中指定「每小時計費」欄位的值，將用戶與計費費率關聯。\
如需建立使用者的詳細資訊，請參閱文章 [新增使用者](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md)

![](assets/qs-user-edit-ui-with-rp-and-billing-per-hour-field-1-350x152.png)

### 任務職責開單費率 {#job-role-billing-rates}

作為Adobe Workfront管理員，在您建立職務角色時，可以通過指定「開單/小時」欄位的值，將其與開單費率關聯。

您可以使用Workfront系統的基本貨幣或使用其他自訂貨幣來定義職務職責開單費率的值。

有關建立職務角色和覆蓋其貨幣的詳細資訊，請參閱文章 [建立和管理作業角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)

![](assets/billing-rate-for-role-1-350x294.png)

### 項目或任務的固定計費率 {#fixed-billing-rates-for-projects-or-tasks}

除了用戶和職務角色每小時費率外，您還可以有以下固定計費率：

* 固定每小時收入類型的固定金額
* 固定收入類型的固定金額

如需如何使用固定計費率來計算收入的詳細資訊，請參閱 [任務收入類型概覽](#overview-of-task-revenue-types).

### 改寫開單費率 {#override-billing-rates}

>[!IMPORTANT]
>
>您可以改寫與職務職責關聯的開單費率。 您不能改寫用戶開單費率或固定費率。

您可以改寫以下職務的職務開單費率：

* 特定公司

   有關建立公司特定職務職責開單費率的詳細資訊，請參閱 [建立和編輯公司](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* 特定專案

   有關建立專用於項目的職務職責開單費率的詳細資訊，請參閱文章 [改寫任務職責開單費率和計算項目收入概覽](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## 跟蹤收入金額

當根據任務的「計畫時間」建立任務時，Workfront可以自動追蹤計畫收入。

當任務、問題和專案上記錄實際小時數時，它也可以自動追蹤實際收入。

下表顯示與任務、問題和項目相關聯的收入類型。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">計畫收入</td> 
   <td> <p>對於任務，這是與「計畫小時數」任務關聯的收入。 所有任務的「計畫小時數」累計到項目的「計畫小時數」，以便計算項目「計畫小時數」。 </p> <p>如需Workfront中「計畫小時數」的詳細資訊，請參閱 <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">計畫小時數概觀</a>. </p> <p>Workfront使用以下公式計算任務和項目的計畫收入：</p> <p><code>Task Planned Revenue = Planned Hours * Billing hourly rate</code> </p> <p><code>Project Planned Revenue = SUM (All tasks Planned Revenue) +&nbsp;Fixed Revenue</code> </p> 
   <p><b>附註</b>

<p>在「項目詳細資訊」區域和項目報表中顯示的項目計畫收入與在「利用率」報表中顯示的「計畫收入」不同。 </p> <p>「項目詳細資訊」區域中的「計畫收入」反映與任務「計畫小時數」和項目「固定收入」關聯的任務收入。 「利用率報表」中的「計畫收入」僅顯示與項目上任務分配的「計畫小時數」關聯的「計畫收入」。 </p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p>如果項目有1個10小時的任務，並分配給一個每小時費率為$20的顧問，而項目有$100的固定收入，則「利用率」報表將顯示「計畫收入」為$200（與任務上的小時相關聯的計畫收入）。 「項目詳細資訊」部分顯示$300（任務的計畫收入和項目的固定收入）。 </p> 
     </div> </p> <p>任務計畫收入使用分配給任務的用戶或職務角色的按小時計費費率計算。 任務的「收入類型」會影響用於計算計畫收入的費率（用戶或職責）。 如需詳細資訊，請參閱本文的下列章節：</p> 
    <ul> 
     <li> <p><a href="#overview-of-task-revenue-types" class="MCXref xref">任務收入類型概覽</a> </p> </li> 
     <li> <p><a href="#revenue-calculations-for-tasks-based-on-user-and-role-assignments" class="MCXref xref">基於用戶和角色分配的任務的收入計算</a> </p> </li> 
    </ul> <p>有關「利用率」報表中計畫收入計算的資訊，請參閱 <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">查看資源利用資訊 </a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">實際收入*</td> 
   <td> <p>與「實際小時數」任務、問題和項目相關聯。 </p> <p>一般而言，Workfront會使用此公式計算實際收入：</p> <p><code>Planned Revenue = Planned Hours * Billing rate</code> </p> <p>有關「利用率」報表中實際收入計算的資訊，請參閱 <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">查看資源利用資訊 </a>. </p> <p><b>筆尖</b>

您無法在問題層查看實際收入，但與問題上的實際小時數關聯的收入將影響項目的實際收入。 </p> </td>
</tr> 
 </tbody> 
</table>

*對於「實際小時數」，使用者的費率一律指記錄該小時數的使用者，或其工作角色的費率。 如需Workfront何時使用使用者比率，以及何時使用其工作角色比率的相關資訊，請參閱 [收入計算](#revenue-calculations) 一節。

<!--Note from the table for Planned Revenue line: 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the note below is duplicated in this article: /Content/Resource Mgmt/Resource utilization/view-utilization-information.htm and in the glossary)</p>
    -->

例如，如果具有「用戶每小時收入類型」的任務計畫花費2小時，且分配給該任務的用戶每小時費率為$30，則任務的「計畫收入」為$60。 完成任務後，如果用戶僅將1.5小時記錄為完成任務的實際逗留時間，則實際收入金額為$45。 如果未分配給該任務的另一個用戶記錄了該時間，則實際收入將根據該用戶的開單費率計算。

您可以透過下列方式記錄收入：

* 通過定義任務的「收入類型」，以及將分配給工作項目的用戶或角色與開單費率關聯。 這將按工作項上的計畫小時數或實際小時數計算收入。 您可以設定每小時費率的最高收費額，或者不設上限。\
   有關指定任務的「收入類型」的詳細資訊，請參閱文章 [編輯任務](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

* 為任務或項目按固定收入費率計費。\
   如果任務具有固定收入，則「固定收入」金額將添加為任務或項目的「計畫收入」，而任務的「計畫收入」將可以作為「固定收入」添加到「開單記錄」中。
* 通過為項目設定固定計費固定收入比率，然後為項目內的任務設定小時費率。 Workfront會將工作的小時費率新增至專案的固定費率。\
   例如，使用Workfront的機械師可以輸入部件成本作為項目的固定收入，然後按小時開具修復汽車所花費的費用。 固定項目或任務的收入則在完成時實現。

您還可以將任務標籤為「不可開單」，在這種情況下，沒有與這些任務關聯的計畫收入或實際收入。

## 任務收入類型概覽 {#overview-of-task-revenue-types}

依預設，所有新任務的「收入類型」會根據您的Workfront或群組管理員所指定的「任務和問題偏好設定」來設定。\
如需定義Workfront執行個體的任務和問題偏好設定的詳細資訊，請參閱文章 [配置全系統任務和問題首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

項目所有者可以修改項目的「收入類型」任務和「固定收入」。\
如需指定專案固定收入的詳細資訊，請參閱文章 [編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md).\
有關指定任務的「收入類型」的詳細資訊，請參閱文章 [編輯任務](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

您可以將下列收入類型套用至您的工作或專案：

<table border="1" cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>收入類型</strong> </p> </th> 
   <th> <p><strong>說明</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>固定收入</p> </td> 
   <td> <p>此類型可與專案和任務搭配使用。 </p> <p>將範本附加至專案時，範本的「固定收入」會新增至專案的「固定收入」。 如需詳細資訊，請參閱 <a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md" class="MCXref xref">將範本附加至專案的概觀</a>. </p> <p>對於任務，無論任務分配如何，任務上的收入始終使用任務上指定的固定金額計算。 </p> <p>「來自子項的固定收入」任務累計到父項任務的「收入」，然後累計到項目的收入。 如果在父任務和/或項目上定義了固定金額，則該金額將添加到從任何子任務累計的計畫收入中。</p> <p>任務上的固定收入金額可以包含在項目上的計費記錄中。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>使用者小時</p> </td> 
   <td> <p>此類型只能用於任務。 </p> <p>您為特定用戶設定的開單費率乘以該任務的計畫小時數，就成為任務的計畫收入金額。 您為特定用戶設定的開單費率乘以用戶根據任務記錄的小時數，即為任務的實際收入額。 <br>例如，當您建立用戶並為其「每小時開單」欄位設定了$20時，如果用戶為時間表上的任務提交了5小時，則任務的「實際開單」金額為$100。</p> <p><b>筆尖</b>

這是建立任務時的預設收入類型。</p> </td>
</tr> 
  <tr> 
   <td> <p>角色小時</p> </td> 
   <td> <p>此類型只能用於任務。</p> <p>此類型類似於「用戶每小時」，但使用工作角色費率，而非用戶費率。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>每小時使用大寫</p> </td> 
   <td> <p>此類型只能用於任務。</p> <p>任務按每小時用戶計費，但您可以指定任務的最大限額。 <br>例如，如果用戶的計費費率為$25，但任務的「上限金額」為$20，並且用戶記錄了1小時，則任務的實際收入為$20。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>角色每小時，上限</p> </td> 
   <td> <p>此類型只能用於任務。</p> <p>此類型類似於「使用上限時每小時的使用者」，但使用工作角色費率，而非使用者費率。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>使用者小時加固定</p> </td> 
   <td> <p>此類型只能用於任務。 </p> <p>任務按「每小時用戶」開單，但有「固定金額」，您可以將其添加到用戶費率中。 任務上指定的固定金額可以包含在項目的開單記錄中。 固定金額不會乘以任務上的小時數。 只有使用者計費率才有。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>角色小時加固定</p> </td> 
   <td> <p>此類型只能用於任務。 </p> <p>任務在「每小時角色」中按小時計費，但您可以將其添加到角色費率中的附加固定金額。 任務上指定的固定金額可以包含在項目的開單記錄中。 固定金額不會乘以任務上的小時數。 只有作業角色計費率才有。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>固定小時</p> </td> 
   <td> <p>此類型只能用於任務。</p> <p>您為任務設定的上限或固定金額乘以針對任務輸入的小時數（無論用戶或其職務）即為開單金額。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>不可記帳</p> </td> 
   <td> <p>此類型只能用於任務。</p> <p>此收入類型對收入沒有影響。 </p> <p>如果父對象具有此設定，則具有計費類型的子任務仍將正常應用。</p> <p>當無權訪問財務資料的用戶或對模板沒有財務權限的用戶從該模板建立項目時，這是項目任務的預設收入類型。</p> <p>如需存取金融資料的相關資訊，請參閱文章 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">授予金融資料的存取權</a>.<br>有關對象的財務權限的資訊，請參見文章 <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">對象共用權限概述</a>.<br>如需從範本建立專案的相關資訊，請參閱文章 <a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">使用範本建立專案</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

## 父任務的收入概覽

如果將獨立任務更改為父任務，且其上包含開單資訊，則新父任務仍保留以前應用到該任務的任何開單資訊，以及以前應用的小時數。 從記錄到子任務的小時開始的任何開單資訊都將統計為新父任務的實際收入。

來自子任務的計畫收入也累計到父任務。

## 問題的收入概覽

問題沒有計畫或實際收入金額，但可以有實際成本。

如果您記錄問題的小時數，並使用標示為「計為收入」的小時類型，則Workfront會根據登入該時間的使用者比率計算實際成本金額。 此數字將添加到項目的實際成本中。 小時數也可包含在計費記錄中。

如需追蹤成本的詳細資訊，請參閱文章 [追蹤成本](../../../manage-work/projects/project-finances/track-costs.md).

如需有關小時類型的詳細資訊，請參閱文章 [管理小時類型](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## 收入計算

* [基於用戶和角色分配的任務的收入計算](#revenue-calculations-for-tasks-based-on-user-and-role-assignments)

### 基於用戶和角色分配的任務的收入計算 {#revenue-calculations-for-tasks-based-on-user-and-role-assignments}

計算任務的收入時，請考慮以下事項：

* 如果使用者或工作角色顯示的比率為$0.00,Workfront會讀取為有效金額，並將此金額乘以該任務上的小時數來計算收入。 如果您不想顯示任務的收入，請確保用戶或職務角色的計費率欄位為空。
* 在應用職務職責開單費率時，Workfront會使用項目層的改寫費率，而不是在每次項目存在改寫費率時在系統層定義的該職責的開單費率。
* 如果任務上有多個受分配人，則以下概述的情況適用於每個受分配人。

根據任務分配在收入計算中使用費率的層次結構。

如果您的Workfront管理員已啟用 **手動將作業角色分配給小時條目** 在「時間表和小時首選項」區域中設定，並且項目上的用戶登錄時間選擇與此時間關聯的不同角色，則任務或項目的實際收入始終根據與小時錄入關聯的角色進行計算。 有關為特定作業角色啟用記錄時間的資訊，請參閱文章 [時間表和小時首選項](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

根據收入類型和任務分配的性質計算任務收入時，存在以下方案：

* **任務的收入類型為用戶每小時**

   <table style="table-layout:auto"> 
   <col> 
   <col> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">每小時費率</td> 
     <td>無分配</td> 
     <td>用戶分配</td> 
     <td>職務角色分配</td> 
    </tr> 
    <tr> 
     <td role="rowheader">計畫收入的每小時開單費率</td> 
     <td>$0.00</td> 
     <td> 如果使用者的設定檔中有計費費率，則該費率用於計算計畫收入。 否則，將使用其主要作業角色的系統計費率。 <br><p><b>注意</b>  可以將用戶分配給具有其其中一個輔助作業角色的任務，但是在此處改用主作業角色的比率。</p></td> 
     <td>分配給任務的任務職責的系統開單費率用於計算計畫收入。 </td> 
    </tr> 
    <tr> 
     <td role="rowheader">實際收入的每小時計費率</td> 
     <td>如果記錄小時的使用者設定檔中有計費率，系統會使用該費率。 <br>否則，將使用其主要職務角色的計費率。 如果沒有與用戶或其主要角色相關聯的開單費率，則實際收入為$0.00。 <br><p><b>附註</b>

   即使將另一個用戶分配給任務，也只考慮與記錄時間的用戶相關聯的比率。</p></td>
   <td>如果記錄小時的使用者設定檔中有計費率，系統會使用該費率。 <br>否則，將使用其主要職務角色的計費率。 如果沒有與用戶或其主要角色相關聯的開單費率，則實際收入為$0.00。 <br><p><b>附註</b>

   即使將另一個用戶分配給任務，也只考慮與記錄時間的用戶相關聯的比率。</p></td>
   <td>如果記錄小時的使用者設定檔中有計費率，系統會使用該費率。 否則，將使用其主要職務角色的計費率。<br><p><b>附註</b>

   如果用戶記錄時間沒有與其相關聯的計費費率，並且他們沒有其職務職責或其職務職責的計費費率，則使用與任務相關聯的職務職責的費率。 如果此角色沒有開單費率，則收入為$0.00</p></td>
   </tr> 
   </tbody> 
  </table>

* **任務的收入類型為每小時角色**

   <table style="table-layout:auto"> 
   <col> 
   <col> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">每小時費率</td> 
     <td>無分配</td> 
     <td>用戶分配</td> 
     <td>職務角色分配</td> 
    </tr> 
    <tr> 
     <td role="rowheader">計畫收入的每小時開單費率</td> 
     <td>$0.00</td> 
     <td>Workfront會查看使用者在計算計畫收入的任務上所履行的工作職責。 <br>如果使用者未與任務上的任何角色相關聯，則收入為$0.00。 </td> 
     <td>分配給任務的任務職責的開單費率用於計算計畫收入。</td> 
    </tr> 
    <tr> 
     <td role="rowheader">實際收入的每小時計費率</td> 
     <td>Workfront會使用記錄時間之使用者的主要工作角色的計費率。 <br>如果記錄時間的用戶沒有與他們相關聯的職務角色，或者主要職務角色沒有開單費率，則實際收入為$0.00。 </td> 
     <td> 如果記錄時間的用戶被分配給任務，則與任務上的用戶關聯的任務角色的開單費率用於計算實際收入。 否則，將使用其主要職務角色的計費率。 如果用戶沒有主要職務職責，或者其主要職務職責沒有開單費率，則實際收入為$0.00。 </td> 
     <td>如果將記錄時間的用戶的作業角色之一分配給該任務，則使用該作業角色率。 如果分配給任務的任務角色沒有與記錄時間的用戶關聯，則使用用戶主要角色的開單費率來計算實際收入。 如果用戶沒有作業角色或沒有與其主要作業角色相關聯的比率，則使用分配給該任務的作業角色的比率。 </td> 
    </tr> 
   </tbody> 
  </table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>Ideal table but does not come across Markdown</p>
<table style="table-layout:auto">
<col>
<col>
<col>
<col>
<col>
<col>
<col>
<tbody>
<tr>
<td colspan="3">Revenue Type = User Hourly</td>
<td colspan="4">Revenue Type = Role Hourly</td>
</tr>
<tr>
<td> <p> </p> </td>
<td> <p><strong>No Assignment</strong> </p> </td>
<td> <p><strong>User Assignment</strong> </p> </td>
<td> <p><strong>Job Role Assignment</strong> </p> </td>
<td> <p><strong>No Assignment</strong> </p> </td>
<td> <p><strong>User Assignment</strong> </p> </td>
<td> <p><strong>Job Role Assignment</strong> </p> </td>
</tr>
<tr>
<td> <p><strong>Billing per hour rate for Planned Revenue</strong> </p> </td>
<td> <p>$0.00</p> </td>
<td> <p> If a user has a billing rate in their profile, then that rate is used to calculate Planned Revenue. Otherwise, the system billing rate of their primary job role is used. <br><note type="note">
The user can be assigned to the task with one of their secondary job roles, but the rate of the primary job role is used here instead.
</note></p> </td>
<td> <p> The system billing rate of the job role assigned to the task is used to calculate Planned Revenue. </p> </td>
<td> <p>$0.00</p> </td>
<td> <p>Workfront looks at the job role that the user fulfills on the task to calculate the Planned Revenue. <br>If the user is not associated with any role on the task, the Revenue is $0.00. </p> </td>
<td> <p>The billing rate of the job role assigned to the task is used to calculate Planned Revenue. </p> <p> </p> <p> </p> </td>
</tr>
<tr>
<td> <p><strong>Billing per hour rate for Actual Revenue</strong> </p> </td>
<td colspan="2"> <p>If the user logging the hours has a billing rate in their profile, that rate is used. <br>Otherwise, the billing rate of their primary job role is used. If there is no billing rate associated with the user or their primary role, the Actual Revenue is $0.00. <br><note type="note">
Only the rates associated with the user logging the time are taken into account for the calculation, even when another user is assigned to the task.
</note></p> </td>
<td> If the user logging the hours has a billing rate in their profile, that rate is used. Otherwise, the billing rate of their primary job role is used.<br><note type="note">
If the user logging time has no billing rate associated with them, and they do not have a job role or a billing rate for their job role, then the rate from the job role associated with the task is used. If there is no billing rate for this role, the revenue is $0.00
</note></td>
<td> <p>Workfront uses the billing rate of the primary job role of the user logging the time. <br>If the user logging the time has no job role associated with them, or if the primary job role has no billing rate, the Actual Revenue is $0.00. </p> </td>
<td> <p> If the user logging the time is assigned to the task, the billing rate of the job role associated with the user on the task is used to calculate the Actual Revenue. Otherwise, the billing rate of their primary job role is used. If the user has no primary job role or if their primary job role has no billing rate, the Actual Revenue is $0.00. </p> </td>
<td> <p>If one of the job roles of the user logging the time is assigned to the task, that job role rate is used. If the job role assigned to the task is not associated with the user logging the time, then the billing rate of the primary role of the user is used to calculate the Actual Revenue. If the user does not have a job role or there is no rate associated with their primary job role, then the rate of the job role assigned to the task is used. </p> </td>
</tr>
</tbody>
</table>
</div>
-->

### 項目的收入計算

您可以追蹤專案的下列收入類型：

* 項目的計畫收入按以下公式計算：

   ```
   Project Planned Revenue = SUM(Task Planned Revenue)+ Fixed Revenue
   ```

   有關如何計算任務計畫收入的資訊，請參閱 [基於用戶和角色分配的任務的收入計算](#revenue-calculations-for-tasks-based-on-user-and-role-assignments) 一節。

* 項目的實際收入按以下公式計算：

   ```
   Project Actual Revenue = SUM (Task Actual Revenue) + (Hours logged for the project x User Billing per Hour Rate) + SUM (Hours logged for the issues x User Billing per Hour rate)
   ```

有關如何計算實際收入的任務的資訊，請參閱 [基於用戶和角色分配的任務的收入計算](#revenue-calculations-for-tasks-based-on-user-and-role-assignments) 一節。

對於與直接記錄至專案或問題的時數相關聯的實際收入，Workfront會使用記錄專案時間之使用者的計費比率。 如果使用者的設定檔沒有相關聯的計費費率，Workfront會使用其主要職務角色的計費費率。 如果兩者的比率均為零，則與項目上記錄的小時數或問題相關聯的實際收入為零。
