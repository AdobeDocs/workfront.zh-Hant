---
product-area: enterprise-scenario-planner-product-area
keywords: 發佈，計畫，專案，案例，案例
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 透過在情境規劃工具中發佈行動方案來更新或建立專案
description: 您可以透過在Adobe Workfront情境規劃工具中發佈情境，從現有方案建立專案，以及更新先前連結至方案的專案。
author: Alina
feature: Workfront Scenario Planner
exl-id: 46d3666a-4454-4a84-8c02-a79f3947a18f
source-git-commit: 9babe17ad862925440e555f881bf753fb443b67d
workflow-type: tm+mt
source-wordcount: '1722'
ht-degree: 0%

---

# 透過發佈中的方案更新或建立專案 [!DNL Scenario Planner]

從發佈情境 [!DNL Adobe Workfront Scenario Planner] 完成下列作業：

* 從情境上的方案建立專案，並將它們連結在一起。
* 使用已連結方案中的資訊，更新已連結至情境上方案的專案。 當您將專案匯入計畫時，專案也可以連結到方案。 如需詳細資訊，請參閱 [將專案匯入至中的計畫 [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md)

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 計畫*</p> </td> 
   <td>[！UICONTROL Business]或更高版本</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 授權*</p> </td> 
   <td> <p>[！UICONTROL Review]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td>產品 </td> 
   <td> <p>您必須為以下專案購買額外的授權： [!DNL Adobe Workfront Scenario Planner] 以存取本文所述的功能。</p> <p>如需有關取得 [!DNL Workfront Scenario Planner]，請參閱 <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">使用所需的存取權 [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p></p> <p>存取層級*</p> </td> 
   <td> 
    <ul> 
    <li>[！UICONTROL Edit]存取對象 [!DNL Scenario Planner] 和專案</li></ul>

<p><b>附註</b>

如果您還是沒有存取權，請詢問您的 [!DNL Workfront] 管理員是否對您的存取層級設定其他限制。 如需瞭解如何 [!DNL Workfront] 管理員可以變更您的存取層級，請參閱 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr data-mc-conditions=""> 
   <td> <p>物件許可權</p> </td> 
   <td> 
    <ul> 
     <li>計畫的[！UICONTROL Manage]許可權 </li> 
     <li>已發佈專案的[！UICONTROL Manage]許可權</li> 
    </ul> <p>如需請求專案其他存取許可權的詳細資訊，請參閱 <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> <p>如需請求對計畫的額外存取許可權的相關資訊，請參閱 <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">請求對中的計畫的存取權 [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需關於存取的其他資訊，請參閱 [!DNL Workfront Scenario Planner]，請參閱 [使用所需的存取權 [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

## 先決條件

開始之前：

* 您必須先建立和儲存計畫，才能從中發佈方案。
* 必須在「設定」的「專案偏好設定」區域中啟用「允許使用者建立專案，而不使用範本設定」 。 如需詳細資訊，請參閱 [設定全系統專案偏好設定](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## 將方案發佈至專案的相關考量事項

* 您只能從計畫發佈一個情境。
* 一個行動方案只能連結至一個專案。
* 當行動方案屬於不同計畫時，一個專案可連結至多個行動方案。

  >[!TIP]
  >
  >當一個專案存在於多個計畫上，而您從所有計畫發佈資訊至專案時，最新的發佈會覆寫現有的 [!DNL Scenario Planner] 有關專案的資訊。

* 如果透過將專案匯入計畫而在計畫上建立了方案，則發佈方案也會以方案資訊更新連結的專案。

  >[!TIP]
  >
  >您可以將相同專案匯入多個計畫。 發佈可能會覆寫連結至多個方案的專案上的方案資訊。

  如需透過匯入專案來建立方案的相關資訊，請參閱 [將專案匯入至中的計畫 [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* 對專案所做的任何變更都不會轉移到連結的方案。



## 發佈行動方案

>[!IMPORTANT]
>
>如果您對計畫上的方案進行任何變更，包括解決衝突，則必須重新發佈方案，才能在專案上顯示新資訊。 只有當您發佈對應的方案時，此資訊才會顯示在連結至方案的專案上。 如需解決方案之間衝突的詳細資訊，請參閱 [解決中的方案衝突 [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md)

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![](assets/main-menu-icon.png) (位於Workfront的右上角)，然後按一下 **[!UICONTROL 情境]**
1. （選擇性和條件性）如果要從現有計畫發佈，請按一下 **[!UICONTROL 篩選]** 圖示 ![](assets/filter-nwepng.png) 在計畫的右上角，並選取下列其中一個選項：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL All]</td> 
      <td>顯示您所擁有或與您共用的所有計畫。 這是預設值。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL我的計畫]</td> 
      <td>顯示您建立的計畫。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL已共用給我]</td> 
      <td> <p>顯示您未建立但與您共用的計畫。</p> <p>重要：您必須擁有與您共用之計畫的[！UICONTROL管理]許可權，才能發佈計畫。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/plans-filters-dropdown-options-scenario-planer.png)

1. （可選）按一下 **[!UICONTROL 搜尋]** 圖示 ![](assets/search-icon.png) 並開始輸入計畫的名稱，以便在清單中快速找到它。
1. （視條件而定）若要從新計畫發佈，請建立計畫。

   如需有關建立計畫的資訊，請參閱 [在中建立和編輯計畫 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md) .

1. （選擇性）按一下現有計畫的名稱，並為計畫建立新案例。

   如需有關建立計畫案例的資訊，請參閱 [在中建立和比較計畫案例 [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).

1. （選用）更新現有計畫或新計畫的方案，或建立新計畫。

   如需關於建立方案的資訊，請參閱 [在中建立和編輯方案 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

1. 按一下 **[!UICONTROL 儲存計畫]**.
1. 從中選擇您要發佈的情境 **[!UICONTROL 初始案例]** 下拉式功能表，然後按一下 **[!UICONTROL 前往發佈]** ![](assets/go-to-publish-button-icon.png) 位於右上角。

   或

   按一下 **[!UICONTROL 比較案例]**，將游標停留在您要發佈的情境卡片上，然後按一下 **[!UICONTROL 前往發佈]** ![](assets/go-to-publish-button-icon.png).

   此 [!UICONTROL 發佈方案] 頁面隨即顯示，並顯示情境中所有方案的清單。 如果先前已發佈任何方案，專案圖示 ![](assets/project-icon-sp.png) 會顯示在它們的名稱和 **[!UICONTROL 上次發佈日期]** 日期會填入清單中。

   >[!TIP]
   >
   >透過匯入專案建立的方案也會顯示專案圖示 ![](assets/project-icon-sp.png) 名稱右側

   ![](assets/project-icons-and-last-published-date-in-publish-initiative-page-350x63.png)

1. （選擇性和條件性）如果要從現有計畫發佈，請按一下 **[!UICONTROL 篩選]** 圖示 ![](assets/filter-nwepng.png) 在計畫的右上角，並選取下列其中一個選項：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL All]</td> 
      <td>顯示所選情境的所有方案。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL已發佈]</td> 
      <td>顯示您或其他使用者先前發佈的方案。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL已取消發佈]</td> 
      <td> <p>顯示未發佈的方案。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/initiatives-fitler-in-publishing-screen-scenario-planner.png)

1. （可選）按一下 **[!UICONTROL 搜尋]** 圖示 ![](assets/search-icon.png) 並開始輸入方案的名稱以在清單中快速找到。
1. 選取一或多個要發佈的方案，並從這些方案建立或更新專案，然後按一下 **[!UICONTROL 發佈方案]**.

   這會從每個選取的方案建立新專案，或是更新現有的連線專案（如果發佈的方案已連結至專案）。

   >[!TIP]
   >
   >新專案與已發佈方案的名稱相同。

1. （視條件而定）執行下列任一項作業：

   * 如果您發佈了一個方案，請按一下 **[!UICONTROL 檢視關聯的專案]** 以開啟從方案建立或更新的專案。
   * 如果您發佈多個方案，請按一下 **[!UICONTROL 檢視關聯的專案]** 以開啟從方案發佈的專案清單。 [!DNL Workfront] 套用 [!DNL Scenario Planner] 依預設，專案會篩選至專案清單。 最近發佈的專案會顯示在清單頂端。

     ![](assets/scenario-planner-filter-after-publishing-initiatives-350x81.png)

1. 移至下列區域以檢視專案上的方案資訊：

   * **此 [!UICONTROL 更新] 區段**：會發佈更新以指出專案已建立或已透過方案更新。 更新包含建立或更新專案的方案名稱，以及包含該方案的計畫的連結名稱。 您可以按一下更新中的計畫名稱，以開啟中的計畫 [!DNL Scenario Planner].

     ![](assets/update-stream-confirmation-of-publish-on-project-350x65.png)

   * **此 [!UICONTROL 概觀] 的區域 [!UICONTROL 專案詳細資訊] 區段**：新的 [!DNL Scenario Planner] 區段會在此區域中建立，並包含來自連結方案的資訊。

     ![](assets/scenario-planner-on-project-details-350x135.png)

     下列方案資訊會發佈在 [!DNL Scenario Planner] 的區域 [!UICONTROL 專案詳細資訊] 區段：

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader"><span>[！UICONTROL方案期間]</span> </td> 
        <td><span>專案連結至方案時，對應方案的持續時間。 此欄位不可編輯。</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[！UICONTROL上次發佈日期]</span> </td> 
        <td><span>專案上次從對應方案發佈的日期。</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[！UICONTROL方案開始日期]</span> </td> 
        <td><span>當專案連結至方案時，方案開始月份的第一天。</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[！UICONTROL方案結束日期]</span> </td> 
        <td><span>方案結束月份的最後一天，即專案連結至方案時。 </span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>FTE和時數中的[！UICONTROL方案工作角色]</span> </td> 
        <td> <p>方案之相關職務角色及其時間配置的相關資訊。 其中包括：</p> 
         <ul> 
          <li>工作角色名稱</li> 
          <li>FTE數量</li> 
          <li> <p>所有FTE的小時數</p> <p>您可以使用時數或FTE來預估計畫或方案所需的工作角色數量。</p> <p>如需詳細資訊，請參閱 <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">在「情境規劃工具」中建立和編輯計畫</a>. </p> </li> 
         </ul> 
      <p><b>秘訣</b>

     如果方案中每個月的工作角色數量不同，此欄位會顯示方案所需的最大角色數量。 例如，如果您在1月需要1名顧問，在2月需要2名，則欄會顯示2FTE以及所有月份2個FTE的對應時數金額。</p> </td>
     </tr> 
      </tbody> 
     </table>

     >[!NOTE]
     >
     >所有使用者具有 [!UICONTROL 檢視] 對專案的存取權可看到 [!DNL Scenario Planner] 中的區段 [!UICONTROL 概觀] 區域。 您可以控制此區域是否顯示在 [!UICONTROL 詳細資料] 區段（使用版面配置範本）。 如果使用者沒有關聯的版面配置範本，預設會顯示此區域。
     >
     >   
     >   
     >   * 有關新增或移除中的區域的資訊 [!UICONTROL 詳細資料] 區段使用版面配置範本，請參閱 [自訂 [!UICONTROL 詳細資料] 使用版面配置範本檢視](../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).
     >   * 如需有關檢視資訊的詳細資訊，請參閱 [!UICONTROL 概觀] 的區域 [!UICONTROL 專案詳細資訊]，請參閱 [[!UICONTROL 管理] 專案中的資訊 [!UICONTROL 概觀] 區域](../manage-work/projects/manage-projects/understand-project-overview-area.md).
     >   
     >

   * **此 [!UICONTROL 角色分配] 面板於 [!UICONTROL 工作負載平衡器] 或專案的工作清單**：除了專案上的角色配置外，此區域中還會填入有關行動方案上的角色配置的資訊。

     如需詳細資訊，請參閱 [協調專案與方案之間資源配置的概要](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

     ![](assets/role-allocation-panel-350x174.png)

     對專案日期或資源所做的任何變更，都不會影響對應的方案或專案上包含方案資訊的任何區域。

   * **此 [!UICONTROL 資源預算] 的區域 [!UICONTROL 業務案例] 專案的**：管理專案資源的新選項，使用 [!DNL Scenario Planner] 資訊新增至 [!UICONTROL 資源預算] 的區域 [!UICONTROL 業務案例] 專案的。

     如需詳細資訊，請參閱 [預算中的資源 [!UICONTROL 業務案例] 使用 [!DNL Scenario Planner]](../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

     ![](assets/sp-in-business-case-selected-350x110.png)

1. （選擇性）檢閱下列資訊： [!DNL Scenario Planner] 發佈情境後：

   * 已發佈的情境會成為您從中發佈方案後的第一個情境。
   * 將情境發佈至少一次後，您就無法再從任何其他情境發佈。
   * 此 [!UICONTROL 前往發佈] 從案例發佈至少一個方案後，選項會從所有其他案例中移除。
   * 綠色指標會顯示在計畫中已發佈方案的專案圖示旁。

     ![](assets/indicator-for-published-initiative-icon-350x119.png)

   * 綠色「已發佈」指標會顯示在情境頂端和情境卡片，而情境卡片會填入「已發佈」欄位，指出情境中已發佈的行動方案數目。

     ![](assets/published-scenario-highlighted-350x632.png)

     >[!TIP]
     >
     >如果刪除從情境方案發佈的所有專案，則會移除已發佈情境的指示。 如需詳細資訊，請參閱 [刪除專案](../manage-work/projects/manage-projects/delete-projects.md).

1. （可選）更新方案資訊並重複上述程式以重新發佈方案並更新連結專案上的方案資訊。

   如需有關編輯方案的資訊，請參閱 [在中建立和編輯方案 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).


