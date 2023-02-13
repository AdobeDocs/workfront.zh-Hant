---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: 在迭代中建立敏捷的故事
description: 本文說明當您已處於迭代階段時，如何建立新的敏捷故事。
author: Lisa
feature: Agile
exl-id: 9712e065-5fbf-4deb-a39f-36e0e918ed12
source-git-commit: 094a9d453476418cbe1b065930eb3a179e4cf73a
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 0%

---

# 在迭代中建立敏捷的故事

本文說明當您已處於迭代階段時，如何建立新的敏捷故事。 有關從任務、問題或其他領域建立敏捷故事的資訊，請參閱 [!DNL Adobe Workfront]，請參閱 [將動態添加到現有小版本](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

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
   <td> <p>[!UICONTROL管理]對文章所在項目的訪問</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 在迭代中建立敏捷的故事

1. 轉到要建立動態的敏捷迭代：

   1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe] Workfront，然後按一下 **[!UICONTROL 團隊]**.

   1. （選用）按一下 **[!UICONTROL 交換組]** 圖示 ![切換團隊表徵圖](assets/switch-team-icon.png)，然後從下拉式選單中選取新的Scrum團隊，或在搜尋列中搜尋團隊。

   1. 在左側面板中，選取 **[!UICONTROL 迭代]**.
   1. 按一下要建立動態的特定小版本的名稱。
   1. 在左側面板中，選取 **[!UICONTROL 故事]**.

1.  按一下 **[!UICONTROL 新動態].**
1. 指定下列資訊：

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL文章名稱]</strong></td>
      <td>輸入動態名稱。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL描述]</strong></td>
      <td>輸入動態說明。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL就緒]</strong></td>
      <td>如果文章已準備好要添加到小版本，請選擇此選項。 選取此選項時，它會向使用者指出積壓工作中哪些動態已準備好新增至小版本。<br>無論文章是否被標籤，都可以將其添加到小版本 <strong>[!UICONTROL就緒]。</strong></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL估計]（點）</strong></td>
      <td>指定動態的估計值。 如果您的敏捷團隊已設定為以點數估計動態，則預設為1點等於8小時。 在文章中將預估值新增為[!UICONTROL計畫小時數]。<br>例如，如果您將動態估計為3點，預設行為是將24個計畫小時新增至動態。<br>如果動態包含子任務，請記住，所有子任務的合併估計將決定父動態的估計。 如需詳細資訊，請參閱 <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/add-a-subtask-to-an-existing-story-scrum.md" class="MCXref xref">在[!UICONTROL Scrum]展示板上將子任務添加到現有文章</a>.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL父項項目]</strong></td>
      <td>開始鍵入與此文章關聯的項目名稱。<br>依預設，動態顏色會顯示為此專案中其他動態的相同顏色。<br>項目的狀態必須設定為[!UICONTROL當前]。 如果專案的狀態為[!UICONTROL目前]以外的任何值，則下拉式功能表中不會顯示它。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL父任務]</strong></td>
      <td>選擇父項目後，您可以選擇父項任務。 當您選擇父任務時，系統會將文章建立為所選項目上父任務的子任務。<br>開始輸入動態的父任務名稱，然後在下拉清單中顯示時按一下。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL自訂Forms]</strong></td>
      <td>選取要新增至動態的任何自訂表單。</td>
     </tr>
    </tbody>
   </table>

1. 按一下 **[!UICONTROL 儲存動態]**.
