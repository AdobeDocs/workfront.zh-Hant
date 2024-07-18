---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 更新「情境規劃工具」中的方案優先順序
description: 優先處理方案非常重要，因為方案會依照其在計畫上的列出順序，從計畫接收職務角色和預算資源。
author: Alina
feature: Workfront Scenario Planner
exl-id: 45f019de-b29c-477b-8bd1-f32ef21c1015
source-git-commit: e152c20e7b987f4bef7ffd6ee534c059f7b9bf45
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# 更新[!DNL Scenario Planner]中的方案優先順序

優先處理方案非常重要，因為方案會依照其在計畫上的列出順序，從計畫接收職務角色和預算資源。

您可以優先處理您建立之計畫或他人與您共用的計畫上的方案。

如需有關建立計畫的資訊，請參閱[在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md)中建立和編輯計畫。

如需關於建立方案的資訊，請參閱[在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md)中建立和編輯方案。

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
   <td> <p>您必須為[!DNL Adobe Workfront Scenario Planner]購買額外的授權，才能存取本文所述的功能。</p> <p>如需有關取得[!DNL Workfront Scenario Planner]的資訊，請參閱<a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">使用[!DNL Scenario Planner]</a>所需的存取權。 </p> </td> 
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

## 更新方案優先順序

當您變更方案的優先順序時，即會修改它們在計畫中的清單順序。

我們建議您將更緊急的倡議放在計畫的頂端，而更流暢的倡議（只有在資源可用的情況下才能完成）放在計畫的底部。

>[!NOTE]
>
>[!DNL Workfront]會依照方案在計畫上的列出順序，將計畫資源配置給方案。
>
>例如，如果計畫有3個可用的工程師和方案1和方案2，每個都需要2個工程師來完成，且兩個工程師都排程在相同的時間範圍內，Workfront會將2個工程師與方案1建立關聯，並將剩下一個可用的工程師與方案2建立關聯。 在此案例中，方案2會顯示為發生衝突，因為它缺少一位工程師。 有時候，變更方案的優先順序是避免計畫衝突的唯一方法。

若要更新方案優先順序：

1. 按一下&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下[!UICONTROL 案例]。

   計劃清單隨即顯示。

1. 按一下計畫的名稱以開啟，然後找到您要排定優先順序的方案。
1. 按一下一或多個方案名稱左側的方塊，然後執行下列任一項作業：

   * 按一下其中一個所選方案名稱左側的控點，然後在清單中將其向上或向下拖曳以變更方案的優先順序。

     Workfront會顯示所選方案的數量。

     ![](assets/multi-select-initiative-number.png)

   * 按一下計畫底部的&#x200B;**[!UICONTROL 優先順序]**&#x200B;方塊，然後選擇下列選項：

      * **[!UICONTROL 前]**：將選取的方案移至方案清單的頂端。 選取的方案會先列在計畫上。
      * **[!UICONTROL 底部]**：將選取的方案移至方案清單底部。 選取的方案會列在計畫的最後。
      * **[!UICONTROL 選取數字]**：將選取的方案移至您在此指定的方案之後。

        ![](assets/prioritize-initiatives-expanded-highlighted-350x171.png)

     [!DNL Workfront]會立即放置您指定的所選方案，且所有方案的數量會據此更新。

1. 按一下&#x200B;**[!UICONTROL 儲存計畫]**&#x200B;以儲存變更。
