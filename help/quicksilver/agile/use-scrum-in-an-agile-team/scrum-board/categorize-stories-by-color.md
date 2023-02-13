---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: 依色彩分類Scrum展示板上的動態
description: Scrum展示板文章的預設顏色關聯會因文章展示板位於迭代版本還是位於項目而有所不同。
author: Lisa
feature: Agile
exl-id: 8e351505-73d1-4c8f-b369-53c965b88c95
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# 依照上的顏色分類動態 [!UICONTROL Scrum] 展示板

## 變更動態的預設顏色關聯

文章的預設顏色關聯會因文章展示板位於小版本還是項目而有所不同：

* **[!UICONTROL 迭代]**:在小版本中，文章展示板圖磚會根據文章關聯的專案進行色彩編碼。 （每個專案在展示板上都會任意指定顏色。） 您可以變更每個敏捷團隊的預設行為。 小版本上敏捷動態的顏色可以與項目（預設）、動態優先順序、所有者或自由格式相連結。 如需詳細資訊，請參閱 [設定如何在敏捷動態展示板上為動態使用顏色指標](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur4) 在文章中 [配置Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

* **[!UICONTROL 專案]**:在專案中，任何子任務都會與父任務的顏色匹配，因此任何指定泳道中所有文章的顏色都相同。 如果任務沒有任何子任務或沒有父任務，則在建立任務時，會隨機將顏色分配給任務。 您可以修改敏捷視圖以變更此預設行為。 專案上敏捷動態的顏色可以與父動態（預設）、動態優先順序、擁有者或自由表單系結。 如需詳細資訊，請參閱 [建立或自訂 [!UICONTROL 敏捷] 檢視](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) in [檢視概觀，於 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

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
   <td> <p>[!UICONTROL Worker]或更高版本</p> <p>注意：如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可以更改您的訪問級別，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 使用自由格式時變更文章的顏色

如果已設定敏捷團隊設定，則 [!UICONTROL 將卡片顏色關聯至] 選項設為 [!UICONTROL 自由格式]，使用者可以手動變更個別動態圖磚的顏色。 這對於傳達對團隊或組織而言重要的其他類型資訊非常有用：

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe] Workfront，然後按一下 **[!UICONTROL 團隊]**.

1. （選用）按一下 **[!UICONTROL 交換組]** 圖示 ![切換團隊表徵圖](assets/switch-team-icon.png)，然後從下拉式選單中選取新的Scrum團隊，或在搜尋列中搜尋團隊。

1. 在左側面板中，選取 **[!UICONTROL 迭代]** 要選擇特定的小版本，或選擇 **[!UICONTROL 當前迭代]**.
1. 將滑鼠移到文章圖磚頂端的彩色橫幅上。

   ![](assets/agile-story-color1-nwe-350x140.png)

1. 按一下 **[!UICONTROL 變更顏色]**，然後選取所需的顏色。

   ![](assets/agile-story-color2-nwe-350x138.png)
