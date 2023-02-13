---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 將項目導入方案計畫器中的計畫
description: 您可以將現有專案匯入計畫中。 導入的項目將轉換為方案，您可以在計畫中管理它們，就像管理新方案一樣。 原項目仍與新倡議有聯繫。
author: Alina
feature: Workfront Scenario Planner
exl-id: 20429bb1-c158-433b-9790-325cd577248e
source-git-commit: 844dddec944b6cfb0957eecf09c2980e9d0577cc
workflow-type: tm+mt
source-wordcount: '1699'
ht-degree: 0%

---

# 將專案匯入至 [!DNL Scenario Planner]

您可以將現有專案匯入計畫中。 導入的項目將轉換為方案，您可以在計畫中管理它們，就像管理新方案一樣。 原項目仍與新倡議有聯繫。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: add information about what happens when you import projects and where the info from projects show up;</p>
<p>- the hours/ FTE come from WorkPerDay</p>
<p>- if a task has a Duration of 0, the FTE should be 0 for that asignee but it should still come across) </p>
</div>
-->

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> 計劃*</b> </p> </td> 
   <td>[!UICONTROL Business]或更高版本</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> 授權*</b> </p> </td> 
   <td> <p>[!UICONTROL Review]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td><b>產品</b> </td> 
   <td> <p>您必須為 [!DNL Adobe Workfront Scenario Planner] 存取本文所述功能。</p> <p>如需有關取得 [!DNL Workfront Scenario Planner]，請參閱 <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">使用 [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>訪問級別配置*</strong> </td> 
   <td> <p>[!UICONTROL Edit]或更高版本 [!DNL Scenario Planner]</p> <p>注意：如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可以更改您的訪問級別，請參閱 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>物件權限</strong> </p> </td> 
   <td> <p>計畫的[!UICONTROL管理]權限</p> <p>有關請求對計畫進行額外訪問的資訊，請參閱 <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">請求方案計畫員中計畫的訪問權</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 關於將項目作為新計畫導入計畫的考慮

* 您必須先建立項目，才能將它們作為新方案導入計畫中。

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: no caveats for project statuses yet, mentioned in the import steps as a tip) </p>
  -->

* 你至少 [!UICONTROL 檢視] 項目的權限，以便將項目作為新計畫導入計畫。
* 您可以將相同的專案匯入多個計畫。
* 您要匯入的專案必須在計畫的時間範圍中包含日期。 您無法匯入具有 [!UICONTROL 計畫完成日期] 早於計劃開始或 [!UICONTROL 計劃開始日期] 遲於計畫結束。
* 一次無法匯入超過100個專案。
* 有些項目資訊也被導入計畫中，成為主動資訊。 有關將哪些項目資訊導入計畫並成為計畫資訊的資訊，請參見 [導入計畫的項目資訊](#project-information-imported-into-the-plan) 一節。
* 在連結項目上發生的更改不會影響計畫上的舉措。
* 計畫上的方案發生的更改不會自動影響連結的項目方案更改只有當您從計畫發佈方案時才會影響連結的項目。 如需發佈活動如何影響連結專案的相關資訊，請參閱 [更新或建立專案，方法是在 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).
* 刪除已通過導入項目建立的方案不會刪除項目。
* 刪除連結到方案的項目不會刪除方案。

## 導入計畫的項目資訊 {#project-information-imported-into-the-plan}

將項目導入計畫時，也會將一些項目資訊導入計畫，並將其變為計畫資訊。 下表顯示了將項目導入計畫時，哪些項目資訊成為計畫資訊：

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: add what happens if you import a 5 year project to a 1 year plan - how does this display?) </p>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>專案資訊</td> 
   <td>計畫資訊 </td> 
  </tr> 
  <tr> 
   <td>專案名稱</td> 
   <td>方案名稱</td> 
  </tr> 
  <tr> 
   <td>專案計畫日期</td> 
   <td> <p>計畫的開始和結束月份。</p> <p>如果項目在月中間開始或結束，則導入的日期將延長，以覆蓋計畫中的整個月。 例如，如果項目計畫日期為2020年3月20日至5月5日，則導入計畫的日期為2020年3月至5月。</p> <p>如果計畫起始日期或完成日期超出計畫的持續時間，則會顯示一個可視指示，即導入的計畫在計畫之前或之後開始或結束。 </p> </td> 
  </tr> 
  <tr> 
   <td>指派給任務和問題的作業角色</td> 
   <td> <p>計畫工作角色. </p> <p>備註:   <p>如果用戶在項目的生命期內更改了角色，則導入的角色取決於導入項目時分配的狀態。 存在下列情況：</p> 
     <ul> 
      <li> <p>如果分配給任務的用戶或問題在將其分配標籤為[!UICONTROL Done]後更改了其角色， [!DNL Workfront] 將用戶在將分配標籤為[!UICONTROL Done]之前履行的角色導入計畫。</p> </li> 
      <li> <p>如果分配給某個任務或問題的用戶在項目的生命週期中更改了角色，但在導入項目時，其在任務或問題上的分配未標籤為[!UICONTROL Done], [!DNL Workfront] 僅匯入所指派使用者的目前角色。 </p> </li> 
     </ul> <p>有關分配狀態的資訊，請參閱 <a href="../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md" class="MCXref xref">Adobe [!DNL Workfront] 術語</a>. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>與分配給任務或問題的作業角色關聯的項目[!UICONTROL計畫時數]</td> 
   <td> <p><span>根據計畫設定為使用FTE還是小時，項目上任務的[!UICONTROL計畫小時數]將變為</span> [!UICONTROL必需FTE] <span>或計畫上的[!UICONTROL所需小時數]</span>. </p> <p>有關設定計畫以使用FTE或小時的資訊，請參閱 <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">在 [!DNL Scenario Planner]</a>. </p> <p>請考量下列事項：</p> 
    <ul> 
     <li> <p>[!DNL Workfront] 使用分配給任務和問題的作業角色或分配給任務或問題的用戶在項目上關聯的作業角色，並將它們作為必需的作業角色轉移到新方案。 </p> </li> 
     <li> <p>當計畫設定為使用FTE時，與項目任務和問題上的任務職責相關聯的計畫小時數將首先轉換為FTE。 然後，此FTE將分配給計畫的工作角色。 <span>計畫小時數在 [!DNL Workfront]. 如果任務或問題跨越多個月，則計畫期間內每個月的計畫小時數量將以每月FTE轉換，並轉移到計畫的每個月。</span></p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例： </b></span></span><span>例如，如果在9月將任務分配給80個計畫小時的職務職責，則導入的職務職責在9月為方案顯示0.5 FTE。</span> </p> </li> 
     <li> <p>[!DNL Workfront] 使用以下公式計算與方案關聯的必需職務職責的FTE:</p> <p><code>Required Job Role FTE (initiative) = Job Role assignment Planned Hours (</code><code>from tasks and issues on the project)/ 160</code> </p> <p>提示：此 [!DNL Scenario Planner] 假設一個月內有160個工作小時。</p> <p>例如，如果項目的持續時間為1200分鐘，並且項目上的職務職責與600分鐘的計畫小時相關聯，則其FTE為0.5。導入項目時，新建立的方案的必需職務職責FTE為方案的每月0.5。 </p> </li> 
     <li>當將任務職責分配給項目中計畫時數為零的任務時，預設情況下，方案的任務職責的必需FTE為零。 <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         (NOTE: this used to be 1, not zero in Production) 
       </MadCap:conditionalText>
      --></li> 
     <li>將任務角色分配給項目上的任務時，其持續時間為零[!UICONTROL Duration]，則為必需FTE <span>或小時</span> 對於方案的工作角色，預設情況下為零，即使任務具有計畫小時數。 </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>



## 將項目導入計畫

>[!IMPORTANT]
>
>將項目導入計畫後，這些項目就成為計畫的倡議。 雖然這兩個項目是連結的，但它們作為獨立實體存在，並且在更新時不會自動影響彼此。
>
>發生以下情況：
>
>* 在將項目導入計畫後，對項目的更改不會影響計畫。這些更改包括對職務職責分配的更改。
>
>  <!--
>  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this might change if projects will ever affect initiatives automatically) </p>>
>  -->
>
>* 計畫的更改會影響 [!DNL Scenario Planner] 區域時，才會將方案發佈到相應的項目。 否則，它們不會影響 [!UICONTROL 計畫小時數] 項目任務和問題的資訊。
>
>  如需發佈活動如何影響連結專案的詳細資訊，請參閱  [通過在方案計畫器中發佈方案來更新或建立項目](../scenario-planner/publish-scenarios-update-projects.md).

1. 按一下 **[!UICONTROL 主菜單]** ![](assets/main-menu-icon.png) 在 [!DNL Workfront]，然後按一下 [!DNL Scenarios] 若要存取 [!DNL Scenario Planner].

1. 按一下要導入項目的計畫的名稱。
1. 按一下 **[!UICONTROL 新計畫]**，然後按一下 **[!UICONTROL 匯入專案]**.

   此 [!UICONTROL 匯入專案] 框。 計畫時間範圍內包含日期的專案會顯示在清單中。

   ![](assets/project-import-ui-projects-selected-350x72.png)

   >[!TIP]
   >
   >任何狀態的專案都會顯示在清單中。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the status of the projects in the import projects UI might change; right now it's ALL statuses)</p>
   -->

1. （選用）按一下 **[!UICONTROL 篩選圖示]** ![](assets/filter-nwepng.png)並從清單中選取可用的篩選器，以減少清單中的專案數量。 依預設，專案清單會依使用者目前在專案清單中選取的專案篩選條件來篩選。

1. （選用）按一下 **[!UICONTROL 搜尋圖示]** ![](assets/search-icon.png) 和新增顯示在畫面上任何欄位上的關鍵字。 包含搜尋字的項目會自動顯示在清單中，且所有項目都會隱藏。

1. （條件性）按一下 **[!UICONTROL X圖示]** 移除搜尋並顯示所有專案。
1. 選取最多100個專案，然後按一下 **[!UICONTROL 匯入]**.

   這些項目作為新舉措導入。

   請注意下列事項：

   * 專案圖示 ![](assets/project-icon-sp.png) 顯示在方案名稱的右側。
   * 如果項目時間表超過計畫的持續時間，則計畫欄的結尾會向左（當起始日期早於計畫日期時）或向右（當終止日期晚於計畫日期時）指定的邊距。

      ![](assets/project-bar-earlier-than-the-plan-start-date-350x39.png)

   * 已更新月數和工作角色，以符合專案的月數和工作角色。
   >[!TIP]
   >
   >與任務職責相關的成本在方案層更新，不會從項目導入。

1. 按一下代表新計畫的欄以開啟右側的計畫詳細資訊面板。

   ![](assets/initiative-duration-with-project-duration-details-panel-350x292.png)

   在 **[!UICONTROL 計畫持續時間]** 區域檢閱下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL計畫持續時間]</td> 
      <td>這是計畫的持續時間（以月為單位）。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL計畫]</td> 
      <td>計畫的開始和結束日期。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL項目]</td> 
      <td> <p>連結項目的[!UICONTROL計劃開始]和[!UICONTROL完成日期]。</p> <p>提示：如果缺少[!UICONTROL項目]資訊，則刪除了項目。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 編輯方案的名稱。 依預設，它會符合專案的名稱。
1. （選用）執行下列其中一項作業：

   * 更新作業角色(在 **[!UICONTROL 必需的作業角色]** 節
   * 更新 **[!UICONTROL 固定成本]** 在 **[!UICONTROL 成本]** 節

   * 按一下 **[!UICONTROL 更新可用作業角色]** 或 **[!UICONTROL 更新可用預算]** 解決新倡議與該計畫的其他倡議之間的衝突。

1. （有條件）按一下 **[!UICONTROL 套用]** 以保存對計畫的更改。
1. 按一下 **[!UICONTROL 保存計畫]** 以儲存對您計畫的變更。
1. （可選）要將您對方案所做的更改更新回從導入的項目，請從計畫發佈項目。 如需發佈計畫的相關資訊，請參閱 [更新或建立專案，方法是在 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).
1. （選用）按一下專案圖示以存取連結的專案。

   ![](assets/project-icon-on-initiative-highlighted-350x49.png)
