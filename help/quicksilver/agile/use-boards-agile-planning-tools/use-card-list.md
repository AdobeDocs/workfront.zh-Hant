---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: 使用卡片清單
description: 您可以在工作流程上建立卡片清單，並將卡片新增到疊代。
author: Lisa
feature: Agile
exl-id: 2976f7e8-be84-4d27-9d70-8430392d5331
source-git-commit: d44eb048103e469bc072cc5287947fea471668b3
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 0%

---

# 使用卡片清單

>[!IMPORTANT]
>
>工作串流無法供所有客戶使用。

您可以在工作流程上建立卡片清單，並將卡片新增到疊代。

卡片清單可作為工作流程的待處理工作。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計畫*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權*</strong></td> 
   <td> <p>[！UICONTROL Request]或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

## 將卡片新增至卡片清單

{{step1-to-boards}}

1. 若要開啟工作流程，請按一下[檢視工作流程]。[!UICONTROL ****]
1. 按一下&#x200B;[!UICONTROL **卡片清單**]&#x200B;標籤。
1. 按一下&#x200B;[!UICONTROL **新增卡片**]。
1. 在&#x200B;[!UICONTROL **建立/編輯卡片**]&#x200B;對話方塊中，新增下列資訊：

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td><strong>[！UICONTROL名稱]</strong></td> 
      <td>卡片名稱。</td> 
     </tr> 
     <tr> 
      <td><strong>[！UICONTROL說明]</strong></td> 
      <td>卡片的說明。</td> 
     </tr>
     <tr> 
      <td><strong>[！UICONTROL估算]</strong></td> 
      <td>要完成的卡片預計小時數。 這僅是手動輸入。</td> 
     </tr>
     <tr> 
      <td><strong>[！UICONTROL狀態]</strong></td> 
      <td>選取卡片的狀態。</td> 
     </tr>
     <tr> 
      <td><strong>[！UICONTROL反複專案]</strong></td> 
      <td>選取要指派卡片的目標反複專案。</td> 
     </tr>
     <tr> 
      <td><strong>[！UICONTROL受託人]</strong></td> 
      <td><p>若要指派卡片，請在搜尋欄位中開始輸入名稱，然後在其顯示在清單中時選取它。 您可以同時新增個人和團隊，也可以將多個人員或團隊指派至卡片。</p><p>受指派人必須是工作流程的成員，否則他們不會出現在選取專案清單中。</p></td> 
     </tr>
    </tbody> 
   </table>

1. 按一下「[!UICONTROL **儲存**]」。
1. 繼續新增卡片，直到您建立卡片清單為止。

## 檢視卡片

若要檢視單一清單中工作流程的所有卡片，請按一下[卡片清單]索引標籤上的[清單檢視]。[!UICONTROL ****]

若要檢視依反複專案分組的工作流的所有卡片，請按一下&#x200B;[!UICONTROL **反複專案檢視**]。 未計畫的卡片會顯示在自己的群組中。

若要編輯現有卡片，請在清單中選取該卡片，然後按一下[編輯]。[!UICONTROL ****]

若要刪除卡片，請在清單中選取該卡片，然後按一下&#x200B;[!UICONTROL **刪除**]。

### 篩選卡片

卡片只能從疊代板封存。 封存卡片時，除非您篩選以顯示已封存的卡片，否則卡片清單中不會顯示卡片。 如需有關封存卡片的資訊，請參閱[從展示板刪除或封存卡片](/help/quicksilver/agile/get-started-with-boards/delete-board-items.md)。

1. 存取工作流程的卡片清單。
1. 按一下&#x200B;[!UICONTROL **篩選器**]&#x200B;並選取&#x200B;[!UICONTROL **全部**]、[!UICONTROL **使用中的卡片**]&#x200B;或&#x200B;[!UICONTROL **已封存的卡片**]。

   將預設以外的篩選器套用至卡片清單時，篩選器圖示![已套用篩選器](assets/boards-filterapplied-30x30.png)上會顯示指示器。

### 在卡片清單中搜尋

1. 存取工作流程的卡片清單。
1. 按一下「[!UICONTROL **搜尋**]」並輸入搜尋字詞。 然後，按下Enter。

   所有包含搜尋字詞的卡片都會顯示。
按一下X以清除搜尋。

   ![搜尋展示板中的卡片](assets/boards-searchbox.png)

## 將卡片新增至反複專案

>[!NOTE]
>
>您必須先建立反複專案，才能在其中新增卡片。 如需詳細資訊，請參閱[在工作流](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md)中建立反複專案。

1. 存取工作流程的卡片清單。
1. 選取&#x200B;[!UICONTROL **反複專案檢視**]&#x200B;以檢視哪些卡片已指派給反複專案，哪些是未計畫的。
1. 在清單中選取未計畫的卡片，然後按一下[編輯]。[!UICONTROL ****]
1. 在&#x200B;[!UICONTROL **反複專案**]&#x200B;欄位中選取反複專案。
1. 如果您使用劇本點，請在&#x200B;[!UICONTROL **預估**]&#x200B;欄位中輸入值。
1. 按一下「[!UICONTROL **儲存**]」。

   卡片會移至疊代，疊代量度會反映卡片和點的數量。

   您也可以將卡片從「未計畫的卡片」群組拖放至反複專案，或按一下「[!UICONTROL **新增卡片**]」以將卡片新增至反複專案。

>[!TIP]
>
>如果您已建立反複專案程式板，卡片清單上所有未計畫的卡片都會顯示在[!UICONTROL 待處理專案]欄中。 將卡片移至另一欄時，它會成為作用中疊代的一部分。 您新增到卡片清單中疊代的卡片會根據其狀態新增到欄。
