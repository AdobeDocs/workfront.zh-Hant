---
product-area: resource-management
navigation-topic: resource-planning
title: 在資源規劃工具中計算成本
description: 您可以在Adobe Workfront資源規劃工具中使用成本值（而不是時數或FTE值）來預算資源。 成本值無法用於「資源規劃工具」中的**依使用者檢視**檢視。
author: Lisa
feature: Resource Management
exl-id: 2f3ca8c2-51b3-4282-af8b-7f433365d386
source-git-commit: 987b6e9b5f6b1feb323906cf7c24f5024fc84663
workflow-type: tm+mt
source-wordcount: '1392'
ht-degree: 0%

---

# 在資源規劃工具中計算成本

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Alina: ***Linked to the Planning in the Resource Planner article, Understanding areas of the Resource Planner. - do not move/ change/ delete.)</p>
-->

<!--'(Alina: ***Linked to the Planning in the Resource Planner article, Understanding areas of the Resource Planner. - do not move/ change/ delete.)'-->

您可以在Adobe Workfront資源規劃工具中使用成本值（而不是時數或FTE值）來預算資源。 資源規劃工具中的&#x200B;**依使用者的檢視**&#x200B;檢視無法使用成本值。

>[!IMPORTANT]
>
>您必須將使用者和職位角色與每小時成本費率相關聯，才能在資源規劃工具中顯示成本資訊。\
>如需將每小時成本費率與工作角色產生關聯的詳細資訊，請參閱[建立和管理工作角色](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)。\
>如需將每小時成本費率與使用者產生關聯的詳細資訊，請參閱[編輯使用者的設定檔](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

在編列資源預算之前，請確定您已清楚瞭解需要完成的工作（計畫時數、約當全職人數或成本），以及使用者開放工作的時間（可用時數、約當全職人數或成本）。\
如需有關在按時數或約當全職人數進行預算時瞭解資源規劃工具中資訊的更多資訊，請參閱資源規劃工具專案與角色檢視中的[時數概觀、約當全職人數和成本資訊](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)。

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
   <td> <p>編輯對資源管理的存取權，包括存取資源規劃工具中的編輯優先順序和預算時數</p> <p>編輯財務資料、專案和使用者的存取權</p></td> 
  </tr> 
  <tr> 
   <td>物件許可權</td> 
   <td> <p>管理您要為其編列預算資訊之專案的許可權，並具備管理財務的能力</p></td>
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在資源規劃工具（依成本）中顯示資訊

依預設，可用性和配置資訊會顯示在資源規劃工具的時數中。

若要在資源規劃工具中依成本顯示可用、計畫和預算資訊：

{{step1-to-resourcing}}

1. 前往資源規劃工具。
1. （視條件而定）選取&#x200B;**依專案檢視**&#x200B;或&#x200B;**依角色檢視**。\
   預設會選取&#x200B;**依專案檢視**。\
   配置和可用性資訊會以時數顯示。

1. 從&#x200B;**小時**&#x200B;下拉式功能表中，選取&#x200B;**成本**。

   如果您無權存取存取存取層級中的財務資料，則此選項不可用。\
   如果專案的幣別與系統幣別不同，則這些專案的「成本」會顯示在以系統幣別轉換的資源規劃工具。 您的系統管理員會定義系統貨幣。\
   如需在Workfront中設定系統貨幣和轉換率的詳細資訊，請參閱[設定匯率](../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md)。\
   ![costs_in_the_planner_with_no_budgeting.png](assets/costs-in-the-planner-with-no-budgeting-350x240.png)

## 在資源規劃工具中計算可用成本

若要在「資源規劃工具」中顯示「可用成本」值，您必須具備下列專案：

* 使用者和角色的每小時成本費率
* 有關使用者可用性的資訊。

  取得使用者可用性相關資訊取決於您的Workfront管理員如何設定資源管理偏好設定。\
  如需有關計算使用者使用狀態及設定資源管理喜好設定的詳細資訊，請參閱[設定資源管理喜好設定](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)。

下表說明如何在「資源規劃工具」中計算「可用成本」：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>可用成本</strong> </th> 
   <th><strong>計算</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>使用者可用成本</td> 
   <td> <p>「每位使用者的可用成本」使用下列公式計算：</p> <p><code>Available User Cost = User Available Hours * User Cost per Hour Rate</code> </p> <p><b>附註</b>

如果使用者設定檔中沒有每小時成本費率，則計算時會使用列出該使用者之職務角色的每小時成本費率。 如果使用者沒有關聯的角色，則可用使用者成本為$0。 </p> </td>
</tr> 
  <tr> 
   <td>角色可用成本</td> 
   <td> <p>「每個角色的可用成本」使用下列公式計算：</p> <p><code>Available Role Cost = Role Available Hours * Role Cost per Hour Rate</code> </p> <p><b>附註</b>

如果角色沒有每小時成本費率，則可用角色成本為$0。</p> </td>
</tr> 
  <tr> 
   <td>專案可用成本</td> 
   <td> <p>「每個專案的可用成本」使用下列公式計算：</p> <p><code>Available Project Cost = SUM(User Available Hours * User Cost per Hour Rate)</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

## 在資源規劃工具中計算計畫成本

雖然您無法在資源規劃工具中檢視任務資訊，但使用者、角色和專案的計畫成本是透過考量下列任務資訊來計算的：

* 任務的指派型別。\
  您可以讓任務保持未指派狀態，或將下列實體指派給任務：

   * 使用者（無論是否擁有工作角色）
   * 角色
   * 團隊\
     從資源規劃工具的角度來看，指派給團隊的任務會視為未指派。

* 專案上任務的&#x200B;**成本型別**。\
  如需有關任務的成本型別的詳細資訊，請參閱[追蹤成本](../../manage-work/projects/project-finances/track-costs.md)。

* 職務角色和使用者成本費率的有效日期。

  例如，如果角色或使用者在2月有10個計畫時數，在3月有10個計畫時數，但成本費率已從$12變更為$20 （在3月），則2月的計畫成本值為$120 （在3月），計畫成本為$200 （在3月）。

>[!NOTE]
>
>使用者計畫成本不會影響專案計畫成本。 只有角色計畫成本會影響資源規劃工具中的專案計畫成本。

計算使用者、角色和專案的計畫成本時，有下列情況：

* 當&#x200B;**成本型別**&#x200B;為&#x200B;**使用者小時**&#x200B;且任務上有&#x200B;**無指派**&#x200B;時：

   * **角色和使用者計畫成本**：

     角色和使用者計畫成本為$0.00。

   * **專案計畫成本**：

     專案計畫成本為$0.00。

* 當&#x200B;**成本型別**&#x200B;為&#x200B;**使用者小時**，且任務中有&#x200B;**使用者指派**&#x200B;時：

   * **角色和使用者計畫成本**：

     「使用者計畫成本」使用下列公式計算：

     `User Planned Cost Rate = User Planned Hours * User Cost per Hour Rate`

     如果使用者在其設定檔中有成本費率，則會使用該費率來計算計畫成本。 否則，會使用其主要角色的系統層級每小時成本費率。

     >[!NOTE]
     >
     >您可以將使用者指派給具有其中一個次要工作角色的任務，但此處會改用主要工作角色的速率。

     角色計畫成本使用下列公式計算：

     `Role Planned Cost = SUM(User Planned Cost)`

   * **專案計畫成本**：

     專案計畫成本為$0.00。

* 當&#x200B;**成本型別**&#x200B;為&#x200B;**使用者小時**，且任務上有&#x200B;**工作角色指派**&#x200B;時：

   * **角色和使用者計畫成本**：

     使用者計畫成本為$0.00。

     角色計畫成本使用下列公式計算：

     `Role Planned Cost = Role Planned Hours * Role Cost per Hours`

     系統會使用指派給任務之工作角色的系統層級每小時成本費率來計算計畫成本。

   * **專案計畫成本**：

     專案計畫成本為$0.00。

* 當&#x200B;**成本型別**&#x200B;為&#x200B;**每小時**&#x200B;角色，且任務上有&#x200B;**無指派**&#x200B;時：

   * **角色和使用者計畫成本**：

     角色和使用者計畫成本為$0.00。

   * **專案計畫成本**：

     專案計畫成本為$0.00。

* 當&#x200B;**成本型別**&#x200B;為&#x200B;**每小時**&#x200B;角色，且任務上有&#x200B;**使用者指派**&#x200B;時：

   * **角色和使用者計畫成本**：

     使用者計畫成本為$0.00。

     角色計畫成本的計算公式如下：

     `Role Planned Cost = Role Planned Hours * Role Cost per Hours`

     Workfront會檢視使用者在任務上所履行的工作角色，以計算該角色的計畫成本。

     如果使用者未與任務上的任何角色相關聯，則計畫成本為$0.00。

   * **專案計畫成本**：

     專案計畫成本使用下列公式計算：

     `Project Planned Cost = SUM(Role Planned Costs)`

* 當&#x200B;**成本型別**&#x200B;為&#x200B;**角色每小時**，且任務上有&#x200B;**工作角色指派**&#x200B;時：

   * **角色和使用者計畫成本**：

     使用者計畫成本為$0.00。

     角色計畫成本的計算公式如下：

     `Role Planned Cost = Role Planned Hours * Role Cost per Hours`

     Workfront會檢視使用者在任務上所履行的工作角色，以計算該角色的計畫成本。

   * **專案計畫成本**：

     專案計畫成本使用下列公式計算：

     `Project Planned Cost = SUM(Role Planned Costs)`

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(table below ideal but drafted because it does not display correctly in Markdown)</p>
-->

<!--
<table style="table-layout:auto">
<col>
<col>
<col>
<col>
<col>
<col>
<col>
<tbody>
<tr>
<td rowspan="2">&nbsp;</td>
<td colspan="3"> <p><strong>Cost Type = User Hourly</strong> </p><strong>User Planned Cost</strong> </td>
<td colspan="3"> <p><strong>Cost Type = Role Hourly</strong> </p><strong>Role Planned Cost</strong> </td>
</tr>
<tr>
<td> <p><strong>No Assignment</strong> </p> </td>
<td> <p><strong>User Assignment</strong> </p> </td>
<td> <p><strong>Job Role Assignment</strong> </p> </td>
<td> <p><strong>No Assignment</strong> </p> </td>
<td> <p><strong>User Assignment</strong> </p> </td>
<td> <p><strong>Job Role Assignment</strong> </p> </td>
</tr>
<tr>
<td> <p><strong>User and Role Planned Cost</strong> </p> <p> </p> </td>
<td> <p>The Role and User Planned Costs are $0.00.</p> </td>
<td> <p> The User Planned Cost is calculated using the following formula: </p> <p><code> User Planned Cost Rate = User Planned Hours * User Cost per Hour Rate </code> </p> <p> If a user has a cost rate in their profile, then that rate is used to calculate Planned Cost. Otherwise, the system-level Cost per Hour rate of their Primary Role is used. <br><note type="note">
The user can be assigned to the task with one of their secondary job roles, but the rate of the primary job role is used here instead.
</note></p> <p> The Role Planned Cost is calculated using the following formula: </p> <p><code>Role Planned Cost = SUM(User Planned Cost)</code> </p> </td>
<td> <p> The User Planned Cost is $0.00. </p> <p> The Role Planned Cost is calculated using the following formula: </p> <p><code> Role Planned Cost = Role Planned Hours * Role Cost per Hours </code> </p> <p> The system-level Cost per Hour rate of the job role assigned to the task is used to calculate Planned Cost. </p> </td>
<td> <p>The Role and User Planned Costs are $0.00.</p> </td>
<td> <p> The User Planned Cost is $0.00. </p> <p> The Role Planned Cost is calculated by the following formula: </p> <p><code>Role Planned Cost = Role Planned Hours * Role Cost per Hours</code> </p> <p>Workfront looks at the job role that the user fulfills on the task to calculate the Planned Cost for the role. </p> <p> If the user is not associated with any role on the task, the Planned Cost is $0.00. </p> </td>
<td> <p> The User Planned Cost is $0.00. </p> <p> The Role Planned Cost is calculated by the following formula: </p> <p><code>Role Planned Cost = Role Planned Hours * Role Cost per Hours</code> </p> <p>Workfront looks at the job role that the user fulfills on the task to calculate the Planned Cost for the role. </p> <p> </p> <p> </p> </td>
</tr>
<tr>
<td rowspan="2"> <p><strong>Project Planned Cost</strong> </p> <p> </p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td colspan="2"> <p> The Project Planned Cost is calculated using the following formula: </p> <p><code> Project Planned Cost = SUM(Role Planned Costs) </code> </p> <p> </p> </td>
</tr>
<tr>
<td colspan="6"> <note type="note">
User Planned Costs do not influence the Project Planned Cost. Only the Role Planned costs affect the Project Planned Costs, in the Resource Planner.
</note> </td>
</tr>
</tbody>
</table>
-->

## 在資源規劃工具中計算預算成本

若要在「資源規劃工具」中顯示預算成本值，您必須具備下列專案：

* 角色、使用者和專案的預算時數。
* 使用者和角色的每小時成本費率。

>[!NOTE]
>
>專案的預算時數是根據角色的預算時數來計算，而不是根據使用者的預算時數。

下表說明如何在資源規劃工具中計算預算成本：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>預算成本</strong> </th> 
   <th><strong>計算</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>使用者預算成本</td> 
   <td> <p>每位使用者的預算成本的計算公式如下：</p> <p><code>Budgeted User Cost = User Budgeted Hours * User Cost per Hour Rate</code> </p> <p> <p><b>附註</b>

如果使用者在其設定檔中沒有每小時成本費率，則預算使用者成本為$0.00。</p> </p> </td>
</tr> 
  <tr> 
   <td>角色預算成本</td> 
   <td> <p>角色預算成本使用下列公式計算：</p> <p><code>Role Budgeted Cost = Role Budgeted Hours * Role Cost per Hour Rate</code> </p> <p> <p><b>附註</b>

如果角色沒有每小時成本費率，則預算角色成本為$0.00。</p> </p> </td>
</tr> 
  <tr> 
   <td>專案預算成本</td> 
   <td> <p>每個專案的預算成本使用下列公式計算：</p> <p><code>Project Budgeted Cost = SUM(Role Budgeted Cost). </code> </p> </td> 
  </tr> 
 </tbody> 
</table>
