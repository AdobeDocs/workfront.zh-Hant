---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: 管理展示板的欄
description: 依預設，新展示板包含三欄。 您可以新增更多欄、變更欄的順序、重新命名欄，以及刪除任何您不需要的欄。 您也可以定義欄原則。
author: Lisa
feature: Agile
exl-id: a736cdfe-5ddc-4bf4-82a1-a78d16c0d70b
source-git-commit: 040dd446ff2b347dabf8a139feb17fd1a7d50e4e
workflow-type: tm+mt
source-wordcount: '1149'
ht-degree: 0%

---

# 管理展示板的欄

<!-- Audited: 05/2024 -->

依預設，新展示板包含三欄。 您可以新增更多欄、變更欄的順序、重新命名欄，以及刪除任何您不需要的欄。

欄設定包含原則，可讓您定義卡片移至該欄時會發生什麼的選項。

如需在欄中排序卡片的相關資訊，請參閱[在展示板中篩選和搜尋](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md)。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td> <p>新增：投稿人或更高版本 </p>
        <p>或</p> 
        <p>目前： [！UICONTROL Request]或以上 </p></td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

## 新增欄到展示板

{{step1-to-boards}}

1. 存取展示板。 如需詳細資訊，請參閱[建立或編輯展示板](../../agile/get-started-with-boards/create-edit-board.md)。
1. 按一下現有資料行右邊的&#x200B;**[!UICONTROL 新增資料行]**。
1. 在新欄中輸入名稱，然後按一下&#x200B;**[!UICONTROL 新增欄]**。

   ![新增欄](assets/boards-add-column.png)

>[!TIP]
>
>若要新增輸入資料行，請參閱[將輸入資料行新增到展示板](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md)。

## 重新排序展示板上的欄

1. 存取展示板。
1. 將欄拖放至正確的順序。 在將欄拖到其他位置之前，請務必選擇欄的頂端。

   ![拖放資料行](assets/boards-dragdropcolumn.png)

## 重新命名展示板欄

1. 存取展示板。
1. 按一下欄名稱，鍵入新名稱，然後按Enter鍵。

   或

   按一下欄上的&#x200B;**[!UICONTROL 更多]**&#x200B;功能表![更多功能表](assets/more-icon-spectrum.png)，然後選取&#x200B;**[!UICONTROL 編輯]**。 在[設定]區域中，在&#x200B;**[!UICONTROL 資料行名稱]**&#x200B;欄位中輸入新名稱，然後按一下&#x200B;**[!UICONTROL 關閉]**。

## 刪除展示板欄

從展示板中刪除欄時，該欄無法復原。

1. 存取展示板。
1. 按一下欄上的&#x200B;**[!UICONTROL 更多]**&#x200B;功能表![更多功能表](assets/more-icon-spectrum.png)，然後選取&#x200B;**[!UICONTROL 刪除]**。

   >[!NOTE]
   >
   >包含卡片（包括已封存的卡片）的欄無法刪除。 如果您嘗試刪除包含卡片的欄，則必須為這些卡片選擇另一欄。

## 顯示卡片計數

您可以使用組態設定來顯示每欄中的卡片數量。

如果您在欄上使用WIP限制，則不會新增個別的卡片計數器。 如需WIP限制的詳細資訊，請參閱[管理展示板上的[!UICONTROL 進行中工作] (WIP)限制](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md)。

1. 存取展示板。
1. 按一下主機板右側的&#x200B;**[!UICONTROL [設定]]**&#x200B;以開啟[設定]面板。
1. 展開&#x200B;**[!UICONTROL 欄]**。
1. 開啟&#x200B;**[!UICONTROL 顯示欄卡片計數]**。

   ![開啟卡片計數器](assets/display-card-count.png)

   卡片計數器會出現在每欄的頂端。

1. 按一下&#x200B;**[!UICONTROL 隱藏設定]**&#x200B;以關閉[!UICONTROL 設定]面板。

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
1. 按一下欄上的&#x200B;**[!UICONTROL 更多]**&#x200B;功能表![更多功能表](assets/more-icon-spectrum.png)，然後選取&#x200B;**[!UICONTROL 編輯]**。

   [!UICONTROL 設定]區域出現。 **[!UICONTROL 資料行名稱]**&#x200B;可讓您知道您正為哪個資料行定義設定。

1. 啟用&#x200B;**[!UICONTROL 自動更新欄位值]**&#x200B;原則，以在卡片移至此欄位時自動變更特定欄位值。

   ![資料行設定與原則](assets/boards-column-policies-enabled.png)

1. （選用）設定卡片狀態的值：

   1. 選取&#x200B;**[!UICONTROL 狀態]**&#x200B;核取方塊。

   1. 選取卡片移至此欄時要套用的狀態。

      資料行](assets/boards-column-status.png)的![狀態

      也會顯示已連線卡片的狀態轉譯選項。 （狀態轉譯不適用於臨時卡。） 這些選項決定在連線的卡片移至此欄時，套用到[!DNL Workfront]中任務或問題的自訂狀態。

   1. 選取&#x200B;[!UICONTROL **自訂**]&#x200B;狀態以套用至任務與問題的卡片。

      將卡片移至此欄時，[!DNL Workfront]會先嘗試套用自訂狀態（例如「已解決」）。 如果該卡片無法使用選取的自訂狀態，系統會提示您選擇與系統狀態相對應的其他狀態（從上面的步驟b）。 如需狀態的詳細資訊，請參閱[狀態概觀](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md)。

      此外，如果所連線任務或問題的狀態變更為欄原則中設定的自訂或系統狀態，卡片將自動移動到欄。

1. （選用）為卡片受指派人設定值：

   1. 選取&#x200B;**[!UICONTROL 被指定者]**&#x200B;核取方塊。
   1. 選取動作。

      * **[!UICONTROL 新增至受指派人]：**&#x200B;您選取的受指派人在卡片移至此欄位時，會新增至卡片上的現有受指派人清單。
      * **[!UICONTROL 覆寫受指派人]：**&#x200B;您選取的受指派人覆寫所有其他受指派人，並在卡片移至此欄位時成為卡片上的唯一受指派人。

   1. 按一下&#x200B;[!UICONTROL **新增工作分派**]&#x200B;並搜尋使用者。 從搜尋結果中選取受指派人。 所有Workfront使用者和團隊都可供選擇。

      ![欄](assets/boards-column-assignees.png)的被指定者

1. （選用）設定卡片標籤的值：

   1. 選取&#x200B;**[!UICONTROL 卡片]**&#x200B;核取方塊。
   1. 選取動作。

      * **[!UICONTROL 新增至標籤]：**&#x200B;當您選取的標籤移至此欄時，會新增至卡片上的現有標籤清單。
      * **[!UICONTROL 覆寫標籤]：**&#x200B;您選取的標籤會覆寫所有其他標籤，並在卡片移至此欄位時成為卡片上的唯一標籤。

   1. 從下拉式清單中選取標籤。 只有已在[!UICONTROL 標籤管理員]中建立的標籤才可供選擇。 如需新增標籤的相關資訊，請參閱[新增標籤](/help/quicksilver/agile/get-started-with-boards/add-tags.md)。

      資料行](assets/boards-column-tags.png)的![標籤

1. 啟用&#x200B;**[!UICONTROL 進行中工作限制]**&#x200B;原則以限制可新增到資料行的卡片數量。 然後，在&#x200B;**[!UICONTROL 設定限制]**&#x200B;欄位中輸入限制數字。

   ![欄](assets/boards-wip-limit-in-column.png)的WIP限制

   如需詳細資訊，請參閱[管理主機板上的進行中工作(WIP)限制](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md)。

1. 按一下&#x200B;**[!UICONTROL 關閉]**&#x200B;以結束[設定]區域並檢視資料行及其卡片。
