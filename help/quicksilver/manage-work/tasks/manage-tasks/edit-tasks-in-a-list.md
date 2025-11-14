---
product-area: projects
navigation-topic: manage-tasks
title: 編輯清單中的任務
description: 您可以編輯工作清單中顯示的欄位，以編輯工作清單中的工作資訊。 您必須在工作清單中定義「計畫模式」，以指示您要將變更儲存至Workfront的方式。 您可以手動或自動儲存變更。
author: Alina
feature: Work Management
exl-id: 2af81907-3657-459e-b780-65983e224ca8
source-git-commit: 8cd6c47acf8de313bab5fe7298125eb63cc10faf
workflow-type: tm+mt
source-wordcount: '2851'
ht-degree: 3%

---

# 編輯清單中的任務 {#edit-tasks-in-a-list}

<!-- Audited: 10/2025 -->

<!--

<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> -->

您可以編輯工作清單中顯示的欄位，以編輯工作清單中的工作資訊。 如需有關編輯工作的其他方式的資訊，請參閱[編輯工作](../../../manage-work/tasks/manage-tasks/edit-tasks.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>標準<p>
   <p>工作或更高</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯任務與專案的存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>貢獻或更高許可權給任務和專案</p></td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++ 

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard<p>
   <p>Current: Work or higher</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks and&nbsp;Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute or higher permissions to the task and the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 編輯清單中任務的相關考量事項 {#considerations-about-editing-tasks-in-a-list}

編輯清單中的任務是一種同時變更多個任務的快速方法，同時可清楚瞭解您的變更可能會如何影響專案時間表。

編輯清單中的任務時，請考量下列事項：

* 與在「編輯」方塊中編輯任務時需要「管理任務許可權」不同，您只能在具有「貢獻任務」許可權的清單中編輯任務。 這可讓您編輯任務的下列有限資訊：

   * 說明
   * 狀態
   * 完成百分比
   * 自訂表格資訊

     >[!NOTE]
     >
     >只有在您具有更新欄位的許可權時，才能編輯清單中的任務自訂欄位。

   * 記錄時數
   * 修改指派
   * 檢視財務資訊
   * 新增費用、任務或問題

* 您可以編輯下列清單中的工作：

   * 專案的任務區段
   * 專案的子任務區段
   * 任務報告

     >[!NOTE]
     >
     >依預設，Workfront會自動將您對任務所做的變更儲存在「子任務」區段或任務報告中。

* 您可以透過在開始編輯任務之前定義「計畫模式」，來控制Workfront何時儲存您對清單中的任務所做的變更。

  您可以透過下列方式，在Workfront儲存您所做的變更之間做出決定：

   * 每次變更後自動
   * 手動，只在您按一下[儲存]之後。

  如需有關在Workfront儲存您對清單中的工作所做的變更時進行設定的資訊，請參閱本文中[編輯清單中的工作之前](#modify-plan-mode-before-editing-tasks-in-a-list)一節的「修改計畫模式」。

* 其他使用者必須先重新整理頁面，才能檢視您對任務所做的更新。

## 在編輯清單中的任務之前修改計畫模式

您可以決定對清單中的工作所做的變更是否會在發生時自動儲存，或者是否要手動儲存每個變更。 若要這麼做，您必須先修改工作清單中的「計畫模式」，才能編輯工作。

>[!IMPORTANT]
>
>根據您是自動或手動儲存任務，當您編輯清單中的任務時，可能會覆寫其他人的資訊。 如需詳細資訊，請參閱[在任務清單中儲存並行變更的概觀](../../../manage-work/tasks/manage-tasks/save-concurrent-changes-in-a-task-list.md)。

針對已選取「自動」或「自動」及「變更時」作為「更新型別」的專案，當您在清單中儲存變更時，Workfront會更新專案時間表，以及所有專案內和跨專案相依性。 如果專案較大或有許多相依性，則時間表計算可能需要很長的時間。 根據您選取來儲存變更的方法，某些編輯任務清單的方法可能比其他方法更快。

您可以控制Workfront何時儲存您對清單中任務所做的變更。 存在下列情況：

* 您可以讓Workfront在每次更新後自動儲存變更。

  如需詳細資訊，請參閱本文中的[設定計畫模式以自動儲存變更](#set-the-plan-mode-to-automatically-save-changes)一節。

* 您可使用「儲存」按鈕手動控制一次套用多個變更的時間。

  如需詳細資訊，請參閱本文中的[設定計畫模式以手動儲存變更](#set-the-plan-mode-to-manually-save-changes)一節。

### 設定計畫模式以自動儲存變更

>[!TIP]
>
>如果您的專案有超過2000個任務或具有大量相依性，儲存您的變更和所有專案相依性可能會較慢。

自動儲存您的工作清單變更時，請考量下列事項：

* 您可以將自訂檢視套用至任務清單，並編輯您有權更新的任何任務相關欄位。
* 您無法回覆自動儲存的變更。 這是預設設定。
* 當專案更新型別為自動或自動且變更時，Workfront會在每次變更後自動重新計算專案的時間表以及所有專案內和跨專案相依性。 如需有關專案更新型別的資訊，請參閱[選取專案更新型別](../../../manage-work/projects/manage-projects/select-project-update-type.md)。

若要編輯清單中的工作並自動儲存變更，請執行下列動作：

{{step1-to-projects}}

1. 在&#x200B;**專案**&#x200B;頁面上，選取專案。
1. 在左側面板中，按一下&#x200B;**工作**&#x200B;區段。

1. 按一下清單頂端的&#x200B;**計畫模式**&#x200B;圖示![計畫模式圖示](assets/plan-mode-icon.png)，並確認已選取&#x200B;**自動儲存**&#x200B;選項。

   ![啟用自動儲存設定](assets/autosave-setting-enabled-quicksilver-task-list-350x308.png)

1. 編輯您有權手動更新的任何欄位。

1. （選擇性）按下&#x200B;**Escape**&#x200B;以取消變更。
1. 在鍵盤上按&#x200B;**Enter** (Windows)或&#x200B;**Return** (Mac)以儲存您對工作與專案時間表所做的變更。
1. （選擇性）用滑鼠右鍵按一下要修改的工作。

   或

   按一下工作名稱右側的&#x200B;**更多**&#x200B;功能表![](assets/more-icon-task-list.png)。

1. （選擇性）從下列選項中選取：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">在新標籤中打開</td> 
      <td>在新的瀏覽器標籤中開啟工作。 </td> 
     </tr> 
          <tr> 
      <td role="rowheader">插入上述任務</td> 
      <td>在選取的工作上方插入工作。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">在下方插入任務</td> 
      <td>在選取的任務下插入任務</td> 
     </tr>
     <tr> 
      <td role="rowheader">編輯</td> 
      <td><p>開啟「編輯任務」方塊，您可以在此編輯任務。</p><p>如需有關編輯任務的資訊，請參閱<a href="#edit-tasks-in-a-list" class="MCXref xref">在清單中編輯任務</a>。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">刪除</td> 
      <td><p>刪除工作。</p><p>如需有關刪除工作的資訊，請參閱<a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">刪除工作</a>。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">縮排</td> 
      <td><p>將工作縮排一個層級。 </p><p>此選項只會在獨立工作上顯示。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">升級</td> 
      <td><p>將任務凸排一個層級。 </p><p>此選項只會在子項任務上顯示。 </p></td> 
     </tr>  
     <tr> 
      <td role="rowheader">複製</td> 
      <td><p>在相同專案中建立任務的重複版本。 </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">複製到...</td> 
      <td><p>將任務複製到另一個專案。</p><p>如需有關複製和複製任務的資訊，請參閱<a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">複製和複製任務</a>。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">移至...</td> 
      <td><p>將任務移至另一個專案。</p><p>如需關於移動任務的資訊，請參閱<a href="../../../manage-work/tasks/manage-tasks/move-tasks.md" class="MCXref xref">移動任務</a>。</p></td> 
     </tr> 
    </tbody> 
   </table>

### 設定計畫模式以手動儲存變更 {#edit-tasks-in-a-list-and-manually-save-changes}

您可以手動儲存對清單中的工作所做的變更。 以這種方式儲存變更時，您有彈性在儲存前將其還原。

>[!TIP]
>
>* 當您在「子任務」區段或任務報告中編輯清單中的任務時，無法反轉對這些任務所做的變更。
>* 您可以回覆的變更數量沒有限制。 您可以逐一反轉所有任務，直到達到任務的原始狀態。
>

手動將變更儲存在工作清單中時，請考量下列事項：

* 為了手動儲存任務清單變更，您需要管理任務和專案的許可權。
* 您無法編輯專案。 編輯專案的選項已停用。
* 您無法更新專案標頭中的資訊。 您只能在手動儲存工作清單中的變更時執行下列動作：

   * 訂閱專案。
   * 將專案新增至您的最愛清單。
   * 按一下清單中的任務名稱以開啟任務。

* 大量編輯工作。 選取多個任務時，「編輯」圖示會停用。
* Workfront只有在您儲存變更後，才會觸發您對工作進行變更的通知。

有2種方式可手動儲存清單中任務的變更：

* [當您選取[手動儲存標準]選項時，手動儲存工作清單中的變更](#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-standard-option)
* [當您選取「手動儲存時程表計畫」選項時，手動儲存工作清單中的變更](#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-timeline-planning-option)

#### 選取「手動儲存標準」選項時，手動儲存工作清單中的變更 {#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-standard-option}

>[!TIP]
>
>如果您的專案有超過2000個任務，或如果它有許多相依性，則可能需要一段時間才能直觀地識別您對任務所做的變更，以及這些變更如何影響所有專案相依性。 在此情況下，儲存您的變更可能需要比預期更長的時間。

選取「手動儲存標準」選項後，更新清單中的任務時，請考量下列事項：

* 您可以將自訂檢視套用至任務清單，並編輯您有權在該檢視中管理的任何任務相關欄位。
* 當專案「更新型別」為「自動」或「自動」且「變更時」時，Workfront會在您按一下「儲存」後計算專案的時間表，以及專案內和跨專案的所有相依性。 如需有關專案更新型別的資訊，請參閱[選取專案更新型別](../../../manage-work/projects/manage-projects/select-project-update-type.md)。

若要在選取「手動儲存標準」選項時編輯清單中的工作：

{{step1-to-projects}}

1. 在&#x200B;**專案**&#x200B;頁面上，選取專案。

1. 在左側面板中，按一下&#x200B;**工作**&#x200B;區段。

1. 按一下清單頂端的&#x200B;**計畫模式**&#x200B;圖示![計畫模式圖示](assets/plan-mode-icon.png)。

1. 在&#x200B;**計畫模式**&#x200B;對話方塊中，選取&#x200B;**手動儲存**，然後按一下&#x200B;**標準**。

   ![啟用手動儲存設定](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. 按一下&#x200B;**套用**。 此時會顯示工具列設定，其中包含還原、重做和儲存變更的選項。

   ![手動儲存工具列](assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png)

1. 按一下您有權手動更新的任何欄位。 欄位會變成可編輯，您可以進行變更。

1. 在鍵盤上按&#x200B;**Enter** (Windows)或&#x200B;**Return** (Mac)以暫時儲存您所做的變更。

1. （選擇性）按一下&#x200B;**復原**&#x200B;圖示![復原圖示](assets/undo-icon-on-task-list.png)來回覆變更，並將欄位恢復為原始狀態。

1. （選擇性和條件性）按一下&#x200B;**重做**&#x200B;圖示![重做圖示](assets/redo-icon-on-task-list.png)，還原您回覆的變更。

1. （選擇性）用滑鼠右鍵按一下要修改的工作。

   或

   按一下&#x200B;**更多**&#x200B;功能表![](assets/more-icon-task-list.png)。

1. （選擇性）從下列選項中選取：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">在新標籤中打開</td> 
      <td>在新的瀏覽器標籤中開啟工作。 </td> 
     </tr> 
          <tr> 
      <td role="rowheader">插入上述任務</td> 
      <td>在選取的工作上方插入工作。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">在下方插入任務</td> 
      <td>在選取的任務下插入任務</td> 
     </tr> 
     <tr> 
      <td role="rowheader">刪除</td> 
      <td>如需有關刪除工作的資訊，請參閱<a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">刪除工作</a>。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">縮排</td> 
      <td> <p>將工作縮排一個層級。 </p> <p>此選項只會在獨立工作上顯示。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">升級</td> 
      <td> <p>將任務凸排一個層級。 </p> <p>此選項只會在子項任務上顯示。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">複製</td> 
      <td> <p>在相同專案中建立任務的重複版本。 </p> <p>如需有關複製和複製任務的資訊，請參閱<a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">複製和複製任務</a>。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 當您變更任務的時間表時，Workfront會更新所有專案內和跨專案相依性。
1. 當您想要永久保留工作變更並儲存專案的時間表時，請按一下[儲存]。****

#### 當您選取「手動儲存時程表計畫」選項時，手動儲存工作清單中的變更 {#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-timeline-planning-option}

儲存您的變更和所有專案相依性會更快速。 這不適用於具有超過2000個任務的專案。

>[!IMPORTANT]
>
>建議您在編輯數百個以上且有許多相依性的大型任務清單時，使用此選項。 使用此選項可讓您以視覺化方式識別變更，比使用手動儲存選項快得多。

在工作清單中使用「手動儲存時程表計畫」選項時，請考量下列事項：

* 您無法將「手動儲存時間表計畫」選項套用至具有超過2000個任務的專案。
* 您無法將自訂檢視、篩選或分組套用至工作清單。 「檢視」、「篩選」和「群組」下拉式功能表，以及「敏捷檢視」圖示都會停用。 依預設套用的檢視包含有限數目的欄位。
* 當專案的「更新型別」為「自動」或「自動」且「變更時」時，每次變更後會自動計算專案的時間表和所有專案內的相依性。
* 當專案更新型別為「自動」或「自動」且「變更時」時，會在您按一下「儲存」後計算跨專案相依性。 如需有關專案更新型別的資訊，請參閱[選取專案更新型別](../../../manage-work/projects/manage-projects/select-project-update-type.md)。

若要在使用「手動儲存時間表規劃」選項時編輯清單中的工作：


{{step1-to-projects}}

1. 在&#x200B;**專案**&#x200B;頁面上，選取專案。

1. 在左側面板中，按一下&#x200B;**工作**&#x200B;區段。

1. 按一下清單頂端的&#x200B;**計畫模式**&#x200B;圖示![計畫模式圖示](assets/plan-mode-icon.png)。

1. 在&#x200B;**計畫模式**&#x200B;對話方塊中，選取&#x200B;**手動儲存**，然後按一下&#x200B;**時間表計畫**。

   ![套用時間表規劃設定](assets/manual-timeline-planning-setting-enabled-quicksilver-task-list-350x490.png)

   >[!TIP]
   >
   >超過2000個任務的專案的&#x200B;**時間計畫**&#x200B;選項會變暗。

1. 按一下&#x200B;**套用**。

   清單中會發生下列變更：

   * 「檢視」、「群組」和「篩選」下拉式功能表已移除，且檢視由下列欄位取代：

      * 任務編號
      * 任務名稱
      * 限制類型
      * 期間
      * 規劃開始日期
      * 規劃完成日期
      * 前置任務
      * 指派
      * 狀態
      * 完成百分比

   * 敏捷檢檢視示已移除。
   * 此時會顯示工具列設定，其中包含還原、重做和儲存變更的選項。

     ![手動儲存工具列](assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png)

1. 編輯您有權手動更新的任何欄位。

1. 在鍵盤上按&#x200B;**Enter** (Windows)或&#x200B;**Return** (Mac)以暫時儲存您所做的變更。
1. （選擇性）按一下&#x200B;**復原**&#x200B;圖示![復原圖示](assets/undo-icon-on-task-list.png)來回覆變更，並將欄位恢復為原始狀態。
1. （選擇性和條件性）按一下&#x200B;**重做**&#x200B;圖示![重做圖示](assets/redo-icon-on-task-list.png)以復原您回覆的變更。

1. （選擇性）用滑鼠右鍵按一下要修改的工作。

   或

   按一下&#x200B;**更多**&#x200B;功能表![](assets/more-icon-task-list.png)。

1. 從下列選項中選取：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">在新標籤中打開</td> 
      <td>在新的瀏覽器標籤中開啟工作。 </td> 
     </tr> 
          <tr> 
      <td role="rowheader">插入上述任務</td> 
      <td>在選取的工作上方插入工作。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">在下方插入任務</td> 
      <td>在選取的任務下插入任務</td> 
     </tr> 
     <tr> 
      <td role="rowheader">刪除</td> 
      <td>如需有關刪除工作的資訊，請參閱<a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">刪除工作</a>。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">縮排</td> 
      <td> <p>將工作縮排一個層級。 </p> <p>此選項只會在獨立工作上顯示。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">升級</td> 
      <td> <p>將任務凸排一個層級。 </p> <p>此選項只會在子項任務上顯示。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">複製</td> 
      <td> <p>在相同專案中建立任務的重複版本。 </p> <p>如需有關複製和複製任務的資訊，請參閱<a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">複製和複製任務</a>。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 當您變更任務的時間表時，Workfront會更新所有專案內和跨專案相依性。
1. 當您想要永久保留工作變更並儲存專案的時間表時，請按一下[儲存]。****

## 使用「摘要」編輯清單中的任務

{{step1-to-projects}}

1. 在&#x200B;**專案**&#x200B;頁面上，選取專案。

1. 在左側面板中，按一下&#x200B;**工作**&#x200B;區段。 專案上的任務清單隨即顯示。

1. 選取您要編輯的工作，然後按一下清單右上角的&#x200B;**開啟摘要**&#x200B;圖示![開啟摘要圖示](assets/task-summary-icon.png)。 **任務摘要**&#x200B;面板隨即開啟。

1. （選擇性）在&#x200B;**更新**&#x200B;區域輸入工作的更新。
1. 按一下下列任一圖示或區域，移至工作並編輯工作層次的資訊：

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">文件</td> 
      <td>將檔案新增至工作。 </td> 
     </tr> 
          <tr> 
      <td role="rowheader">自訂表單</td> 
      <td>新增或移除自訂表格，或更新表格上的資訊。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">時數</td> 
      <td>記錄時數。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">核准</td> 
      <td>新增任務核准。</td> 
     </tr> 
     <tr> 
    </tbody> 
   </table>

1. 按一下面板右上角的&#x200B;**X**&#x200B;以將其關閉。

## 大量編輯任務

您可以一次編輯多個任務。 確保您擁有工作的管理許可權以便編輯。

{{step1-to-projects}}

1. 在&#x200B;**專案**&#x200B;頁面上，選取專案。
1. 在左側面板中，按一下&#x200B;**工作**&#x200B;區段。

1. 按一下清單頂端的&#x200B;**計畫模式**&#x200B;圖示![計畫模式圖示](assets/plan-mode-icon.png)，並確認已選取&#x200B;**自動儲存**&#x200B;選項。

   ![啟用自動儲存設定](assets/autosave-setting-enabled-quicksilver-task-list-350x308.png)

   >[!IMPORTANT]
   >
   >手動儲存任務時，您無法大量編輯任務。

1. 在工作清單中選取多個工作。
1. （選擇性）按一下工作清單頂端的&#x200B;**更多**&#x200B;功能表![更多功能表](assets/more-icon.png)，然後&#x200B;**重新計算運算式**&#x200B;以更新計算自訂欄位中的所有資訊。
1. 按一下&#x200B;**編輯**&#x200B;圖示![編輯圖示](assets/qs-edit-icon.png)。 **編輯任務**&#x200B;對話方塊會在新體驗中開啟。

   編輯所有任務的資訊與編輯一個任務的資訊相同。

   如需編輯工作的詳細資訊，請參閱[編輯工作](../../../manage-work/tasks/manage-tasks/edit-tasks.md)。

1. （視條件而定）在新體驗中，執行下列動作：

   1. 指定您要在下列任一區域變更所有所選工作的資訊：

      * 概觀
      * 指派
      * 自訂表單
      * 財務
      * 設定
      * 設定
      * 評論

      >[!NOTE]
      >
      >* 您正在所有選取的任務上變更的資訊將會覆寫個別任務（**工作總攬**&#x200B;欄位除外）的現有資訊。 在大量編輯中新增受指派人，會將該受指派人新增至所有選取的任務。 如果將其他受指派人指派給所選任務，則除了透過大量編輯新增的受指派人外，受指派人將維持受指派狀態。
      >* 如果您想要編輯任務「工期」，則選取的任務必須具有相同的任務限制。 否則，**持續時間**&#x200B;欄位不會填入。
      >
      >* 清單中只會顯示作用中的自訂表單。 如果所選的任務沒有任何常見的自訂表格，則本節不會列出任何表格。
      >* 您只能在表單上編輯附加到所有選定任務且您有權編輯的欄位。  如需大量編輯自訂表單的相關資訊，請參閱[管理附加到物件的自訂表單](../../../workfront-basics/work-with-custom-forms/manage-custom-forms-attached-to-objects.md)。

   1. 按一下「**儲存**」。
   1. （選擇性）按一下&#x200B;**編輯工作**&#x200B;方塊底部的&#x200B;**切換回舊體驗**。

1. （視條件而定）在舊體驗中，執行下列動作：

   1. 指定您要在下列任一區域變更所有所選工作的資訊：

      * 概觀
      * 設定
      * 指派
      * 自訂表單
      * 評論

   1. （選擇性）在&#x200B;**自訂Forms**&#x200B;區段中，選取&#x200B;**重新計算自訂運算式**&#x200B;選項，以確保附加到所選工作的自訂表單上的所有計算自訂欄位都是最新的。
   1. 按一下&#x200B;**儲存變更**。 您所做的所有變更現在會顯示在所有選取的任務中。

