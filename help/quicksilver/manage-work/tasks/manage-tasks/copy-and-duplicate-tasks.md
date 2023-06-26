---
product-area: projects
navigation-topic: manage-tasks
title: 複製和複製任務
description: 您可以將任務從專案複製到另一個專案，也可以複製同一專案中的任務。
author: Alina
feature: Work Management
exl-id: daf89062-cf58-4c39-83ff-727d969a9630
source-git-commit: 1f749ba9a54ce75a917e4b1e95713ac7abeaa66b
workflow-type: tm+mt
source-wordcount: '1705'
ht-degree: 1%

---

# 複製和複製任務

您可以將任務從專案複製到另一個專案，也可以複製同一專案中的任務。

您可以一次複製或複製一個或多個任務或父任務。

## 存取需求

<!-- drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a task</p> <p>Contribute or higher permissions to the project</p> 
   <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>工作或以上 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯對任務和專案的存取權</p> <p><b>附註</b>

如果您仍然沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理任務的許可權 </p> <p>貢獻或更高的專案許可權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 複製任務的注意事項

複製任務時，請考量下列事項：

* 問題不會與任務一起複製。
* 里程碑會傳輸到複製的任務並從原始任務中移除。
* 將任務從一個專案複製到另一個專案時，可能會重新計算任務日期。 重新計算將考慮新專案使用的排程和專案的「排程起始日期」資訊。

您可以在Adobe Workfront Web應用程式的下列區域中複製任務：

* 在任務層級，從 **「更多」圖示** ![](assets/qs-more-menu-19x7.png) 在任務名稱的右側。

  如需詳細資訊，請參閱 [在任務層級複製任務](#copy-a-task-at-the-task-level) 章節。

* 在任務清單中，執行下列任一項作業：

   * 以滑鼠右鍵按一下工作名稱。
   * 選取任務（或多項任務）並展開 **更多** 圖示 ![](assets/more-icon-task-list.png) 位於工作清單頂端。
   * 選取任務並展開 **更多** 圖示 ![](assets/more-icon-task-list.png) 位於任務名稱旁。

     選取多個任務時，此選項無法使用。

  如需詳細資訊，請參閱 [複製清單中的任務](#copy-tasks-in-a-list) 章節。

## 複製清單中的任務 {#copy-tasks-in-a-list}

1. 前往包含您要複製之任務的一或多個任務的專案。

   或

   前往任務報告。

1. 按一下 **任務** 在左側面板中。
1. 按一下 **計畫模式功能表** ![](assets/qs-list-mode-or-save-mode-icon-small.png) ，則 **自動儲存**.

   >[!IMPORTANT]
   >
   >只有在自動儲存變更時，您才能複製清單中的任務。 如需有關編輯任務時儲存選項的資訊，請參閱 [編輯清單中的任務](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

1. 選取要複製的一個或多個任務，然後執行下列任一項作業：

   * 按一下 **更多選單** 在任務清單頂端，然後按一下 **複製到**.
   * 以滑鼠右鍵按一下選取的任務，然後按一下 **複製到**.
   * 選取一個任務時，按一下 **更多** 功能表 ![](assets/more-icon-task-list.png) 在清單中工作名稱旁邊，然後按一下 **複製到**.

   ![](assets/copy-task-in-list-nwe-350x131.png)

1. 繼續複製工作，如區段中所述 [在任務層級複製任務](#copy-a-task-at-the-task-level) 從步驟4開始。

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: is this still accurate?!)
   </MadCap:conditionalText>
   -->

## 在任務層級複製任務 {#copy-a-task-at-the-task-level}

除了複製任務清單中的任務外，您也可以在開啟任務後複製任務。 

1. 透過搜尋來尋找Workfront系統中的任務。
1. 按一下工作名稱以開啟。 
1. 按一下 **更多** 下拉式功能表 ![](assets/qs-more-menu.png) 在任務名稱旁邊，然後按一下 **複製** **至**.

   ![](assets/taskcopy-to-at-the-task-level-nwe-350x200.png)

   「複製工作」方塊隨即顯示。

1. （可選）更新 **任務名稱**.

   >[!TIP]
   >
   >選擇複製清單中的多個任務時，此欄位會變暗且無法編輯。 您可以將滑鼠游標停留在「任務名稱」欄位上，所有選取的任務清單隨即顯示。
   >
   >![](assets/copy-task-multiple-tasks-box-with-list-of-task-names-nwe-350x130.png)

1. 輸入的名稱 **目的地專案** 您要將任務複製到 **選取目標專案** 欄位。 

   >[!TIP]
   >
   >* 專案名稱區分大小寫。
   >* 您也可以開始輸入「參考編號」或輸入專案的ID。 這可能會協助您區分具有相同名稱的專案。
   >* 清單中只會顯示100個專案。

   預設會顯示目前的專案名稱。 如果您想要複製相同專案中的任務，請保留此欄位不變。

1. （視條件而定）按一下 **要求存取權** 以請求專案的存取權（如果您沒有所選專案的存取權）。
1. （視條件而定）如果您有權將任務新增至目的地專案上的任務之一，請繼續將任務複製到所選目的地專案，而不請求存取權。

   ![](assets/copy-task-request-access-from-project-nwe-350x125.png)

   >[!TIP]
   >
   >當Workfront管理員阻止將任務新增到這些專案時，如果所選專案處於未決核准、已完成或無法使用，則會顯示類似訊息。 如需詳細資訊，請參閱 [設定系統範圍的專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. 按一下 **選項** 然後，在左側面板中，取消選取您不想要與任務一起複製的任務屬性。 預設會選取所有選項。

   >[!TIP]
   >
   選取，然後取消選取 **全選** 取消選取所有選項。

   取消選取下列選項，不將它們轉移到複製的工作。 下表說明取消選取選項時會發生什麼情況：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">約束</td> 
      <td> <p>根據專案排程模式設定，任務限制會設定為「儘快」或「儘可能遲」。</p> <p> 選取後，任務的目前限制會轉移到複製的任務。 </p> <p>備註：當將具有日期特定限制的任務移轉或複製到其他專案時，且任務的限制日期在新專案日期以外時，「任務限制」會變更為「儘快」或「儘可能延遲」，或調整專案的「計劃開始日期」或「計畫完成日期」。 日期特定限制的部分範例為必須開始於、必須完成於、開始時間不早於、開始時間不晚於等。 有關任務限制以及任務限制或專案日期如何受到影響的資訊，請參閱 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">任務限制總覽</a> 並尋找特定限制。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">指派</td> 
      <td> <p>所有指派都將從任務中移除。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">核准流程</td> 
      <td>所有核准流程都會從任務中移除。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">進度</td> 
      <td>任務狀態為「新增」。 否則，複製的任務會保留現有任務的狀態。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">財務資訊</td> 
      <td>工作的財務資訊即被移除。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">所有前置任務</td> 
      <td> <p>這表示相依性不會延續到複製的任務。 </p> <p>選取後，會保留複製任務群組內的前置任務，而刪除其他前置任務。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">文件</td> 
      <td> <p>附加到任務的檔案不會轉移到複製的任務。 這包括版本、校樣和連結的檔案。</p> <p>這不包括檔案核准。 複製任務時永遠無法複製檔案核准。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">提醒通知</td> 
      <td>任務提醒不會轉移到複製的任務。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">費用</td> 
      <td>登入任務的費用不會轉移到複製的任務。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">權限</td> 
      <td>Workfront會移除顯示在工作「共用」清單中的所有實體名稱。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">自訂資料</td> 
      <td> <p>自訂欄位的值會被清除，且自訂表單會傳輸到複製的任務。 </p> <p>選取後，自訂欄位的表單和值都會轉移至複製的任務。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

1.  （可選）按一下 **選取父系** 然後，在左側面板中，選取您想要成為所複製任務之父系的目的專案中的任務。

   >[!TIP]
   >
   選取複製清單中的多個任務時，所有選取的任務都會成為選取父系的子系。

   執行下列任一項作業來選取父系：

   * 在任務清單中，選取專案計畫中的父項之一。
   * 按一下搜尋圖示 ![搜尋圖示](assets/search-icon.png) 並按名稱搜尋父系任務。

   任務應出現在清單中。

   ![使用搜尋功能移動任務時選取父系任務 ](assets/select-parent-when-moving-tasks-with-search-functionality-nwe-350x110.png)

1. 找到父項之後，選取父項的選項按鈕。 

   如果您未選取父系任務，任務會作為主要任務而非子任務複製，並放置在目標專案上任務清單的末尾。 

1. 按一下 **複製任務**

   或

   按一下 **複製任務** 當您在清單中選取多個任務時。
複製的任務現在位於指定的專案上，並且是所選父系任務的子任務或專案上的最後一個任務。

## 複製任務

如果您需要相同專案上的相同任務，可以快速複製任務清單中的任務。

* [複製任務的注意事項](#considerations-for-duplicating-tasks)
* [複製任務](#duplicate-tasks)

### 複製任務的注意事項 {#considerations-for-duplicating-tasks}

* 只有在工作清單按工作編號排序時，您才能複製工作清單中的工作。

* 新任務將與原始任務同名。
* 您無法選取哪些資訊會複製到新任務。 根據預設，幾乎所有來自原始任務的資訊都會轉移到複製任務，包括父項關係。
* 下列專案未轉移到新任務：

   * 記錄時數
   * 附註
   * 問題
   * 只有屬於同一組複製任務的前置任務會與其後續任務一起複製。

     **範例：** 例如，如果您同時複製任務2及其前置任務任務1，則會有任務2的副本和任務1的副本。 任務1的副本將是任務2副本的前置任務。 但如果您只複製任務2而沒有複製其前置任務，則其副本將沒有前置任務。

* 當您複製父系任務時，即使未選取子系任務，所有子系任務也會複製。
* 您可以同時複製多個任務。

  不過，您無法同時複製多個非循序的工作。

* 里程碑會移至新任務並從原始任務中移除。

### 複製任務

1. 前往包含您要複製之一或多個任務的專案。
1. 按一下 **任務** 在左側面板中。
1. 執行下列任一項作業：

   * （視條件而定）按一下 **計畫模式功能表** ![](assets/qs-list-mode-or-save-mode-icon-small.png) > **自動儲存**，選取您要複製的任務，然後按一下 **更多選單** ![](assets/qs-more-menu-29x11.png) > **複製**.

     ![](assets/duplicate-tasks-in-list-nwe-350x196.png)

   * （視條件而定）按一下 **計畫模式功能表** ![](assets/qs-list-mode-or-save-mode-icon-small.png) > **手動儲存** > **標準** 或 **時間表規劃**，然後執行下列動作：

      1. 選取要複製的一個或多個任務，然後按一下 **複製**.
      1. （可選）按一下 **還原** 以反轉您的變更而不複製任務。
      1. （選擇性和條件性）按一下 **取消復原** 如果您先前已按一下 **還原**，以保留變更並複製任務。

      1. 按一下 **儲存** 以儲存變更。

   1. 編輯清單中的任務
