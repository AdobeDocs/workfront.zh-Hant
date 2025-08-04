---
product-area: templates
keywords: 任務，預設，自動化，建立
navigation-topic: templates-navigation-topic
title: 編輯範本任務
description: 建立範本後，您可以編輯有關範本任務的資訊。 使用範本建立專案或將範本附加到專案後，您在範本任務上更新的資訊會與專案任務相關聯。
author: Alina
feature: Work Management
exl-id: 2df8522e-7eee-4440-be0f-f7483c5acdb0
source-git-commit: a92c85ad5f58700138d7750423cc3d134d980a9e
workflow-type: tm+mt
source-wordcount: '2493'
ht-degree: 4%

---

# 編輯範本任務

<!--Audited: 09/2024-->

建立範本後，您可以編輯範本任務的資訊。 使用範本建立專案或將範本附加到專案後，您在範本任務上更新的資訊會與專案任務相關聯。

如需建立範本的相關資訊，請參閱[建立專案範本](../../../manage-work/projects/create-and-manage-templates/create-template.md)。

您可以編輯範本任務或大量編輯範本任務。

>[!NOTE]
>
>您無法大量編輯屬於不同範本的範本任務。 您只能編輯屬於相同範本的範本任務。


## 存取需求

+++ 展開以檢視存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>標準 </p>
   <p>規劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級</td> 
   <td> <p>編輯範本的存取權</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權 </td> 
   <td> <p>管理範本的許可權。 </p> <p>範本任務的Contribute或更高許可權。</p> </td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

開始之前，您必須

* 建立範本。

  如需建立範本的相關資訊，請參閱[建立專案範本](../../../manage-work/projects/create-and-manage-templates/create-template.md)。

## 編輯範本任務

您可以使用「編輯範本任務」或「範本任務詳細資訊」區域編輯範本任務。 下列步驟說明如何在「編輯範本任務」方塊中編輯任務。

{{step1-to-templates}}

1. 按一下範本名稱以開啟。
1. 按一下左側面板中的&#x200B;**範本任務**。
1. 按一下清單中範本任務的名稱以開啟範本任務。
1. （選擇性）按一下左側面板中的&#x200B;**前置任務**&#x200B;區段，為範本任務新增前置任務。 新增範本任務前置任務與新增專案任務前置任務類似。 如需詳細資訊，請參閱[使用前置任務區域建立前置任務關係](/help/quicksilver/manage-work/tasks/use-prdcssrs/create-predecessors-in-predecessors-area.md)。
1. （選擇性）按一下左側面板中的&#x200B;**子任務**&#x200B;區段，為範本任務新增子系。 為範本任務新增子任務與新增專案任務子任務類似。 如需詳細資訊，請參閱文章[建立子任務](/help/quicksilver/manage-work/tasks/create-tasks/create-subtasks.md)中的「從任務建立子任務區段」一節。

1. （視條件而定）若要編輯範本任務的有限資訊，請按一下左側面板中的&#x200B;**範本任務詳細資訊**，然後移至[詳細資訊]區段的區域以編輯每個區域的資訊。
1. （選擇性）按一下&#x200B;**全部收合**&#x200B;圖示![全部收合圖示](assets/collapse-all-icon.png)以收合所有區域。
1. 若要編輯詳細資訊區段中的資訊，請按一下&#x200B;**編輯**&#x200B;圖示![編輯圖示](assets/edit-icon.png)，然後從下列任何區域選取，或按一下&#x200B;**編輯全部**&#x200B;以編輯所有區域的資訊：

   * 概觀
   * 自訂表單

     只有當物件附有自訂表單時，才會顯示自訂表單的名稱。

   * 財務

   >[!TIP]
   >
   >如需詳細資訊區域中顯示的所有欄位相關資訊，請使用「編輯範本任務」方塊繼續編輯所有欄位，如下所述。
1. （選擇性）若要大量編輯數個範本工作，請選取多個範本工作，然後按一下範本清單頂端的&#x200B;**編輯**。
1. （視條件而定）若要同時編輯範本任務或數個任務的所有相關資訊，請按一下以從清單中選取它們，然後按一下清單頂端的&#x200B;**編輯**&#x200B;圖示![編輯圖示](assets/edit-icon.png)。

   **編輯範本任務**&#x200B;方塊隨即顯示。

   >[!TIP]
   >
   >您也可以在清單中選取範本任務，然後按一下「編輯」以開啟「編輯範本任務」方塊。

   ![編輯範本任務](assets/edit-template-tasks-box-classic-350x356.png)

1. 請考慮在下列任何一節中指定資訊：

   * [概觀](#overview)
   * [財務](#finance)
   * [設定](#settings)
   * [指派](#assignments)
   * [自訂表單](#custom-forms)
   * [評論](#comment)

### 概觀 {#overview}

1. 如上所述，開始編輯範本任務。
1. 按一下&#x200B;**概觀**。

   ![edit_task_overview.png](assets/edit-task-overview-350x438.png)

1. 更新下列任一專案：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>名稱</strong> </td> 
      <td>指定範本工作的名稱。 大量編輯範本任務時不會顯示此欄位。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>說明</strong> </td> 
      <td>新增關於範本任務的其他資訊。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td>指定與範本任務相關資訊相關的網頁連結。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>優先順序</strong> </td> 
      <td> <p>這是視覺化旗標，可讓您排定範本工作的優先順序。 </p> <p>從下列選項中選取：</p> 
       <ul> 
        <li> <p><strong>無</strong> </p> </li> 
        <li> <p><strong>低</strong> </p> </li> 
        <li> <p> <b>一般</b></p> </li> 
        <li> <p><b>高</b> </p> </li> 
        <li> <p><b>緊急</b> </p> </li> 
       </ul> <p>根據Workfront管理員選取的專案偏好設定，您的優先順序名稱可能會不同。 如需有關編輯優先順序的詳細資訊，請參閱<a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">建立及自訂優先順序</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>期間類型</strong> </td> 
      <td> <p>從此範本建立的未來任務將具有此期間型別。 <br>期間型別識別下列專案之間的關係：</p> <p> — 指派給任務的資源數量</p> <p> — 完成任務所需的總工作量</p> <p> — 任務的總持續時間。 </p> <p>期間型別可讓您根據作業的需求設定一致的資源指定。 如需有關任務期間型別的詳細資訊，請參閱<a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任務期間與期間型別概觀</a>。</p> <p>從下列選項中選取：</p> 
       <ul> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">計算的工作分派</span> </p> </li> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">已計算的工作</span> </p> </li> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">投入比導向</span> </p> </li> 
        <li> <p style="font-weight: bold;"><span style="font-weight: normal;">簡單</span> <br> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>期間</strong> </td> 
      <td> <p>指定未來工作的持續時間，單位為分鐘、小時、天、周或月。 從此範本建立的未來任務將在此指定持續時間。</p> <p>依預設，Workfront會測量持續時間（以天為單位）。 這是您允許任務在必須完成之前保持未完成的時間。 當任務的<strong>期間型別</strong>為<strong>簡單</strong>，或<strong>任務限制</strong>為<strong>固定日期</strong>時，您無法指定任務的期間。</p> <p><b>重要</b></p> <p>期間通常是範本任務的計劃開始與計畫完成日期之間的時間量，因此，會影響範本的時間表。 這會決定從範本建立的未來專案的時間表。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>規劃時數</strong> </td> 
      <td> <p>指定使用此範本建立的專案上未來任務的計畫時數。 這是工作的受指派人完成工作所需的實際時間。 當<strong>工期型別</strong>設定為<strong>已計算的工作分派</strong>時，您只能指定任務的計畫時數。 </p> </td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>任務限制</strong> </td> 
      <td> <p>從此範本建立的專案上的任務將具有此限制。 任務限制可識別任務何時必須完成。 </p> <p>從下列選項中選取：</p> 
       <ul> 
        <li><strong>固定日期</strong>。 指定<strong>計劃開始</strong>和<strong>計畫完成日期。</strong></li> 
        <li><strong>必須在</strong>開始。 指定<strong>計劃開始日期。</strong></li> 
        <li><strong>必須在</strong>完成。 指定<strong>計畫完成日期</strong>。</li> 
        <li><strong>儘快</strong> </li> 
        <li>儘可能遲<strong></strong> </li> 
        <li style="font-weight: bold;"><strong>最早可用時間</strong> </li> 
        <li style="font-weight: bold;"><strong>最新可用時間</strong> </li> 
        <li>開始時間不晚於。 指定<strong>計劃開始日期</strong>。</li> 
        <li><strong>開始時間不早於</strong>。 指定<strong>計劃開始日期</strong>。</li> 
        <li><strong>完成時間不超過</strong>。 指定<strong>計畫完成日期</strong>。</li> 
        <li><strong>完成時間不早於</strong>。 指定<strong>計畫完成日期</strong>。</li> 
       </ul> <p>如需任務限制的詳細資訊，請參閱<a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">任務限制總覽</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span style="font-weight: bold;">開始日</span><span style="font-weight: normal;"> （選擇性和條件性）</span> </td> 
      <td> <p> 只有當「任務限制」為下列其中一項時，才能指定範本任務的「開始日」：</p> 
       <ul> 
        <li>必須開始時間</li> 
        <li>開始時間不早於</li> 
        <li>開始時間不晚於</li> 
        <li>固定日期</li> 
       </ul> <p>這會對應未來專案時間表內任務開始日期。 對於所有其他限制，Workfront會根據任務之間的前置任務相依性計算「開始日」。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>完成日</strong><span style="font-weight: normal;"> （選擇性和條件性）</span> </td> 
      <td> <p> 只有當「任務限制」為下列其中一項時，才能指定範本任務的「完成日」：</p> 
       <ul style="list-style-type: circle;"> 
        <li>必須完成時間</li> 
        <li>完成時間不早於</li> 
        <li>完成時間不晚於</li> 
        <li>固定日期</li> 
       </ul> <p>這將對應於未來專案時間表內任務完成的日期。 對於所有其他限制，Workfront會根據持續期間和前置任務相依性計算「完成日」。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （選擇性）根據您要修改的資訊，繼續編輯下列區段。

   或

   按一下「**儲存變更**」。

### 財務 {#finance}

1. 如上所述，開始編輯範本任務。
1. 按一下&#x200B;**財務**。

   ![edit_task_finance.png](assets/edit-task-finance-350x216.png)

1. 更新下列任一專案：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>成本型別</strong> </td> 
      <td> <p>指定未來作業的成本型別。 這將根據任務的小時數，決定如何計算任務成本。 </p> <p>從下列選項中選取：</p> 
       <ul> 
        <li> <p style="font-weight: normal;"><span>無費用</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>固定小時</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>使用者小時</span> </p> </li> 
        <li> <p style="font-weight: normal;"><span>角色小時</span> </p> </li> 
       </ul> <p>如需追蹤成本的詳細資訊，請參閱<a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">追蹤成本</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>收入型別</strong> </td> 
      <td> <p>指定未來工作的「收入型別」。 這將根據任務的小時數，決定如何計算任務的收入。</p> <p style="font-weight: normal;">從下列選項中選取： </p> 
       <ul> 
        <li> <p style="font-weight: normal;">不可計費</p> </li> 
        <li> <p style="font-weight: normal;">使用者每小時</p> </li> 
        <li> <p style="font-weight: normal;">角色每小時</p> </li> 
        <li> <p style="font-weight: normal;">固定每小時</p> </li> 
        <li> <p style="font-weight: normal;">受限使用者小時</p> </li> 
        <li> <p style="font-weight: normal;">受限角色小時</p> </li> 
        <li> <p style="font-weight: normal;">使用者小時加固定</p> </li> 
        <li> <p style="font-weight: normal;">角色小時加固定</p> </li> 
        <li> <p style="font-weight: normal;">固定收入</p> </li> 
       </ul> <p>如需有關追蹤收入的詳細資訊，請參閱<a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">帳單與收入概觀</a>。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （選擇性）根據您要修改的資訊，繼續編輯下列區段。

   或

   按一下「**儲存變更**」。

### 設定 {#settings}

1. 如上所述，開始編輯範本任務。
1. 按一下&#x200B;**設定**。

   ![編輯範本任務設定](assets/edit-template-tasks-settings-classic-350x231.png)

1. 更新下列任一專案：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
   <tr> 
      <td role="rowheader"><p><b>里程碑</b></p></strong> </td> 
      <td> <p>選擇要與所選範本任務關聯的里程碑。</p>

   <p><b>重要</b></p>
   <p>您必須將里程碑路徑與範本建立關聯，才能顯示此欄位。 如需詳細資訊，請參閱<a href="../create-and-manage-templates/edit-templates.md">編輯專案範本</a>。</p> 
   </td> 
     </tr>
     <tr> 
      <td role="rowheader"><strong>追蹤模式</strong> </td> 
      <td> <p>指定未來任務進度狀態的追蹤方式。 </p> <p>從下列選項中選取：</p> 
       <ul> 
        <li> <p><strong>使用者必須更新</strong> </p> </li> 
        <li> <p><strong>假設於時間</strong> </p> </li> 
        <li> <p><strong>忽略遲到警告</strong> </p> </li> 
        <li> <p><strong>自動完成</strong> </p> </li> 
        <li> <p><strong>前置任務</strong> </p> </li> 
       </ul> <p>如需有關工作的追蹤模式的詳細資訊，請參閱<a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">工作追蹤模式概觀</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>核准流程</strong> </td> 
      <td> <p>選取您要與範本任務關聯的核准流程。 您的Workfront管理員必須定義系統層級任務核准流程，您才能將其與範本任務建立關聯。 <span>擁有核准程式管理存取許可權的使用者也可以建立群組特定的核准程式。</span>如需建立核准流程的詳細資訊，請參閱<a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">建立工作專案的核准流程</a>。</p> <p>新增核准程式時，請考量下列事項： </p> 
       <ul> 
       <li>清單中只會顯示有效的核准流程。 </li> 
       <li> <p>系統範圍及群組特定的核准程式會顯示在清單中。 與範本以外的群組相關聯的核准程式不會顯示在清單中。</p> <p>重要：如果與範本關聯的群組變更，群組特定核准流程會變成單一使用核准流程。 如需關於專案群組的變更或核准程式變更如何影響核准設定的詳細資訊，請參閱<a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">群組和核准程式變更如何影響指派的核准程式</a>。 </p> </li> 
       <li> <p>如果您新增單次使用的核准流程，在此欄位中會顯示為「&lt;Custom&gt;」。 如需詳細資訊，請參閱<a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">將新的或現有的核准程式與工作建立關聯</a>。 </p> <!--<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will be valid only for Classic when they edit the Edit Template box in NWE)</p>--> </li> 
       <li> <p>大量編輯範本任務時，會出現下列情況：</p> 
       <ul> 
       <li> <p>當您從相同的範本群組選取範本任務時，系統層次和群組層次核准程式都會顯示在此欄位中。</p> </li> 
       <li> <p>當您從不同的範本群組選取範本任務時，此欄位中只會顯示系統層級的核准程式。</p> </li> 
       <li> <p>當任何範本任務附加單一使用核准程式時，它會由您選取的系統層級<span>或群組層級核准程式</span>取代。 </p> </li> 
       </ul> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>提醒通知</strong> </td> 
      <td> <p>選取您要附加至範本任務的提醒通知。 它們將會附加到從此範本建立的專案上的未來任務中。 您的系統管理員必須先設定「提醒通知」，您才能在任務中選取它們。 如需設定提醒通知的詳細資訊，請參閱<a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">設定提醒通知</a>。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （選擇性）根據您要修改的資訊，繼續編輯下列區段。

   或

   按一下「**儲存變更**」。

### 指派 {#assignments}

1. 如上所述，開始編輯範本任務。
1. 按一下&#x200B;**指派**。

   ![assignments_edit_tasks.png](assets/assignments-edit-tasks-350x87.png)

1. 按一下「**新增受指派人**」以將新的受指派人新增至範本任務。 您可以將使用者、角色或專案團隊指派給任務。 一個任務可以有多個受指派人。 從此範本任務建立時，未來任務將擁有相同的資源指派給它。
1. （選擇性）如果您有多個受指派人，請選取「**所有者**」選項按鈕，指出哪個使用者或角色被視為任務所有者或主要受指派人。 Workfront會將您指派給範本任務的第一個使用者或工作角色標籤為擁有者或主要受指派人。
1. （條件式與選擇性）如果您的任務限制是計算的工作或投入比導向，請為每個受指派人指定&#x200B;**配置%** （配置百分比）。 這是受指派人排程中可在此任務上花費的時間。 變更受指派人的配置百分比將會變更任務的計畫時數。
1. （條件式與選擇性）如果您的任務限製為「簡單」，請指定每個受指派人的&#x200B;**小時**

   或

   指定範本任務的&#x200B;**計畫時數**&#x200B;總數。 這會將總時數平均分配到所有被指定者。

1. （條件式與選擇性）如果您的任務限製為「簡單」，請以天為單位指定範本任務的&#x200B;**工期**。 這會成為從此範本建立之任務的工期。
1. （選擇性）從&#x200B;**受指派人的角色**&#x200B;下拉式功能表中選取角色。 這是受指派人可以在此未來任務中履行的角色。 下拉式功能表中只會顯示與其設定檔中每個受指派人相關聯的工作角色。
1. （選擇性）根據您要修改的資訊，繼續編輯下列區段。

   或

   按一下「**儲存變更**」。

### 自訂表單 {#custom-forms}

您可以定義自訂表單，當任務新增至專案時，預設會自動附加至任務。 如需關於設定專案以包含預設任務自訂表單的資訊，請參閱文章[編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md)中的[任務]區段。

您也可以新增自訂表單至範本任務，以在從範本建立專案時新增自訂表單至專案的未來任務。

1. 如上所述，開始編輯範本任務。
1. 按一下&#x200B;**自訂Forms**。

   ![custom_forms_edit_task.png](assets/custom-forms-edit-task-350x136.png)

1. 選取您想要與範本任務建立關聯的一或多個自訂表單。

   您必須先建置自訂表單，才能在此欄位中選取它們。
清單中只會顯示作用中的自訂表單。
如需建立自訂表單的詳細資訊，請參閱[建立自訂表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。
您最多可以將十個自訂表單新增到範本任務中。
表單會自動新增至從範本建立的任務。
1. （條件式與選擇性）如果您將自訂表單附加到範本任務，請編輯表單上的任何欄位。 您必須指定所有必填欄位，然後才能儲存範本任務。

   >[!NOTE]
   >
   >根據您的Workfront管理員如何設定自訂表單中區段的許可權，不是每個人都可以檢視或編輯給定自訂表單上的相同欄位。 編輯自訂表單區段中欄位的許可權取決於範本任務或未來任務的許可權。\
   >如需設定自訂表單區段許可權的相關資訊，請參閱[共用自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md)。\
   >如需設定工作許可權的相關資訊，請參閱[共用工作](../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md)。\
   >如需關於設定範本許可權的資訊，請參閱[共用範本](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md)。

1. （選擇性）根據您要修改的資訊，繼續編輯下列區段。

   或

   按一下「**儲存變更**」。

### 評論 {#comment}

1. 如上所述，開始編輯範本任務。
1. 按一下&#x200B;**註解**。

   ![comment_edit_task.png](assets/comment-edit-task-350x138.png)

1. 指定要在可用欄位中範本任務的更新資料流中顯示的註解。 每個人都可以看見此註解，只要他們擁有範本和範本任務的檢視存取權，以及檢視註解的存取權。
1. 按一下「**儲存變更**」。

   當您或其他使用者從此範本建立專案時，您套用至範本任務的所有設定都會成為專案任務的設定。
