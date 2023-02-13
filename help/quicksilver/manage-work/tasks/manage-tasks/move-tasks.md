---
product-area: projects
navigation-topic: manage-tasks
title: 移動任務
description: 您可以在Adobe Workfront中將工作移至不同專案或不同的父任務。
author: Alina
feature: Work Management
exl-id: 93295d70-a6cf-46ca-b621-228fa6c983f5
source-git-commit: 23a08c929b0a227c7a555af70ff731ef2df7a179
workflow-type: tm+mt
source-wordcount: '1360'
ht-degree: 2%

---

# 移動任務

您可以在下列物件之間移動Adobe Workfront中的工作：

* 專案的臨機任務。
* 從項目到另一個項目的任務。
* 另一個專案中不同父項下專案的任務。
* 同一項目內不同父項下的任務。

您可以在任務層移動任務，也可以從任務清單中移動任務。

## 存取需求

您必須具備下列存取權，才能執行本文中的動作：

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
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對任務和項目的訪問</p> <p><b>附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理任務權限</p> <p>為專案貢獻或更高權限，並能新增工作</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 在清單中移動任務

要移動任務清單中顯示的任務，請執行以下操作：

1. 轉到包含要移動的任務或任務的項目。
1. 按一下 **工作** 顯示任務清單。
1. 確保 **自動儲存** 切換為啟用，然後選擇要移動的任務或任務。

   ![](assets/autosave-icon-on-highlighted-350x202.png)

   >[!IMPORTANT]
   >
   >當 **自動儲存** 切換為已停用。

1. （可選和條件性）如果要移動同一項目中選定的任務，請按一下您選擇的任務，將它們拖放到您希望在項目中移動的位置。

   將任務放置在項目上正確的位置後，您對任務層次結構所做的更改將立即保存。 與每個任務相關聯的所有資訊都與任務一起移動。

1. （條件性）選擇要移動的任務或任務，並執行以下操作之一：

   * 按一下 **更多** 功能表 ![](assets/qs-more-menu.png) 在任務清單頂端，按一下 **移至**.
   * 以滑鼠右鍵按一下選取的任務，然後按一下 **移至**.
   * 選取一個任務時，按一下 **更多** 功能表 ![](assets/more-icon-task-list.png) 在清單中的任務名稱旁邊，然後按一下 **移至**.

   ![](assets/move-task-in-list-nwe-350x119.png)

   移動任務框隨即顯示

1. 繼續移動任務，如一節中所述 [在任務層移動任務](#move-a-task-at-the-task-level) 在本文中，從步驟4開始。

   <!--
   is this still accurate?!
   -->

## 在任務層移動任務 {#move-a-task-at-the-task-level}

除了從任務清單中移動任務外，還可以在開啟任務後在任務級別移動任務。 

1. 在您的Workfront系統中搜尋任務，以尋找該任務。
1. 按一下任務的名稱以開啟它。
1. 按一下 **更多** 下拉式功能表 ![](assets/qs-more-menu.png) 在任務名稱旁，按一下 **移至**. 「移動任務」框隨即顯示。

   ![](assets/move-task-at-task-level-nwe-350x222.png)

1. （選用）更新 **任務名稱**. 任務在新位置中以新名稱移動。 Workfront不會記錄任務的原始名稱。

   >[!TIP]
   >
   >選擇在清單中移動多個任務時，此欄位呈灰色且不可編輯。 您可以暫留在「任務名稱」欄位上，並顯示所有選定任務的清單。
   >
   >
   >![](assets/move-task-multiple-tasks-box-with-list-of-task-names-nwe-350x142.png)

1. 輸入 **目的地專案** 在 **選擇目標項目** 欄位。

   如果要移動同一項目中的任務，請輸入當前項目的名稱。

   >[!TIP]
   >
   >* 專案名稱區分大小寫。
   >* 您也可以開始輸入參考編號或輸入專案ID。 這可協助您區分名稱相同的專案。
   >* 清單中只會顯示100個專案。


1. （有條件）按一下 **要求存取** 若要請求專案的存取權，請先確認您沒有所選專案的存取權。
1. （條件性）如果您有權將任務添加到目標項目上的任務之一，則繼續將任務移動到所選目標項目，而不請求訪問權。

   ![](assets/move-task-request-access-from-project-nwe-350x120.png)

   >[!TIP]
   >
   >如果所選專案處於待核准、已完成或已結束狀態，當Workfront管理員防止將任務新增至這些專案時，則會顯示類似的訊息。 如需詳細資訊，請參閱 [配置系統範圍的項目首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. （選用）按一下 **選項** 在左側面板中

   或

   向下捲動至 **選項** ，然後取消選取下表中列出的任何項目，以從移動的任務中移除這些項目。 預設會選取所有選項。

   >[!IMPORTANT]
   取消選取「選項」清單中的項目會導致資料遺失。 將刪除來自現有任務的資訊，且無法恢復。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">全選</td> 
      <td>取消選擇此選項可在將任務移動到新位置時從任務中刪除所有資訊。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">約束</td> 
      <td> <p>根據「項目計畫模式」設定，任務約束將設定為「盡快」或「盡可能晚」。</p> <p> 選定後，任務的當前約束將隨任務轉移。 </p> 
      <p><b>附註</b>

   將具有日期特定約束的任務移動或複製到另一個項目時，如果任務的約束日期在新項目的日期之外，則任務約束將更改為「盡快」或「盡快延遲」，或調整項目的計劃開始或計畫完成日期。

   以下是日期特定限制的範例：
   <ul>
      <li> 開始日期</li>
      <li> 必須完成時間</li>
      <li> 開始時間不早於</li>
      <li> 開始時間不晚於</li>
      </ul>

   有關任務約束以及如何影響任務約束或項目日期的資訊，請參閱 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">任務約束概覽</a> 並尋找特定的限制。</p> </td>
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
      <td>任務狀態為「新建」。 否則，將保留現有任務狀態。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">財務資訊</td> 
      <td>任務的財務資訊將被刪除，Workfront會將任務成本類型更新為「無成本」，並將任務收入類型更新為「不可開單」。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">所有前置任務</td> 
      <td> <p>選中後，當將任務移動到另一個項目時，相依性將成為跨項目的前置項。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">文件</td> 
      <td> <p>附加到任務的文檔不會轉移到移動的任務。 這包括版本、校樣和連結的檔案。</p> <p>這不包括文檔批准。 移動任務時，無法移動文檔批准。</p> 
      <b>附註</b>

   如果您選擇不隨任務移動文檔，則文檔將被刪除並放入資源回收筒30天。 管理員可以還原它們，並在移動的任務中還原它們。

   如果任務在移動後被刪除，則恢復的文檔將放置在恢復任務的管理員用戶頁的「文檔」區域中。

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">提醒通知</td> 
      <td>任務提醒不會轉移到移動的任務。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">費用</td> 
      <td>記錄在任務上的費用不會轉移到移動的任務。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">權限</td> 
      <td> <p>Workfront會移除任務「共用」清單中顯示之所有實體的名稱。 </p> </td> 
     </tr> 
    </tbody> 
   </table>



1. （選用）按一下 **選擇父級** 在左側面板中

   或

   捲動至 **選擇父級** 節，然後選擇目標項目中要成為移動任務父項的任務。

   >[!TIP]
   選擇在清單中移動多個任務時，所有選定任務都將成為選定父項的子項。

   通過執行以下操作之一選擇父級：

   * 在任務清單中，選擇項目計畫中的父項之一。
   * 按一下搜尋圖示 ![搜尋圖示](assets/search-icon.png) 並按名稱搜索父任務。

   任務應出現在清單中。

   ![使用搜索功能移動任務時選擇父任務 ](assets/select-parent-when-moving-tasks-with-search-functionality-nwe-350x110.png)

1. 找到父級的單選按鈕後，選擇該單選按鈕。

   如果未選擇父任務，則任務將作為主任務而非子任務移動，並且這些任務將放在目標項目上的任務清單的末尾。

1. 按一下 **移動任務**

   或

   按一下 **移動任務** 在清單中選擇多個任務時。
移動的任務現在位於指定的項目上，並且是父任務的子任務或項目上的最後一個任務。
