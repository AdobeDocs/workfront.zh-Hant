---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 刪除「情境規劃工具」中的計畫
description: 您可以刪除您建立的計畫。 您無法刪除與您共用的計畫。
author: Alina
feature: Workfront Scenario Planner
exl-id: 74515723-3822-425a-aa9e-970af63f9189
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 0%

---

# 刪除[!DNL Scenario Planner]中的計畫

您可以刪除您建立的計畫。 您無法刪除與您共用的計畫。

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b>計畫*</b> </p> </td> 
   <td>[！UICONTROL Business]或更高版本</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b>授權*</b> </p> </td> 
   <td> <p>[！UICONTROL Review]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td><b>產品</b> </td> 
   <td> <p>您必須為[!DNL Adobe Workfront Scenario Planner]購買額外的授權，才能存取本文所述的功能。</p> <p>如需有關取得[!DNL Workfront Scenario Planner]的資訊，請參閱<a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">使用[!DNL Scenario Planner]</a>所需的存取權。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>存取層級設定*</strong> </td> 
   <td> <p>[！UICONTROL Edit]或以上版本的 [!DNL Scenario Planner]</p> <p>注意：如果您還是沒有存取權，請詢問您的[!DNL Workfront]管理員是否對您的存取層級設定了其他限制。 如需Workfront管理員如何變更存取層級的詳細資訊，請參閱<a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>物件許可權</strong> </p> </td> 
   <td> <p>[！UICONTROL Manage]計畫的許可權</p> <p>如需有關請求對計畫的額外存取權的資訊，請參閱<a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">在[!DNL Scenario Planner]</a>中請求對計畫的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

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

1. 按一下&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下[!UICONTROL 案例]。

   計劃清單隨即顯示。

1. 按一下計畫名稱以開啟。
1. 按一下計畫名稱右側的&#x200B;**[!UICONTROL 更多功能表]** ![](assets/more-menu.png)，然後按一下&#x200B;**[!UICONTROL 刪除]** > **[!UICONTROL 是，刪除它]**。

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
1. 從情境卡的右上角，按一下&#x200B;**[!UICONTROL 更多]**&#x200B;功能表![](assets/more-menu.png)，然後按一下&#x200B;**[!UICONTROL 刪除]**。

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


