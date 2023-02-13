---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 配置系統範圍的項目首選項
description: 作為 [!DNL Adobe Workfront] 管理員，您可以為整個系統中建立的所有項目配置預設首選項。 這些首選項會影響項目、任務和問題行為。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1a1affed-1b06-442c-98b2-9f360eee767b
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '2475'
ht-degree: 1%

---

# 配置系統範圍的項目首選項

作為 [!DNL Adobe Workfront] 管理員，您可以為整個系統中建立的所有項目配置預設首選項。 這些首選項會影響項目、任務和問題行為。

>[!NOTE]
>
>預設情況下，這些首選項被鎖定，除非您為整個系統中的所有組解鎖這些首選項，否則組管理員無法在組級別修改它們。 如需詳細資訊，請參閱 [鎖定或解鎖系統中所有組的項目首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td>[!UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置</td> 
   <td> <p>您必須是 [!DNL Workfront] 管理員。</p> <p><b>注意</b>:如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 為整個組織配置項目首選項

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **[!UICONTROL 專案偏好設定]** > **[!UICONTROL 專案]**.

1. 在顯示的頁面上，繼續下列4個區段的其中一個，以設定的偏好設定 [!UICONTROL 專案狀態], [!UICONTROL 時間軸], [!UICONTROL 業務案例]，和 [!UICONTROL 死後生命].
1. 如果希望組織中的所有組使用相同的項目首選項，請確保鎖定每個首選項 ![](assets/lock-toggle-button.png) （此為預設值）。

   >[!IMPORTANT]
   >
   >項目首選項被鎖定後，系統中的所有組將繼承您對該首選項所做的任何更改。 務必與整個組織的使用者和群組通訊，以確保以您設定專案偏好設定的方式滿足所有需求。

   有關解鎖首選項以便所有組都可以自行配置和管理首選項的資訊，請參見 [鎖定或解鎖系統中所有組的項目首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

1. 按一下&#x200B;**[!UICONTROL 儲存]**。

* [[!UICONTROL 專案狀態]](#project-status)
* [[!UICONTROL 時間表]](#timelines)
* [[!UICONTROL 業務案例]](#business-cases)
* [[!UICONTROL 到期後生命期]](#life-after-death)

### 專案狀態 {#project-status}

為整個系統中新建立的項目配置以下任何首選項：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL允許用戶不使用模板而建立項目]</td> 
   <td>  <p>從以下區域建立專案時，此偏好設定可讓使用者無須使用範本即可建立專案： </p>
      <ul>
        <li>
        <p>在專案清單中使用[!UICONTROL新增專案]選項</p>
        </li>
          <li>
          <p>將問題從問題頁面轉換為專案</p>
          </li>
         </ul>
        <p>預設會啟用此偏好設定。 </p> 
        <p><b>附註</b></p>
        <p> 組管理員可以更改組的此首選項。 當用戶屬於具有不同首選項的多個組時，如果用戶的「首頁組」啟用了此首選項，則允許用戶建立不含模板的項目。</p> 
        </td> 
  </tr>
  <tr> 
   <td role="rowheader">[!UICONTROL將新項目的狀態設定為]</td> 
   <td> <p>確定新項目的狀態。</p>  <p><b>附註</b>  
     <ul> 
      <li>若您或其他 [!DNL Workfront] 管理員隱藏此處選擇的狀態，預設狀態將更改為狀態清單中的第一個狀態。</li> 
     </ul> 
     <ul> 
      <li> <p>如果鎖定的系統或組狀態被設定為預設狀態，之後有人解除鎖定，則系統會嘗試將其替換為相同狀態類型的鎖定狀態。</p> <p>如果找不到，則會尋找必要狀態：</p> 
       <ul> 
        <li>如果存在相當於未鎖定預設狀態的必需狀態，則必需狀態將變為預設狀態，即使它處於未鎖定狀態。</li> 
        <li>如果所有必需狀態均不等於未鎖定的預設狀態，則狀態清單中的第一個必需狀態將變為預設狀態。</li> 
       </ul> <p>如需所需狀態的詳細資訊，請參閱文章 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">訪問系統項目狀態清單</a>, <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">訪問系統任務狀態清單</a>，和 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">訪問系統問題狀態清單</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL根據]計算完成百分比</td> 
   <td> <p>項目或父任務的完成百分比取決於任務的整體進度。 此資訊可以根據項目上任務的「持續時間」或「計畫時數」計算。</p> <p>如果選擇[!UICONTROL持續時間]，則項目中每個任務的持續時間將決定項目的整體完成百分比，而每個子任務的持續時間將決定其父任務的整體完成百分比。</p> <p>如果選擇[!UICONTROL持續時間]，請務必在[!UICONTROL時間軸]部分中指定[!UICONTROL每工作日的典型小時數]和[!UICONTROL每週的典型工作日數]。 [!DNL Workfront] 根據「持續時間」計算任務完成百分比時，會使用此資訊。 </p> <p>如果選擇[!UICONTROL計畫小時數]，請確保每個項目上的所有任務都已定義[!UICONTROL計畫小時數]，並且該金額不為零。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL根據進度狀態自動設定項目的條件]</td> 
   <td> <p>此首選項允許用戶手動設定項目的[!UICONTROL條件]（在Target上]、[!UICONTROL在風險中]、[!UICONTROL在故障中]）或 [!DNL Workfront] 根據專案在時間軸上的進度，自動設定[!UICONTROL條件]（進度狀態）。 如需專案條件的詳細資訊，請參閱 <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">專案條件和條件類型概觀</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL自動建立基線]</p> </td> 
   <td> <p>當項目狀態更改為[!UICONTROL當前]時，此首選項會自動建立任務和項目詳細資訊的基線（快照）。 如需建立基線的相關資訊，請參閱 <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">建立專案基線</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL效能索引方法] </p> </td> 
   <td> <p>項目的效能索引方法(PIM)控制該方法 [!DNL Workfront] 用於計算掙值度量，如[!UICONTROL成本效能指數](CPI)和[!UICONTROL完成時估計](EAC)。 如需詳細資訊，請參閱 <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">計算[!UICONTROL成本效能指數](CPI)</a> 和 <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL完成時計算估計](EAC)</a></p> 
    <ul> 
     <li><strong>[!UICONTROL以小時為基礎]</strong>: [!DNL Workfront] 使用[!UICONTROL計畫時數]來計算效能量度，如EAC和CPI。 根據小時計算PIM時，EAC會顯示為小時數。 請確定您有[!UICONTROL計畫小時數]的值，而不是零。</li> 
     <li> <p><strong>[!UICONTROL基於成本]</strong>: [!DNL Workfront] 使用[!UICONTROL計畫人工成本]來計算效能度量，如EAC和CPI。 確保您的工作角色或用戶與每小時成本費率相關聯。 根據成本計算PIM時，EAC會顯示為貨幣值。</p> <p>項目經理可以使用[!UICONTROL項目詳細資訊]中的[!UICONTROL財務]區域在項目級別修改此設定。 如需詳細資訊，請參閱 <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">管理項目[!UICONTROL Finance]區域中的資訊</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL完成時的估計]</p> </td> 
   <td> <p>決定哪些資料 [!DNL Workfront] 用於計算[!UICONTROL完成時估計](EAC)，它表示項目的預計總成本。</p> 
    <ul> 
     <li><strong>[!UICONTROL在項目級別計算]</strong>：父任務和項目的EAC通過在EAC公式中輸入[!UICONTROL實際小時數]或[!UICONTROL實際人工成本]來確定。 此計算包括直接添加到父任務或項目的[!UICONTROL實際小時數]或[!UICONTROL成本和費用]。</li> 
     <li> <p><strong>[!UICONTROL從任務/子任務匯總]</strong>:父任務和項目的EAC通過加總每個子任務的EAC來確定。 此計算不包括直接添加到父任務或項目的[!UICONTROL實際小時數]或[!UICONTROL實際成本和費用]。</p> <p>項目經理可以使用[!UICONTROL項目詳細資訊]中的[!UICONTROL財務]區域在項目級別修改此設定。有關詳細資訊，請參閱 <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">管理項目[!UICONTROL Finance]區域中的資訊</a>.</p> </li> 
    </ul> <p>有關EAC計算方式的詳細資訊，請參見 <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">完成時計算[!UICONTROL估計](EAC)</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 時間表 {#timelines}

為整個系統中新建立的項目配置以下任何首選項：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL從]計畫</td> 
   <td> <p>確定新項目是從建立日期開始還是從完成日期開始計畫。</p> 
    <ul> 
     <li><strong>[!UICONTROL開始日期]</strong>:新任務預設為[!UICONTROL盡快]任務約束，系統將提示項目經理為項目提供[!UICONTROL計畫起始日期]。</li> 
     <li><strong>[!UICONTROL完成日期]</strong>:新任務預設為[!UICONTROL（盡可能晚）任務約束，系統將提示項目經理為項目提供[!UICONTROL計畫完成日期]。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL用戶關閉時間]</td> 
   <td> <p>確定任務的主要受託人的休息時間是否調整項目上該任務的計畫日期。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL將用戶時間考慮為任務持續時間]</strong>:為任務的主要受託人計畫的任何時間，如果在任務期間發生了關閉時間，則會調整任務的計畫日期。 這是預設設定。 </p> <p>例如，如果某個約束為[!UICONTROL Ass Op Hos Possy Pe Mek Op Peffice]的任務計畫在6月1日開始並在6月3日完成，而主要受託人在6月2日標籤為「Time-off」，則任務的計畫日期將調整為6月1日到6月4日。</p> <p><b>重要</b>:選擇此設定時，任務的持續時間不會更改。 根據「任務約束」，僅更改計畫日期。</p> </li> 
     <li><strong>[!UICONTROL忽略任務持續時間中的用戶超時]</strong>:項目上每個任務的計畫日期仍按原計畫進行，即使任務的主要受託人在其期間有時間休息。</li> 
    </ul> <p>為此設定選取選項時，請考量下列事項：</p> 
    <ul> 
     <li>更改此設定時，只有在更改後建立的項目和模板才會繼承更新的設定。 </li> 
     <li> <p>任務的任務約束值確定要調整的計畫任務日期： </p> 
      <ul> 
       <li>計畫開始日期</li> 
       <li>計畫完成日期</li> 
       <li>兩個日期</li> 
       <li>兩個日期都沒有。 </li> 
      </ul> <p>例如，如果任務的約束為[!UICONTROL固定日期]，則當主要受託人超時時，即使選擇了「[!UICONTROL在任務持續時間中考慮用戶超時」選項，日期也不會調整。 有關任務約束的資訊，請參閱 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">任務約束概覽</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL項目時間表將自動重新計算]</p> </td> 
   <td> <p>決定何時重新計算專案時間表。 有關重新計算項目時間軸的資訊，請參閱 <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">重新計算項目時間表</a>.</p> <p>預設會啟用下列選項。 您可以選取下列一或多個設定：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL每晚]</strong>:選擇此選項可以每晚重新計算項目時間表。 您對專案所做的任何可能會影響時間軸的變更都不會立即顯示。 [!DNL Workfront​​​] 僅在滿足以下兩個條件的項目的夜間重新計算時間：</p> <p> 
       <ul> 
        <li>狀態為[!UICONTROL當前]</li> 
        <li>過去3個月有過更新</li> 
       </ul> </p> </li> 
     <li> <p><strong>項目範圍更改時</strong>:選擇此選項可在項目範圍發生更改時立即重新計算項目時間表。 有關構成項目範圍更改的資訊，請參見 <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">重新計算項目時間表</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL當將多個用戶分配給任務時，請使用的計畫]</p> </td> 
   <td> <p>如果項目沒有分配計畫，或者分配給其任務的用戶沒有為其分配計畫， [!DNL Workfront] 使用系統預設計畫來計算任務的時間軸。</p> <p>如果在項目中為同一任務分配了多個用戶，並且分配給任務的用戶也分配了調度，[!UICONTROL Workfront]將使用以下調度：</p> 
    <ul> 
     <li><strong>[!UICONTROL主分配]</strong>: [!DNL Workfront] 使用任務上的主分配計畫來計算時間表。</li> 
     <li><strong>[!UICONTROL項目]</strong>: [!DNL Workfront] 使用項目的時間表來計算每個任務的時間表。</li> 
    </ul> <p>如需排程的詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">建立排程</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL時間軸計算] </p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL每個工作日的典型小時數]</strong>:為將負責專案的使用者設定一般工作日的小時數。 預設為8小時。</li> 
    </ul> 
    <ul> 
     <li><strong>[!UICONTROL每週一般工作日]</strong>:為將負責專案的使用者設定標準工作周。 預設為5天。</li> 
    </ul> <p>這2個選項將天轉換為小時，或將週轉換為天。</p> <p>例如，如果您的任務具有8個計畫小時，並且持續時間是根據計畫小時數計算的， [!DNL Workfront] 將這些小時轉換為天，以便將「持續時間」顯示為天。</p> <p>從「典型[!UICONTROL每週工作天數]」欄位， [!DNL Workfront] 計算系統的「等效全職(FTE)」值。 這就是 [!DNL Workfront] 在計算用戶分配時使用。</p> <p>在計畫項目時間表、資源預算或根據項目記錄時間時，將使用這些值。 </p> <p>為系統中的用戶建立工時單時不使用這些工時表，如 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL配置]時間表和小時首選項</a>.</p> <p><b>注意</b>: [!DNL Workfront] 管理員無法解鎖[!UICONTROL時間軸計算]首選項。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL自定義季度]</p> </td> 
   <td> <p>為將負責專案的使用者設定自訂每年季度。 自訂季度通常是季度，與日曆年度中傳統的季度劃分不匹配。 您可以新增多個自訂季別。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">啟用項目的自定義季數</a>.</p>  <p><b>注意</b>: [!DNL Workfront] 管理員無法解鎖[!UICONTROL自定義季度]首選項。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 業務案例] {#business-cases}

您可以在整個系統中為新建立的項目建立業務案例，以提交項目請求。 您可以定義偏好設定，以決定 **[!UICONTROL 業務案例]** 表單。 建議您啟用這些選項，以便使用其他工具，例如 [!UICONTROL Portfolio優化程式]，請正確更新。 如需每個欄位顯示內容的詳細資訊，請參閱 [定義業務案例](../../../manage-work/projects/define-a-business-case/define-business-case.md).

在 [!DNL Workfront] 管理員會啟用 [!UICONTROL 業務案例]，專案擁有者就可以在專案層級建立業務案例。 有關建立業務案例的資訊，請參閱 [為項目建立業務案例](../../../manage-work/projects/define-a-business-case/create-business-case.md).

### [!UICONTROL 到期後生命期] {#life-after-death}

為整個系統中新建立的項目配置以下任何首選項：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL在將專案標示為「完成」後，人們仍可] </p> </td> 
   <td> <p>確定組織（或組，如果要配置組的項目首選項）的規則，以確定在項目狀態標籤為[!UICONTROL完成]後是否可以刪除任務或問題。</p> 
    <ul> 
     <li><strong>[!UICONTROL刪除任務]</strong>:允許用戶在項目被標籤為[!UICONTROL完成]後從項目中刪除任務。<br></li> 
     <li><strong>[!UICONTROL刪除問題]</strong>:可讓使用者在專案標示為[!UICONTROL完成]後，從專案刪除問題。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL在將項目標籤為「完成」、「死」或「待批准」後，人們仍然可以]</p> </td> 
   <td> <p>確定組織（或組，如果您正在為組配置項目首選項）的規則，以了解在標籤項目狀態後項目中的任務、問題、文檔和其他對象會發生什麼情況 <strong>[!UICONTROL完成]</strong>, <strong>[!UICONTROL死亡]</strong>，或 <strong>[!UICONTROL待批准]</strong>.</p> 
    <ul> 
     <li><strong>[!UICONTROL添加和編輯任務]</strong> 允許用戶：
      <ul>
       <li>在項目被標籤為[!UICONTROL Complete]、[!UICONTROL Dead]或[!UICONTROL Pending Approval]後編輯項目內的任務。 這包括添加小時和更改任務上的費用條目。</li>
       <li>新增任務至專案。</li>
      </ul></li> 
     <li><strong>[!UICONTROL添加和編輯問題]</strong>:允許用戶：
      <ul>
       <li>在項目被標籤為[!UICONTROL Complete]、[!UICONTROL Dead]或[!UICONTROL Pending Approval]後，編輯項目內的問題。</li>
       <li>在專案標示為[!UICONTROL Complete]或[!UICONTROL Dead]後，將問題新增至專案。 （您無法向[!UICONTROL待批准]項目添加問題。）</li>
      </ul></li> 
     <li> <p><strong>[!UICONTROL向項目及其任務和問題添加文檔]</strong>:允許用戶在將項目標籤為[!UICONTROL Complete]或[!UICONTROL Dead]後，將文檔添加到項目（或將文檔添加到項目內的任務和問題）。</p> <p>此選項不適用於待批准的項目。</p> </li> 
     <li> <p><strong>[!UICONTROL附加模板]</strong>:允許用戶在將項目標籤為[!UICONTROL Complete]或[!UICONTROL Dead]後將模板附加到項目。</p> <p>此選項不適用於待批准的項目。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
