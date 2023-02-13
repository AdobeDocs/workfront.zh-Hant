---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 更新方案計畫器中的方案優先順序
description: 排定計畫的優先順序非常重要，因為計畫按計畫上列出的順序接收計畫中的職務和預算資源。
author: Alina
feature: Workfront Scenario Planner
exl-id: 45f019de-b29c-477b-8bd1-f32ef21c1015
source-git-commit: e152c20e7b987f4bef7ffd6ee534c059f7b9bf45
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 0%

---

# 更新 [!DNL Scenario Planner]

排定計畫的優先順序非常重要，因為計畫按計畫上列出的順序接收計畫中的職務和預算資源。

您可以根據您建立的計畫或某人與您共用的計畫來排定方案優先順序。

如需建立計畫的相關資訊，請參閱 [在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

有關建立方案的資訊，請參閱 [在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

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
   <td> <p>您必須為 [!DNL Adobe Workfront Scenario Planner] 存取本文所述功能。</p> <p>如需有關取得 [!DNL Workfront Scenario Planner]，請參閱 <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">使用 [!DNL Scenario Planner]</a>. </p> </td> 
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

## 更新計畫優先事項

當更改方案的優先順序時，您將修改其計畫的清單順序。

我們建議您將更緊迫的計畫放在計畫的最上方，將更流動的計畫放在計畫的最下方 — 這些計畫可以隨時執行，而且只有在有資源的情況下才能執行。

>[!NOTE]
>
>[!DNL Workfront] 按計畫上列出的順序將計畫資源分配給計畫。
>
>例如，如果計畫中有3個可用工程師和計畫1和計畫2，每個都需要2個工程師完成，並且兩個工程師都計畫在同一時間範圍內，則Workfront將2個工程師與計畫1關聯，將1個剩餘的可用工程師與計畫2關聯。 在這種情況下，計畫2顯示存在衝突，因為它缺少一個工程師。 有時，更改計畫的優先順序是避免計畫衝突的唯一方法。

要更新方案優先順序，請執行以下操作：

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png)，然後按一下 [!UICONTROL 藍本].

   計劃清單隨即顯示。

1. 按一下計畫的名稱以開啟它，然後找出要排定優先順序的方案。
1. 按一下一個或多個方案名稱左側的框，然後執行以下操作之一：

   * 按一下選定方案名稱左側的句柄，然後將其向上或向下拖動到清單中，以更改方案的優先順序。

      Workfront會顯示選取的方案數量。

      ![](assets/multi-select-initiative-number.png)

   * 按一下 **[!UICONTROL 優先順序]** 框，然後從以下選項中選擇：

      * **[!UICONTROL 頂端]**:將所選方案移到方案清單的頂部。 選定的方案將首先列在計畫上。
      * **[!UICONTROL 底部]**:將所選方案移到方案清單的底部。 所選方案將列在計畫的最後。
      * **[!UICONTROL 選擇數字]**:在您在此處指定的計畫之後移動所選計畫。

         ![](assets/prioritize-initiatives-expanded-highlighted-350x171.png)
      [!DNL Workfront] 立即將選定的方案置於您指示的位置，並相應更新所有方案的數量。


1. 按一下 **[!UICONTROL 保存計畫]** 來儲存變更。
