---
product-area: projects
navigation-topic: manage-tasks
title: 編輯任務
description: 您可以編輯已建立或您擁有Contribute或「管理」許可權之工作的相關資訊。
author: Alina
feature: Work Management, Tasks
role: User
exl-id: 572c6008-3a67-47ae-8f5d-6b871ef1f37b
source-git-commit: 34b1bf4e776a1f5b4a413ab9f78bed63c4b64f45
workflow-type: tm+mt
source-wordcount: '3727'
ht-degree: 3%

---

# 編輯任務

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: some information in this area is repeated in the following articles. If you need to update a fied, update it in both:</p>
<p>** Task finances in details</p>
<p>** Task information in overview)</p>
</div>
-->


您可以編輯已建立或您擁有Contribute或「管理」許可權之工作的相關資訊。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級*</td> 
   <td> <p>編輯任務與專案的存取權</p> <p><b>附註</b>

如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需有關Workfront管理員如何變更您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> 
    <ul> 
     <li> <p>貢獻許可權給任務，以編輯任務詳細資訊區域中的下列資訊： </p>
     <ul>
     <li>說明</li>
     <li>狀態</li>
     </ul>  
      </li> 
     <li> <p>管理任務的許可權，以編輯詳細資訊區域和編輯任務方塊中的所有資訊</p> </li> 
    </ul> 
    <ul> 
     <li> <p>貢獻專案或更高的許可權</p> </li> 
    </ul> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 編輯任務的限制

有一些限制可能會阻止您編輯任務。

編輯任務時，請考量下列事項：

* 更新任務會觸發狀態為「目前」的專案通知。 為避免指派給任務的使用者感到困惑，請在專案處於「目前」狀態時，儘可能限制編輯任務。
* 您無法編輯核准流程中的任務。 您只能記錄時間或更新核准程式中任務的狀態。

  ![](assets/edit-task-in-approval-process-nwe-350x148.png)

* 只有當Workfront管理員或群組管理員在專案偏好設定區域中啟用此功能時，您才能編輯檔案，並將其新增到專案上狀態為「完成」、「廢棄」或「未決核准」的任務中。 如需關於設定專案偏好設定的資訊，請參閱 [設定全系統專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* 當專案被標籤為「完成」、「廢棄」或處於「核准程式」中時，您可以隨時編輯任務的下列資訊：

   * 記錄時間
   * 編輯現有費用
   * 附加自訂表單

* 其他使用者必須先重新整理頁面，才能檢視您對任務所做的更新。

## 編輯清單中的任務

您可以透過內聯編輯清單檢視中顯示的欄位，編輯任務清單中的任務資訊。

如需有關編輯清單中工作的資訊，請參閱 [編輯清單中的任務](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

## 使用「摘要」編輯清單中的任務

您可以使用「摘要」面板編輯清單中的任務。 如需有關在「摘要」面板中編輯任務的資訊，請參閱 [編輯清單中的任務](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md) 文章。

## 在「編輯任務」方塊中編輯任務

您可以使用「編輯任務」或「任務詳細資訊」區域編輯任務。 下列步驟說明如何在「編輯任務」方塊中編輯任務。

1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 按一下 **專案**，然後按一下專案名稱以開啟。
1. 按一下 **任務** 在左側面板中。
1. 按一下您要編輯的工作。
1. （視條件而定）若要編輯任務的有限資訊，請按一下 **任務詳細資訊** 在左側面板中。

   ![](assets/nwe-task-details-expanded-350x273.png)

   請考慮編輯「工作詳細資訊」段落中下列區域的資訊：

   * **概觀**

     此區域預設為展開。

   * **自訂表單**

     只有當物件附有自訂表單時，才會顯示自訂表單的名稱。

   * **財務**

   >[!NOTE]
   >
   >視您的Workfront管理員或群組管理員修改版面配置範本的方式而定，可能會重新排列或不顯示任務詳細資訊區域中的欄位。 如需詳細資訊，請參閱 [使用版面配置範本自訂詳細資料檢視](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   如需「任務詳細資訊」區段中可見欄位的相關資訊，請繼續編輯「編輯任務」方塊中的任務，如下所述。

   若要編輯「詳細資訊」段落中的資訊，請執行下列動作：

   1. （可選）按一下 **全部收合** 圖示 ![](assets/collapse-all-icon.png) 以收合所有區域。
   1. （選擇性和條件性）收合區域時，按一下 **向右鍵** ![](assets/right-pointing-arrow.png) 展開每個區域旁的要編輯區域。
   1. 如需在「工作詳細資訊」標籤中編輯資訊的詳細資訊，請參閱下列文章：

      * [在任務詳細資訊總覽區域中管理任務資訊](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md)
      * [在任務詳細資訊區段中管理任務財務](../../../manage-work/tasks/manage-tasks/task-finances-in-details.md)

   1. （可選）如果沒有附加到工作的自訂表格，請開始在 **新增自訂表格** 欄位，然後在清單中顯示時選取它，然後按一下 **儲存變更**.
   1. （可選）按一下 **匯出** 圖示 ![](assets/export.png) 若要將概述和自訂表單資訊匯出至PDF檔案，請按一下 **匯出**. 從下列選項中選取：

      * 全選（至少附加一個自訂表單時顯示）
      * 概觀
      * 一或多個自訂表單的名稱

      PDF檔案會下載到您的電腦。

      ![](assets/export-issue-details-selection-box-with-export-button-350x418.png)

      如需詳細資訊，請參閱 [匯出自訂表單和物件詳細資料](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

1. （視條件而定）若要編輯關於任務的所有資訊，請以具有任務管理許可權的使用者身分，按一下 **更多** 功能表 ![](assets/more-icon.png) 在任務名稱旁，然後按一下 **編輯**.

   或

   從工作清單中，選取工作，然後按一下 **編輯** 圖示 ![](assets/edit-icon.png) 在清單頂端。

   「編輯任務」方塊開啟。

   >[!IMPORTANT]
   >
   >您必須有任務的管理許可權才能看到編輯選項。

   所有工作列位都可在「編輯任務」方塊中使用，並按左側面板中列出的區域分組。

   >[!NOTE]
   >
   >視您的Workfront管理員或群組管理員修改版面配置範本的方式而定，可能會重新排列或不顯示任務詳細資訊區域中的欄位。 如需詳細資訊，請參閱 [使用版面配置範本自訂詳細資料檢視](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   請考慮在下列任何一節中指定資訊：

   * [任務名稱](#task-name)
   * [概觀](#overview)
   * [指派](#assignments)
   * [自訂表單](#Custom%C2%A0F)
   * [財務](#finance)
   * [設定](#settings)

   >[!NOTE]
   >
   >視您的Workfront管理員或群組管理員設定版面配置範本的方式而定，編輯任務方塊中的欄位可能會重新排列或不顯示。 如需詳細資訊，請參閱 [使用版面配置範本自訂詳細資料檢視](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

### 任務名稱 {#task-name}

1. 如上所述開始編輯您的工作。
1. 按一下 **任務名稱** 在左側面板中。

   ![](assets/nwe-task-name-section-edit-task-box-350x122.png)

1. 更新工作的名稱。

1. 按一下 **儲存** 或繼續下列章節。

### 概觀 {#overview}

1. 如上所述開始編輯您的工作。
1. 按一下 **概觀** 在左側面板中。

   ![](assets/nwe-overview-section-edit-task-box-350x257.png)

1. 更新下列有關工作的資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">說明</td> 
      <td>新增關於工作的其他資訊。 </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader"><span style="font-weight: bold;">基本資訊區段</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">狀態</td> 
      <td> <p>選取任務的狀態，以指出任務處於哪個開發階段。</p> <p><b>秘訣</b>

   您可以在任務標題中更新任務狀態。 </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">優先順序</td> 
      <td> <p>這是視覺化標幟，可讓您排定工作的優先順序。 </p> <p>從下列選項中選取： </p> 
       <ul> 
      <li> <p> 無</p> </li> 
      <li> <p> 低 </p> </li> 
      <li> <p>標準 </p> </li> 
      <li> <p>高 </p> </li> 
      <li> <p> 緊急 </p> </li> 
       </ul> <p>根據Workfront管理員選取的專案偏好設定，您的優先順序名稱可能會不同。 如需有關工作優先順序的資訊，請參閱 <a href="../../../manage-work/tasks/task-information/task-priority.md" class="MCXref xref">更新任務優先順序</a>. </p> </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader"><span style="font-weight: bold;">任務日期和限制區段</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">任務限制</td> 
      <td> <p>透過指定工作限制來決定必須完成工作的時間。 </p> <p>從下列選項中選取： </p> 
       <ul> 
      <li> <p><span>固定日期</span> </p> <p>指定 <strong>計劃開始</strong> 和 <strong>計畫完成日期</strong>. </p> </li> 
      <li> <p><span>必須開始於</span> </p> <p>指定 <strong>計劃開始日期</strong>. </p> </li> 
      <li> <p><span>必須完成時間</span> </p> <p>指定 <strong>計畫完成日期</strong>. </p> </li> 
       </ul> 
       <ul> 
      <li> <p><span>儘快</span></p> </li> 
      <li> <p><span>儘可能遲</span></p> </li> 
      <li> <p><span>最早可用時間</span></p> </li> 
      <li> <p> <span>最新可用時間</span></p> </li> 
      <li> <p><span>開始時間不晚於</span> </p> </li> 
      <li> <p>指定計劃開始日期</p> </li> 
      <li> <p><span>開始時間不早於</span> </p> <p>指定 <strong>計劃開始日期</strong>. </p> </li> 
      <li> <p> 完成 <span>不晚於</span></p> <p>指定 <strong>計畫完成日期</strong>. </p> </li> 
      <li> <p> 完成 <span>不早於</span></p> <p>指定 <strong>計畫完成日期</strong></p> </li> 
       </ul> <p>有關任務限制的詳細資訊，請參閱 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">任務限制總覽</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">認可日期和時間</td> 
      <td> <p>這是指派給任務的使用者認可完成任務的日期。 這可能與計畫完成日期不同。 僅受指派人可以編輯此欄位。 如需Workfront中認可日期的相關資訊，請參閱 <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">認可日期總覽</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">計劃開始日期和時間</td> 
      <td> <p>任務計劃開始的時間。 任務的計劃開始日期已設定且受許多因素影響：</p> 
       <ul> 
      <li>根據系統內任務計劃開始日期的偏好設定，專案上新任務的開始日期可以是今天，或是預設的專案開始日期。 <span>與專案相關之群組的群組管理員也可以為群組設定此偏好設定。</span> 如需有關系統層級或群組層級工作偏好設定的詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">設定系統範圍的任務和問題偏好設定</a>.</li> 
      <li>根據任務的前置任務，Workfront會選擇計劃開始日期作為前置任務完成後下一個可用日期，或開始日期（取決於前置任務關係）。 如需前置任務關係的詳細資訊，請參閱 <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">前置任務概觀</a>.</li> 
      <li>當任務限製為「固定日期」或「必須開始日期」時，專案經理或任務擁有者可以手動設定計劃開始日期。 如需有關任務限制的詳細資訊，請參閱 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">任務限制總覽</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">計畫完成日期和時間</td> 
      <td> <p>計畫的任務時顯示的預計完成日期。 計畫完成日期可由許多因素設定：</p> 
       <ul> 
      <li>從計劃開始日期通過將任務的期間新增到計劃開始日期來計算計畫完成日期。 當專案經理或Workfront指定任務的期間時，這會觸發計畫完成日期的更新。 如果計畫日期變更，通常是因為期間已更新。</li> 
      <li>當任務限製為「固定日期」或「必須完成日期」時，專案經理或任務擁有者可以手動設定計畫完成日期。 如需有關任務限制的詳細資訊，請參閱 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">任務限制總覽</a>.</li> 
      <li>如果任務的期間型別變更，並且任務上的資源數量同時變更，則計畫完成日期也會變更。 如需持續時間型別的詳細資訊，請參閱 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任務期間與期間型別概觀</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">實際開始日期和時間</td> 
      <td> <p>指定作業的實際開始日期。 當您將任務的狀態變更為進行中時，通常會自動填入預設值。 專案經理或任務擁有者也可以手動修改實際開始日期。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">實際完成日期和時間</td> 
      <td> <p>指定任務完成時的實際日期和時間。 任務完成的預設日期與時間一律與狀態變為「已完成」的實際時間一致。 專案經理或任務擁有者也可以手動修改實際完成日期。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><b>「工作時間」區段</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">工作投入 </td> 
      <td>

   <p>完成任務所需的工時量。 您的專案經理可能會決定使用此欄位而不是計畫時數來預估完成任務所需的工作。 只有在符合下列條件時，才會顯示此欄位：</p> 
      <ul> 
      <li> <p>任務具有簡單期間型別。 </p> <p><b>秘訣</b>

   如果您變更任務期間型別，此欄位會變暗。 </p> </li>
   <li>您的專案經理已啟用使用工作量以自動計算專案上的任務計畫時數欄位。 </li> 
      </ul> 
      <p>從下列選項中選取：</p> 
      <ul> 
      <li>小</li> 
      <li>Medium <span style="font-weight: normal;">（這是新任務的預設值）</span></li> 
      <li>大</li> 
      </ul> 
      <p><b>附註</b>

   更新工作量可能會更新任務計畫時數。 如果專案的「更新型別」為「自動」，則立即進行更新。 當專案更新型別是手動時，您必須重新計算時間表以檢視更新的計畫時數。 </p>

   <p>如需有關使用工作量而非計畫時數來估計任務工作的資訊，請參閱 <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">工作投入概觀</a>. </p> 
    </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **儲存** 或繼續下列章節。

### 指派 {#assignments}

1. 如上所述開始編輯您的工作。
1. 按一下 **指定任務** 在左側面板中。

   ![](assets/nwe-assignments-section-edit-task-box-350x217.png)

1. 按一下 **搜尋人員、角色和團隊** 並開始輸入您要指派給任務的使用者、角色或團隊名稱，然後按一下它，或當它顯示在清單上時按下Enter鍵。

   >[!NOTE]
   >
   >如果使用者名稱包含特殊字元，您必須在搜尋欄位中包含特殊字元。

   >[!TIP]
   >
   >您可以指派多個使用者、工作角色或團隊。 您只能指派作用中的使用者、工作角色和團隊。
   >
   >如果使用者、工作角色或團隊在停用之前已被指派，則他們仍被指派給工作專案。 在此情況下，我們建議採取下列步驟：
   >
   >* 將工作專案重新指派給作用中的資源。
   >* 將已停用團隊中的使用者與作用中團隊建立關聯，並將工作專案重新指派給作用中團隊。

1. （選擇性）藉由選取 **所有者** 名稱旁的單選按鈕。 團隊不能是任務的主要受指派人。
1. （條件式與選用式）更新下列欄位：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">期間類型</td> 
      <td> <p>這會識別下列專案之間的關係： </p> 
       <ul> 
      <li> <p>指派給任務的資源數 </p> </li> 
      <li> <p>完成任務所需的總工作量 </p> </li> 
      <li> <p> 任務的總持續時間。 </p> </li> 
       </ul> <p>您的Workfront管理員 <span> 或群組管理員</span> 選取系統或群組中工作的預設「期間型別」設定。 如需有關設定專案預設值的資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">設定全系統專案偏好設定</a>. </p> <p>期間型別可讓您根據作業的需求設定一致的資源指定。 如需有關任務期間型別的詳細資訊，請參閱 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任務期間與期間型別概觀</a>. </p> <p>從下列選項中選取： </p> 
       <ul> 
      <li> <p>已計算的任務指派 </p> </li> 
      <li> <p> 已計算的工作 </p> </li> 
      <li> <p>投入比導向 </p> </li> 
      <li> <p>簡單</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">各事件的持續時間</td> 
      <td> <p>這僅顯示在遞回任務的父繫上。 它會顯示每個週期性任務的持續時間，如建立任務時定義。 如需建立週期性工作的相關資訊，請參閱 <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">建立週期性任務</a>. </p> <p> <b>注意</b>

   在個別週期性任務中修改的持續時間不顯示此欄位中指示的值。 </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">期間</td> 
      <td> 
      <div> 
      <div> 
      <p>這是您允許任務在完成前保持開啟的時間長度。 </p> 
      <p><b>重要</b>

   由於任務期間通常是計劃開始與計畫完成日期之間的時間量，因此會影響專案的時間表。</p>

   <p>若要指出工作的持續時間與時間單位，請執行下列動作：</p> 
      <ul> 
      <li> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">輸入時間長度，然後從下拉式選單中的可用時間單位中選取。</p> <p><b>秘訣</b></p>
      當您更新任務清單中的任務期間時，可以使用時間單位的縮寫。 </p> </li> 
      </ul> 
      <p> 您可以從下表中的一般時間或經歷時間選項中選擇： </p> 
      <table style="table-layout:auto"> 
      <col> 
      <col data-mc-conditions=""> 
      <tbody> 
      <tr> 
      <td>時間單位</td> 
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
      <td>天。 這是預設值。 </td> 
      <td>D</td> 
      </tr> 
      <tr> 
      <td>週</td> 
      <td>週</td> 
      </tr> 
      <tr> 
      <td>個月</td> 
      <td>T</td> 
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

   <p><b>附註</b>

   <p>經過的時間是任務期間的時間單位。 這是任務的計劃開始日期與計畫完成日期之間的時間，包括假日、週末和休假。 換句話說，經過的時間就是行事曆的天數。

   正常時間會將假日、週末和休假列入考量，並將他們排除在任務的持續時間之外。 如需工作持續時間的詳細資訊，請參閱 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任務期間與期間型別概觀</a>. </p>
   </div> 
   </div> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">規劃時數</td> 
   <td> <p>指定任務的計畫時數（以時數為單位）。 這是工作的受指派人完成工作所需的實際時間。 當「期間型別」設定為「計算的指定任務」時，您只能指定任務的計畫時數。 如需持續時間型別的詳細資訊，請參閱 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任務期間與期間型別概觀</a>.</p> 
   <b>注意</b>
   <p>
   建立週期性任務時，計畫時數是每個事件的計畫時數。 父系任務的計畫時數是所有發生次數的所有計畫時數總計。 如需建立週期性工作的相關資訊，請參閱 <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">建立週期性任務</a>.
   </p>

   </td> 
   </tr> 
   <tr> 
   <td role="rowheader">配置</td> 
   <td> <p>如果您的任務限制是已計算的工作或投入比導向，請指定 <strong>配置%</strong> （配置百分比）來指定每個受指派人。 這是受指派人排程中可在此任務上花費的時間。 變更受指派人的配置百分比將會變更任務的計畫時數。 </p> <p>當「任務限制」為「簡單」時，您可以指定下列專案：</p> 
      <ul> 
      <li> <p>每個受指派人的分配時數。</p> </li> 
      <li> <p>任務的計畫時數</p> </li> 
      <li> <p>任務期間</p> </li> 
      </ul> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">受指派人角色</td> 
   <td> <p>從中選擇一個角色 <strong>受指派人的角色</strong> 當您選取某人作為受指派人時，出現下拉式功能表。 這是受指派人可以在此任務上履行的角色。 </p> <p><b>秘訣</b>

   下拉式功能表中只會顯示與其設定檔中每個受指派人相關聯的工作角色。</p> </td>
   </tr> 
      </tbody> 
      </table>

1. 按一下 **儲存** 或繼續下列章節。

### 自訂表單

您可以定義預設自訂表單，以在任務新增至專案時自動附加至任務。 如需有關設定專案以納入所有新任務的預設任務自訂表單的資訊，請參閱文章中的「任務」一節 [編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md).

1. 如上所述開始編輯工作。
1. 按一下 **自訂Forms** ，或按一下自訂表單的名稱（若已附加）。

   ![](assets/nwe-custom-forms-section-edit-task-box-350x127.png)

1. 按一下 **新增自訂表格** 並選取您想要與工作建立關聯的一或多個自訂表單。 您必須先建置自訂表單，才能在此欄位中選取它們。 清單中只會顯示作用中的自訂表單。

   如需建立自訂表單的詳細資訊，請參閱 [建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).您最多可以新增十個自訂表單至任務。

1. （視條件而定）如果您將自訂表單附加到任務，請編輯表單上的任何欄位。 您必須先指定所有必填欄位，然後才能儲存任務。

   >[!NOTE]
   >
   >根據您的Workfront管理員如何設定自訂表單中區段的許可權，不是每個人都可以檢視或編輯給定自訂表單上的相同欄位。 編輯自訂表單區段中欄位的許可權取決於您對任務本身的許可權。 如需關於設定工作許可權的資訊，請參閱 [共用任務](../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).

1. 按一下 **儲存** 或繼續下列章節。

### 財務 {#finance}

1. 開始編輯您的工作，如中所述 [編輯任務](#Edit2) 一節。
1. 按一下 **財務** 在左側面板中。

   ![](assets/nwe-finance-section-edit-task-box-350x298.png)

1. 更新下列欄位：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">成本類型</td> 
      <td> <p>指定作業的成本型別。 這將決定如何根據任務的小時數計算任務成本。 </p> <p>從下列選項中選取： </p> 
       <ul> 
        <li> <p>無成本</p> </li> 
        <li> <p>固定每小時 </p> </li> 
        <li> <p> 使用者每小時 </p> </li> 
        <li> <p> 角色每小時</p> </li> 
       </ul> <p>如需有關追蹤成本的詳細資訊，請參閱 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">追蹤成本</a> . 您的Workfront管理員或群組管理員會為您的系統或群組中的任務選取預設成本型別設定。 如需有關設定專案預設值的資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">設定全系統專案偏好設定</a> .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">收入類型</td> 
      <td> <p>指定工作的收入型別。 這將根據任務的小時數，決定如何計算任務的收入。 </p> <p>從下列選項中選取： </p> 
       <ul> 
      <li> <p> 不可計費 </p> </li> 
      <li> <p>使用者每小時 </p> </li> 
      <li> <p>角色每小時 </p> </li> 
      <li> <p>固定每小時 </p> </li> 
      <li> <p>受限使用者小時 </p> </li> 
      <li> <p>受限角色小時 </p> </li> 
      <li> <p>使用者小時加固定 </p> </li> 
      <li> <p>角色小時加固定 </p> </li> 
      <li> <p>固定收入 </p> </li> 
       </ul> <p>如需有關追蹤收入的詳細資訊，請參閱<a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">帳單與收入概要</a> . </p> <p>您的Workfront管理員或群組管理員會為您的系統或群組中的任務選取預設收入型別設定。 如需有關設定專案預設值的資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">設定全系統專案偏好設定</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **儲存** 或繼續下列章節。

### 設定 {#settings}

1. 開始編輯您的工作，如中所述 [編輯任務](#Edit2) 一節。
1. 按一下 **設定** 在左側面板中。

   ![](assets/nwe-settings-section-edit-task-box-350x304.png)

1. 更新下列欄位：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">追蹤模式</td> 
      <td> <p>指定追蹤任務進度狀態的方式。 </p> <p>從下列選項中選取： </p> 
       <ul> 
      <li> <p> 使用者必須更新 </p> </li> 
      <li> <p>假設準時 </p> </li> 
      <li> <p>忽略遲到警告</p> </li> 
      <li> <p> 自動完成 </p> </li> 
      <li> <p>前置任務 </p> </li> 
       </ul> <p>如需有關工作的追蹤模式的詳細資訊，請參閱 <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">任務追蹤模式概觀</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">資源平準</td> 
      <td> <p>選取 <strong>從資源平準排除</strong> 欄位，表示希望將指派給任務的資源從平準中排除。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">平準延遲</td> 
      <td> <p>指定平準延遲（以小時為單位）。 </p> <p> 如需有關平準延遲的詳細資訊，請參閱 <a href="../../../manage-work/tasks/task-information/task-leveling-delay.md" class="MCXref xref">更新任務平準延遲</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">核准程序</td> 
      <td> <p>選取您要與工作關聯的核准程式。 您的Workfront管理員必須定義系統層級的核准流程，您才能將其與任務建立關聯。 擁有核准流程管理存取許可權的使用者也可以建立群組特定的核准流程。 </p> <p>如需有關建立核准流程的詳細資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md">建立工作專案的核准流程</a>. 新增核准程式時，請考量下列事項： </p> 
       <ul>

   <li> <p>清單中只會顯示有效的核准流程。 </p> </li>

   <li> <p>系統範圍及群組特定的核准程式會顯示在清單中。 與專案群組以外的群組相關聯的核准程式不會顯示在清單中。 </p>

   <p><b>重要</b>

   如果專案的群組變更，先前附加的群組特定核准流程會變成單一使用核准流程。 如需關於專案群組變更或核准流程變更如何影響核准設定的詳細資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md">群組和核准流程變更如何影響指派的核准流程</a>. </p>

   </li>

   <li> <p>您可以定義預設核准流程，以在任務新增至專案時自動附加至任務。 如需關於設定專案以包含預設任務核准流程的資訊，請參閱文章中的「任務」一節 <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">編輯專案</a>. </p> </li>

   <li> <p>大量編輯任務時，會出現下列情況： </p> 
      <ul> 
      <li> <p>當您從相同群組選取多項作業時，系統層次與群組層次核准程式都會顯示在此欄位中。 </p> </li> 
      <li> <p>當您從不同的群組選取多個任務時，此欄位中只會顯示系統層級的核准流程。 </p> </li> 
      <li> <p>當任何作業附加單一使用核准程式時，您選取的系統層級或群組層級核准程式會取代該作業。 </p> </li>

   </ul> </li> 
      </ul> </td> 
     </tr> 
    </tbody> 
   </table>
    </li>

1. 按一下「**儲存**」。

<!--notes from the table: <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this bullet stays here although the sections it might appear in are QS only, so we can use the snippet for both Qs and classic)</p>       -->

## 在任務標題中編輯任務（受限）

您可以在任務標題中編輯有限數量的資訊。

您的系統或群組管理員可以自訂您在任務標題中看到的欄位。 如需詳細資訊，請參閱 [使用版面配置範本自訂物件標頭](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).


![](assets/qs-task-header-without-approvals-and-with-dependecies-350x17.png)

預設情況下，以下欄位包含在任務標題中：

* 任務名稱
* 完成百分比
* 指派
* 規劃完成日期

  >[!CAUTION]
  >
  >某些任務限制和其他相依性可能會阻止您編輯此欄位。 有關作業限制的資訊，請參閱 [任務限制總覽](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* 狀態
* 如果您在目前的核准程式中設為核准者，請進行核准決定

## 大量編輯任務

您可以大量編輯清單中的任務，並在選擇自動儲存對清單中的任務所做的變更時，同時更新其所有資訊。

如需大量儲存任務的詳細資訊，請參閱文章中的「大量編輯任務」一節 [編輯清單中的任務](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).
