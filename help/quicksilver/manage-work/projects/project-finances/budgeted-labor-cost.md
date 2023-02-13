---
content-type: reference
product-area: projects
navigation-topic: financials
title: 了解項目的預算人工成本和預算工時
description: 了解項目的預算人工成本和預算工時
author: Alina
feature: Work Management
exl-id: 01020bbb-7cf9-4461-b0b6-dcbbc537c616
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1128'
ht-degree: 0%

---

# 了解項目的預算人工成本和預算工時

<!--
<(NOTE: Keep the structure of this article similar to Calculating Budgeted Cost)</p>
-->

您可以使用Adobe Workfront資源計畫器為工作預算資源。

在為項目工作預算資源時，Workfront會根據每小時成本值計算職責、項目和用戶的預算人工成本。

項目的資源計畫員預算人工成本是與分配給完成項目工作的任務職責相關聯的成本與可能承擔每個職責完成工作的估計小時數（資源計畫員預算小時數）之間的計算。

>[!IMPORTANT]
>
>用戶的資源計畫員預算人工成本不會影響項目的人工成本。 只有職務職責的人工成本會影響項目成本。

## 任務職責和項目的預算人工成本概覽

Workfront使用項目上職務職責的預算人工成本來計算項目的預算人工成本。

>[!TIP]
>
>在「業務案例」中，項目的預算人工成本在報表和清單中顯示為資源計畫員預算人工成本。

此 **預算人工成本** （或資源計畫員預算人工成本）按以下公式計算：

`Resource Planner Budgeted Labor Cost = SUM ( Resource Planner Budgeted Hours for each job role on the project * Cost per Hour rate of each job role on the project)`

上述計算中使用的欄位參考下列項目：

* 在項目或「資源計畫員」的「資源預算」區域中為任務職責編入預算的小時數。

   有關資源計畫員中預算資源的詳細資訊，請參閱文章中的「資源計畫員中的預算資源」部分 [資源計畫員概覽](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

   有關在「業務案例」的「資源預算」區域中預算資源的詳細資訊，請參閱 [業務案例中的預算資源](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

* 此 **作業角色的每小時成本率** 在上述計算中，是指與項目上的每個任務職責相關聯的成本。\
   有關建立和管理職務職責以及將其與成本費率關聯的詳細資訊，請參閱文章 [建立和管理作業角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

>[!NOTE]
>
>Workfront會使用專案的貨幣計算所有成本資訊。 如果在「資源計畫員」中為資源指定「預算小時數」，則禁用更改項目幣種的選項。\
>如需變更專案貨幣的詳細資訊，請參閱文章 [更改項目幣種](../../../manage-work/projects/project-finances/change-project-currency.md).

## 用戶預算人工成本概覽

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Update the following section in the Create a Business Case article, as well, when you update it here.)</p>
-->

>[!IMPORTANT]
>
>用戶預算的人工成本不會影響項目的預算人工成本。 只有項目上任務職責的人工成本會影響項目的資源計畫員預算人工成本。
> 
>所有用戶的所有人工成本合計可能等於或不等於與用戶關聯的任務職責的資源計畫員預算人工成本。
>
>如果您估計資源計畫員中用戶的預算小時數，則與它們關聯的成本是與用戶關聯的任務職責的成本。 它們不是與使用者或其費率相關的成本。

如果用戶與項目上的任務職責相關聯，並且其小時數已預算在資源計畫器中，則其預算人工成本將按以下名稱顯示，具體取決於您在Workfront中查看這些職責的位置：

* [!UICONTROL **預算人工成本**]:業務案例的「資源預算」區域，其各自職責。

   ![](assets/budgeted-labor-cost-for-users-in-business-case-highlighted-350x73.png)

* [!UICONTROL **BDG**]:按成本查看「項目」和「職責」視圖中的資訊時，資源計畫員。

   ![](assets/budgeted-labor-cost-for-users-in-rp-project-view-cost--highlighted-350x115.png)

如果用戶滿足以下要求，則用戶將顯示在Business Case的「資源預算」區域中其各自的職責下，或顯示在Oracle Resource Planner中：

* 它們與專案上的其中一個工作角色相關聯。
* 它們在資源計畫器中指定了預算小時數。
* 他們的設定檔有相關聯的每小時成本率。

   有關向用戶添加每小時成本費率的詳細資訊，請參閱文章 [編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* 用戶是與項目關聯的一個資源池的一部分。

用戶的預算人工成本按以下公式計算：

`User Budgeted Labor Cost = Budgeted hours for the user on the project * Cost per Hour rate of the user`

## 查找項目的預算人工成本

「業務案例」或「資源計畫員」的「資源預算」區域中反映的「預算人工成本」將以下名稱顯示在Workfront的以下區域：

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td><strong>預算人工成本顯示名稱</strong></td> 
     <td><strong>Workfront地區</strong></td> 
    </tr> 
    <tr> 
     <td>預算勞力成本</td> 
     <td>業務案例的資源預算區</td> 
    </tr> 
    <tr> 
     <td>預算成本</td> 
     <td><p>利用率報表成本視圖</p><p>如需詳細資訊，請參閱 <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">查看利用率資訊</a> .</p></td> 
    </tr> 
    <tr> 
     <td>預算 </td> 
     <td>按成本列出的資源計畫員項目或職責視圖</td> 
    </tr> 
    <tr> 
     <td>資源計畫員項目預算人工成本</td> 
     <td> <p>專案報表</p> <p>項目（財務資料）報告</p> <p>任務報告</p> <p>問題報告</p> <p>預算小時報表</p> <p>如需建立報表的相關資訊，請參閱文章 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">建立自訂報表</a>.</p> </td> 
    </tr> 
   </tbody> 
  </table>

>[!NOTE]
>
>如果您使用「Adobe Workfront方案計畫器」來預算項目資源，則「業務案例」的「資源預算」區域中的「預算人工成本」與與項目連結的方案的「人員成本」相同。 方案規劃器僅適用於新的Adobe Workfront體驗，需要額外的許可。 有關Workfront方案計畫器的資訊，請參閱 [方案計畫員概覽](../../../scenario-planner/scenario-planner-overview.md). 有關使用方案計畫員編製預算資源的資訊，請參閱 [使用方案計畫器在業務案例中的預算資源](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

## 找出項目的預算小時數

<!--
(NOTE: Keep the structure of this article similar to Calculating Budgeted Cost)
-->

預算小時數影響項目的預算人工成本（或資源計畫員預算成本）的值。

項目的預算人工成本是與分配給完成項目工作的職務職責相關的成本，以及每個職責完成工作所可能承擔的估計小時數（預算小時數）。

您可以在下表所列欄位中檢視Workfront的預算小時數。

>[!NOTE]
>
>Workfront中「預算小時數」的其他提及是指使用已從Workfront移除的已棄用功能編入預算的小時數。 這些欄位僅供檢視，當您使用目前的資源預算工具時，不會更新為目前的資訊。

在「業務案例」或「資源計畫員」的「資源預算」區域中預算的小時數顯示在Workfront的以下區域中，並以以下名稱顯示：

* **小時**:業務案例的資源預算區
* **BDG**：按小時查看的資源計畫員
* **預算小時數**:利用率報告小時視圖有關資訊，請參閱 [查看資源利用資訊](../../../resource-mgmt/resource-utilization/view-utilization-information.md).
* **巴德。 小時**:預算小時報表

   「預算小時數」報告中的「預算小時數」對象指與已廢止的資源管理工具相關的資訊。 只有&quot;巴德&quot; 此報表中的「小時數」欄位是指在「資源計畫員」或項目業務案例的「資源預算」區域中預算的小時數。

   如需建立報表的詳細資訊，請參閱文章 **建立自訂報表**.
* **資源計畫員預算小時數**:（在以下報告中）:

   * 專案報表
   * 項目（財務資料）報告
   * 任務報告
   * 問題報告
   * 預算小時報表
