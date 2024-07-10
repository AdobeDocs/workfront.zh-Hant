---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: 在展示板上使用連線的卡片
description: 您可以在展示板上新增卡片，該卡片會連線至Workfront中的現有任務和問題。
author: Lisa
feature: Agile
exl-id: c6d979dd-e4a4-48a5-a91b-b31d7ef848d1
source-git-commit: 5c093edc97afdbd1d88824376ce4b019f71e099f
workflow-type: tm+mt
source-wordcount: '1492'
ht-degree: 0%

---

# 在展示板上使用連線的卡片

<!-- Audited: 2/2024 -->

您可以在展示板上新增卡片，該卡片會連線至中的現有任務和問題 [!DNL Workfront].

當一個位置中的卡片的下列任一詳細資料更新時，另一個位置中的卡片會自動更新：

* [!UICONTROL 名稱]
* [!UICONTROL 說明]
* [!UICONTROL 被指定者]
* [!UICONTROL 狀態]
* [!UICONTROL 計畫完成日期]
* [!UICONTROL 預估] / [!UICONTROL 劇本點]
* [!UICONTROL 子任務]
* [!UICONTROL 文件]

>[!NOTE]
>
>每個展示板只能新增一次單一連線任務或問題。 相同任務或問題可以連線到多個展示板。

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
   <td>
   <p>新增：投稿人或更高版本</p>
   <p>或</p>
   <p>目前：要求或以上</p>
 </td> 
  </tr> 
  <tr>
   <td role="rowheader">存取層級設定</td>
   <td><p>檢視或更高的任務和問題存取權</p></td>
  </tr>
  <tr>
   <td role="rowheader">物件許可權</td>
   <td><p>檢視Workfront任務或問題的或更高許可權</p>
   <p><strong>注意：</strong> 擁有任務或問題檢視許可權的使用者無法在與其連線的卡片上進行任何操作，包括將卡片移動到展示板上的另一欄。 檢視使用者只能開啟卡片以檢視其屬性，並開啟連線的工作或問題。 若要請求其他存取權，請開啟任務或問題並在那裡請求存取權。</td>
  </tr>
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## 新增連線的卡片

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon.png) 在Adobe Workfront的右上角，或（如果有的話）按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon-left-nav.png) 然後按一下「 」 **[!UICONTROL 展示板]**.
1. 存取展示板。 如需詳細資訊，請參閱 [建立或編輯展示板](../../agile/get-started-with-boards/create-edit-board.md).
1. 按一下 **[!UICONTROL 新增卡片] > [!UICONTROL 已連線的卡片]**.
1. 選擇專案，然後選擇要新增為展示板上卡片的任務或問題。

   您可以選取多個物件，而且它們都將新增為個別的卡片。

   >[!NOTE]
   >
   >* 搜尋結果中只能使用您有權使用的物件。 如果專案變暗，則表示該專案已經加入展示板中。
   >* 當您依據以下條件篩選時： **[!UICONTROL 我擁有的專案]** 或 **[!UICONTROL 我參與的專案]**，等同於完成、廢棄或已拒絕狀態的專案不會包括在內。 您仍然可以使用搜尋這些專案 **[!UICONTROL 全部]** 篩選。

1. 按一下 **[!UICONTROL 新增]**.

   ![搜尋要連線的任務或問題](assets/boards-tasksissues-350x94.png)

   卡片會新增至最左側的欄底部。 連線的 [!DNL Workfront] 物件與其工作負責人會顯示在卡片上。

   ![已連線的卡片](assets/boards-connected-card-first-added.png)

1. 按一下 ![開啟任務或問題](assets/boards-launch-icon.png) 以開啟 [!DNL Workfront] 新瀏覽器標籤中的任務或問題。
1. 若要編輯卡片詳細資料，請按一下卡片（不在卡片名稱中）。

   或

   按一下 **[!UICONTROL 更多]** 功能表 ![更多選單](assets/more-icon-spectrum.png) 在卡片上，然後選取 **[!UICONTROL 編輯]**.

1. 在 **[!UICONTROL 卡片詳細資料]** 方塊，新增或更新下列資訊：

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL名稱]</strong></td> 
      <td>變更名稱也會變更已連線的名稱 [!DNL Workfront] 物件。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL說明]</strong></td> 
      <td>變更說明也會變更已連線的說明 [!DNL Workfront] 物件。 您可以在說明中新增URL，這些URL在儲存卡片時就會變成可點按的連結。</td> 
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL欄]</strong></td>
      <td>選取卡片的欄。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL狀態]</strong></td>
      <td><p>選取卡片的狀態。 預設值為[！UICONTROL New]、[！UICONTROL In Progress]和[！UICONTROL Complete]，但為中的專案定義的任何自訂狀態。 [!DNL Workfront] 也可供使用。</p>
      <p>如果您已啟用欄原則來更新欄位值，則變更卡片上的狀態會自動將卡片移動到對應的欄。 如需詳細資訊，請參閱文章中的「定義欄設定和原則」 <a href="/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md" class="MCXref xref">管理展示板欄</a>.</p>
      <p>如果您按一下 <strong>[！UICONTROL標籤完成]</strong> 在卡片頂端，狀態會自動變更為「完成」。</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL計畫完成]</strong></td>
      <td>變更此日期也會變更已連線上的規劃完成日期 [!DNL Workfront] 物件。</td>
     </tr>
      <tr>
      <td role="rowheader"><strong>[！UICONTROL估算]</strong></td>
      <td><p>要完成的卡片小時數。</p><p>變更預估也會變更連線上的劇本點值 [!DNL Workfront] 物件。</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL指定任務]</strong></td>
      <td><p>若要指派更多人員或團隊給卡片，請按一下 <strong>[！UICONTROL新增指派]</strong> 並開始在搜尋欄位中輸入名稱。 然後，當它顯示在結果清單中時選取它。 您可以新增個人和團隊。 已連線的卡片只允許一個群組指派。</p>
      <p>您選取的任何受指派人也會指派至中的任務或問題 [!DNL Workfront].</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL標籤]</strong></td>
      <td><p>搜尋並選取卡片的標籤。</p>
      <p>如需建立新標籤的詳細資訊，請參閱 <a href="../../agile/get-started-with-boards/add-tags.md" class="MCXref xref">新增標籤</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL自訂欄位]</strong></td>
      <td><p>您新增的任何自訂欄位都會顯示在此區域中。</p>
      <p>如需詳細資訊，請參閱 <a href="/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md">自訂要在卡片上顯示的欄位</a>.</p></td>
     </tr>
     <tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL Subtask]</strong></td>
      <td><p>任務的任何現有子任務都會出現在此區段中。 按一下 <strong>[！UICONTROL新增子任務]</strong> 以新增子任務。</p>
      <p>區段頂端的計數器顯示已完成子工作的數目以及子工作的總數。</p>
      <p>如需子工作的詳細資訊，請參閱 <a href="/help/quicksilver/agile/get-started-with-boards/manage-subtasks-on-boards.md">管理展示板上的子任務</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL檢查清單]</strong></td>
      <td><p>按一下 <strong>[！UICONTROL新增檢查清單專案]</strong>. 然後，輸入專案的標題並按Enter鍵。 系統會自動新增另一個專案。 繼續輸入標題以新增更多專案。</p>
      <p>檢查清單頂端的計數器顯示已完成的專案數和專案總數。</p> <p>如需檢查清單專案的詳細資訊，請參閱 <a href="/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md">管理卡片上的檢查清單專案</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL檔案]</strong></td>
      <td>針對現有檔案，將滑鼠停留在檔案縮圖上，然後按一下 <strong>預覽</strong> 在瀏覽器中檢視檔案，或 <strong>下載</strong> 將檔案下載到您的電腦。 如需新檔案，請參閱 <a href="/help/quicksilver/agile/get-started-with-boards/add-documents-on-cards.md">在卡片上新增檔案</a>.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL小時]</strong></td>
      <td>請參閱下方的「在連線的卡片上記錄時數」。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[！UICONTROL註解]</strong></td>
      <td><p>按一下 <strong>[！UICONTROL新增註解]</strong> 欄位並輸入您的註解。 使用格式化工具來格式化文字。 若要標籤人員或團隊，請使用註釋區域底部的搜尋方塊。 使用者不必是展示板的成員。 已連線卡片上的標籤使用者將收到電子郵件通知。</p><p>按一下 <strong>[！UICONTROL提交]</strong> 將註解新增至卡片。</p>
      <p>如需註解的詳細資訊，請參閱 <a href="/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md">更新工作</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL系統活動]</strong></td> 
      <td><p>如果您有 <strong>系統活動</strong> 啟用為卡片區段，活動會顯示在此區域中。</p> <p>如需詳細資訊，請參閱 <a href="/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md">自訂要在卡片上顯示的欄位</a> 和 <a href="/help/quicksilver/administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md">系統追蹤更新</a>.</p></td>
     </tr>     
    </tbody> 
   </table>

   使用左側導覽面板在卡片詳細資訊的欄位區段之間移動。

1. 按一下 **[!UICONTROL 關閉]** 以返回展示板。
連線物件、受託人、標籤、到期日、檢查清單計數器、預估時數和狀態都會顯示在卡片上。

   ![卡片已新增到展示板](assets/boards-connected-card-details-110922.png)

## 中斷連線的卡片

您可以將已連線的卡片與其Workfront物件中斷連線，而卡片會保留在展示板上，作為您可編輯的臨機操作卡片。

若要中斷主機板層級的連線：

1. 存取展示板。
1. 按一下 **[!UICONTROL 更多]** 功能表 ![更多選單](assets/more-icon-spectrum.png) ，然後選取「 」 **[!UICONTROL 中斷連線]**.
1. 按一下 **[!UICONTROL 中斷連線]** 於確認訊息上。

若要中斷卡層級的連線：

1. 存取主機板並開啟已連線的卡片。
1. 按一下 **[!UICONTROL 更多]** 功能表 ![更多選單](assets/more-icon-spectrum.png) 在卡片詳細資訊的連線區域中，然後選取 **[!UICONTROL 中斷連線]**.
1. 按一下 **[!UICONTROL 中斷連線]** 於確認訊息上。

## 將臨機操作卡片轉換為已連線的卡片

建立Ad Hoc卡片後，可將其轉換為已連線的卡片。 如需關於臨時卡片的詳細資訊，請參閱 [新增臨機卡到展示板](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md).

1. 存取展示板並開啟ad hoc資訊卡。
1. 驗證卡片上的名稱和說明。 它們將被新增到您在中建立的任務或問題中 [!DNL Workfront].
1. 在 [!UICONTROL 連線] 卡片詳細資訊區域，按一下 **[!UICONTROL 與Workfront連結]**.
1. 在 [!UICONTROL 連線卡片] 視窗中，選取您是要建立任務還是問題。
1. 搜尋並選取要新增任務或問題的專案。

   >[!NOTE]
   >
   >* 搜尋結果中只能使用您有權使用的物件。
   >* 當您依據以下條件篩選時： **[!UICONTROL 我擁有的專案]** 或 **[!UICONTROL 我參與的專案]**，等同於 [!UICONTROL 完成]， [!UICONTROL 廢棄]，或 [!UICONTROL 已拒絕] 不包含狀態。 您仍然可以使用搜尋這些專案 **[!UICONTROL 全部]** 篩選。

1. 按一下 **[!UICONTROL 連線]**.

   ![將ad hoc卡片連線到Workfront](assets/boards-connect-ad-hoc-card.png)

   專案名稱會顯示在卡片詳細資料的「連線」區域中。

1. 按一下 **[!UICONTROL 關閉]** 以返回展示板。

## 在已連線的卡片上記錄時數

您必須擁有正確的許可權，才能記錄連線任務或問題的時數。

依預設，已連線的卡片上不會顯示時間記錄欄位。 您必須啟用 [!UICONTROL **小時**] 在 [!UICONTROL 設定] 區域在 [!UICONTROL 卡片]. 如需詳細資訊，請參閱 [自訂要在卡片上顯示的欄位](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

1. 輸入任務或問題的小時數。
1. 選取 [!UICONTROL 小時型別] （如果不同於預設值）。
1. 按一下 [!UICONTROL **記錄時間**].

   ![在卡片上記錄時數](assets/log-hours-on-card.png)

   登入卡片的時間也會儲存在已連線的任務或問題上。

在資訊卡上記錄時間與在工作或問題上記錄時間相同。 如需詳細資訊，請參閱文章中的「在專案、任務或問題上記錄時間」 [記錄時間](/help/quicksilver/timesheets/create-and-manage-timesheets/log-time.md).

