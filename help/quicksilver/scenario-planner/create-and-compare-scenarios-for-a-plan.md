---
product-previous: enterprise-scenario-planner
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 在「案例規劃工具」中建立並比較計畫案例
description: 當您規劃公司的長期策略時，一開始您可能沒有或想過很多資訊。 需要時間和實驗才能得出利害關係人可以接受的最終策略。 進行「假設」分析，為您的計畫建立多個情境，可協助您準確預測及評估潛在的情況，並最終制定最佳的計畫。
author: Alina
feature: Workfront Scenario Planner
exl-id: 9a79ef81-6271-4cc9-b701-3ba0aeafb324
source-git-commit: aa2e9a012a60ab10e2d027dedae520b5e06686c7
workflow-type: tm+mt
source-wordcount: '931'
ht-degree: 1%

---

# 在[!DNL Scenario Planner]中建立和比較計畫案例

<!--Audited: 07/2024-->

當您規劃公司的長期策略時，一開始您可能沒有或想過很多資訊。 需要時間和實驗才能得出利害關係人可以接受的最終策略。 進行「假設」分析，為您的計畫建立多個情境，可協助您準確預測及評估潛在的情況，並最終制定最佳的計畫。

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
   <td> <p>[！UICONTROL Light]或更高</p> 
   <p>[！UICONTROL Review]或更高版本</p> </td> 
  </tr> 
    <tr> 
   <td>存取層級設定</td> 
   <td> <p>[！UICONTROL Edit]對的存取權 [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr> 
   <td> <p>物件許可權 </p> </td> 
   <td> <p>[！UICONTROL Manage]計畫的許可權</p> </td> 
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

## 建立案例

案例是計畫的復本。 您可以建立所需數量的情境。 不過，我們建議您儘可能減少情境的數量，以便輕鬆比較。

{{step1-to-scenario-planner}}

1. 建立計畫或按一下現有計畫的名稱。

   如需有關建立計畫的資訊，請參閱[在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md)中建立和編輯計畫。

   您建立的第一個計畫會自動儲存為&quot;[!UICONTROL 初始情境]&quot;。

1. 按一下現有情境旁邊的向下箭頭，然後按一下「**[!UICONTROL 複製]**」圖示。

   ![複製案例](assets/copy-scenarios-ui-and-highlighted-icon-350x95.png)

   這會建立一個新情境，其資訊與複製的情境相同。 如果它是計畫的第二個案例，則會自動命名為「[!UICONTROL 案例2]」；如果它是第三個案例，則會自動命名為「[!UICONTROL 案例3]」，以此類推。 您無法重新命名情境。 您可以建立的復本數目沒有限制。

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE:this might change)
   </MadCap:conditionalText>
   -->

1. 請透過下列任一方式更新您的新情境：

   * 建立、更新或刪除方案

     >[!TIP]
     >
     >當您刪除案例中的方案時，它只會從選取的案例中移除，而不會從所有案例中移除。

     如需關於建立方案的資訊，請參閱[在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md)中建立和編輯方案。

   * 更新方案的優先順序
   * 調整人員或預算資訊
   * 檢閱並調整情境中的方案衝突

     如需解決衝突的資訊，請參閱[解決 [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md)中的方案衝突。

1. 按一下&#x200B;**[!UICONTROL 儲存計畫]**&#x200B;以儲存變更。

## 比較情境

建立情境後，您可以加以比較，找出最適合貴組織的情境。

1. 移至您要比較案例的計畫。
1. 按一下&#x200B;**[!UICONTROL 比較案例]**。 案例比較頁面隨即顯示。

   計畫的所有現有情境都會以並排卡片格式顯示。 初始情境一律先列出，且為靜態。

   ![感應卡](assets/scenario-cards-overlapping-350x166.png)

1. （選用）向右捲動以檢視所有案例卡。

   情境卡上會顯示下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>情境的名稱</td> 
      <td> <p>Workfront自動產生的名稱，無法編輯。 例如，「[！UICONTROL初始情境]」、「[！UICONTROL情境2]」等。 </p> </td> 
     </tr> 
     <tr> 
      <td>案例說明</td> 
      <td>手動輸入專案，您可在此說明情境的詳細資訊。 </td> 
     </tr> 
     <tr> 
      <td>可用的職位角色</td> 
      <td>在計畫期間可從計畫預算取得的工作角色數量。 </td> 
     </tr> 
     <tr> 
      <td>必要職位角色</td> 
      <td>所需的職務角色數量（根據您的方案）。 </td> 
     </tr> 
     <tr> 
      <td>預算</td> 
      <td>在此案例中為計畫定義的預算總計。 如需計畫的預算資訊，請參閱<a href="../scenario-planner/plans-overview.md" class="MCXref xref">中的[!DNL Scenario Planner]</a>計畫總覽。 </td> 
     </tr> 
     <tr> 
      <td>成本</td> 
      <td>與案例上的方案相關聯的成本。 如需有關成本的資訊，請參閱<a href="../scenario-planner/initiatives-overview.md" class="MCXref xref">中的[!DNL Scenario Planner]</a>方案概觀。 </td> 
     </tr> 
     <tr> 
      <td>使用情況</td> 
      <td>此情境中計畫的[！UICONTROL預算使用率]百分比。 如需[！UICONTROL預算使用率]百分比的相關資訊，請參閱<a href="../scenario-planner/plans-overview.md" class="MCXref xref">中的[!DNL Scenario Planner]</a>計畫總覽。 </td> 
     </tr> 
     <tr> 
      <td>淨值</td> 
      <td>此情境中計畫的[！UICONTROL淨值]。 如需有關計畫的[！UICONTROL淨值]的資訊，請參閱<a href="../scenario-planner/plans-overview.md" class="MCXref xref">中的[!DNL Scenario Planner]</a>計畫總覽。 </td> 
     </tr> 
     <tr> 
      <td>方案</td> 
      <td>此情境中計畫的方案數。</td> 
     </tr> 
     <tr> 
      <td>衝突</td> 
      <td>在此情境的計畫中顯示任何衝突型別的方案數目。 如需方案衝突的資訊，請參閱<a href="../scenario-planner/resolve-conflicts-in-sp.md" class="MCXref xref">解決[!DNL Scenario Planner]</a>中的方案衝突。 </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >當初始案例與其他案例之間的資訊不同時，在變更的值旁邊會顯示向上或向下箭頭，以表示該值比初始案例增加或減少。
   >
   >
   >情景卡片上的![箭頭](assets/arrows-on-scenario-cards-highlighted-350x70.png)
   >
   >例如，預算、工作角色數量、行動方案數量可能會從一個情境變更為另一個情境。

1. 按一下情境的名稱以存取並進行變更。

   如需詳細資訊，請參閱本文中的[建立案例](#create-scenarios)一節。

1. 按一下&#x200B;**[!UICONTROL 新增說明]**&#x200B;以新增情境的說明

   或

   按一下說明欄位進行更新，然後按一下畫面上的任何位置以儲存變更。

1. （選擇性）按一下&#x200B;**[!UICONTROL 更多]**&#x200B;功能表![更多圖示](assets/more-icon.png)以&#x200B;**[!UICONTROL 複製]**&#x200B;或&#x200B;**[!UICONTROL 刪除]**&#x200B;情境。

   ![複製或刪除情境](assets/copy-or-delete-scenario-links-from-card-350x109.png)

   當您複製案例時，它會自動出現在卡片頁面上，並會根據以下模式重新命名：「[!UICONTROL 案例] `<next number in order>`」。

1. （視條件而定）如果您按一下&#x200B;**[!UICONTROL 刪除]**，請按一下&#x200B;**[!UICONTROL 是，刪除]**&#x200B;以進行確認。

   已刪除的案例無法復原。

   如需有關刪除情境的資訊，請參閱[刪除 [!DNL Scenario Planner]](../scenario-planner/delete-plans.md)中的計畫。

1. 按一下&#x200B;**[!UICONTROL 儲存計畫]**&#x200B;以儲存您的案例與計畫。
