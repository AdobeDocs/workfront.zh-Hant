---
navigation-topic: use-lists
title: 開始使用 [!DNL Adobe Workfront]中的清單
description: 您可以檢視 [!DNL Adobe Workfront] 中的物件清單，以取得有關物件的資訊，例如它們的開始和到期日、指派給它們的使用者，以及與它們關聯的其他物件。
feature: Get Started with Workfront
author: Lisa
exl-id: d4262b8e-bbe0-4ac2-8f1f-5d32541311c8
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '2397'
ht-degree: 0%

---

# 開始使用[!DNL Adobe Workfront]中的清單

<!--
{{highlighted-preview}}
-->

您可以檢視[!DNL Adobe Workfront]中的物件清單，以取得它們的相關資訊，例如它們的開始和到期日、指派給它們的使用者，以及與它們關聯的其他物件。

以下是[!DNL Workfront]中清單的某些特性：

* 清單每五分鐘自動重新整理一次，以更新系統中其他使用者在其他地方更新的資訊。
* [!DNL Workfront]中的某些區域已預先設定預設的物件清單。

  您可以自訂這些預先設定的清單中的大部分。

* [!DNL Workfront]管理員可以建立自訂清單，以套用至[!DNL Workfront]的各個區域。

  如需有關建立系統層級清單的詳細資訊，請參閱文章[建立、編輯和共用預設篩選器、檢視和群組](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-and-share-default-fvgs.md)。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計畫*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權*</strong></td> 
   <td> <p>[！UICONTROL Request]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>存取層級設定*</strong></td> 
   <td> <p>[！UICONTROL檢視]或更高的篩選器、檢視、群組存取權</p> <P>對於[！UICONTROL設定]區域中的專案，您需要該專案的管理存取權或[！UICONTROL系統管理員]存取層級。</P> <p>注意：如果您還是沒有存取權，請詢問您的[!DNL Workfront]管理員是否對您的存取層級設定了其他限制。<br>如需[!DNL Workfront]管理員如何變更存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件許可權</strong></td> 
   <td> <p>[！UICONTROL檢視]或具有共用存取權的更高許可權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td>
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

## 物件清單

以下是您可以在[!DNL Workfront]中找到的一些物件清單型別，以及當您有權檢視物件時，預設會顯示這些清單的一些區域。

>[!NOTE]
>
>* 此清單並不完整。 這些物件清單中的每一份也都會出現在報表或儀表板上。 例如，包含專案報告的專案報告或控制面板也會顯示專案清單。
>* 在此清單中，「選取」表示您需要按一下專案名稱，而不是按一下名稱左邊的核取方塊。


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>[!DNL Workfront] 清單</strong></th> 
   <th><strong>物件清單的位置</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>投資組合清單</td> 
   <td> 
    <ul> 
     <li> <p>[！UICONTROLPortfolio]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>計劃清單</td> 
   <td> 
    <ul> 
     <li> <p>[！UICONTROLPortfolio] &gt;[！UICONTROL選取投資組合] &gt;[！UICONTROL計畫]</p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>[！UICONTROL程式]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>專案清單</td> 
   <td> 
    <ul> 
     <li> <p>[！UICONTROL專案]</p> </li> 
     <li> <p>[！UICONTROLPortfolio] &gt;[！UICONTROL選取投資組合] &gt;[！UICONTROL專案]</p> </li> 
     <li> <p>[！UICONTROLPortfolio] &gt;[！UICONTROL選取投資組合] &gt;[！UICONTROL計畫] &gt;[！UICONTROL選取計畫] &gt;[！UICONTROL專案]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>任務清單</td> 
   <td> 
    <ul> 
     <li> <p>[！UICONTROL專案] &gt;[！UICONTROL選取專案] &gt; [！UICONTROL任務]</p> </li> 
     <li> <p>[！UICONTROL專案] &gt;[！UICONTROL選取專案] &gt;[！UICONTROL任務] &gt;[！UICONTROL選取任務] &gt;[！UICONTROL子任務]</p> </li> 
     <li> <p>[！UICONTROL專案] &gt;[！UICONTROL選取專案] &gt;[！UICONTROL任務] &gt;[！UICONTROL選取任務] &gt; [！UICONTROL前置任務*]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>問題清單</td> 
   <td> 
    <ul> 
     <li> <p>[！UICONTROL專案] &gt; [！UICONTROL Select]專案&gt;[！UICONTROL問題]</p> </li> 
     <li> <p>[！UICONTROL專案] &gt;[！UICONTROL選取專案] &gt;[！UICONTROL任務] &gt;[！UICONTROL選取任務] &gt; [！UICONTROL問題]</p> </li> 
     <li> <p>[！UICONTROL專案] &gt;[！UICONTROL選取專案] &gt;[！UICONTROL任務] &gt;[！UICONTROL選取任務] &gt;[！UICONTROL子任務] &gt;[！UICONTROL選取任務] &gt; [！UICONTROL問題]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>報告清單</td> 
   <td> 
    <ul> 
     <li> <p>  [！UICONTROL報表]  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>控制面板清單</td> 
   <td> 
    <ul> 
     <li> <p>[！UICONTROL儀表板]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>反複專案清單</td> 
   <td> 
    <ul> 
     <li> <p>[！UICONTROL團隊] &gt; [！UICONTROL反複專案]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>使用者清單</td> 
   <td> 
    <ul> 
     <li> <p>[！UICONTROL使用者]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>檔案清單</td> 
   <td> 
    <ul> 
     <li> <p>[！UICONTROL檔案]</p> </li> 
     <li> <p>[！UICONTROLPortfolio] &gt;[！UICONTROL選取投資組合] &gt; [！UICONTROL檔案]</p> </li> 
     <li> <p>[！UICONTROLPortfolio] &gt; [！UICONTROL選擇產品組合] &gt;[！UICONTROL計畫] &gt;[！UICONTROL選擇計畫] &gt;[！UICONTROL檔案]</p> </li> 
     <li> <p>[！UICONTROL專案] &gt;[！UICONTROL選取專案] &gt;[！UICONTROL檔案]</p> </li> 
     <li> <p>[！UICONTROL專案] &gt;[！UICONTROL選取專案] &gt;[！UICONTROL任務] &gt;[！UICONTROL選取任務] &gt; [！UICONTROL檔案]</p> </li> 
     <li> <p>[！UICONTROL專案] &gt; [！UICONTROL選取專案&gt; [！UICONTROL問題] &gt;[！UICONTROL選取問題] &gt; [！UICONTROL檔案]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>時程表清單</td> 
   <td> 
    <ul> 
     <li> <p>[！UICONTROL時間表] &gt; [！UICONTROL所有時間表]*</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>收費率清單</td> 
   <td> 
    <ul> 
     <li> <p>[！UICONTROL專案] &gt;[！UICONTROL選取專案] &gt;[！UICONTROL收費率*]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>付費記錄清單</td> 
   <td> 
    <ul> 
     <li> <p>[！UICONTROL專案] &gt; [！UICONTROL選取專案] &gt; [！UICONTROL付費記錄]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>風險清單</td> 
   <td> 
    <ul> 
     <li> <p>[！UICONTROL專案] &gt;[！UICONTROL選取專案] &gt;[！UICONTROL風險]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>費用清單</td> 
   <td> 
    <ul> 
     <li> <p>[！UICONTROL專案] &gt;[！UICONTROL Select]專案&gt;[！UICONTROL費用]</p> </li> 
     <li> <p>[！UICONTROL專案] &gt; [！UICONTROL選取專案] &gt;[！UICONTROL任務] &gt;[！UICONTROL選取任務] &gt;[！UICONTROL費用]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>小時專案清單</td> 
   <td> 
    <ul> 
     <li> <p>[！UICONTROL專案] &gt;[！UICONTROL選取專案</p> </li> 
     <li> <p>[！UICONTROL專案] &gt;[！UICONTROL選取專案] &gt;[！UICONTROL任務] &gt;[！UICONTROL選取任務] &gt;[！UICONTROL小時]</p> </li> 
     <li> <p>[！UICONTROL專案] &gt;[！UICONTROL select]專案&gt;[！UICONTROL問題] &gt;[！UICONTROL select]問題&gt;[！UICONTROL小時]</p> </li>
    </ul> </td> 
  </tr>
  <tr> 
   <td class="preview">自訂表單清單</td> 
   <td> 
    <ul> 
     <li class="preview"> <p>[！UICONTROL安裝程式] &gt;[！UICONTROL自訂Forms]</p>
     <!--Remove the following note box when this goes to Production. Or do this when the Preview highlighting becomes available.-->
     <p><b>注意</b>：目前僅可在預覽環境中使用</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td>群組或子群組清單</td> 
   <td> 
    <ul> 
     <li> <p>[！UICONTROL設定] &gt;[！UICONTROL群組]</p> </li>
     <li> <p>[！UICONTROL設定] &gt;[！UICONTROL群組] &gt;[！UICONTROL選取父群組] &gt;[！UICONTROL子群組] </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>團隊清單</td> 
   <td> 
    <ul> 
     <li> <p>[！UICONTROL設定] &gt;[！UICONTROL團隊]</p> </li> 
    </ul> </td> 
  </tr>
  <tr> 
   <td>公司清單</td> 
   <td> 
    <ul> 
     <li> <p>[！UICONTROL設定] &gt;[！UICONTROL公司]</p> </li> 
    </ul> </td> 
  </tr>
  <tr> 
   <td>排程清單</td> 
   <td> 
    <ul> 
     <li> <p>[！UICONTROL設定] &gt;[！UICONTROL排程]</p> </li> 
    </ul> </td> 
  </tr>
  <tr> 
   <td>版面配置範本清單</td> 
   <td> 
    <ul> 
     <li> <p>[！UICONTROL安裝程式] &gt;[！UICONTROL配置範本]</p> </li> 
    </ul> </td> 
  </tr>
 </tbody> 
</table>

您無法自訂指定區域的清單。 [!DNL Workfront]管理員可以在系統層級建立自訂清單，或者，如果您的存取層級允許您編輯報告，則可以為此物件建立報告。

## 清單元素

清單包含定義其格式的特定元素以及顯示的資訊。 您可以找到數個預設可用的系統清單元素。 您也可以建立符合您需求的自訂元素。

>[!NOTE]
>
>當您從清單中選取新的篩選器、檢視或群組時，即使您登出[!DNL Workfront]或關閉瀏覽器，該選取仍會保留。

以下是清單的元素：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>元素</strong></th> 
   <th><strong>說明</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>[！UICONTROL篩選器]</strong></td> 
   <td> <p>篩選器會根據您指定的條件，將不必要的資訊排除在清單之外。 </p> <p>如需詳細資訊，請參閱<a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">篩選器總覽</a>。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>[！UICONTROL檢視]</strong></td> 
   <td> <p>檢視會定義要在熒幕上顯示的欄位（欄）。</p> <p>如需詳細資訊，請參閱[!DNL Adobe Workfront]</a>中的<a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">檢視總覽。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>[！UICONTROL群組]</strong></td> 
   <td> <p>群組會根據您指定的條件，將清單中的物件區分為不同的區域。</p> <p>例如，清單中的問題可依狀態或優先順序顯示在區段中。</p> <p>在標準群組中最多可以有三層群組，如果您在文字模式中配置群組，則可以新增第四層。</p> <p>如需群組的詳細資訊，請參閱[!DNL Adobe Workfront]</a>中的<a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">群組概觀。</p> <p>如需文字模式的詳細資訊，請參閱<a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md" class="MCXref xref">文字模式概觀</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

依預設，這些元素會顯示在每個清單的頂端。 它們是粘性的，而且不會在您捲動清單時移動。 將滑鼠移至每個元素的圖示上以識別它們。

![](assets/nwe-list-elements.png)

您可以自訂下列區域中的清單元素，並與其他使用者共用它們：

* 在文章的[開始使用 [!DNL Adobe Workfront]](#default-workfront-lists)中的清單一節中找到任何系統預設清單
* 與您共用的任何報告

清單的建置元素與報表的建置元素相同。

如需有關建立和自訂清單與報表的建置元素的詳細資訊，請參閱[報表元素：篩選器、檢視和群組](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)。

## 列出動作

您可以在清單中完成下列動作：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>動作</strong></th> 
   <th><strong>信息</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>內嵌編輯</strong> </td> 
   <td> <p>直接在清單中編輯物件及其資訊。</p> <p>如需詳細資訊，請參閱<a href="../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md" class="MCXref xref">在[!DNL Adobe Workfront]</a>的清單中內嵌編輯專案。</p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><strong>更新為[！UICONTROL摘要]</strong> </td> 
   <td> <p>使用[！UICONTROL摘要]面板更新專案層級的任務和問題。</p> <p>提示： 「摘要」並非適用於所有物件，且無法在「任務」或「問題」報告中使用。</p> <p>如需詳細資訊，請參閱<a href="../../../workfront-basics/the-new-workfront-experience/summary-overview.md" class="MCXref xref">摘要概觀</a>。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>自訂清單顯示</strong> </td> 
   <td> <p>自訂清單的外觀和感覺、欄的排列、專案的排序順序或顯示的專案數。</p> <p>注意：當您登出[!DNL Workfront]或關閉瀏覽器時，您對要在頁面上顯示的專案數所做的變更將會還原。 變更也可能會在8小時後回覆。</p> <p>如需詳細資訊，請參閱<a href="../../../workfront-basics/navigate-workfront/use-lists/modify-list-display.md" class="MCXref xref">修改清單的顯示方式</a>。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>快速篩選</strong> </td> 
   <td> <p>套用快速篩選以僅尋找對您重要的專案，以便您快速檢閱、更新或與他人共用這些專案。</p> <p>重要：您可以使用快速篩選來尋找包含搜尋字詞的專案，無論該專案是否顯示在您的熒幕上，或是在您捲動至頁面底部之後顯示。 使用瀏覽器的搜尋功能時，您只能找到畫面上已顯示的專案。 如果您的清單有多個頁面，快速篩選器只會尋找目前頁面上的專案。</p> <p>如需詳細資訊，請參閱<a href="../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md" class="MCXref xref">將快速篩選套用至清單</a>。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>匯出</strong> </td> 
   <td> <p>從[!DNL Workfront]匯出物件清單。 當清單包含超過2000個專案時，匯出清單是檢閱一個頁面上所有專案的唯一方法。</p> <p>如需匯出清單的詳細資訊，請參閱<a href="../../../workfront-basics/navigate-workfront/use-lists/export-lists.md" class="MCXref xref">匯出清單</a>。 如需匯出格式和限制的詳細資訊，請參閱<a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">匯出資料</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 清單工具列

下表列出工具列中許多可用的圖示，並指出當您按一下這些圖示時，會發生什麼情況：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>圖示</strong></td> 
   <td><strong>說明</strong></td> 
   <td><strong>按一下</strong></td> 
  </tr> 
  <tr> 
   <td> <img src="assets/add-icon-plus-in-circle.png"> </td> 
   <td>[！UICONTROL新增專案或使用者]</td> 
   <td>開啟更多選項，包括新增專案或使用者。</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-insert-task-above-icon-in-new-toolbar.png"> </td> 
   <td>[！UICONTROL在上方插入任務]</td> 
   <td> <p>在選取的工作上方插入工作。</p> <p>這僅適用於任務。 </p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-insert-task-below-icon-in-new-toolbar.png"> </td> 
   <td>[！UICONTROL在下方插入任務]</td> 
   <td> <p>在選取的工作下方插入工作。</p> <p>這僅適用於任務。 </p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/edit-icon.png"> </td> 
   <td>[！UICONTROL編輯]</td> 
   <td>編輯選取的專案。</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/copy-icon.png"> </td> 
   <td>[！UICONTROL副本]</td> 
   <td>複製選取的專案。</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/delete.png"> </td> 
   <td>[！UICONTROL Delete]</td> 
   <td>刪除選取的專案。</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-add-to-iteration-icon-in-new-toolbar-for-issues.png"> </td> 
   <td>[！UICONTROL新增至]</td> 
   <td> <p>開啟對話方塊，將選取的問題新增至反複專案。</p> <p>這僅適用於問題。</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/share-icon.png"> </td> 
   <td>[！UICONTROL Share]</td> 
   <td>共用選取的專案。</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-indent-outdent-tasks-icon-in-new-toolbar.png"> </td> 
   <td>[！UICONTROL縮排和凸排任務] </td> 
   <td> <p>縮排或縮排選取的工作。 </p> <p>這僅適用於任務。 </p> </td> 
  </tr> 
  <tr> 
   <td><img src="assets/more-icon.png"></a> </td> 
   <td>[！UICONTROL更多]</td> 
   <td>開啟所選專案的其他選項。</td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/search-icon.png"> </p> </td> 
   <td> <p>[！UICONTROL快速篩選] </p> </td> 
   <td> <p>開啟快速篩選搜尋方塊，以尋找顯示的清單中的專案。</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/export.png"> </td> 
   <td>[！UICONTROL Export]</td> 
   <td>將清單匯出為PDF、Excel或定位字元分隔的檔案。</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-agile-icon-in-new-toolbar-task-list.png"> </td> 
   <td>[！UICONTROL敏捷檢視]</td> 
   <td>在敏捷檢視中顯示清單。<br>這僅適用於工作。</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-gantt-chart-icon-in-new-toolbar.png"> </td> 
   <td>[！UICONTROL甘特圖]</td> 
   <td> <p>在[！UICONTROL甘特圖]檢視中顯示清單。</p> <p>這僅適用於專案和任務。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-filter-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-filter-in-new-toolbar-with-blue-dot---small.png"> </p> </td> 
   <td>[！UICONTROL篩選器]下拉式功能表</td> 
   <td> <p>顯示篩選器清單以及管理篩選器的其他選項，包括建立篩選器。 </p> <p>在小熒幕上，篩選器名稱會由篩選器圖示取代。 當您套用「[！UICONTROL All]」以外的任何篩選器時，「篩選器」圖示上會顯示一個藍點。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-view-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-view-in-new-toolbar-with-blue-dot.png"> </p> </td> 
   <td>[！UICONTROL檢視]下拉式功能表</td> 
   <td> <p>顯示檢視清單以及管理檢視的其他選項，包括建立檢視。 </p> <p>在小熒幕上，檢視名稱會由[！UICONTROL檢視]圖示取代。 當您套用「[！UICONTROL標準]」以外的任何檢視時，「[！UICONTROL檢視]」圖示上會顯示一個藍點。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-grouping-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-grouping-in-new-toolbar-with-blue-dot.png"> </p> </td> 
   <td>[！UICONTROL Grouping]下拉式功能表</td> 
   <td> <p>顯示群組清單以及管理群組的其他選項，包括建立群組。 </p> <p>在小熒幕上，群組名稱會被[！UICONTROL群組]圖示取代。 當您套用「[！UICONTROL Nothing]」以外的任何分組時，[！UICONTROL Grouping]圖示上會顯示一個藍點。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-autosave-icon-in-new-toolbar-for-tasks.png"> </td> 
   <td> <p>[！UICONTROL計畫模式]</p> </td> 
   <td> <p>選擇您要自動或手動儲存您在工作清單中所做的變更。 </p> <p>如需有關編輯清單中工作的資訊，請參閱<a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md" class="MCXref xref">編輯清單中的工作</a>。 </p> <p>這僅適用於任務。</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/summary-panel-icon.png"> </td> 
   <td>[！UICONTROL摘要]</td> 
   <td> <p>顯示或隱藏所選專案的[！UICONTROL摘要]方塊。</p> <p>這僅適用於任務和問題。</p> <p>如需新[!DNL Adobe Workfront]體驗中[！UICONTROL摘要]面板的相關資訊，請參閱<a href="/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md" class="MCXref xref">摘要概觀</a>。</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/remove-icon---x-in-circle.png"> </td> 
   <td>[！UICONTROL移除]</td> 
   <td>從清單中移除某些專案。 例如，作為管理群組或子群組成員資格的群組管理員，請依照<a href="/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md" class="MCXref xref">檢視和管理群組成員資格</a>中的說明移除群組成員。</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/comment-icon.png"> </td> 
   <td>[！UICONTROL Comment] /[！UICONTROL Update]</td> 
   <td> <p>輸入註解或更新。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 清單與報告之間的差異

清單和報表都是包含物件型別相關資訊的格點。

下表概述清單與報告之間的異同：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>功能</strong> </th> 
   <th><strong>清單</strong> </th> 
   <th><strong>報告</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>任何人都能建立這些檔案</p> </td> 
   <td>✓ <span>*</span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>只有[!DNL Workfront]管理員和具有[！UICONTROL Plan]授權的使用者可以建立他們</p> </td> 
   <td> </td> 
   <td>✓ **</td> 
  </tr> 
  <tr> 
   <td> <p>預設集可從以下位置取得： [!DNL Workfront]</p> </td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td> <p>可在標準模式下自訂</p> </td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td> <p>可在文字模式中自訂</p> </td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td> <p>您可以與其他使用者共用</p> </td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td> <p>您可在系統內共用這些區段</p> </td> 
   <td>✓ (A)</td> 
   <td> ✓ (A) </td> 
  </tr> 
  <tr> 
   <td> <p>您可以在系統外部共用它們</p> </td> 
   <td> </td> 
   <td>✓ (A) </td> 
  </tr> 
  <tr> 
   <td> <p>您可以匯出為.pdf、[!DNL Excel]和Tab字元分隔格式</p> </td> 
   <td>✓ (A)</td> 
   <td> ✓ (A) </td> 
  </tr> 
  <tr> 
   <td> <p>您可以排程在電子郵件中傳送</p> </td> 
   <td> </td> 
   <td>✓ (A) </td> 
  </tr> 
  <tr> 
   <td> <p>您可以新增到版面範本</p> </td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>您可以將其新增到自訂部分 </p> </td> 
   <td> </td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td> <p>您可以將它們新增到儀表板</p> </td> 
   <td> ✓ *** </td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td> <p>您可以使用提示來自訂它們顯示的內容</p> </td> 
   <td> </td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td> <p>您可以在圖表中顯示它們</p> </td> 
   <td> </td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td> <p>您可以內嵌編輯物件</p> </td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
 </tbody> 
</table>

您必須有權存取篩選器、檢視和群組，才能建立它們。 如需詳細資訊，請參閱[授予篩選器、檢視和群組的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md)。

您必須有權存取篩選器、檢視和群組以及報告、儀表板和行事曆，才能建立它們。 如需詳細資訊，請參閱[授予報告、儀表板和行事曆的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)。

只有在報表建立者將清單元素設定為在控制面板上顯示時，您才能自訂置於控制面板上的報表清單。

>[!NOTE]
>
>您必須先建立報表並將其新增至控制面板，才能將清單新增至控制面板。

如需建立報告的詳細資訊，請參閱[建立自訂報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。 如需有關建立自訂區段的資訊，請參閱[建立自訂標籤或區段](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md)。

## 更新清單和舊版清單之間的差異

[!DNL Workfront]中有兩種型別的清單：

* 舊版清單

  ![](assets/legacy-list-screen-shot-blue-groupings-350x101.png)

* 更新的清單

  ![](assets/updated-list-screen-shot-gray-groupings-350x71.png)

兩種型別的清單都出現在[!DNL Adobe Workfront]中。

[!DNL Adobe Workfront]中的所有清單和報告都會更新，以下清單除外：

* 在[!UICONTROL 設定]區域中的清單
* 在[!UICONTROL 報表]區域中的清單

下表顯示[!DNL Workfront]中舊版與更新清單之間的部分差異：

<!--
<span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> [Legacy does not equal Classic. Legacy lists appear in NWE and Classic. Updated lists appear in NWE and Classic.]</span>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>舊版清單</b></td> 
   <td><b>更新的清單</b></td> 
  </tr> 
  <tr> 
   <td> <p>舊版字型、欄標題、藍色群組色彩配置</p> </td> 
   <td> <p>更新字型、欄標題、灰色群組色彩配置</p> </td> 
  </tr> 
  <tr> 
   <td> <p>較緩慢的內嵌編輯</p> </td> 
   <td> <p>更快速的內嵌編輯</p> </td> 
  </tr> 
  <tr> 
   <td> <p>依預設顯示<strong>100</strong>個專案</p> </td> 
   <td> <p>依預設顯示<strong>所有</strong>或最多<strong>2000</strong>個專案</p> </td> 
  </tr> 
  <tr> 
   <td> <p>使用CTRL+F尋找清單中的專案</p> </td> 
   <td> <p>使用快速篩選器快速尋找大型清單中的資訊</p> <p>如需有關在清單中使用快速篩選的資訊，請參閱<a href="../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md" class="MCXref xref">將快速篩選套用至清單</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>您無法內嵌編輯具有RTF格式的自訂欄位。</td> 
   <td> <p>自訂欄位中含格式的文字可設定為允許粗體、斜體、底線、專案符號、編號、超連結和區塊引號。</p> <p>如需詳細資訊，請參閱<a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">建立或編輯自訂表格</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>條件式格式可以變更清單中連結的文字顏色</td> 
   <td>無法套用文字顏色變更至清單中的連結</td> 
  </tr> 
 </tbody> 
</table>
