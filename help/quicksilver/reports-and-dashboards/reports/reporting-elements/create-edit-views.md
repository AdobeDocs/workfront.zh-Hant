---
product-area: reporting
navigation-topic: reporting-elements
title: 在Adobe Workfront建立或編輯視圖
description: 可以使用視圖自定義在螢幕上顯示的資訊類型。 您可以在Adobe Workfront使用多種視圖。
author: Nolan
feature: Reports and Dashboards
exl-id: 8fcd6320-c939-4195-8972-5c31575f78cb
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '1750'
ht-degree: 1%

---

# 在Adobe Workfront建立或編輯視圖

可以使用視圖自定義在螢幕上顯示的資訊類型。 您可以在Adobe Workfront使用多種視圖。

本文介紹如何為清單和報告建立和編輯標準視圖，以及如何建立敏捷視圖。 有關詳細資訊，請參見 [Adobe Workfront視圖概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)。

## 訪問要求

您必須具有以下訪問權限才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront計畫</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront許可證*</strong></td> 
   <td> <p>請求或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>訪問級別配置*</strong></td> 
   <td> <p>編輯對篩選器、視圖、分組的訪問</p> <p>編輯對報表、儀表板、日曆的訪問，以在報表中建立視圖</p> <p>注：如果您仍然沒有訪問權限，請詢問您的Workfront管理員是否在您的訪問級別設定了其他限制。 有關Workfront管理員如何修改您的訪問級別的資訊，請參見 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自定義訪問級別</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>對象權限</strong></td> 
   <td> <p>管理對報表的權限以在報表中建立或編輯視圖</p> <p>管理視圖的權限以編輯它</p> <p>有關請求附加訪問的資訊，請參見 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求訪問對象 </a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要瞭解您擁有的計畫、許可證類型或訪問權限，請與您的Workfront管理員聯繫。

## 建立或自定義視圖

建立或定制視圖的過程因建立或定制標準視圖還是敏捷視圖而不同。

* [建立或自定義標準視圖](#create-or-customize-a-standard-view)
* [建立或自定義敏捷視圖](#create-or-customize-an-agile-view)

### 建立或自定義標準視圖 {#create-or-customize-a-standard-view}

您可以建立新的標準視圖，也可以定制先前建立的現有標準視圖。

1. 按一下 **視圖** 建立或自定義視圖的任意清單上的下拉菜單。
1. （可選）要自定義現有視圖，請選擇要自定義的標準視圖。\
   標準視圖可在Workfront的任何類型清單（如報表、項目清單或任務清單）中使用。
1. 按一下 **視圖** 下拉菜單，然後按一下 **自定義視圖** 或 **新建視圖**。\
   的 **自定義視圖** 對話框。

1. 在 **列預覽** ，執行下列任何操作：

   * 通過按一下列標題，然後選擇新欄位來修改任何列的值。
   * 通過按一下 **添加列**，開始鍵入要添加的列的名稱，然後在下拉清單中按一下它。
   * 通過將列標題拖動到新位置來調整列的顯示順序。

      * （可選）在 **列設定** 的 **按以下方式匯總此列** 下拉清單，然後選擇用於匯總資訊的可用選項之一。 選擇此選項時，列中的資訊將聚合到報表的分組中。\
         對於日期欄位，您可以通過以下選項來匯總值：

         * 最大值
         * 最小值

         對於數字和幣種欄位，您可以通過以下選項來匯總值：

         * 計數
         * Sum
         * 平均
         * 最大值
         * 最小值

         >[!NOTE]
         >
         >在分組中聚合以下欄位的值時，父對象（例如，父任務）適用以下例外：
         >   
         >   * 除「實際工時」（例如，計畫/實際人工成本、計畫/實際費用成本、計畫/實際成本、計畫小時數）外，所有數字和幣種欄位僅合計子任務和獨立任務的值。 它們不會聚合父任務或父項父項的值。
         >   * 實際工時匯總主父任務和獨立任務的值；它們不會聚合父任務或子任務的父任務的編號。
         >   * 數字和貨幣值的自定義資料欄位聚合所有任務：父母、子代、父母的父母和獨立任務。


         有關在報告中使用分組的詳細資訊，請參閱文章 [Adobe Workfront分組概覽](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)。

      * （可選）按一下 **高級選項** 指定列的以下資訊：

         <table style="table-layout:auto"> 
         <col> 
         <col> 
         <tbody> 
          <tr> 
           <td role="rowheader"><strong>自訂欄標籤</strong></td> 
           <td><p>指定列的自定義標籤。 此標籤將替換預設標籤。</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>欄位格式</strong></td> 
           <td>選擇要為列中的欄位顯示值的格式。</td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>在報告面板上顯示此欄</strong></td> 
           <td><p>選擇此選項可在報告與另一個報告並排顯示時在儀表板上顯示此列。 取消選中此選項時，在儀表板上查看報告時不顯示此列，其中報告並排顯示。</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>欄規則</strong></td> 
           <td><p>按一下 <strong>為此列添加規則</strong> 的子菜單。 添加規則後，可以定義欄位和文本樣式，以顯示與該規則匹配的欄位。 按一下 <strong>添加規則</strong> 定義完規則後。</p></td> 
          </tr> 
         </tbody> 
        </table>

         有關有條件地設定報表視圖格式的詳細資訊，請參閱文章 [在文本模式中使用條件格式](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md)。



1. （條件）如果按一下 **高級選項**&#x200B;按一下 **完成**。

1. 按一下 **保存視圖** 建立新視圖或用更改替換當前視圖。\
   或\
   按一下 **另存為新視圖** 將更改另存為新視圖。

   >[!TIP]
   >
   >的 **另存為新視圖** 是自定義內置的Workfront視圖時唯一可用的選項。

   您的訪問權限決定了視圖的保存方式。 如果最初建立了視圖，則可以保存更改；否則，系統將提示您保存版本。 請記住，您對視圖所做的更改會影響與其共用視圖的用戶。

### 建立或自定義敏捷視圖 {#create-or-customize-an-agile-view}

您可以建立新的敏捷視圖或自定義先前建立的現有敏捷視圖。

>[!IMPORTANT]
>
>敏捷視圖僅在查看項目時可用。

有關敏捷視圖的詳細資訊，請參閱文章 [在敏捷視圖中管理項目](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md)。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: [! The information in the following steps is more or less duplicated in "Creating and Managing Agile Teams."])</p>
-->

要建立或自定義敏捷視圖：

1. 轉到項目任務清單。
1. 按一下 **敏捷情節提要** 表徵圖 ![](assets/agile-storyboard-nwe.png)。

1. （條件）要自定義現有的敏捷視圖：

   1. 按一下 **視圖** 下拉菜單，然後選擇要自定義的「敏捷」視圖。\
      無法自定義預設的「敏捷」視圖。

   1. 按一下 **視圖** 再次下拉菜單，然後按一下 **自定義視圖**。\
      ![](assets/view-agile-customize.png)

1. （條件）要建立新的敏捷視圖，請按一下 **新建視圖**。\
   的 **自定義敏捷視圖** 對話框。

1. 在 **自定義敏捷視圖** 對話框，為「敏捷」視圖指定名稱。\
   我們建議您在視圖名稱中包含「敏捷」一詞，因此用戶知道這是一個敏捷視圖。\
   此名稱顯示在 **視圖** 下拉菜單。

1. 定義要在敏捷視圖中的文章板上顯示的狀態列。 這些是由Workfront管理員定義的任務狀態，如中所述 [建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)。

   只有系統狀態才可用於敏捷故事板。 如果狀態僅對您所屬的單個組可用，則敏捷故事板上的狀態不可用。 此外，在敏捷視圖中查看項目時，處於僅對自定義組可用狀態的任務不可見。

   用戶可以在敏捷故事板上的這些狀態列之間移動故事。\
   定義狀態列時，可以執行以下操作：

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>重新排序狀態列：</strong> </td> 
      <td> 將狀態列拖動到希望其顯示的順序。<br><img src="assets/agile-project-reorderstatuses-350x141.png" alt="" style="width: 350;height: 141;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>刪除狀態列：</strong> </td> 
      <td>按一下要刪除的列上的(x)表徵圖。<br>除非已將自定義狀態添加到視圖，並且自定義狀態等於「新建」，否則無法刪除「新建」狀態。<br>有關建立自定義狀態的資訊，請參見 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">建立或編輯狀態</a>。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>添加狀態列：</strong> </td> 
      <td> <p>按一下 <strong>加</strong> 表徵圖，然後選擇要添加的狀態。<br>將顯示所有預設系統狀態以及與您共用的任何自定義狀態。<br>您最多可以配置10個狀態來顯示。</p></td> 
     </tr> 
    </tbody> 
   </table>

   <!--
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE FOR ADD STATUS COLUMNS: research this and add: [! What if the status has been shared with me or a group I'm in (so I can see it here), but the status hasn't been shared with another user who also has access to a project where I later apply this view? Can that user still see this status on the project?]) </p>
       -->

1. 在 **將卡顏色關聯到** 的子菜單。

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>本文:</strong> </td> 
      <td>任何子任務都與父任務的顏色匹配，因此任何給定泳道中的所有文章的顏色都相同。<br>如果任務沒有子任務或沒有父任務，則在建立顏色時，顏色會隨機分配給任務。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>自由格式:</strong> </td> 
      <td> 預設情況下，所有卡都顯示為藍色，直到用戶手動更改顏色（如文章中所述） <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/categorize-stories-by-color.md" class="MCXref xref">按顏色對Scrum板上的文章進行分類</a>。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>優先順序:</strong> </td> 
      <td> <p> 顏色與文章優先順序相關聯，如下所示：</p> 
       <ul> 
        <li>高=紅色</li> 
        <li>中=黃色</li> 
        <li>低=綠色<br>如果您的Workfront管理員已為您的Workfront系統配置了自定義優先順序，則最高優先順序為紅色，第二高優先順序為黃色，其餘為綠色。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>任務擁有人:</strong> </td> 
      <td> 具有相同主要受分配人的所有文章顏色相同。<br>主要工作負責人是最初分配給任務的用戶。 </td> 
     </tr> 
    </tbody> 
   </table>

1. 在 **敏捷** 的 **其他欄位** 的 **添加欄位**，然後選擇要添加到文章卡的欄位。 （這些欄位與建立自定義視圖或建立報表列時可以添加的欄位相同。）\
   重複此過程，將文章卡片最多添加三個欄位。\
   在將欄位添加到文章卡時，欄位是僅查看的，並且僅在填充欄位時才顯示。

   預設情況下，文章卡上顯示以下類型的資料：

   * 文章名稱，其連結直接指向任務
   * 具有直接指向項目的連結的項目名稱\
      僅當在迭代中使用敏捷視圖時，才會顯示此連結；在項目上使用「敏捷」視圖時不顯示。
   * 任務說明
   * 當前承諾
   * 通過調整完成百分比本身或通過調整完成的點數或小時數來查看和編輯完成百分比
   * 已指派的使用者

   可以在文章卡上顯示其他資料（包括自定義資料）。 出於多種原因，您可能希望在文章卡上顯示其他欄位。 例如，如果您正在處理項目內多個客戶的案例，則可能希望顯示客戶ID，或者您可能希望顯示任務起始日期。

1. 按一下&#x200B;**儲存**。\
   您的訪問權限決定了視圖的保存方式。 如果最初建立了視圖，則可以保存更改；否則，系統將提示您保存版本。 請記住，您對視圖所做的更改會影響與其共用視圖的用戶。

1. （可選）按一下 **清單視圖** 表徵圖 ![](assets/list-view-in-agile-view-for-tasks.png) 的子菜單。
