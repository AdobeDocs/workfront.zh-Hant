---
product-area: projects
navigation-topic: manage-projects
title: 編輯專案
description: 您可以視需要經常在Adobe Workfront中編輯專案。 理想情況下，當專案處於「計畫」狀態時，您應該編輯專案。
author: Alina
feature: Work Management, Projects
role: User
exl-id: a6a1f178-189a-4c41-835b-7726081a2b49
source-git-commit: 821e31b8c6023a9ec4e017cc5548bb9fd930983c
workflow-type: tm+mt
source-wordcount: '7486'
ht-degree: 1%

---

# 編輯專案

<!--Audited: 01/2024-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

<!--
<p>***Linked to many articles,</p>
<p>The Resource Pools part also duplicates in the "Working with Resource Pools" article </p>
<p>The Update Type section is also documented in Selecting the Project Update Type article</p>
<p>Keep the reference link to the other article that also documents the Update Type) </p>
<p>(NOTE 2: information described here also exists in these articles:</p>
<p>** Project Overview area</p>
<p>**Manage project Finance area</p>
<p>If you need to update just one field, check to see if that field is also listed there and update in both places.)</p>
</div>
-->

您可以視需要經常在Adobe Workfront中編輯專案。 建議您在專案狀態變更為目前後立即編輯專案，藉由傳送有關變更的通知給整個專案團隊，以避免混淆。

理想情況下，當專案處於「計畫」狀態時，您應該編輯專案。 如需有關專案團隊的資訊，請參閱 [專案團隊概述](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## 存取需求

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>新增：標準 </p> 
   或
   <p>目前：計畫 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯專案的存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> 
     <p>管理專案的許可權 </p> 
     <p> 如需有關專案許可權的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">在Adobe Workfront中共用專案</a>.</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 編輯專案的限制

有些限制可能會阻止您編輯專案。

編輯專案時，請考量下列事項：

* 您無法編輯處於核准流程的專案，除非記錄時間並變更狀態。
* 只有在Workfront管理員或群組管理員在專案偏好設定區域中啟用此功能時，您才能將檔案或範本附加至狀態為「完成」、「廢棄」或「擱置核准」的專案。 如需關於設定專案偏好設定的資訊，請參閱 [設定全系統專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* 您只能在處於廢棄或完成狀態的專案上編輯下列資訊：

   * 修改現有費用。
   * 新增、移除或編輯自訂表格。

## 編輯專案

透過編輯專案，您可以修改專案的資訊和設定，以及專案上的任務和問題。

本文中提及的某些設定可能會根據其建立專案之範本中的狀態從預設狀態進行修改。

如需有關編輯範本的資訊，請參閱 [編輯專案範本](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

如需有關從範本建立專案的資訊，請參閱 [使用範本建立專案](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md).

{{step1-to-projects}}

1. （選用）按一下 **我參與的專案** 或 **我擁有的專案** 右上角以顯示您擁有之專案或您身為專案團隊成員的專案。

   ![](assets/projects-on-my-own-buttons-350x302.png)

   >[!NOTE]
   >
   >如果您是群組管理員，則可在「群組」區域以及「專案」區域中看見並編輯群組的專案。 如需詳細資訊，請參閱 [建立和修改群組的專案](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

1. 按一下您要編輯的專案名稱以開啟專案頁面。

1. （選用）若要編輯專案的有限資訊，請按一下 **專案詳細資訊** 在左側面板中。 如果您想要編輯專案的所有相關資訊，請繼續進行步驟5。 <!--accurate?!-->

   ![](assets/nwe-project-details-expanded-350x298.png)

   >[!NOTE]
   >
   >視您的Workfront管理員或群組管理員修改版面配置範本的方式而定，專案詳細資訊區域中的欄位可能會重新排列或不顯示。 如需詳細資訊，請參閱 [使用版面配置範本自訂詳細資料檢視](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   若要編輯「詳細資訊」段落中的資訊，請執行下列動作：

   1. （可選）按一下 **全部收合** 圖示 ![](assets/collapse-icon.png)  以收合所有區域。
   1. （選擇性和條件性）收合區域時，按一下 **向右鍵** ![](assets/right-pointing-arrow.png) 展開每個區域旁的要編輯區域。
   1. 如需有關在專案詳細資訊索引標籤中編輯資訊的詳細資訊，請參閱下列文章：

      * [管理專案概述區域中的資訊](../../../manage-work/projects/manage-projects/understand-project-overview-area.md)
      * [管理專案財務區域的資訊](../../../manage-work/projects/project-finances/manage-project-finance-area.md)

   1. （可選）若要附加自訂表單，請在 **新增自訂表格** 欄位，然後在清單中顯示時選取它，然後按一下 **儲存變更**.
   1. （可選）按一下 **匯出** 圖示 ![](assets/export.png) 若要將概述和自訂表單資訊匯出至PDF檔案，請按一下 **匯出**. 從下列選項中選取：

      * 全選（至少附加一個自訂表單時顯示）
      * 概觀
      * 一或多個自訂表單的名稱

      PDF檔案會下載到您的電腦。

      ![](assets/export-issue-details-selection-box-with-export-button-350x418.png)

      如需詳細資訊，請參閱 [匯出自訂表單和物件詳細資料](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

   如需「專案詳細資訊」區段中可見欄位的相關資訊，請繼續在「編輯專案」方塊中編輯專案，如下所述。
1. 若要編輯專案的所有相關資訊，請按一下 **更多** 功能表 ![](assets/qs-more-menu.png) 在專案名稱旁，然後按一下 **編輯**.

   或

   從專案清單中，選取一或多個專案，然後按一下 **編輯** 圖示 ![](assets/edit-icon.png) 在清單頂端。

   如需大量編輯專案的詳細資訊，請參閱區段 [大量編輯專案](#edit-projects-in-bulk) 本文章內容。

   此 **編輯專案** 方塊開啟。

   >[!IMPORTANT]
   >
   >您必須有專案的管理許可權才能看到編輯選項。

   所有專案欄位都可在「編輯專案」方塊中使用，並按左側面板中列出的區域分組。

   >[!NOTE]
   >
   >視您的Workfront管理員或群組管理員修改版面配置範本的方式而定，編輯專案方塊左側面板中的區域或這些區域中列出的任何欄位可能會重新排列或不顯示。 如需詳細資訊，請參閱 [使用版面配置範本自訂詳細資料檢視](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. （視條件而定）如果您按一下 **更多** 功能表，然後 **編輯**，請更新左側面板所列之下列任一區域中的資訊：

   * [專案名稱](#project-name)
   * [概觀](#overview)
   * [自訂表單](#custom-forms)
   * [財務](#finance)
   * [專案設定](#project-settings)
   * [任務設定](#task-settings)
   * [問題設定](#issue-settings)
   * [存取](#access)

   >[!NOTE]
   >
   >根據您的Workfront管理員為專案的詳細資訊區域設定版面配置範本的方式，您的環境中編輯專案方塊中的區段和欄位可能會不同。 如需詳細資訊，請參閱 [使用版面配置範本自訂詳細資料檢視](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

### 專案名稱 {#project-name}

1. 如上所述開始編輯您的專案。
1. 按一下 **專案名稱** 在左側面板中。

   ![](assets/nwe-project-name-in-edit-project-box-350x125.png)

1. 更新專案名稱。

   大量編輯專案時，您無法編輯專案名稱。

### 概觀 {#overview}

1. 如上所述開始編輯您的專案。
1. 按一下 **概觀** 在左側面板中。

   ![](assets/nwe-overview-in-edit-project-box-350x172.png)

1. 更新下列專案相關資訊：

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
         <td role="rowheader"><strong>說明</strong> </td> 
         <td> <p>新增關於專案的其他資訊。</p> </td> 
      </tr> 
      <tr> 
         <td role="rowheader"><strong>狀態</strong> </td> 
         <td> <p>選取專案狀態。 您無法在所有任務和問題完成之前將專案標籤為完成。 如需有關專案狀態的資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref">存取系統專案狀態清單</a></p> </td> 
      </tr> 
      <tr> 
         <td role="rowheader"><strong>優先順序</strong> </td> 
         <td> <p> <p>這只是一個視覺化的標幟，可讓您排定專案的優先順序。</p> <p>根據Workfront管理員選取的專案偏好設定，您的優先順序名稱可能會不同。 如需有關編輯優先順序的詳細資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">建立和自訂優先順序</a></p> </p> </td> 
      </tr> 
      <tr> 
         <td role="rowheader"><strong>URL</strong> </td> 
         <td> <p>指定與此專案相關資訊的網頁連結。</p> </td> 
      </tr> 
      <tr> 
         <td role="rowheader"><strong>條件型別</strong> </td> 
         <td> <p>在下列條件型別之間選取： 
         <ul> 
         <li><strong>手動：</strong> 專案所有者手動設定專案條件。</li> 
         <li><strong>進度狀態：</strong> Workfront會根據關鍵路徑上任務的進度狀態自動設定條件。 如需瞭解進度狀態的詳細資訊，請參閱 <a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">任務進度狀態總覽</a>.</li> 
         </ul><p>您的Workfront管理員<span> 或群組管理員</span> 選取系統專案狀態計算方式的預設值 <span>或您的群組</span>. 如需有關設定專案預設值的資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">設定全系統專案偏好設定</a>. </p></p> </td> 
      </tr> 
      <tr> 
         <td role="rowheader"><strong>條件</strong> </td> 
         <td> <p> <p>(僅在選取後顯示 <strong>手動</strong> 針對 <strong>條件型別</strong>)：選取「條件」以指出專案進行方式。 </p> <p>如需如何自動或手動設定專案條件的資訊，請參閱 <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">專案狀態與狀態型別概觀</a></p> </p> </td> 
      </tr> 
      <tr> 
         <td role="rowheader"><strong>排程模式</strong> </td> 
         <td> <p>指定專案是從「開始日期」排程，還是從「完成日期」排程。 此選取範圍決定專案上任務的計畫日期。 
         <ul> 
         <li><strong>開始日期</strong>：根據預設，專案的第一個任務的計劃開始日期與專案相同。 有關任務計劃開始日期的資訊，請參閱 <a href="../../../manage-work/tasks/task-information/task-planned-start-date.md" class="MCXref xref">任務計劃開始日期總覽</a>. 專案時間表會從開始日期開始計算，而專案完成日期則由系統根據所有任務的持續時間來計算。 </li> 
         <li><strong>完成日期</strong>：專案的最後一項任務與專案具有相同的規劃完成日期。 專案時間表會從「完成日期」開始計算，而專案的「開始日期」則由系統計算，方法是從專案的「完成日期」減去所有任務的持續時間。 </li> 
         </ul><p>您的Workfront管理員<span> 或群組管理員</span> 選取系統或群組的預設「排程模式」設定。 如需有關設定專案預設值的資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">設定全系統專案偏好設定</a>.</p></p> </td> 
      </tr> 
      <tr> 
         <td role="rowheader"><strong>計劃開始日期和時間</strong> </td> 
         <td> <p> <p>指定選取時的日期 <strong>從開始日期排程</strong>. <br></p> <p>當您選取時，這是唯讀欄位 <strong>從完成日期排程</strong>.<br></p> </p> </td> 
      </tr> 
      <tr> 
         <td role="rowheader"><strong>計畫完成日期和時間</strong> </td> 
         <td> <p>指定選取時的日期 <strong>從完成日期排程</strong>. </p> <p>當您選取時，這是唯讀欄位 <strong>從開始日期排程</strong>.<br></p> </td> 
      </tr> 
      <tr> 
         <td role="rowheader"><strong>專案組合</strong></td> 
         <td>指出專案所屬的Portfolio。 您必須先建立Portfolio，它才會出現在下拉式清單中。 只有作用中的專案組合可以與專案相關聯。 如需關於建立投資組合的詳細資訊，請參閱 <a href="../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md" class="MCXref xref">建立投資組合 </a>.</td> 
      </tr> 
      <tr> 
         <td role="rowheader"><strong>方案</strong></td> 
         <td> <p>如果您為專案選取了Portfolio，請為專案指定計畫。 某些Portfolio可能沒有計畫。 您必須先建立程式，它才會顯示在此下拉式清單中。 只有作用中的方案才能與專案建立關聯。 </p> <p>如需有關建立程式的詳細資訊，請參閱 <a href="../../../manage-work/portfolios/create-and-manage-programs/create-program.md" class="MCXref xref">建立方案</a>.</p> </td> 
      </tr> 
      <tr> 
         <td role="rowheader"><strong>群組</strong></td> 
         <td> <p> <p>指定與專案相關聯的群組名稱。 </p>這是必填欄位。 您無法擁有未與群組相關聯的專案。 </p> <p>您可以將游標移至正確的群組上，並按一下資訊圖示，藉此確定您選取的群組正確 <img src="assets/info-icon.png"> 隨即顯示。 這會顯示工具提示，列出群組的相關資訊，例如群組及其管理員上方的群組階層。</p> 依照預設，除非您指定不同的群組，否則下列其中一個群組會在建立專案時自動與專案相關聯：</p> 
         <ul> 
         <li> <p><span>從專案區域建立專案時，專案建立者的「主群組」會與專案相關聯。</span> </p> <p>從投資組合或計畫中的專案區段建立專案時，也會發生這種情況。</p> </li> 
         <li> <p>從設定區域中群組的主要頁面建立專案時，該群組會與專案相關聯。</p> </li> 
         </ul> </p> <p> <img src="assets/group-details-widget-350x351.png" style="width: 350;height: 351;"> </p> 
         <p><b>附註</b></p>
         <ul>
         <li><p>如果專案或其任務或問題與群組層級自訂狀態相關聯，變更專案群組可能會導致專案狀態、任務或問題變更以符合新群組。</p></li>
         <li><p>如果專案或其任務或問題已使用群組層級自訂狀態與群組層級核准流程相關聯，變更群組可能會在先前群組的核准狀態與系統層級現有的核准狀態之間產生衝突。</p>
         <p>在更新群組之前，請考慮移除專案的群組層級核准流程，或其任務或問題。</p>
         <p>如需有關建立群組層次核准流程的資訊，請參閱 <a href="../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md" class="MCXref xref">群組層級核准流程</a>.</p>
         <p>如需有關建立群組層級自訂狀態的資訊，請參閱 <a href="../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md" class="MCXref xref">建立或編輯群組狀態</a></p></li></ul> </td> 
      </tr> 
      <tr> 
         <td role="rowheader"><strong>公司</strong> </td> 
         <td> <p>指定與專案關聯的公司。 您必須先建立公司，才能將其與專案建立關聯。 只有作用中的公司可以與專案建立關聯。 如需建立公司的詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md" class="MCXref xref">建立和編輯公司</a>.</p> </td> 
      </tr> 
      <tr> 
         <td role="rowheader"><strong>專案所有者</strong> </td> 
         <td> <p>開始輸入使用者的名稱以將其新增至專案，然後在其顯示在清單中時選取它。 使用者會新增至專案團隊，並自動獲得專案的管理許可權。 指定為專案所有者的使用者必須是Workfront作用中使用者。</p>
         </td> 
      </tr> 
      <tr> 
         <td role="rowheader"><strong>專案贊助者</strong> </td> 
         <td> <p>開始輸入使用者的名稱以將其新增至專案，然後在其顯示在清單中時選取它。 使用者會新增至專案團隊，並自動獲得專案的檢視許可權。 指定為專案贊助者的使用者必須是Workfront作用中使用者。<br></p> </td> 
      </tr> 
      <tr> 
         <td role="rowheader"><strong>資源管理員</strong> </td> 
         <td> <p> 開始輸入使用者的名稱以將其新增至專案，然後在其顯示在清單中時選取它們。 使用者會新增至專案團隊，並自動獲得專案的管理許可權，且可指派資源給專案上的任務和問題。 即使使用者從Resource Manager欄位中移除，他們仍保留專案的管理許可權。 您可以指定一個以上的Resource Manager。<br></p> </td> 
      </tr>

   <tr> 
         <td role="rowheader"><strong>轉換的問題建立者</strong> </td> 
         <td> <p> 依預設，此欄位會自動填入建立專案轉換來源問題的使用者名稱。 您可以在Workfront中以任何其他使用者的名稱更新此名稱。 <br></p> </td> 
      </tr>

   </tbody> 
      </table>

   >[!TIP]
   >
   >更新「專案所有者」、「專案贊助者」和「資源管理員」欄位時，請注意顯示圖片、使用者的主要角色或其電子郵件地址，以區分具有相同名稱的使用者。
   >
   >使用者必須至少與一個工作角色相關聯，才能在您新增時檢視該角色。
   >
   >您必須在存取層級中啟用檢視聯絡資訊設定，使用者才能檢視使用者的電子郵件。 如需詳細資訊，請參閱 [授予使用者存取許可權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

1. （選擇性）根據您要修改的資訊，繼續編輯下列區段

   或

   按一下「**儲存**」。

### 自訂表單 {#custom-forms}

根據您的存取層級和您對專案的許可權，以下是不同的情境：

* 如果您沒有專案的編輯自訂表單許可權，您將無法編輯任何附加的自訂表單上的欄位。 您只能檢視附加到專案的自訂表單上的欄位。
* 如果您擁有自訂表單上區段的「檢視」（而非「編輯」）存取權，則無法編輯該區段中的欄位。
* 如果您無權存取附加到專案的其中一個自訂表單上的區段，則該區段不會顯示在「編輯專案」方塊中。

選取多個專案進行大量編輯時，會出現下列情況：

* 如果您沒有至少一個選定專案的編輯自訂表單許可權，則無法編輯任何附加的自訂表單上的欄位。 您只能檢視附加的自訂表單上的欄位
* 如果您擁有自訂表單上區段的「檢視」（而非「編輯」）存取權，則無法編輯該區段中的欄位。 您只能檢視該區段中的欄位。
* 如果您無權存取附加到至少一個專案的其中一個自訂表單上的區段，則該區段不會顯示在「編輯專案」方塊中。
* 如果在附加到所有專案的任何自訂表單上有必填欄位，並且您選擇了一個欄位而沒有實際編輯它，則必須捨棄對該欄位所做的變更或新增資訊到該欄位中，然後才能儲存您選擇的專案。 如果您完全未選取必填欄位，則即使必填欄位為空白，也可以儲存您選取的專案。

如需自訂表格存取許可權的相關資訊，請參閱下列文章：

* [共用自訂表格](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md)
* [新增分割槽符號至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)

若要在編輯專案時編輯自訂表單上的資訊：

1. 如上所述開始編輯您的專案。
1. 按一下 **自訂Forms** 在左側面板中。

   ![](assets/nwe-custom-forms-in-edit-project-box-350x170.png)

1. 按一下 **新增自訂表格** 方塊並從清單中選取一個表單，以將其附加至專案。 依預設，前40個表單會依字母順序顯示。 如果您在清單中沒有看到表單，請開始輸入表單的名稱，然後當表單出現在清單中時選取它。

   >[!NOTE]
   >
   >您必須先建置自訂表單，才能在此欄位中選取它們。 只有作用中的自訂表單會出現在清單中。 如需建立自訂表單的詳細資訊，請參閱 [建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md). 您最多可以新增十個自訂表單至專案。


1. （視條件而定）如果您將自訂表單附加至專案，請編輯表單上的任何欄位。 您必須先指定所有必填欄位，才能儲存專案。
1. （可選）按一下 **X圖示** 在自訂表單名稱右側，將其移除，然後按一下 **移除**.
1. （選擇性）根據您要修改的資訊，繼續編輯下列區段

   或

   按一下「**儲存**」。

### 財務 {#finance}

根據您的存取層級和您對專案的許可權，以下是不同的情境：

* 如果您擁有專案的「檢視財務資料」和「檢視財務」許可權，則只能檢視「財務」區段中的欄位。 您無法編輯此節中的欄位。
* 如果您擁有專案上財務資料的編輯存取權和管理財務許可權，您可以更新此區段中的欄位。

選取多個專案進行大量編輯時，會出現下列情況：

* 如果您選取至少一個您擁有「檢視財務」（而不是「管理財務」）許可權的專案，則只能檢視此區段中所有選定專案的欄位。 您無法大量編輯Finance區段中的欄位。
* 如果您選取至少一個您沒有財務許可權的專案，則此區段完全不顯示。

若要編輯「財務」區域中的欄位：


1. 如上所述開始編輯您的專案。
1. 按一下 **財務** 在左側面板中。

   ![](assets/nwe-finance-in-edit-project-box-350x183.png)

1. 更新專案的下列財務資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>貨幣</strong> </td> 
      <td> <p> <p>如果專案的貨幣與系統的預設貨幣不同，請指定專案的貨幣。 如果專案已經有財務資訊，則您無法變更專案的貨幣。 如果系統中只有預設貨幣，則不會顯示此欄位。 </p> <p>如需貨幣的詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">設定匯率</a>.<br></p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>預算</strong> </td> 
      <td> 指定專案的預算。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>績效指數方法</strong> </td> 
      <td> <p>選取 <b>基於小時</b>，或 <b>基於成本</b> 以指出專案的「已認列值」量度（例如「成本績效指數」或「預估實際成本」）是否使用時數或成本計算。 </p> <p>如需有關績效指數方法的詳細資訊，請參閱 <a href="../../../manage-work/projects/project-finances/set-pim.md" class="MCXref xref">設定績效指數方法(PIM)</a>. </p> <p>您的Workfront管理員<span> 或群組管理員</span> 選取系統或群組的預設「績效指數方法」設定。 如需有關設定專案預設值的資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">設定全系統專案偏好設定</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>預估完成成本</strong> </td> 
      <td> <p> <p>指定Workfront應如何計算預估完成成本(EAC)。 </p>
      從下列選項中選取： 
      <ul><li><b>在專案層級上計算</b></li>
      <li><b>從任務/子任務彙總</b></li> </ul>
      <p>如需有關如何計算「完工估算」的詳細資訊，請參閱 <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref">計算完工估算(EAC)</a>.</p> <p>您的Workfront或群組管理員會為您的系統或群組選取預設的預估完成時間設定。 如需有關設定專案預設值的資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">設定全系統專案偏好設定</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>計畫收益</strong> </td> 
      <td> <p>預估專案的計畫收益。 這用於專案和Portfolio最佳化工具的業務案例。 如需有關專案計畫收益的詳細資訊，請參閱 <a href="../../../manage-work/projects/project-finances/project-planned-benefit.md" class="MCXref xref">專案計畫收益總覽</a>. 計算專案淨值時，會考慮專案的計畫收益。 </p> <p>如需詳細資訊，請參閱 <a href="../../../manage-work/portfolios/portfolio-optimizer/manage-projects-in-portfolio-optimizer.md" class="MCXref xref">在Portfolio最佳化工具中管理專案</a> .<br></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>實際收益</strong> </td> 
      <td> <p>預估專案的實際收益。 這是貨幣金額，代表您的公司或部門在此專案完成後可獲得的利益。 </p> </td> 
     </tr> 
      <tr> 
      <td role="rowheader"><strong>固定成本</strong> </td> 
      <td> <p>指定專案的固定成本。 這與專案時數所產生的人工成本，以及專案費用金額所產生費用成本不同。 計算專案的淨值時會考慮專案的固定成本，而且該成本是預算成本的一部分。<br></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>固定收入</strong> </td> 
      <td> <p>指定專案的固定收入。<br></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （選擇性）根據您要修改的資訊，繼續編輯下列區段。

   或

   按一下「**儲存**」。

### 專案設定 {#project-settings}

1. 如上所述開始編輯您的專案。
1. 按一下 **專案設定** 在左側面板中。

   ![](assets/nwe-project-settings-in-edit-project-box-350x380.png)

1. 更新下列資訊：

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
      <td role="rowheader"><strong>里程碑路徑</strong> </td> 
       <td> <p>選取專案的里程碑路徑。 只有作用中的里程碑路徑會顯示在清單中。</p> <p>如需里程碑路徑的詳細資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">建立里程碑路徑</a>.</p> </td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>完成模式</strong> </td> 
      <td> <p>控制如何將專案標示為完成。 從下列選項中選取： 
       <ul> 
       <li><p><strong>自動</strong>：完成所有任務和問題後，專案會標示為完成。</p><p>專案狀態只有在任務完成時專案狀態為目前時，才會自動變更為完成。 </p></li> 
       <li><strong>手動</strong>：當所有任務和問題完成時，您必須手動選取專案的完成狀態。</li> 
       </ul></p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>摘要完成模式</strong></td> 
       <td> <p>控制如何將父系任務標示為完成。 從下列選項中選取： 
       <ul> 
       <li><strong>自動</strong>：當子系任務完成並更新子系完成百分比時，父系任務會標籤為「完成」並自動更新其完成百分比。 </li> 
       <li><strong>手動</strong>：您必須手動更新完成百分比和父系任務的狀態，不論對子系任務進行什麼變更。 這可讓您標籤已完成父系任務，即使子任務未完成。 </li> 
       </ul></p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>更新類型</strong></td> 
       <td> <p>控制您對專案時間表所做的變更何時儲存在專案或父任務上。 例如，專案的下列變更會觸發專案時間表更新： 
       <ul> 
       <li>更新任務日期</li> 
       <li>變更任務的前置任務關係</li> 
       <li><p>除了變更任務限制或期間型別外，變更父子關係、新增或移除工作分派。</p><p>任務更新時，其父物件（父任務或專案）會在「更新型別」所指示的時間更新。 </p><p>如果在選取「自動與變更時」或「僅變更」更新型別時，父物件未在變更後立即更新，請重新整理頁面</p><p>從下列選項中選取： </p><p>- <strong>自動與變更時</strong> （預設設定）：每次在專案或專案所依存之其他專案中發生變更時（變更時），都會更新專案時間表。 專案時間表也會每晚更新（自動）。</p><p>這是此欄位的建議設定，因為它可確保專案隨時保持最新。</p><p>當您對觸發時間表重新計算的任務或專案執行動作時，所有可用日期會立即顯示，讓您繼續工作。 在具有100個以上任務的專案中，需要更長重新計算的日期會短暫顯示為問號（1到5秒之間，大型專案最多會顯示一分鐘）。 這表示重新計算尚未完成，日期可能會變更。</p><p>- <strong>僅變更</strong>：每次在專案或專案所依存的其他專案中發生變更時，專案時間表都會更新。 如果變更很少發生在專案或時間表所依賴的其他專案中，您可能會想要選取此選項。</p><p>- <strong>僅限自動</strong>：專案時間表會每晚更新；變更後不會立即更新時間表。</p><p>如果每天在專案或時間表相依的其他專案中發生許多變更，您可能會想要選取此選項。 但是，請注意，您選擇了此設定，因為專案不會在進行變更的同時更新。</p><p>- <strong>僅限手動</strong>：專案時間表只有在您選取「重新計算時間表」選項時才會更新。 如需手動重新計算專案時間表的相關資訊，請參閱 <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">重新計算專案時間表</a>. </p><p>如果您一次對專案進行許多變更，且希望在所有變更完成後（而不是在每次個別變更後）重新計算時間表，則可能需要選取此選項。</p></li> 
       </ul></p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>排程</strong> </td> 
       <td> <p>選取專案的排程。 這應該是指派給大多數處理專案的人的相同排程。 您必須先建立排程，才能將其指派給專案或使用者。 如果您尚未在系統中建立自訂排程，則會選取「預設排程」。</p> <p>如需建立排程的詳細資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">建立排程</a>. </p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>使用者休假</strong> </td> 
       <td> <p>決定任務的主要受指派人的休假是否調整專案上的任務計畫日期。 </p><p>您的Workfront管理員<span> 或群組管理員</span> 為您的系統選取此設定的預設值 <span>或您的群組</span>. 如需有關設定專案預設值的資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">設定全系統專案偏好設定</a>. </p><p>從下列選項中選取：<br>- <strong>考量使用者在任務持續期間的休假</strong>：選取此選項時，如果休假發生在任務持續期間，則任務的計畫日期會根據任務的主要受指派人的休假而調整。 </p><p>例如，如果一項限製為「儘快」的任務排程在6月1日開始並在6月3日完成，而主要受指派人已在6月2日標示為「休假」，則啟用此選擇時，任務計畫日期為6月1日至6月4日。 根據「任務限制」，下列案例會存在： </p> 
       <ul> 
       <li>對於與計畫起始日期相關的作業限制（儘快、最早可用時間、開始時間不得早於、開始時間不得晚於、必須開始於），計畫起始日期不會變更，但計畫完成日期會變更。</li> 
       <li>對於與從完成日期開始的計畫相關的作業限制（儘可能遲、最晚可用時間、完成時間不得早於、完成時間不得晚於、完成時間不得晚於），計畫完成日期不會變更，但計劃開始日期會變更。</li> 
       <li>對於具有固定日期限制的任務，「計劃開始日期」和「完成日期」都不會變更。 </li> 
       </ul><p>當您選取此設定時，工作的持續時間不會變更。 根據任務限制，只有計畫日期會變更。 有關任務限制的資訊，請參閱 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">任務限制總覽</a>. </p><p>- <strong>忽略使用者在任務持續期間的休假</strong>：選取此選項時，即使任務的主要受指派人在任務持續期間有休假，專案上任務的計畫日期仍保持原始計畫。 </p><p>選取此設定的選項時，請考量下列事項：</p> 
       <ul> 
       <li><p>新專案的此設定預設選項與系統層級專案偏好設定相同。 </p><p>有關系統層級專案偏好設定的資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">設定全系統專案偏好設定</a>. </p></li> 
       <li>將範本附加到現有專案時，專案上的設定會更新以符合其中一個範本。 </li> 
       <li><p>Workfront會根據任務的任務限制值決定要調整哪些計畫任務日期。 根據具體情況，計劃開始日期或計畫完成日期（或兩者）可能會受到影響，或甚至可能維持相同。 例如，如果任務具有固定日期的限制時，即使在 <strong>考量使用者在任務持續期間的休假</strong> 已選取。 </p></li> 
       </ul></td> 
      </tr> 
      <tr> 
       <td role="rowheader"><strong>資源平準模式</strong> </td> 
       <td> <p> <p>從下列選項中選取：</p> <p>- <strong>手動</strong>：您必須手動平準資源（此為預設設定）</p> <p>- <strong>自動</strong>：Workfront會調整您的資源層級。</p> <p>如需資源平準的詳細資訊，請參閱 <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md" class="MCXref xref">在甘特圖中平準資源 </a>.</p> </p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"><strong>風險</strong> </td> 
       <td> <p> <p>定義專案的風險等級。 風險只是專案風險程度的指標。 您可以根據風險等級來排定執行專案的優先順序。</p> <p> <p>考慮從下列風險等級中選取：</p> <p> — 極低</p> <p> — 低</p> <p> — 中</p> <p> — 高</p> <p> — 非常高</p> <p>您無法自訂您在此指出的風險等級。</p> <p>這些風險與專案存續期間可能發生的潛在風險無關，您應該在專案的「風險」標籤或「業務案例」中記錄這些風險。 有關潛在專案風險的資訊，請參閱 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/edit-create-risk-types.md" class="MCXref xref">編輯和建立風險型別</a>. </p> </p> </p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"><strong>資源集區</strong> </td> 
       <td> <p> <p>指定與專案關聯的資源集區。 資源集區是使用者集合，需要同時完成專案並允許在資源規劃工具中編列專案預算。 如需有關資源集區的詳細資訊，請參閱 <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> 資源集區概觀 </a>. </p> <p>當您大量編輯專案時，此欄位中只會出現所有選定專案通用的資源集區。 如果選取的專案沒有共用資源集區，此欄位將為空白。 您在此指定的資源集區將覆寫專案的個別資源集區。</p> </p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <strong>允許公司層級的收費率覆寫專案層級的收費率</strong></td> 
       <td>選取此選項可允許公司層級的收費率覆寫歷史職務角色費率，除非這些費率標示為已記帳。 啟用此選項會覆寫歷史職務角色費率，除非將它們標籤為已記帳。 <br>如需詳細資訊，請參閱 <a href="../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md" class="MCXref xref">以公司層級的收費率覆寫專案層級的收費率</a>.</td> 
      </tr> 
      <tr> 
       <td role="rowheader"><strong>此專案需要時間核准</strong></td> 
       <td> <p> 選取此選項可要求專案所有者核准登入專案的時間。 如果您使用「計費記錄」並選取此選項，則只有專案中已核准的時數，才會顯示為「計費記錄」的可用計費時數。 核准專案的時間與核準時程表無關。 </p> <p>如需有關專案需要時間核准的詳細資訊，請參閱 <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" class="MCXref xref">專案需要時間核准</a>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"><strong>篩選小時型別</strong> 和</span> <strong>小時型別</strong></td> 
       <td> <p> <p>從下列選項中選取：</p> 
       <ul> 
       <li> <p>選取 <strong>否</strong> 讓專案可用的所有特定專案小時型別。 （這是預設選取範圍）</p> <p>或</p> </li> 
       <li>選取 <strong>是</strong> 若只要讓專案特定時數型別的子集可在專案上使用，則從「 」中選擇您想要提供使用的時數型別 <b>小時型別</b> 欄位。</li> 
       <p><b>秘訣</b></p>
       <p>此 <b>小時型別</b> 當您選取時，欄位不可編輯 <b>否</b>.</p> 
       <p>如果您選取此選項，則在記錄專案時數（或專案內任務和問題）時，只有您選取的時數型別可供選取。 您必須至少選取一個小時型別；如果您選取此選項而未選取任何小時型別，則專案上將會提供所有小時型別。</p> </ul>

   <p>必須在個別使用者層級做出相同的小時型別選擇，以便使用者在專案上檢視這些小時型別選項。 如需在使用者層級定義時數型別的詳細資訊，請參閱 <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">記錄時間</a>. </p> </p> </td> 
      </tr> 
      <tr data-mc-conditions=""> 
       <td role="rowheader"><strong>提醒通知</strong> </td> 
       <td> <p> <p>選取應與專案關聯的提醒通知。 您必須為專案設定提醒通知，此欄位才能在編輯專案期間顯示。 如需有關設定提醒通知的詳細資訊，請參閱 <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md"><a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">設定提醒通知</a> .</a></p> </p> </td> 
      </tr> 
      <tr data-mc-conditions=""> 
       <td role="rowheader"><strong>核准流程</strong></td> 
       <td> <p>選取您要與專案關聯的核准流程。 您的Workfront管理員必須定義系統層級的核准流程，您才能將其與專案建立關聯。 <span>擁有核准流程管理存取許可權的使用者也可以建立群組特定的核准流程。</span> 如需有關建立核准流程的詳細資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">建立工作專案的核准流程</a>.</p> <p>新增核准程式時，請考量下列事項： </p> 
       <ul> 
       <li>清單中只會顯示有效的核准流程。 </li> 
       <li> <p>系統範圍及群組特定的核准程式會顯示在清單中。 與專案群組以外的群組相關聯的核准程式不會顯示在清單中。</p> <p>如果與專案相關聯的群組變更，群組特定的核准流程會變成單一使用的核准流程。 如需關於專案群組變更或核准流程變更如何影響核准設定的詳細資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">群組和核准流程變更如何影響指派的核准流程</a>. </p> </li> <!--(NOTE: this bullet stays here although the sections it might appear in are QS only, so we can use the snippet for both Qs and classic)-->
       <p>大量編輯專案時，會出現下列情況：</p> 
       <ul> 
       <li> <p>當您從相同群組選取專案時，系統層次和群組層次核准流程都會顯示在此欄位中。</p> </li> 
       <li> <p>當您從不同的群組選取專案時，此欄位中只會顯示系統層級的核准流程。</p> </li> 
       <li> <p>當任何專案附加單一使用核准程式時，您選取的系統層次或群組層次核准程式會取代該程式。 </p> </li> 
      </ul> </td> 
      </tr> 
      <tr> 
      </tr> 
      </tbody> 
      </table>

1. （選擇性）根據您要修改的資訊，繼續編輯下列區段。

   或

   按一下「**儲存**」。

### 任務設定 {#task-settings}

您可以定義預設值，在將新任務新增至專案時，這些預設值將與所有新任務相關聯。

如需這些設定如何影響建立新工作的詳細資訊，請參閱區段 [將任務新增至專案時的任務預設值](../../../manage-work/tasks/create-tasks/create-tasks-overview.md#understa) 在文章中 [建立任務總覽](../../../manage-work/tasks/create-tasks/create-tasks-overview.md).

1. 如上所述開始編輯您的專案。
1. 按一下 **任務設定** 在左側面板中。

   ![](assets/nwe-task-settings-in-edit-project-box-350x211.png)

1. 在 **任務預設核准流程** 方塊中，選取當您新增至專案時，要與所有新任務關聯的任務「核准流程」。

   您的Workfront管理員（或具有核准流程管理存取許可權的使用者）必須先為任務建立系統層級或群組層級的核准流程，您才能將其與專案相關聯。 清單中只會顯示有效的核准流程。 如需有關建立核准流程的資訊，請參閱 [建立工作專案的核准流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md). 有關專案群組的變更或核准流程中的變更如何影響核准設定的資訊，請參閱 [群組和核准流程變更如何影響指派的核准流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md).

   大量編輯專案時，會出現下列情況：

   * 當您從相同群組選取多個專案時，系統層次與群組特定作業核准流程都會顯示在此欄位中。
   * 當您從不同的群組選取多個專案時，此欄位中只會顯示系統層級的作業核准流程。

1. 在 **任務預設自訂Forms** 方塊中，選取當您新增至專案時，要與所有新任務產生關聯的一或多個自訂表單。 您必須先建置自訂表單，才能在此欄位中選取它們。 清單中只會顯示作用中的自訂表單。 如需建立自訂表單的詳細資訊，請參閱 [建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md). 您最多可以將十個自訂表單與任務建立關聯。
1. （選用）選取 **使用工作量自動計算任務計畫時數** 如果您想透過使用工作量而不是計畫時數來啟用管理工作量。

   ![](assets/nwe-work-effort-on-projects-350x182.png)

1. （條件式與選擇性）如果您選取使用工作量自動計算作業計畫時數，請按一下每個工作量層次的下拉式功能表，並選取每個層次的百分比。 下列百分比值為預設值：

   | 大小 | 百分比 |
   |---|---|
   | 小 | 25% |
   | 中 | 50% |
   | 大 | 75% |

   >[!TIP]
   >
   >當專案更新型別設定為自動且您選取此設定時，任務的計畫時數會根據任務持續期間和工作投入百分比（如果它們設定為零）進行更新。 如需有關使用工作量計畫任務之工作量的詳細資訊，請參閱 [工作投入概觀](../../../manage-work/tasks/task-information/work-effort.md).

1. （選擇性）根據您要修改的資訊，繼續編輯下列區段。

   或

   按一下「**儲存**」。

### 問題設定 {#issue-settings}

1. 如上所述開始編輯您的專案。
1. 按一下 **問題設定** 在左側面板中。

   ![](assets/nwe-issue-settings-in-edit-project-box-350x306.png)

1. （可選）取消選取 **允許使用者新增內嵌問題** 選項。 預設會選取此選項。

   取消選取此選項時，使用者無法將內聯問題新增到專案或問題區段中的任務。

   >[!TIP]
   >
   >如果您要強制使用者完成新問題欄位或與新問題相關聯的自訂表單，請取消選取此選項。 讓使用者輸入問題內嵌，可讓他們在建立問題時略過「新問題」欄位和自訂表單。 如需有關設定欄位和新問題的自訂表單的資訊，請參閱 [建立請求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

   取消選取此選項時，擁有將問題新增至專案或任務之許可權的使用者可以透過以下方式進行：

   * 按一下專案或任務的問題區段中，問題清單頂端的「新增問題」 。
   * 當專案設定為請求佇列時，他們可以在請求區域中輸入新請求。

   >[!NOTE]
   >
   >當大量編輯專案時，如果至少有一個專案已啟用此設定，則會啟用此設定；如果所有選取的專案都已停用，則會停用此設定。

   <!--drafted for bulk edit projects: the statement above needs to be corrected when the new UI for bulk edit projects is updated; not sure if we'll need to describe this at all or we can cover this in  a "Considerations" mini section inside the Editing in bulk section below- ??? -->

1. （選擇性）根據您要修改的資訊，繼續編輯下列區段。

   或

   按一下「**儲存**」。

### 存取 {#access}

1. 如上所述開始編輯您的專案。
1. 按一下 **存取** 在左側面板中。

   ![](assets/nwe-access-in-edit-project-box-350x262.png)

1. 指定下列專案 **存取** 專案資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>將某人指派給任務時</strong></td> 
      <td><p>選取自 <strong>檢視</strong>， <strong>Contribute，</strong> 或 <strong>管理</strong> 任務的存取權。 指派給任務的使用者會自動被授予此任務的存取權。</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>同時授與專案的存取權</strong></td> 
      <td><p>選取自 <strong>檢視</strong>， <strong>Contribute</strong>，或 <strong>管理</strong> 專案的存取權。 指派給任務的使用者也會自動被授予此專案的存取權。<br></p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>將某人指派給問題時</strong></td> 
      <td><p>選取自 <strong>檢視</strong>， <strong>Contribute，</strong> 或 <strong>管理</strong> 存取問題。 指派給問題的使用者會自動被授予此問題的存取權。 如需詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">共用問題 </a>.<br></p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>同時授與專案的存取權</strong></td> 
      <td><p>選取自 <strong>檢視</strong>， <strong>Contribute</strong>，或 <strong>管理</strong> 專案的存取權。 指派給問題的使用者也被自動授予此專案的存取權。<br></p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>某人提交請求時：授予他們存取權</strong></td> 
      <td><p>選取自 <strong>檢視</strong>， <strong>Contribute</strong>，或 <strong>管理</strong> 請求的存取權。 當專案也是請求佇列並且使用者向專案提交請求時，他們被授予對他們提交的請求的這種存取權。 如需將專案設定為請求佇列的詳細資訊，請參閱 <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">建立請求佇列</a>.<br></p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>來自相同公司的人員將針對所有要求繼承相同權限。</strong></td> 
      <td><p>如果您希望來自相同公司的人員擁有專案上所有請求的相同存取權（無論他們是否提交請求），請選取此欄位。<br></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>某人獲得此專案的存取權時：表示預設的存取權……</strong></td> 
      <td><p>選取您希望使用者在專案上擁有的存取選項（如果專案已與他們共用）。 如果指定為，則選取其存取權的特定選項 <strong>檢視者</strong>， <strong>貢獻者</strong>，或 <strong>管理員</strong> 與他們共用專案時。 </p><p>此 <strong>刪除</strong> 中的存取權 <strong>管理</strong> 許可權層級會決定是否允許使用者刪除專案本身。 使用者 <strong>管理</strong> 存取專案可以刪除專案中的任務和問題，無論是否選取此選項（如果有的話） <strong>管理</strong> 任務和問題的許可權。 </p></td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下「**儲存**」。

### 連結的資料夾

連結資料夾功能會自動在Adobe Experience Manager Assets中建立資料夾，並將這些資料夾連結至Workfront。

只有符合下列所有條件時，才會顯示此區段：

* 您的組織已移轉至Adobe Admin Console
* 您的組織已啟用並設定與Adobe Experience Manager的整合
* 用來建立此專案的範本已啟用並設定了連結資料夾。

如需有關編輯連結資料夾的說明，請參閱 [編輯專案中的工作流程值](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md#edit-workflow-values-in-a-project) 在文章中使用工作流程在Experience Manager Assets整合。

>[!NOTE]
>
>由於連結資料夾是在建立專案時建立的，因此編輯現有專案上的連結資料夾工作流程會無效。 在建立專案時按預期編輯這些值。

## 在專案標題中編輯專案（受限）

您可以編輯專案標題中的有限資訊量。

您的系統或群組管理員可以自訂您在專案標題中看到的欄位。

![](assets/project-header-350x18.png)

預設情況下，下列欄位會包含在專案標題中。

* 專案名稱
* 完成百分比
* 專案所有者
* 計畫完成日期和時間

  >[!NOTE]
  >
  >只有當專案是從「完成日期」開始排程時，您才能編輯此欄位。 從開始日期開始排程專案時，Workfront會根據任務的持續期間計算規劃完成日期和時間。

* 狀況

  >[!NOTE]
  >
  >僅當專案的條件型別為手動時，才能編輯此欄位。 當「條件型別」設定為「進度狀態」時，Workfront會根據任務的進度計算條件。 如需詳細資訊，請參閱 [專案狀態與狀態型別概觀](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

* 狀態
* 如果您在目前的核准程式中設為核准者，請進行核准決定

## 大量編輯專案

您可以大量編輯專案，並同時更新所有選定專案的資訊。

大量編輯專案時，請考慮下列事項：

* 您正在選取的所有專案上變更的資訊會覆寫個別專案的現有資訊，但Resource Manager欄位除外。

  在大量編輯專案時新增資源管理員會將該管理員新增到所有選取的專案。 如果其他資源管理員與所選專案相關聯，則除了透過大量編輯新增的專案外，這些資源管理員還會保留在專案上。

* 當您為相同欄位選取具有不同值的專案時，該欄位會在「編輯專案」方塊中顯示「多個值」指示器。 核取方塊、選項按鈕和切換的欄位旁邊會有一個「多個值」指示器。

  ![](assets/multiple-values-indicator-dates-bulk-edit-projects.png)

* 除了「多個值」指標外，當至少有一個選定專案上的選定選項不同時，具有多個選項的欄位會以下列其中一種方式顯示：

   * 核取方塊欄位中會有一行，而不是針對已勾選部分而非所有選定專案的選項勾選的核取方塊。

     ![](assets/multiple-values-indicator-check-boxes-bulk-edit-projects.png)

   * 切換型別欄位會顯示為暗灰色，且中間會有一個切換選項，該選項已啟用部分而非所有選定專案。

  ![](assets/multiple-values-highlighted-bulk-edit-projects.png)

   * 已選取部分選項但不是全部選項的單選按鈕型別欄位，會將所有單選按鈕顯示為空白。

     ![](assets/multiple-values-indicator-radio-buttons-bulk-edit-projects.png)

* 當您在多選項欄位（例如顯示為一組切換或核取方塊的欄位）中更新一個選項時，所選專案之間的所有其他選項必須相符。

  >[!IMPORTANT]
  >
  >例如，您可能會有一個核取方塊欄位，其中包含三個核取方塊（「選項1」、「選項2」及「選項3」），且所有專案的「選項1」都會取消勾選，部分專案的「選項2」及「選項3」也會取消勾選，其他您選取的專案則會取消勾選。 如果您要核取所有專案的選項1，您還必須使選項2和3符合所有選取的專案，然後才能儲存變更，因此您必須選取或取消選取它們，以便它們在所有選取的專案上相符。 如果您未變更任何選項，您可以依原樣儲存欄位，而專案會保留其所有選項的目前選擇。

* 當您選取屬於不同群組的多個專案時，「狀態」欄位中顯示的狀態是系統層級狀態，而不是群組層級狀態。

若要大量編輯專案：

{{step1-to-projects}}

1. 在清單中選取數個專案。
1. 按一下 **編輯** 圖示 ![](assets/edit-icon.png) 在清單頂端。
此 **編輯專案** 對話方塊開啟。

   ![](assets/edit-projects-in-bulk-modal-unshimmed.png)

視您的Workfront管理員或群組管理員修改版面配置範本的方式而定，編輯專案方塊左側面板中的區域或這些區域中列出的任何欄位可能會重新排列或不顯示。 如需詳細資訊，請參閱 [使用版面配置範本自訂詳細資料檢視](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. 按一下 **概觀** 以編輯所選專案的一般資訊。  如需有關編輯「概述」區域的詳細資訊，請參閱區段 [概觀](#overview) 本文章內容。

   >[!TIP]
   >
   >您編輯的欄位會以淺紫色背景顯示。

1. 按一下 **自訂Forms** 編輯、新增或取代與所選專案相關聯的自訂表單。

   附加到所有選定專案的自訂表單會顯示在 **通用的自訂表單** 中的子區段 **自訂Forms** 區域。

   ![](assets/custom-forms-in-common-unshimmed.png)

   >[!TIP]
   >
   >   所有選定專案通用的表單名稱會顯示在「編輯專案」方塊的左側面板中。

1. 開始在中輸入自訂表單的名稱 **新增自訂表格** 欄位。


   ![](assets/forms-already-attached-indication-in-bulk-editing-projects-unshimmed.png)

   已附加到所選專案的自訂表單會顯示在 **附加的表單** 中的子區段 **新增自訂表格** 欄位。

   可與專案相關聯但未附加至任何選定專案的其他自訂表單會顯示在 **要新增的Forms** 中的子區段 **新增自訂表格** 欄位。

1. 按一下以選取中的其他自訂表格 **新增自訂表格** 或 **要新增的Forms** 子區段（當它顯示在清單中時）。

   當自訂表單已附加到某些所選專案時，表單名稱旁邊會顯示新增表單時已附加表單的專案數量。

1. （可選）按一下 **x** 圖示並按一下「 」，接著按一下「 」 **移除** 以將其從所有選取的專案中移除。

   >[!CAUTION]
   >
   >移除自訂表單會導致表單上所有現有的自訂欄位資訊遺失。 無法復原此錯誤。

   如需編輯自訂表單的詳細資訊，請參閱區段 [自訂Forms](#custom-forms) 本文章內容。

1. 按一下 **財務** 以編輯所有選取專案的財務資訊。
如需有關編輯「財務」區域的詳細資訊，請參閱區段 [財務](#finance) 本文章內容。
1. 按一下 **專案設定** 以編輯所有選定專案的設定。
如需有關編輯「專案設定」區域的詳細資訊，請參閱區段 [專案設定](#project-settings) 本文章內容。
1. 按一下 **任務設定** 以編輯所有選定專案的工作設定。
如需有關編輯「工作設定」區域的詳細資訊，請參閱區段 [任務設定](#task-settings) 本文章內容。
1. 按一下 **問題設定** 以編輯所有選定專案的問題設定。
如需有關編輯問題設定區域的詳細資訊，請參閱區段 [問題設定](#issue-settings) 本文章內容。
1. 按一下 **存取** 以編輯所有選取專案的存取設定。
如需有關編輯「存取」區域的詳細資訊，請參閱區段 [存取](#access) 本文章內容。
1. （可選）若要移除您在「編輯專案」方塊中新增的任何資訊，請將游標移至已編輯的欄位上，然後按一下 **x** 捨棄欄位右上角的圖示。

   ![](assets/discard-icon-for-field-edit-projects-in-bulk-unshimmed.png)

1. （選用）按一下 **取消** 在底部 **編輯專案** 頁面以移除對所有專案進行的所有變更。
1. 按一下「**儲存**」。


<!-- Old information for how to bulk edit in classic/ before project bulk edit redesign: 

### Edit projects in bulk in the Production environment

To edit projects in bulk:

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront.

1. Click **Projects**.  
1. Select several projects in the list.
1. Click **Edit**.

   The **Edit Projects** dialog box opens.

   ![](assets/edit-projects-in-bulk-nwe-350x303.png)

1. Specify the information on all selected projects in the following sections:

   * **Overview**

     For information, see the [Overview](#overview) section in this article.
   
   * **Finance**

     For information, see the [Finance](#finance) section in this article.
   
   * **Portfolio**

     For information, see the "Project association" section in the [Overview](#overview) section in this article.
   
   * **Settings**

     For information, see the [Project Settings](#project-settings) section in this article.
   
   * **Access**

     For information, see the [Access](#access) section in this article.
   
   * **Custom Forms**

     For information, continue with step 7 below.

     <!--   
     <p>(NOTE:&nbsp;make sure this stays accurate)</p>   
     

   * **Tasks**

     For information, see the [Task Settings](#task-settings) section in this article.
   
   * **Issues**

     For information, see the   [Issue Settings](#issue-settings) section in this article.
   
   * **Comment**

     For information, continue with step 9 below.

     <!--   
     <p>(NOTE: ensure this step stays accurate)</p>   
     


1. (Optional) In the Settings area, select any of the following options:

   * **Recalculate Costs and Revenues**: Select this option to recalculate Costs and Revenues on all projects selected.
   * **Recalculate Timelines**: Select this option to recalculate the Timelines of all projects selected.
   * **Recalculate Scorecards**: Select this option to recalculate the Scorecard values for all projects selected.

   ![recalculate_costs__scorecards__etc_in_bulk_edit_for_projects.PNG](assets/recalculate-costs--scorecards--etc-in-bulk-edit-for-projects-350x225.png)

1. Click **Custom Forms** to edit the custom forms attached to all the projects selected.

   If the projects selected do not have any common custom forms, no forms are listed in this section.

   You can edit only the fields on the forms that are attached to all projects selected and which you have permissions to edit. 

1. (Optional) In the Custom Forms section, select the **Recalculate Custom Expressions** option to ensure that all Calculated Custom Fields that are on the Custom Forms attached to the projects selected are up to date.

   >[!IMPORTANT]
   >
   >We recommend not to select more than 500 projects at a time when you recalculate custom expressions.

1. (Optional) Click **Comment**, then select the Post an update to each project box and specify a comment that you want to display in the updates stream of the project in the available field and do one of the following:

   * Click the **People** icon ![](assets/people-icon-updates-classic.png) to tag a user who will be notified about your comment.
   * Click the **Lock** icon ![](assets/lock-icon-open-updates-classic.png) to restrict your comment only to people within your company.

   This comment is visible for everyone with View access to the project and with access to view Notes.

1. Click **Save Changes**.

   All changes you made are now visible on all the selected projects.

-->