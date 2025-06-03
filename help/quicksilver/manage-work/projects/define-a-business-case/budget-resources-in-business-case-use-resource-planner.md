---
navigation-topic: business-case-and-scorecards
title: 使用資源規劃工具在業務案例中預算資源
description: 作為資源計畫的一部份，當您建立業務案例時，可以使用專案層次的資源規劃工具來編列完成專案中工作所需的職務角色預算。
author: Alina
feature: Work Management
exl-id: 51ebb940-111c-442f-a8a6-287a04d2db68
source-git-commit: 9cfb67f627c06a5926e820860d52ba9f1ab58bcf
workflow-type: tm+mt
source-wordcount: '1240'
ht-degree: 0%

---

# 使用資源規劃工具在業務案例中預算資源

<!--Audited: 01/2025-->

作為資源計畫的一部份，當您建立業務案例時，可以使用專案層次的資源規劃工具來編列完成專案中工作所需的職務角色預算。

如需建立業務案例的詳細資訊，請參閱[為專案建立業務案例](../../../manage-work/projects/define-a-business-case/create-business-case.md)。

>[!TIP]
>
>您在專案層次「資源供需規劃員」中輸入的資訊，也會顯示在系統層次「資源供需規劃員」中。 反之亦然。 如需資源規劃工具的相關資訊，請參閱[資源規劃工具概觀](../../../resource-mgmt/resource-planning/get-started-resource-planner.md)。

您也可以使用Adobe Workfront案例規劃工具，為業務案例中的資源編列預算。 如需詳細資訊，請參閱使用案例規劃工具[&#128279;](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md)的業務案例中的預算資源。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>目前：Prime或更新版本</p>
   <p>舊版：Pro或更高版本</p> 
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>目前：淺色或更高</p>
   <p>舊版：檢閱或更高版本</p>

<p><b>重要：</b></p> 
   <p>新增：您必須擁有標準授權，才能修改資源預算資訊。 </p> 
   <p>目前：您必須擁有計畫授權，才能修改資源預算資訊。 </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯下列專案的存取權： </p> 
    <ul> 
     <li> <p>專案</p> </li> 
     <li> <p>資源管理</p> </li> 
     <li> <p>財務資料</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理專案的許可權</p> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

開始之前，您必須執行下列動作：

* 滿足Adobe Workfront中資源規劃的所有必要條件。 如需詳細資訊，請參閱[資源規劃工具概觀](../../../resource-mgmt/resource-planning/get-started-resource-planner.md)。

* 將資源集區與專案建立關聯。

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:(you must have tasks assigned to job roles and users on the project - this is optional because the users and their roles come from the pools))</p>
  -->

  >[!NOTE]
  >
  >您不能為指派給業務案例中問題的資源編列預算。 您可以在系統層級的資源規劃工具中編列預算。 如需資源規劃工具的詳細資訊，請參閱[資源規劃工具概觀](../../../resource-mgmt/resource-planning/get-started-resource-planner.md)。

* 雖然這不是先決條件，但我們也建議您為專案上的任務指定計畫時數。 這有助於您瞭解任務可能需要完成的工作量，有助於決定資源應編列預算用於完成任務的多少時間。 如需將任務與計畫時數建立關聯的資訊，請參閱[編輯任務](../../../manage-work/tasks/manage-tasks/edit-tasks.md)。

## 將資源集區套用至業務案例中的專案與預算資源

>[!IMPORTANT]
>
>您可以為資源編列為期15年的預算。 如果您為持續期間超過15年的專案編列資源預算，預算資訊可能不準確。

若要針對沒有資源集區的專案，在業務案例中套用資源集區和預算專案資源：

1. 移至您要編列資源預算的專案。
1. 按一下左側面板中的&#x200B;**業務案例**。
1. （視條件而定）如果貴公司沒有Workfront Scenario Planner的授權，請按一下&#x200B;**資源預算**&#x200B;區段中的&#x200B;**編輯資源預算**，然後繼續步驟5。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode,QuicksilverOrClassic.Quicksilver">(NOTE: ensure it stays right - this is 5 instead of 6 because step 2 won't print for nwe)</p>
   -->

1. （選擇性和條件性）如果專案資訊是從「情境規劃工具」上的方案發佈的，請執行下列任一項作業：

   * 在&#x200B;**中選取資源規劃工具選擇要用於計算專案預算勞力成本的時數**&#x200B;欄位，然後按一下&#x200B;**選擇>編輯資源預算**。

     ![資源規劃工具中的業務案例](assets/business-case-rp-selected-with-choose-button-350x120.png)

   * 如果已選取案例規劃工具來編列專案的資源，請按一下&#x200B;**變更** > **編輯資源預算**。

     ![情境規劃工具中的業務案例](assets/business-case-sp-selected-change-option-to-switch-to-rp-highlighted-350x88.png)

   這會使用專案的預算時數來計算專案的預算勞力成本。

   Scenario Planner僅在新的Adobe Workfront體驗中可用，並且需要額外的授權。 如需Workfront Scenario Planner的相關資訊，請參閱[Scenario Planner概觀](../../../scenario-planner/scenario-planner-overview.md)。

   >[!NOTE]
   >
   >建議您在開始處理專案時，決定使用資源規劃工具或情境規劃工具。 在專案生命週期中經常在這兩個之間切換，可能會造成您為專案編列資源預算的方式不一致。

1. 在&#x200B;**選取資源集區**&#x200B;欄位中，指定一或多個&#x200B;**資源集區**。

   您只能指定以作用中使用者填入的資源集區。

   >[!TIP]
   >
   >如果專案已與資源集區相關聯，則預設會顯示資源規劃工具。 若要將更多資源集區新增至專案，請編輯專案。 如需有關編輯專案的資訊，請參閱[編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md)。

1. 按一下&#x200B;**套用**。

   針對選取的專案顯示「資源規劃工具」。

   依預設，與此專案相關聯的前20個職務角色會依字母順序列在「資源預算」區段中。 

   如需資源規劃工具的詳細資訊，請參閱[資源規劃工具概觀](../../../resource-mgmt/resource-planning/get-started-resource-planner.md)。

   ![BC_resource_budgeting_area.png](assets/bc-resource-budgeting-area-350x276.png)

1. （選擇性和條件性）展開工作角色以檢視與工作角色相關聯的使用者。

   >[!NOTE]
   >
   >只有符合下列條件時，作用中的使用者才會顯示在與其相關聯的工作角色下：
   >
   >   
   >   
   >   * 它們屬於專案的其中一個資源集區。
   >   * 他們已指派預算時數。
   >   * 它們與專案的其中一個工作角色相關聯。
   >   
   >

    

1. 按一下&#x200B;**今天**&#x200B;以返回今天的時間範圍。
1. （選擇性）按一下&#x200B;**周**、**月**&#x200B;或&#x200B;**季**，以不同時間範圍顯示專案的資訊。
1. （選擇性）按一下&#x200B;**小時**&#x200B;下拉式功能表，然後選取&#x200B;**小時**、**FTE**&#x200B;或&#x200B;**成本**，以變更資訊在資源規劃工具中的顯示方式。 小時依預設顯示。

1. （選擇性）按一下&#x200B;**匯出**，將資源規劃工具匯出至Excel檔案。

   >[!NOTE]
   >
   >您一次最多可以匯出12個時間段的資料。

1. （選擇性）按一下&#x200B;**全熒幕**&#x200B;圖示![full_screen_RP_in_BC.png](assets/full-screen-rp-in-bc.png)以全熒幕模式顯示「資源規劃工具」。

1. 執行下列其中一項作業，以使用者、角色或專案的小時、FTE或成本值更新&#x200B;**BDG** （預算時數）欄位：

   * 手動估算角色、使用者或專案的「小時」、「約當全職人數」或「成本」值。

     或

   * 按一下專案或工作角色的&#x200B;**選項**&#x200B;圖示，然後選取選項以自動為角色、使用者或專案編列時數預算。

   如需有關資源規劃工具專案檢視中預算的詳細資訊，請參閱資源規劃工具中使用專案和角色檢視的[預算資源](../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md)。

   >[!NOTE]
   >
   >您可以針對「資源預算」區域中顯示的任何時間範圍預算資源的時數、FTE或成本，而不受專案時間表的影響。 例如，如果您想要指出您的資源在專案的時間表期間可能無法使用（這些資源與計畫時數相關聯），但它們可能在另一個時間可供使用，您可以透過為計畫時數為零的時間範圍編列預算來執行此操作，前提是這些資源可供使用。

1. （選擇性）若要瞭解您是否可以將預算時數、FTE或成本移動到另一個時間範圍，請按一下&#x200B;**選項**&#x200B;圖示，然後&#x200B;**調整預算日期**。

   如需有關調整預算日期的詳細資訊，請參閱[在資源規劃工具](../../../resource-mgmt/resource-planning/adjust-budgeting-dates.md)中調整預算日期。

1. 按一下「**儲存**」。

   如果您的每小時成本費率與工作角色相關聯，則資源預算區域中的資源預算會計算專案的&#x200B;**預算勞力成本**。 預算勞力成本會顯示在業務案例的資源預算區域與業務案例摘要中。

   >[!TIP]
   >
   >成本會以專案的貨幣顯示在業務案例中。

   業務案例中指定的預算資訊也會顯示在資源規劃工具。

   複製專案時，您還可以選擇將預算時數複製到新專案。 僅複製資源規劃工具中的預算時數。 如需詳細資訊，請參閱[複製專案](../manage-projects/copy-project.md)。
