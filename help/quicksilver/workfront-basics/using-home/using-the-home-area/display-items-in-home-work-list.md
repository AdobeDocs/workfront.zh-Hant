---
product-area: projects
navigation-topic: use-the-home-area
title: 在 [!UICONTROL 工作清單] 在首頁
description: 此 [!UICONTROL 工作清單] 在 [!UICONTROL 首頁] 區域顯示分配給您的所有工作項。 您可以控制要在 [!UICONTROL 工作] 清單，如下所述。
author: Lisa
feature: Get Started with Workfront, Work Management
exl-id: eac2e065-9e32-43c1-90ff-0f841b508c35
source-git-commit: c111ae72da39fc1637320d993906ae9451e17e99
workflow-type: tm+mt
source-wordcount: '1602'
ht-degree: 0%

---

# 在 [!UICONTROL 工作清單] 在首頁

此 [!UICONTROL 工作清單] 在 [!UICONTROL 首頁] 區域顯示分配給您的所有工作項。 您可以控制要在 [!UICONTROL 工作] 清單，如下所述。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權*</strong></td> 
   <td> <p>[!UICONTROL Review]僅用於批准</p> <p>對於所有其他對象， [!UICONTROL工作]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>訪問級別配置*</strong></td> 
   <td> <p>[!UICONTROL視圖]或更高版本對項目、任務、問題和文檔的訪問</p> <p>注意：如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件權限</strong></td> 
   <td> <p>將權限或更高版本貢獻給您需要處理的任務和問題</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 篩選 [!UICONTROL 工作清單]

您可以篩選 [!UICONTROL 工作清單] 以僅查看特定類型的項目。 例如，您可以篩選 [!UICONTROL 工作清單] 以僅顯示問題或請求。

>[!NOTE]
>
>篩選器選項會儲存在瀏覽器中。 如果您一致地在同一台電腦上使用相同的瀏覽器（且未清除網站資料），則選取的篩選器不會變更。 如果您切換瀏覽器或電腦，則篩選器會回復為預設選項，取消選取所有篩選器。

1. 按一下 **[!UICONTROL 主菜單]** ![](assets/main-menu-icon.png) 在右上角，按一下 **[!UICONTROL 首頁]**.
1. 按一下 **[!UICONTROL 篩選]** ![](assets/filter-nwepng.png) 下拉式功能表。
1. 從下列篩選選項中選取，以指定您要顯示的項目類型：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL全部]</strong></td> 
      <td>顯示並選取所有項目。 這包括任務、問題、批准、個人任務以及已完成的任務和問題。 </td>
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL工作]</strong></td> 
      <td> <p>僅顯示您當前正在處理的任務。 這些是指派給您的任務，您已按一下[!UICONTROL Work On It]按鈕。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL任務準備開始]</strong></td> 
      <td> 
       <div> 
        <p>僅顯示可供您啟動的任務。 以下兩個陳述必須為true:</p> 
        <ul> 
         <li> <p>這些任務及其父代沒有前任，也沒有任務限制，無法使其工作。</p> </li> 
         <li> <p>任務的[!UICONTROL計劃開始日期]是過去或將來最多兩週。</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL任務未就緒]</strong></td> 
      <td> 
       <div> 
        <p>僅顯示尚未準備好開始的任務。 以下任一陳述必須為true:</p> 
        <ul> 
         <li> <p>這些任務及其父代可能有前置任務或任務限制，這些限制會阻止他們工作。</p> </li> 
         <li> <p>這些任務的[!UICONTROL計劃開始日期]在未來超過兩週。</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL處理的問題]</strong></td> 
      <td> <p>只顯示您目前處理的問題。 您已按一下「[!UICONTROL Work On It]」按鈕，指派給您的問題。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！請求的UICONTROL問題]</strong></td> 
      <td>僅顯示您被指派但尚未按一下[!UICONTROL Work On It]按鈕的問題。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>個人</strong></td> 
      <td>僅顯示個人任務。 這些是您建立為[!UICONTROL要執行的任務]的任務，如一節中所述 <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#creating-a-personal-task">建立個人任務</a> 在文章中 <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md">從[!UICONTROL首頁]區域建立工作項</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL批准]</strong></td> 
      <td> 
       <div> 
        <p>僅顯示指派或委派給您的核准以及您已提交的核准。 批准包括對工作項（項目、任務和問題）的批准，以及對文檔、校樣、訪問請求和時間表的批准。 如需核准的詳細資訊，請參閱下列文章：</p> 
        <ul> 
         <li><a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">查看批准</a> </li> 
        </ul> 
        <ul> 
         <li> <p><a href="../../../review-and-approve-work/manage-approvals/manage-approvals.md" class="MCXref xref">工作核准</a> </p> </li> 
        </ul> 
        <p>注意：您提交的批准和您也是批准者之一的批准將計算兩次。</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL已完成]</strong></td> 
      <td> <p>僅顯示已完成的任務、問題和個人任務。 已完成的工作將顯示前兩週的工作，並根據完成的周將其分組到工作清單中。 未包含核准。</p> <p>除非您選擇此篩選器，否則已完成的工作將隱藏在[!UICONTROL工作清單]中。</p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

   >[!TIP]
   >
   >* 篩選選項基於對象（任務、問題、批准、個人任務）。
   >* 任務和問題會根據狀態進一步篩選，以便我們做好處理這些任務和問題的準備([!UICONTROL 工作], [!UICONTROL 準備開始], [!UICONTROL 未就緒] 對於任務和 [!UICONTROL 工作] 和 [!UICONTROL 已請求] )。 您可以選擇顯示特定狀態的任務或問題，或按一下任務或問題以選擇和顯示所有狀態。
   >* 已完成項目有個別的篩選器，其中包含工作和問題。 這不包括核准。 此 [!UICONTROL 已完成] 篩選器包括個人任務。
   >* 一次只能選取一個狀態。 例如，您只能顯示 [!UICONTROL 工作] 任務和僅 [!UICONTROL 已請求] 問題。
   >* 您無法對指派給其中一個團隊的項目套用篩選，而且這些項目不會納入直接指派給您的項目中。



1. （選用）進一步組織 [!UICONTROL 工作清單]，如一節所述 [依日期、專案和優先順序分組和排序](#group-and-sort-by-date-project-and-priority) 這篇文章。

## 分組並排序依據 [!UICONTROL 日期], [!UICONTROL 專案]，和 [!UICONTROL 優先順序]

您可以分組並排序 [!UICONTROL 工作清單] by [!UICONTROL 計畫完成日期], [!UICONTROL 提交日期], [!UICONTROL 專案]，或 [!UICONTROL 我的優先順序]. 您選擇的選項決定項目在 [!UICONTROL 工作清單].

1. 按一下 **[!UICONTROL 主菜單]** ![](assets/main-menu-icon.png) 在右上角，按一下 **[!UICONTROL 首頁]**.
1. 按一下 **[!UICONTROL 分組依據]** 下拉式功能表。

   ![](assets/group-by-drop-down-expanded-in-home-with-planned-start-date-nwe-350x273.png)

1. 從下列選項中選取：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL計畫完成]</strong></td> 
      <td> <p> 根據項目的[!UICONTROL計畫完成日期]，項目在[!UICONTROL工作清單]中以下分組顯示（每個分組中包含的項目數以標題標題旁邊的括弧顯示）:</p> 
       <ul> 
        <li> <p>[!UICONTROL延遲]</p> </li> 
        <li> <p>[!UICONTROL無計畫完成日期]</p> </li> 
        <li> <p>[！本週]</p> <p>預設會展開此群組。</p> </li> 
        <li> <p>[!UICONTROL下週]</p> </li> 
        <li> <p>[!UICONTROL計畫完成日期]，後跟各種[!UICONTROL計畫完成日期]（多組）</p> </li> 
        <li> <p>[!UICONTROL完成]</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL計劃開始]</strong></td> 
      <td> <p>項目會根據其[!UICONTROL計劃開始日期]，在[!UICONTROL工作清單]中以下分組顯示（每個分組中包含的項目數以標題標題旁邊的括弧顯示）:</p> 
       <ul> 
        <li> <p>[!UICONTROL延遲]</p> </li> 
        <li> <p>[！本週] </p> <p>預設會展開此群組。</p> </li> 
        <li> <p>[!UICONTROL下週]</p> </li> 
        <li> <p>[!UICONTROL計畫]，後面接著各種[!UICONTROL計劃開始日期]（多個分組）</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL提交日期]</strong></td> 
      <td> <p>項目在[!UICONTROL工作清單]中按以下分組顯示（每個分組中包含的項目數以標題標題旁邊的括弧顯示）:</p> 
       <ul> 
        <li> <p>[!UICONTROL無提交日期]</p> </li> 
        <li> <p>[!UICONTROL下週提交]</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL項目]</strong></td> 
      <td>項目會根據項目分組，並且項目在[!UICONTROL工作清單]中按字母順序顯示。 （每個分組中包含的項目數會顯示在標題旁的括弧中。）</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL我的優先順序]</strong></td> 
      <td>項目會依您選擇的順序顯示。 如需詳細資訊，請參閱 <a href="../../../workfront-basics/using-home/using-the-home-area/prioritize-work-in-home.md" class="MCXref xref">在[!UICONTROL首頁]區域中排定工作優先順序</a>.</td> 
     </tr> 
    </tbody> 
   </table>

>[!NOTE]
>
>預設排序為遞增排序。 如果您將排序變更為降序，則選取的排序選項會儲存在瀏覽器中。 如果您在同一台電腦上一致使用相同的瀏覽器（且未清除網站資料），則排序不會變更，但如果您切換瀏覽器或電腦，排序會變更為預設排序。

## 查看延遲項

[!DNL Adobe Workfront] 使用以下日期來確定工作請求是否延遲：

* **工作**: [!UICONTROL 計畫完成日期]
* **問題**: [!UICONTROL 計畫完成日期]
* **檔案**: [!UICONTROL 提交日期]
* **工時單**: [!UICONTROL 提交日期]
* **核准**: [!UICONTROL 提交日期]
* **校樣核准**: [!UICONTROL 校樣截止日期]

## 搜尋 [!UICONTROL 工作清單]

搜尋 [!UICONTROL 工作清單]，則會在搜尋中傳回指派給您的任何項目（甚至畫面上目前未載入的項目）。 若 [!UICONTROL 顯示完成] 選項，則也會傳回您在過去兩週內標示為完成的任何項目。

此外，僅搜索工作項的名稱（不搜索工作項內的資訊，也不搜索工作項所在項目的名稱）。

若要搜尋 [!UICONTROL 工作清單]:

1. 按一下 **[!UICONTROL 主菜單]** ![](assets/main-menu-icon.png) 在右上角，按一下 **[!UICONTROL 首頁]**.
1. （選用）篩選 [!UICONTROL 工作清單]，如 [篩選 [!UICONTROL 工作清單]](#filter-the-work-list) 和 [依日期、專案和優先順序分組和排序](#group-and-sort-by-date-project-and-priority).

1. （可選）如果要搜索已完成的工作項，必須配置 [!UICONTROL 工作清單] 顯示搜索前已完成的項。
1. ![](assets/search-icon-highlighted-home-new-filters-and-sorting-nwe-350x238.png)

1. 開始鍵入您正在搜索的項目名稱的名稱。\
   此 [!UICONTROL 工作清單] 會自動篩選為包含具有相符名稱的項目。

## 更改工作清單的大小

您可以變更 [!UICONTROL 工作清單] 這樣，它就會佔用大約四分之一的家庭區域到大約一半的家庭區域 [!UICONTROL 首頁] 的上界。

1. 按一下 **[!UICONTROL 主菜單]** ![](assets/main-menu-icon.png) 在右上角，按一下 **[!UICONTROL 首頁]**.
1. 將滑鼠移至 [!UICONTROL 工作清單]，然後向左或向右拖曳，直到「工作清單」達到所需大小為止。

## 折疊和展開群組

中的項目 [!UICONTROL 工作清單] 會以群組顯示。 您可以折疊和展開群組，以控制指定時間頁面上顯示的資訊量。

您可以在 [!UICONTROL 工作清單] 以更好地控制可見的資訊。\
依預設， [!UICONTROL 本週] 分組會展開，而所有其他分組則會收合。 下次訪問「首頁」區域時，系統將記住您所做的任何更改。

1. 按一下 **[!UICONTROL 主菜單]** ![](assets/main-menu-icon.png) 在右上角，按一下 **[!UICONTROL 首頁]**.
1. 按一下 **[!UICONTROL 展開]** 或 **[!UICONTROL 折疊]** 要展開或折疊的任何分組旁邊的箭頭。

   ![](assets/expand-section-icon-highlighted-home-new-filters-and-sorting-nwe-350x268.png)

   或\
   若要同時展開或折疊所有群組，請按一下 **[!UICONTROL 展開]** 或 **[!UICONTROL 折疊]** 按住鍵時，在任何分組旁邊的箭頭 [!UICONTROL Shift] 鍵。
