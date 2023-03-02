---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: 在主板上使用連接的卡
description: 您可以在主板上新增資訊卡，連線至Workfront中的現有工作和問題。
author: Lisa
feature: Agile
exl-id: c6d979dd-e4a4-48a5-a91b-b31d7ef848d1
source-git-commit: 1817f3b1a5950823ff6ce600b1fef09ff4ca6767
workflow-type: tm+mt
source-wordcount: '1227'
ht-degree: 0%

---

# 在主板上使用連接的卡

您可以在主板上新增卡片，卡片已連線至 [!DNL Workfront].

在某個位置更新資訊卡的下列任何一項詳細資訊時，就會在另一個位置自動更新：

* [!UICONTROL 名稱]
* [!UICONTROL 說明]
* [!UICONTROL 受託人]
* [!UICONTROL 狀態]
* [!UICONTROL 規劃完成日期]
* [!UICONTROL 估計] / [!UICONTROL 文章點]

>[!NOTE]
>每個主板只能添加一次單個連接的任務或問題。 同一任務或問題可以連接到多個主板。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計劃*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權*</strong></td> 
   <td> <p>[!UICONTROL Request]或更高版本</p> </td> 
  </tr> 
  <tr>
   <td role="rowheader"><strong>訪問級別配置*</strong></td>
   <td><p>[!UICONTROL View]或更高版本對任務和問題的訪問</p></td>
  </tr>
  <tr>
   <td role="rowheader"><strong>物件權限</strong></td>
   <td><p>[!UICONTROL View]或更高的Workfront任務或問題權限</p></td>
  </tr>
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 添加已連接的卡

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **[!UICONTROL 展示板]**.
1. 存取展示板。 如需詳細資訊，請參閱 [建立或編輯展示板](../../agile/get-started-with-boards/create-edit-board.md).
1. 按一下 **[!UICONTROL 新增卡片] > [!UICONTROL 已連接卡]**.
1. 選擇專案，然後選擇要新增為展示板上資訊卡的任務或問題。

   您可以選取多個物件，且這些物件都會以個別卡片的形式新增。

   >[!NOTE]
   >
   >* 搜索結果中只有您有權限的對象。 如果項目呈暗灰色，它已添加到展示板中。
   >* 篩選依據時 **[!UICONTROL 我擁有的專案]** 或 **[!UICONTROL 正在執行的項目]**，則不會包含等同於「完成」、「無效」或「已拒絕」狀態的專案。 您仍可使用 **[!UICONTROL 全部]** 篩選。


1. 按一下 **[!UICONTROL 新增]**.

   ![搜索要連接的任務或問題](assets/boards-tasksissues-350x94.png)

   卡片會新增至最左側欄的底部。 已連接 [!DNL Workfront] 物件及其指派者會顯示在卡片上。

   >[!NOTE]
   >
   >若受託人 [!DNL Workfront] 任務或問題不是展示板上的成員，它們未分配給資訊卡。

   ![已連接的卡片](assets/boards-connected-card-first-added.png)

1. 按一下 ![開啟任務或問題](assets/boards-launch-icon.png) 開啟 [!DNL Workfront] 任務或問題。
1. 若要編輯卡片詳細資訊，請按一下卡片（而非卡片名稱中）。

   或

   按一下 **[!UICONTROL 更多]** 功能表 ![更多功能表](assets/more-icon-spectrum.png) 在「 」卡片上，然後選取 **[!UICONTROL 編輯]**.

1. 在 **[!UICONTROL 卡片詳細資訊]** 框中，添加或更新以下資訊：

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL名稱]</strong></td> 
      <td> <p>更改名稱也會更改連接的名稱 [!DNL Workfront] 物件。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL描述]</strong></td> 
      <td> <p>更改說明還更改了連接的說明 [!DNL Workfront] 物件。</p> </td> 
     </tr> 
     <tr>
      <td role="rowheader"><strong>[!UICONTROL受分配者]</strong></td>
      <td><p>若要指派更多人員或團隊至資訊卡，請開始在搜尋欄位中輸入名稱，然後在資訊卡顯示於清單時加以選取。 您可以新增個人和團隊。 在連接的卡上僅允許一個團隊分配。</p>
      <p>受分配者必須是板上的成員，否則他們不會出現在選擇清單中。 當團隊是展示板上的成員時，可將個別團隊成員指派給資訊卡。</p>
      <p>您選擇的任何受分配者也將分配給 [!DNL Workfront].</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL列]</strong></td>
      <td><p>選取卡片的欄。</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL狀態]</strong></td>
      <td><p>選取卡片的狀態。 預設值為[!UICONTROL New]、[!UICONTROL In Progress]和[!UICONTROL Complete]，但是為中的項目定義的任何自定義狀態 [!DNL Workfront] 也可供使用。</p>
      <p>如果您已啟用欄位原則來更新欄位值，變更卡片上的狀態會自動將卡片移至對應的欄。 如需詳細資訊，請參閱文章中的「定義欄設定和原則」 <a href="/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md" class="MCXref xref">管理展示板欄</a>.</p>
      <p>如果您按一下 <strong>[!UICONTROL標籤完成]</strong> 在卡片頂端，狀態會自動變更為「完成」。</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL計畫完成]</strong></td>
      <td><p>更改此日期也會更改連接的計畫完成日期 [!DNL Workfront] 物件。</p></td>
     </tr>
      <tr>
      <td role="rowheader"><strong>[!UICONTROL估計]</strong></td>
      <td><p>卡片完成的小時數。</p><p>如果您對 [!DNL Workfront] [!UICONTROL主板]，更改估計也會更改連接的故事點值 [!DNL Workfront] 物件。</p><p>如果您不選擇使用早期功能，此欄位僅為手動輸入，值不能超過99。</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL標籤]</strong></td>
      <td><p>搜尋並選取卡片的標籤。</p>
      <p>如需建立新標籤的詳細資訊，請參閱 <a href="../../agile/get-started-with-boards/add-tags.md" class="MCXref xref">新增標籤</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL檢查清單項]</strong> </td> 
      <td> <p>按一下 <strong>[!UICONTROL添加檢查清單項]</strong>. 然後，鍵入項目的標題，然後按Enter鍵。 系統會自動新增另一個項目。 繼續輸入標題以添加更多項。</p> <p>核對清單頂端的計數器會顯示已完成項目的數量和項目總數。</p> <p>如需檢查清單項目的詳細資訊，請參閱 <a href="/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md">管理卡上的檢查清單項目</a>.</p></td>
     </tr>
    </tbody> 
   </table>

1. 按一下 **[!UICONTROL 關閉]** 回到董事會。
連接的對象、受分配者、標籤、到期日、檢查清單計數器、估計小時數和狀態顯示在卡上。

   ![新增至展示板的資訊卡](assets/boards-connected-card-details-110922.png)

## 斷開已連接的卡

您可以從其Workfront物件中斷已連線的卡片，而卡片會作為您可編輯的臨機卡片保留在展示板上。

要在主板級別斷開連接：

1. 進入展示板。
1. 按一下 **[!UICONTROL 更多]** 功能表 ![更多功能表](assets/more-icon-spectrum.png) 在已連接的卡上，然後選擇 **[!UICONTROL 斷開連接]**.
1. 按一下 **[!UICONTROL 斷開連接]** 在確認訊息上。

要在卡級別斷開連接：

1. 進入主板並開啟已連接的卡。
1. 按一下 **[!UICONTROL 更多]** 功能表 ![更多功能表](assets/more-icon-spectrum.png) 在卡詳細資訊的「連接」區域中，選擇 **[!UICONTROL 斷開連接]**.
1. 按一下 **[!UICONTROL 斷開連接]** 在確認訊息上。

## 將臨機卡轉換為已連接的卡

建立隨選卡片後，您可將其轉換為已連線的卡片。 如需臨機卡的詳細資訊，請參閱 [新增臨機卡至展示板](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md).

1. 存取展示板並開啟臨機資訊卡。
1. 驗證卡上的名稱和說明。 它們將新增至您在中建立的任務或問題 [!DNL Workfront].
1. 在 [!UICONTROL 連線] 卡片詳細資訊的區域，按一下 **[!UICONTROL 連線Workfront]**.
1. 在 [!UICONTROL 連接卡] ，選擇是建立任務還是問題。
1. 搜索並選擇項目以添加任務或問題。

   >[!NOTE]
   >
   >* 搜索結果中只有您有權限的對象。
   >* 篩選依據時 **[!UICONTROL 我擁有的專案]** 或 **[!UICONTROL 正在執行的項目]**，專案等於 [!UICONTROL 完成], [!UICONTROL 死亡]，或 [!UICONTROL 已拒絕] 狀態未包含。 您仍可使用 **[!UICONTROL 全部]** 篩選。


1. 按一下 **[!UICONTROL Connect]**.

   ![將臨機卡連線至Workfront](assets/boards-connect-ad-hoc-card.png)

   專案名稱會顯示在卡片詳細資訊的「連線」區域中。

1. 按一下 **[!UICONTROL 關閉]** 回到董事會。

## 登錄已連接的卡的時數

>[!NOTE]
>
>只有透過Workfront展示板的早期功能選擇，才能使用此功能。

您必須擁有正確的權限才能登錄所連接任務或問題的數小時。

依預設，連線的卡片上不會顯示時間記錄欄位。 您必須啟用 [!UICONTROL **小時**] 在 [!UICONTROL 設定] 區域 [!UICONTROL 卡片]. 如需詳細資訊，請參閱 [自訂卡片上顯示的欄位](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

1. 輸入任務或問題的小時數。
1. 選取 [!UICONTROL 小時類型] （如果與預設值不同）。
1. 按一下 [!UICONTROL **記錄時間**].

   ![登錄卡時數](assets/log-hours-on-card.png)

   卡上記錄的時間也會儲存在所連接的任務或問題上。

卡上的記錄時間與任務或問題的記錄時間相同。 如需詳細資訊，請參閱文章中的「登入專案、工作或問題的時間」 [記錄時間](/help/quicksilver/timesheets/create-and-manage-timesheets/log-time.md).

