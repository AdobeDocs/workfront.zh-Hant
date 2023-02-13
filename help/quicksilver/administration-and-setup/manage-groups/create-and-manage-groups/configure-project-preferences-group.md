---
title: 配置組的項目首選項
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
description: 如果您是組管理員，而Adobe Workfront管理員為系統中的所有組解除鎖定項目首選項，則可以為組配置該首選項以影響組建立的所有後續項目。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: c69097fb-99e4-441b-9599-fd8af2dd7116
source-git-commit: 11c4028038fe3d410ee0d4f238d2138435d9a3fa
workflow-type: tm+mt
source-wordcount: '2643'
ht-degree: 2%

---

# 配置組的項目首選項

如果您是組管理員，而Adobe Workfront管理員為系統中的所有組解除鎖定項目首選項，則可以為組配置該首選項以影響組建立的所有後續項目。

如果您管理的群組上方有任何群組，其管理員也可以對您的群組執行此動作。 Workfront管理員（適用於任何群組）也是如此。

>[!NOTE]
>
>* 通常，未鎖定首選項會無限期保持未鎖定狀態。 如果Workfront管理員重新鎖定，系統設定會再次生效，且群組管理員所做偏好設定的設定會遺失。
>* 為與項目關聯的組設定的首選項優先於為建立項目的用戶的「首頁組」設定的首選項。
>* 某些組級別首選項會影響您為組建立的項目模板。 如需詳細資訊，請參閱 [從「組」區域查看、使用和建立組的模板](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view) 在文章中 [建立和修改群組的專案範本](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
>
>* 在Workfront管理員解除系統級別偏好設定的鎖定後，您可以進行設定，然後將其鎖定，以確保群組及其子群組中的每個人都使用相同的設定。 這與Workfront管理員必須為系統中的每個人設定和鎖定偏好設定的功能平行。 如需詳細資訊，請參閱 [鎖定或解除鎖定子組的項目、任務或問題首選項](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).
>


任務和問題首選項以及工時單和小時首選項也可以進行組級別配置。 如需詳細資訊，請參閱 [配置組的任務和問題首選項](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md) 和 [配置組的時間表和小時首選項](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

有關Workfront管理員如何解鎖項目首選項的資訊，請參見 [鎖定或解鎖系統中所有組的項目首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

## 存取需求

您必須具備下列條件才能執行本文所述步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront計畫*</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> <p>您必須是群組的群組管理員或Workfront管理員。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">群組管理員</a> 和 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;如果您需要了解您擁有的計畫或授權類型，請聯絡Workfront管理員。

## 為組配置未鎖定項目首選項

>[!TIP]
>
>如果您是Workfront管理員，可以前往「設定>專案偏好設定>專案」 ，然後在頁面頂端的方塊中搜尋群組名稱，以略過步驟1至4。

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **群組** ![](assets/groups-icon.png).

1. 按一下要配置其項目首選項的組的名稱。
1. 在左側面板中，按一下 **專案偏好設定**.
1. 在顯示的頁面上，繼續以下4個部分之一，以配置「項目狀態」、「時間軸」、「業務案例」和「死亡後生命」的首選項。

   >[!TIP]
   >
   >如果您將滑鼠指標暫留在偏好設定上，系統會顯示工具提示來告知您該偏好設定已鎖定，您可以要求Workfront管理員為組織中的所有群組解除鎖定。

* [專案狀態](#project-status)
* [時間表](#timelines)
* [業務案例](#business-cases)
* [到期後生命期](#life-after-death)

### 專案狀態 {#project-status}

為與組關聯的新建立項目配置以下任何首選項：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>

<tr><td>允許使用者在不使用範本的情況下建立專案</td>
<td><p>從以下區域建立專案時，此偏好設定可讓使用者無須使用範本即可建立專案：</p>
<ul>
<li><p>在專案清單中使用「新增專案」選項</p></li>

<li><p>將問題從問題頁面轉換為專案</p></li>
</ul>

<p>預設情況下，系統級別會啟用此首選項。</p>
<p><b>附註</b></p>
<p>當使用者屬於具有不同偏好設定的多個群組時，如果其中至少一個群組已啟用此偏好設定，則允許使用者建立不含範本的專案。</p>
</td></tr>
  <tr> 
   <td role="rowheader">將新項目的狀態設定為</td> 
   <td> <p>確定新項目的狀態。</p> <p><b>附註</b>   
     <ul> 
      <li>如果您或其他Workfront管理員隱藏此處選取的狀態，預設狀態會變更為狀態清單中的第一個狀態。</li> 
     </ul> 
     <ul> 
      <li data-mc-conditions="SnippetConditions-wf-groups.groups">對於組項目首選項，只能選擇鎖定狀態或必需狀態作為預設狀態。</li> 
      <li> <p>如果鎖定的系統或組狀態被設定為預設狀態，之後有人解除鎖定，則系統會嘗試將其替換為相同狀態類型的鎖定狀態。</p> <p>如果找不到，則會尋找必要狀態：</p> 
       <ul> 
        <li>如果存在相當於未鎖定預設狀態的必需狀態，則必需狀態將變為預設狀態，即使它處於未鎖定狀態。</li> 
        <li>如果所有必需狀態均不等於未鎖定的預設狀態，則狀態清單中的第一個必需狀態將變為預設狀態。</li> 
       </ul> <p>如需所需狀態的詳細資訊，請參閱文章 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">訪問系統項目狀態清單</a>, <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">訪問系統任務狀態清單</a>，和 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">訪問系統問題狀態清單</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">根據計算完成百分比</td> 
   <td> <p>項目或父任務的完成百分比取決於任務的整體進度。 此資訊可以根據項目上任務的「持續時間」或「計畫時數」計算。</p> <p>如果選擇「持續時間」，則項目中每個任務的持續時間將決定項目的整體完成百分比，而每個子任務的持續時間將決定其父任務的整體完成百分比。</p> <p>如果選擇「持續時間」，請確保在「時間軸」部分中指定「每工作日的典型小時數」和「每週的典型工作日數」。 Workfront根據「持續時間」計算任務完成百分比時，會使用此資訊。 </p> <p>如果選擇「計畫小時數」，請確保每個項目上的所有任務都定義了「計畫小時數」，並且該金額不是零。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">根據進度狀態自動設定專案條件</td> 
   <td> <p>此偏好設定可讓使用者手動設定專案的條件（在Target上、有風險、有問題），或讓Workfront根據專案在時間軸上的進度自動設定條件（進度狀態）。 如需專案條件的詳細資訊，請參閱 <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">專案條件和條件類型概觀</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>自動建立基準線</p> </td> 
   <td> <p>當項目狀態更改為「當前」時，此首選項會自動建立任務和項目詳細資訊的基線（快照）。 如需建立基線的相關資訊，請參閱 <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">建立專案基線</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>績效指數方法 </p> </td> 
   <td> <p>項目的效能指數方法(PIM)控制Workfront用於計算掙值度量的方法，如成本效能指數(CPI)和完成估計(EAC)。 如需詳細資訊，請參閱 <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">計算成本績效指數(CPI)</a>和 <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">完成時計算估計值(EAC)</a></p> 
    <ul> 
     <li><strong>小時型</strong>:Workfront使用「計畫時數」來計算EAC和CPI等效能量度。 根據小時計算PIM時，EAC會顯示為小時數。 請確定您有「計畫小時數」的值，而非零。</li> 
     <li> <p><strong>成本型</strong>:Workfront使用「計畫人工成本」來計算績效量度，如EAC和CPI。 確保您的工作角色或用戶與每小時成本費率相關聯。 根據成本計算PIM時，EAC會顯示為貨幣值。</p> <p>項目經理可以使用項目詳細資訊中的「財務」區域在項目級別修改此設定。有關詳細資訊，請參閱 <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">管理項目財務區域中的資訊</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>預估完成成本 </p> </td> 
   <td> <p>確定Workfront用於計算完成估計(EAC)的資料，該估計表示項目的預計總成本。</p> 
    <ul> 
     <li><strong>在專案層級計算</strong>：父任務和項目的EAC通過在EAC公式中輸入「實際小時數」或「實際人工成本」來確定。 此計算包括直接添加到父任務或項目的實際小時數或成本和費用。</li> 
     <li> <p><strong>從任務/子任務匯總</strong>:父任務和項目的EAC通過加總每個子任務的EAC來確定。 此計算不包括直接添加到父任務或項目的實際小時數或實際成本和費用。</p> <p>項目經理可以使用項目詳細資訊中的「財務」區域在項目級別修改此設定。有關詳細資訊，請參閱 <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">管理項目財務區域中的資訊</a>.</p> </li> 
    </ul> <p>有關EAC計算方式的詳細資訊，請參見 <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">完成時計算估計值(EAC)</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 時間表 {#timelines}

為與組關聯的新建立項目配置以下任何首選項：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">排程開始時間</td> 
   <td> <p>確定新項目是從建立日期開始還是從完成日期開始計畫。</p> 
    <ul> 
     <li><strong>開始日期</strong>:新任務預設為「盡快」任務約束，系統將提示項目經理為項目提供「計畫起始日期」。</li> 
     <li><strong>完成日期</strong>:新任務預設為「最晚可能的任務約束」，系統將提示項目經理為項目提供計畫完成日期。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">使用者休假</td> 
   <td> <p>確定任務的主要受託人的休息時間是否調整項目上該任務的計畫日期。</p> 
    <ul> 
     <li> <p><strong>考慮任務持續時間中的用戶超時</strong>:為任務的主要受託人計畫的任何時間，如果在任務期間發生了關閉時間，則會調整任務的計畫日期。 這是預設設定。 </p> <p>例如，如果計畫在6月1日開始並在6月3日完成具有「盡快約束」的任務，而主要受託人在6月2日標籤為「超時」，則任務的計畫日期將調整為6月1日到6月4日。</p> <p><b>重要</b>:選擇此設定時，任務的持續時間不會更改。 根據「任務約束」，僅更改計畫日期。</p> </li> 
     <li><strong>忽略任務持續時間中的用戶超時</strong>:項目上每個任務的計畫日期仍按原計畫進行，即使任務的主要受託人在其期間有時間休息。</li> 
    </ul> <p>為此設定選取選項時，請考量下列事項：</p> 
    <ul> 
     <li>更改此設定時，只有在更改後建立的項目和模板才會繼承更新的設定。 </li> 
     <li> <p>任務的任務約束值確定要調整的計畫任務日期： </p> 
      <ul> 
       <li>計畫開始日期</li> 
       <li>計畫完成日期</li> 
       <li>兩個日期</li> 
       <li>兩個日期都沒有。 </li> 
      </ul> <p>例如，如果任務的約束為「固定日期」，則當主要受託人有超時時，即使選擇了「考慮用戶在任務期間的超時」選項，日期也不會調整。 有關任務約束的資訊，請參閱 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">任務約束概覽</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>將自動重新計算項目時間表</strong> </p> </td> 
   <td> <p>決定何時重新計算專案時間表。 有關重新計算項目時間軸的資訊，請參閱 <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">重新計算項目時間表</a>.</p> <p>預設會啟用下列選項。 您可以選取下列一或多個設定：</p> 
    <ul> 
     <li> <p><strong>每晚</strong>:選擇此選項可以每晚重新計算項目時間表。 您對專案所做的任何可能會影響時間軸的變更都不會立即顯示。 Workfront​ ​只​會在夜間重新計算符合下列兩個條件之專案的時間表：</p> <p> 
       <ul> 
        <li>狀態為「當前」</li> 
        <li>過去3個月有過更新</li> 
       </ul> </p> </li> 
     <li> <p><strong>項目範圍更改時</strong>:選擇此選項可在項目範圍發生更改時立即重新計算項目時間表。 有關構成項目範圍更改的資訊，請參見 <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">重新計算項目時間表</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>將多個用戶分配給任務時，請使用</strong> </p> </td> 
   <td> <p>如果項目沒有分配計畫，或者分配給其任務的用戶沒有為其分配計畫，則Workfront會使用系統預設計畫來計算任務的時間軸。</p> <p>如果在項目中為同一任務分配了多個用戶，並且分配給任務的用戶也分配了調度，則Workfront將使用以下調度：</p> 
    <ul> 
     <li><strong>主分配</strong>:Workfront使用任務上的主分配計畫來計算時間表。</li> 
     <li><strong>專案</strong>:Workfront會使用專案的排程來計算每個任務的時間軸。</li> 
    </ul> <p>如需排程的詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">建立排程</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>時間表計算 </p> </td> 
   <td> 
    <ul> 
     <li><strong>每個工作日的一般小時數</strong>:為將負責專案的使用者設定一般工作日的小時數。 預設為8小時。</li> 
    </ul> 
    <ul> 
     <li><strong>每週的一般工作日</strong>:為將負責專案的使用者設定標準工作周。 預設為5天。</li> 
    </ul> <p>這2個選項將天轉換為小時，或將週轉換為天。</p> <p>例如，如果您的任務具有8個計畫小時，並且持續時間是根據計畫小時數計算的，則Workfront會將這些小時轉換為天，以便將持續時間顯示為天。</p> <p>從「每週一般工作天數」欄位中，Workfront會計算系統的「相當全職(FTE)」值。 這是Workfront在計算使用者分配時使用的功能。</p> <p>在計畫項目時間表、資源預算或根據項目記錄時間時，將使用這些值。 </p> <p>為系統中的用戶建立工時單時不使用這些工時表，如 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">配置工時單和小時首選項</a>.</p> <p><b>注意</b>:Workfront管理員無法解除鎖定時間軸計算偏好設定。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p><strong>自訂季度</strong> </p> </td> 
   <td> <p>為將負責專案的使用者設定自訂每年季度。 自訂季度通常是季度，與日曆年度中傳統的季度劃分不匹配。 您可以新增多個自訂季別。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">啟用項目的自定義季數</a>.</p> <p><b>注意</b>:Workfront管理員無法解除鎖定自訂季度偏好設定。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 業務案例 {#business-cases}

您可以為與組關聯的新建項目建立業務案例，以提交項目請求。 您可以定義偏好設定，以決定 **業務案例** 表單。 建議您啟用這些選項，以便其他工具(例如Portfolio優化程式)正確更新。 如需每個欄位顯示內容的詳細資訊，請參閱 [定義業務案例](../../../manage-work/projects/define-a-business-case/define-business-case.md).

在Workfront管理員啟用「業務案例」部分後，項目所有者就可以在項目級別建立「業務案例」。 有關建立業務案例的資訊，請參閱 [為項目建立業務案例](../../../manage-work/projects/define-a-business-case/create-business-case.md).

### 到期後生命期  {#life-after-death}

為與組關聯的新建立項目配置以下任何首選項：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><strong>專案標示為「完成」後，使用者仍可</strong> </p> </td> 
   <td> <p>確定組織（或組，如果要配置組的項目首選項）的規則，以確定在項目狀態標籤為「完成」後是否可以刪除任務或問題。</p> 
    <ul> 
     <li><strong>刪除任務</strong>:可讓使用者在專案標示為「完成」後，從專案刪除工作。<br></li> 
     <li><strong>刪除問題</strong>:可讓使用者在專案標示為「完成」後，從專案刪除問題。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>將項目標籤為「完成」、「已死」或「待批准」後，人們仍然可以</strong> </p> </td> 
   <td> <p>確定組織（或組，如果您正在為組配置項目首選項）的規則，以了解在標籤項目狀態後項目中的任務、問題、文檔和其他對象會發生什麼情況 <strong>完成</strong>, <strong>死亡</strong>，或 <strong>待批准</strong>.</p> 
    <ul> 
     <li><strong>添加和編輯任務</strong> 允許用戶： 
      <ul> 
       <li>在項目被標籤為「完成」、「無效」或「待批准」後，編輯項目內的任務。 這包括添加小時和更改任務上的費用條目。</li> 
       <li>新增任務至專案。</li> 
      </ul></li> 
     <li><strong>新增和編輯問題</strong>:允許用戶： 
      <ul> 
       <li>在項目標籤為「完成」、「無效」或「待批准」後，編輯項目內的問題。</li> 
       <li>在專案標示為「完成」或「已停用」後，將問題新增至專案。 （您無法向「待批准」的項目添加問題。）</li> 
      </ul></li> 
     <li> <p><strong>將文檔添加到項目及其任務和問題</strong>:允許用戶在將項目標籤為「完成」或「無效」後將文檔添加到項目（或將文檔添加到項目內的任務和問題）。</p> <p>此選項不適用於待批准的項目。</p> </li> 
     <li> <p><strong>附加範本</strong>:允許用戶在將項目標籤為「完成」或「無效」後將模板附加到項目。</p> <p>此選項不適用於待批准的項目。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
