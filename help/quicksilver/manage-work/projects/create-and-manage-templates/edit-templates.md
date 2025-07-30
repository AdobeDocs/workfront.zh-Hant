---
product-area: templates
navigation-topic: templates-navigation-topic
title: 編輯專案範本
description: 您可以編輯專案範本，以反映未來專案的程式與設定變更。 您可以一次編輯一個範本，也可以大量編輯多個範本。
author: Alina
feature: Work Management
exl-id: da0fca31-6a50-4862-ad9a-a453ef968773
source-git-commit: f4ea19368b664d0b3a47f93c70fd489685791538
workflow-type: tm+mt
source-wordcount: '5045'
ht-degree: 2%

---

# 編輯專案範本

<!-- Audited: 7/2025 -->

<!--The Resource Pools part also duplicates in the "Working with Resource Pools" article-->

<!--
<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> 

-->


您可以編輯專案範本，以反映未來專案的程式與設定變更。

更新並儲存範本上的變更後，當使用範本建立專案時，新變更會顯示在新專案中。

您在範本上進行的變更不會反映在目前使用該範本的專案上。

您可以一次編輯一個範本，也可以大量編輯範本。

## 存取需求

+++ 展開以檢視存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td>
      <p>新增：標準</p>
      <p>或</p>
      <p>目前：計畫</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級</td> 
   <td> <p>編輯範本的存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> 
    <ul> 
     <li> <p>貢獻範本的許可權以在「範本詳細資訊」索引標籤中進行編輯</p> </li> 
     <li> <p>管理範本的許可權，以在「編輯範本」方塊中編輯範本</p> </li> 
   </td> 
  </tr> 
 </tbody> 
</table>

*如需此表格中資訊的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 編輯範本 {#edit-a-template}

1. 移至您要編輯的範本。
1. （視條件而定）若要編輯範本的有限資訊，請按一下左側面板中的&#x200B;**範本詳細資料**，然後移至左側面板中列出的區域，以編輯每個區域的資訊。
1. 若要編輯詳細資訊區段中的資訊，請按一下&#x200B;**編輯**&#x200B;圖示![編輯圖示](assets/edit-icon.png)，然後從下列任何區域選取，或按一下&#x200B;**編輯全部**&#x200B;以編輯所有區域的資訊：

   * 概觀
   * 自訂表單

   只有當物件附有自訂表單時，才會顯示自訂表單的名稱。

   * 財務

   >[!TIP]
   >
   >如需詳細資訊區域中顯示的所有欄位相關資訊，請使用下方的「編輯範本」方塊繼續編輯所有欄位。

1. （視條件而定）若要編輯範本的所有相關資訊，請按一下範本名稱旁的&#x200B;**更多**&#x200B;功能表![更多圖示](assets/qs-more-icon-on-an-object.png)，然後按一下&#x200B;**編輯**。

   **編輯範本**&#x200B;方塊開啟。 此方塊中的區段包含「範本詳細資訊」區段中的可用欄位以及其他欄位。

1. 請考慮編輯下列任一節中的資訊：

   * [範本名稱](#template-name)
   * [總覽](#overview-preview)
   * [財務](#finance-preview)
   * [自訂表單](#custom-forms-preview)
   * [範本設定](#template-settings)
   * [工作設定](#task-settings)
   * [問題設定](#issue-settings)
   * [存取](#access-preview)
   * [評論](#comment)
   <!--* [Linked folders](#linked-folders-conditional-availability) -->


### 範本名稱{#template-name}

1. 如上所述開始編輯您的範本。
1. 在&#x200B;**編輯範本**&#x200B;方塊中，按一下&#x200B;**範本名稱**。
1. 更新或取代範本的名稱。
1. （選擇性）根據您要修改的資訊，繼續編輯下列區段

   或

   按一下「**儲存**」。

### 概觀 {#overview-preview}

1. 如上所述開始編輯您的範本。
1. 在&#x200B;**編輯範本**&#x200B;方塊中，按一下&#x200B;**概觀**。

   ![編輯範本方塊概觀區段](assets/edit-template-box-overview-section.png)

1. 更新下列欄位：

   <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
         <tr> 
         <td role="rowheader"><strong>說明</strong></td> 
         <td>新增範本的其他相關資訊。</td> 
       </tr> 
         <tr> 
         <td role="rowheader"><strong>優先順序</strong></td> 
         <td><p>這只是一個視覺化的標幟，可讓您為未來的專案設定優先順序。 從下列選項中選取：</p> 
         <ul> 
         <li><p><strong>無</strong></p></li> 
         <li><p><strong>低</strong></p></li> 
         <li><p><strong>正常</strong></p></li> 
         <li><p><strong>高</strong></p></li> 
         <li><p><strong>緊急</strong></p></li> 
         </ul><p><p>根據Workfront管理員選取的專案偏好設定，您的優先順序名稱可能會不同。 如需有關編輯優先順序的詳細資訊，請參閱<a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">建立及自訂優先順序</a>。</p></p></td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>URL</strong></td> 
         <td>指定與此範本相關資訊的網頁連結。</td> 
       </tr>
<tr> 
      <td role="rowheader"><strong>為作用中</strong></td> 
      <td><p>如果您希望範本為作用中範本，請開啟此選項。 其他使用者可在建立專案時找到此範本並將其附加至專案。 如果您要停用不再使用的範本，請關閉選項。 無法將已停用的範本附加到專案。 這預設為啟用。 </p><p><b>秘訣</b></p>

<p>您可以從範本標題停用範本，如本文的「啟動或停用範本」一節中所述。</p></td> 
     </tr>

<tr> 
<td role="rowheader"><strong>狀況類型</strong></td> 
   <td><p>在下列條件型別之間選取：</p> 
   <ul> 
   <li><strong>手動：</strong>專案所有者手動設定專案上的專案狀態。 <strong></strong></li> 
   <li><strong>進度狀態：</strong> Workfront會根據關鍵路徑上任務的進度狀態，自動設定未來專案的條件。 如需瞭解進度狀態的詳細資訊，請參閱<a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">任務進度狀態概觀</a>。</li> 
   </ul>
   </td> 
   </tr> 
   <tr> 
   <td role="rowheader"><strong>排程模式</strong></td> 
   <td><p>指定使用此範本的專案是從<strong>開始日期</strong>排程，還是從<strong>完成日期</strong>排程。 此選取範圍會決定使用此範本之專案中未來任務的計畫日期。 </p><p>從下列選項中選取： </p> 
   <ul> 
   <li><p><strong>從開始日期排程</strong>：範本的開始日期實際上是開始日期。 當您從「開始日期」排程範本時，Adobe Workfront會根據所有範本工作的「持續時間」計算範本的「完成日期」。 範本的開始日期成為未來專案的規劃開始日期。</p></li> 
   <li><p><strong>從完成日期排程</strong>：範本的完成日期實際上是完成日期。 當您從「完成日期」排程範本時，Workfront會根據所有範本任務的持續時間計算範本的「開始日期」。 範本的「完成日」成為未來專案的「計畫完成日」。 </p></li> 
   </ul><p>如需範本任務開始與完成天數的詳細資訊，請參閱<a href="../../../manage-work/projects/create-and-manage-templates/overview-of-start-completion-day-on-template.md" class="MCXref xref">範本中開始與完成天數的概述</a>。 </p><p>範本的「排程起始日期」設定與專案的設定類似。 您的Workfront管理員會為您的系統中的專案選取預設的「排程起始日期」設定。 如需有關設定專案預設值的資訊，請參閱<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">設定全系統的專案偏好設定</a>。</p></td> 
   </tr>

<tr> 
   <td role="rowheader"><strong>專案組合</strong></td> 
   <td><p>針對從此範本建立的專案指定Portfolio。 您必須先建立Portfolio，才能讓其出現在下拉式清單中。 </p><p>只有作用中的投資組合會顯示在清單中。 如需關於建立投資組合的詳細資訊，請參閱<a href="../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md" class="MCXref xref">建立投資組合</a>。</p></td> 
   </tr> 
   <tr> 
   <td role="rowheader"><strong>方案</strong></td> 
   <td><p>如果您為範本選取Portfolio，請為未來的專案指定<strong>方案</strong>。 部分投資組合可能沒有計畫。 您必須先建立程式，它才會顯示在此下拉式清單中。 清單中只會顯示使用中的程式。</p><p>如需建立程式的詳細資訊，請參閱<a href="../../../manage-work/portfolios/create-and-manage-programs/create-program.md" class="MCXref xref">建立程式</a>。</p></td> 
   </tr>  
   <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td role="rowheader"><strong>群組</strong></td> 
   <td><p>在下拉式清單中，選取要與從範本建立的專案相關聯的群組。 可以是任何層級的群組。 </p><p>您可以暫留在正確的群組上，並按一下旁邊顯示的資訊圖示<img src="assets/info-icon.png">，確定您選取的群組正確。 這會顯示工具提示，列出群組的相關資訊，例如群組及其管理員上方的群組階層。</p> <p><b>附註</b>

<ul> 
   <li><p>在群組頁面的「專案」區域中，當有人使用未選取群組的範本建立專案時，系統會建立目前開啟的群組與專案之間的關聯。</p><p>這與當使用者使用未選取群組的範本建立專案時，系統將使用者的「主群組」與專案關聯的其他區域不同。</p></li> 
   <li><p>如果使用者在建立專案時或在將任務或問題轉換為專案時選取已選取群組的範本，則使用者可以為專案選擇不同的群組。</p></li> 
   <li>雖然此欄位僅在新的Adobe Workfront體驗中可在範本中使用，但您可在範本中的清單與報表以及Adobe Workfront Classic中檢視。 </li> 
   </ul> </p></td> 
   </tr> 
   <tr> 
   <td role="rowheader"><strong>公司</strong></td> 
   <td><p>指定您要與範本建立關聯的公司。 清單中只會顯示作用中的公司。</p></td> 
   </tr> 
   <tr> 
   <td role="rowheader"><strong>範本所有者</strong></td> 
   <td><p>指定為範本擁有者的使用者必須是Workfront作用中使用者。 </p><p>請考量下列有關指定為「範本擁有者」的使用者： </p> 
   <ul> 
   <li>系統會自動授予使用者範本的管理許可權。 </li> 
   <li>他們會被新增至專案團隊，並自動獲得從範本建立的專案的管理許可權。 </li> 
   <li>從此範本建立專案時，他們就會成為專案所有者。 </li> 
   <li> 如果指定為範本擁有者的使用者從存取層級對範本或專案具有有限的存取權，則其範本和專案的管理許可權將受到限制。 例如，如果他們只有其存取層級中的範本或專案的檢視存取權，當他們被指定為範本擁有者時，他們將會自動獲得範本和專案的檢視許可權。</li>
   </ul></td> 
   </tr> 
   <tr> 
   <td role="rowheader"><strong>範本贊助者</strong></td> 
   <td><p>將範本新增至專案時，此欄位中指定的使用者會成為專案贊助者。 此使用者會新增至專案團隊，並自動獲得專案的檢視許可權。 被指定為範本贊助者的使用者必須是Workfront作用中使用者。 </p></td> 
   </tr> 
   <tr> 
   <td role="rowheader"><strong>資源管理員</strong></td> 
   <td><p>指定的使用者會自動獲得管理未來專案的許可權，並且可以指派資源給專案的任務和問題。 您可以指定一個以上的Resource Manager。 </p></td> 
   </tr> 
</table>

1. （選擇性）根據您要修改的資訊，繼續編輯下列區段。

   或

   按一下「**儲存**」。

### 財務 {#finance-preview}

1. 如上所述開始編輯您的範本。
1. 在&#x200B;**編輯範本**&#x200B;方塊中，按一下&#x200B;**財務**。

   ![編輯範本方塊財務區段](assets/edit-template-box-finance-section.png)

1. 更新下列欄位：

   <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody>
       <tr> 
         <td role="rowheader"><strong> 貨幣</strong></td> 
         <td><p>若與系統的預設貨幣不同，請指定未來專案的貨幣。 如果系統中只有預設貨幣，則不會顯示此欄位。<br>如需貨幣詳細資訊，請參閱<a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">設定匯率</a>。</p></td> 
       </tr>
       <tr> 
       <td role="rowheader"><strong>預算</strong></td> 
       <td><p>指定從此範本建立之專案的預算。</p></td> 
       </tr>  
       <tr> 
         <td role="rowheader"><strong>績效指數方法</strong></td> 
         <td><p>選擇Workfront計算未來專案盈餘量度的方式。 從下列選項中選擇：
         <ul>
         <li>基於小時</li>
         <li>基於成本</li>
         </ul>

   如需有關績效指數方法的詳細資訊，請參閱<a href="../../../manage-work/projects/project-finances/set-pim.md" class="MCXref xref">設定績效指數方法(PIM)</a>。 </p></td>
   </tr> 
         <tr> 
         <td role="rowheader"><strong>規劃收益</strong></td> 
         <td><p>指定從此範本建立之專案的計畫收益。 計畫收益用於專案和Portfolio Optimizer的業務案例。 </p><p>如需有關專案計畫權益的詳細資訊，請參閱<a href="../../../manage-work/projects/project-finances/project-planned-benefit.md" class="MCXref xref">專案計畫權益概觀</a>。 計算專案淨值時，會考慮專案的計畫收益。 </p><p>如需使用Portfolio Optimizer的詳細資訊，請參閱<a href="../../../manage-work/portfolios/portfolio-optimizer/manage-projects-in-portfolio-optimizer.md" class="MCXref xref">在Portfolio Optimizer中管理專案</a> </p></td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>固定成本</strong></td> 
         <td><p>指定從此範本建立之專案的「固定成本」。 這與專案時數所產生的人工成本，以及專案費用金額所產生費用成本不同。 計算專案的淨值時會考慮專案的固定成本，而且該成本是預算成本的一部分。</p></td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>固定收入</strong></td> 
       <td><p>指定從此範本建立之專案的「固定收入」 。</p></td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>此專案需要時間核准</strong></td> 
       <td><p>選取此選項可要求從此範本建立的未來專案的專案所有者核准登入專案的時間。 如果您使用「計費記錄」並選取此選項，則只有專案中已核准的時數，才會顯示為「計費記錄」的可用計費時數。 核准專案的時間與核準時程表無關。 如需專案需要核准時間的詳細資訊，請參閱<a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" class="MCXref xref">專案需要核准時間</a>。</p></td> 
       </tr> 
       </tbody> 
      </table>

1. （選擇性）根據您要修改的資訊，繼續編輯下列區段。

   或

   按一下「**儲存**」。

### 自訂表單 {#custom-forms-preview}

1. 如上所述開始編輯您的範本。
1. 在&#x200B;**編輯範本**&#x200B;方塊中，按一下&#x200B;**自訂Forms**。

   ![編輯範本方塊自訂Forms區段](assets/edit-template-box-custom-forms-section.png)

   已附加至範本的自訂表單的名稱會顯示在左側面板中。

1. 在&#x200B;**新增自訂表單**&#x200B;欄位內按一下，然後選取您要與範本關聯的一或多個自訂表單。 您必須先建置自訂表單，才能在此欄位中選取它們。

   清單中只會顯示作用中的自訂表單。 如需建立自訂表單的詳細資訊，請參閱[建立自訂表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

   您最多可以新增10個自訂表單至範本。

   表單將新增至從此範本建立的專案。

1. （選用）更新自訂表單上任何欄位中的資訊。 此資訊將會傳輸至將使用範本建立的專案。

1. （選擇性）按一下自訂表單名稱右邊的&#x200B;**x**&#x200B;圖示，然後按一下[移除]&#x200B;**&#x200B;**&#x200B;以從範本中移除它。

1. （選擇性）根據您要修改的資訊，繼續編輯下列區段。

   或

   按一下「**儲存**」。

### 範本設定 {#template-settings}

1. 如上所述開始編輯您的範本。
1. 在&#x200B;**編輯範本**&#x200B;方塊中，按一下&#x200B;**專案設定**。

   ![編輯範本方塊範本設定區段](assets/edit-template-box-project-settings-section.png)

1. 更新下列欄位：

   <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
       <tr> 
       <td role="rowheader"><strong>里程碑路徑</strong> </td> 
       <td> <p>選取範本的里程碑路徑。 只有作用中的里程碑路徑會顯示在清單中。<br>如需里程碑路徑的詳細資訊，請參閱<a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">建立里程碑路徑</a>。</p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>完成模式</strong> </td> 
         <td> <p>控制如何將未來的專案標示為完成。 <br>從下列選項中選取：</p> 
         <ul> 
         <li> <p><strong>自動</strong>：當所有任務和問題都完成時，專案會標示為完成。</p> </li> 
         <li> <p><strong>手動</strong>：您必須在所有任務和問題都完成時，手動選取專案的完成狀態。 </p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>摘要完成模式</strong> </td> 
       <td> <p>控制如何將未來專案上的父系任務標示為完成。 <br>從下列選項中選取：</p> 
       <ul> 
       <li> <p><strong>自動</strong>：父系任務標示為「完成」，而且當子系任務完成且子系完成百分比更新時，父系任務會自動更新完成百分比。 </p> </li> 
       <li> <p><strong>手動</strong>：您必須手動更新完成百分比和父系任務的狀態，而不考慮對子系任務所做的變更。 </p> </li> 
       </ul> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>更新型別</strong> </td> 
         <td> <p>控制您對未來專案時間表所做的變更何時儲存在專案上。 </p> 
         <b>範例</b> 
         <p>專案的下列變更會觸發專案時間表更新：</p> 
         <ul> 
         <li> <p>更新任務日期</p> </li> 
         <li> <p>變更前置任務關係<br></p> </li> 
         <li> <p>變更父子關係</p> </li> 
         <li> <p>除了變更任務限制或期間型別之外，還新增或移除指派。</p> </li> 
         </ul> 
         </div> <p>從下列選項中選取：<br></p> 
         <ul> 
         <li> <p><strong>自動與開啟變更</strong> （預設設定）：每當專案或時間表所依存之其他專案中發生變更（開啟變更）時，未來專案時間表就會更新。 專案時間表也會每晚更新（自動）。<br>這是此欄位的建議設定，因為它可確保專案時間表隨時保持最新。<br>當您對觸發時間表重新計算的任務或專案執行動作時，所有可用日期會立即顯示，讓您繼續工作。 在具有100個以上任務的專案中，需要更長重新計算的日期會短暫顯示為問號（1到5秒之間，大型專案最多會顯示一分鐘）。 這表示重新計算尚未完成，日期可能會變更。<br></p> </li> 
         </ul> 
         <ul> 
         <li> <p><strong>僅變更</strong>：每次在專案或時間表所依存的其他專案中發生變更時，專案時間表都會更新。 如果變更很少發生在專案或時間表所依賴的其他專案中，您可能會想要選取此選項。<br></p> </li> 
         </ul> 
         <ul> 
         <li> <p><strong>僅限自動</strong>：專案時間表每晚都會更新；變更後不會立即更新。<br>如果每天在專案或時間表所依賴的其他專案中發生許多變更，您可能會想要選取此選項。 但是，請注意，您選擇了此設定，因為專案不會在進行變更的同時更新。<br></p> </li> 
         </ul> 
         <ul> 
         <li> <p><strong>僅手動</strong>：專案時間表只有在您選取重新計算時間表的選項時才會更新，如<a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">重新計算專案時間表</a>中所述。<br></p> </li> 
         </ul> <p>如果您一次對專案進行許多變更，且希望在所有變更完成後（而不是在每次個別變更後）重新計算時間表，則可能需要選取此選項。</p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>排程</strong> </td> 
         <td> <p>選取範本的排程。 這會成為從此範本建立的專案排程。 這應該是指派給大多數處理專案的人的相同排程。 您必須先建立排程，才能將其指派給範本。<br>如需建立排程的詳細資訊，請參閱<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">建立排程</a>。 <br>如果您尚未在系統中建立自訂排程，則會選取[預設排程]。 </p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>使用者休假</strong> </td> 
         <td> <p>決定任務之主要受指派人的休假是否調整任務計畫日期。 當您將範本附加到現有專案時，並且範本對此欄位的設定與專案不同，專案上的設定保持不變。 新範本此設定的預設選項與系統層級專案偏好設定相同。 </p> <p>如需系統層級專案偏好設定的相關資訊，請參閱<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">設定全系統的專案偏好設定</a>。 </p> <p>如需此設定如何影響專案上任務日期的詳細資訊，請參閱<a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">編輯專案</a>。<br>從下列選項中選取：<br></p> 
         <ul> 
         <li> <p><strong>考慮使用者在任務持續期間的休假</strong>：選取此選項時，如果休假發生在任務持續期間，則根據任務的主要受指派人的休假，調整從此範本建立的專案上任務的計畫日期。 </p> </li> 
         <li> <p><strong>忽略使用者在任務持續期間的休假</strong>：選取此選項時，即使任務的主要受指派人在任務持續期間具有休假，根據此範本建立的專案上任務的計畫日期仍維持原始計畫。 </p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>資源平準模式</strong> </td> 
         <td> <p>從下列選項中選取：<br></p> 
         <ul> 
         <li> <p><strong>手動</strong>：您必須在從這個範本建立的專案上手動平準資源（這是預設設定）</p> </li> 
         <li> <p><strong>自動：</strong> Workfront會針對未來的專案提供資源層級。 <br>如需資源平準的詳細資訊，請參閱甘特圖<a href="../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md" class="MCXref xref">中的</a>平準資源。 </p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>風險</strong> </td> 
         <td> <p>定義從此範本建立的專案之風險等級。 風險只是專案風險程度的指標。 您可以根據風險等級來排定執行專案的優先順序。<br>請考慮從下列風險等級中選取：<br></p> 
         <ul> 
         <li> <p><strong>極低</strong> </p> </li> 
         <li> <p><strong>低</strong> </p> </li> 
         <li> <p><strong>Medium</strong> </p> </li> 
         <li> <p><strong>高</strong> </p> </li> 
         <li> <p><strong>非常高</strong> </p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>資源集區</strong> </td> 
         <td> <p>指定與範本關聯的資源集區。 資源集區是同時需要用來完成專案的使用者集合。 如需資源集區的詳細資訊，請參閱<a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref">資源集區概述</a>。</p> <p> <p><b>附註</b>

   當您大量編輯範本時，此欄位只會顯示所有選定範本通用的資源集區。 如果選取的範本沒有共用資源集區，此欄位將為空白。 您在此處指定的資源集區將會覆寫範本的個別資源集區。</p> </p> </td>
   </tr>

   <tr> 
      <td role="rowheader"><strong>此專案需要時間核准</strong></td>

<td><p>選取此選項可要求從此範本建立的專案之未來專案所有者核准登入專案的時間。</p> 
   <p>如果您使用「計費記錄」並選取此選項，則只有專案中已核准的時數，才會顯示為「計費記錄」的可用計費時數。 </p>
   <p>核准專案的時間與核準時程表無關。 如需專案需要核准時間的詳細資訊，請參閱<a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" class="MCXref xref">專案需要核准時間</a>。</p>
   </td> 
   </tr> 
   <tr> 
   <td role="rowheader"><strong>篩選時數型別</strong> </td> 
   <td> <p>請考量下列事項：</p> <p>選取<strong>否</strong>，讓所有特定專案小時型別都可在未來的專案中使用。 （這是預設選取範圍）</p> <p>或</p> <p>選取<strong>是</strong>，讓未來的專案只能使用專案特定時數型別的子集，然後選取您想要使用的時數型別。 （按住Shift鍵以選取多個小時型別。）</p> <p>如果您選取此選項，則在記錄專案時數（或專案內任務和問題）時，只有您選取的時數型別可供選取。 您必須至少選取一個小時型別；如果您選取此選項而未選取任何小時型別，則專案上將會提供所有小時型別。</p> <p>必須在個別使用者層級做出相同的小時型別選擇，以便使用者在專案上檢視這些小時型別選項。 </p> <p>如需有關在使用者層級定義時數型別的詳細資訊，請參閱<a href="../../../timesheets/create-and-manage-timesheets/log-time.md#understa" class="MCXref xref">記錄時間</a>的<a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">記錄時間</a>小節。</p> </td> 
   </tr> 
   <tr> 
   <td role="rowheader"><strong>提醒通知</strong> </td> 
   <td>選取應該與未來專案關聯的提醒通知。 您必須為專案設定提醒通知，此欄位才能在編輯範本時顯示。 <br>如需設定提醒通知的詳細資訊，請參閱<a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">設定提醒通知</a>。</td> 
   </tr>
   <tr> 
   <td role="rowheader"><strong>核准流程</strong> </td> 
   <td> <p>選取您要與範本產生關聯的核准程式。 您的Workfront管理員或具有核准流程管理存取權的使用者必須定義系統層級或群組層級的專案核准流程，您才能將其與範本建立關聯。 如需建立核准流程的詳細資訊，請參閱<a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">建立工作專案的核准流程</a>。</p> <p>新增核准程式時，請考量下列事項： </p> 
   <ul> 
   <li>清單中只會顯示有效的核准流程。 </li> 
   <li> <p>系統範圍及群組特定的核准程式會顯示在清單中。 與範本以外的群組相關聯的核准程式不會顯示在清單中。</p> <p><b>重要</b>

如果與範本關聯的群組變更，群組特定核准流程會變成單一使用核准流程。 如需關於專案群組的變更或核准程式變更如何影響核准設定的詳細資訊，請參閱<a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md">群組和核准程式變更如何影響指派的核准程式</a>。 </p> </li>
<li> <p>如果您新增單次使用的核准程式，在此欄位中顯示為「自訂」。 如需詳細資訊，請參閱<a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">將新的或現有的核准程式與工作建立關聯</a>。 </p> 
      </li> 
      <li> <p>大量編輯範本時，會出現下列情況：</p> 
      <ul> 
         <li> <p>當您從相同群組選取範本時，系統層次與群組層次核准程式都會顯示在此欄位中。</p> </li> 
         <li> <p>當您從不同的群組選取範本時，此欄位中只會顯示系統層級的核准程式。</p> </li> 
         <li> <p>當任何範本附加單一使用核准流程時，它會由您選取的系統層級取代。 </p> </li> 
      </ul> </li> 
      </ul> </td> 
       </tr>  
       </tbody> 
      </table>

1. （選擇性）根據您要修改的資訊，繼續編輯下列區段。\
   或
1. 按一下「**儲存**」。

### 任務設定 {#task-settings}

當您將新任務新增至使用範本建立的專案時，您可以定義與所有新任務關聯的預設值。

如需這些設定如何影響建立新工作的資訊，請參閱[建立工作概覽](../../../manage-work/tasks/create-tasks/create-tasks-overview.md)。

1. 如上所述開始編輯您的範本。
1. 在&#x200B;**編輯範本**&#x200B;方塊中，按一下&#x200B;**工作設定**。

   ![編輯範本方塊任務設定區段](assets/edit-template-box-task-settings-section.png)

1. 在&#x200B;**任務預設核准流程**&#x200B;方塊中，選取當您新增至從此範本建立的專案時，要與所有新任務關聯的核准流程。 您必須先建立任務的核准流程，然後才能將其與任務建立關聯。 清單中只會顯示有效的核准流程。 如需有關建立核准流程的詳細資訊，請參閱[建立核准流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)。
1. 在「**任務預設自訂Forms**」方塊中，選取當您新增至從此範本建立的專案時，要與所有新任務關聯的一個或多個自訂表單。 您必須先建置自訂表單，才能在此欄位中選取它們。 清單中只會顯示作用中的自訂表單。 如需建立自訂表單的詳細資訊，請參閱[建立自訂表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。 您最多可以將十個自訂表單與任務建立關聯。
1. （選擇性）如果您要在從範本建立的專案中使用工作量而非計畫時數來啟用管理任務付出，請選取&#x200B;**使用工作量自動計算任務計畫時數**。
1. （條件式與選擇性）如果您選取使用工作量自動計算任務計畫時數，請按一下下拉式功能表，以更新每個工作量層級的百分比。 預設值為下列百分比值：

   | 工作投入等級 | 百分比值 |
   |---|---|
   | 小 | 25% |
   | 中 | 50% |
   | 大 | 75% |

   如需使用工作量來管理專案上任務之工作量的相關資訊，請參閱[工作量概觀](../../../manage-work/tasks/task-information/work-effort.md)。

1. （選擇性）根據您要修改的資訊，繼續編輯下列區段。

   或

   按一下「**儲存**」。

### 問題設定 {#issue-settings}

透過編輯問題設定，您可以防止使用者在將來的專案中新增使用範本建立的問題。

1. 如上所述開始編輯您的範本。
1. 在&#x200B;**編輯範本**&#x200B;方塊中，按一下&#x200B;**問題設定**。

   ![編輯範本方塊問題設定區段](assets/edit-template-box-issue-settings-section.png)

1. （選擇性）取消選取&#x200B;**允許使用者新增內嵌問題**&#x200B;選項。 預設為啟用。

   停用此選項時，當從範本建立專案時，使用者無法將內聯問題新增到專案或問題區段中的任務。

   >[!TIP]
   >
   >如果您要強制使用者完成新問題欄位或與新問題相關聯的自訂表單，請停用此選項。

   當停用此選項時，具有將問題新增至從範本建立的專案之許可權的使用者可以使用「新增問題」按鈕或與專案關聯的請求佇列來這樣做。

   如需有關在專案上設定問題設定的詳細資訊，請參閱文章[編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md#issue)中的[問題設定](../../../manage-work/projects/manage-projects/edit-projects.md)區段。

   如需有關在專案上建立問題的資訊，請參閱[建立問題](../../../manage-work/issues/manage-issues/create-issues.md)。

1. （選擇性）根據您要修改的資訊，繼續編輯下列區段。

   或

   按一下「**儲存**」。

### 存取 {#access-preview}

1. 如上所述開始編輯您的範本。
1. 在&#x200B;**編輯範本**&#x200B;方塊中，按一下&#x200B;**存取**。

   ![編輯範本方塊存取區段](assets/edit-template-box-access-section.png)

   使用範本建立專案時，您為範本指定的存取權將成為與專案相關聯的使用者存取權。

   指定範本的下列&#x200B;**存取**&#x200B;資訊：

   <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
       <tr> 
         <td role="rowheader"><strong>將某人指派給任務時</strong> </td> 
         <td> <p>從<strong>檢視</strong>、<strong>Contribute、</strong>或<strong>管理</strong>工作存取權中選取。 指派給任務的使用者會自動被授予此任務的存取權。 </p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>同時授與專案的存取權</strong> </td> 
         <td> <p> 從<strong>檢視</strong>、<strong>貢獻</strong>或<strong>管理</strong>專案存取權中選取。 指派給任務的使用者也會自動被授予此專案的存取權。 </p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>將某人指派給問題時</strong> </td> 
         <td> <p>從<strong>檢視</strong>、<strong>Contribute、</strong>或<strong>管理</strong>存取問題中選取。 指派給問題的使用者會自動被授予此問題的存取權。 </p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>同時授與專案的存取權</strong> </td> 
         <td> <p> 從<strong>檢視</strong>、<strong>貢獻</strong>或<strong>管理</strong>專案存取權中選取。 指派給問題的使用者也被自動授予此專案的存取權。 </p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>某人提交要求時：授予他們存取權</strong> </td> 
         <td> <p> 從<strong>檢視</strong>、<strong>Contribute</strong>或<strong>管理</strong>要求存取權中選取。 當他們向專案提交請求時，他們被授予對所提交請求的存取權。 如需詳細資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">共用問題</a>。</p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>來自相同公司的人員將會為所有要求繼承相同的許可權</strong> </td> 
         <td> <p>如果您希望來自相同公司的人員擁有專案上所有請求的相同存取權（無論他們是否提交請求），請選取此欄位。</p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>某人獲得此專案的存取權時：授予他們存取權……</strong> </td> 
         <td> <p>選取您希望使用者在專案上擁有的存取選項（如果專案已與他們共用）。 選取存取權的特定選項，如果它們被指定為<strong>檢視者</strong>、<strong>貢獻者</strong>，或是<strong>管理員</strong> （共用專案時）。 </p> </td> 
       </tr> 
       </tbody> 
      </table>

1. （選擇性）根據您要修改的資訊，繼續編輯下列區段。

   或

   按一下「**儲存**」。

   您的變更將會針對此範本提交。

   現在，當您使用此範本建立專案時，所有這些設定都將轉移到新專案。

<!--I don't think this note is valid anymore - this note was on Edit project when the section below was in that article, by mistake: 
>[!NOTE]
>
>Because linked folders are created when the project is created, editing the linked folder workflow on an existing project is ineffective. Editing these values when creating a project functions as expected.-->

<!-- This section is here by mistake - it should be maybe in layout templates?? 

### Linked folders (conditional availability) {#linked-folders}

Linked folder functionality automatically creates folders in Adobe Experience Manager Assets, and connects these folders to Workfront. 

This section appears only if all of the following apply:

* Your organization has been migrated to the Adobe Admin Console
* Your organization has enabled and configured an integration with Adobe Experience Manager
* The template has enabled and configured linked folders.

For instructions on editing Linked folders, see [Edit workflow values in a project](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md#edit-workflow-values-in-a-project) in the article [Use workflows in the Experience Manager Assets integration](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md).

-->

### 評論

1. 如上所述開始編輯您的範本。
1. 在&#x200B;**編輯範本**&#x200B;方塊中，按一下&#x200B;**註解**。

   ![編輯範本方塊註解區段](assets/edit-template-box-comment-section.png)
1. 新增您正在進行之更新的相關註解、標籤其他使用者，或選取&#x200B;**我的公司私有**&#x200B;方塊，讓貴公司的使用者無法存取更新，然後按一下[儲存]。**&#x200B;**

## 大量編輯範本

您可以大量編輯範本，並同時更新其所有資訊。

<!--
Editing templates in bulk differs depending on which environment you are using. 

### Edit templates in bulk in the Production environment 

*****************and hide the first line below************ -->

若要大量編輯範本：

{{step1-to-templates}}

1. 在清單中選取數個範本。
1. 按一下&#x200B;**編輯**&#x200B;圖示![編輯圖示](assets/edit-icon.png)。

   **編輯範本**&#x200B;對話方塊開啟。

   ![編輯範本](assets/edit-templates-in-bulk-box-nwe-350x327.png)

1. 按一下左側的區段以編輯所有選取的範本。

   如需有關編輯範本資訊的詳細資訊，請參閱本文中的[編輯範本](#edit-a-template)一節。

1. 更新所選範本的下列區段：

   * 概觀
   * 財務
   * 專案組合
   * 設定
   * 存取
   * 自訂表單
   * 任務
   * 問題
   * 評論

1. 按一下「**儲存變更**」。

   您所做的所有變更現在會顯示在所有選取的範本上。

<!--
<div class="preview">

### Edit templates in bulk in the Preview environment 

*****************and hide/delete the first line below************

To edit templates in bulk:

{{step1-to-templates}}

1. Select several templates in the list.
1. Click the **Edit** icon ![Edit icon](assets/edit-icon.png).

   The **Edit Templates** dialog box opens.

   ![Edit templates in bulk box](assets/edit-templates-in-bulk-box.png)

1. Click the sections on the left to edit all selected templates.

   For more information about editing information on templates, see the [Edit a template](#edit-a-template) section in this article.

1. Update the following sections of the selected templates:

   * Overview
   * Custom Forms
   * Finance
   * Template Settings
   * Task Settings
   * Issue Settings
   * Access
   * Comment

1. Click **Save**.

   All changes you made are now visible on all the selected templates.

</div>

-->

## 將任務新增至範本

建立範本並編輯範本資訊後，您就可以新增任務至範本。

將任務新增至範本類似於將任務新增至專案。

如需將任務新增至專案的詳細資訊，請參閱[在專案中建立任務](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md)。

當您將任務新增到範本時，範本的持續時間以及範本的開始和完成天數會相應變更。 如需範本與範本任務開始與完成天數的詳細資訊，請參閱[範本中開始與完成天數的概述](../../../manage-work/projects/create-and-manage-templates/overview-of-start-completion-day-on-template.md)。

## 新增更多專案至範本

建立範本並編輯範本資訊後，您就可以新增更多專案至範本。 從範本建立專案時，您新增的專案將可用於該專案。

將下列專案新增至範本與將它們新增至專案相同：

* 文件
* 風險

  如需建立風險的詳細資訊，請參閱[在專案上建立和編輯風險](/help/quicksilver/manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md)。

* 核准流程

  如需將核准程式與工作產生關聯的資訊，請參閱[將新的或現有的核准程式與工作產生關聯](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)。

* 計費費率

  為範本新增收費率與為專案新增收費率類似。 如需詳細資訊，請參閱專案層級[的](/help/quicksilver/manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md)覆寫工作角色收費率。

* 費用

  如需新增費用的詳細資訊，請參閱[管理專案費用](../../../manage-work/projects/project-finances/manage-project-expenses.md)。

* 佇列詳細資訊

  如需有關將佇列詳細資料新增至專案或範本的資訊，請參閱[建立請求佇列](/help/quicksilver/manage-work/requests/create-and-manage-request-queues/create-request-queue.md)。

* 主題群組與佇列主題

  如需有關將主題群組和佇列主題新增至專案或範本的資訊，請參閱下列文章：

   * [建立主題群組](/help/quicksilver/manage-work/requests/create-and-manage-request-queues/create-topic-groups.md)
   * [建立佇列主題](/help/quicksilver/manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)

您可以將下列專案新增至範本中的任務：

* 文件
* 費用

  如需新增費用的詳細資訊，請參閱[管理專案費用](../../../manage-work/projects/project-finances/manage-project-expenses.md)。

* 核准

  如需將核准與工作建立關聯的詳細資訊，請參閱[將新的或現有的核准程式與工作建立關聯](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)。


## 啟用或停用範本

如果您希望使用者找不到範本並無法從中建立專案，您可以停用範本。 您無法將已停用的範本附加到專案，也無法使用它來建立專案。

已停用的範本不會影響使用它們建立的現有專案。

若要停用範本：

1. 移至使用中的範本，然後按一下範本名稱旁的&#x200B;**更多** ![更多圖示](assets/qs-more-icon-on-an-object.png)功能表，然後按一下&#x200B;**停用**。

   ![停用範本](assets/deactivate-template-link-in-more-menu.png)

   範本已不在使用中，使用者無法找到範本以從中建立專案。
1. （選擇性）若要啟用範本，請按一下範本名稱旁的&#x200B;**更多** ![更多圖示](assets/qs-more-icon-on-an-object.png)功能表，然後按一下&#x200B;**啟用**。

   此範本現在已啟用，可附加至專案或用來建立專案。


<!--
Editing a template differs depending on what environment you choose. 

### Edit a template in the Production environment {#edit-a-template-in-the-production-environment} 

1. Go to the template you want to edit.
1. (Conditional) To edit limited information about the template,  click **Template Details** in the left panel, then go to the areas listed in the left panel to edit information for each area. 
1. To edit information in the Details section, click the **Edit** icon ![Edit icon](assets/edit-icon.png), then select from any of the areas below, or click **Edit all** to edit information in all areas:

   * Overview
   * Custom Forms

     Names of customs forms display only if there are custom forms attached to the object.
   
   * Finance

   >[!TIP]
   >
   >For information about all fields that display in the Details area, continue with editing all fields using the Edit Template box below.

1. (Conditional) To edit all information about the template, click the **More** menu ![More icon](assets/qs-more-icon-on-an-object.png) next to the name of the template, then click **Edit**.

   The **Edit Template** box opens. The sections in this box contain the same fields available in  the Template Details section .

1. Consider editing information in any of the following sections:

   * [Overview](#overview) 
   * [Finance](#finance) 
   * [Portfolio](#portfolio) 
   * [Settings](#settings) 
   * [Access](#access) 
   * [Custom Forms](#custom-forms) 
   * [Tasks](#tasks) 
   * [Issues](#issues) 
   * [Comment](#comment)

### Overview {#overview}

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Overview**.

   ![Edit template overview](assets/edit-template-overview-with-tasks-and-issues-350x210.png)

1. Update the following fields:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Name</strong></td> 
      <td>Specify a name for the template.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Description</strong></td> 
      <td>Add additional information about the template.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Is Active</strong></td> 
      <td><p>Select this checkbox if you want the template to be active. Other users can find this template and attach it to projects when creating projects. Deselect this checkbox if you want to deactivate templates that are no longer used. Deactivated templates cannot be attached to projects. This is enabled by default. </p><p><b>TIP</b>
      
      You can deactivate a template from the template header as described in the [Activate or deactivate a template](#activate-or-deactivate-a-template) section in this article.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong></td> 
      <td>Specify a web link that relates to information about this template.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Schedule From</strong></td> 
      <td><p>Specify whether the project using this template is scheduled from the <strong>Start Date</strong>, or from the <strong>Completion Date</strong>. This selection determines the planned dates of the future tasks on the project using this template. </p><p>Select from the following: </p> 
       <ul> 
        <li><p><strong>Schedule From Start Date</strong>: The Start Date of the template is actually the Start Day. When you schedule a template from Start Date, Adobe Workfront calculates the Completion Day of the template based on the Duration of all the template tasks. The Start Day of the template becomes the Planned Start Date of the future project.</p></li> 
        <li><p><strong>Schedule from Completion Date</strong>: The Completion Date of the template is actually the Completion Day. When you schedule a template from Completion Date, Workfront calculates the Start Day of the template based on the Duration of all the template tasks. The Completion Day of the template becomes the Planned Completion Date of the future project. </p></li> 
       </ul><p>For more information about the Start and Completion Days of template tasks, see <a href="../../../manage-work/projects/create-and-manage-templates/overview-of-start-completion-day-on-template.md" class="MCXref xref">Overview of Start and Completion Days in a template</a>. </p><p>The Schedule From setting for templates is similar to that of projects. Your Workfront administrator selects the default Schedule From setting for the projects in your system. For information about setting project defaults, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Condition Type</strong></td> 
      <td><p>Select between the following Condition Types:</p> 
       <ul> 
        <li><strong>Manual:</strong> The project owner sets the Condition of the project on the project manually. <strong></strong></li> 
        <li><strong>Progress Status:</strong> Workfront automatically sets the Condition of the future project based on the Progress Status of tasks on the Critical Path. For more information about understanding Progress Status, see <a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Task Progress Status overview</a>.</li> 
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priority</strong></td> 
      <td><p>This is just a visual flag for you which allows you to prioritize your future projects. Select from the following options:</p> 
       <ul> 
        <li><p><strong>None</strong></p></li> 
        <li><p><strong>Low</strong></p></li> 
        <li><p><strong>Normal</strong></p></li> 
        <li><p><strong>High</strong></p></li> 
        <li><p><strong>Urgent</strong></p></li> 
       </ul><p><p>Depending on the Project Preferences selected by your Workfront administrator, the names of priorities might be different for you. For more information about editing priorities, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">Create and customize priorities</a>.</p></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Template Owner</strong></td> 
      <td><p>The user who is designated as the Template Owner must be a Workfront active user. </p><p>Consider the following about the user designated as the Template Owner: </p> 
       <ul> 
        <li>They are automatically given Manage permissions to the template. </li> 
        <li>They are added to the project team and are automatically given Manage permissions to the project created from the template. </li> 
        <li>They become the Project Owner, when the project is created from this template. </li> 
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Template Sponsor</strong></td> 
      <td><p>The user specified in this field becomes the Project Sponsor, when the template is added to the project. This user is added to the project team and is automatically given view permissions to the project. The user who is designated as the Template Sponsor must be a Workfront active user. </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Resource Manager</strong></td> 
      <td><p>The specified users are automatically given manage permissions to the future projects and can assign resources to the tasks and issues of the projects. You can specify more than one Resource Manager. </p></td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>Group</strong></td> 
      <td><p>In the drop-down list, select the group that you want to be associated with projects created from the template. It can be a group of any level. </p><p>You can make sure you are selecting the right group by hovering over it and clicking the information icon <img src="assets/info-icon.png"> that displays next to it. This displays a tooltip listing information about the group, such as the hierarchy of groups above it and its administrators.</p> <p><b>NOTES</b>
      
    <ul> 
    <li><p>In the Projects area on a group's page, when someone creates a project using a template that doesn't have a group selected, the system associates the currently open group with the project.</p><p>This is different from other areas where the system associates a user's Home Group with the project when the user creates the project using a template that doesn't have a group selected.</p>
    </li> 
      <li><p>If a user selects a template that has a group selected while creating a project—or while converting a task or issue to a project—the user can choose a different group for the project.</p></li> 
      <li>Though this field is available in templates only in the new Adobe Workfront experience, you can see it in lists and reports both there and in Adobe Workfront Classic. </li> 
      </ul> </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Company</strong></td> 
      <td><p>Specify the Company that you want to associate with the template. Only active companies display in the list.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.

   Or

   Click **Save Changes**.

### Finance {#finance}

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Finance**.

   ![Edit template finance](assets/edit-template-finance-with-tasks-and-issues-350x259.png)

1. Update the following fields:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Performance Index Method</strong></td> 
      <td><p>Specify whether the Earned Value metrics of the future project are calculated using hours or costs. For more information about the Performance Index Method, see <a href="../../../manage-work/projects/project-finances/set-pim.md" class="MCXref xref">Set the Performance Index Method (PIM)</a>. </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Budget</strong></td> 
      <td><p>Specify a Budget for the projects that are created from this template.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Fixed Cost</strong></td> 
      <td><p>Specify the Fixed Cost for the projects that are created from this template. This is different than the Labor Cost which comes from the hours on the project and the Expense Cost which comes from the amount of expenses on the project. The Fixed Cost of a project is taken into account when calculating the Net Value of a project and it is part of the Budgeted Cost.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Fixed Revenue</strong></td> 
      <td><p>Specify the Fixed Revenue for the projects that are created from this template.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Template Currency</strong></td> 
      <td><p>Specify the currency for the future project, if it is different than the default currency of your system. This field is not visible if you have only the default currency in the system.<br>For more information about currency, see <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Set up exchange rates</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Require time to be approved for this project</strong></td> 
      <td><p>Select this option to require the Project Owner of the future project created from this template to approve time logged on the project. If you are using Billing Records and you select this option, only the approved hours on the project appear as available billable hours for the Billing Records. Approving time on the project is independent of approving timesheets. For more information about requiring time to be approved on a project, see <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" class="MCXref xref">Require time to be approved for a project</a>.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.

   Or

   Click **Save Changes**.

### Portfolio {#portfolio}

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Portfolio**.

   ![Edit template portfolio](assets/edit-template-portfolio-with-tasks-and-issues-350x228.png)

1. Update the following fields:

   <table style="table-layout:auto">
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Portfolio</strong></td> 
      <td><p>Specify a Portfolio for the projects that are created from this template. You must create a Portfolio first, before it appears in the drop-down list. </p><p>Only active portfolios display in the list. For more information about creating portfolios, see <a href="../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md" class="MCXref xref">Create a portfolio </a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Program</strong></td> 
      <td><p>If you selected a Portfolio for the template, specify a <strong>Program</strong> for the future project. Some Portfolios might not have Programs. You must create a Program first, before it appears in this drop-down list. Only active programs display in the list.</p><p>For more information about creating programs, see <a href="../../../manage-work/portfolios/create-and-manage-programs/create-program.md" class="MCXref xref">Create a program</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Planned Benefit</strong></td> 
      <td><p>Specify the Planned Benefit of the projects that are created from this template. The Planned Benefit is used in the Business Case of the project and the Portfolio Optimizer. </p><p>For more information about the Planned Benefit of a project, see <a href="../../../manage-work/projects/project-finances/project-planned-benefit.md" class="MCXref xref">Overview of project Planned Benefit</a>. The Planned Benefit of a project is taken into account when the Net Value of a project is calculated. </p><p>For more information about using the Portfolio Optimizer, see <a href="../../../manage-work/portfolios/portfolio-optimizer/manage-projects-in-portfolio-optimizer.md" class="MCXref xref">Manage projects in the Portfolio Optimizer</a> </p></td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.

   Or

   Click **Save Changes**.

### Settings {#settings}

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Settings**.

   ![Edit template settings](assets/edit-template-settings-with-tasks-and-issues-350x336.png)

1. Update the following fields: 

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Milestone Path</strong> </td> 
      <td> <p>Select a Milestone Path for the template. Only active milestone paths display in the list.<br>For more information about Milestone Paths, see <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">Create a milestone path</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Completion Mode</strong> </td> 
      <td> <p>Controls how the future project will be marked as Complete. <br>Select from the following options:</p> 
       <ul> 
        <li> <p><strong>Automatic</strong>: The project is marked Complete when all the tasks and issues are completed.</p> </li> 
        <li> <p><strong>Manual</strong>: You have to manually select the Complete status for the project, when all the tasks and issues are completed. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Summary Completion Mode</strong> </td> 
      <td> <p>Controls how the parent tasks on the future project are marked as Complete. <br>Select from the following options:</p> 
       <ul> 
        <li> <p><strong>Automatic</strong>: The parent tasks are marked Complete and they update their percent complete automatically, as the children tasks are completed and the percent complete of the children is updated. </p> </li> 
        <li> <p><strong>Manual</strong>: You have to manually update the percent complete and the status of the parent tasks, independently of what changes are made to the children tasks. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Update Type</strong> </td> 
      <td> <p>Controls when the changes you make to the timeline of the future project are saved on the project. </p> 
       <b>EXAMPLE </b> 
        <p>The following changes to the project trigger an update to the timeline of the project:</p> 
        <ul> 
         <li> <p>update the dates of tasks</p> </li> 
         <li> <p>change predecessor relationships<br></p> </li> 
         <li> <p>change parent-child relationships</p> </li> 
         <li> <p>add or remove assignments in addition to changing the task constraint or duration type.</p> </li> 
        </ul> 
       </div> <p>Select from the following options:<br></p> 
       <ul> 
        <li> <p><strong>Automatic and On Change</strong> (Default setting): The future project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on (On Change). The project timeline is also updated each night (Automatic).<br>This is the recommended setting for this field because it ensures that the project timeline is always up to date.<br>When you perform an action on a task or project that triggers a timeline recalculation, all available dates are immediately displayed, allowing you to continue working. On projects with more than 100 tasks, dates that require longer recalculations display briefly as a question mark (between 1 and 5 seconds, or up to a minute for large projects). This indicates that the recalculation is not yet finished, and the dates are subject to change.<br></p> </li> 
       </ul> 
       <ul> 
        <li> <p><strong>Change Only</strong>: The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on. You might want to select this option if changes rarely occur in the project or in other projects that the timeline is dependent on.<br></p> </li> 
       </ul> 
       <ul> 
        <li> <p><strong>Automatic Only</strong>: The project timeline is updated each night; it is not updated immediately after changes are made.<br>You might want to select this option if many changes occur each day in the project or in other projects that the timeline is dependent on. However, be aware that you chose this setting, as the project will not update at the same time that the changes are made.<br></p> </li> 
       </ul> 
       <ul> 
        <li> <p><strong>Manual Only</strong>: The project timeline is updated only when you select the option to Recalculate Timelines, as described in <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Recalculate project timelines</a>.<br></p> </li> 
       </ul> <p>You might want to select this option if you are making many changes to the project at one time, and you want the timeline recalculation to occur after all of the changes have been made (rather than after each individual change).</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Schedule</strong> </td> 
      <td> <p>Select a schedule for your template. This will become the schedule of the project that is created from this template. This should be the same schedule assigned to most people that are working on the project. You must create a schedule before you can assign it to a template.<br>For more information about creating schedules, see <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>. <br>If you have not created custom schedules in your system, the Default Schedule is selected. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>User Time Off</strong> </td> 
      <td> <p>Determines whether the time off of the Primary Assignee of a task adjusts the task planned dates. When you attach the template to an existing project, and the template has a different setting for this field than the project, the setting on the project remains unchanged. The default option for this setting for a new template is the same as the system-level project preference. </p> <p>For information about the project preferences at the System level, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>. </p> <p>For information about how this setting affects the task dates on a project, see <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.<br>Select from the following options:<br></p> 
       <ul> 
        <li> <p><strong>Consider user time off in task durations</strong>: When selecting this option, the planned dates of the tasks on the project created from this template adjust according to the time off of the Primary Assignee of the task, if the time off occurs during the duration of the task. </p> </li> 
        <li> <p><strong>Ignore user time off in task durations</strong>: When selecting this option, the planned dates of the tasks on the project created from this template remain as originally planned, even if the Primary Assignee of the task has time off during the duration of the task. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Resource Leveling Mode</strong> </td> 
      <td> <p>Select from the following options:<br></p> 
       <ul> 
        <li> <p><strong>Manual</strong>: you must manually level your resources on the project created from this template (this is the default setting)</p> </li> 
        <li> <p><strong>Automatic:</strong> Workfront levels the resources on the future project. <br>For more information about Resource Leveling, see <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md" class="MCXref xref">Level Resources in the Gantt Chart </a>. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Risk</strong> </td> 
      <td> <p>Define the level of risk of the projects created from this template. The risk is just an indicator of how risky a project can be. You can prioritize the execution of your projects based on the level of risk.<br>Consider selecting from the following levels of risk:<br></p> 
       <ul> 
        <li> <p><strong>Very Low</strong> </p> </li> 
        <li> <p><strong>Low</strong> </p> </li> 
        <li> <p><strong>Medium</strong> </p> </li> 
        <li> <p><strong>High</strong> </p> </li> 
        <li> <p><strong>Very High</strong> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Resource Pools</strong> </td> 
      <td> <p>Specify the resource pools associated with the template. Resource pools are collections of users that are needed at the same time for the completion of a project. For more information about resource pools, see <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Resource pools overview </a>.</p> <p> <p><b>NOTE</b> 
      
      When you edit templates in bulk, only the resource pools that are common to all the templates selected appear in this field. If the templates selected have no shared resource pools, this field will be empty. The resource pools you specify here will overwrite the templates' individual resource pools.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Approval Process</strong> </td> 
      <td> <p>Select the approval process you want to associate with the template. Your Workfront administrator or a user with administrative access to Approval Processes must define system-level or group-level project approval processes before you can associate them with a template. For more information about creating approval processes, see <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Create an approval process for work items</a>.</p> <p>Consider the following when adding approval processes: </p> 
      <ul> 
      <li>Only active approval processes display in the list. </li> 
      <li> <p>System-wide and group-specific approval processes display in the list. An approval process associated with a group other than that of the template does not display in the list.</p> <p><b>IMPORTANT</b> 
      
      If the group associated with the template changes, the group-specific approval process becomes a single-use approval process. For more information about how changes to the group of the project or changes in the approval process affect approval settings, see <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md">How group and approval process changes affect assigned approval processes</a>. </p> </li> 
      <li> <p>If you added a single-use approval process, it displays as "Custom" in this field. For information, see <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">Associate a new or existing approval process with work</a>. </p> 
      </li> 
      <li> <p>When bulk-editing templates, the following scenarios exist:</p> 
      <ul> 
         <li> <p>When you select templates from the same group, both system-level and group-level approval processes display in this field.</p> </li> 
         <li> <p>When you select templates from different groups, only system-level approval processes display in this field.</p> </li> 
         <li> <p>When any of the templates has a single-use approval process attached, it is replaced by the system-level you select. </p> </li> 
      </ul> </li> 
      </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Filter Hour Types</strong> </td> 
      <td> <p>Consider the following:</p> <p>Select <strong>No</strong> to make all project-specific hour types available on the future project. (This is the default selection)</p> <p>Or</p> <p>Select <strong>Yes</strong> to make only a subset of the project-specific hour types available on the future project, then select the hour types you want to make available. (Hold the Shift key to select multiple hour types.)</p> <p>If you select this option, only the hour types you select are made available to select when logging hours on the project (or on tasks and issues within the project). You must select at least one hour type; if you select this option and you do not select any hour types, all hour types are made available on the project.</p> <p>The same hour type selections must be made at the individual user level in order for the user to see these hour type options on the project. </p> <p>For more information about defining hour types at the user level, see the section <a href="../../../timesheets/create-and-manage-timesheets/log-time.md#understa" class="MCXref xref">Log time</a> in <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Log time</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Reminder Notification</strong> </td> 
      <td>Select the Reminder Notification that should be associated with the future project. You must configure Reminder Notifications for projects for this field to appear during editing a template. <br>For more information about configuring Reminder Notifications, see <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Set up reminder notifications</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.  
   Or
1. Click **Save Changes**.

### Access {#access}

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Access**.

   ![Edit template access](assets/edit-template-access-with-tasks-and-issues-350x241.png)

   The Access you specify for your template will become the Access of users associated with the project when the template is used to create a project.

   Specify the following **Access** information for the template:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>When someone is assigned to a task</strong> </td> 
      <td> <p>Select from <strong>View</strong>, <strong>Contribute,</strong> or <strong>Manage</strong> access to a task. The user assigned to a task is automatically granted this access to the task. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Also grant access to the project</strong> </td> 
      <td> <p> Select from <strong>View</strong>, <strong>Contribute</strong>, or <strong>Manage</strong> access to the project. The user assigned to a task is automatically granted this access to the project, as well. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>When someone is assigned to an issue</strong> </td> 
      <td> <p>Select from <strong>View</strong>, <strong>Contribute,</strong> or <strong>Manage</strong> access to an issue. The user assigned to an issue is automatically granted this access to the issue. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Also grant access to the project</strong> </td> 
      <td> <p> Select from <strong>View</strong>, <strong>Contribute</strong>, or <strong>Manage</strong> access to the project. The user assigned to an issue is automatically granted this access to the project, as well. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>When someone submits a request: Give them access</strong> </td> 
      <td> <p> Select from <strong>View</strong>, <strong>Contribute</strong>, or <strong>Manage</strong> access to the request. When they submit a request to the project, they are granted this access to the request they submitted. For more information, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>People from the same company will inherit the same permissions for all requests</strong> </td> 
      <td> <p>Select this field if you want people from the same company to have the same access to all the requests on the project, whether they submitted them or not.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>When someone is given access to this project: Give them access to ...</strong> </td> 
      <td> <p>Select the access options that you want users to have on the project, if the project is shared with them. Select the specific options for their access, if they are designated as <strong>Viewers</strong>, <strong>Contributors</strong>, or <strong>Managers</strong> when sharing the project with them. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.

   Or

   Click **Save Changes**.

### Custom Forms {#custom-forms}

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Custom Forms**.

   ![edit_tempate_custom_forms.png](assets/edit-tempate-custom-forms-tasks-with-issues-sections-350x136.png)

1. Select the custom form or forms that you want to associate with the template. You must build the custom forms before they are available to select in this field.

   Only active custom forms display in the list. s

   You can add up to ten custom forms to a template.

   The forms will be added to the project that is created from this template. 

1. (Optional) Continue editing the following section, depending on the information you want to modify.

   Or

   Click **Save Changes**.

### Tasks {#tasks}

You can define the defaults that will be associated with all the new tasks when you add them to a project that is created from the template.

For information about how these settings affect creating new tasks, see [Create tasks overview](../../../manage-work/tasks/create-tasks/create-tasks-overview.md).

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Tasks**.

   ![Edit template tasks](assets/edit-template-with-tasks-and-issue-sections-350x144.png)

1. In the **Task Default Approval Process** box, select the Approval Process you want to associate with all new tasks when you add them to a project created from this template. You must create an Approval Process for tasks before you can associate it with tasks. Only active approval processes display in the list. For more information about creating Approval Processes, see [Creating Approval Processes](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).
1. In the **Task Default Custom Forms** box, select the custom form or forms that you want to associate with all new tasks when you add them to a project created from this template. You must build the custom forms before they are available to select in this field. Only active custom forms display in the list. You can associate up to ten custom forms with a task.
1. (Optional) **Select Use Work Effort to automatically calculate task Planned Hours** if you want to enable managing task effort by using&nbsp;Work Effort instead of Planned Hours in the project created from the template.
1. (Conditional and optional) If you selected Use Work Effort to automatically calculate task Planned Hours, click the drop-down menu to update the percentage for each level of Work Effort. The following percentage values are the defaults:
 
   | Work Effort level |Percentage value|
   |---|---|
   | Small |25% |
   | Medium |50% |
   | Large |75% |

  For information about using Work Effort to manage the effort on tasks on projects, see [Work Effort overview](../../../manage-work/tasks/task-information/work-effort.md).

1. (Optional) Continue editing the following section, depending on the information you want to modify.

   Or

   Click **Save Changes**.

### Issues {#issues}

By editing issue settings, you can prevent users from adding issues inline in the future project created from the template.

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Issues**.

   ![Edit template issues](assets/edit-template-box-with-issues-nwe-350x171.png)

1. (Optional) Deselect the **Allow users to add issues inline** option. It is enabled by default.

   When disabling this option users cannot add issues inline to the project or the tasks in the Issues section, when the project is created from the template.

   >[!TIP]
   >
   >Disable this option if you want to enforce users to complete the New Issue Fields or the custom forms associated with new issues.

   When disabling this option, users with permissions to add issues to the project created from the template can do so by using the New Issue button or a request queue associated with the project.

   For more information about configuring issue settings on projects, see the [Issue Settings](../../../manage-work/projects/manage-projects/edit-projects.md#issue) section in the article [Edit projects](../../../manage-work/projects/manage-projects/edit-projects.md).

   For information about creating issues on projects, see [Create issues](../../../manage-work/issues/manage-issues/create-issues.md). 

1. (Optional) Continue editing the following section, depending on the information you want to modify.

   Or

   Click **Save Changes**.

### Comment {#comment}

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Comment**.

   ![edit_templates_comment.png](assets/edit-templates-comment-with-tasks-and-issues-350x177.png)

1. Specify a comment that you want to display in the updates stream of the template in the available field.

   This comment is visible for everyone with View access to the template and with access to view Notes.

1. Click **Save Changes**.

   Your changes will be submitted for this template.

   Now, when you use this template to create a project all these settings will transfer to the new project.


   <!--drafted section below for the edit template story: 
   remove this tag and add the Preview blurb at the top of this article in yellow, if it's not already there. Keep the "div class" tags below until 23.1 production: 


### Edit a template in the Preview environment {#edit-a-template-in-the-preview-environment}
-->