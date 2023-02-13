---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 刪除方案計畫器中的方案
description: 您可以刪除您建立的計畫或某人與您共用的計畫的方案。 您無法恢復已刪除的方案。
author: Alina
feature: Workfront Scenario Planner
exl-id: 799ca02e-c513-4409-b327-1ce7d8eb19ae
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '529'
ht-degree: 1%

---

# 刪除 [!DNL Scenario Planner]

您可以刪除您建立的計畫或某人與您共用的計畫的方案。 您無法恢復已刪除的方案。

## 存取需求

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
   <td> <p>您必須為 [!DNL Adobe Workfront Scenario Planner] 存取本文所述功能。 </p> <p>如需有關取得 [!DNL Workfront Scenario Planner]，請參閱 <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">使用[!UICONTROL方案規劃器]所需的訪問權</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>訪問級別配置*</strong> </td> 
   <td> <p>[!UICONTROL Edit]或更高版本 [!DNL Scenario Planner]</p> <p>注意：如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可以更改您的訪問級別，請參閱 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>物件權限</strong> </p> </td> 
   <td> <p>計畫的[!UICONTROL管理]權限</p> <p>有關請求對計畫進行額外訪問的資訊，請參閱 <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">在 [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 刪除方案

刪除方案時，請考慮下列事項：

* 刪除方案會從計畫中刪除與方案關聯的任務職責和成本資訊的所需金額。
* 刪除通過導入項目建立的方案不會刪除與方案關聯的項目。
* 刪除已至少發佈到項目一次的方案將產生以下結果：

   * 方案會從中刪除，但 [!DNL Scenario Planner] 區域仍保留在 [!UICONTROL 專案詳細資料] 區段。
   * 如果您刪除的方案是方案中唯一已發佈的方案，則也會刪除已發佈計畫的指標。

      如需將方案發佈至專案的相關資訊，請參閱 [更新或建立專案，方法是在 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

      有關通過導入項目來建立方案的資訊，請參閱 [將專案匯入至 [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md) .

您可以一次刪除一個方案，也可以大量刪除多個方案。

* [刪除一個方案](#delete-one-initiative)
* [大量刪除方案](#delete-initiatives-in-bulk)

### 刪除一個方案 {#delete-one-initiative}

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png)，然後按一下 [!UICONTROL 藍本].

   計劃清單隨即顯示。

1. 按一下計畫的名稱以開啟它，然後找到要刪除的計畫。
1. 執行下列任一項作業：

   * 按一下 **[!UICONTROL 更多功能表]** ![](assets/more-menu.png) 在方案名稱的右側，然後按一下 **[!UICONTROL 刪除]** > **[!UICONTROL 是，刪除它]**.

   * 選擇方案左側的框，然後按一下 **[!UICONTROL 刪除]** 在顯示於計畫底部的浮動菜單上，然後按一下 **[!UICONTROL 是，刪除它]**.

   從計畫中刪除該計畫及其工作角色和費用資訊。

1. 按一下 **[!UICONTROL 保存計畫]** 來儲存變更。

### 大量刪除方案 {#delete-initiatives-in-bulk}

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png)，然後按一下 [!UICONTROL 藍本].

   計劃清單隨即顯示。

1. 按一下計畫的名稱以開啟它，然後找到要刪除的計畫。
1. 選擇要刪除的方案左側的框，然後按一下 **[!UICONTROL 刪除]** 從顯示在計畫底部的菜單中，按一下 **[!UICONTROL 是，刪除]**.

   ![](assets/bottom-manage-initiative-menu-350x45.png)

   計畫中刪除了計畫及其工作角色和成本資訊。

1. 按一下 **[!UICONTROL 保存計畫]** 來儲存變更。
