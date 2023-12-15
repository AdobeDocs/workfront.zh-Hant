---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 設定全系統專案偏好設定
description: 作為 [!DNL Adobe Workfront] 管理員，您可以為在整個系統中建立的所有專案設定預設偏好設定。 這些偏好設定會影響專案、任務和問題行為。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1a1affed-1b06-442c-98b2-9f360eee767b
source-git-commit: fb1c7ade6622db391e0dac54f37603efe9dc0a58
workflow-type: tm+mt
source-wordcount: '2522'
ht-degree: 0%

---

# 設定全系統專案偏好設定

作為 [!DNL Adobe Workfront] 管理員，您可以為在整個系統中建立的所有專案設定預設偏好設定。 這些偏好設定會影響專案、任務和問題行為。

>[!NOTE]
>
>依照預設，這些偏好設定會鎖定，群組管理員無法在群組層級修改它們，除非您為整個系統中的所有群組解除鎖定它們。 如需詳細資訊，請參閱 [鎖定或解除鎖定系統中所有群組的專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

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
   <td>[！UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是 [!DNL Workfront] 管理員。</p> <p><b>注意</b>：如果您還是沒有存取權，請詢問您的 [!DNL Workfront] 管理員是否對您的存取層級設定其他限制。 如需瞭解如何 [!DNL Workfront] 管理員可以修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 設定整個組織的專案偏好設定

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![](assets/main-menu-icon.png) 位於的右上角 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **[!UICONTROL 專案偏好設定]** > **[!UICONTROL 專案]**.

1. 在出現的頁面上，繼續下列的4個區段之一，以設定偏好設定 [!UICONTROL 專案狀態]， [!UICONTROL 時間表]， [!UICONTROL 業務案例]、和 [!UICONTROL 死亡後期限].
1. 如果您希望整個組織中的所有群組都使用相同的專案偏好設定，請確定每個偏好設定都已鎖定 ![](assets/lock-toggle-button.png) （這是預設值）。

   >[!IMPORTANT]
   >
   >鎖定專案偏好設定時，對該偏好設定所做的任何變更都會被系統中的所有群組繼承。 務必與整個組織的使用者和群組溝通，以確保以您設定專案偏好設定的方式考慮到所有需求。

   如需解鎖偏好設定以便所有群組可以自行設定及管理的相關資訊，請參閱 [鎖定或解除鎖定系統中所有群組的專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

1. 按一下「**[!UICONTROL 儲存]**」。

* [[!UICONTROL 專案狀態]](#project-status)
* [[!UICONTROL 時間表]](#timelines)
* [[!UICONTROL 業務案例]](#business-cases)
* [[!UICONTROL 結束後期限]](#life-after-death)

### 專案狀態 {#project-status}

為整個系統的新建立專案設定下列任一偏好設定：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL允許使用者在不使用範本的情況下建立專案]</td> 
   <td>  <p>此偏好設定可讓使用者在從下列區域建立專案時，無需使用範本即可建立專案： </p>
      <ul>
        <li>
        <p>在專案清單中使用[！UICONTROL新增專案]選項</p>
        </li>
          <li>
          <p>從問題頁面將問題轉換為專案</p>
          </li>
         </ul>
        <p>此偏好設定預設為啟用。 </p> 
        <p><b>附註</b></p>
        <p> 群組管理員可以變更群組的此偏好設定。 當使用者屬於具有不同偏好設定的多個群組時，如果使用者的主群組啟用了此偏好設定，則允許使用者建立沒有範本的專案。</p> 
        </td> 
  </tr>
  <tr> 
   <td role="rowheader">[！UICONTROL將新專案狀態設定為]</td> 
   <td> <p>決定新專案的狀態。</p>  <p><b>注意</b>  
     <ul> 
      <li>如果您或另一個 [!DNL Workfront] 管理員會隱藏此處選取的狀態，預設狀態會變更為狀態清單中的第一個狀態。</li> 
     </ul> 
     <ul> 
      <li> <p>如果鎖定的系統或群組狀態設定為預設狀態，稍後有人將其解鎖，則系統會嘗試以相同狀態型別的鎖定狀態來取代它。</p> <p>如果找不到，會尋找必要的狀態：</p> 
       <ul> 
        <li>如果必要的狀態等於已解除鎖定的預設狀態，則即使已解除鎖定，「必要」狀態也會變成預設狀態。</li> 
        <li>如果所有必要狀態都不等同於已解除鎖定的預設狀態，則狀態清單中的第一個必要狀態會成為預設狀態。</li> 
       </ul> <p>如需必要狀態的相關資訊，請參閱文章 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">存取系統專案狀態清單</a>， <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">存取系統工作狀態清單</a>、和 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">存取系統問題狀態清單</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL計算完成百分比依據]</td> 
   <td> <p>專案或父系任務的完成百分比取決於任務的整體進度。 此資訊可以根據專案上任務的期間或計畫時數計算。</p> <p>如果您選取[！UICONTROL工期]，專案中每個任務的「工期」會決定專案的整體完成百分比，而每個子任務的「工期」則會決定其父系任務的整體完成百分比。</p> <p>如果您選取[！UICONTROL Duration]，請務必在[！UICONTROL時間表]區段中指定[！UICONTROL每工作日一般小時數]和[！UICONTROL每週一般工作日數]。 [!DNL Workfront] 根據期間計算任務的完成百分比時，會使用此資訊。 </p> <p>如果您選取[！UICONTROL計畫時數]，請確認每個專案上的所有任務已定義總計[！UICONTROL計畫時數]，且該金額不是零。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL根據進度狀態自動設定專案條件]</td> 
   <td> <p>此偏好設定可讓使用者手動設定專案的[！UICONTROL條件] ([！UICONTROL On Target]、[！UICONTROL At Risk]、[！UICONTROL In Trouble])或具有 [!DNL Workfront] 根據專案在時間表上的進度自動設定[！UICONTROL條件] （進度狀態）。 如需專案條件的詳細資訊，請參閱 <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">專案狀態與狀態型別概觀</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL自動建立基準線]</p> </td> 
   <td> <p>當專案狀態變更為[！UICONTROL目前]時，此偏好設定會自動建立任務和專案詳細資訊的基準（快照）。 如需有關建立基準線的資訊，請參閱 <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">建立專案基準線</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL績效指數方法] </p> </td> 
   <td> <p>專案的績效指數方法(PIM)控制此方法 [!DNL Workfront] 使用計算收益值量度，例如[！UICONTROL成本績效指數] (CPI)和[！UICONTROL完工估算] (EAC)。 如需詳細資訊，請參閱 <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">計算[！UICONTROL成本績效指數] (CPI)</a> 和 <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">[！UICONTROL完工估算計算] (EAC)</a></p> 
    <ul> 
     <li><strong>[！UICONTROL Hour-based]</strong>： [!DNL Workfront] 使用[！UICONTROL計畫時數]計算EAC和CPI等績效量度。 當根據時數計算PIM時，EAC會顯示為時數。 確保您有[！UICONTROL計畫時數]的值，而不是零。</li> 
     <li> <p><strong>[！UICONTROL基於成本]</strong>： [!DNL Workfront] 使用[！UICONTROL計畫勞力成本]計算EAC和CPI等績效量度。 確保您的工作角色或使用者與每小時成本費率相關聯。 根據「成本」計算PIM時，EAC會顯示為貨幣值。</p> <p>專案經理可以使用[！UICONTROL專案詳細資料]中的[！UICONTROL財務]區域，在專案層級修改此設定。 如需詳細資訊，請參閱 <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">管理專案[！UICONTROL Finance]區域中的資訊</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL完工估算]</p> </td> 
   <td> <p>決定哪些資料 [!DNL Workfront] 使用計算[！UICONTROL預估完成成本] (EAC)，代表專案的預估總成本。</p> 
    <ul> 
     <li><strong>[！UICONTROL在專案層級計算]</strong>：父系任務和專案的EAC是在EAC公式中輸入[！UICONTROL實際時數]或[！UICONTROL實際勞力成本]來決定。 此計算包括直接新增到父級任務或專案的[！UICONTROL實際時數]或[！UICONTROL成本和費用]。</li> 
     <li> <p><strong>[！UICONTROL從任務/子任務彙總]</strong>：父系任務和專案的EAC是由每個子系任務的EAC相加決定。 此計算不包括直接新增至父級任務或專案的[！UICONTROL實際時數]或[！UICONTROL實際成本和費用]。</p> <p>專案經理可以使用[！UICONTROL專案詳細資料]中的[！UICONTROL財務]區域，在專案層級修改此設定。如需詳細資訊，請參閱 <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">管理專案[！UICONTROL Finance]區域中的資訊</a>.</p> </li> 
    </ul> <p>如需有關EAC如何計算的詳細資訊，請參閱 <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">計算[！UICONTROL完工估算] (EAC)</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 時間表 {#timelines}

為整個系統的新建立專案設定下列任一偏好設定：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL排程起始日期]</td> 
   <td> <p>決定新專案是從開始日期排程，還是從建立專案時的完成日期排程。</p> 
    <ul> 
     <li><strong>[！UICONTROL開始日期]</strong>：新任務預設為[！UICONTROL Task Constraint （儘快）並提示專案經理提供專案的[！UICONTROL規劃開始日期]。</li> 
     <li><strong>[！UICONTROL完成日期]</strong>：新任務預設為[！UICONTROL儘可能遲]任務限制，並且會提示專案經理提供專案的[！UICONTROL規劃完成日期]。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL使用者休假]</td> 
   <td> <p>決定任務的主要受指派人的休假是否調整專案上該任務的計畫日期。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL考量使用者在任務持續期間的休假]</strong>：如果休假發生在任務持續期間，為任務的主要受指派人排定的任何休假都會調整任務的計畫日期。 這是預設設定。 </p> <p>例如，如果限製為[！UICONTROL]的任務排程在6月1日開始並在6月3日完成，而主要受指派人將6月2日標籤為休假，則任務的計畫日期將調整為6月1日至6月4日。</p> <p><b>重要</b>：任務期間在選取此設定時不會變更。 根據任務限制，只有計畫日期會變更。</p> </li> 
     <li><strong>[！UICONTROL忽略使用者在任務持續期間的休假]</strong>：專案上每個任務的計畫日期仍維持原計畫，即使任務的主要受指派人在其期間有休假。</li> 
    </ul> <p>選取此設定的選項時，請考量下列事項：</p> 
    <ul> 
     <li>當您變更此設定時，只有變更後建立的專案和範本會繼承更新的設定。 </li> 
     <li> <p>任務的「任務限制」值決定要調整哪些計畫任務日期： </p> 
      <ul> 
       <li>計畫開始日期</li> 
       <li>計畫完成日期</li> 
       <li>兩個日期</li> 
       <li>兩者皆非。 </li> 
      </ul> <p>例如，如果任務的限製為[！UICONTROL固定日期]，則即使選取了[！UICONTROL考慮使用者在任務期間內的休息時間]選項，當主要受指派人具有休息時間時，日期也不會調整。 有關任務限制的資訊，請參閱 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">任務限制總覽</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL專案時間表將自動重新計算]</p> </td> 
   <td> <p>決定重新計算專案的時間表。 如需重新計算專案時間表的相關資訊，請參閱 <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">重新計算專案時間表</a>.</p> <p>預設會啟用下列選項。 您可以選取下列一或多個設定：</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL每晚]</strong>：選取此項以每晚重新計算專案時間表。 您對專案所做的任何可能影響時間表的變更都不會立即顯示。 [!DNL Workfront​​​] 只有在滿足以下兩個條件的專案中，才會在夜間重新計算時間表：</p> <p> 
       <ul> 
        <li>狀態為[！UICONTROL目前]</li> 
        <li>在過去3個月內已更新</li> 
        <li>更新型別為下列其中一項：</li>
        <ul>
        <li>自動與專案變更時</li>
        <li>僅限變更</li>
        <li>僅限自動</li> 
      </ul>       
    <b>秘訣</b>
    <p>此設定不會影響更新型別為「僅限手動」的專案。</p>
    <li> <p><strong>專案範圍變更時</strong>：選取此專案可在專案範圍變更時立即重新計算專案時間表。 如需有關構成專案範圍變更之內容的資訊，請參閱 <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">重新計算專案時間表</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL將多位使用者指派到一個任務時，請使用]的排程</p> </td> 
   <td> <p>如果專案未指派排程，或指派給其任務的使用者未指派排程， [!DNL Workfront] 使用系統預設排程來計算任務的時間表。</p> <p>如果您在專案中將多個使用者指派給同一個任務，而且指派給該任務的使用者也指派了時間表，則[！UICONTROL Workfront]會使用以下時間表：</p> 
    <ul> 
     <li><strong>[！UICONTROL主要指派]</strong>： [!DNL Workfront] 使用任務上主要指派的排程來計算時間表。</li> 
     <li><strong>[！UICONTROL專案]</strong>： [!DNL Workfront] 使用專案排程來計算每項工作的時間表。</li> 
    </ul> <p>如需排程的詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">建立排程</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[！UICONTROL時間表計算] </p> </td> 
   <td> 
    <ul> 
     <li><strong>[！UICONTROL每工作日一般小時數]</strong>：針對將處理專案的使用者，設定一般工作日的小時數。 預設值為8小時。</li> 
    </ul> 
    <ul> 
     <li><strong>[！UICONTROL每週一般工作天數]</strong>：為處理專案的使用者設定標準工作週。 預設值為5天。</li> 
    </ul> <p>這2個選項會將天數轉換為小時，或將周數轉換為天數。</p> <p>例如，如果您有一個任務具有8個計畫時數，而持續時間是根據計畫時數計算的， [!DNL Workfront] 將這些小時轉換為天，以便將「持續時間」顯示為天。</p> <p>從一般[！UICONTROL每週工作天數]欄位， [!DNL Workfront] 會計算系統的全時當量(FTE)值。 這是什麼 [!DNL Workfront] 在計算使用者的分配時使用。</p> <p>當您計畫專案時間表、編列資源預算或針對專案記錄時間時，會使用這些值。 </p> <p>當您在系統中為使用者建立時程表時，不會使用這些時間表，如中所述 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">[！UICONTROL設定]時程表和小時偏好設定</a>.</p> <p><b>注意</b>： [!DNL Workfront] 管理員無法解鎖[！UICONTROL時間表計算]喜好設定。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[！UICONTROL自訂季度]</p> </td> 
   <td> <p>為將處理專案的使用者設定自訂每年季度。 自訂季度通常是不符合日曆年度中傳統季度劃分的季度。 您可以新增多個自訂季度。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">啟用專案的自訂季度</a>.</p>  <p><b>注意</b>： [!DNL Workfront] 管理員無法解鎖[！UICONTROL自訂季度]喜好設定。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 業務案例] {#business-cases}

您可以為整個系統的新建立專案建立業務案例，以提交專案請求。 您可以定義偏好設定以決定哪些區域可顯示在 **[!UICONTROL 業務案例]** 表單。 建議您啟用這些選項，以便其他工具(例如 [!UICONTROL Portfolio最佳化工具]，請正確更新。 如需每個欄位顯示內容的詳細資訊，請參閱 [定義業務案例：文章索引](../../../manage-work/projects/define-a-business-case/define-business-case.md).

在 [!DNL Workfront] 管理員會啟用 [!UICONTROL 業務案例]，專案所有者就可以在專案層級建立業務案例。 如需建立業務案例的相關資訊，請參閱 [為專案建立業務案例](../../../manage-work/projects/define-a-business-case/create-business-case.md).

### [!UICONTROL 結束後期限] {#life-after-death}

為整個系統的新建立專案設定下列任一偏好設定：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL將專案標籤為完成之後，人員仍可] </p> </td> 
   <td> <p>決定您的組織（或群組，如果您是設定群組的專案偏好設定）的規則，這些規則有關於在專案狀態標籤為[！UICONTROL完成]後是否可以刪除任務或問題。</p> 
    <ul> 
     <li><strong>[！UICONTROL刪除任務]</strong>：可讓使用者在專案被標示為[！UICONTROL完成]後，從專案中刪除任務。<br></li> 
     <li><strong>[！UICONTROL刪除問題]</strong>：可讓使用者在專案標籤為[！UICONTROL完成]後，從專案中刪除問題。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL將專案標籤為「完成」、「廢棄」或「未決核准」之後，人員仍可]</p> </td> 
   <td> <p>決定您的組織（或群組，如果您是設定群組的專案偏好設定）的規則，這些規則有關於標示專案狀態後專案中任務、問題、檔案和其他物件會發生什麼情況 <strong>[！UICONTROL完成]</strong>， <strong>[！UICONTROL廢棄]</strong>，或是 <strong>[！UICONTROL未決核准]</strong>.</p> 
    <ul> 
     <li><strong>[！UICONTROL新增及編輯工作]</strong> 允許使用者：
      <ul>
       <li>在專案標籤為[！UICONTROL完成]、[！UICONTROL已廢棄]或為[！UICONTROL未決核准]之後，編輯專案中的任務。 這包括新增時數以及變更任務上的費用輸入項。</li>
       <li>將任務新增至專案。</li>
      </ul></li> 
     <li><strong>[！UICONTROL新增和編輯問題]</strong>：允許使用者：
      <ul>
       <li>在專案標籤為[！UICONTROL完成]、[！UICONTROL廢棄]或[！UICONTROL未決核准]之後，編輯專案中的問題。</li>
       <li>在專案標籤為[！UICONTROL完成]或[！UICONTROL已廢棄]後，將問題新增至專案。 （您無法將「[！UICONTROL未決核准]」問題新增至專案。）</li>
      </ul></li> 
     <li> <p><strong>[！UICONTROL將檔案新增至專案及其任務和問題]</strong>：可讓使用者在專案標籤為[！UICONTROL完成]或[！UICONTROL廢棄]後，將檔案新增至專案（或將檔案新增至專案內的任務和問題）。</p> <p>此選項不適用於等待核准的專案。</p> </li> 
     <li> <p><strong>[！UICONTROL附加範本]</strong>：允許使用者在專案標籤為[！UICONTROL完成]或[！UICONTROL廢棄]後，將範本附加至專案。</p> <p>此選項不適用於等待核准的專案。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
