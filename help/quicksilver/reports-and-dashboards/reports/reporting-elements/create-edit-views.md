---
product-area: reporting
navigation-topic: reporting-elements
title: 在Adobe Workfront中建立或編輯檢視
description: 您可以使用檢視來自訂顯示在熒幕上的資訊型別。 您可以在Adobe Workfront中使用數種檢視。
author: Nolan
feature: Reports and Dashboards
exl-id: 8fcd6320-c939-4195-8972-5c31575f78cb
source-git-commit: a4ccd48956fedbafc04ce19198592efdad49e5a3
workflow-type: tm+mt
source-wordcount: '1777'
ht-degree: 1%

---

# 在Adobe Workfront中建立或編輯檢視

您可以使用檢視來自訂顯示在熒幕上的資訊型別。 您可以在Adobe Workfront中使用數種檢視。

本文說明如何建立和編輯清單與報告的標準檢視，以及如何建立敏捷檢視。 如需詳細資訊，請參閱 [Adobe Workfront中的檢視概觀](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

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
   <td> <p>要求或以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>存取層級設定*</strong></td> 
   <td> <p>編輯篩選器、檢視、群組的存取權</p> <p>編輯對報告、儀表板、行事曆的存取權，以在報告中建立檢視</p> <p>注意：如果您仍然沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件許可權</strong></td> 
   <td> <p>管理報表的許可權，以建立或編輯報表中的檢視</p> <p>管理檢視的許可權以進行編輯</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 建立或自訂檢視

建立或自訂檢視的流程會有所不同，這取決於您是要建立或自訂標準檢視還是敏捷檢視。

* [建立或自訂標準檢視](#create-or-customize-a-standard-view)
* [建立或自訂敏捷檢視](#create-or-customize-an-agile-view)

### 建立或自訂標準檢視 {#create-or-customize-a-standard-view}

您可以建立新的標準檢視，也可以自訂先前建立的現有標準檢視。

1. 按一下 **檢視** 下拉式選單，位於您要建立或自訂檢視的任何清單上。
1. （可選）若要自訂現有檢視，請選取您要自訂的標準「檢視」。\
   Workfront中任何型別的清單（例如報告、專案清單或工作清單）上都可以使用標準檢視。
1. 按一下 **檢視** 下拉式功能表，然後按一下 **自訂檢視** 或 **新增檢視**.\
   此 **自訂檢視** 對話方塊隨即顯示。

1. 在 **欄預覽** 章節，執行下列任一項作業：

   * 按一下欄標題，然後選取新欄位，修改任何欄的值。
   * 按一下以新增欄 **新增欄**，開始輸入您要新增的欄名稱，然後當它出現在下拉式清單中時按一下它。
   * 將欄標題拖曳至新位置，調整欄的顯示順序。

      * （選用）在 **欄設定** 區域，按一下 **此欄的摘要方式** 下拉式清單，然後選取其中一個可用選項來彙總資訊。 選擇此選項時，欄中的資訊會聚總在報表的群組中。\
        對於日期欄位，您可以透過下列選項彙總值：

         * 最大值
         * 最小值

        針對數字與幣別欄位，您可以透過下列選項彙總值：

         * 計數
         * Sum
         * 平均
         * 最大值
         * 最小值

        >[!NOTE]
        >
        >當您彙總分組中下列欄位的值時，下列例外情況適用於父系物件（例如父系任務）：
        >   
        >   * 除「實際時數」（例如，計畫/實際勞力成本、計畫/實際費用成本、計畫/實際成本、計畫時數）之外的所有數字與幣別欄位，只會彙總子系任務和獨立任務的值。 它們不會彙總父系任務的值或父系父系的值。
        >   * 實際時數彙總主要父任務和獨立任務的值；它們不會彙總父任務父任務或子任務的數字。
        >   * 數字和貨幣值的自訂資料欄位會彙總所有任務：父項、子項、父項的父項以及獨立任務。
        >   
        >

        如需在報表中使用分組的詳細資訊，請參閱文章 [Adobe Workfront中的群組概觀](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

      * （可選）按一下 **進階選項** 指定欄的下列資訊：

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
           <td>選取您要為欄中的欄位顯示值的格式。</td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>在報告面板上顯示此欄</strong></td> 
           <td><p>當報告與其他報告並排顯示時，選取此選項可在控制面板上顯示此欄。 取消選取此選項時，在報告並排顯示的儀表板上檢視報告時不會顯示此欄。</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>欄規則</strong></td> 
           <td><p>按一下 <strong>為此欄新增規則</strong> 以定義欄的規則。 新增規則後，您可以定義欄位和文字樣式，以顯示符合該規則的欄位。 按一下 <strong>新增規則</strong> 定義完規則之後。</p></td> 
          </tr> 
         </tbody> 
        </table>

        如需有關在報表中有條件地格式化檢視的詳細資訊，請參閱文章 [在文字模式中使用條件式格式](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

1. （視條件而定）如果您按一下 **進階選項**，按一下 **完成**.

1. 按一下 **儲存檢視** 以建立新檢視或以您所做的變更取代目前檢視。\
   或\
   按一下 **另存為新檢視** 將變更另存為新檢視。

   >[!TIP]
   >
   >此 **另存為新檢視** 是自訂內建Workfront檢視時唯一可用的選項。

   您的存取權會指定檢視的儲存方式。 如果您最初建立了檢視，則可以儲存變更；否則，系統會提示您儲存版本。 請記住，您對檢視所做的變更會影響已共用檢視的使用者。

### 建立或自訂敏捷檢視 {#create-or-customize-an-agile-view}

您可以建立新的敏捷檢視，或是自訂您先前建立的現有敏捷檢視。

>[!IMPORTANT]
>
>敏捷檢視僅在檢視專案時可用。

如需關於敏捷檢視的詳細資訊，請參閱文章 [在敏捷檢視中管理專案](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).

>[!NOTE]
>
>此程式僅適用於舊版敏捷檢視，不適用於專案的展示板檢視。

若要建立或自訂敏捷檢視：

1. 前往專案上的任務清單。
1. 按一下 **展示板** 圖示 ![展示板圖示](assets/board-icon-for-agile-view.png)，然後按一下 **使用舊版敏捷** 在展示板檢視上。

1. （視條件而定）若要自訂現有的敏捷檢視：

   1. 按一下 **檢視** 下拉式功能表，然後選取您要自訂的敏捷檢視。\
      您無法自訂預設的敏捷檢視。

   1. 按一下 **檢視** 再次使用下拉式功能表，然後按一下 **自訂檢視**.\
      ![](assets/view-agile-customize.png)

1. （視條件而定）若要建立新的敏捷檢視，請按一下 **新增檢視**.\
   此 **自訂敏捷檢視** 對話方塊隨即顯示。

1. 在 **自訂敏捷檢視** 對話方塊中，指定敏捷檢視的名稱。\
   我們建議您在檢視名稱中加入「敏捷」一詞，讓使用者知道這是敏捷檢視。\
   此名稱會顯示在 **檢視** 下拉式功能表。

1. 定義要在敏捷檢視的內文板上顯示的狀態列。 這些是由Workfront管理員定義的工作狀態，如中所述 [建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

   只有系統狀態可用於敏捷故事板。 如果狀態僅適用於您所屬的個別群組，則無法在敏捷故事板上取得狀態。 此外，在敏捷檢視中檢視專案時，看不到狀態為僅供自訂群組使用的任務。

   使用者可以在敏捷內文板上的這些狀態列之間移動內文。\
   定義狀態列時，您可以執行下列動作：

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>重新排序狀態列：</strong> </td> 
      <td> 將狀態列拖曳至您要顯示的順序。<br><img src="assets/agile-project-reorderstatuses-350x141.png" alt="" style="width: 350;height: 141;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>移除狀態列：</strong> </td> 
      <td>按一下您要移除之欄上的(x)圖示。<br>除非已新增自訂狀態至檢視，且該自訂狀態等於「新增」，否則您無法移除「新增」狀態。<br>如需建立自訂狀態的詳細資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">建立或編輯狀態</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>新增狀態列：</strong> </td> 
      <td> <p>按一下 <strong>加號</strong> 圖示，然後選取您要新增的狀態。<br>所有預設系統狀態以及已與您共用的任何自訂狀態都會顯示。<br>您可以設定顯示最多10個狀態。</p></td> 
     </tr> 
    </tbody> 
   </table>

   <!--
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE FOR ADD STATUS COLUMNS: research this and add: [! What if the status has been shared with me or a group I'm in (so I can see it here), but the status hasn't been shared with another user who also has access to a project where I later apply this view? Can that user still see this status on the project?]) </p>
       -->

1. 在 **將卡片顏色關聯至** 區域，從下列選項中選取：

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>本文:</strong> </td> 
      <td>任何子任務都和父任務的顏色相符，因此任何指定泳道中所有劇本的顏色都相同。<br>如果任務沒有任何子任務或沒有父任務，則在建立顏色時，顏色會隨機指派給任務。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>自由格式:</strong> </td> 
      <td> 所有卡片預設都會顯示為藍色，直到使用者手動變更顏色為止，如文章所述 <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/categorize-stories-by-color.md" class="MCXref xref">在Scrum展示板上依顏色分類劇本</a>. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>優先順序:</strong> </td> 
      <td> <p> 顏色與內文優先順序相關聯，如下所示：</p> 
       <ul> 
        <li>高=紅色</li> 
        <li>中=黃色</li> 
        <li>低=綠色<br>如果您的Workfront管理員已設定Workfront系統的自訂優先順序，最高優先順序為紅色，次高為黃色，其餘為綠色。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>任務擁有人:</strong> </td> 
      <td> 具有相同主要受指派人的所有劇本都是相同的色彩。<br>主要受指派人是首次指派給任務的使用者。 </td> 
     </tr> 
    </tbody> 
   </table>

1. 在 **敏捷** 區段，在 **其他欄位** 區域，按一下 **新增欄位**，然後選取您要新增至劇本卡的欄位。 （這些欄位與建立自訂檢視或建立報表欄位時可新增的欄位相同。）\
   重複此程式，為劇本卡新增最多三個額外的欄位。\
   將欄位新增至內文卡時，欄位僅供檢視，且僅在填入欄位時顯示。

   預設情況下，內文卡上會顯示下列型別的資料：

   * 內文名稱，內有直接指向任務的連結
   * 有直接連結至專案的專案名稱\
     此連結只有在疊代上使用敏捷檢視時才會顯示；在專案上使用敏捷檢視時則不會顯示。
   * 任務說明
   * 目前承諾
   * 檢視並編輯完成百分比，方法是調整完成百分比本身，或調整完成點數或時數
   * 已指派的使用者

   您可以在故事卡上顯示其他資料（包括自訂資料）。 出於各種原因，您可能想要在內文卡上顯示其他欄位。 例如，如果您正在專案中處理多個客戶的劇本，或想要顯示「任務開始日期」，您可能會想要顯示「客戶ID」。

1. 按一下&#x200B;**儲存**。\
   您的存取權會指定檢視的儲存方式。 如果您最初建立了檢視，則可以儲存變更；否則，系統會提示您儲存版本。 請記住，您對檢視所做的變更會影響已共用檢視的使用者。

1. （可選）按一下 **清單** 圖示以返回任務清單。
