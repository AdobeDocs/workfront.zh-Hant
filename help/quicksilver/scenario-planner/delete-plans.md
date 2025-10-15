---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 刪除「案例規劃工具」中的計畫
description: 您可以刪除您建立的計畫。 您無法刪除與您共用的計畫。
author: Alina
feature: Workfront Scenario Planner
exl-id: 74515723-3822-425a-aa9e-970af63f9189
source-git-commit: aa2e9a012a60ab10e2d027dedae520b5e06686c7
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 1%

---

# 刪除[!DNL Scenario Planner]中的計畫

您可以刪除您建立的計畫。 您無法刪除與您共用的計畫。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 封裝</p> </td> 
   <td> 
   <p>Workfront Ultimate</p>
<p><b>附註</b></p>
<p>如果您有不同的Workfront套件，請洽詢您的Workfront代表。</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 授權</p> </td> 
   <td> <p>[!UICONTROL Light]或更高</p> 
   <p>[!UICONTROL Review]或更高版本</p> </td> 
  </tr> 
    <tr> 
   <td>存取層級設定</td> 
   <td> <p>[!UICONTROL Edit]對的存取權 [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr> 
   <td> <p>物件許可權 </p> </td> 
   <td> <p>[!UICONTROL Manage]計畫的許可權</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關存取Scenario Planner的詳細資訊，請參閱[使用 [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md)所需的存取。

如需Workfront存取需求的相關資訊，請參閱[Workfront檔案的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <ul></li>
   <li><p>New: Ultimate </p></li>
   <p>The Scenario Planner is not available for the new Workfront Select or Workfront Prime plans. </p>
   <li><p>Current: [!UICONTROL Business] or higher</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td> <p>New: Light or higher</p> 
   <p>Current: [!UICONTROL Review] or higher</p> </td> 
  </tr> 
  <tr> 
   <td>Product* </td> 
   <td> <ul><li><p>For the new Workfront plans:</p><p> Adobe Workfront</li></p>
   <li><p>For the current Workfront plans: </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront Scenario Planner</p></li></ul>
   
   <p>For more information, see <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level </td> 
   <td> <p>[!UICONTROL Edit] access to the [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p>[!UICONTROL Manage] permissions to a plan</p> <p>For information on requesting additional access to a plan, see <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Request access to a plan in the [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 刪除計劃

>[!IMPORTANT]
>
>您無法復原已刪除的計畫。

您可以刪除計畫，也可以刪除計畫中的一個情境。

* [刪除計畫](#delete-plans)
* [刪除情境](#delete-scenarios)

### 刪除計劃

>[!IMPORTANT]
>
>刪除計畫時，請考量下列事項：
>
>* 也會刪除與計畫相關的所有資訊。 其中包括與計畫相關的所有案例與方案，包括職位角色與成本的資訊。 此資訊無法復原。
>* 如果計畫包含已發佈的案例，則會保留連結至已刪除方案的專案，且[!DNL Scenario Planner]區域仍保留在[!UICONTROL 專案詳細資料]區段中。
>
>  如需將方案發佈至專案的資訊，請參閱[在 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)中發佈方案以更新或建立專案。

若要刪除計畫，請執行下列步驟：

{{step1-to-scenario-planner}}

計劃清單隨即顯示。

1. 按一下計畫名稱以開啟。
1. 按一下計畫名稱右側的&#x200B;**[!UICONTROL 更多功能表]** ![更多功能表](assets/more-menu.png)，然後按一下&#x200B;**[!UICONTROL 刪除]** > **[!UICONTROL 是，刪除]**。

   計畫即被刪除，您將返回計劃清單。

### 刪除情境 {#delete-scenarios}

>[!IMPORTANT]
>
>刪除案例時，請考量下列事項：
>
>* 刪除情境將會從此情境中刪除所有行動方案及其資訊。 如果方案被複製到其他情境，則會保留在其他情境中。
>* 刪除案例時，後續案例會採用已刪除案例的數量，並保留計數順序。 例如，如果您刪除案例4，案例5會變成案例4。
>* 如果案例上的某些方案已發佈，則會保留連結至方案的專案，且「案例規劃工具」區域會保留在連結的專案上
>* 如果發佈的行動方案存在於另一個情境中，則會停留在該情境中，包括其至專案的連結。 從其他情境發佈這些方案，會以來自這些情境的新資訊更新連結的專案。
>
>  如需將方案發佈至專案的資訊，請參閱[在 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)中發佈方案以更新或建立專案。

若要刪除案例，請執行下列動作：

1. 移至您要刪除情境的計畫。

   依預設，會顯示初始案例。

1. 按一下&#x200B;**[!UICONTROL 比較案例]**。
1. 從情境卡的右上角，按一下&#x200B;**[!UICONTROL 更多]**&#x200B;功能表![更多](assets/more-menu.png)，然後按一下&#x200B;**[!UICONTROL 刪除]**。

   情境已刪除。

1. 按一下&#x200B;**[!UICONTROL 儲存計畫]**&#x200B;以儲存變更。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Delete initiatives</h2>
<p>(NOTE: moved this section to its own article about deleting initiatives) </p> <note type="important">
<p>Consider the following when deleting initiatives:</p>
<ul>
<li>Deleting an initiative deletes the job roles and cost information from the initiative.</li>
<li><span>When you delete an initiative that is published to a project, the initiative is removed from the scenario but the Scenario Planner area remains in the Project Details section.</span> </li>
<li> <p>If the initiative you delete is the only published initiative on the scenario, the indicator that the plan has been published is also removed. </p> <p>For information about publishing initiatives to projects, see <a href="../scenario-planner/publish-scenarios-update-projects.md" class="MCXref xref">Update or create projects by publishing initiatives in the Scenario Planner</a>.</p> </li>
</ul>
</note>
<p>To delete an initiative:</p>
<ol>
<li value="1"> <p> <p>Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png">, then click Scenarios.</p> </p> <p>A list of plans displays. </p> </li>
<li value="2">Click the name of a plan to open it, then locate the initiative you want to delete.</li>
<li value="3"> <p>Click the <strong>More menu</strong> <img src="assets/more-menu.png"> to the right of the initiative name, then click <strong>Delete</strong> > <strong>Yes, delete it</strong>. </p> <p>The initiative is deleted. </p> </li>
<li value="4">Click <strong>Save Plan</strong> to save your changes. </li>
</ol>
</div>
-->


