---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 刪除Scenario Planner中的方案
description: 您可以刪除您建立之計畫上的方案，或他人與您共用的計畫上的方案。 您無法復原已刪除的方案。
author: Alina
feature: Workfront Scenario Planner
exl-id: 799ca02e-c513-4409-b327-1ce7d8eb19ae
source-git-commit: a79e4146ce6d076ef0e3707416a9c21d643b96e1
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 2%

---

# 刪除[!DNL Scenario Planner]中的方案

您可以刪除您建立之計畫上的方案，或他人與您共用的計畫上的方案。 您無法復原已刪除的方案。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 計畫*</p> </td> 
   <td> <ul></li>
   <li><p>新增：Ultimate </p></li>
   <p>新的Workfront Select或Workfront計畫無法使用「情境規劃工具」。 </p>
   <li><p>目前： [！UICONTROL Business]或更高版本</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 授權*</p> </td> 
   <td> <p>新增：淺色或更高</p> 
   <p>目前： [！UICONTROL Review]或以上</p> </td> 
  </tr> 
  <tr> 
   <td>產品* </td> 
   <td> <ul><li><p>針對新的Workfront計畫：</p><p> Adobe Workfront</li></p>
   <li><p>針對目前的Workfront計畫： </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront情境規劃工具</p></li></ul>

<p>如需詳細資訊，請參閱<a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">使用[!DNL Scenario Planner]</a>所需的存取權。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>存取層級 </td> 
   <td> <p>[！UICONTROL Edit]對的存取權 [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>物件許可權 </p> </td> 
   <td> <p>[！UICONTROL Manage]計畫的許可權</p> <p>如需有關請求對計畫的額外存取權的資訊，請參閱<a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">在[!DNL Scenario Planner]</a>中請求對計畫的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱[Workfront檔案的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 刪除行動方案

刪除行動方案時，請考量下列事項：

* 刪除方案會從計畫中移除所需的工作角色數量，以及與方案相關的成本資訊。
* 刪除透過匯入專案建立的方案並不會刪除與該方案相關聯的專案。
* 刪除已發佈至專案至少一次的方案會產生下列結果：

   * 已從情境中刪除方案，但[!DNL Scenario Planner]區域仍保留在[!UICONTROL 專案詳細資料]區段中。
   * 如果您刪除的方案是情境上唯一發佈的方案，則也會移除已發佈計畫的指標。

     如需將方案發佈至專案的資訊，請參閱[在 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)中發佈方案以更新或建立專案。

     如需透過匯入專案來建立方案的相關資訊，請參閱[在 [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md)中將專案匯入計畫。

您可以一次刪除一個行動方案，也可以大量刪除多個行動方案。

* [刪除一個行動方案](#delete-one-initiative)
* [大量刪除方案](#delete-initiatives-in-bulk)

### 刪除一個方案 {#delete-one-initiative}

{{step1-to-scenario-planner}}

計劃清單隨即顯示。

1. 按一下計畫的名稱以開啟計畫，然後找到您要刪除的方案。
1. 執行下列其中一項：

   * 按一下方案名稱右側的&#x200B;**[!UICONTROL 更多功能表]** ![](assets/more-menu.png)，然後按一下&#x200B;**[!UICONTROL 刪除]** > **[!UICONTROL 是，刪除它]**。

   * 選取方案左側的方塊，然後按一下出現在計畫底部的浮動功能表上的&#x200B;**[!UICONTROL 刪除]**，然後按一下&#x200B;**[!UICONTROL 是，刪除它]**。

   方案及其工作角色與成本資訊會從計畫中刪除。

1. 按一下&#x200B;**[!UICONTROL 儲存計畫]**&#x200B;以儲存變更。

### 大量刪除方案 {#delete-initiatives-in-bulk}

{{step1-to-scenario-planner}}

計劃清單隨即顯示。

1. 按一下計畫的名稱以開啟計畫，然後找到您要刪除的方案。
1. 選取您要刪除之方案左側的方塊，然後在計畫底部出現的功能表中按一下&#x200B;**[!UICONTROL [刪除]]**，然後按一下&#x200B;**[!UICONTROL [是，刪除]]**。

   ![](assets/bottom-manage-initiative-menu-350x45.png)

   方案及其工作角色和成本資訊會從計畫中刪除。

1. 按一下&#x200B;**[!UICONTROL 儲存計畫]**&#x200B;以儲存變更。
