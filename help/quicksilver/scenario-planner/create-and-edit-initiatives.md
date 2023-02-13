---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 在方案計畫器中建立和編輯方案
description: 使用Adobe Workfront方案計畫器時，您可以在您建立或與您共用的計畫中建立方案。 通過建立計畫，您可以顯示較小的組織單位對計畫完成的貢獻。 例如，如果貴組織有未來三年的計畫以擴展到新市場，則您可以在此計畫內為每個部門建立方案，以估計每個部門完成此計畫所需的人員和預算。
author: Alina
feature: Workfront Scenario Planner
exl-id: a811bad0-d3c0-4cba-8b78-d9a14ffc8482
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '1623'
ht-degree: 0%

---

# 在 [!DNL Scenario Planner]

使用 [!UICONTROL Adobe Workfront方案規劃器]，您可以在您建立或與您共用的計畫中建立方案。 通過建立計畫，您可以顯示較小的組織單位對計畫完成的貢獻。 例如，如果貴組織有未來三年的計畫以擴展到新市場，則您可以在此計畫內為每個部門建立方案，以估計每個部門完成此計畫所需的人員和預算。

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 計劃*</p> </td> 
   <td>[!UICONTROL Business]或更高版本</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 授權* </p> </td> 
   <td> <p>[!UICONTROL Review]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td>產品 </td> 
   <td> <p>您必須為 [!DNL Adobe Workfront Scenario Planner] 存取本文所述功能。 </p> <p>如需有關取得 [!DNL Workfront Scenario Planner]，請參閱 <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">使用 [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>訪問級別配置* </td> 
   <td> <p>[!UICONTROL Edit]或更高版本 [!DNL Scenario Planner]</p> <p>如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可以更改您的訪問級別，請參閱 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>物件權限 </p> </td> 
   <td> <p>計畫的[!UICONTROL管理]權限</p> <p>有關請求對計畫進行額外訪問的資訊，請參閱 <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">在 [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 必要條件

您必須建立計畫，或者其他用戶必須與您共用計畫，然後才能在該計畫內建立計畫。 如需建立計畫的相關資訊，請參閱 [在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

如需計畫的詳細資訊，請參閱 [計畫概覽 [!DNL Scenario Planner]](../scenario-planner/initiatives-overview.md).

## 建立方案

您可以以下列方式建立方案：

* 白手起家。
* 將項目導入計畫

   有關將項目作為計畫中的方案導入的資訊，請參見 [將專案匯入至 [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* 複製現有方案。

   有關複製方案的資訊，請參閱 [複製 [!DNL Scenario Planner]](../scenario-planner/copy-initiatives.md).

要從頭開始建立計畫：

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png)，然後按一下 [!UICONTROL 藍本].

1. 按一下要為其建立方案的計畫的名稱。
1. 按一下 **+圖示** 左側 **[!UICONTROL 新舉措]**

   或

   按一下 **[!UICONTROL 新舉措]** 下拉式功能表中選取 **[!UICONTROL 新舉措]** 或 **[!UICONTROL 匯入專案].**

1. 在 **[!UICONTROL 無標題計畫]** 欄位，然後按Enter或按一下頁面上的其他位置。

   方案以藍色條顯示在計畫的時間軸上。 預設情況下，計畫的持續時間為一個月，始於計畫的第一個月。

1. （可選）拖曳左面板與時間軸之間的分隔列，調整左面板的大小。

1. （可選）拖動計畫欄的末尾，將其持續時間延長到一個多月，然後將其釋放到您希望計畫的結束月。
1. （可選和條件性）如果方案的持續時間短於計畫的持續時間，請將方案欄拖放到計畫時間軸上的不同位置，以將其移動到另一個時間範圍。

   ![](assets/move-initiative-back-and-forth-on-the-timeline-350x71.png)

   >[!IMPORTANT]
   >
   >您只能選取以月為單位的持續時間。 您從頭建立的計畫的持續時間不能超過計畫的持續時間。

1. （選用）從 **[!UICONTROL 月]** 下拉菜單中，選擇以下選項之一以更改計畫的時間軸：

   | 下拉式功能表選項 | 說明 |
   |---|---|
   | [!UICONTROL 月] | 按月顯示時間軸。 這是一年期計畫的預設選項。 |
   | [!UICONTROL 季度] | 按季度顯示時間軸。 此選項僅在 [!UICONTROL 持續時間] 三五年。 這是3年計畫的預設選項。 |
   | [!UICONTROL 年] | 按年顯示時間軸。 此選項僅在 [!UICONTROL 持續時間] 計畫是五年。 這是5年計畫的預設選項。 |


1. （可選）從左向右滾動以查看計畫的整個持續時間。
1. （選用）按一下 **[!UICONTROL 今天]** 指示線，返回至目前日期。

   ![](assets/today-indicator-350x160.png)

   >[!TIP]
   >
   >如果您的計畫是在未來或過去，並且不包括目前日期，則不會顯示「今天」指標。

1. 按一下方案的欄。 計畫詳細資訊面板在右側開啟。

   ![](assets/initiative-details-panel-multiple-months-350x626.png)

   指定或檢閱下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">行動方案期間</td> 
      <td>計畫持續時間（以月為單位）。 </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">開始和結束日期</td> 
      <td>計畫的開始和結束日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">「必需作業角色」部分 </td> 
      <td> <p>按一下 <strong>[!UICONTROL開始鍵入作業角色]</strong> 欄位，然後從清單中選取角色，或開始輸入<span>活動</span> 工作角色。 </p> <p><span>根據計畫設定為使用FTE還是小時，</span> 在FTE中添加此計畫所需的職務角色數 <span><span>或小時</span></span><span> 計畫中每月</span>. <span>預設會顯示計畫的前三個月。</span></p> <p><span>更新計畫的作業角色資訊也更新計畫的「必需」作業角色資訊。</span> </p> <p>有關設定計畫以使用FTE或小時的資訊，請參閱 <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">在 [!DNL Scenario Planner]</a>. </p> <p>提示：  
        <ul> 
         <li> <p><span>使用[!UICONTROL Tab]鍵可移至下個月。</span> </p> </li> 
         <li> <p> 全部 <span>活動</span> 按一下此欄位時，系統中會列出作業角色。 </p> </li> 
         <li> <p>已添加到計畫的「可用」作業角色的作業角色將首先顯示。 有關將可用作業角色添加到計畫的資訊，請參閱 <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">在方案計畫員中建立和編輯計畫</a>. </p> </li> 
         <li> <p>[!DNL Workfront] 認為全職等同值是160小時，一個月。 </p> </li> 
        </ul> </p> <p>您可以輸入小於1 FTE的數字或小數的FTE <span>或</span> <span data-mc-edit-date="2021-04-22T16:51:21.5923499-04:00" data-mc-editor="alinawilson" data-mc-comment=" yellow" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2021-04-19T13:45:00.3159349-04:00">小時</span>. 例如，0.5顧問職位意味著顧問會將其一半的FTE（通常為4小時，其中8小時為1名FTE）用於執行此計畫。 </p> <p>對於方案計畫器中的所有計算，Workfront使用以下值：1 FTE = 8小時。 </p> </td> 
     </tr> 
     <tr> 
      <td rowspan="3" role="rowheader">費用科</td> 
      <td> <p>計畫的總成本顯示在[!UICONTROL成本]部分的右側。 [!DNL Workfront] 使用以下公式計算方案的成本：</p> <p><code>[!UICONTROL Initiative Costs] = [!UICONTROL Fixed Costs] + [!UICONTROL People] Costs</code> </p> </td> 
     </tr> 
     <tr> 
      <td> <p>在 <strong>[!UICONTROL固定成本]</strong> 欄位中，手動輸入您認為完成此計畫所需費用的粗估計金額。 這不應包括與為該舉措估計的工作角色相關的費用。</p> <p><span>使用Tab鍵時，通過從一個月移至下一個月，輸入方案的每個月的金額。</span> </p> </td> 
     </tr> 
     <tr> 
      <td> 
       <div> 
        <p>根據計畫設定為使用FTE還是小時，[!UICONTROL Workfront]使用以下公式來計算[!UICONTROL人員成本]:</p> 
        <ul> 
         <li> <p>使用FTE時： </p> <p><code>[!UICONTROL People Costs] = SUM(Job role hourly rate * Number of months in the Duration * 160 * Number of FTEs)</code>，其中160是一個月內的總工時數。 </p> </li> 
         <li> <p style="font-weight: normal;">使用小時數時： </p> <p style="font-weight: normal;"><code>Monthly People Costs = SUM(Job role hourly rate * Number of hours estimated for an initiative)</code> </p> <p style="font-weight: normal;">有關將計畫設定為使用小時或FTE的資訊，請參閱 <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">在方案計畫員中建立和編輯計畫</a>.</p> </li> 
        </ul> 
        <p>人員成本以在「匯率」首選項中選擇的基本貨幣計算。 有關匯率的資訊，請參見 <a href="../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">設定匯率</a>.</p> 
        <p>更新計畫的成本資訊也更新計畫的[!UICONTROL成本]區域。 </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader"> <p style="font-weight: normal;">在定義了計畫所需的任務職責和成本值並修改計畫的持續時間後，可能會發生以下情況之一：</p> 
       <ul> 
        <li> <p style="font-weight: normal;">如果你縮短計畫， [!DNL Workfront] 刪除與從計畫中刪除的時間相關的所需資源量和成本。 工作角色仍保留在計畫中，但沒有必要的FTE或 <span data-mc-edit-date="2021-04-19T13:46:01.5004065-04:00" data-mc-editor="alinawilson" data-mc-comment="drafted, yellow" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2021-04-19T13:45:58.7938344-04:00">小時</span>. 計畫和預算的可用資源保持不變。<br>有關計畫的更新資訊，請參閱 <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">在 [!DNL Scenario Planner]</a>. </p> </li> 
        <li> <p style="font-weight: normal;">如果您延長計畫的時間，則必須指定計畫上新添加的月份的職務和成本金額。 </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Net Value] 節</td> 
      <td>在 <strong>[!DNL Net Value]</strong> 部分，在 <strong>[!UICONTROL計畫福利]</strong> 欄位。 這就是你認為實現這一計畫的好處。 </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >如果您已經定義了計畫的職務職責數和預算、正在編輯的職務職責數和方案的成本，以及上面所有方案的成本，並且它們均超過了您為計畫指定的金額， [!DNL Workfront] 可能會發現您沒有足夠的資源來完成計畫。 [!DNL Workfront] 在嘗試實現此計畫時，會將此標籤為衝突，並將其顯示為紅色欄。 所有跟在矛盾計畫之後的計畫都以紅色背景顯示。 您可能需要調整計畫的某些需求，從資源不足的第一個開始。 有關調整衝突方案的資訊，請參見 [解決 [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md).

1. （選用）暫留在工作角色的名稱上，然後按一下 **[!UICONTROL 垃圾桶圖示]** ![](assets/delete.png) 從計畫中移除。

1. （條件性）如果您對方案進行了更改，請按一下 **[!UICONTROL 套用]**.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: Add more steps here as you can do more in the Initiative box over time)
   </MadCap:conditionalText>
   -->

1. （條件性）若您未進行任何變更，請按一下 **X** 表徵圖，以關閉它。
1. （可選）更新計畫的優先順序。

   有關排定計畫優先順序的資訊，請參見 [更新方案計畫器中的方案優先順序](../scenario-planner/prioritize-initiatives.md).

   >[!TIP]
   >
   >清單中第一的計畫優先順序較高，在清單中下方所列的計畫之前獲得資源。

1. 按一下 **[!UICONTROL 保存計畫]**.

   該計畫現已納入您的計畫。

   有關從計畫中刪除方案的資訊，請參閱 [刪除 [!DNL Scenario Planner]](../scenario-planner/delete-initiatives.md).
