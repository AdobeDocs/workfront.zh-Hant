---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 在Scenario Planner中建立和編輯方案
description: 使用Adobe Workfront Scenario Planner時，您可以在已建立或已與您共用的計畫中建立方案。 透過建立方案，您可以顯示較小的組織單位對計畫的完成有何貢獻。 例如，如果貴組織有未來三年的計畫要擴展至新的市場，您可以在此計畫內為每個部門建立方案，以估計每個部門完成此計畫所需的人數和預算。
author: Alina
feature: Workfront Scenario Planner
exl-id: a811bad0-d3c0-4cba-8b78-d9a14ffc8482
source-git-commit: a79e4146ce6d076ef0e3707416a9c21d643b96e1
workflow-type: tm+mt
source-wordcount: '1625'
ht-degree: 0%

---

# 在[!DNL Scenario Planner]中建立和編輯方案

<!--Audited: 07/2024-->

使用[!UICONTROL Adobe Workfront Scenario Planner]時，您可以在已建立或已與您共用的計畫中建立方案。 透過建立方案，您可以顯示較小的組織單位對計畫的完成有何貢獻。 例如，如果貴組織有未來三年的計畫要擴展至新的市場，您可以在此計畫內為每個部門建立方案，以估計每個部門完成此計畫所需的人數和預算。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 計畫*</p> </td> 
   <td> <ul></li>
   <li><p>新增：Ultimate </p></li>
   <p>新的Workfront Select或Workfront計畫無法使用「情境規劃工具」。 </p>
   <li><p>目前： [！UICONTROL Business]或更高版本</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 授權*</p> </td> 
   <td> <p>新增：淺色或更高</p> 
   <p>目前： [！UICONTROL Review]或以上</p> </td> 
  </tr> 
  <tr> 
   <td>產品* </td> 
   <td> <ul><li><p>針對新的Workfront計畫：</p><p> Adobe Workfront</li></p>
   <li><p>針對目前的Workfront計畫： </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront情境規劃工具</p></li></ul>

<p>如需詳細資訊，請參閱<a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">使用[!DNL Scenario Planner]</a>所需的存取權。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>存取層級 </td> 
   <td> <p>[！UICONTROL Edit]對的存取權 [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>物件許可權 </p> </td> 
   <td> <p>[！UICONTROL Manage]計畫的許可權</p> <p>如需有關請求對計畫的額外存取權的資訊，請參閱<a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">在[!DNL Scenario Planner]</a>中請求對計畫的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱[Workfront檔案的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

您必須先建立計畫，或必須讓其他使用者與您共用計畫，才能在該計畫內建立方案。 如需有關建立計畫的資訊，請參閱[在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md)中建立和編輯計畫。

如需有關哪些方案的詳細資訊，請參閱 [!DNL Scenario Planner]](../scenario-planner/initiatives-overview.md)中的[方案概觀。

## 建立方案

您可以透過下列方式建立方案：

* 從頭開始。
* 將專案匯入計畫

  如需有關將專案匯入為計畫中的方案的資訊，請參閱[將專案匯入 [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md)中的計畫。

* 複製現有方案。

  如需複製方案的相關資訊，請參閱[複製 [!DNL Scenario Planner]](../scenario-planner/copy-initiatives.md)中的方案。

若要從頭開始建立方案：

{{step1-to-scenario-planner}}

1. 按一下要建立方案的計畫名稱。
1. 按一下&#x200B;**[!UICONTROL 新行動方案]**&#x200B;左側的&#x200B;**+圖示**

   或

   按一下&#x200B;**[!UICONTROL 新方案]**&#x200B;下拉式功能表，然後選取&#x200B;**[!UICONTROL 新方案]**&#x200B;或&#x200B;**[!UICONTROL 匯入專案]。**

1. 在&#x200B;**[!UICONTROL 未命名的方案]**&#x200B;欄位中輸入方案的名稱，然後按Enter鍵或按一下頁面上的其他位置。

   方案會以藍色列顯示在計畫的時間表上。 依預設，方案的持續期間為一個月，且一律從計畫的第一個月開始。

1. （可選）在左側面板和時間軸之間拖曳分隔列，以調整左側面板的大小。

1. （可選）拖曳方案列的結尾以將其持續時間延長至超過一個月，並在您希望方案結束月份的位置發行。
1. （選擇性和條件性）如果方案的持續時間比計畫的持續時間短，請將方案列拖放到計畫時間軸上的不同位置，以將其移動到另一個時間範圍。

   ![](assets/move-initiative-back-and-forth-on-the-timeline-350x71.png)

   >[!IMPORTANT]
   >
   >您只能選取以月為單位的持續時間。 您從頭開始建立的方案期間不能超過計畫的期間。

1. （選擇性）從&#x200B;**[!UICONTROL 月]**&#x200B;下拉式功能表中，選取下列其中一個選項以變更計畫的時間表：

   | 下拉式功能表選項 | 說明 |
   |---|---|
   | [!UICONTROL 個月] | 按月顯示時間表。 這是一年計畫的預設選項。 |
   | [!UICONTROL 季] | 依季度顯示時間軸。 只有在計畫的[!UICONTROL 期間]為3或5年時，才能使用此選項。 這是3年計畫的預設選項。 |
   | [!UICONTROL 年] | 按年顯示時間軸。 只有在計畫的[!UICONTROL 期間]為5年時，才能使用此選項。 這是5年計畫的預設選項。 |


1. （可選）從左向右捲動以檢視方案的整個期間。
1. （選擇性）按一下&#x200B;**[!UICONTROL Today]**&#x200B;指標行以回到目前日期。

   ![](assets/today-indicator-350x160.png)

   >[!TIP]
   >
   >如果您的計畫是未來或過去的計畫，且不包含目前日期，則不會顯示「今天」指標。

1. 按一下方案列。 方案詳細資訊面板會在右側開啟。

   ![](assets/initiative-details-panel-multiple-months-350x626.png)

   指定或檢閱下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">行動方案期間</td> 
      <td>行動方案的持續時間（月數）。 </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">開始和結束日期</td> 
      <td>方案的開始和結束日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">必要職務角色段落 </td> 
      <td> <p>按一下<strong>[！UICONTROL開始輸入工作角色]</strong>欄位，然後從清單中選取一個角色，或開始輸入<span>n個使用中</span>工作角色的名稱。 </p> <p><span>根據計畫是設定為使用FTE或時數，</span>在計畫</span>的每個月中，新增此方案在FTE <span><span>或時數</span></span><span>中所需的工作角色數量。 <span>預設會顯示方案的前三個月。</span></p> <p><span>更新方案的工作角色資訊也會更新計畫的必要工作角色資訊。</span> </p> <p>如需設定計畫以使用FTE或時數的詳細資訊，請參閱<a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">在[!DNL Scenario Planner]</a>中建立和編輯計畫。 </p>
      <p><b>重要</b></p>  
      <p>對於[!DNL Scenario Planner]中的所有計算，[!DNL Workfront]會使用以下值： 1 FTE = 8小時。 </p>

   <p><b>秘訣</b></p>

   <ul> 
       <li> <p><span>使用[！UICONTROL Tab]鍵移至下個月。</span> </p> </li> 
      <li> <p> 當您按一下此欄位時，系統會列出系統中所有的<span>使用中</span>工作角色。 </p> </li> 
       <li> <p>已新增至計畫之可用職務角色的工作角色會先顯示。 如需有關將可用職務角色新增至計畫的資訊，請參閱<a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">在Scenario Planner中建立及編輯計畫</a>。 </p> </li> 
       <li> <p>[!DNL Workfront] 認為全時相當於一個月160小時。 </p> <p>對於「情境規劃工具」中的所有計算，Workfront會使用以下值： 1 FTE = 8小時。 </p></li> 
      </ul> </p> <p>您可以為FTE <span>或</span> <span>小時</span>輸入小於1 FTE或小數點的數字。 例如，0.5的顧問工作角色表示顧問將投入一半FTE （通常是4小時，其中8小時是1 FTE）來處理此方案。 </p>  </td> 
     </tr> 
     <tr> 
      <td rowspan="3" role="rowheader">成本區段</td> 
      <td> <p>方案的總成本會顯示在[！UICONTROL Costs]區段的右側。 [!DNL Workfront]使用下列公式計算方案的成本：</p> <p><code>[!UICONTROL Initiative Costs] = [!UICONTROL Fixed Costs] + [!UICONTROL People] Costs</code> </p> </td> 
     </tr> 
     <tr> 
      <td> <p>在<strong>[！UICONTROL固定成本]</strong>欄位中，手動輸入您認為完成此方案所需成本的粗略預估金額。 這不應包括與方案估計的工作角色相關的成本。</p> <p><span>使用Tab鍵時，從一個月移至下個月，以輸入方案每個月的金額。</span> </p> </td> 
     </tr> 
     <tr> 
      <td> 
       <div> 
        <p>視計畫設定為使用FTE或時數而定，[！UICONTROL Workfront]會使用下列公式來計算[！UICONTROL人員成本]：</p> 
        <ul> 
         <li> <p>使用FTE時： </p> <p><code>[!UICONTROL People Costs] = SUM(Job role hourly rate * Number of months in the Duration * 160 * Number of FTEs)</code>，其中160是一個月內的工作時數總計。 </p> </li> 
         <li> <p style="font-weight: normal;">使用時數時： </p> <p style="font-weight: normal;"><code>Monthly People Costs = SUM(Job role hourly rate * Number of hours estimated for an initiative)</code> </p> <p style="font-weight: normal;">如需有關設定計畫以使用時數或FTE的資訊，請參閱<a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">在「情境規劃工具」中建立和編輯計畫</a>。</p> </li> 
        </ul> 
        <p>人員成本是以您在「匯率」偏好設定中選取的基本貨幣計算。 如需有關匯率的資訊，請參閱<a href="../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">設定匯率</a>。</p> 
        <p>更新方案的成本資訊也會更新計畫的[！UICONTROL成本]區域。 </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader"> <p style="font-weight: normal;">在您為方案定義所需的工作角色和成本值，並修改方案的持續時間後，可能會出現下列其中一種情況：</p> 
       <ul> 
        <li> <p style="font-weight: normal;">如果您縮短方案，[!DNL Workfront]會移除所需的資源量，以及與從計畫移除的時間相關的成本。 工作角色仍保留在計畫中，但他們沒有必要的FTE或<span data-mc-edit-date="2021-04-19T13:46:01.5004065-04:00" data-mc-editor="alinawilson" data-mc-comment="drafted, yellow" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2021-04-19T13:45:58.7938344-04:00">小時</span>。 計畫與預算的可用資源保持不變。<br>如需更新計畫的資訊，請參閱<a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">在[!DNL Scenario Planner]</a>中建立和編輯計畫。 </p> </li> 
        <li> <p style="font-weight: normal;">如果您讓方案的時間更長，您必須指定方案上新增加月份的工作角色和成本數量。 </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Net Value] 區段</td> 
      <td>在<strong>[!DNL Net Value]</strong>區段中，在<strong>[！UICONTROL計畫收益]</strong>欄位中手動輸入粗略預估金額。 這就是您認為達成此計畫將會帶來的好處。 </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >如果您已定義計畫的職務角色數目和預算，以及您正在編輯之方案及其上所有方案的職務角色數目和成本，而且這些數目和成本都超過您為計畫指定的金額，[!DNL Workfront]可能會發現您沒有足夠資源完成方案。 [!DNL Workfront]在嘗試達成此方案時將其標籤為衝突，並將其顯示為紅色長條。 衝突行動方案之後的所有行動方案都會以紅色背景顯示。 您可能需要從資源不足的第一個方案開始，調整方案的部分需求。 如需有關調整衝突方案的資訊，請參閱[解決 [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md)中的方案衝突。

1. （選用）將滑鼠指標暫留在工作角色的名稱上，然後按一下&#x200B;**[!UICONTROL 垃圾桶圖示]** ![](assets/delete.png)，將其從方案移除。

1. （視條件而定）如果您變更方案，請按一下&#x200B;**[!UICONTROL 套用]**。

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: Add more steps here as you can do more in the Initiative box over time)
   </MadCap:conditionalText>
   -->

1. （視條件而定）如果您未進行任何變更，請按一下方案詳細資料面板右上角的&#x200B;**X**&#x200B;圖示以將其關閉。
1. （選用）更新方案的優先順序。

   如需排定方案優先順序的資訊，請參閱情境規劃工具](../scenario-planner/prioritize-initiatives.md)中的[更新方案優先順序。

   >[!TIP]
   >
   >在清單中排在第一位的方案有較高的優先順序，且在清單中較低位置列出的方案之前取得資源。

1. 按一下&#x200B;**[!UICONTROL 儲存計畫]**。

   方案現在包含在您的計畫中。

   如需有關從計畫中刪除方案的資訊，請參閱[刪除 [!DNL Scenario Planner]](../scenario-planner/delete-initiatives.md)中的方案。
