---
content-type: overview
product-area: agile-and-teams
navigation-topic: agile-navigation-topic
title: 將輸入欄新增到展示板
description: 您可以選擇將輸入欄新增到您的展示板，在任務與問題新增到Workfront時，根據您定義的篩選器自動提取作為連線卡片。
author: Lisa
feature: Agile
exl-id: 4991f4f7-6f3d-4e15-ae8d-96433ed46557
source-git-commit: 1b91cac202151cd60f16b4ef034b60f840088aea
workflow-type: tm+mt
source-wordcount: '1090'
ht-degree: 1%

---

# 將輸入欄新增到展示板

您可以選擇將引入欄新增到您的展示板，在將任務和問題新增到時，會自動提取作為已連線卡片的任務和問題 [!DNL Workfront]，根據您定義的篩選器而定。 輸入欄可做為Kanban團隊的待處理欄、支援團隊檢視新增至請求佇列之問題的輸入位置，或您所需的任何其他目的。

展示板上只允許有一個輸入欄，且一律顯示為最左側的欄。

動態展示板上沒有輸入欄。 不過，您可以更新篩選器，以定義將哪些卡片帶入動態展示板。 在動態板上變更這些篩選器時，不會成為Workfront任務或問題一部分的卡片設定（例如標籤）會重設。

輸入欄限製為300個任務和300個問題。 在輸入欄中的專案預設順序如下：

任務：

* 主要順序：專案名稱
* 次要順序：工作分解結構

問題：

* 主要順序：專案名稱
* 次要順序：參考編號

>[!IMPORTANT]
>
>如果有多位使用者同時使用主機板，建議經常重新整理主機板。 重新整理頁面有助於將展示板上的視覺變更保持最新，並防止重複卡片從引入欄移至展示板之類的問題。

如需欄的詳細資訊，請參閱 [管理展示板欄](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). 如需有關已連線卡片的資訊，請參閱 [在展示板上使用連線的卡片](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

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
   <td> <p>[!DNL Request] 或更高</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 使用簡單篩選器建立輸入欄

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](assets/main-menu-icon.png) (位於Adobe Workfront的右上角)，然後按一下 **[!UICONTROL 展示板]**.
1. 存取展示板。 如需詳細資訊，請參閱 [建立或編輯展示板](../../agile/get-started-with-boards/create-edit-board.md).
1. 按一下 **[!UICONTROL 設定]** ，以開啟「設定」面板。
1. 展開 **[!UICONTROL 展示板]**.
1. 開啟 **[!UICONTROL 將專案動態攝入展示板]**.

   ![輸入欄簡單篩選器選項](assets/intake-column-simple-filters.png)

   輸入欄新增在展示板的左側。 在您套用篩選器之前，該區段會保持空白。

1. （選用）搜尋並選取 [!DNL Workfront] [!UICONTROL **專案**].
1. （選用）搜尋並選取使用者或團隊 [!UICONTROL **指定任務**].
1. 選取 [!UICONTROL **包含已完成的工作**] 以在輸入欄中顯示具有「完成」狀態的任務和問題。

   >[!NOTE]
   >
   >如果未選取此選項，當處於其他狀態的卡片標示為完成時，它們會「脫落」在展示板上，且不再顯示。

1. 按一下 [!UICONTROL **套用**].

   所有物件都會以連線的卡片形式顯示在看板輸入欄中。

   ![輸入欄](assets/intake-column-added3.png)

## 使用進階篩選器建立輸入欄

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](assets/main-menu-icon.png) (位於Adobe Workfront的右上角)，然後按一下 **[!UICONTROL 展示板]**.
1. 存取展示板。 如需詳細資訊，請參閱 [建立或編輯展示板](../../agile/get-started-with-boards/create-edit-board.md).
1. 按一下 **[!UICONTROL 設定]** ，以開啟「設定」面板。
1. 展開 **[!UICONTROL 展示板]**.
1. 開啟 **[!UICONTROL 將專案動態攝入展示板]**.

   輸入欄新增在展示板的左側。 在您套用篩選器之前，該區段會保持空白。

1. 按一下 [!UICONTROL **使用進階篩選**].
1. 按一下 **[!UICONTROL 新增篩選來源]** 並選取 **[!UICONTROL 任務]** 或 **[!UICONTROL 問題]**.

   ![輸入欄進階篩選器選項](assets/intake-column-advanced-filters1.png)

   >[!NOTE]
   >
   >您可以篩選輸入欄以同時包含任務和問題，但您必須為每個物件型別個別設定篩選器。
   >
   >此外，已儲存的篩選器和系統預設篩選器可供您選取。

1. 在篩選器面板上，按一下 **[!UICONTROL 新增篩選器]** 以開始使用。

   ![按一下新增篩選器](assets/intake-filter-dialog5.png)

1. 建立您的篩選器，然後按一下 **[!UICONTROL 另存新檔]**.

   ![篩選產生器](assets/intake-filter-dialog6.png)

   此範例顯示特定專案中處於以下狀態之任務的篩選器： [!UICONTROL 新增] 或 [!UICONTROL 進行中].

   >[!NOTE]
   >
   >建議不要在面板篩選器上使用「我」（已登入的使用者）萬用字元，因為不保證會一律顯示已登入使用者的任務或問題。 設定包含正確任務和問題的展示板後，您可以篩選展示板以顯示特定受指派人的專案。 如需詳細資訊，請參閱 [在展示板中篩選和搜尋](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

   如需建立篩選的詳細資訊，請參閱文章中的「在標準產生器中建立或編輯篩選」一節 [在中建立或編輯篩選器 [!DNL Adobe Workfront]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

1. 命名篩選器並按一下 **[!UICONTROL 儲存]**.

   ![輸入篩選的名稱](assets/intake-filter-dialog7.png)

   為篩選器指定唯一名稱可讓您稍後搜尋。

1. 該篩選器會出現在您儲存的篩選器清單中，並自動套用至輸入欄。 按一下篩選器面板頂端的X以將其關閉。

   ![已儲存的篩選器](assets/intake-filter-dialog8.png)

1. （可選）若要與其他人共用篩選，請將游標移至已儲存的篩選上，按一下 **[!UICONTROL 更多]** 功能表 ![更多選單圖示](assets/more-icon-spectrum.png)，並選取 **[!UICONTROL 共用]**. 在「篩選器」共用方塊中，選擇要共用的使用者或團隊。 如需詳細資訊，請參閱 [共用篩選、檢視或分組](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).
1. （選用）若要在輸入欄中同時包含任務和問題，請按一下 **[!UICONTROL 篩選來源]** 並選取其他物件以建立另一個濾鏡。
1. 新增完篩選器後，請檢閱輸入欄，確認顯示正確的任務和問題。

   ![輸入欄](assets/intake-column-added3.png)

   >[!NOTE]
   >
   >您可以隨時更新篩選器，方法是開啟「設定」面板，按一下 **[!UICONTROL 篩選來源]**，並選取 **[!UICONTROL 任務]** 或 **[!UICONTROL 問題]**.

## 使用輸入欄

您必須將輸入欄中的卡片移至其他展示板欄，才能對其進行編輯。 您可以按一下卡片，以唯讀檢視開啟它，或按一下 ![開啟任務或問題](assets/boards-launch-icon.png) 在新的瀏覽器標籤中開啟任務或問題。

您可以手動重新排序輸入欄上的專案。

攝入欄右上角的圖示會顯示欄中目前有多少卡片，以及已套用多少篩選器。

1. （選用）若要搜尋輸入欄中的專案，請按一下 ![搜尋圖示](assets/search-icon.png) 在欄上。
1. （可選）若要將卡片從輸入欄移入另一欄，請將卡片拖放至您要顯示的位置。

   或

   按一下 **[!UICONTROL 更多]** 功能表 ![更多選單圖示](assets/more-icon-spectrum.png) ，然後選取「 」 **[!UICONTROL 移動]**. 然後，在 **[!UICONTROL 移動專案]** 方塊，選擇另一欄，然後選取 **[!UICONTROL 移動]**.

1. （選用）若要刪除輸入欄，請按一下 **[!UICONTROL 更多]** 功能表 ![更多選單圖示](assets/more-icon-spectrum.png) 並選取 **[!UICONTROL 刪除]**.

