---
product-area: projects
navigation-topic: manage-tasks
title: 在「任務詳細資訊概覽」區域中管理任務資訊
description: 在「任務詳細資訊概覽」區域中管理任務資訊
author: Alina
feature: Work Management
exl-id: 4980b28f-914d-4cf9-813f-14983aac660b
source-git-commit: 7e591a8eb801da463f05b574c091f68278974ad7
workflow-type: tm+mt
source-wordcount: '2072'
ht-degree: 5%

---

# 在「任務詳細資訊概覽」區域中管理任務資訊

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some of the information (fields) in this article is also in the Edit tasks article; if you need to update one field, do it in both articles)</p>
-->

通過訪問「任務詳細資訊」部分的「概述」區域，可以查看或編輯任務的資訊。 在此區域中可查看或編輯的欄位數量有限。 有關編輯任務的所有資訊的資訊，請參閱 [編輯任務](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

本文介紹如何在「任務詳細資訊」的「概述」區域中查看或編輯資訊。 有關更新「任務詳細資訊」的其他區域的資訊，請參閱以下文章：

* [在「任務詳細資訊」部分中管理任務財務](../../../manage-work/tasks/manage-tasks/task-finances-in-details.md)
* [將自訂表單新增至物件](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)
* [管理附加到對象的自定義表單](../../../workfront-basics/work-with-custom-forms/manage-custom-forms-attached-to-objects.md)

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <caption style="text-align: left;">
   *若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。 
 </caption> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront<b> 計畫*</b> </p> </td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront<b> 授權*</b> </p> </td> 
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>訪問級別配置*</strong> </td> 
   <td> <p>查看或更高程度地訪問項目和任務</p> <p>如果您有正確的存取層級，但仍無法編輯工作的「詳細資訊」區段，請詢問您的Adobe Workfront是否在您的存取層級設定了其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>物件權限</strong> </p> </td> 
   <td> <p>為專案貢獻或更高權限</p> <p>檢視任務的權限，以在「詳細資訊」區段中檢視資訊。 </p> <p>管理任務的權限以更新詳細資訊區段中的資訊。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 在「任務詳細資訊概述」部分中編輯任務資訊

1. 轉到要查看或編輯的任務。
1. 按一下 **任務詳細資訊** 中。
1. 前往 **概述** 區域，查看有關任務的詳細資訊。

   預設情況下，「概述」是「任務詳細資訊」部分的第一個區域，並且展開。

   >[!NOTE]
   >
   >視您的Workfront管理員或群組管理員設定「配置範本」的方式而定，「任務詳細資料」區段中的欄位可能會重新排列或未顯示。 如需詳細資訊，請參閱 [使用版面範本自訂「詳細資料」檢視](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. 按一下 **編輯** 圖示 ![](assets/edit-icon.png) 在「詳細資料」區段的右上角，按一下 **概述**.

   >[!TIP]
   >
   >您無法編輯由Workfront自動產生或您沒有編輯權限的欄位。

1. 按一下欄位或按一下，編輯任何可供編輯的欄位 **+添加** 將資訊添加到空欄位。
1. 查看或編輯列出的以下任何欄位。

   並非所有欄位都可編輯。  

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">說明</td> 
      <td> <p>有關任務的其他資訊</p> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">參考號碼</td> 
      <td>這是Workfront為系統中所有對象生成的任務的唯一值。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>具有任務管理權限的用戶可以在此欄位中指定指向內部或外部頁面的連結。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">狀態</td> 
      <td> <p>選擇任務的狀態，該狀態指示任務所處的開發階段。</p> <p>提示：您可以更新任務題頭中的任務狀態。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">優先順序</td> 
      <td> <p>這是視覺標幟，可讓您排定工作的優先順序。 </p> <p>從下列選項中選取： </p> 
       <ul> 
        <li> <p> 無</p> </li> 
        <li> <p> 低 </p> </li> 
        <li> <p>標準 </p> </li> 
        <li> <p>高 </p> </li> 
        <li> <p> 緊急 </p> </li> 
       </ul> <p>視您的Workfront管理員選取的「專案偏好設定」而定，優先順序的名稱可能會有所不同。 有關任務優先順序的資訊，請參見 <a href="../../../manage-work/tasks/task-information/task-priority.md" class="MCXref xref">更新任務優先順序</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">期間類型</td> 
      <td> <p>這可識別下列項目之間的關係： </p> 
       <ul> 
        <li> <p>分配給任務的資源數 </p> </li> 
        <li> <p>完成任務所需的總工作量 </p> </li> 
        <li> <p> 任務的總持續時間。 </p> </li> 
       </ul> <p>您的Workfront管理員 <span> 或組管理員</span> 選擇系統或組中任務的預設「持續時間類型」設定。 有關設定項目預設值的資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">配置系統範圍的項目首選項</a>. </p> <p>持續時間類型使您能夠根據任務的需要設定一致的資源分配。 有關任務的「持續時間類型」的詳細資訊，請參閱 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任務持續時間和持續時間類型概覽</a>. </p> <p>從下列選項中選取： </p> 
       <ul> 
        <li> <p>已計算的任務指派 </p> </li> 
        <li> <p> 已計算的工作 </p> </li> 
        <li> <p>投入比導向 </p> </li> 
        <li> <p>簡單</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">期間</td> 
      <td> 
       <div> 
        <div> 
         <p>這是您允許任務在完成之前保持開啟的時間。 </p> 
         <p>重要：由於任務持續時間通常是計劃開始日期和計畫完成日期之間的時間量，因此會影響項目的時間軸。</p> 
         <p>要指示任務的持續時間和時間單位，請執行以下操作：</p> 
         <ul> 
          <li> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">輸入時間長度，然後從下拉式功能表中可用的時間單位中選取。</p> </li> </ul>

   <p><strong>筆尖</strong></p> <p> 在任務清單中更新任務的持續時間時，可以使用時間單位的縮寫。 </p>      <p> 您可以從下表中的一般時間或經過的時間選項中進行選擇： </p> 
         <table style="table-layout:auto"> 
          <col> 
          <col data-mc-conditions=""> 
          <tbody> 
           <tr> 
            <td>單位</td> 
            <td>縮寫</td> 
           </tr> 
           <tr> 
            <td>分鐘</td> 
            <td>一</td> 
           </tr> 
           <tr> 
            <td>時數</td> 
            <td>H</td> 
           </tr> 
           <tr> 
            <td>天. 這是預設值。 </td> 
            <td>D</td> 
           </tr> 
           <tr> 
            <td>週</td> 
            <td>三</td> 
           </tr> 
           <tr> 
            <td>月</td> 
            <td>二</td> 
           </tr> 
           <tr> 
            <td>經過的分鐘數</td> 
            <td>EM</td> 
           </tr> 
           <tr> 
            <td>經過的時數</td> 
            <td>EH</td> 
           </tr> 
           <tr> 
            <td>經過的天數</td> 
            <td>ED</td> 
           </tr> 
           <tr> 
            <td>經過的週數</td> 
            <td>EW</td> 
           </tr> 
           <tr> 
            <td>經過的月數</td> 
            <td>ET</td> 
           </tr> 
          </tbody> 
         </table> 
         <p><strong>附註</strong> </p>
         <p> 已用時間是任務持續時間的單位。 它是任務（包括節假日、週末和休假時間）的「計畫起始日期」和「計畫完成日期」之間的時間。 換句話說，經過的時間是日曆天數的過去。 常規時間會考慮節假日、週末和休假時間，並將它們從任務的「持續時間」中排除。 有關任務持續時間的詳細資訊，請參閱 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任務持續時間和持續時間類型概覽</a>. </p> 
         <p> 
         <!--You cannot specify the Duration of a task when the Duration Type of the task is Simple, or when the Task Constraint is Fixed Dates. (NOTE: Anna said this is now possible for all duration types in the Assignments area. It's not here, but to clear confusion, I am drafting this out of here.)--></p> 
        </div> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">預計持續時間</td> 
      <td> <p>預計起始日期和預計完成日期之間的天數差。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">實際持續時間</td> 
      <td> <p>實際開始日期與實際完成日期之間的天數差。 這是完成這項工作所花的時間。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">計畫小時數</td> 
      <td> <p>指定任務的計畫小時數（以小時為單位）。 這是任務的受分配者完成任務所需的實際時間。 當「期間類型」設定為「計算分配」時，您只能指定任務的計畫小時數。 如需持續時間類型的詳細資訊，請參閱 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任務持續時間和持續時間類型概覽</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">實際工作</td> 
      <td>用戶在任務上記錄的小時數。 </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">工作量 </td> 
      <td> 
       <div> 
        <p>完成任務所需的工作量。 您的項目經理可能會決定使用此欄位，而不是「計畫小時」來估計完成任務所需的工作量。 只有在符合下列條件時，此欄位才會顯示：</p> 
        <ul> 
         <li> <p>該任務具有「簡單持續時間類型」。 </p> <p>提示：如果更改任務「持續時間類型」，則此欄位將變灰。 </p> </li> 
         <li>您的項目經理啟用了「使用工作量」欄位，以自動計算項目上的任務計畫小時數。 </li> 
        </ul> 
        <p>從下列選項中選取：</p> 
        <ul> 
         <li>小</li> 
         <li>中 <span style="font-weight: normal;">（這是新任務的預設值）</span></li> 
         <li>大</li> 
        </ul> 
        <p><strong>附註</strong></p> 
        <p> 更新工作量可以更新任務「計畫小時數」。 如果項目「更新類型」為「自動」，則更新為立即更新。 當項目更新類型為「人工」時，必須重新計算時間軸，才能查看更新的計畫小時數。 </p> 
        <p>有關使用工作量（而非計畫小時）來估計任務工作量的資訊，請參閱 <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">工作成果概觀</a>. </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">任務限制</td> 
      <td> <p>通過指定任務約束來決定何時必須完成任務。 </p> <p>從下列選項中選取： </p> 
       <ul> 
        <li> <p><span>固定日期</span> </p> <p>指定 <strong>計劃開始</strong> 和 <strong>計畫完成日期</strong>. </p> </li> 
        <li> <p><span>必須開始時間</span> </p> <p>指定 <strong>計劃開始日期</strong>. </p> </li> 
        <li> <p><span>必須完成時間</span> </p> <p>指定 <strong>計畫完成日期</strong>. </p> </li> 
       </ul> 
       <ul> 
        <li> <p><span>盡快</span></p> </li> 
        <li> <p><span>盡可能晚</span></p> </li> 
        <li> <p><span>最早可用時間</span></p> </li> 
        <li> <p> <span>最晚可用時間</span></p> </li> 
        <li> <p><span>開始時間不晚於</span> </p> </li> 
        <li> <p>指定計劃開始日期</p> </li> 
        <li> <p><span>開始時間不早於</span> </p> <p>指定 <strong>計劃開始日期</strong>. </p> </li> 
        <li> <p> 完成 <span>不遲於</span></p> <p>指定 <strong>計畫完成日期</strong>. </p> </li> 
        <li> <p> 完成 <span>早於</span></p> <p>指定 <strong>計畫完成日期</strong></p> </li> 
       </ul> <p>有關「任務約束」的詳細資訊，請參閱 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">任務約束概覽</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">計畫開始日期</td> 
      <td> <p>計劃開始任務時。 任務的計畫起始日期是設定的，並受多種因素的影響：</p> 
       <ul> 
        <li>根據任務計劃開始日期的全系統首選項，預設情況下，項目上新任務的開始日期可以是今天，也可以是項目的開始日期。 <span>與項目關聯的組的組管理員也可以為組設定此首選項。</span> 有關係統級或組級任務首選項的詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">配置全系統任務和問題首選項</a>.</li> 
        <li>根據任務的前置任務，Workfront將選擇計畫起始日期作為前置任務完成後的下一個可用日期，或根據前置任務關係開始。 如需先前關係的詳細資訊，請參閱 <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">任務前置任務概述</a>.</li> 
        <li>當任務約束為「固定日期」或「必須開始」時，項目經理或任務責任人可以人工設定計畫起始日期。 有關任務約束的詳細資訊，請參閱 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">任務約束概覽</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">預計開始日期</td> 
      <td> <p>根據以前任務的進度和完成開始任務的「實際」日期。 這是計算欄位，您無法手動編輯。</p> <p> 最初計畫項目時，預計起始日期和計畫起始日期的起始日期相同。 如果項目演化且任務尚未開始，則預計的開始日期可能會從計畫的開始日期移開。 如需預計開始日期的詳細資訊，請參閱 <a href="../../../manage-work/projects/planning-a-project/project-projected-start-date.md" class="MCXref xref">項目預計起始日期概覽</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">實際開始日期</td> 
      <td> <p>指定任務的實際起始日期。 當您將任務的狀態更改為「正在進行」時，通常會自動填入預設值。 項目經理或任務責任人也可以人工修改實際起始日期。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">計畫完成日期</td> 
      <td> <p>計畫任務時顯示的預計完成日期。 計畫完成日期可以由多種因素設定：</p> 
       <ul> 
        <li>計畫完成日期從計畫起始日期計算，方法是將任務的持續時間添加到計畫起始日期。 當項目經理或Workfront指定任務的持續時間時，將觸發對計畫完成日期的更新。 如果計畫日期變更，通常是因為的持續時間已更新。</li> 
        <li>當任務約束為「固定日期」或「必須完成」時，項目經理或任務責任人可以人工設定計畫完成日期。 有關任務約束的詳細資訊，請參閱 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">任務約束概覽</a>.</li> 
        <li>如果任務的「持續時間類型」更改，且任務上的資源數同時更改，則計畫完成日期也會更改。 如需持續時間類型的詳細資訊，請參閱 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任務持續時間和持續時間類型概覽</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">預計完成日期</td> 
      <td> <p>根據先前任務的進度和受讓人對任務進行的進度更新，將完成任務的「實際」日期。 這是計算欄位，您無法手動編輯。</p> <p> 預計完成日期和計畫完成日期的起始時間與最初計畫項目時相同。 如果項目發展，並且任務尚未啟動，則預計完成日期可能會從計畫完成日期移開。 有關預計完成日期的詳細資訊，請參閱 <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">項目、任務和問題的預計完成日期概覽</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">實際完成日期</td> 
      <td> <p>指定任務完成時的實際日期和時間。 任務完成時的預設日期和時間始終與狀態變為「完成」時的實際時間一致。 項目經理或任務責任人也可以人工修改實際完成日期。 </p> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">認可日期</td> 
      <td> <p>這是分配給任務的用戶提交完成任務的日期。 這可以與計畫完成日期不同。 僅受指派人可以編輯此欄位。如需Workfront中提交日期的相關資訊，請參閱 <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">提交日期概述</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">輸入日期</td> 
      <td>建立任務的日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">輸入者</td> 
      <td>建立任務的人員。</td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">上次更新日期</td> 
      <td> <p>上次更新任務的日期。 </p> <p>提示：Workfront會在每次有人編輯並儲存任務時記錄「更新日期」。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">上次更新者</td> 
      <td> <p>上次更新任務的人員。</p> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">週期頻率</td> 
      <td> <p>這只會顯示在循環工作的上層。 這是重複執行中的任務發生的頻率。 有關建立循環任務的資訊，請參閱 <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">建立循環任務</a>. </p> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">各事件的持續時間</td> 
      <td> <p>這只會顯示在循環工作的上層。 它顯示每個循環任務的持續時間。 有關建立循環任務的資訊，請參閱 <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">建立循環任務</a>. </p> <p><strong>附註</strong></p> <p> 在個別循環任務中修改的持續時間不會顯示此欄位中指出的值。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted, to keep it focused JUST on the Overview section and not others.) </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Custom Forms</strong> to add or forms or edit information on the existing custom forms.&nbsp;</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Expand any of the existing custom forms to edit them, or start typing in the <strong>Add custom form</strong> box in the upper-right corner to add a new form. </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about adding or editing custom forms, see the following articles:</p>
   -->

   <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md" class="MCXref xref">Add a custom form to an object</a> </li>   
     -->

   <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="../../../workfront-basics/work-with-custom-forms/manage-custom-forms-attached-to-objects.md" class="MCXref xref">Manage custom forms attached to objects</a> </li>   
     -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click&nbsp;<strong>Finance</strong>, then <strong>Edit Finance</strong> to view or edit financial information for the task. </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Expand the <strong>Finance</strong> area in the Details section, then double-click any editable field to update it. </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about editing financial information for a task, see <a href="../../../manage-work/tasks/manage-tasks/task-finances-in-details.md" class="MCXref xref">Manage task finances in the Task Details section</a>. </p>
   -->

1. 按一下 **儲存變更**.
