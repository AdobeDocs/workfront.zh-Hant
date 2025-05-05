---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 設定全系統的專案偏好設定
description: 作為 [!DNL Adobe Workfront] 管理員，您可以為在整個系統中建立的所有專案設定預設偏好設定。 這些偏好設定會影響專案、任務和問題行為。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 1a1affed-1b06-442c-98b2-9f360eee767b
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '2695'
ht-degree: 1%

---

# 設定整個系統的專案偏好設定

<!--Audited: 12/2023-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


作為[!DNL Adobe Workfront]管理員，您可以為在整個系統中建立的所有專案設定預設偏好設定。 這些偏好設定會影響專案、任務和問題行為。

>[!NOTE]
>
>依照預設，這些偏好設定會鎖定，群組管理員無法在群組層級修改它們，除非您為整個系統中的所有群組解除鎖定它們。 如需詳細資訊，請參閱[鎖定或解除鎖定系統中所有群組的專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] 計劃</p></td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td><p>新增：[!UICONTROL Standard]</p>
   或
   <p>目前： [!UICONTROL 計畫]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td>[!UICONTROL 系統管理員]</td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 設定整個組織的專案偏好設定

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**[!UICONTROL 專案偏好設定]** > **[!UICONTROL 專案]**。

1. 在&#x200B;**專案偏好設定**&#x200B;頁面上，繼續下列四個區段之一，設定[!UICONTROL 專案狀態]、[!UICONTROL 時間表]、[!UICONTROL 業務案例]及[!UICONTROL 死亡後期限]的偏好設定。
1. 如果您希望整個組織的所有群組都使用相同的專案偏好設定，請確定每個偏好設定都已鎖定![鎖定切換](assets/lock-toggle-button.png) （這是預設值）。

   >[!IMPORTANT]
   >
   >鎖定專案偏好設定時，對該偏好設定所做的任何變更都會被系統中的所有群組繼承。 務必與整個組織的使用者和群組溝通，以確保以您設定專案偏好設定的方式考慮到所有需求。

   如需解鎖喜好設定以便所有群組可以自行設定及管理的相關資訊，請參閱[鎖定或解鎖系統中所有群組的專案喜好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md)。

1. 按一下「**[!UICONTROL 儲存]**」。

* [[!UICONTROL 專案狀態]](#project-status)
* [[!UICONTROL 時間表]](#timelines)
* [[!UICONTROL 業務案例]](#business-cases)
* [[!UICONTROL 死亡後期限]](#life-after-death)

### 專案狀態 {#project-status}

為整個系統的新建立專案設定下列任一偏好設定：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 允許使用者在不使用範本的情況下建立專案]</td> 
   <td>  <p>此偏好設定可讓使用者在從下列區域建立專案時，無需使用範本即可建立專案： </p>
      <ul>
        <li>
        <p>在專案清單中使用[!UICONTROL 新增專案]選項</p>
        </li>
          <li>
          <p>從問題頁面將問題轉換為專案</p>
          </li>
         </ul>
        <p>此偏好設定預設為啟用。 </p> 
        <p><b>附註</b></p>
        <p> 群組管理員可以變更群組的此偏好設定。 當使用者屬於具有不同偏好設定的多個群組時，如果使用者的主群組已啟用此偏好設定，則使用者可以建立沒有範本的專案。</p> 
        </td> 
  </tr>
  <tr> 
   <td role="rowheader">[!UICONTROL 將新專案狀態設定為]</td> 
   <td> <p>決定新專案的狀態。</p>  <p><b>附註</b>  
     <ul> 
      <li>如果您或其他[!DNL Workfront]管理員隱藏此處選取的狀態，預設狀態會變更為狀態清單中的第一個狀態。</li> 
     </ul> 
     <ul> 
      <li> <p>如果鎖定的系統或群組狀態設定為預設狀態，稍後有人將其解鎖，則系統會嘗試以相同狀態型別的鎖定狀態來取代它。</p> <p>如果找不到，會尋找必要的狀態：</p> 
       <ul> 
        <li>如果必要的狀態等於已解除鎖定的預設狀態，則即使已解除鎖定，「必要」狀態也會變成預設狀態。</li> 
        <li>如果所有必要狀態都不等同於已解除鎖定的預設狀態，則狀態清單中的第一個必要狀態會成為預設狀態。</li> 
       </ul> <p>如需必要狀態的相關資訊，請參閱文章<a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">存取系統專案狀態清單</a>、<a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">存取系統任務狀態清單</a>，以及<a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">存取系統問題狀態清單</a>。</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 計算完成百分比依據]</td> 
   <td> <p>Workfront會使用專案中每個任務的完成百分比以及每個任務的期間或計畫時數，來計算專案或父任務的完成百分比。</p><p>每個任務的完成百分比由任務受指派人手動設定。</p><p>您可以在此處選擇Workfront將使用任務的持續時間或計畫時數來計算專案的完成百分比。</p> <p>如果您選取[!UICONTROL 工期]，專案中每個任務的「工期」會決定專案的整體完成百分比，而每個子任務的「工期」則會決定其父系任務的整體完成百分比。</p> <p>如果您選取[!UICONTROL Duration]，請務必在[!UICONTROL 時間表]區段中指定[!UICONTROL 每工作日一般小時數]和[!UICONTROL 每週一般工作日數]。 根據「持續時間」計算任務的完成百分比時，[!DNL Workfront]會使用此資訊。 </p> <p>如果您選取[!UICONTROL 計畫時數]，請確認每個專案上的所有任務已定義總計[!UICONTROL 計畫時數]，且該金額不是零。</p><p>如需詳細資訊，請參閱<a href="/help/quicksilver/manage-work/tasks/task-information/project-percent-complete.md">專案完成百分比總覽</a>。</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 根據進度狀態自動設定專案條件]</td> 
   <td> <p>此偏好設定可讓使用者手動將專案的[!UICONTROL Condition]設定為([!UICONTROL On Target]，[!UICONTROL At Risk]，[!UICONTROL In Trouble])，或讓[!DNL Workfront]根據專案在時間表上的進度自動設定[!UICONTROL Condition] （進度狀態）。 如需有關專案條件的詳細資訊，請參閱<a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">專案條件和條件型別概觀</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 自動建立基準線]</p> </td> 
   <td> <p>當專案狀態變更為[!UICONTROL 目前]時，此偏好設定會自動建立任務和專案詳細資訊的基準（快照）。 如需建立基準的相關資訊，請參閱<a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">建立專案基準</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 績效指數方法] </p> </td> 
   <td> <p>專案的績效指數方法(PIM)控制[!DNL Workfront]用來計算收益值量度的方法，例如[!UICONTROL 成本績效指數] (CPI)和[!UICONTROL 完工估算] (EAC)。 如需詳細資訊，請參閱<a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">計算[!UICONTROL 成本績效指數] (CPI)</a>和<a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL 計算完工估算] (EAC)</a></p> 
    <ul> 
     <li><strong>[!UICONTROL 小時型]</strong>： [!DNL Workfront]使用[!UICONTROL 計畫時數]來計算效能量度，例如EAC和CPI。 當根據時數計算PIM時，EAC會顯示為時數。 確保您有[!UICONTROL 計畫時數]的值，而不是零。</li> 
     <li> <p><strong>[!UICONTROL 基於成本]</strong>： [!DNL Workfront]使用[!UICONTROL 計畫勞力成本]來計算績效量度，例如EAC和CPI。 確保您的工作角色或使用者與每小時成本費率相關聯。 根據「成本」計算PIM時，EAC會顯示為貨幣值。</p> <p>專案經理可以使用[!UICONTROL 專案詳細資料]中的[!UICONTROL 財務]區域，在專案層級修改此設定。 如需詳細資訊，請參閱<a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">管理專案[!UICONTROL 財務]區域</a>中的資訊。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 完工估算]</p> </td> 
   <td> <p>決定[!DNL Workfront]使用哪些資料來計算代表專案預計總成本的[!UICONTROL 預估完成成本] (EAC)。</p> 
    <ul> 
     <li><strong>[!UICONTROL 在專案層級計算]</strong>：父系任務和專案的EAC是在EAC公式中輸入[!UICONTROL 實際時數]或[!UICONTROL 實際勞力成本]來決定。 此計算包括直接新增到父級任務或專案的[!UICONTROL 實際時數]或[!UICONTROL 成本和費用]。</li> 
     <li> <p><strong>[!UICONTROL 從任務/子任務彙總]</strong>：父任務和專案的EAC是由每個子任務的EAC總和所決定。 此計算不包括直接新增至父級任務或專案的[!UICONTROL 實際時數]或[!UICONTROL 實際成本和費用]。</p> <p>專案經理可以使用[!UICONTROL 專案詳細資料]中的[!UICONTROL 財務]區域，在專案層級修改此設定。如需詳細資訊，請參閱專案[!UICONTROL 財務]區域</a>中的<a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">管理資訊。</p> </li> 
    </ul> <p>如需EAC如何計算的詳細資訊，請參閱<a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">計算[!UICONTROL 完工估算] (EAC)</a>。</p> </td> 
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
   <td role="rowheader">[!UICONTROL 排程起始日期]</td> 
   <td> <p>決定新專案是從開始日期排程，還是從建立專案時的完成日期排程。</p> 
    <ul> 
     <li><strong>[!UICONTROL 開始日期]</strong>：新任務會儘快預設為任務限制，並且會提示專案經理提供專案的[!UICONTROL 計劃開始日期]。</li> 
     <li><strong>[!UICONTROL 完成日期]</strong>：新任務預設為[!UICONTROL 儘可能遲]任務限制，並且會提示專案經理提供專案的[!UICONTROL 規劃完成日期]。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 使用者休假]</td> 
   <td> <p>決定任務的主要受指派人的休假是否調整專案上該任務的計畫日期。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 考量使用者在任務持續期間內的休假]</strong>：如果休假發生在任務持續期間，則任務的主要受指派人排定的任何休假都會調整任務的計畫日期。 這是預設設定。 </p> <p>例如，如果限製為的任務排程在6月1日開始並在6月3日完成，而主要受指派人將6月2日標籤為休假，則任務的計畫日期將調整為6月1日至6月4日。</p> <p><b>重要</b>：</p> <p>當您選取此設定時，工作的持續時間不會變更。 根據任務限制，只有計畫日期會變更。</p> </li> 
     <li><strong>[!UICONTROL 忽略使用者在任務持續期間的休假]</strong>：專案上每個任務的計畫日期仍維持原計畫，即使任務的主要受指派人在其持續期間具有休假。</li> 
    </ul> <p>選取此設定的選項時，請考量下列事項：</p> 
    <ul> 
     <li>當您變更此設定時，只有變更後建立的專案和範本會繼承更新的設定。 </li> 
     <li> <p>任務的「任務限制」值決定要調整哪些計畫任務日期： </p> 
      <ul> 
       <li>計畫開始日期</li> 
       <li>計畫完成日期</li> 
       <li>兩個日期</li> 
       <li>兩者皆非。 </li> 
      </ul> <p>例如，如果任務的限製為[!UICONTROL 固定日期]，則即使選取了[!UICONTROL 考慮使用者在任務期間內的休息時間]選項，當主要受指派人具有休息時間時，日期也不會調整。 如需任務限制的相關資訊，請參閱<a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">任務限制總覽</a>。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 專案時間表會自動重新計算]</p> </td> 
   <td> <p>決定重新計算專案的時間表。 如需重新計算專案時間表的相關資訊，請參閱<a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">重新計算專案時間表</a>。</p> <p>預設會啟用下列選項。 您可以選取下列一或多個設定：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Every night]</strong>：選取此項可每晚重新計算專案時間表。 您對專案所做的任何可能影響時間表的變更都不會立即顯示。 [!DNL Workfront​​​]只會在符合下列兩個條件的專案在夜間重新計算時間表：</p> <p> 
       <ul> 
        <li>狀態為[!UICONTROL 目前]</li> 
        <li>在過去3個月內已更新</li> 
        <li>更新型別為下列其中一項：</li>
        <ul>
        <li>自動與專案變更時</li>
        <li>僅限變更</li>
        <li>僅限自動</li> 
      </ul>       
    <b>秘訣：</b>
    <p>此設定不會影響更新型別為「僅限手動」的專案。</p>
    <li> <p><strong>當專案範圍變更時</strong>：選取此專案可在專案範圍變更時立即重新計算專案時間表。 如需有關構成專案範圍變更的資訊，請參閱<a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">重新計算專案時間表</a>。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 將多位使用者指派到一個任務時，請使用]的排程</p> </td> 
   <td> <p>如果專案未指派排程，或指派給其任務的使用者未指派排程，[!DNL Workfront]會使用系統預設排程來計算任務的時間表。</p> <p>如果您將多位使用者指派至專案中的相同任務，且專案已指派排程，且指派至任務的使用者也已指派排程，則[!UICONTROL Workfront]會使用以下排程：</p> 
    <ul> 
     <li><strong>[!UICONTROL 主要指派]</strong>： [!DNL Workfront]使用任務上主要指派的排程來計算時間表。</li> 
     <li><strong>[!UICONTROL 專案]</strong>： [!DNL Workfront]會使用專案的排程來計算每項工作的時間表。</li> 
    </ul> <p>如需排程的詳細資訊，請參閱<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">建立排程</a>。</p> </td> 
  </tr>

</tr> 
  <tr> 
   <td role="rowheader"> <p>當一位使用者被指派一項任務時，請使用以下的排程…</p> </td> 
   <td> 
<p>如果專案未指派排程，或指派給其任務的使用者未指派排程，[!DNL Workfront]會使用系統預設排程來計算任務的時間表。</p>

<p>如果您指派一位使用者給專案中的任務，且指派給任務的專案和使用者都有與其關聯的排程，則[!UICONTROL Workfront]會使用以下排程：</p> 
    <ul> 
     <li><strong>[!UICONTROL 使用者]</strong>： [!DNL Workfront]使用工作上指派使用者的排程來計算時間表。</li> 
     <li><strong>[!UICONTROL 專案]</strong>： [!DNL Workfront]使用專案排程來計算任務的時間表。</li> 
    </ul> <p>如需排程的詳細資訊，請參閱<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">建立排程</a>。</p>
</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL 時間表計算] </p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Typical hours per work day]</strong>：針對將處理專案的使用者，設定一般工作日的小時數。 預設值為8小時。</li> 
    </ul> 
    <ul> 
     <li><strong>[!UICONTROL 每週一般工作天數]</strong>：為處理專案的使用者設定標準工作週。 預設值為5天。</li> 
    </ul> <p>這2個選項會將天數轉換為小時，或將周數轉換為天數。</p> <p>例如，如果您有具有8個計畫時數的任務，而持續時間是根據計畫時數計算的，則[!DNL Workfront]會將這些時數轉換為天數，以便將持續時間顯示為天。</p> <p>從一般[!UICONTROL 每週工作天數]欄位中，[!DNL Workfront]會計算您系統的完全時間當量(FTE)值。 這是[!DNL Workfront]在計算使用者的配置時使用的專案。</p> <p>當您計畫專案時間表、編列資源預算或針對專案記錄時間時，會使用這些值。 </p> <p>當您在系統中建立使用者的時程表時，不會使用這些時間表，如<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL 設定]時程表和小時偏好設定</a>中所述。</p> <p><b>附註</b>：</p> <p>[!DNL Workfront] 管理員無法解鎖[!UICONTROL 時間表計算]喜好設定。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL 自訂季度]</p> </td> 
   <td> <p>為將處理專案的使用者設定自訂每年季度。 自訂季度通常是不符合日曆年度中傳統季度劃分的季度。 您可以新增多個自訂季度。 如需詳細資訊，請參閱<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">啟用專案的自訂季度</a>。</p>  <p><b>附註</b>： </p><p>[!DNL Workfront] 管理員無法解鎖[!UICONTROL 自訂季度]喜好設定。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 業務案例] {#business-cases}

您可以為整個系統的新建立專案建立業務案例，以提交專案請求。 您可以定義偏好設定來決定可在&#x200B;**[!UICONTROL 業務案例]**&#x200B;表單上看到的區域。 建議您啟用這些選項，以便其他工具(例如[!UICONTROL Portfolio最佳化工具])能夠正確更新。 如需每個欄位顯示內容的詳細資訊，請參閱[定義業務案例：文章索引](../../../manage-work/projects/define-a-business-case/define-business-case.md)。

在[!DNL Workfront]管理員啟用[!UICONTROL 業務案例]的區段後，專案所有者便可以在專案層級建立業務案例。 如需建立業務案例的相關資訊，請參閱[為專案建立業務案例](../../../manage-work/projects/define-a-business-case/create-business-case.md)。

### [!UICONTROL 死亡後期限] {#life-after-death}

為整個系統的新建立專案設定下列任一偏好設定：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 將專案標籤為完成之後，人員仍可] </p> </td> 
   <td> <p>決定您的組織（或群組，如果您是設定群組的專案偏好設定）的規則，這些規則有關於在專案狀態標籤為[!UICONTROL 完成]後是否可以刪除任務或問題。</p> 
    <ul> 
     <li><strong>[!UICONTROL 刪除任務]</strong>：允許使用者在專案標籤為[!UICONTROL 完成]之後，從專案中刪除任務。<br></li> 
     <li><strong>[!UICONTROL 刪除問題]</strong>：允許使用者在專案標籤為[!UICONTROL 完成]之後，從專案刪除問題。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 將專案標籤為「完成」、「廢棄」或「未決核准」之後，人員仍可]</p> </td> 
   <td> <p>決定組織（或群組，如果您正在設定群組的專案偏好設定）的規則，這些規則有關於專案狀態標籤為<strong>[!UICONTROL 完成]</strong>、<strong>[!UICONTROL 廢棄]</strong>或是<strong>[!UICONTROL 未決核准]</strong>後，專案中任務、問題、檔案和其他物件會發生什麼情況。</p> 
    <ul> 
     <li><strong>[!UICONTROL 新增及編輯工作：]</strong>允許使用者：
      <ul>
       <li><p>在專案標籤為[!UICONTROL 完成]、[!UICONTROL 已廢棄]或為[!UICONTROL 未決核准]之後，編輯專案中的任務。</p>
           <p>備註：即使未選取此選項，使用者也可以新增及編輯費用專案。 記錄時數有單獨的設定。 若要允許或防止使用者在狀態為「完成」或「無法使用」的專案上記錄時間，請參閱<a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">設定時程表和小時偏好設定</a>。</p></li>
       <li>將任務新增至專案。</li>
      </ul></li>
     <li><strong>[!UICONTROL 新增和編輯問題]</strong>：允許使用者：
      <ul>
       <li>在專案標籤為[!UICONTROL 完成]、[!UICONTROL 廢棄]或[!UICONTROL 未決核准]之後，編輯專案中的問題。</li>
       <li>在專案標籤為[!UICONTROL 完成]或[!UICONTROL 已廢棄]後，將問題新增至專案。 （您無法將「[!UICONTROL 未決核准]」問題新增至專案。）</li>
      </ul></li> 
     <li> <p><strong>[!UICONTROL 將檔案新增至專案及其任務和問題]</strong>：允許使用者在專案標籤為[!UICONTROL 完成]或[!UICONTROL 已廢棄]後，將檔案新增至專案（或將檔案新增至專案內的任務和問題）。</p> <p>此選項不適用於等待核准的專案。</p> </li> 
     <li> <p><strong>[!UICONTROL 附加範本]</strong>：允許使用者在專案標籤為[!UICONTROL 完成]或[!UICONTROL 已廢棄]之後，將範本附加至專案。</p> <p>此選項不適用於等待核准的專案。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
