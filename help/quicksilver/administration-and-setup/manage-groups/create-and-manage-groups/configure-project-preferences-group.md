---
title: 設定群組的專案偏好設定
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
description: 如果您是群組管理員且Adobe Workfront管理員為系統中的所有群組解除鎖定專案偏好設定，您可以為群組設定該偏好設定，以影響您的群組建立的所有後續專案。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: c69097fb-99e4-441b-9599-fd8af2dd7116
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '2767'
ht-degree: 2%

---

# 設定群組的專案偏好設定


<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

如果您是群組管理員且Adobe Workfront管理員為系統中的所有群組解除鎖定專案偏好設定，您可以為群組設定該偏好設定，以影響您的群組建立的所有後續專案。

如果您管理的群組之上有任何群組，其管理員也可以為您的群組執行此動作。 Workfront管理員也是如此（適用於任何群組）。

>[!NOTE]
>
>* 通常，已解鎖的偏好設定會無限期地保持解鎖狀態。 如果Workfront管理員將其重新鎖定，系統設定將再次生效，並且群組管理員所做的偏好設定設定將遺失。
>* 為與專案關聯的群組設定的偏好設定優先於為建立專案之使用者的「首頁」群組設定的偏好設定。
>* 有些群組層級偏好設定會影響您為群組建立的專案範本。 如需詳細資訊，請參閱文章[建立及修改群組的專案範本](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md)中的「群組」區域](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view)，一節[「檢視、使用及建立群組的範本」。
>
>* Workfront管理員在系統層級解除鎖定偏好設定後，您可以對其進行設定，然後將其鎖定，以確保您的群組及其子群組中的每個人都使用相同的設定。 此功能與Workfront管理員必須為系統中的每個人設定並鎖定偏好設定的功能平行。 如需詳細資訊，請參閱[鎖定或解除鎖定子群組的專案、任務或問題偏好設定](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md)。
>

任務與問題偏好設定、時程表與小時偏好設定也可能使用群組層級設定。 如需詳細資訊，請參閱[設定群組的任務和問題偏好設定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)以及[設定群組的時程表和小時偏好設定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md)。

如需Workfront管理員如何解除鎖定專案偏好設定的相關資訊，請參閱[鎖定或解除鎖定系統中所有群組的專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>新增：標準</p>
       <p>或</p>
       <p>目前：計畫</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td>您必須是群組的群組管理員或系統管理員。</td>
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 設定群組的解除鎖定專案偏好設定

>[!TIP]
>
>如果您是Workfront管理員，可以前往「設定>專案偏好設定>專案」，然後在頁面頂端的方塊中搜尋群組名稱，略過步驟1至4。

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**群組** ![群組圖示](assets/groups-icon.png)。

1. 按一下要設定其專案偏好設定的群組名稱。
1. 在左側面板中，按一下&#x200B;**專案偏好設定**。
1. 在出現的頁面上，繼續下列的4個區段之一，以設定專案狀態、時間表、業務案例和死後存留的偏好設定。

   >[!TIP]
   >
   >如果您將游標停留在偏好設定上，且顯示工具提示以告知您該偏好設定已鎖定，您可以要求Workfront管理員為組織中的所有群組解除鎖定該偏好設定。

* [專案狀態](#project-status)
* [時間表](#timelines)
* [業務案例](#business-cases)
* [到期後生命期](#life-after-death)

### 專案狀態 {#project-status}

為與群組關聯的新建立專案設定下列任一偏好設定：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>

<tr><td>允許使用者在不使用範本的情況下建立專案</td>
<td><p>此偏好設定可讓使用者在從下列區域建立專案時，無需使用範本即可建立專案：</p>
<ul>
<li><p>在專案清單中使用新專案選項</p></li>

<li><p>從問題頁面將問題轉換為專案</p></li>
</ul>

<p>系統層級預設會啟用此喜好設定。</p>
<p><b>附註</b></p>
<p>當使用者屬於具有不同偏好設定的多個群組時，如果使用者至少有一個群組啟用此偏好設定，則允許使用者建立沒有範本的專案。</p>
</td></tr>
  <tr> 
   <td role="rowheader">將新專案狀態設為</td> 
   <td> <p>決定新專案的狀態。</p> <p><b>附註</b>   
     <ul> 
      <li>如果您或其他Workfront管理員隱藏此處選取的狀態，預設狀態會變更為狀態清單中的第一個狀態。</li> 
     </ul> 
     <ul> 
      <li data-mc-conditions="SnippetConditions-wf-groups.groups">對於群組專案偏好設定，您只能選取鎖定狀態或必要狀態作為預設狀態。</li> 
      <li> <p>如果鎖定的系統或群組狀態設定為預設狀態，稍後有人將其解鎖，則系統會嘗試以相同狀態型別的鎖定狀態來取代它。</p> <p>如果找不到，會尋找必要的狀態：</p> 
       <ul> 
        <li>如果必要的狀態等於已解除鎖定的預設狀態，則即使已解除鎖定，「必要」狀態也會變成預設狀態。</li> 
        <li>如果所有必要狀態都不等同於已解除鎖定的預設狀態，則狀態清單中的第一個必要狀態會成為預設狀態。</li> 
       </ul> <p>如需必要狀態的相關資訊，請參閱文章<a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">存取系統專案狀態清單</a>、<a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">存取系統任務狀態清單</a>，以及<a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">存取系統問題狀態清單</a>。</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">計算完成百分比，依據為</td> 
   <td> <p>專案或父系任務的完成百分比取決於任務的整體進度。 此資訊可以根據專案上任務的期間或計畫時數計算。</p> <p>如果您選取「工期」，專案中每個任務的「工期」會決定專案的整體完成百分比，而每個子任務的「工期」則會決定其父系任務的整體完成百分比。</p> <p>如果您選取「工期」，請務必在「時間表」區段中指定「每工作日一般小時數」和「每週一般工作日數」。 根據期間計算任務的完成百分比時，Workfront會使用此資訊。 </p> <p>如果您選取「計畫時數」，請確認每個專案上的所有任務都已定義計畫時數金額，且該金額不是零。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">根據進度狀態自動設定專案條件</td> 
   <td> <p>此偏好設定可讓使用者手動設定專案條件（達成目標、有風險、存在問題），或讓Workfront根據專案在時間上的進度自動設定條件（進度狀態）。 如需有關專案條件的詳細資訊，請參閱<a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">專案條件和條件型別概觀</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>自動建立基準線</p> </td> 
   <td> <p>當專案狀態變更為目前時，此偏好設定會自動建立任務與專案詳細資訊的基準（快照）。 如需建立基準的相關資訊，請參閱<a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">建立專案基準</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>績效指數方法 </p> </td> 
   <td> <p>專案的績效指數方法(PIM)會控制Workfront用來計算「收益值」量度的方法，例如「成本績效指數(CPI)」和「完工估算(EAC)」。 如需詳細資訊，請參閱<a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">計算成本績效指數(CPI)</a>和<a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">計算完工估算(EAC)</a></p> 
    <ul> 
     <li><strong>小時制</strong>： Workfront會使用計畫時數來計算效能量度，例如EAC和CPI。 當根據時數計算PIM時，EAC會顯示為時數。 確保您有計畫時數的值，而不是零。</li> 
     <li> <p><strong>以成本為基礎</strong>： Workfront使用計畫勞力成本來計算績效量度，例如EAC和CPI。 確保您的工作角色或使用者與每小時成本費率相關聯。 根據「成本」計算PIM時，EAC會顯示為貨幣值。</p> <p>專案經理可以使用[專案詳細資料]中的[財務]區域，在專案層級修改此設定。如需詳細資訊，請參閱<a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">專案財務區域</a>中的管理資訊。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>預估完成成本 </p> </td> 
   <td> <p>決定Workfront要使用哪些資料來計算預估完成成本(EAC)，以代表專案的預估總成本。</p> 
    <ul> 
     <li><strong>在專案層級計算</strong>：父系任務與專案的EAC是由在EAC公式中輸入「實際時數」或「實際勞力成本」所決定。 此計算包括直接新增到父級任務或專案的實際時數或成本和費用。</li> 
     <li> <p><strong>從任務/子任務累計</strong>：父任務和專案的EAC是由每個子任務的EAC相加所決定。 此計算不包括直接新增至父級任務或專案的實際時數或實際成本與費用。</p> <p>專案經理可以使用[專案詳細資料]中的[財務]區域，在專案層級修改此設定。如需詳細資訊，請參閱<a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">專案財務區域</a>中的管理資訊。</p> </li> 
    </ul> <p>如需EAC如何計算的詳細資訊，請參閱<a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">完工估算(EAC)</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 時間表 {#timelines}

為與群組關聯的新建立專案設定下列任一偏好設定：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">排程開始時間</td> 
   <td> <p>決定新專案是從開始日期排程，還是從建立專案時的完成日期排程。</p> 
    <ul> 
     <li><strong>開始日期</strong>：新任務預設為「儘可能早」的任務限制，並且會提示專案經理提供專案的計劃開始日期。</li> 
     <li><strong>完成日期</strong>：新任務預設為「儘可能晚的任務限制」，並且會提示專案經理提供專案的計畫完成日期。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">使用者休假</td> 
   <td> <p>決定任務的主要受指派人的休假是否調整專案上該任務的計畫日期。</p> 
    <ul> 
     <li> <p><strong>考量使用者在任務持續期間的休假</strong>：如果休假發生在任務持續期間，則為任務的主要受指派人排定的任何休假都會調整任務的計畫日期。 這是預設設定。 </p> <p>例如，如果一項限製為「儘快」的任務排程在6月1日開始並在6月3日完成，而主要受指派人將6月2日標籤為休假，則任務的計畫日期將調整為6月1日到6月4日。</p> <p><b>重要</b>：當您選取此設定時，工作的期間不會變更。 根據任務限制，只有計畫日期會變更。</p> </li> 
     <li><strong>忽略使用者在任務持續期間的休假</strong>：專案上每個任務的計畫日期仍保持原始計畫，即使任務的主要受指派人在其持續期間有休假。</li> 
    </ul> <p>選取此設定的選項時，請考量下列事項：</p> 
    <ul> 
     <li>當您變更此設定時，只有變更後建立的專案和範本會繼承更新的設定。 </li> 
     <li> <p>任務的「任務限制」值決定要調整哪些計畫任務日期： </p> 
      <ul> 
       <li>計畫開始日期</li> 
       <li>計畫完成日期</li> 
       <li>兩個日期</li> 
       <li>兩者皆非。 </li> 
      </ul> <p>例如，如果任務具有固定日期的限制條件，則即使選取了考慮使用者在任務持續時間中的休假選項，當主要受指派人具有休假時日期也不會調整。 如需任務限制的相關資訊，請參閱<a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">任務限制總覽</a>。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>專案時間表將自動重新計算</strong> </p> </td> 
   <td> <p>決定重新計算專案的時間表。 如需重新計算專案時間表的相關資訊，請參閱<a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">重新計算專案時間表</a>。</p> <p>預設會啟用下列選項。 您可以選取下列一或多個設定：</p> 
    <ul> 
     <li> <p><strong>每晚</strong>：選取此項可每晚重新計算專案時間表。 您對專案所做的任何可能影響時間表的變更都不會立即顯示。 Workfront​​只會​在夜間重新計算同時符合下列兩個條件的專案的時間表：</p> <p> 
       <ul> 
        <li>具有目前狀態</li> 
        <li>在過去3個月內已更新</li> 
       </ul> </p> </li> 
     <li> <p><strong>當專案範圍變更時</strong>：選取此專案可在專案範圍變更時立即重新計算專案時間表。 如需有關構成專案範圍變更的資訊，請參閱<a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">重新計算專案時間表</a>。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>將多位使用者指派到一個任務時，請使用……</strong>的排程 </p> </td> 
   <td> <p>如果專案未指派排程，或指派給其任務的使用者未指派排程，Workfront會使用系統預設排程來計算任務的時間表。</p> <p>如果您將多位使用者指派給專案中擁有指派排程的相同任務，且指派給任務的使用者也擁有指派給他們的排程，則Workfront會使用下列排程：</p> 
    <ul> 
     <li><strong>主要指派</strong>： Workfront使用任務上主要指派的排程來計算時間表。</li> 
     <li><strong>專案</strong>： Workfront會使用專案排程來計算每項工作的時間表。</li> 
    </ul> <p>如需排程的詳細資訊，請參閱<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">建立排程</a>。</p> </td> 
  </tr> 
 <tr> 
   <td role="rowheader"> <p><strong>將一位使用者指派給任務時，請使用……</strong>的排程 </p> </td> 
   <td> <p>如果專案未指派排程，或指派給其任務的使用者未指派排程，[!DNL Workfront]會使用系統預設排程來計算任務的時間表。</p>

<p>如果您將一位使用者指派至專案中的任務，且專案與使用者都有相關的排程，則[！UICONTROL Workfront]會使用下列排程：</p> 
    <ul> 
     <li><strong>[！UICONTROL User]</strong>：指派的使用者計算時間表的工作排程。</li> 
     <li><strong>[！UICONTROL專案]</strong>：計算任務時間表之專案的排程。</li> 
    </ul> <p>如需排程的詳細資訊，請參閱<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">建立排程</a>。</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>時間表計算 </p> </td> 
   <td> 
    <ul> 
     <li><strong>每個工作日一般小時數</strong>：為將處理專案的使用者設定一般工作日內的小時數。 預設值為8小時。</li> 
    </ul> 
    <ul> 
     <li><strong>每週一般工作天數</strong>：為處理專案的使用者設定標準工作週。 預設值為5天。</li> 
    </ul> <p>這2個選項會將天數轉換為小時，或將周數轉換為天數。</p> <p>例如，如果您有具有8個計畫時數的任務，而持續時間是根據計畫時數計算的，則Workfront會將這些時數轉換為天數，以便將持續時間顯示為天。</p> <p>Workfront會從「每週一般工作天數」欄位計算系統的「相當於全職(FTE)」值。 這是Workfront在計算使用者的分配時所使用的專案。</p> <p>當您計畫專案時間表、編列資源預算或針對專案記錄時間時，會使用這些值。 </p> <p>當您在系統中建立使用者的時程表時，不會使用這些時間表，如<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">設定時程表和小時偏好設定</a>中所述。</p> <p><b>注意</b>： Workfront管理員無法解除鎖定時間表計算偏好設定。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p><strong>自訂季度</strong> </p> </td> 
   <td> <p>為將處理專案的使用者設定自訂每年季度。 自訂季度通常是不符合日曆年度中傳統季度劃分的季度。 您可以新增多個自訂季度。 如需詳細資訊，請參閱<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">啟用專案的自訂季度</a>。</p> <p><b>注意</b>： Workfront管理員無法解除鎖定自訂季度偏好設定。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 業務案例 {#business-cases}

您可以為與群組關聯的新建立專案建立業務案例，以提交專案請求。 您可以定義偏好設定來決定可在&#x200B;**業務案例**&#x200B;表單上看到的區域。 建議您啟用這些選項，以便其他工具(例如Portfolio最佳化程式)能夠正確更新。 如需每個欄位顯示內容的詳細資訊，請參閱[定義業務案例：文章索引](../../../manage-work/projects/define-a-business-case/define-business-case.md)。

Workfront管理員啟用業務案例的區段後，專案所有者就可以在專案層級建立業務案例。 如需建立業務案例的相關資訊，請參閱[為專案建立業務案例](../../../manage-work/projects/define-a-business-case/create-business-case.md)。

### 到期後生命期  {#life-after-death}

為與群組關聯的新建立專案設定下列任一偏好設定：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><strong>將專案標籤為完成之後，人員仍可</strong> </p> </td> 
   <td> <p>決定您的組織（或群組，如果您正在設定群組的專案偏好設定）的規則，這些規則有關於在專案狀態標籤為「完成」後是否可以刪除任務或問題。</p> 
    <ul> 
     <li><strong>刪除任務</strong>：允許使用者在專案標籤為「完成」後，從專案中刪除任務。<br></li> 
     <li><strong>刪除問題</strong>：允許使用者在專案標籤為「完成」後，從專案中刪除問題。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>將專案標籤為「完成」、「廢棄」或「未決核准」之後，人員仍可</strong> </p> </td> 
   <td> <p>決定組織（或群組，如果您正在設定群組的專案偏好設定）的規則，這些規則有關於專案狀態標籤為<strong>完成</strong>、<strong>廢棄</strong>或<strong>未決核准</strong>後，專案中任務、問題、檔案和其他物件所發生的情況。</p> 
    <ul> 
     <li><strong>新增及編輯工作</strong>允許使用者： 
      <ul> 
       <li>在專案標籤為「完成」、「廢棄」或「未決核准」後，編輯專案中的任務。 這包括新增時數以及變更任務上的費用輸入項。</li> 
       <li>將任務新增至專案。</li> 
      </ul></li> 
     <li><strong>新增及編輯問題</strong>：允許使用者： 
      <ul> 
       <li>在專案標籤為「完成」、「廢棄」或「未決核准」後，編輯專案中的問題。</li> 
       <li>在專案被標示為完成或廢棄後，將問題新增至專案。 （您無法將問題新增至擱置核准的專案。）</li> 
      </ul></li> 
     <li> <p><strong>將檔案新增至專案及其任務和問題</strong>：允許使用者在專案被標示為完成或廢棄後，將檔案新增至專案（或將檔案新增至專案內的任務和問題）。</p> <p>此選項不適用於等待核准的專案。</p> </li> 
     <li> <p><strong>附加範本</strong>：允許使用者在專案被標示為完成或廢棄後，將範本附加至專案。</p> <p>此選項不適用於等待核准的專案。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
