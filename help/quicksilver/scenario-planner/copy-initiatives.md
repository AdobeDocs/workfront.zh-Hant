---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 在Scenario Planner中複製方案
description: 您可以複製現有方案來建立方案。 您可以複製您建立之計畫或某人員與您共用之計畫上的方案。
author: Alina
feature: Workfront Scenario Planner
exl-id: 0aadb074-69c3-4229-a01a-7cabdb87e7cb
source-git-commit: aa2e9a012a60ab10e2d027dedae520b5e06686c7
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# 複製[!DNL Scenario Planner]中的方案

<!--Audited: 07/2024-->

您可以複製現有方案來建立方案。 您可以複製您建立之計畫或某人員與您共用之計畫上的方案。

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

## 複製方案

複製行動方案時，請考量下列事項：

* 複製方案會將副本放置在與原始方案相同的計畫上。
* 複製方案會將下列資訊從原始方案複製並新增至新方案：

   * [!UICONTROL 期間]
   * [!UICONTROL 職位角色]
   * [!UICONTROL 人員]和[!UICONTROL 固定成本]
   * [!UICONTROL 計畫收益]

* 如果原始方案中存在下列資訊，則複製方案可修改計畫的下列資訊：

   * 所需的工作角色數量
   * [!UICONTROL 成本]
   * [!UICONTROL 計畫使用率]
   * 工作角色使用率
   * [!UICONTROL 淨值]

* 複製透過匯入專案建立或已發佈至專案至少一次的方案具有下列含義：

   * 不會複製與方案相關聯的專案。
   * 它不會將複製的方案連線到專案。
   * 對於已發佈至少一次的專案，它不會修改專案上的[!DNL Scenario Planner]區段。

  如需將方案發佈至專案的資訊，請參閱[在 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)中發佈方案以更新或建立專案。

  如需透過匯入專案來建立方案的相關資訊，請參閱[將專案匯入 [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md)中的計畫。

## 複製方案

{{step1-to-scenario-planner}}

計劃清單隨即顯示。

1. 按一下計畫的名稱以開啟，然後找到您要複製的方案。
1. 選取您要複製的一或多個方案左側的方塊，然後在計畫底部出現的功能表中按一下&#x200B;**[!UICONTROL 複製]**。

   ![複製方案](assets/bottom-manage-initiative-menu-350x45.png)

   [!DNL Workfront]會立即複製行動方案，並將其放置在最後一個選取的行動方案下。

   所複製方案的名稱是&#x200B;*的`<Name of original initiative>`*&#x200B;副本。

   >[!NOTE]
   >
   >根據您插入新方案的位置，現有方案的數量可能會變更。

1. 更新所複製方案的名稱。

   >[!TIP]
   >
   >建議您一律更新行動方案的名稱，以免再次複製行動方案時產生混淆。

1. （選用）更新新建立方案的優先順序。

   如需排定方案優先順序的資訊，請參閱[更新 [!DNL Scenario Planner]](../scenario-planner/prioritize-initiatives.md)中的方案優先順序。

1. 按一下&#x200B;**[!UICONTROL 儲存計畫]**&#x200B;以儲存變更。
