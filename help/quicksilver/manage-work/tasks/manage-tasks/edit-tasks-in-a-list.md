---
product-area: projects
navigation-topic: manage-tasks
title: 編輯清單中的任務
description: 通過編輯清單中顯示的欄位，可以編輯任務清單中的任務資訊。 有關編輯任務的其他方法的資訊，請參閱編輯任務。
author: Alina
feature: Work Management
exl-id: 2af81907-3657-459e-b780-65983e224ca8
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '2828'
ht-degree: 2%

---

# 編輯清單中的任務 {#edit-tasks-in-a-list}

通過編輯清單中顯示的欄位，可以編輯任務清單中的任務資訊。 有關編輯任務的其他方法的資訊，請參閱 [編輯任務](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

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
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對任務和項目的訪問</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>為任務和項目貢獻或更高權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 關於編輯清單中任務的考量事項 {#considerations-about-editing-tasks-in-a-list}

在清單中編輯任務是同時更改多個任務的快速方法，可以清楚地查看更改對項目時間軸的影響。

編輯清單中的任務時，請考量下列事項：

* 與在「編輯」框中編輯任務時需要管理權限不同，您只能使用任務的「貢獻」權限編輯清單中的任務。 這允許您編輯任務的以下有限資訊：

   * 說明
   * 狀態
   * 完成百分比
   * 自訂表單資訊

      >[!NOTE]
      >
      >只有具有更新欄位的權限時，才能編輯清單中的任務自定義欄位。

   * 記錄時數
   * 修改分配
   * 查看財務資訊
   * 添加費用、任務或問題

* 您可以在下列清單中編輯任務：

   * 項目的「任務」部分
   * 專案的子任務區段
   * 任務報告

      >[!NOTE]
      >
      >依預設，Workfront會自動將您對子任務區段或任務報表中的任務所做的變更儲存。

* 您可以控制Workfront何時將您對清單中的任務所做的變更儲存。 您的變更可以自動儲存，或手動儲存。

   如需有關在Workfront儲存您對清單中的任務所做變更時進行設定的資訊，請參閱 [在編輯清單中的任務時選擇保存選項](#select-a-save-option-when-editing-tasks-in-a-list) 一節。

## 在編輯清單中的任務時選擇保存選項 {#select-a-save-option-when-editing-tasks-in-a-list}

您可以決定對清單中的任務所做的變更會在發生時自動儲存，或是要手動儲存每項變更時自動儲存。

>[!IMPORTANT]
>
>根據您是自動還是手動保存任務，在編輯清單中的任務時可能會覆蓋其他人的資訊。 如需Workfront如何儲存您與其他使用者同時執行之工作的變更的詳細資訊，請參閱 [在任務清單中保存併發更改的概述](../../../manage-work/tasks/manage-tasks/save-concurrent-changes-in-a-task-list.md).

在已選擇「自動」或「自動」和「更改時」作為「更新類型」的項目清單中保存更改時，Workfront會更新項目時間軸，以及所有項目內和跨項目依賴項。 如果項目很大或有大量依賴項，時間軸計算可能需要很長的時間。 某些編輯任務清單的方法可能比其他方法更快，具體取決於您選擇的保存更改的方法。

您可以控制Workfront何時將您對清單中的任務所做的變更儲存。 存在下列情況： 

* 您可以在每次更新後，讓Workfront自動儲存變更。

   如需詳細資訊，請參閱 [編輯清單中的任務並自動保存更改](#edit-tasks-in-a-list-and-automatically-save-changes) 這篇文章。

* 您可以透過手動使用「儲存」按鈕，控制一次套用多項變更的時間。

   如需詳細資訊，請參閱 [編輯清單中的任務並手動保存更改](#edit-tasks-in-a-list-and-manually-save-changes) 這篇文章。

### 編輯清單中的任務並自動保存更改 {#edit-tasks-in-a-list-and-automatically-save-changes}

>[!TIP]
>
>如果您的專案有2000多個工作，或有許多相依性，儲存變更和所有專案相依性可能會變慢。

自動保存任務清單更改時，請考慮以下事項：

* 您可以將自定義視圖應用到任務清單，並編輯您有權更新的任何任務相關欄位。
* 無法反轉自動儲存的變更。 這是預設設定。
* Workfront會在每次變更後，當專案更新類型為「自動」或「自動」和「隨時變更」時，自動重新計算專案時間軸以及所有專案內和跨專案相依性。 有關項目更新類型的資訊，請參閱 [選擇項目更新類型](../../../manage-work/projects/manage-projects/select-project-update-type.md).

要編輯清單中的任務並自動保存更改，請執行以下操作：

1. 前往專案，然後按一下 **工作** 區段。
1. 按一下 **計畫模式菜單** ![](assets/qs-list-mode-or-save-mode-icon-small.png) 並確認 **自動儲存** 選項。

   ![](assets/autosave-setting-enabled-quicksilver-task-list-350x308.png)

1. 編輯您擁有手動更新權限的任何欄位。

   ![](assets/inline-editing-a-task-350x26.png)

1. （可選）按 **逸出** 來取消變更。
1. 按Enter鍵保存對任務和項目時間軸所做的更改。
1. （選用）以滑鼠右鍵按一下您要修改的任務。

   或

   按一下 **更多** 功能表 ![](assets/more-icon-task-list.png) 的右側。

1. （選用）從下列選項中選取：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>在新索引標籤中開啟</strong></td> 
      <td>在新瀏覽器頁簽中開啟任務。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>編輯</strong></td> 
      <td><p>開啟 <strong>編輯任務</strong> 框中，可在其中編輯任務。</p><p>有關編輯任務的資訊，請參閱 <a href="#edit-tasks-in-a-list" class="MCXref xref">編輯清單中的任務</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">刪除</td> 
      <td><p>刪除任務。</p><p>有關刪除任務的資訊，請參閱 <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">刪除任務</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">縮進</td> 
      <td><p>按一級縮進任務。 </p><p>此選項僅顯示在獨立任務上。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">升級</td> 
      <td><p>將任務縮排一個級別。 </p><p>此選項僅顯示在子任務上。 </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">插入上述任務</td> 
      <td>在選定任務的上方插入任務。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">在下方插入任務</td> 
      <td>在所選任務下插入任務</td> 
     </tr> 
     <tr> 
      <td role="rowheader">重複</td> 
      <td><p>在同一個項目中建立任務的重複版本。 </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">複製到</td> 
      <td><p>將任務複製到另一個項目。</p><p>有關複製和複製任務的資訊，請參見 <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">複製和複製任務</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">移至</td> 
      <td><p>將任務移動到另一個項目。</p><p>有關移動任務的資訊，請參閱 <a href="../../../manage-work/tasks/manage-tasks/move-tasks.md" class="MCXref xref">移動任務</a>.</p></td> 
     </tr> 
    </tbody> 
   </table>

   更改會自動保存，您無法撤消這些更改。

### 編輯清單中的任務並手動保存更改 {#edit-tasks-in-a-list-and-manually-save-changes}

您可以手動儲存對清單中的任務所做的變更。 以此方式儲存變更時，您可以彈性地在儲存前還原變更。

>[!TIP]
>
>* 在「子任務」部分或任務報表中編輯任務時，無法撤消對清單中任務所做的更改。
>* 您可以反轉的變更數量並無限制。 您可以逐一反轉所有任務，直到達到任務的原始狀態。
>


手動將更改保存到任務清單時，請考慮以下事項：

* 要手動保存任務清單更改，需要權限來管理任務和項目。
* 無法編輯項目。 編輯專案的選項已停用。
* 無法更新項目標題中的資訊。 在任務清單中手動保存更改時，只能執行以下操作：

   * 訂閱專案。
   * 將專案新增至您的最愛清單。
   * 在清單中按一下任務名稱以開啟任務。

* 大量編輯工作。 選擇多個任務時，「編輯」表徵圖被禁用。
* Workfront只會在您儲存變更後，才會觸發您對工作所做變更的相關通知。

有兩種方式可手動儲存清單中任務的變更。 以下說明這兩種方式。

* [選擇「手動保存標準」選項時，手動保存任務清單中的更改](#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-standard-option)
* [選擇「手動保存時間軸計畫」選項時，手動保存任務清單中的更改](#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-timeline-planning-option)

#### 選擇「手動保存標準」選項時，手動保存任務清單中的更改 {#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-standard-option}

>[!TIP]
>
>如果您的專案有超過2000個工作，或有許多相依性，可能需要一段時間才能以視覺化方式識別您對工作所做的變更，以及這些變更如何影響所有專案相依性。 在這種情況下，如果您的專案有2000多個工作，或是相依性很高，則儲存變更可能需要更長的時間。

在選擇「手動保存標準」選項後更新清單中的任務時，請考慮以下事項：

* 您可以將自定義視圖應用到任務清單，並編輯您有權在該視圖中管理的任何任務相關欄位。
* 當項目更新類型為「自動」或「自動」和「更改時」時，Workfront會在您按一下「保存」後計算項目的時間軸以及項目內和跨項目的所有依賴項。 有關項目更新類型的資訊，請參閱 [選擇項目更新類型](../../../manage-work/projects/manage-projects/select-project-update-type.md).

要在選擇「手動保存標準」選項時編輯清單中的任務，請執行以下操作：

1. 前往專案，然後按一下 **工作** 區段。
1. 按一下 **計畫模式** 功能表 ![](assets/qs-list-mode-or-save-mode-icon-small.png) 在清單頂端選取 **手動儲存**，然後按一下 **標準** > **套用**.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

   工具列設定隨即顯示，提供還原、重做和儲存變更的選項。

   ![](assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png)

1. 在您擁有手動更新權限的任何欄位內按一下。 欄位變成可編輯，您可以進行變更。

   ![](assets/inline-editing-a-task-350x26.png)

1. 按下Enter鍵以暫時儲存您所做的變更。
1. （選用）按一下 **還原圖示** ![](assets/undo-icon-on-task-list.png) 要反轉更改並將欄位返回到其原始狀態。
1. （選用和條件式）按一下 **重做圖示** ![](assets/redo-icon-on-task-list.png) 還原您回復的變更。

1. （選用）以滑鼠右鍵按一下您要修改的任務。

   或

   按一下 **更多** 功能表 ![](assets/more-icon-task-list.png).

1. （選用）從下列選項中選取：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>在新索引標籤中開啟</strong> </td> 
      <td>在新瀏覽器頁簽中開啟任務。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">刪除</td> 
      <td>有關刪除任務的資訊，請參閱 <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">刪除任務</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">縮進</td> 
      <td> <p>按一級縮進任務。 </p> <p>此選項僅顯示在獨立任務上。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">升級</td> 
      <td> <p>將任務縮排一個級別。 </p> <p>此選項僅顯示在子任務上。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">插入上述任務</td> 
      <td>在選定任務的上方插入任務。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">在下方插入任務</td> 
      <td>在所選任務下插入任務</td> 
     </tr> 
     <tr> 
      <td role="rowheader">重複</td> 
      <td> <p>在同一個項目中建立任務的重複版本。 </p> <p>有關複製和複製任務的資訊，請參見 <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">複製和複製任務</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Workfront會在您變更工作時間軸時，更新所有專案內和跨專案的相依性。
1. 按一下 **儲存** 要永久保留任務更改並保存項目時間軸時。

#### 選擇「手動保存時間軸計畫」選項時，手動保存任務清單中的更改 {#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-timeline-planning-option}

儲存變更和所有專案相依性都更快。 這不適用於具有2000個以上任務的項目。

>[!IMPORTANT]
>
>建議您在編輯包含數百個具有大量相依性之工作的大量清單時，使用此選項。 使用此選項，您能以比使用手動儲存選項更快的速度以視覺方式識別變更。

在任務清單中使用「手動保存時間線計畫」選項時，請考慮以下事項：

* 不能將「手動保存時間軸計畫」選項應用於具有2000多個任務的項目。
* 不能將自定義視圖、篩選器或分組應用到任務清單。 「檢視」、「篩選」、「分組」下拉式功能表以及「敏捷檢視」圖示會停用。 依預設套用的檢視包含有限的欄位數。
* 在項目更新類型為「自動」或「自動」和「更改時」時，每次更改後，都會自動計算項目時間軸和項目內所有依賴項。
* 當項目更新類型為「自動」或「自動」且「更改時」時，按一下「保存」後，將計算跨項目相依性。 有關項目更新類型的資訊，請參閱 [選擇項目更新類型](../../../manage-work/projects/manage-projects/select-project-update-type.md).

要在使用「手動保存時間軸計畫」選項時編輯清單中的任務，請執行以下操作：

1. 前往專案，然後按一下 **工作** 區段。
1. 按一下 **計畫模式** 功能表 ![](assets/qs-list-mode-or-save-mode-icon-small.png) 在清單頂端選取 **手動儲存**，然後按一下 **時間表規劃**> **套用**.

   對於具有2000多個任務的項目，此選項將呈灰色。

   ![](assets/manual-timeline-planning-setting-enabled-quicksilver-task-list-350x490.png)

   >[!TIP]
   >
   >當您離開此頁面時，Workfront會重新啟用「自動儲存」選項。

   請注意清單中的下列變更：

   * 「視圖」(View)、「分組」(Grouping)和「篩選器」(Filter)下拉菜單被刪除，視圖被以下欄位替換：

      * 任務編號
      * 任務名稱
      * 限制類型
      * 期間
      * 計畫開始日期
      * 計畫完成日期
      * 前置任務
      * 指派
      * 狀態
      * 完成百分比
   * 移除敏捷檢視圖示。
   * 工具列設定隨即顯示，提供還原、重做和儲存變更的選項。

      ![](assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png)


1. 編輯您擁有手動更新權限的任何欄位。

   ![](assets/inline-editing-a-task-350x26.png)

1. 按下Enter鍵以暫時儲存您所做的變更。
1. （選用）按一下 **還原圖示** ![](assets/undo-icon-on-task-list.png) 要反轉更改並將欄位返回到其原始狀態。
1. （選用和條件式）按一下 **重做圖示** ![](assets/redo-icon-on-task-list.png) 恢復已撤消的更改。

1. （可選）按一下右鍵要修改的任務

   或

   按一下 **更多** 功能表 ![](assets/more-icon-task-list.png).

1. 從下列選項中選取：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>在新索引標籤中開啟</strong> </td> 
      <td>在新瀏覽器頁簽中開啟任務。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">刪除</td> 
      <td>有關刪除任務的資訊，請參閱 <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">刪除任務</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">縮進</td> 
      <td> <p>按一級縮進任務。 </p> <p>此選項僅顯示在獨立任務上。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">升級</td> 
      <td> <p>將任務縮排一個級別。 </p> <p>此選項僅顯示在子任務上。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">插入上述任務</td> 
      <td>在選定任務的上方插入任務。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">在下方插入任務</td> 
      <td>在所選任務下插入任務</td> 
     </tr> 
     <tr> 
      <td role="rowheader">重複</td> 
      <td> <p>在同一個項目中建立任務的重複版本。 </p> <p>有關複製和複製任務的資訊，請參見 <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">複製和複製任務</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Workfront會在您變更任務時間軸時，更新所有專案內和跨專案的相依性。
1. 按一下 **儲存** 要永久保留任務更改並保存項目時間軸時。

## 使用「摘要」編輯清單中的任務

1. 前往包含您要編輯之任務的專案。
1. 按一下&#x200B;**工作** 中。

   專案上的任務清單隨即顯示。

1. 按一下「更多」功能表 ![](assets/more-icon-task-list.png) 在任務名稱后，按一下 **開啟摘要**. 選擇要編輯的任務，然後按一下 **開啟摘要圖示** ![](assets/qs-open-summary-icon-in-new-toolbar-small.png) 在清單的右上角。

   此 **摘要** 開啟。

   ![](assets/qs-task-right-panel-in-a-task-list-350x328.png)

1. （選用）按一下 **X圖示** 在「摘要」的右上方，關閉面板並內嵌編輯工作。

   按照有關編輯清單中任務的步驟內嵌編輯任務。

   有關編輯清單中任務的資訊，請參閱 [關於編輯清單中任務的考量事項](#considerations-about-editing-tasks-in-a-list) 這篇文章。

1. （可選）在 **更新** 的上界。
1. 按一下以下任何表徵圖或區域以轉至任務並編輯任務級別的資訊：

   | 文件 | 按一下 **按一下這裡以新增** 向任務添加文檔。 |
   |---|---|
   | 詳细資訊 | 按一下以更新有關任務的資訊。 |
   | 自訂表單 | 按一下以新增或移除自訂Forms，或更新表單上的資訊。 |
   | 時數 | 按一下以記錄小時數。 |
   | 核准 | 按一下以添加任務批准。 |

   {style=&quot;table-layout:auto&quot;}

1. 在更新完任務後，按一下瀏覽器上的返回按鈕返回任務清單。

## 大量編輯任務

您可以一次編輯多個工作。 請確定您擁有可編輯工作的管理權限。

1. 前往包含您要大量編輯之任務的專案。
1. 按一下 **工作** 中。
1. 確保 **自動儲存** 選項。

   >[!IMPORTANT]
   >
   >手動保存任務時無法批量編輯任務。

   有關在清單中保存對任務更改的方式的詳細資訊，請參閱 [關於編輯清單中任務的考量事項](#considerations-about-editing-tasks-in-a-list) 這篇文章。

1. 在任務清單中選擇多個任務。
1. 按一下 **編輯圖示** ![](assets/qs-edit-icon.png).

   此 **編輯任務** 對話框。

1. 指定您要為所選任務更改的資訊。

   編輯所有任務的資訊與編輯一個任務的資訊相同。 如果要編輯任務持續時間，所選任務必須具有相同的任務約束；否則， **持續時間** 欄位未填入。

   有關編輯任務的詳細資訊，請參閱 [編輯任務](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

   >[!NOTE]
   >
   >您正在更改的所有選定任務的資訊將覆蓋有關單個任務的現有資訊，但 **分配** 欄位。 在批量編輯中添加新的受託人將將該受託人添加到所有選定任務。 如果將其他受分配者指派給所選任務，則除了通過批量編輯添加的受分配者之外，這些受分配者將繼續被指派。

1. 按一下 **自訂Forms** 編輯附加到所有選定任務的自定義表單。 清單中只會顯示使用中的自訂表單。

   如果所選任務沒有任何常見的自定義表單，則此部分中不列出任何表單。

   您只能編輯表單上附加至所選任務且您有權編輯的欄位。

1. （選用）在自訂Forms區段中，選取 **重新計算自定義運算式** 選項，確保附加至所選任務的自訂表單上的所有計算自訂欄位都是最新的。
1. 按一下 **儲存變更**.

   您所做的所有變更現在都會顯示在所有選取的任務上。

如需大量編輯自訂表單的相關資訊，請參閱 [管理附加到對象的自定義表單](../../../workfront-basics/work-with-custom-forms/manage-custom-forms-attached-to-objects.md).
