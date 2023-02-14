---
navigation-topic: business-case-and-scorecards
title: 使用資源計畫器在業務案例中的預算資源
description: 作為資源計畫的一部分，您可以使用項目層資源計畫器來預算在構建業務案例時完成項目中的工作所需的任務職責。
author: Alina
feature: Work Management
exl-id: 51ebb940-111c-442f-a8a6-287a04d2db68
source-git-commit: 5433008d93e99d69f8116e222bfce02411b77825
workflow-type: tm+mt
source-wordcount: '1249'
ht-degree: 0%

---

# 使用資源計畫器在業務案例中的預算資源

<!--drafted for the Budgeted Hours story: 

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> -->

作為資源計畫的一部分，您可以使用項目層資源計畫器來預算在構建業務案例時完成項目中的工作所需的任務職責。

有關建立業務案例的詳細資訊，請參閱 [為項目建立業務案例](../../../manage-work/projects/define-a-business-case/create-business-case.md).

>[!TIP]
>
>您在項目層資源計畫器中輸入的資訊也顯示在系統層資源計畫器中。 相反，情況也是如此。 有關資源計畫員的資訊，請參閱 [資源計畫員概覽](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

您也可以使用Adobe Workfront方案計畫器來預算業務案例中的資源。 如需詳細資訊，請參閱 [使用方案計畫器在業務案例中的預算資源](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront計畫</a>*</td> 
   <td> <p>Pro或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront授權概觀</a>*</td> 
   <td> <p>審核或更高版本</p> <p>重要：您必須擁有計畫許可證才能修改資源預算資訊。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對以下項目的存取權： </p> 
    <ul> 
     <li> <p>專案</p> </li> 
     <li> <p>資源管理</p> </li> 
     <li> <p>財務資料</p> </li> 
    </ul> <p>有關訪問預算資源所需的資訊，另請參閱 <a href="../../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">獲得Adobe Workfront預算資源所需資源</a>.</p> <p>注意：如果您仍無權存取，請洽詢您的Adobe Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理專案的權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

開始之前，您必須執行下列操作：

* 符合Adobe Workfront中資源規劃的所有必要條件。 如需詳細資訊，請參閱 [資源計畫員概覽](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

* 將資源池與項目關聯。

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:(you must have tasks assigned to job roles and users on the project - this is optional because the users and their roles come from the pools))</p>
  -->

   >[!NOTE]
   您無法為分配給業務案例中的問題的資源進行預算。 您可以在系統層資源計畫器中預算這些資源。 有關資源計畫員的詳細資訊，請參閱 [資源計畫員概覽](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

* 雖然這不是先決條件，但我們也建議您為專案上的工作指定「計畫小時數」。 這有助於您了解任務可能需要完成的工作量，有助於在完成任務的預算中花費大量時間來決定資源。 有關將任務與計畫小時數關聯的資訊，請參閱 [編輯任務](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## 在業務案例中將資源池應用於項目和預算資源

>[!IMPORTANT]
您可以將資源預算為15年。 如果為持續時間超過15年的項目預算資源，則預算資訊可能不準確。

要在業務案例中為沒有資源池的項目應用資源池和預算項目資源，請執行以下操作：

1. 轉到要為其預算資源的項目。
1. 按一下 **業務案例** 中。
1. （條件性）如果貴公司沒有Workfront方案規劃程式的授權，請按一下 **編輯資源預算** 在 **資源預算** ，然後繼續步驟5。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode,QuicksilverOrClassic.Quicksilver">(NOTE: ensure it stays right - this is 5 instead of 6 because step 2 won't print for nwe)</p>
   -->

1. （可選和條件性）如果項目資訊是從方案計畫員的方案發佈的，請執行以下操作之一：

   * 在 **選擇要用於計算項目預算人工成本的小時數** 欄位，然後按一下 **選擇>編輯資源預算**.

      ![](assets/business-case-rp-selected-with-choose-button-350x120.png)

   * 如果為項目的預算資源選擇了方案計畫器，請按一下 **變更** > **編輯資源預算**.

      ![](assets/business-case-sp-selected-change-option-to-switch-to-rp-highlighted-350x88.png)
   這將使用項目的預算小時數來計算項目的預算人工成本。

   方案規劃器僅適用於新的Adobe Workfront體驗，需要額外的許可。 有關Workfront方案計畫器的資訊，請參閱 [方案計畫員概覽](../../../scenario-planner/scenario-planner-overview.md).

   >[!NOTE]
   建議您在開始處理項目時決定是使用資源計畫員還是方案計畫員。 在專案期間經常在兩者之間切換，可能會造成您為專案預算資源的方式不一致。

1. 在 **選擇資源池** 欄位，指定一或多個 **資源池**.

   只能指定已填充活動用戶的資源池。

   >[!TIP]
   如果項目已與資源池關聯，則預設情況下會顯示資源計畫器。 要向項目添加更多資源池，請編輯項目。 如需編輯專案的相關資訊，請參閱 [編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md).

1. 按一下 **套用**.

   系統將顯示選定項目的資源計畫器。

   預設情況下，與此項目關聯的前20個任務角色按字母順序列在「資源預算」部分中。 

   有關資源計畫員的詳細資訊，請參閱 [資源計畫員概覽](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

   ![BC_resource_budgeting_area.png](assets/bc-resource-budgeting-area-350x276.png)

1. （可選和條件性）展開工作角色，查看與其相關聯的使用者。

   >[!NOTE]
   只有在與其關聯的作業角色符合以下條件時，活動用戶才會顯示在其下：
   * 它們屬於項目的一個資源池。
   * 他們已分配預算小時數。
   * 它們與項目的任一工作角色相關聯。


    

1. 按一下 **今天** 回到今天的時間範圍。
1. （選用）按一下 **周**, **月** 或 **季度** 以顯示不同時段中的項目資訊。
1. （選用）按一下 **小時** 下拉式功能表，然後選取 **小時**,**FTE**，或 **成本** 更改資訊在資源計畫器中的顯示方式。 預設會顯示小時數。

1. （選用）按一下 **匯出** 將資源計畫器導出為Excel檔案。

   >[!NOTE]
   一次最多可匯出12個時段的資料。

1. （選用）按一下 **全螢幕** 圖示 ![full_screen_RP_in_BC.png](assets/full-screen-rp-in-bc.png) 以全螢幕模式顯示資源計畫器。

1. 更新 **BDG** （預算小時數）欄位，通過以下操作之一，為用戶、角色或項目指定小時、FTE或成本值：

   * 人工估計角色、用戶或項目的小時數、FTE或成本值。

      或

   * 按一下 **選項** 表徵圖，並選擇一個選項以自動為角色、用戶或項目預算小時數。
   有關資源計畫員的「項目視圖」中預算的詳細資訊，請參閱 [使用「項目」和「職責」視圖在資源計畫器中使用預算資源](../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

   >[!NOTE]
   您可以為資源在「資源預算」區域中顯示的任意時間範圍預算小時數、FTE或成本，而不受項目時間軸的影響。 例如，如果您想要指明資源可能在項目時間軸期間不可用（在該時間軸與計畫小時數關聯），但在其他時間可能可用，則可以通過為計畫小時數為零的時間範圍編製預算來執行此操作（如果計畫小時數可用）。

1. （可選）要了解是否可以將預算的小時數、FTE或成本移至其他時間範圍，請按一下 **選項** ，則 **調整預算日期**.

   有關調整預算日期的詳細資訊，請參閱 [在資源計畫器中調整預算日期](../../../resource-mgmt/resource-planning/adjust-budgeting-dates.md).

1. 按一下&#x200B;**儲存**。

   如果您有與任務職責關聯的「每小時成本」費率，則預算「資源預算」區域中的資源將計算 **預算人工成本** 的URL。 預算的人工成本顯示在「業務案例」的「資源預算」區域和「業務案例匯總」中。

   >[!TIP]
   成本以項目的幣種顯示在「業務案例」中。

   在「業務案例」中指定的預算資訊也顯示在「資源計畫器」中。

   <!--drafted for Budgeted Hours: 
   <span class="preview">When you copy a project, you have the option to also copy the Budgeted Hours to the new project. Only hours budgeted in the Resource Planner are copied. For more information, see [Copy a project](../manage-projects/copy-project.md)</span>
   -->
