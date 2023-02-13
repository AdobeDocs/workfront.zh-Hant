---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: 將子任務添加到Scrum板上的現有文章
description: 為現有動態建立子任務時，請記住項目的「完成模式」設定，因為這會影響動態的更新方式。
author: Lisa
feature: Agile
exl-id: 264e66e9-94c7-4904-baad-f733d39b4791
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '656'
ht-degree: 0%

---

# 將子任務新增至 [!UICONTROL Scrum] 展示板

為現有動態建立子任務時，請記住以下事項：

**當 [!UICONTROL 完成模式] 專案的設定設為 [!UICONTROL 手動]:**

* 將含有子任務的父文章移動到 [!UICONTROL 完成] 將父項動態更新為100%，且 [!UICONTROL 狀態] to [!UICONTROL 完成]. 未更新子任務。
* 若要更新 [!UICONTROL 完成百分比] 對於故事，您必須從 [!UICONTROL 故事] 標籤或 [!UICONTROL 詳細資料] 頁。

**當 [!UICONTROL 完成模式] 專案的設定設為 [!UICONTROL 自動]**:

* 將含有子任務的父文章移動到 [!UICONTROL 完成] 將父項動態更新為100%，且 [!UICONTROL 狀態] to [!UICONTROL 完成]. 子任務也會更新為100%，而 [!UICONTROL 狀態] 更新為 [!UICONTROL 完成].
* 若要更新 [!UICONTROL 完成百分比] 為了講故事，您必須更新 [!UICONTROL 完成百分比] 的子任務。 此 [!UICONTROL 完成百分比] 根據 [!UICONTROL 完成百分比] 所有子任務。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計劃*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權*</strong></td> 
   <td> <p>[!UICONTROL工作]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>訪問級別配置*</strong></td> 
   <td> <p>[!UICONTROL Worker]或更高版本</p> <p>注意：如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件權限</strong></td> 
   <td> <p>[!UICONTROL Contribute]或[!UICONTROL Manage]對子任務所在任務的訪問</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 將子任務添加到Scrum板上的現有文章

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 團隊]**.

1. （選用）按一下 **[!UICONTROL 交換組]** 圖示 ![切換團隊表徵圖](assets/switch-team-icon.png)，然後從下拉式選單中選取新的Scrum團隊，或在搜尋列中搜尋團隊。

1. 轉到包含要添加子任務的文章的敏捷小版本或項目。 有關如何導航到小版本的資訊，請參閱 [查看小版本](../../../agile/use-scrum-in-an-agile-team/iterations/view-iteration.md).
1. 前往動態展示板上要新增子任務的動態圖磚。
1. 按一下 **[!UICONTROL 添加子任務]** 在主文章卡片上，建立文章的子任務。

   ![添加子任務](assets/agile-story-addsubtask-NWE.png)

   或

   按一下 **[!UICONTROL 添加子任務]** 在子任務表徵圖上建立子任務。

   [!DNL Workfront] 支援無限層級的子任務，但敏捷動態展示板上只會顯示兩個層級（子任務的子任務）。

   ![添加子任務](assets/agile-story-addsubtask2-NWE.png)

   將子任務新增至目前沒有游泳道的動態時，父任務會提升至 [!UICONTROL 父項動態] 欄和子任務在泳道內移動。

1. 指定下列資訊：

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL子任務名稱]</strong></td>
      <td> 指定子任務的名稱。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL描述]</strong></td>
      <td>指定子任務的說明。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL估計]</strong></td>
      <td>指定子任務的估計值。<br><p>建立估計時，請記住以下事項：</p>
       <ul>
        <li>如果您的敏捷團隊已設定為以點數估計動態，則預設為1點等於8小時。 在文章中將預估值新增為[!UICONTROL計畫小時數]。</li>
        <li>所有子任務的合併估計確定父項動態的估計。 如需詳細資訊，請參閱 <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/update-status-of-stories-and-subtasks.md" class="MCXref xref">更新Scrum板上的動態和子任務的狀態</a>.</li>
        <li>建立新子任務時，已設定[!UICONTROL估計]欄位。 如果重置子任務的估計值，則將重置父層層層層的估計值（因為父層層層是其所有子任務的總和）。</li>
       </ul><br></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL計畫小時數]</strong></td>
      <td> （僅適用於項目）指定任務的計畫小時數。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL分配]</strong></td>
      <td>開始鍵入要分配子任務的團隊的名稱，然後在下拉清單中顯示該子任務時按一下它。</td>
     </tr>
    </tbody>
   </table>

1. 按一下 **[!UICONTROL 建立]**。
