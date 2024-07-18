---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 刪除Scenario Planner中的方案
description: 您可以刪除您建立之計畫上的方案，或他人與您共用的計畫上的方案。 您無法復原已刪除的方案。
author: Alina
feature: Workfront Scenario Planner
exl-id: 799ca02e-c513-4409-b327-1ce7d8eb19ae
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '529'
ht-degree: 0%

---

# 刪除[!DNL Scenario Planner]中的方案

您可以刪除您建立之計畫上的方案，或他人與您共用的計畫上的方案。 您無法復原已刪除的方案。

## 存取需求

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
   <td> <p>您必須為[!DNL Adobe Workfront Scenario Planner]購買額外的授權，才能存取本文所述的功能。 </p> <p>如需有關取得[!DNL Workfront Scenario Planner]的資訊，請參閱<a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">使用[！UICONTROL Scenario Planner]所需的存取權</a>。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>存取層級設定*</strong> </td> 
   <td> <p>[！UICONTROL Edit]或以上版本的 [!DNL Scenario Planner]</p> <p>注意：如果您還是沒有存取權，請詢問您的[!DNL Workfront]管理員是否對您的存取層級設定了其他限制。 如需[!DNL Workfront]管理員如何變更您的存取層級的詳細資訊，請參閱<a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>物件許可權</strong> </p> </td> 
   <td> <p>[！UICONTROL Manage]計畫的許可權</p> <p>如需有關請求對計畫的額外存取權的資訊，請參閱<a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">在[!DNL Scenario Planner]</a>中請求對計畫的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

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

1. 按一下&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下[!UICONTROL 案例]。

   計劃清單隨即顯示。

1. 按一下計畫的名稱以開啟計畫，然後找到您要刪除的方案。
1. 執行下列其中一項：

   * 按一下方案名稱右側的&#x200B;**[!UICONTROL 更多功能表]** ![](assets/more-menu.png)，然後按一下&#x200B;**[!UICONTROL 刪除]** > **[!UICONTROL 是，刪除它]**。

   * 選取方案左側的方塊，然後按一下出現在計畫底部的浮動功能表上的&#x200B;**[!UICONTROL 刪除]**，然後按一下&#x200B;**[!UICONTROL 是，刪除它]**。

   方案及其工作角色與成本資訊會從計畫中刪除。

1. 按一下&#x200B;**[!UICONTROL 儲存計畫]**&#x200B;以儲存變更。

### 大量刪除方案 {#delete-initiatives-in-bulk}

1. 按一下&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下[!UICONTROL 案例]。

   計劃清單隨即顯示。

1. 按一下計畫的名稱以開啟計畫，然後找到您要刪除的方案。
1. 選取您要刪除之方案左側的方塊，然後在計畫底部出現的功能表中按一下&#x200B;**[!UICONTROL [刪除]]**，然後按一下&#x200B;**[!UICONTROL [是，刪除]]**。

   ![](assets/bottom-manage-initiative-menu-350x45.png)

   方案及其工作角色和成本資訊會從計畫中刪除。

1. 按一下&#x200B;**[!UICONTROL 儲存計畫]**&#x200B;以儲存變更。
