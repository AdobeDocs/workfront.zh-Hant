---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: 管理展示板的欄
description: 依預設，新展示板包含三欄。 您可以新增更多欄、變更欄的順序、重新命名欄，以及刪除任何您不需要的欄。
author: Lisa
feature: Agile
exl-id: a736cdfe-5ddc-4bf4-82a1-a78d16c0d70b
source-git-commit: 99eaafe4b2143f0e29bf677904c1caa8a19d5192
workflow-type: tm+mt
source-wordcount: '1149'
ht-degree: 0%

---

# 管理展示板的欄

依預設，新展示板包含三欄。 您可以新增更多欄、變更欄的順序、重新命名欄，以及刪除任何您不需要的欄。

欄設定包含原則，可讓您定義卡片移至該欄時會發生什麼的選項。

如需在欄中排序卡片的相關資訊，請參閱 [在展示板中篩選和搜尋](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

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

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 新增欄到展示板

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![](assets/main-menu-icon.png) 位於的右上角 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 展示板]**.
1. 存取展示板。 如需詳細資訊，請參閱 [建立或編輯展示板](../../agile/get-started-with-boards/create-edit-board.md).
1. 按一下 **[!UICONTROL 新增欄]** 位於現有欄的右側。
1. 在新欄中輸入名稱，然後按一下 **[!UICONTROL 新增欄]**.

   ![新增欄](assets/boards-add-column.png)

>[!TIP]
>
>若要新增輸入欄，請參閱 [將輸入欄新增到展示板](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## 重新排序展示板上的欄

1. 存取展示板。
1. 將欄拖放至正確的順序。 在將欄拖到其他位置之前，請務必選擇欄的頂端。

   ![拖放欄](assets/boards-dragdropcolumn.png)

## 重新命名展示板欄

1. 存取展示板。
1. 按一下欄名稱，鍵入新名稱，然後按Enter鍵。

   或

   按一下 **[!UICONTROL 更多]** 功能表 ![更多選單](assets/more-icon-spectrum.png) 在欄上並選取 **[!UICONTROL 編輯]**. 在「設定」區域中，於 **[!UICONTROL 欄名稱]** 欄位，然後按一下 **[!UICONTROL 關閉]**.

## 刪除展示板欄

從展示板中刪除欄時，該欄無法復原。

1. 存取展示板。
1. 按一下 **[!UICONTROL 更多]** 功能表 ![更多選單](assets/more-icon-spectrum.png) ，然後選取「 」 **[!UICONTROL 刪除]**.

   >[!NOTE]
   >
   >包含卡片（包括已封存的卡片）的欄無法刪除。 如果您嘗試刪除包含卡片的欄，則必須為這些卡片選擇另一欄。

## 顯示卡片計數

您可以使用組態設定來顯示每欄中的卡片數量。

如果您在欄上使用WIP限制，則不會新增個別的卡片計數器。 如需在製品限制的詳細資訊，請參閱 [管理 [!UICONTROL 工作進行中] (WIP)主機板限制](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md).

1. 存取展示板。
1. 按一下 **[!UICONTROL 設定]** ，以開啟「設定」面板。
1. 展開 **[!UICONTROL 欄]**.
1. 開啟 **[!UICONTROL 顯示欄卡片計數]**.

   ![開啟卡片計數器](assets/display-card-count.png)

   卡片計數器會出現在每欄的頂端。

1. 按一下 **[!UICONTROL 隱藏設定]** 以關閉 [!UICONTROL 設定] 面板。

## 定義欄設定和原則

欄原則包括自動更新欄位值，以及設定進行中的工作限制。

更新狀態的原則會自動對卡片和欄生效：

* 當卡片移至具有原則的欄時，卡片狀態會更新為原則中定義的狀態。 這同時適用於ad hoc和連線的卡片。
* 當卡片上的臨機操作或已連線卡片狀態更新以符合原則中的欄狀態時，或連線卡片狀態更新到Workfront中的其他位置時，卡片會自動移動到該欄。 此外，如果卡片上的自訂狀態符合指派給欄的系統狀態，則卡片會移至該欄。

如果卡片狀態不符合任何現有欄原則中設定的任何狀態，則卡片將保留在放置它的欄中。

>[!NOTE]
>
>動態展示板總是將卡片放置在與其狀態相符的欄中，無論欄原則是啟用還是停用。 當您重新整理展示板時，卡片將返回其指派的欄。
> 
>此外，對於所有展示板型別，如果您將卡片從一欄移動到另一欄具有相同狀態，當您重新整理展示板時，卡片將返回到原始欄。

1. 存取展示板。
1. 按一下 **[!UICONTROL 更多]** 功能表 ![更多選單](assets/more-icon-spectrum.png) ，然後選取「 」 **[!UICONTROL 編輯]**.

   此 [!UICONTROL 設定] 區域隨即顯示。 此 **[!UICONTROL 欄名稱]** 讓您知道要為哪一欄定義設定。

1. 啟用 **[!UICONTROL 自動更新欄位值]** 將卡片移至此欄時自動變更特定欄位值的原則。

   ![欄設定和原則](assets/boards-column-policies-enabled.png)

1. （選用）設定卡片狀態的值：

   1. 選取 **[!UICONTROL 狀態]** 核取方塊。

   1. 選取卡片移至此欄時要套用的狀態。

      ![欄的狀態](assets/boards-column-status.png)

      也會顯示已連線卡片的狀態轉譯選項。 （狀態轉譯不適用於臨時卡。） 這些選項決定套用至中任務或問題的自訂狀態 [!DNL Workfront] 將已連線的卡片移至此欄時。

   1. 選取 [!UICONTROL **自訂**] 要套用至任務卡和問題的狀態。

      將卡片移至此欄時， [!DNL Workfront] 會先嘗試套用自訂狀態（例如「已解決」）。 如果該卡片無法使用選取的自訂狀態，系統會提示您選擇與系統狀態相對應的其他狀態（從上面的步驟b）。 如需狀態的詳細資訊，請參閱 [狀態概觀](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

      此外，如果所連線任務或問題的狀態變更為欄原則中設定的自訂或系統狀態，卡片將自動移動到欄。

1. （選用）為卡片受指派人設定值：

   1. 選取 **[!UICONTROL 被指定者]** 核取方塊。
   1. 選取動作。

      * **[!UICONTROL 新增至受指派人]：** 當您將受指派人移至此欄時，您選取的受指派人會新增至卡片上的現有受指派人清單中。
      * **[!UICONTROL 覆寫受指派人]：** 您選取的受指派人會覆寫所有其他的受指派人，並在卡片移至此欄位時，成為卡片上的唯一受指派人。

   1. 按一下 [!UICONTROL **新增指定任務**] 和搜尋使用者。 從搜尋結果中選取受指派人。 所有Workfront使用者和團隊都可供選擇。

      ![欄的受指派人](assets/boards-column-assignees.png)

1. （選用）設定卡片標籤的值：

   1. 選取 **[!UICONTROL 卡片]** 核取方塊。
   1. 選取動作。

      * **[!UICONTROL 新增到標籤上]：** 當卡片移至此欄時，您選取的標籤會新增至卡片上的現有標籤清單中。
      * **[!UICONTROL 覆寫標籤]：** 您選取的標籤會覆寫所有其他標籤，並在卡片移至此欄時，成為卡片上的唯一標籤。

   1. 從下拉式清單中選取標籤。 僅已在中建立的標籤 [!UICONTROL 標籤管理員] 可供選擇。 如需新增標籤的詳細資訊，請參閱 [新增標籤](/help/quicksilver/agile/get-started-with-boards/add-tags.md).

      ![欄的標籤](assets/boards-column-tags.png)

1. 啟用 **[!UICONTROL 創作中的作品限制]** 限制可新增到欄中的卡片數量原則。 然後，在 **[!UICONTROL 設定限制]** 欄位。

   ![欄的WIP限制](assets/boards-wip-limit-in-column.png)

   如需詳細資訊，請參閱 [管理展示板上的進行中工作(WIP)限制](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md).

1. 按一下 **[!UICONTROL 關閉]** 以結束「設定」區域並檢視欄及其卡片。
