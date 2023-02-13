---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 在方案計畫器中複製方案
description: 您可以複製現有的方案來建立方案。 您可以複製您建立的計畫或某人與您共用的計畫的方案。
author: Alina
feature: Workfront Scenario Planner
exl-id: 0aadb074-69c3-4229-a01a-7cabdb87e7cb
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 1%

---

# 複製 [!DNL Scenario Planner]

您可以複製現有的方案來建立方案。 您可以複製您建立的計畫或某人與您共用的計畫的方案。

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
   <td> <p>[!DNL Adobe Workfront]<b> 授權</b>*</p> </td> 
   <td> <p>[!UICONTROL Review]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td><b>產品</b> </td> 
   <td> <p>您必須為 [!DNL Adobe Workfront Scenario Planner] 存取本文所述功能。</p> <p>如需有關取得 [!DNL Workfront Scenario Planner]，請參閱 <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">使用 [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>訪問級別配置*</strong> </td> 
   <td> <p>[!UICONTROL Edit]或更高版本 [!DNL Scenario Planner]</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 若要了解 [!DNL Workfront] 管理員可以更改您的訪問級別，請參閱 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>物件權限</strong> </p> </td> 
   <td> <p>計畫的[!UICONTROL管理]權限</p> <p>有關請求對計畫進行額外訪問的資訊，請參閱 <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">在 [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 複製計畫

複製計畫時，請考量下列事項：

* 複製方案會將副本置於與原始方案相同的計畫上。
* 複製計畫副本並將以下資訊從原始計畫添加到新計畫：

   * [!UICONTROL 期間]
   * [!UICONTROL 工作角色]
   * [!UICONTROL 人員] 和 [!UICONTROL 固定成本]
   * [!UICONTROL 計畫收益]

* 如果原始方案上存在資訊，複製方案可以修改計畫的以下資訊：

   * 所需數量的作業角色
   * [!UICONTROL 成本]
   * [!UICONTROL 計畫利用率]
   * 作業角色利用率
   * [!UICONTROL 淨值]

* 複製通過導入項目而建立或已至少發佈到項目一次的方案具有以下含義：

   * 它不會複製與方案相關聯的專案。
   * 它不會將複製的方案連接到項目。
   * 不會修改 [!DNL Scenario Planner] 區段，針對已至少發佈一次的專案。

   如需將方案發佈至專案的相關資訊，請參閱 [更新或建立專案，方法是在 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

   有關通過導入項目來建立方案的資訊，請參閱 [將專案匯入至 [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md) .

## 複製計畫

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png)，然後按一下 [!UICONTROL 藍本].

   計劃清單隨即顯示。

1. 按一下計畫的名稱以開啟它，然後找到要複製的方案。
1. 選擇要複製的方案或方案左側的框，然後按一下 **[!UICONTROL 複製]** 從顯示在計畫底部的菜單中。

   ![](assets/bottom-manage-initiative-menu-350x45.png)

   [!DNL Workfront] 立即複製計畫，並將其置於最後選定計畫的下面。

   複製的方案的名稱為 *[!UICONTROL 副本]`<Name of original initiative>`*.

   >[!NOTE]
   >
   >根據您插入新方案的位置，現有方案的數量可能會改變。

1. 更新複製的方案的名稱。

   >[!TIP]
   >
   >建議您一律更新方案名稱，以避免在您想要再次複製時產生混淆。

1. （可選）更新新建立的方案的優先順序。

   有關排定計畫優先順序的資訊，請參見 [更新 [!DNL Scenario Planner]](../scenario-planner/prioritize-initiatives.md).

1. 按一下 **[!UICONTROL 保存計畫]** 來儲存變更。
