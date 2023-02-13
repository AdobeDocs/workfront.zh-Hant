---
product-area: projects
navigation-topic: manage-tasks
title: 複製和複製任務
description: 您可以將一個任務從一個項目複製到另一個項目，也可以在同一個項目中複製一個任務。
author: Alina
feature: Work Management
exl-id: daf89062-cf58-4c39-83ff-727d969a9630
source-git-commit: 23a08c929b0a227c7a555af70ff731ef2df7a179
workflow-type: tm+mt
source-wordcount: '1670'
ht-degree: 1%

---

# 複製和複製任務

您可以將一個任務從一個項目複製到另一個項目，也可以在同一個項目中複製一個任務。

您可以一次複製或複製一或多個任務或父任務。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td> <p>工作或更高 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對任務和項目的訪問</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理任務的權限 </p> <p>為專案貢獻或更高權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 複製任務的考量事項

複製任務時，請考量下列事項：

* 不會隨任務複製問題。
* 里程碑會轉移到複製的任務，並從原始任務中刪除。

您可以複製Adobe Workfront Web應用程式下列區域中的任務：

* 在任務層級，從 **更多圖示** ![](assets/qs-more-menu-19x7.png) 的右側。

   如需詳細資訊，請參閱 [在任務級別複製任務](#copy-a-task-at-the-task-level) 一節。

* 在任務清單中，通過執行以下操作之一：

   * 以滑鼠右鍵按一下任務的名稱。
   * 選擇任務（或任務）並展開 **更多** 圖示 ![](assets/more-icon-task-list.png) 在任務清單的頂部。
   * 選擇任務並展開 **更多** 圖示 ![](assets/more-icon-task-list.png) 在任務名稱旁邊。

      選擇多個任務時，此選項不可用。
   如需詳細資訊，請參閱 [複製清單中的任務](#copy-tasks-in-a-list) 一節。

## 複製清單中的任務 {#copy-tasks-in-a-list}

1. 轉到包含要複製的任務或任務的項目。

   或

   轉到任務報告。

1. 按一下 **工作** 中。
1. 按一下 **計畫模式菜單** ![](assets/qs-list-mode-or-save-mode-icon-small.png) ，然後 **自動儲存**.

   >[!IMPORTANT]
   >
   >只有在自動保存更改時，才能複製清單中的任務。 有關在編輯任務時保存選項的資訊，請參閱 [編輯清單中的任務](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

1. 選擇要複製的任務或任務，然後執行以下操作之一：

   * 按一下 **更多功能表** 在任務清單頂端，按一下 **複製到**.
   * 以滑鼠右鍵按一下選取的任務，然後按一下 **複製到**.
   * 選取一個任務時，按一下 **更多** 功能表 ![](assets/more-icon-task-list.png) 在清單中的任務名稱旁邊，然後按一下 **複製到**.
   ![](assets/copy-task-in-list-nwe-350x131.png)

1. 繼續複製任務，如一節所述 [在任務級別複製任務](#copy-a-task-at-the-task-level) 從步驟4開始。

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: is this still accurate?!)
   </MadCap:conditionalText>
   -->

## 在任務級別複製任務 {#copy-a-task-at-the-task-level}

除了複製任務清單中的任務之外，還可以在開啟任務後複製任務。 

1. 在您的Workfront系統中搜尋任務，以尋找該任務。
1. 按一下任務的名稱以開啟它。 
1. 按一下 **更多** 下拉式功能表 ![](assets/qs-more-menu.png) 在任務名稱旁，按一下 **複製** **to**.

   ![](assets/taskcopy-to-at-the-task-level-nwe-350x200.png)

   「複製任務」框隨即顯示。

1. （選用）更新 **任務名稱**.

   >[!TIP]
   >
   >選擇複製清單中的多個任務時，此欄位呈暗灰色且不可編輯。 您可以暫留在「任務名稱」欄位上，並顯示所有選定任務的清單。
   >
   >![](assets/copy-task-multiple-tasks-box-with-list-of-task-names-nwe-350x130.png)

1. 輸入 **目的地專案** 要複製 **選擇目標項目** 欄位。 

   >[!TIP]
   >
   >* 專案名稱區分大小寫。
   >* 您也可以開始輸入參考編號或輸入專案ID。 這可協助您區分名稱相同的專案。
   >* 清單中只會顯示100個專案。


   預設會顯示目前的專案名稱。 如果要複製同一項目中的任務，請將此欄位保持不變。

1. （有條件）按一下 **請求存取** 若要請求專案的存取權，請先確認您沒有所選專案的存取權。
1. （條件性）如果您有權將任務添加到目標項目上的任務之一，則繼續將任務複製到所選目標項目，而不請求訪問權。

   ![](assets/copy-task-request-access-from-project-nwe-350x125.png)

   >[!TIP]
   >
   >如果所選專案處於待核准、已完成或已結束狀態，當Workfront管理員防止將任務新增至這些專案時，則會顯示類似的訊息。 如需詳細資訊，請參閱 [配置系統範圍的項目首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. 按一下 **選項** 在左側面板中，取消選擇您不想隨任務一起複製的任務屬性。 預設會選取所有選項。

   >[!TIP]
   選取然後取消選取 **全選** 取消選取所有選項。

   取消選取下列選項，以不將它們轉移至複製的任務。 下表說明取消選取選項後會發生什麼情況：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">約束</td> 
      <td> <p>根據「項目計畫模式」設定，任務約束將設定為「盡快」或「盡可能晚」。</p> <p> 選定後，任務的當前約束將轉移到複製的任務。 </p> <p>注意：將具有日期特定約束的任務移動或複製到另一個項目時，如果任務的約束日期在新項目的日期之外，則任務約束將更改為「盡快」或「盡快延遲」，或調整項目的計劃開始或計畫完成日期。 某些日期特定限制的範例必須開始、必須結束、開始時間不早於、開始時間不晚於等。 有關任務約束以及如何影響任務約束或項目日期的資訊，請參閱 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">任務約束概覽</a> 並尋找特定的限制。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">指派</td> 
      <td> <p>所有分配都從任務中刪除。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">核准流程</td> 
      <td>所有批准過程都將從任務中刪除。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">進度</td> 
      <td>任務狀態為「新建」。 否則，複製的任務將保留現有任務的狀態。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">財務資訊</td> 
      <td>任務的財務資訊被刪除。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">所有前置任務</td> 
      <td> <p>這表示相依性不會繼續保留至複製的工作。 </p> <p>選中後，將保留複製任務組中的前置任務，刪除其他任務。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">文件</td> 
      <td> <p>附加到任務的文檔不會轉移到複製的任務。 這包括版本、校樣和連結的檔案。</p> <p>這不包括文檔批准。 複製任務時，不能複製文檔批准。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">提醒通知</td> 
      <td>任務提醒不會轉移到複製的任務。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">費用</td> 
      <td>記錄在任務上的費用不會轉移到複製的任務。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">權限</td> 
      <td>Workfront會移除任務「共用」清單中顯示之所有實體的名稱。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">自訂資料</td> 
      <td> <p>系統會清除自訂欄位的值，並將自訂表單傳輸至複製的任務。 </p> <p>選取後，自訂欄位的表單和值都會轉移至複製的任務。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

1.  （選用）按一下 **選擇父級** 在左側面板中，選擇目標項目中要成為複製任務父項的任務。

   >[!TIP]
   選擇在清單中複製多個任務時，所有選定任務都將成為選定父項的子項。

   通過執行以下操作之一選擇父級：

   * 在任務清單中，選擇項目計畫中的父項之一。
   * 按一下搜尋圖示 ![搜尋圖示](assets/search-icon.png) 並按名稱搜索父任務。
   任務應出現在清單中。

   ![使用搜索功能移動任務時選擇父任務 ](assets/select-parent-when-moving-tasks-with-search-functionality-nwe-350x110.png)

1. 找到父級的單選按鈕後，選擇該單選按鈕。 

   如果未選擇父任務，則這些任務將作為主任務而非子任務複製，並將放在目標項目上的任務清單的末尾。 

1. 按一下 **複製任務**

   或

   按一下 **複製任務** 在清單中選擇多個任務時。
複製的任務現在位於指定的項目上，並且是選定父任務的子任務或項目上的最後一個任務。

## 複製任務

如果在同一個項目上需要相同的任務，可以快速將任務複製到任務清單中。

* [複製任務的考量事項](#considerations-for-duplicating-tasks)
* [複製任務](#duplicate-tasks)

### 複製任務的考量事項 {#considerations-for-duplicating-tasks}

* 只有在按任務編號排序清單時，才能在任務清單中複製任務。

* 新任務的名稱將與原始任務相同。
* 無法選擇要複製到新任務的資訊。 預設情況下，原始任務中的幾乎所有資訊都將傳輸到重複任務，包括父關係。
* 下列項目不會轉移到新任務：

   * 記錄時數
   * 附註
   * 問題
   * 只有同一組複製任務中的前置任務也會隨其後續任務一起複製。

      **範例：** 例如，如果您同時複製任務2及其前身任務1，則您將有任務2的副本和任務1的副本。 任務1的副本將是任務2的前身。 但是，如果您只複製任務2而不複製其前身，則其副本將沒有前身。

* 複製父任務時，即使未選擇子任務，所有子任務也會重複。
* 您可以同時複製多個任務。

   但是，不能同時複製多個不是循序的任務。

* 里程碑會移至新任務，並從原始任務中移除。

### 複製任務

1. 轉到包含要複製的任務或任務的項目。
1. 按一下 **工作** 中。
1. 執行下列任一項作業：

   * （條件性）按一下 **計畫模式菜單** ![](assets/qs-list-mode-or-save-mode-icon-small.png) > **自動儲存**，選取您要複製的任務，然後按一下 **更多功能表** ![](assets/qs-more-menu-29x11.png) > **複製**.

      ![](assets/duplicate-tasks-in-list-nwe-350x196.png)

   * （條件性）按一下 **計畫模式菜單** ![](assets/qs-list-mode-or-save-mode-icon-small.png) > **手動儲存** > **標準** 或 **時間表規劃**，然後執行下列動作：

      1. 選擇要複製的任務，然後按一下 **複製**.
      1. （選用）按一下 **還原** 來還原變更，而不複製工作。
      1. （選用和條件式）按一下 **取消復原** 如果您先前曾點按過 **還原**，以保留變更並複製工作。

      1. 按一下 **儲存** 來儲存變更。
   1. 編輯清單中的任務
