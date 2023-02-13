---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 刪除方案計畫員中的計畫
description: 您可以刪除您建立的計畫。 您無法刪除與您共用的計畫。
author: Alina
feature: Workfront Scenario Planner
exl-id: 74515723-3822-425a-aa9e-970af63f9189
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 1%

---

# 刪除 [!DNL Scenario Planner]

您可以刪除您建立的計畫。 您無法刪除與您共用的計畫。

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> 計劃*</b> </p> </td> 
   <td>[!UICONTROL Business]或更高版本</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> 授權*</b> </p> </td> 
   <td> <p>[!UICONTROL Review]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td><b>產品</b> </td> 
   <td> <p>您必須為 [!DNL Adobe Workfront Scenario Planner] 存取本文所述功能。</p> <p>如需有關取得 [!DNL Workfront Scenario Planner]，請參閱 <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">使用 [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>訪問級別配置*</strong> </td> 
   <td> <p>[!UICONTROL Edit]或更高版本 [!DNL Scenario Planner]</p> <p>注意：如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>物件權限</strong> </p> </td> 
   <td> <p>計畫的[!UICONTROL管理]權限</p> <p>有關請求對計畫進行額外訪問的資訊，請參閱 <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">在 [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 刪除計劃

>[!IMPORTANT]
>
>您無法恢復已刪除的計畫。

您可以刪除計畫，也可以刪除計畫中的一個方案。

* [刪除計劃](#delete-plans)
* [刪除方案](#delete-scenarios)

### 刪除計劃

>[!IMPORTANT]
>
>刪除計畫時，請考量下列事項：
>
>* 也會刪除與計畫相關的所有資訊。 這包括與計畫相關聯的所有方案和計畫，包括有關職務和成本的資訊。 無法恢復此資訊。
>* 如果計畫包含已發佈的方案，則會保留連結到已刪除方案的項目，並 [!DNL Scenario Planner] 區域仍保留在 [!UICONTROL 專案詳細資料] 區段。
>
>  如需將方案發佈至專案的相關資訊，請參閱 [更新或建立專案，方法是在 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

要刪除計畫，請執行以下操作：

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png)，然後按一下 [!UICONTROL 藍本].

   計劃清單隨即顯示。

1. 按一下計畫的名稱以開啟它。
1. 按一下 **[!UICONTROL 更多功能表]** ![](assets/more-menu.png) 在計畫名稱的右側，然後按一下 **[!UICONTROL 刪除]** > **[!UICONTROL 是，刪除它]**.

   計畫被刪除，然後您返回計劃清單。

### 刪除方案 {#delete-scenarios}

>[!IMPORTANT]
>
>刪除案例時，請考量下列事項：
>
>* 刪除方案會從方案中刪除所有方案及其資訊。 如果這些方案被複製到其他方案，則方案將保留在其他方案中。
>* 刪除方案時，後續方案會採用已刪除的方案數，並保留計數順序。 例如，如果刪除方案4，則方案5變為方案4。
>* 如果發佈了方案上的某些方案，則保留與方案連結的項目，並且方案規劃器區域仍保留在連結的項目上
>* 如果已發佈的方案存在於另一個方案上，則它們仍存在於該方案上，包括其與項目的連結。 從其他方案發佈這些方案會使用這些方案的新資訊更新連結的項目。
>
>  如需將方案發佈至專案的相關資訊，請參閱 [更新或建立專案，方法是在 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

若要刪除案例：

1. 轉到要刪除方案的計畫。

   依預設，會顯示「初始」藍本。

1. 按一下 **[!UICONTROL 比較方案]**.
1. 從情境卡的右上角，按一下 **[!UICONTROL 更多]** 功能表 ![](assets/more-menu.png)，然後按一下 **[!UICONTROL 刪除]**.

   會刪除案例。

1. 按一下 **[!UICONTROL 保存計畫]** 來儲存變更。

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


