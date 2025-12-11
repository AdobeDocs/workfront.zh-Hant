---
product-area: reporting
navigation-topic: reporting-elements
title: 在Adobe Workfront中建立或編輯檢視
description: 您可以使用檢視來自訂顯示在熒幕上的資訊型別。 您可以在Adobe Workfront中使用數種檢視。
author: Nolan
feature: Reports and Dashboards
exl-id: 8fcd6320-c939-4195-8972-5c31575f78cb
source-git-commit: 0c0ffbeefb0eed8d1ca2a6e68ed19b40080726df
workflow-type: tm+mt
source-wordcount: '898'
ht-degree: 4%

---

# 在Adobe Workfront中建立或編輯檢視

<!-- Audited: 11/2024 -->

您可以使用檢視來自訂顯示在熒幕上的資訊型別。 您可以在Adobe Workfront中使用數種檢視。

本文說明如何建立及編輯清單與報告的標準檢視。

如需詳細資訊，請參閱[Adobe Workfront中的檢視總覽](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 封裝</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</strong></td> 
   <td> 
    <p>投稿人或以上</p>
    <p>要求或更高版本</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯對篩選器、檢視、群組的存取權</p> <p>編輯對報告、儀表板、行事曆的存取權，以在報告中建立檢視</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權，以建立或編輯報表中的檢視</p> <p>管理檢視的許可權以進行編輯</p>
   </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。
+++

## 建立或自訂檢視

建立或自訂檢視的流程會因您建立或自訂標準檢視、敏捷檢視或展示板檢視而有所不同。

* [建立或自訂標準檢視](#create-or-customize-a-standard-view)
* [建立或自訂敏捷檢視](#create-or-customize-an-agile-view)

### 建立或自訂標準檢視 {#create-or-customize-a-standard-view}

您可以建立新的標準檢視，也可以自訂您先前建立的現有標準檢視。

1. 在您要建立或自訂檢視的任何清單上，按一下&#x200B;**檢視**&#x200B;下拉式功能表。

1. 按一下「**+新增檢視**」按鈕以建立新檢視。
或
按一下滑鼠右邊要編輯的現有檢視右邊出現的**編輯**&#x200B;圖示![編輯圖示](assets/edit-icon.png)。
顯示**自訂檢視**&#x200B;對話方塊。

1. 在&#x200B;**資料行預覽**&#x200B;區段中，執行下列任一項作業：

   * 按一下欄標題，然後選取新欄位，修改任何欄的值。
   * 按一下&#x200B;**新增欄**&#x200B;來新增欄，開始輸入您要新增的欄名稱，然後當它出現在下拉式清單中時按一下它。
   * 將欄標題拖曳至新位置，調整欄的顯示順序。

   * 在&#x200B;**資料行設定**&#x200B;區域中，按一下&#x200B;**依**&#x200B;摘要此資料行，然後選擇資料在資料行中的顯示方式。 此選項適用於下列欄型別：
     <table style="table-layout:auto"> 
         <col> 
         <col> 
         <tbody> 
          <tr> 
           <td role="rowheader"><strong>日期欄位</strong></td> 
           <td><ul>
           <li>最大值</li>
         <li>最小值</li>
           </ul></td> 
          </tr> 
          <tr>
           <td role="rowheader"><strong>貨幣欄位</strong></td> 
           <td><ul>
           <li>計數</li>
         <li>Sum</li>
           <li>平均</li>
         <li>最大值</li>
           <li>最小值</li>
         </ul></td> 
          </tr> 
         <tr>
           <td role="rowheader"><strong>字串和布林值欄位</strong></td> 
           <td><ul><li>計數</li></ul>
           <p>注意：Workfront通常不建議依計數彙總布林欄位，因為值將一律為true/false。</p></td> 
          </tr> 
         </tbody> 
        </table>

     >[!NOTE]
     >
     >當您彙總分組中下列欄位的值時，下列例外情況適用於父系物件（例如父系任務）：
     >   
     > * 除「實際時數」之外的所有數字與貨幣欄位（例如，計畫/實際勞力成本、計畫/實際費用成本、計畫/實際成本、計畫時數）會彙總只有子任務與獨立任務的值。 它們不會摘要父系任務的值或父系父系的值。
     > * 實際小時會摘要主要父系和獨立任務的值；它們不會摘要父系任務的父系或子系任務的數字。
     > * 數字和貨幣值的自訂資料欄位會摘要所有工作：父項、子項、父項的父項，以及獨立工作。
     >
     >如需在報告中使用群組的詳細資訊，請參閱文章[ Adobe Workfront中的群組概觀](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)。

      * （選擇性）按一下&#x200B;**進階選項**，為資料行指定下列資訊：

        <table style="table-layout:auto"> 
         <col> 
         <col> 
         <tbody> 
          <tr> 
           <td role="rowheader"><strong>自訂欄標籤</strong></td> 
           <td><p>指定欄的自訂標籤。 此標籤會取代預設標籤。 我們建議僅使用UTF-8字元以避免相容性問題。</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>欄位格式</strong></td> 
           <td>選取您要為欄中的欄位顯示值的格式。</td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>在報告面板上顯示此欄</strong></td> 
           <td><p>當報告與其他報告並排顯示時，選取此選項可在控制面板上顯示此欄。 取消選取此選項時，在報告並排顯示的儀表板上檢視報告時不會顯示此欄。</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>欄規則</strong></td> 
           <td><p>按一下<strong>+為此資料行</strong>新增規則，以定義資料行的規則。 新增規則後，您可以定義欄位和文字樣式，以顯示符合該規則的欄位。 完成規則定義後，按一下<strong>新增規則</strong>。</p></td> 
          </tr> 
         </tbody> 
        </table>

        如需有關報表中有條件格式化檢視表的詳細資訊，請參閱文章[在文字模式中使用條件格式](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md)。

1. （視條件而定）如果您按一下&#x200B;**進階選項**，請按一下&#x200B;**完成**。

1. 按一下&#x200B;**儲存檢視**&#x200B;以建立新檢視，或以您的變更取代目前的檢視。\
   或\
   按一下&#x200B;**另存為新檢視**，將您的變更另存為新檢視。

   >[!TIP]
   >
   >當您自訂內建Workfront檢視時，**另存為新檢視**&#x200B;是唯一可用的選項。

   您的存取權會指定檢視的儲存方式。 如果最初建立的是檢視，您可以儲存變更；否則，系統會提示您儲存版本。 請記住，您對檢視所做的變更會影響已共用檢視的使用者。

### 建立或自訂敏捷檢視 {#create-or-customize-an-agile-view}

敏捷檢視（也稱為面板檢視）只會顯示專案中的任務和問題清單。

它們已預先設定，但您可以修改其特定設定。

如需有關敏捷或展示板檢視的詳細資訊，請參閱文章[在敏捷檢視中管理專案](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md)。

<!-- Legacy Agile views were deprecated with 25.3. This is old: 

>[!NOTE]
>
>This procedure only applies to the legacy Agile view, not to the board view of a project.

To create or customize an Agile view:

1. Go to the list of tasks on a project.
1. Click the **Board** icon ![Board icon](assets/board-icon-for-agile-view.png), and then click **Use legacy agile** on the board view.

1. (Conditional) To customize an existing Agile view:

   1. Click the **View** drop-down menu, then select the Agile view you want to customize.  
      You cannot customize the default Agile view.
   
   1. Click the **View** drop-down menu again, then click **Customize View**.  
      ![Customize view](assets/view-agile-customize.png)

1. (Conditional) To create a new Agile view, click **New View**.  
   The **Customize Agile View** dialog box displays.  

1. In the **Customize Agile View** dialog box, specify a name for the Agile view.  
   We recommend that you include the word "Agile" in your view name, so users know this is an Agile view.  
   This name is displayed in the **View** drop-down menu when selecting a view.

1. Define the status columns to display on the story board in the agile view. These are the task statuses that are defined by the Workfront administrator, as described in [Create or edit a status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

   Only system statuses are available to use on the Agile story board. If a status is available only for an individual group you are a member of, the status is not available on the agile story board. Furthermore, tasks that are in a status that is available only to a custom group are not visible when viewing the project in an Agile view.

   Users can move stories among these status columns on the Agile story board.  
   When defining status columns, you can do the following:

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Reorder status columns:</strong> </td> 
      <td> Drag a status column to the order where you want it to appear.<br><img src="assets/agile-project-reorderstatuses-350x141.png" alt="" style="width: 350;height: 141;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Remove status columns:</strong> </td> 
      <td>Click the (x) icon on the column that you want to remove.<br>You cannot remove the "New" status unless a custom status has been added to the view and that custom status equates with "New."<br>For information about creating a custom status, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Create or edit a status</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Add status columns:</strong> </td> 
      <td> <p>Click the <strong>Plus</strong> icon, then select the status you want to add.<br>All default system statuses are displayed, as well as any custom statuses that have been shared with you.<br>You can configure up to 10 statuses to display.</p></td> 
     </tr> 
    </tbody> 
   </table>

   *********   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE FOR ADD STATUS COLUMNS: research this and add: [! What if the status has been shared with me or a group I'm in (so I can see it here), but the status hasn't been shared with another user who also has access to a project where I later apply this view? Can that user still see this status on the project?]) </p>
       *************

1. In the **Associate Card Color to** area, select from the following options:

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Story:</strong> </td> 
      <td>Any subtasks match the color of the parent task, so that the colors of all stories in any given swimlane are the same.<br>Colors are randomly assigned to tasks when they are created if the task does not have any subtasks or does not have a parent task.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Free Form:</strong> </td> 
      <td> All cards are displayed as blue by default until a user changes the color manually, as described in the article <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/categorize-stories-by-color.md" class="MCXref xref">Categorize stories by color on the Scrum board</a>. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priority:</strong> </td> 
      <td> <p> Colors are associated with the story priority, as follows:</p> 
       <ul> 
        <li>High = Red</li> 
        <li>Medium = Yellow</li> 
        <li>Low = Green<br>If your Workfront administrator has configured custom priorities for your Workfront system, the highest priority is red, the second-highest is yellow, and the remaining are green.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Task Owner:</strong> </td> 
      <td> All stories with the same primary assignee are the same color.<br>The primary assignee is the user who was first assigned to the task. </td> 
     </tr> 
    </tbody> 
   </table>

1. In the **Additional Fields** area, click **Add Field**, then select the field you want to add to story cards. (These are the same fields you can add when creating customizing a view or creating columns for a report.)  
   Repeat this process to add up to three additional fields to the story cards.  
   When you add fields to story cards, fields are view-only and display only when the field is populated.

   By default, the following types of data is displayed on the story card:

   * Story name with a link directly to the task
   * The project name with a link directly to the project  
     This link is displayed only when using the agile view on an iteration; it is not displayed when using an Agile view on a project.
   * The task description
   * Current commitment
   * View and edit the percent complete either by adjusting the percent complete itself or by adjusting the number of points or hours that are complete
   * Assigned Users

   You can display additional data (including custom data) on story cards. You might want to display additional fields on story cards for any number of reasons. For example, you might want to display the Customer ID if you are working on stories for multiple customers within the project, or you might want to display the Task Start Date.

1. Click **Save**.  
   Your access dictates how the view is saved. If you created the view originally, you can save the changes; otherwise, you are prompted to save a version. Keep in mind that changes you make to the view impact users with whom the view has been shared.

1. (Optional) Click the **List** icon to return to the list of tasks.

-->
