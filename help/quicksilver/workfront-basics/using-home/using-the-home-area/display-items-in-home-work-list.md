---
product-area: projects
navigation-topic: use-the-home-area
title: 在首頁區域的[!UICONTROL 工作清單]中顯示專案
description: '[!UICONTROL 首頁]區域中的[!UICONTROL 工作清單]會顯示指派給您的所有工作專案。 您可以透過使用篩選器以及對您的工作專案進行分組和排序，來控制哪些專案顯示在[!UICONTROL 工作清單]中。'
author: Nolan
feature: Get Started with Workfront, Work Management
exl-id: eac2e065-9e32-43c1-90ff-0f841b508c35
source-git-commit: d614d5cbded1de6fd899a47495a6e058f9eaf3cf
workflow-type: tm+mt
source-wordcount: '1843'
ht-degree: 0%

---

# 在[!UICONTROL 首頁]區域的[!UICONTROL 工作清單]中顯示專案

<!-- Audited: 1/2024 -->


[!UICONTROL 首頁]區域中的[!UICONTROL 工作清單]會顯示指派給您的所有工作專案。 您可以透過使用篩選器以及對您的工作專案進行分組和排序，來控制哪些專案顯示在[!UICONTROL 工作清單]中。

>[!NOTE]
>
>* 將問題轉換為任務或專案時，問題會從指派給問題的使用者的首頁區域移除。
>
>* 將任務轉換為專案時，任務會被刪除，並從指派給任務的使用者的「首頁」區域中移除。


## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan]</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權</strong></td> 
   <td> <p>新增：</p><ul><li>[！UICONTROL參與者]僅供核准</li> <li>適用於所有其他物件的[！UICONTROL Standard]或更新版本</li> <p>或</p> 
  </ul><p>目前：</p><ul><li>[！UICONTROL Review]僅供核准</li> <li>適用於所有其他物件的[！UICONTROL Work]或更新版本</li> </td> 
  </tr> </ul>
  <tr> 
   <td role="rowheader"><strong>存取層級設定</strong></td> 
   <td> <p>[！UICONTROL檢視]或更高的專案、任務、問題和檔案存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件許可權</strong></td> 
   <td> <p>您需要處理的任務和問題的Contribute許可權或更高版本</p>  </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 篩選[!UICONTROL 工作清單]

您可以篩選[!UICONTROL 工作清單]中的專案，以僅檢視特定型別的專案。 例如，您可以篩選[!UICONTROL 工作清單]以僅顯示問題或請求。

>[!NOTE]
>
>篩選器選項會儲存在瀏覽器中。 如果您在相同的電腦上持續使用相同的瀏覽器（且不清除網站資料），則選取的篩選器不會變更。 如果您切換瀏覽器或電腦，則篩選器會還原為預設選項，該選項會取消選取所有篩選器。

1. 按一下Adobe Workfront右上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon.png)，或（如果有的話）按一下左上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon-left-nav.png)，然後按一下&#x200B;**[!UICONTROL 首頁]**。
1. 按一下&#x200B;**[!UICONTROL 篩選器]** ![](assets/filter-nwepng.png)下拉式功能表。 如果您已選取任何篩選器，則選取的篩選器數會取代圖示顯示。
1. 從下列篩選選項中選取，以指定要顯示的專案型別：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL All]</strong></td> 
      <td>顯示並選取所有專案。 這包括任務、問題、核准、個人任務，以及已完成的任務和問題。 </td>
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL任務：處理]</strong></td> 
      <td> <p>僅顯示您正在處理的任務。 這些是指派給您已按一下[！UICONTROL處理它]按鈕的任務。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL工作：準備開始]</strong></td> 
      <td> 
       <div> 
        <p>僅顯示已準備好要啟動的任務。 下列兩個陳述式都必須為true：</p> 
        <ul> 
         <li> <p>任務及其父項沒有前置任務或任務限制而無法處理。</p> </li> 
         <li> <p>所有前置任務已完成。</p> </li> 
         <li> <p>任務的[！UICONTROL規劃開始日期]是過去或未來最多兩週。</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL工作：未就緒]</strong></td> 
      <td> 
       <div> 
        <p>僅顯示尚未準備開始的任務。 下列其中一個陳述式必須為true：</p> 
        <ul> 
         <li> <p>任務及其父項可能具有前置任務或任務限制，使其無法處理。</p> </li> 
         <li> <p>這些任務的[！UICONTROL計劃開始日期]在未來的兩週以上。</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL問題：處理]</strong></td> 
      <td> <p>僅顯示您正在處理的問題。 這是指派給您的問題，而您已按一下[！UICONTROL處理它]按鈕。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL問題：已要求]</strong></td> 
      <td>僅顯示已指派給您但尚未按一下[！UICONTROL處理它的問題]按鈕。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>個人</strong></td> 
      <td>僅顯示個人工作。 如文章<a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md">從[！UICONTROL首頁]區域建立工作專案</a>中的<a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#create-a-personal-task">建立個人工作</a>一節所述，這些是您建立為[！UICONTROL待辦事項]的工作。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL核准]</strong></td> 
      <td> 
       <div> 
        <p>僅顯示指派給您或已委派的核准，以及您已提交的核准。 核准包括工作專案（專案、任務和問題）的核准，以及檔案、校樣、存取請求和時程表的核准。 如需核准的詳細資訊，請參閱下列文章：</p> 
        <ul> 
         <li><a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">檢視核准</a> </li> 
        </ul> 
        <ul> 
         <li> <p><a href="../../../review-and-approve-work/manage-approvals/manage-approvals.md" class="MCXref xref">工作核准</a> </p> </li> 
        </ul> 
        <p>備註：您提交且同時也是核准者之一的核准會計算兩次。</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL Delegated： Delegated by me]</strong></td> 
      <td> 
       <div> 
        <p>僅顯示您已委派給其他使用者的工作專案。</p> 
        <p>如需委派工作的詳細資訊，請參閱<a href="/help/quicksilver/manage-work/delegate-work/how-to-delegate-work.md#delegate-tasks-and-issues-to-another-user" class="MCXref xref">將工作與問題委派給其他使用者</a>。
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL已委派：已委派給我]</strong></td> 
      <td> 
       <div> 
        <p>僅顯示其他使用者暫時委派給您的工作專案。</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL已完成]</strong></td> 
      <td> <p>僅顯示已完成的任務、問題和個人任務。 已完成的工作會顯示前兩週，並會根據其完成所在的周分組到「工作清單」中。 不包含核准。</p> <p>已完成的工作會隱藏在[！UICONTROL工作清單]中，除非您選取此篩選器。</p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

   >[!TIP]
   >
   >* 篩選選項是根據物件（任務、問題、核准、個人任務）。
   >* 任務和問題會依據其狀態進一步篩選，其中狀態與處理它們的準備程度相關（[!UICONTROL 處理]、[!UICONTROL 準備開始]、[!UICONTROL 未就緒]工作，以及[!UICONTROL 處理]和[!UICONTROL 要求]問題）。 您可以選擇顯示特定狀態的任務或問題，或按一下任務或問題以選擇並顯示所有狀態。
   >* 已完成專案有單獨的篩選器，其中同時包含任務和問題。 這不包括核准。 [!UICONTROL 已完成]篩選器包含個人工作。
   >* 您可以選取一次只顯示一個狀態。 例如，您只能顯示[!UICONTROL 正在處理]個任務，且只能顯示[!UICONTROL 已請求的]個問題。 您也可以一次選取多個狀態。
   >* 您無法對指派給您其中一個團隊的專案套用篩選器，且團隊指派不會包含在直接指派給您的專案中。


1. （選擇性）進一步組織[!UICONTROL 工作清單]，如本文章的[群組一節中所述，並依日期、專案和優先順序](#group-and-sort-by-date-project-and-priority)排序。

## 群組並依[!UICONTROL 日期]、[!UICONTROL 專案]和[!UICONTROL 優先順序]排序

您可以依[!UICONTROL 計畫完成日期]、[!UICONTROL 認可日期]、[!UICONTROL 專案]或[!UICONTROL 我的優先順序]，將[!UICONTROL 工作清單]群組並排序。 您選擇的選項決定專案在[!UICONTROL 工作清單]中的群組方式。

1. 按一下Adobe Workfront右上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon.png)，或（如果有的話）按一下左上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon-left-nav.png)，然後按一下&#x200B;**[!UICONTROL 首頁]**。
1. 按一下「**[!UICONTROL 分組依據]**」![「分組依據](/help/quicksilver/workfront-basics/using-home/using-the-home-area/assets/grouping-28x19.png)」下拉式功能表。

   <!--
   ![](assets/group-by-drop-down-expanded-in-home-with-planned-start-date-nwe-350x273.png)
   -->

1. 從下列選項中選取：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL計畫完成]</strong></td> 
      <td> <p> 專案會根據其[！UICONTROL計畫完成日期] （每個群組內包含的專案數會顯示在標題標題旁的括弧中），顯示在[！UICONTROL工作清單]的下列群組中：</p> 
       <ul> 
        <li> <p>[！UICONTROL Late]</p> </li> 
        <li> <p>[！UICONTROL無計畫完成日期]</p> </li> 
        <li> <p>[！UICONTROL本週]</p> <p>依預設，此分組是展開的。</p> </li> 
        <li> <p>[！UICONTROL下週]</p> </li> 
        <li> <p>[！UICONTROL已計畫]，接著是各種[！UICONTROL計畫完成日期] （多個群組）</p> </li> 
        <li> <p>[！UICONTROL完成]</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL計劃開始]</strong></td> 
      <td> <p>專案會根據其[！UICONTROL計劃開始日期] （[！UICONTROL工作清單]中每個群組所包含的專案數會顯示在標題標題旁的括弧中），依下列群組顯示：</p> 
       <ul> 
        <li> <p>[！UICONTROL Late]</p> </li> 
        <li> <p>[！UICONTROL本週] </p> <p>依預設，此分組是展開的。</p> </li> 
        <li> <p>[！UICONTROL下週]</p> </li> 
        <li> <p>[！UICONTROL已計畫]，接著是各種[！UICONTROL計劃開始日期] （多個群組）</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL認可日期]</strong></td> 
      <td> <p>專案顯示在[！UICONTROL工作清單]的下列群組中（每個群組中包含的專案數會顯示在標題標題旁的括弧中）：</p> 
       <ul> 
        <li> <p>[！UICONTROL無認可日期]</p> </li> 
        <li> <p>[！UICONTROL下週認可]</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL專案]</strong></td> 
      <td>專案會根據專案分組，且專案會在[！UICONTROL工作清單]中依字母順序顯示。 （每個群組中包含的專案數會顯示在標題標題旁的括弧中。）</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL我的優先順序]</strong></td> 
      <td>專案會依您選擇的順序顯示。 如需詳細資訊，請參閱<a href="../../../workfront-basics/using-home/using-the-home-area/prioritize-work-in-home.md" class="MCXref xref">在[！UICONTROL首頁]區域排定工作優先順序</a>。</td> 
     </tr> 
    </tbody> 
   </table>

>[!NOTE]
>
>預設排序為升序。 如果您將排序變更為降序，則所選的排序選項會儲存在瀏覽器中。 如果您一律在同一部電腦上使用相同的瀏覽器（且不清除網站資料），排序不會變更，但如果您切換瀏覽器或電腦，則排序會變更為預設排序。

## 檢視延遲專案

[!DNL Adobe Workfront]會使用以下日期來判斷工作請求是否延遲：

* **任務**： [!UICONTROL 計畫完成日期]
* **問題**： [!UICONTROL 規劃完成日期]
* **檔案**： [!UICONTROL 提交日期]
* **時程表**：[!UICONTROL 提交日期]
* **核准**： [!UICONTROL 提交日期]
* **校訂核准**： [!UICONTROL 校訂期限]

## 搜尋[!UICONTROL 工作清單]

當您搜尋[!UICONTROL 工作清單]時，指派給您的任何專案都會傳回至搜尋中（甚至包括目前未載入在畫面上的專案）。 如果選取[!UICONTROL 顯示完成]選項，系統也會傳回您在過去兩週內標示為完成的任何專案。

此外，只搜尋工作專案的名稱（不會搜尋工作專案內的資訊，也不會搜尋工作專案所在的專案名稱）。

若要搜尋[!UICONTROL 工作清單]：

1. 按一下Adobe Workfront右上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon.png)，或（如果有的話）按一下左上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon-left-nav.png)，然後按一下&#x200B;**[!UICONTROL 首頁]**。
1. （選擇性）篩選及群組[!UICONTROL 工作清單]，如[中所述。篩選[!UICONTROL 工作清單]](#filter-the-work-list)及[群組，並依日期、專案及優先順序](#group-and-sort-by-date-project-and-priority)排序。

1. （選擇性）如果您要搜尋已完成的工作專案，您必須將[!UICONTROL 工作清單]設定為先顯示已完成的專案，然後再進行搜尋。

1. 按一下「搜尋」圖示![搜尋](/help/quicksilver/workfront-basics/using-home/using-the-home-area/assets/search-icon.png)。
1. 開始輸入您要搜尋的專案名稱。\
   [!UICONTROL 工作清單]會自動篩選為包含具有相符名稱的專案。

## 變更工作清單的大小

您可以變更[!UICONTROL 工作清單]的大小，使其在「首頁」區域約四分之一到[!UICONTROL 首頁]區域約一半之間的任何地方使用。

1. 按一下Adobe Workfront右上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon.png)，或（如果有的話）按一下左上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon-left-nav.png)，然後按一下&#x200B;**[!UICONTROL 首頁]**。
1. 將滑鼠移至[!UICONTROL 工作清單]的右邊緣上方，然後向左或向右拖曳，直到工作清單達到所需大小為止。

## 摺疊和展開群組

[!UICONTROL 工作清單]中的專案會顯示在群組內。 您可以摺疊和展開群組，以控制特定時間頁面上顯示的資訊量。

您可以在[!UICONTROL 工作清單]內摺疊和展開群組，以便更好地控制顯示哪些資訊。\
依預設，[!UICONTROL 本週]群組是展開的，而所有其他群組則是摺疊的。 您所做的任何變更會在下次存取「首頁」區域時被記住。

1. 按一下Adobe Workfront右上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon.png)，或（如果有的話）按一下左上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon-left-nav.png)，然後按一下&#x200B;**[!UICONTROL 首頁]**。
1. 按一下您要展開或收合的任何群組旁的&#x200B;**[!UICONTROL 展開]**&#x200B;或&#x200B;**[!UICONTROL 收合]**&#x200B;箭頭。

   ![](assets/expand-section-icon-highlighted-home-new-filters-and-sorting-nwe-350x268.png)

   或\
   若要同時展開或收合所有群組，請按住[!UICONTROL Shift]鍵，同時按一下任何群組旁的&#x200B;**[!UICONTROL 展開]**&#x200B;或&#x200B;**[!UICONTROL 收合]**&#x200B;箭頭。
