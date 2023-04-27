---
product-area: resource-management
navigation-topic: resource-planning
title: 在資源計畫器中計算成本
description: 您可以使用成本值（而不是小時數或FTE值）來在Adobe Workfront資源計畫器中預算資源。 成本值不適用於資源計畫員中**按用戶**查看。
author: Lisa
feature: Resource Management
exl-id: 2f3ca8c2-51b3-4282-af8b-7f433365d386
source-git-commit: 61a107e1ee8a415fd94e73fc65fa5f59f7de02d1
workflow-type: tm+mt
source-wordcount: '1390'
ht-degree: 0%

---

# 在資源計畫器中計算成本

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Alina: ***Linked to the Planning in the Resource Planner article, Understanding areas of the Resource Planner. - do not move/ change/ delete.)</p>
-->

<!--'(Alina: ***Linked to the Planning in the Resource Planner article, Understanding areas of the Resource Planner. - do not move/ change/ delete.)'-->

您可以使用成本值（而不是小時數或FTE值）來在Adobe Workfront資源計畫器中預算資源。 成本值不適用於&#x200B;**按用戶查看** 在資源計畫器中查看。

>[!IMPORTANT]
>
>您必須將用戶和任務職責與「每小時成本」費率關聯，以便在資源計畫員中顯示「成本」資訊。\
>有關將「每小時成本」費率與任務職責關聯的詳細資訊，請參閱 [建立和管理作業角色](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).\
>有關將「每小時成本」費率與用戶關聯的詳細資訊，請參閱 [編輯使用者的設定檔](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

在為資源編製預算之前，請確保您對需要完成的工作（計畫小時數、FTE或成本）以及用戶開啟工作的時間（可用小時數、FTE或成本）有很好的了解。\
有關在按小時數或FTE編製預算時了解資源計畫員中資訊的詳細資訊，請參閱 [資源計畫員的「項目」和「職責」視圖中的小時數、FTE和成本資訊概覽](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>Pro及更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對資源管理的訪問，包括對資源計畫員中「編輯優先順序」和「預算小時數」的訪問</p> <p>編輯對財務資料、項目和用戶的訪問</p> <p><b>附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理您要預算資訊的項目的權限，並能夠管理財務</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 按成本在資源計畫器中顯示資訊

預設情況下，可用性和分配資訊以小時數顯示在資源計畫器中。

要按成本在資源計畫器中顯示可用、計畫和預算資訊，請執行以下操作：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 按一下 **資源**.
1. 轉至資源計畫器。
1. （條件性）選取 **依專案檢視** 或 **按角色查看**.\
   依預設 **依專案檢視** 中所有規則的URL。\
   分配和可用性資訊以小時顯示。

1. 從 **小時** 下拉式功能表，選取 **成本**.

   如果您在存取層級沒有金融資料的存取權，則此選項無法使用。\
   如果項目的幣種與系統幣種不同，則這些項目的成本將顯示在以系統幣種折換的資源計畫器中。 系統管理員定義系統貨幣。\
   如需在Workfront中設定系統貨幣和轉換率的詳細資訊，請參閱 [設定匯率](../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).\
   ![costs_in_the_planner_with_no_budgeting.png](assets/costs-in-the-planner-with-no-budgeting-350x240.png)

## 在資源計畫器中計算可用成本

要在資源計畫員中顯示可用成本值，您必須具備以下條件：

* 用戶和角色的每小時成本率
* 有關用戶可用性的資訊。

   有關用戶可用性的資訊取決於您的Workfront管理員配置資源管理首選項的方式。\
   有關計算用戶可用性和設定資源管理首選項的詳細資訊，請參閱 [配置資源管理首選項](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

下表說明了如何在資源計畫器中計算可用成本：

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
   <td>用戶可用成本</td> 
   <td> <p>每個用戶的可用成本使用以下公式計算：</p> <p><code>Available User Cost = User Available Hours * User Cost per Hour Rate</code> </p> <p><b>附註</b>

如果用戶的配置檔案中沒有「每小時成本」比率，則計算時將使用其所列任務角色的「每小時成本」比率。 如果用戶沒有與其關聯的角色，則可用用戶成本為$0。 </p> </td>
</tr> 
  <tr> 
   <td>角色可用成本</td> 
   <td> <p>每個角色的可用成本使用以下公式計算：</p> <p><code>Available Role Cost = Role Available Hours * Role Cost per Hour Rate</code> </p> <p><b>附註</b>

如果職責沒有「每小時成本」費率，則「可用職責成本」為$0。</p> </td>
</tr> 
  <tr> 
   <td>項目可用成本</td> 
   <td> <p>每個項目的可用成本使用以下公式計算：</p> <p><code>Available Project Cost = SUM(User Available Hours * User Cost per Hour Rate)</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

## 在資源計畫員中計算計畫成本

雖然您無法在資源計畫員中查看任務資訊，但是用戶、職責和項目的計畫成本是通過考慮以下任務資訊來計算的：

* 任務的分配類型。\
   您可以將任務保留為未分配，或將以下實體分配給任務：

   * 使用者（有或沒有工作角色）
   * 角色
   * 團隊\
      從資源計畫員的角度，將分配給小組的任務視為未分配。

* 此 **成本類型** 執行項目任務。\
   有關任務的「成本類型」的詳細資訊，請參閱 [追蹤成本](../../manage-work/projects/project-finances/track-costs.md).

>[!NOTE]
>
>用戶計畫成本不會影響項目計畫成本。 只有職責計畫成本會影響資源計畫員中的項目計畫成本。

計算用戶、角色和項目的計畫成本時，存在以下情況：

* 當 **成本類型** 為**用戶每小時**，並且 **無分配** 任務：

   * **角色和用戶計畫成本**:

      角色和用戶計畫成本為0.00美元。

   * **項目計畫成本**:

      項目計畫成本為0.00美元。

* 當 **成本類型** is **每小時用戶** 還有 **用戶分配** 任務：

   * **角色和用戶計畫成本**:

      用戶計畫成本使用以下公式計算：



      ```
      User Planned Cost Rate = User Planned Hours * User Cost per Hour Rate
      ```

      如果用戶的配置檔案中有成本費率，則該費率用於計算計畫成本。 否則，將使用其主要角色的系統級每小時成本率。

      >[!NOTE]
      >
      >可以將用戶分配給具有其其中一個輔助作業角色的任務，但是在此處改用主作業角色的比率。

      職責計畫成本使用以下公式計算：

      ```
      Role Planned Cost = SUM(User Planned Cost)
      ```

   * **項目計畫成本**:

      項目計畫成本為0.00美元。

* 當 **成本類型** is **每小時用戶** 還有 **職務分配** 任務：

   * **角色和用戶計畫成本**:

      用戶計畫成本為0.00美元。

      職責計畫成本使用以下公式計算：

      ```
      Role Planned Cost = Role Planned Hours * Role Cost per Hours
      ```

      分配給任務的任務職責的系統層成本/小時費率用於計算計畫成本。

   * **項目計畫成本**:

      項目計畫成本為0.00美元。

* 當 **成本類型** is **角色每小時** 還有 **無分配** 任務：

   * **角色和用戶計畫成本**:

      角色和用戶計畫成本為0.00美元。

   * **項目計畫成本**:

      項目計畫成本為0.00美元。

* 當 **成本類型** is **角色每小時** 還有 **用戶分配** 任務：

   * **角色和用戶計畫成本**:

      用戶計畫成本為0.00美元。

      職責計畫成本按以下公式計算：

      ```
      Role Planned Cost = Role Planned Hours * Role Cost per Hours
      ```

      Workfront查看用戶在任務上履行的職務職責，以計算該職責的計畫成本。

      如果用戶未與任務上的任何角色關聯，則計畫成本為$0.00。

   * **項目計畫成本**:

      項目計畫成本使用以下公式計算：

      ```
      Project Planned Cost = SUM(Role Planned Costs)
      ```

* 當 **成本類型** is **角色每小時** 還有 **職務分配** 任務：

   * **角色和用戶計畫成本**:

      用戶計畫成本為0.00美元。

      職責計畫成本按以下公式計算：

      ```
      Role Planned Cost = Role Planned Hours * Role Cost per Hours
      ```

      Workfront查看用戶在任務上履行的職務職責，以計算該職責的計畫成本。

   * **項目計畫成本**:

      項目計畫成本使用以下公式計算：

      ```
      Project Planned Cost = SUM(Role Planned Costs)
      ```

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

## 計算資源計畫員中的預算成本

要在資源計畫員中顯示預算成本值，您必須具備以下條件：

* 角色、使用者和專案的預算小時數。
* 使用者和角色的每小時成本率。

>[!NOTE]
>
>項目的「預算小時數」是根據「角色」的「預算小時數」計算，而不是根據用戶的「預算小時數」計算。

下表說明了如何在資源計畫器中計算預算成本：

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
   <td>用戶預算成本</td> 
   <td> <p>每個用戶的預算成本使用以下公式計算：</p> <p><code>Budgeted User Cost = User Budgeted Hours * User Cost per Hour Rate</code> </p> <p> <p><b>附註</b>

如果用戶的配置檔案中沒有每小時成本費率，則預算用戶成本為$0.00。</p> </p> </td>
</tr> 
  <tr> 
   <td>職責預算成本</td> 
   <td> <p>職責預算成本使用以下公式計算：</p> <p><code>Role Budgeted Cost = Role Budgeted Hours * Role Cost per Hour Rate</code> </p> <p> <p><b>附註</b>

如果職責沒有「每小時成本」費率，則預算職責成本為$0.00。</p> </p> </td>
</tr> 
  <tr> 
   <td>專案預算成本</td> 
   <td> <p>每個項目的預算成本使用以下公式計算：</p> <p><code>Project Budgeted Cost = SUM(Role Budgeted Cost). </code> </p> </td> 
  </tr> 
 </tbody> 
</table>
