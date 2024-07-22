---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 更新「情境規劃工具」中的方案優先順序
description: 優先處理方案非常重要，因為方案會依照其在計畫上的列出順序，從計畫接收職務角色和預算資源。
author: Alina
feature: Workfront Scenario Planner
exl-id: 45f019de-b29c-477b-8bd1-f32ef21c1015
source-git-commit: 2ff32ba11f9ef214f16b11323386223792b0877e
workflow-type: tm+mt
source-wordcount: '531'
ht-degree: 0%

---

# 更新[!DNL Scenario Planner]中的方案優先順序

優先處理方案非常重要，因為方案會依照其在計畫上的列出順序，從計畫接收職務角色和預算資源。

您可以優先處理您建立之計畫或他人與您共用的計畫上的方案。

如需有關建立計畫的資訊，請參閱[在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md)中建立和編輯計畫。

如需關於建立方案的資訊，請參閱[在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md)中建立和編輯方案。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 計畫*</p> </td> 
   <td> <p>目前： [！UICONTROL Business]或更高版本</p>
   <p>新增：Ultimate </p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 授權*</p> </td> 
   <td> <p>新增：淺色或更高</p> 
   <p>目前： [！UICONTROL Review]或以上</p> </td> 
  </tr> 
  <tr> 
   <td>產品* </td> 
   <td> 
   <p>針對目前的Workfront計畫： </p>
   <p>您必須為[!DNL Adobe Workfront Scenario Planner]購買額外的授權，才能存取本文所述的功能。</p> <p>如需[!DNL Workfront Scenario Planner]的存取與許可權相關資訊，請參閱<a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">使用[!DNL Scenario Planner]</a>所需的存取權。 </p> </td> 
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

## 更新方案優先順序

當您變更方案的優先順序時，即會修改它們在計畫中的清單順序。

我們建議您將更緊急的倡議放在計畫的頂端，而更流暢的倡議（只有在資源可用的情況下才能完成）放在計畫的底部。

>[!NOTE]
>
>[!DNL Workfront]會依照方案在計畫上的列出順序，將計畫資源配置給方案。
>
>例如，如果計畫有3個可用的工程師和方案1和方案2，每個都需要2個工程師來完成，且兩個工程師都排程在相同的時間範圍內，Workfront會將2個工程師與方案1建立關聯，並將剩下一個可用的工程師與方案2建立關聯。 在此案例中，方案2會顯示為發生衝突，因為它缺少一位工程師。 有時候，變更方案的優先順序是避免計畫衝突的唯一方法。

若要更新方案優先順序：

{{step1-to-scenario-planner}}

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
