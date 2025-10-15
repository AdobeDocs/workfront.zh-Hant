---
product-area: reporting
navigation-topic: reporting-elements
title: 在Adobe Workfront中建立或編輯檢視
description: 您可以使用檢視來自訂顯示在熒幕上的資訊型別。 您可以在Adobe Workfront中使用數種檢視。
author: Nolan
feature: Reports and Dashboards
exl-id: 8fcd6320-c939-4195-8972-5c31575f78cb
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '1713'
ht-degree: 1%

---

# 在Adobe Workfront中建立或編輯檢視

<!-- Audited: 11/2024 -->

您可以使用檢視來自訂顯示在熒幕上的資訊型別。 您可以在Adobe Workfront中使用數種檢視。

本文說明如何建立及編輯清單與報告的標準檢視，以及如何建立敏捷檢視。 如需詳細資訊，請參閱[Adobe Workfront中的檢視總覽](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)。

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

建立或自訂檢視的流程會有所不同，這取決於您是要建立或自訂標準檢視還是敏捷檢視。

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

您可以建立敏捷檢視或自訂您先前建立的現有敏捷檢視。

>[!IMPORTANT]
>
>敏捷檢視僅在檢視專案時可用。

如需敏捷檢視的詳細資訊，請參閱文章[在敏捷檢視中管理專案](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md)。

>[!NOTE]
>
>此程式僅適用於舊版敏捷檢視，不適用於專案的展示板檢視。

若要建立或自訂敏捷檢視：

1. 前往專案上的任務清單。
1. 按一下&#x200B;**展示板**&#x200B;圖示![展示板圖示](assets/board-icon-for-agile-view.png)，然後按一下展示板檢視上的&#x200B;**使用舊版敏捷**。

1. （視條件而定）若要自訂現有的敏捷檢視：

   1. 按一下&#x200B;**檢視**&#x200B;下拉式功能表，然後選取您要自訂的敏捷檢視。\
      您無法自訂預設的敏捷檢視。

   1. 再次按一下&#x200B;**檢視**&#x200B;下拉式功能表，然後按一下&#x200B;**自訂檢視**。\
      ![自訂檢視](assets/view-agile-customize.png)

1. （視條件而定）若要建立新的敏捷檢視，請按一下&#x200B;**新檢視**。\
   顯示&#x200B;**自訂敏捷檢視**&#x200B;對話方塊。

1. 在&#x200B;**自訂敏捷檢視**&#x200B;對話方塊中，指定敏捷檢視的名稱。\
   我們建議您在檢視名稱中加入「敏捷」一詞，讓使用者知道這是敏捷檢視。\
   選取檢視時，此名稱會顯示在&#x200B;**檢視**&#x200B;下拉式功能表中。

1. 定義要在敏捷檢視的內文板上顯示的狀態列。 這些是Workfront管理員定義的工作狀態，如[建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)中所述。

   敏捷故事板上只能使用系統狀態。 如果狀態僅適用於您為成員的個別群組，則敏捷故事板上不會提供狀態。 此外，在敏捷檢視中檢視專案時，看不到狀態為僅供自訂群組使用的任務。

   使用者可以在敏捷故事板上的這些狀態列之間移動故事。\
   定義狀態列時，您可以執行下列動作：

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>重新排序狀態列：</strong> </td> 
      <td> 將狀態列拖曳至您要其顯示的順序。<br><img src="assets/agile-project-reorderstatuses-350x141.png" alt="" style="width: 350;height: 141;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>移除狀態資料行：</strong> </td> 
      <td>按一下您要移除之欄上的(x)圖示。<br>除非已新增自訂狀態至檢視，且該自訂狀態等於「新增」，否則您無法移除「新增」狀態。<br>如需建立自訂狀態的詳細資訊，請參閱<a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">建立或編輯狀態</a>。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>新增狀態資料行：</strong> </td> 
      <td> <p>按一下<strong>加號</strong>圖示，然後選取您要新增的狀態。<br>會顯示所有預設的系統狀態，以及與您共用的任何自訂狀態。<br>您可以設定顯示最多10個狀態。</p></td> 
     </tr> 
    </tbody> 
   </table>

   <!--
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE FOR ADD STATUS COLUMNS: research this and add: [! What if the status has been shared with me or a group I'm in (so I can see it here), but the status hasn't been shared with another user who also has access to a project where I later apply this view? Can that user still see this status on the project?]) </p>
       -->

1. 在&#x200B;**將卡片顏色與**&#x200B;區域關聯中，從下列選項中選取：

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>劇本：</strong> </td> 
      <td>任何子任務都符合父任務的顏色，因此任何指定泳道中所有劇本的顏色都相同。<br>如果任務沒有任何子任務或沒有父任務，則會在建立顏色時隨機指派給任務。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>自由格式：</strong> </td> 
      <td> 所有卡片預設都會顯示為藍色，直到使用者手動變更顏色為止，如文章<a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/categorize-stories-by-color.md" class="MCXref xref">在Scrum展示板上依顏色分類劇本</a>中所述。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>優先順序：</strong> </td> 
      <td> <p> 顏色與內文優先順序相關聯，如下所示：</p> 
       <ul> 
        <li>高=紅色</li> 
        <li>Medium =黃色</li> 
        <li>低=綠色<br>如果您的Workfront管理員已設定Workfront系統的自訂優先順序，最高優先順序為紅色，次高為黃色，其餘為綠色。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>工作擁有者：</strong> </td> 
      <td> 所有主要受指派人相同的劇本都是相同的色彩。<br>主要受指派人是第一個受指派工作的使用者。 </td> 
     </tr> 
    </tbody> 
   </table>

1. 在&#x200B;**其他欄位**&#x200B;區域中，按一下&#x200B;**新增欄位**，然後選取您要新增到故事卡的欄位。 （這些欄位與建立自訂檢視或建立報表欄位時可新增的欄位相同。）\
   重複此程式，向劇本卡片新增最多三個額外的欄位。\
   當您新增欄位到內文卡時，欄位是僅供檢視的，並且只有在填入欄位時才顯示。

   預設情況下，內文卡會顯示下列型別的資料：

   * 內文名稱，內含直接連結至工作的連結
   * 含有直接連結至專案的專案名稱\
     此連結只有在疊代上使用敏捷檢視時才會顯示；在專案上使用敏捷檢視時則不會顯示。
   * 任務說明
   * 目前承諾
   * 檢視並編輯完成百分比，方法是調整完成百分比本身，或調整完成點數或時數
   * 已指派的使用者

   您可以在故事卡上顯示其他資料（包括自訂資料）。 基於各種原因，您可能會想要在內文卡上顯示額外的欄位。 例如，如果您正在專案中處理多個客戶的劇本，或想要顯示「作業開始日期」，您可能會想要顯示「客戶ID」。

1. 按一下「**儲存**」。\
   您的存取權會指定檢視的儲存方式。 如果最初建立的是檢視，您可以儲存變更；否則，系統會提示您儲存版本。 請記住，您對檢視所做的變更會影響已共用檢視的使用者。

1. （選擇性）按一下&#x200B;**清單**&#x200B;圖示以返回工作清單。
