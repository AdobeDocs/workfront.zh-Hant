---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: 將子任務新增到Scrum展示板上的現有劇本
description: 建立現有內文的子任務時，請記得專案的「完成模式」設定，因為這會影響內文的更新方式。
author: Lisa
feature: Agile
exl-id: 264e66e9-94c7-4904-baad-f733d39b4791
source-git-commit: d660707dd69fab78095eed1414092a7c909ba174
workflow-type: tm+mt
source-wordcount: '610'
ht-degree: 0%

---

# 將子任務新增至[!UICONTROL Scrum]展示板上的現有劇本

建立現有內文的子任務時，請牢記以下事項：

**專案的[!UICONTROL 完成模式]設定設為[!UICONTROL 手動]：**&#x200B;時

* 將具有子任務的父本文移動到[!UICONTROL 完成]會將父本文更新為100%，並將[!UICONTROL 狀態]更新為[!UICONTROL 完成]。 子任務未更新。
* 若要更新內文的[!UICONTROL 完成百分比]，您必須從[!UICONTROL 內文]索引標籤或物件的[!UICONTROL 詳細資料]頁面進行更新。

**當專案的[!UICONTROL 完成模式]設定設為[!UICONTROL 自動]**&#x200B;時：

* 將具有子任務的父本文移動到[!UICONTROL 完成]會將父本文更新為100%，並將[!UICONTROL 狀態]更新為[!UICONTROL 完成]。 子任務也更新為100%，且[!UICONTROL 狀態]更新為[!UICONTROL 完成]。
* 若要更新內文的[!UICONTROL 完成百分比]，您必須更新任何子任務的[!UICONTROL 完成百分比]。 內文的[!UICONTROL 完成百分比]是根據所有子工作的[!UICONTROL 完成百分比]計算的。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td> <p>新增：[!UICONTROL Standard]</p> 
   或
   <p>目前： [!UICONTROL Work]或更高版本</p> </td> 
  </tr>
   <tr> 
   <td role="rowheader">物件許可權</td> 
   <td>[!UICONTROL Contribute]或[!UICONTROL Manage]子任務所在任務的存取權 </td> 
  </tr>
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 將子任務新增到Scrum展示板上的現有劇本

{{step1-to-team}}

1. （選擇性）按一下&#x200B;**[!UICONTROL 切換群組]**&#x200B;圖示![切換群組圖示](assets/switch-team-icon.png)，然後從下拉式功能表中選取新的Scrum群組或在搜尋列中搜尋群組。

1. 前往包含您要新增子任務之劇本的敏捷疊代或專案。 如需有關如何導覽至反複專案的資訊，請參閱[檢視反複專案](../../../agile/use-scrum-in-an-agile-team/iterations/view-iteration.md)。
1. 移至您想要新增子任務的劇本面板上的劇本拼貼。
1. 按一下主劇本卡片上的&#x200B;**[!UICONTROL 新增子任務]**，以建立該劇本的子任務。

   ![新增子任務](assets/agile-story-addsubtask-NWE.png)

   或

   按一下子任務圖示上的&#x200B;**[!UICONTROL 新增子任務]**，以建立子任務至子任務。

   [!DNL Workfront]支援無限層級的子任務，但敏捷故事板上只顯示兩個層級（子任務的子任務）。

   ![新增子任務](assets/agile-story-addsubtask2-NWE.png)

   將子任務新增至目前沒有泳道的內文時，父任務會提升至[!UICONTROL 父級內文]欄，而子任務會移至泳道內。

1. 指定下列資訊：

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 子任務名稱]</strong></td>
      <td> 指定子工作的名稱。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 說明]</strong></td>
      <td>指定子工作的說明。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 估計]</strong></td>
      <td>指定子任務的預估值。<br><p>建立預估時，請記得下列事項：</p>
       <ul>
        <li>如果您的敏捷團隊設定為以點為單位估計劇本，則預設的1點等於8小時。 預估會新增為內文上的[!UICONTROL 計畫時數]。</li>
        <li>所有子工作的合併估計會決定父劇本的估計值。 如需詳細資訊，請參閱<a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/update-status-of-stories-and-subtasks.md" class="MCXref xref">更新Scrum展示板上內文和子工作的狀態</a>。</li>
        <li>建立新的子任務時，[!UICONTROL 預估]欄位已設定。 如果您重設子任務上的預估，就會重設父內文上的預估（因為父內文是其所有子任務的總和）。</li>
       </ul><br></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 計畫時數]</strong></td>
      <td> （僅適用於專案）指定任務的計畫時數。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 指定任務]</strong></td>
      <td>開始輸入您要指派子任務的專案團隊名稱，然後在它出現在下拉式清單中時按一下它。</td>
     </tr>
    </tbody>
   </table>

1. 按一下「**[!UICONTROL 建立]**」。
