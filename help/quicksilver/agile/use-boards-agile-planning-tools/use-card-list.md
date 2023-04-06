---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: 使用卡片清單
description: 您可以在工作流上建立卡片清單，並將卡片新增至迭代。
author: Lisa
feature: Agile
source-git-commit: 8c02f5364154bdc343512416d0c7e38ef563a170
workflow-type: tm+mt
source-wordcount: '606'
ht-degree: 0%

---

# 使用卡片清單

您可以在工作流上建立卡片清單，並將卡片新增至迭代。

卡清單可作為工作流的積壓工作。

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
   <td> <p>[!UICONTROL Request]或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

## 將資訊卡新增至資訊卡清單

{{step1-to-boards}}

1. 若要開啟工作流，請按一下 [!UICONTROL **檢視工作流**].
1. 按一下 [!UICONTROL **卡片清單**] 標籤。
1. 按一下 [!UICONTROL **新增卡片**].
1. 在 [!UICONTROL **建立/編輯卡片**] 對話框中，添加以下資訊：

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td><strong>[!UICONTROL名稱]</strong></td> 
      <td>卡片的名稱。</td> 
     </tr> 
     <tr> 
      <td><strong>[!UICONTROL描述]</strong></td> 
      <td>卡片的說明。</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL估計]</strong></td> 
      <td>卡完成的預計小時數。 這只是手動輸入。</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL狀態]</strong></td> 
      <td>選取卡片的狀態。</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL迭代]</strong></td> 
      <td>選取要將卡片指派給的小版本。</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL受分配者]</strong></td> 
      <td><p>若要指派資訊卡，請開始在搜尋欄位中輸入名稱，然後在資訊卡顯示於清單時加以選取。 您可以新增個人和團隊，並且可以指派多個人員或團隊至資訊卡。</p><p>受分配者必須是工作流上的成員，否則它們不會出現在選擇清單中。</p></td> 
     </tr>
    </tbody> 
   </table>

1. 按一下&#x200B;[!UICONTROL **儲存**]。
1. 繼續新增資訊卡，直到您建立資訊卡清單為止。

## 檢視資訊卡

若要在單一清單中檢視工作流的所有卡片，請按一下 [!UICONTROL **清單檢視**] （在「卡片清單」頁簽上）。

要查看按小版本分組的工作流的所有卡，請按一下 [!UICONTROL **迭代視圖**]. 計畫外卡顯示在自己的組中。

若要編輯現有的資訊卡，請在清單中選取資訊卡，然後按一下 [!UICONTROL **編輯**].

若要刪除資訊卡，請在清單中選取資訊卡，然後按一下 [!UICONTROL **刪除**].

### 篩選卡

卡片只能從迭代展示板封存。 封存卡片時，除非您篩選以顯示已封存的卡片，否則卡片清單中不會顯示該卡片。 如需封存資訊卡的詳細資訊，請參閱 [從展示板刪除或封存資訊卡](/help/quicksilver/agile/get-started-with-boards/delete-board-items.md).

1. 存取工作流的卡清單。
1. 按一下 [!UICONTROL **篩選**] 選取 [!UICONTROL **全部**], [!UICONTROL **作用中卡**]，或 [!UICONTROL **封存的卡片**].

   當卡片清單上套用預設值以外的篩選時，篩選器圖示上會顯示指標 ![已套用篩選](assets/boards-filterapplied-30x30.png).

### 在卡片清單中搜尋

1. 存取工作流的卡清單。
1. 按一下 [!UICONTROL **搜尋**] 並輸入搜尋詞。 然後，按Enter鍵。

   會顯示包含搜尋詞的所有卡片。
按一下X以清除搜尋。

   ![在展示板中搜尋資訊卡](assets/boards-searchbox.png)

## 將卡片新增至小版本

>[!NOTE]
>
>您必須先建立小版本，才能新增卡片。 如需詳細資訊，請參閱 [在工作流中建立小版本](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

1. 存取工作流的卡清單。
1. 選取 [!UICONTROL **迭代視圖**] 查看哪些卡被分配給小版本，哪些是計畫外的。
1. 在清單中選擇計畫外卡，然後按一下 [!UICONTROL **編輯**].
1. 在 [!UICONTROL **迭代**] 欄位。
1. 如果您使用動態點，請在 [!UICONTROL **估計**] 欄位。
1. 按一下&#x200B;[!UICONTROL **儲存**]。

   卡片會移至小版本，而小版本量度會反映卡片和點的數量。

   您也可以將卡片從「計畫外卡片」組拖放到小版本中，或按一下 [!UICONTROL **新增卡片**] 將新卡添加到小版本。

>[!TIP]
>
>如果已建立迭代流程板，則卡清單上的所有計畫外卡都將顯示在 [!UICONTROL 積壓] 欄。 當卡片移入另一欄時，它會成為作用中小版本的一部分。 您新增至卡片清單中小版本的卡片，會根據其狀態新增至欄。

