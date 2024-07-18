---
content-type: reference
product-area: projects
navigation-topic: financials
title: 瞭解專案的預算勞力成本和預算時數
description: 瞭解專案的預算勞力成本和預算時數
author: Alina
feature: Work Management
exl-id: 01020bbb-7cf9-4461-b0b6-dcbbc537c616
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1128'
ht-degree: 0%

---

# 瞭解專案的預算勞力成本和預算時數

<!--
<(NOTE: Keep the structure of this article similar to Calculating Budgeted Cost)</p>
-->

您可以使用Adobe Workfront資源規劃工具為工作預算資源。

當您為專案工作編列資源預算時，Workfront會根據每小時成本值計算角色、專案和使用者的預算勞力成本。

專案的資源規劃工具預算勞力成本是與指定完成專案工作之職務角色相關成本，與完成工作之每個角色的預估時數金額（資源規劃工具預算時數）之間的計算。

>[!IMPORTANT]
>
>使用者的資源規劃工具預算勞力成本不會影響專案的成本。 只有工作角色的勞力成本會影響專案成本。

## 工作角色與專案的預算勞力成本概要

Workfront使用專案上工作角色的預算勞力成本來計算專案的預算勞力成本。

>[!TIP]
>
>業務案例中專案的預算勞力成本在報表和清單中顯示為「資源規劃工具預算勞力成本」。

專案的&#x200B;**預算勞力成本** （或資源規劃工具預算勞力成本）是根據下列公式計算的：

`Resource Planner Budgeted Labor Cost = SUM ( Resource Planner Budgeted Hours for each job role on the project * Cost per Hour rate of each job role on the project)`

上述計算中所使用的欄位參考下列內容：

* 專案或資源規劃工具之資源預算區域中工作角色的預算時數。

  如需有關資源規劃工具中預算資源的詳細資訊，請參閱文章[資源規劃工具概觀](../../../resource-mgmt/resource-planning/get-started-resource-planner.md)中的「資源規劃工具中的預算資源」一節。

  如需有關業務案例資源預算區域之預算資源的詳細資訊，請參閱業務案例中的[預算資源](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)。

* 在上述計算中，工作角色&#x200B;**的**&#x200B;每小時成本費率是指與專案上每個工作角色相關的成本。\
  如需有關建立和管理職位角色以及將它們與成本費率關聯的詳細資訊，請參閱文章[建立和管理職位角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)。

>[!NOTE]
>
>Workfront會使用專案的貨幣來計算所有成本資訊。 如果您在資源規劃工具中指定資源的預算時數，則會停用變更專案幣別的選項。\
>如需有關變更專案貨幣的詳細資訊，請參閱文章[變更專案貨幣](../../../manage-work/projects/project-finances/change-project-currency.md)。

## 使用者預算勞力成本概要

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Update the following section in the Create a Business Case article, as well, when you update it here.)</p>
-->

>[!IMPORTANT]
>
>使用者預算勞力成本不會影響專案的預算勞力成本。 只有專案上工作角色的勞力成本會影響專案的資源規劃工具預算勞力成本。
> 
>所有使用者的所有勞力成本總計可能等於或不等於與使用者相關聯之職務角色的資源規劃工具預算勞力成本。
>
>如果您在資源規劃工具中估計使用者的預算時數，則與使用者關聯的成本就是與使用者關聯的工作角色成本。 費用與使用者或其費率無關。

如果使用者與專案中的工作角色相關聯，且其時數在資源規劃工具中編列了預算，則其預算勞力成本會根據您在Workfront中檢視他們的位置，以下列名稱顯示：

* [!UICONTROL **預算勞力成本**]：業務案例在其各自角色下的資源預算區域。

  ![](assets/budgeted-labor-cost-for-users-in-business-case-highlighted-350x73.png)

* [!UICONTROL **BDG**]：資源規劃工具在依成本檢視專案和角色檢視中檢視資訊時。

  ![](assets/budgeted-labor-cost-for-users-in-rp-project-view-cost--highlighted-350x115.png)

如果使用者符合下列需求，則他們會在業務案例的資源預算區域顯示其各自的角色下，或顯示在「資源規劃工具」中：

* 它們與專案的其中一個工作角色相關聯。
* 他們已在資源規劃工具中指定預算時數。
* 他們有與其設定檔相關聯的每小時成本費率。

  如需有關新增每小時成本費率給使用者的詳細資訊，請參閱文章[編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

* 使用者屬於與專案關聯的其中一個資源集區。

使用者的預算勞力成本會透過下列公式計算：

`User Budgeted Labor Cost = Budgeted hours for the user on the project * Cost per Hour rate of the user`

## 找出專案的預算勞力成本

反映在業務案例或資源規劃工具的資源預算區域中的預算勞力成本，顯示在Workfront的以下區域中，名稱如下：

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td><strong>預算勞力成本顯示名稱</strong></td> 
     <td><strong>Workfront區域</strong></td> 
    </tr> 
    <tr> 
     <td>預算勞力成本</td> 
     <td>業務案例的資源預算區域</td> 
    </tr> 
    <tr> 
     <td>預算成本</td> 
     <td><p>使用率報表成本檢視</p><p>如需詳細資訊，請參閱<a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">檢視使用率資訊</a>。</p></td> 
    </tr> 
    <tr> 
     <td>預算 </td> 
     <td>資源規劃工具專案或角色檢視，按成本</td> 
    </tr> 
    <tr> 
     <td>資源規劃工具專案預算勞力成本</td> 
     <td> <p>專案報告</p> <p>專案（財務資料）報表</p> <p>任務報告</p> <p>問題報告</p> <p>已編列預算時數報告</p> <p>如需有關建立報告的資訊，請參閱文章<a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">建立自訂報告</a>。</p> </td> 
    </tr> 
   </tbody> 
  </table>

>[!NOTE]
>
>如果您使用「Adobe Workfront案例規劃工具」來預算專案資源，則「業務案例」的「資源預算」區域中的預算勞力成本與連結至專案的方案的「人員成本」相同。 Scenario Planner僅在新的Adobe Workfront體驗中可用，並且需要額外的授權。 如需Workfront Scenario Planner的相關資訊，請參閱[Scenario Planner概觀](../../../scenario-planner/scenario-planner-overview.md)。 如需有關使用「情境規劃工具」預算資源的資訊，請參閱使用「情境規劃工具」的商業案例中的[預算資源](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md)。

## 找出專案的預算時數

<!--
(NOTE: Keep the structure of this article similar to Calculating Budgeted Cost)
-->

預算時數會影響專案的預算勞力成本值（或資源規劃工具預算成本）。

專案的預算勞力成本是與指派完成專案工作之職務角色相關的成本，以及完成工作所需之每個角色的預估時數（預算時數）。

您可以在下表所列欄位中檢視Workfront中的預算時數。

>[!NOTE]
>
>Workfront中提及的「預算時數」指使用已從Workfront移除之已棄用功能的預算時數。 這些是僅供檢視的欄位，當您使用目前的資源預算工具時，不會以目前的資訊更新。

業務案例或資源規劃工具的資源預算區域中所編列的時數，會顯示在Workfront的下列區域中，並以下列名稱顯示：

* **小時**：業務案例的資源預算區域
* **BDG**：資源規劃工具已依時數檢視
* **預算時數**：使用報告時數檢視
如需相關資訊，請參閱[檢視資源使用率資訊](../../../resource-mgmt/resource-utilization/view-utilization-information.md)。
* **預算。 時數**：預算時數報告

  「預算時數」報表中的「預算時數」物件會參考與已棄用資源管理工具相關的資訊。 只有「Bud」。 時數」欄位在此報告中參考資源規劃工具或專案業務案例的資源預算區域中的預算時數。

  如需有關建立報告的詳細資訊，請參閱文章&#x200B;**建立自訂報告**。
* **資源規劃工具預算時數**：在下列報表中：

   * 專案報告
   * 專案（財務資料）報表
   * 任務報告
   * 問題報告
   * 已編列預算時數報告
