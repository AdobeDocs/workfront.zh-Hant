---
product-area: resource-management
navigation-topic: resource-planning
title: 使用專案與角色檢視的資源規劃工具中的預算資源
description: 您可以在Adobe Workfront資源規劃工具中使用專案和角色檢視來預算資源。 您不能使用資源規劃工具中的使用者檢視來編列預算資源。
author: Lisa
feature: Resource Management
exl-id: b1b48529-68e7-4aee-aaa1-d78e91fbb39c
source-git-commit: 987b6e9b5f6b1feb323906cf7c24f5024fc84663
workflow-type: tm+mt
source-wordcount: '2098'
ht-degree: 0%

---

# 使用專案和角色檢視的資源規劃工具中的預算資源

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: broken off of another larger article (Planning in the RP); reformat, restructure, relink)</p>
-->

資源規劃工具的主要功能是為專案上必須完成的工作預算資源。

>[!IMPORTANT]
>
>您必須將&#x200B;**依專案檢視**&#x200B;或&#x200B;**依角色檢視**&#x200B;檢視套用至資源規劃工具，才能為資源編列預算。

在資源規劃工具中開始編列預算資訊之前，請參閱下列文章：

* [資源規劃工具概觀](../../resource-mgmt/resource-planning/get-started-resource-planner.md)
* [在Adobe Workfront中預算資源所需的存取權](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md)
* [資源規劃工具之專案與角色檢視中的時數、約當全職人數及成本資訊概要](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront套件</td> 
   <td><p>任何</p></td>
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td><p>標準</p>
       <p>規劃</p></td> 
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td> <p>編輯對資源管理的存取權，包括存取資源規劃工具中的編輯優先順序和預算時數</p> <p>編輯財務資料的存取權，以按成本預算資源</p> <p>編輯專案和使用者的存取權</p></td> 
  </tr> 
  <tr> 
   <td>物件許可權</td> 
   <td> <p>管理您要編列預算資訊之專案的許可權</p></td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 資源規劃工具中的預算資源

* 專案檢視中的[預算資源](#budget-resources-in-the-project-view)
* [角色檢視中的預算資源](#budget-resources-in-the-role-view)
* [大量預算資源](#budget-resources-in-bulk)

### 專案檢視中的預算資源 {#budget-resources-in-the-project-view}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this section is linked to the Budgeting Project Resources in the Business Case article)</p>
-->

{{step1-to-resourcing}}

1. 依預設會顯示&#x200B;**規劃師**。
1. （視條件而定）選取&#x200B;**依專案檢視**&#x200B;檢視。
1. 展開專案和工作角色，以管理專案、工作角色或使用者的配置。
1. 若要為使用者配置預算，請執行下列其中一項作業：

   * 在&#x200B;**BDG**&#x200B;欄中，手動指定使用者的預算時數、FTE或成本。

   * 按一下使用者工作角色的&#x200B;**更多**&#x200B;功能表，然後按一下&#x200B;**將使用者的計畫時數設定為預算**。\
     每個使用者的預算時數使用下列公式計算：

     `User Budgeted Hours = User Planned Hours`

1. 若要配置職位角色的預算，請執行下列其中一項作業：

   * 在&#x200B;**BDG**&#x200B;欄中，手動指定工作角色的預算時數、FTE或成本。

     >[!NOTE]
     >
     >角色預算時數已新增至專案預算時數。

   * （視條件而定）如果您已為使用者編列預算時數，請按一下工作角色的&#x200B;**更多**&#x200B;功能表，然後按一下角色的&#x200B;**使用者預算時數總計**。\
     每個角色的預算時數使用下列公式計算：

     `Role Budgeted Hours = SUM(User Budgeted Hours)`

   * 按一下專案的&#x200B;**更多**&#x200B;功能表，然後按一下&#x200B;**將角色的計畫時數設定為預算**。\
     每個角色的預算時數使用下列公式計算：\
     *

     `Role Budgeted Hours = Role Planned Hours`

     >[!NOTE]
     >   
     >* 角色預算時數已新增至專案預算時數。
     >* 可以為主要和其他（或次要）角色為使用者編列預算。
     >* 使用者角色的FTE可用性&#x200B;**百分比**&#x200B;必須為與0%不同的數字，才能在「資源規劃工具」中顯示工作角色的值。 如果使用者與具有0% **FTE可用性百分比**&#x200B;的角色相關聯，則該工作角色的可用時數值為零。 在此情況下，角色可能會顯示負值&#x200B;**淨值**。\
     >如需有關工作角色的&#x200B;**FTE可用性百分比**&#x200B;的詳細資訊，請參閱文章[編輯使用者設定檔](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

   * 在&#x200B;**BDG**&#x200B;欄中，手動指定專案的預算時數、FTE或成本。 這會將專案預算時數分配給專案下的每個角色。 存在下列情況：

      * 如果您指定的專案預算時數等於專案計畫時數，則角色預算時數符合角色計畫時數。
      * 如果您指定的專案預算時數與專案計畫時數不相等，則會根據每個角色所需的計畫時數百分比來分配角色預算時數。\
        例如，如果專案有20個計畫時數，這些時數分佈在兩個工作角色之間（顧問需要12個計畫時數，工程師需要8個計畫時數），而您為專案編列了30個小時的預算，則時數分佈如下：顧問角色接收18個預算時數，工程師角色接收12個預算時數。

1. 若要配置專案的預算，請執行下列任一項作業：

   * 為專案下的角色編列預算，如步驟7所述。\
     專案已編列預算時數的計算公式如下：

     `Project Budgeted Hours = SUM(Role Budgeted Hours)`

   * 在&#x200B;**BDG**&#x200B;欄中，手動指定專案的預算時數、FTE或成本。\
     這會更新角色預算時數，如步驟7所述。\
     ![budget_for_project.png](assets/budget-for-project-350x182.png)

1. 按一下「**儲存**」。\
   在資源規劃工具中編列資源預算後，資源的預算時數及與其相關聯的任何成本會列在每個專案的業務案例中。\
   如需瞭解業務案例之資源預算編列區域的詳細資訊，請參閱文章[業務案例區域概觀](../../manage-work/projects/define-a-business-case/areas-of-business-case.md)中的「資源預算」一節。

1. （選擇性）選取使用者檢視，以注意每個使用者在可用和計畫時數之間的任何使用者過度配置或利用不足。 預算時數在使用者檢視中不可見。

   如需Workfront如何計算使用者可用性的相關資訊，請參閱[設定資源管理喜好設定](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)。

### 角色檢視中的預算資源 {#budget-resources-in-the-role-view}

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: THIS IS WRONG - I LOGGED A BUG TO FIX THIS LINK - IT SHOULD GO TO"ACCESS NEEDED TO BUDGET IN THE RP":</p>
<p>Planning in the resource planner has links to the UI - ensure Flare notes are there for this: https://workfront.zendesk.com/hc/en-us/articles/115006356928 - the "Budgeting resources in the role view" is linked to this tooltip: ***This is linked to the product in the RP when the user does not have Manage rights on one of the projects under the role. This tool tip is linked here: "You don't have Manage permissions for all projects. Budget hours by individual project instead. Learn more...")</p>
</div>
-->

您必須擁有專案的資源管理和財務資料的編輯存取權及管理財務許可權，才能在資源規劃工具中編列資源預算。 如果您對工作角色下列出的至少一個專案只有「檢視」存取權，則無法在「角色」檢視中為角色分配預算。 您仍然可以為您擁有管理許可權的專案分配預算。

如需有關預算資源所需存取權的資訊，請參閱文章[在Adobe Workfront中預算資源所需的存取權](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md)。

若要在「資源規劃工具」的「角色」檢視中進行預算分配****請執行下列動作：

1. 按一下Adobe Workfront右上角的&#x200B;**主功能表**&#x200B;圖示![主功能表圖示](assets/main-menu-icon.png)。

1. 按一下「**資源**」。
1. 依預設會顯示&#x200B;**規劃師**。
1. （視條件而定）選取&#x200B;**依角色檢視**&#x200B;檢視。
1. 展開工作角色和專案，以管理專案、工作角色或使用者的配置。
1. 若要為使用者配置預算，請執行下列任一項作業：

   * 在&#x200B;**BDG**&#x200B;欄中，手動指定使用者的預算時數、FTE或成本。
   * 按一下專案的&#x200B;**更多**&#x200B;功能表，然後按一下&#x200B;**將使用者的計畫時數設定為預算**。\
     每個使用者的預算時數使用下列公式計算：

     `User Budgeted Hours = User Planned Hours`

1. 若要配置職位角色的預算，請執行下列其中一項作業：

   * 在&#x200B;**BDG**&#x200B;欄中，手動指定工作角色的預算時數、FTE或成本。\
     這會將角色預算時數分配給您有權管理的專案的專案預算時數。

   * 按一下工作角色的&#x200B;**更多**&#x200B;功能表，然後按一下**將專案的計畫時數設定為預算」。**角色預算時數使用下列公式計算：\
     *

     `Role Budgeted Hours = SUM(Project Budgeted Hours)`

     *專案預算時數使用下列公式計算：

     `Project Budgeted Hours = Project Planned Hours`

   * 在&#x200B;**BDG**&#x200B;欄中，手動指定工作角色下列出專案的預算時數、FTE或成本。\
     這會將專案預算時數新增至角色。

   >[!NOTE]
   >
   >可以為主要和其他（或次要）角色為使用者編列預算。 使用者角色的FTE可用性&#x200B;**百分比**&#x200B;必須為與0%不同的數字，才能在「資源規劃工具」中顯示工作角色的值。 如果使用者與具有0% **FTE可用性百分比**&#x200B;的角色相關聯，則該工作角色的可用時數值為零。 在此情況下，角色可能會顯示負值&#x200B;**淨值**。\
   >如需有關工作角色的&#x200B;**FTE可用性百分比**&#x200B;的詳細資訊，請參閱文章[編輯使用者設定檔](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

1. 若要配置專案的預算，請執行下列任一項作業：

   * 在&#x200B;**BDG**&#x200B;欄中，手動指定專案的預算時數、FTE或成本。\
     這也會更新專案所列出之角色的預算時數。

   * 按一下工作角色的&#x200B;**更多**&#x200B;功能表，然後按一下&#x200B;**將專案的計畫時數設定為預算**。\
     專案已編列預算時數的計算公式如下：

     `Project Budgeted Hours = Project Planned Hours`

     專案預算時數已新增至角色預算時數。

   * （視條件而定）如果您已為使用者編列時數預算，請按一下專案的&#x200B;**更多**&#x200B;功能表，然後按一下專案的&#x200B;**使用者預算時數總計**。\
     專案預算時數使用下列公式計算：

     `Project Budgeted Hours = SUM(User Budgeted Hours)`

     ![budget_by_role.png](assets/budget-by-role-350x181.png)

1. 按一下「**儲存**」。\
   在資源規劃工具中編列資源預算後，資源的預算時數及與其相關聯的任何成本會列在每個專案的業務案例中。
如需有關瞭解業務案例的資源預算編列區域的詳細資訊，請參閱文章[業務案例中的預算資源](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)。

1. （選擇性）選取&#x200B;**依使用者檢視**&#x200B;檢視，以注意每個使用者的可用和計畫時數之間是否有使用者過度配置或利用不足。 「依使用者檢視」檢視中看不到已編列預算時數。

### 大量預算資源 {#budget-resources-in-bulk}

使用快速連結時，您可以大量為資源配置預算。 快速連結僅適用於「專案」和「角色檢視」。

![自動編列預算選項](assets/rp-project-view-with-automatic-budgeting-options-on-project-350x173.png)

>[!NOTE]
>
>使用資源預算分配的快速連結時，預算僅自動套用至畫面上顯示的時間期間。 如果專案的時間表所跨越的時間超過熒幕上顯示的時間表，您必須從左至右捲動，然後使用快速連結來自動為資源編列預算。

若要大量編列資源預算：

1. 前往。\
   如需有關存取資源規劃工具的詳細資訊，請參閱文章[資源規劃工具概觀](../../resource-mgmt/resource-planning/get-started-resource-planner.md)中的「存取資源規劃工具」一節。\
   您可以管理的專案清單會顯示在清單中。

1. （可選）展開每個專案以檢視與其相關聯的工作角色清單。\
   或
1. （選擇性）選取&#x200B;**依角色檢視**，然後展開每個角色以檢視與其關聯的專案清單。
1. 將游標停留在專案或工作角色名稱上。
1. 按一下專案或角色名稱最右邊顯示的&#x200B;**更多**&#x200B;圖示![options_icon_resource_planner.png](assets/options-icon-resource-planner.png)。

1. 按一下其中一個可用選項，即可自動指定其他物件的預算時數(BDG)量。

   根據您在專案或角色上按一下「更多」圖示，大量編列預算的選項會有所不同。 下表說明專案和角色可用的選項：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td> </td> 
      <td><strong>專案檢視</strong> </td> 
      <td><strong>角色檢視</strong> </td> 
     </tr> 
     <tr> 
      <td>專案選項</td> 
      <td> 
       <ul> 
        <li><strong>將角色的計畫時數設定為預算</strong>：選取此選項可讓角色的預算時數與其計畫時數相同。 將為專案預算時數顯示角色的預算時數總計。 </li> 
        <li><strong>調整預算日期</strong> ：選取此選項可將預算時數移至不同的時間範圍。<br>如需有關調整預算日期的相關資訊，請參閱<a href="../../resource-mgmt/resource-planning/adjust-budgeting-dates.md" class="MCXref xref">在資源規劃工具中調整預算日期</a>。</li> 
       </ul> </td> 
      <td> 
       <ul> 
        <li><strong>將使用者的計畫時數設定為預算</strong>：選取此選項可讓使用者的預算時數與其計畫時數相同。 </li> 
        <li><strong>專案的使用者預算時數總計</strong>：選取此選項可將所有使用者預算時數加總在一起，並將總計顯示為專案和角色的預算時數。 建議您手動為使用者編列預算，或先使用上一個選項後，再使用此選項。 </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td>角色選項</td> 
      <td> 
       <ul> 
        <li><strong>將使用者的計畫時數設定為預算</strong>：選取此選項可讓使用者的預算時數與其計畫時數相同。 </li> 
        <li><strong>角色的使用者預算時數總計</strong>：選取此選項可將使用者的所有預算時數加總在一起，並將總計顯示為角色和專案的預算時數。 建議您手動為使用者編列預算，或先使用上一個選項後，再使用此選項。 </li> 
       </ul> </td> 
      <td> 
       <ul> 
        <li><strong>將專案的計畫時數設定為預算</strong>：選取此選項可讓專案預算時數變得與專案計畫時數相同。 </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >如果缺少在資源規劃工具中工作的某些先決條件，則某些選項可能未顯示。
   >
   >
   >如需有關在資源規劃工具中正確編列預算所必須滿足的先決條件的詳細資訊，請參閱[資源規劃工具概觀](../../resource-mgmt/resource-planning/get-started-resource-planner.md)文章中的「在資源規劃工具中工作的先決條件」一節。\
   >例如，某些選項可能不會顯示在下列案例中：
   >
   >   
   >   
   >   * 當專案與資源集區沒有關聯時
   >   * 當與專案關聯的資源集區不包含使用者時
   >   * 當與專案關聯的資源集區包含無關聯工作角色的使用者時。
   >   
   >
