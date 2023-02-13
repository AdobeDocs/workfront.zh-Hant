---
product-area: reporting
navigation-topic: reporting-elements
title: 在Adobe Workfront中建立或編輯檢視
description: 您可以使用檢視來自訂顯示在畫面上的資訊類型。 您可以在Adobe Workfront中使用數種檢視類型。
author: Lisa
feature: Reports and Dashboards
exl-id: 8fcd6320-c939-4195-8972-5c31575f78cb
source-git-commit: 442e0b8fde9e4acaa2686ccd292fb003f72be623
workflow-type: tm+mt
source-wordcount: '1748'
ht-degree: 1%

---

# 在Adobe Workfront中建立或編輯檢視

您可以使用檢視來自訂顯示在畫面上的資訊類型。 您可以在Adobe Workfront中使用數種檢視類型。

本文說明如何建立和編輯清單和報表的標準檢視，以及如何建立敏捷檢視。 如需詳細資訊，請參閱 [Adobe Workfront中的檢視概觀](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront計畫*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront授權*</strong></td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>訪問級別配置*</strong></td> 
   <td> <p>編輯對篩選器、檢視、群組的存取</p> <p>編輯對報表、控制面板、日曆的存取權，以在報表中建立檢視</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件權限</strong></td> 
   <td> <p>管理報表權限以建立或編輯報表中的檢視</p> <p>管理檢視的權限以進行編輯</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 建立或自訂檢視

建立或自訂檢視的程式會因您建立或自訂標準檢視或敏捷檢視而有所不同。

* [建立或自訂標準檢視](#create-or-customize-a-standard-view)
* [建立或自訂敏捷檢視](#create-or-customize-an-agile-view)

### 建立或自訂標準檢視 {#create-or-customize-a-standard-view}

您可以建立新的標準視圖，也可以自訂先前建立的現有標準視圖。

1. 按一下 **檢視** 要建立或自訂檢視之清單上的下拉式功能表。
1. （可選）若要自訂現有檢視，請選取您要自訂的標準檢視。\
   在Workfront中，標準檢視可用於任何類型的清單，例如報表、專案清單或任務清單。
1. 按一下 **檢視** 下拉式功能表，然後按一下 **自訂檢視** 或 **新建視圖**.\
   此 **自訂檢視** 對話框。

1. 在 **欄預覽** ，請執行下列任一操作：

   * 按一下欄標題，然後選取新欄位，修改任何欄的值。
   * 按一下 **添加列**，開始輸入要添加的列的名稱，然後在下拉清單中出現時按一下它。
   * 將欄標題拖曳到新位置，調整欄的顯示順序。

      * （選用）在 **欄設定** ，按一下 **匯總此欄，依** 下拉式清單中，然後選取用於匯總資訊的可用選項之一。 選擇此選項時，欄中的資訊會依報表的群組匯總。\
         對於日期欄位，您可以依照下列選項匯總值：

         * 最大值
         * 最小值

         對於數字和貨幣欄位，您可以依照下列選項匯總值：

         * 計數
         * Sum
         * 平均
         * 最大值
         * 最小值

         >[!NOTE]
         >
         >在按分組方式聚合以下欄位的值時，父對象（例如父任務）適用以下例外：
         >   
         >   * 除「實際小時數」（例如，「計畫/實際人工成本」、「計畫/實際費用成本」、「計畫/實際成本」、「計畫小時數」）之外，所有數字和幣種欄位僅匯總子任務和獨立任務的值。 它們不會匯總父任務或父項的父項的值。
         >   * 「實際小時數」匯總主要父任務和獨立任務的值；它們不會匯總父任務或子任務的父任務的數量。
         >   * 數字和貨幣值的自訂資料欄位會匯總所有任務：父母、子女、父母和獨立任務。


         如需在報表中使用分組的詳細資訊，請參閱文章 [Adobe Workfront中的群組概觀](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

      * （選用）按一下 **進階選項** 指定列的以下資訊：

         <table style="table-layout:auto"> 
         <col> 
         <col> 
         <tbody> 
          <tr> 
           <td role="rowheader"><strong>自訂欄標籤</strong></td> 
           <td><p>指定欄的自訂標籤。 此標籤會取代預設標籤。</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>欄位格式</strong></td> 
           <td>選擇您希望欄中欄位的值顯示的格式。</td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>在報告面板上顯示此欄</strong></td> 
           <td><p>選取此選項，當報告與其他報告並排顯示時，即可在控制面板上顯示此欄。 取消選取此選項時，在並排顯示報表的控制面板上檢視報表時，不會顯示此欄。</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>欄規則</strong></td> 
           <td><p>按一下 <strong>為此欄新增規則</strong> 來定義欄的規則。 新增規則後，您可以定義欄位和文字樣式，以顯示符合該規則的欄位。 按一下 <strong>新增規則</strong> 完成規則的定義後。</p></td> 
          </tr> 
         </tbody> 
        </table>

         如需有條件式格式化報表中檢視的詳細資訊，請參閱文章 [在文字模式中使用條件式格式](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).



1. （條件性）如果您按一下 **進階選項**，按一下 **完成**.

1. 按一下 **保存視圖** 建立新視圖或用更改替換當前視圖。\
   或\
   按一下 **另存為新視圖** 將變更儲存為新檢視。

   >[!TIP]
   >
   >此 **另存為新視圖** 是您自訂內建Workfront檢視時唯一可用的選項。

   您的存取會指定檢視的儲存方式。 如果您原先建立了檢視，則可儲存變更；否則，系統會提示您儲存版本。 請記得，您對檢視所做的變更會影響已共用檢視的使用者。

### 建立或自訂敏捷檢視 {#create-or-customize-an-agile-view}

您可以建立新的敏捷視圖，或自訂您先前建立的現有敏捷視圖。

>[!IMPORTANT]
>
>敏捷視圖僅在查看項目時可用。

如需Agile檢視的詳細資訊，請參閱文章 [在敏捷檢視中管理專案](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: [! The information in the following steps is more or less duplicated in "Creating and Managing Agile Teams."])</p>
-->

要建立或自定義敏捷視圖：

1. 轉至專案的任務清單。
1. 按一下 **敏捷情節提要** 圖示 ![](assets/agile-storyboard-nwe.png).

1. （條件性）若要自訂現有的敏捷檢視：

   1. 按一下 **檢視** 下拉式功能表，然後選取您要自訂的敏捷檢視。\
      您無法自訂預設的Agile檢視。

   1. 按一下 **檢視** 再按一下下拉式功能表，然後按一下 **自訂檢視**.\
      ![](assets/view-agile-customize.png)

1. （條件性）若要建立新的敏捷檢視，請按一下 **新建視圖**.\
   此 **自訂敏捷檢視** 對話框。

1. 在 **自訂敏捷檢視** 對話框，指定敏捷視圖的名稱。\
   建議您在檢視名稱中加入&quot;Agile&quot;一字，讓使用者知道這是Agile檢視。\
   此名稱會顯示在 **檢視** 下拉式選單中。

1. 定義要在敏捷檢視的動態展示板上顯示的狀態欄。 這些是由Workfront管理員定義的任務狀態，如 [建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

   Agile展示板上僅提供系統狀態。 如果狀態僅適用於您所屬的個別群組，則敏捷動態展示板上無法使用狀態。 此外，在敏捷檢視中檢視專案時，狀態僅供自訂群組使用的任務不會顯示。

   使用者可以在Agile動態展示板上的這些狀態欄之間移動動態。\
   定義狀態列時，可以執行以下操作：

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>重新排序狀態列：</strong> </td> 
      <td> 將狀態欄拖曳至您希望其顯示的順序。<br><img src="assets/agile-project-reorderstatuses-350x141.png" alt="" style="width: 350;height: 141;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>刪除狀態列：</strong> </td> 
      <td>在您要移除的欄上按一下(x)圖示。<br>除非已將自訂狀態新增至檢視，且自訂狀態等於「新」，否則您無法移除「新」狀態。<br>如需建立自訂狀態的相關資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">建立或編輯狀態</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>添加狀態列：</strong> </td> 
      <td> <p>按一下 <strong>加號</strong> 表徵圖，然後選擇要添加的狀態。<br>系統會顯示所有預設系統狀態，以及已與您共用的任何自訂狀態。<br>您可以設定最多10個狀態以顯示。</p></td> 
     </tr> 
    </tbody> 
   </table>

   <!--
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE FOR ADD STATUS COLUMNS: research this and add: [! What if the status has been shared with me or a group I'm in (so I can see it here), but the status hasn't been shared with another user who also has access to a project where I later apply this view? Can that user still see this status on the project?]) </p>
       -->

1. 在 **將卡片顏色關聯至** ，請從以下選項中選擇：

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>本文:</strong> </td> 
      <td>任何子任務都與父任務的顏色匹配，因此任何給定泳道中所有文章的顏色都相同。<br>如果任務沒有任何子任務或沒有父任務，則在建立任務時，會隨機將顏色分配給任務。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>自由格式:</strong> </td> 
      <td> 依預設，所有卡片都會顯示為藍色，直到使用者手動變更顏色為止（如文章所述） <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/categorize-stories-by-color.md" class="MCXref xref">依色彩分類Scrum展示板上的動態</a>. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>優先順序:</strong> </td> 
      <td> <p> 顏色與文章優先順序相關聯，如下所示：</p> 
       <ul> 
        <li>高=紅色</li> 
        <li>中=黃色</li> 
        <li>低=綠色<br>如果您的Workfront管理員已設定Workfront系統的自訂優先順序，最高優先順序為紅色，第二高為黃色，其餘為綠色。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>任務擁有人:</strong> </td> 
      <td> 所有與相同主要受託人的動態顏色相同。<br>主要受託人是第一次分配給任務的用戶。 </td> 
     </tr> 
    </tbody> 
   </table>

1. 在 **敏捷** 區段中 **其他欄位** 按一下 **新增欄位**，然後選取您要新增至動態卡片的欄位。 （這些欄位與您在建立自訂檢視或建立報表欄時可新增的欄位相同。）\
   重複此程式，在動態卡片中新增最多三個欄位。\
   將欄位新增至動態卡片時，欄位是僅供檢視的，且只會在填入欄位時顯示。

   依預設，動態卡片上會顯示下列類型的資料：

   * 具有直接連結到任務的動態名稱
   * 具有直接連結至專案的專案名稱\
      只有在小版本上使用敏捷視圖時，才會顯示此連結；在專案上使用敏捷檢視時，不會顯示。
   * 任務說明
   * 當前承諾
   * 通過調整完成百分比本身或通過調整完成的點數或小時數來查看和編輯完成百分比
   * 已指派的使用者

   您可以在動態卡片上顯示其他資料（包括自訂資料）。 基於任何原因，您可能想在動態卡上顯示其他欄位。 例如，如果您正在為專案內的多個客戶撰寫動態，或想顯示「任務開始日期」，則可能會想要顯示「客戶ID」。

1. 按一下&#x200B;**儲存**。\
   您的存取會指定檢視的儲存方式。 如果您原先建立了檢視，則可儲存變更；否則，系統會提示您儲存版本。 請記得，您對檢視所做的變更會影響已共用檢視的使用者。

1. （選用）按一下 **清單檢視** 圖示 ![](assets/list-view-in-agile-view-for-tasks.png) 返回任務清單。
