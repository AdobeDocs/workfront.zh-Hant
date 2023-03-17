---
title: 23.2敏捷增強功能
description: 23.2敏捷增強功能
author: Courtney
draft: Probably
feature: Product Announcements
source-git-commit: 456794da11baf21bcd4f138d15719007ae2759a6
workflow-type: tm+mt
source-wordcount: '1121'
ht-degree: 0%

---

# 23.2敏捷增強功能

本頁說明在「預覽」環境中23.2版所做的所有敏捷增強功能。 這些增強功能將於23.2版的生產環境中提供使用。

如需23.2版本週期中此時所有可用變更的清單，請參閱 [23.2版本概觀](/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-release-overview.md).

## Adobe Workfront展示板中可用的迭代功能

Workfront展示板中提供的數項新功能，讓您能使用靈活的Scrum功能。 這些功能包括：

* 將與同一團隊相關的展示板分組並協作的工作流
* 卡片清單或積壓工作，並可選擇使用來源將卡片連接至Workfront任務和問題
* 迭代規劃和迭代流程板

請注意，集合已重新命名為工作流。 工作流程可協助您以不同方式將資料視覺化。 您可以在清單、展示板或小版本的資訊卡上顯示項目。 工作流中的資訊卡也可在多個展示板之間共用。 您可以使用工作流中的卡片和展示板，輕鬆促進工作流程。

如需詳細資訊，請參閱 [管理工作流](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md), [建立小版本](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration.md)，和 [使用卡片清單](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md). 第二篇文章要等到我發佈分支後，才能在Main中使用。

## 將清單和報表中的任務和問題添加到工作流卡清單

您現在可以直接從清單或報表檢視，將現有工作或問題新增至Workfront展示板中的工作流。 您添加到工作流的任何項目都將作為計畫外卡添加到卡清單中。

如需詳細資訊，請參閱 [將現有任務或問題新增至展示板](/help/quicksilver/agile/get-started-with-boards/add-card-from-list-to-board.md).

## 將自訂欄位新增至展示板上的資訊卡

您現在可以在Adobe Workfront展示板上包含自訂欄位。 欄位必須已在Workfront中建立。 您無法在展示板內設計和建立新的自訂欄位。

和預設欄位一樣，您可以選擇在資訊卡的完整檢視和展示板上的縮合檢視上顯示自訂欄位。

卡片上自訂欄位的任何資料都為唯讀。

如需詳細資訊，請參閱 [自訂卡片上顯示的欄位](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

## 將清單和報表中的工作和問題新增至Workfront展示板

您現在可以直接從清單或報表檢視，將現有工作或問題新增至Workfront展示板。 您新增至展示板的任何項目都會變成已連線的資訊卡。

此外，「展示板」欄位現在可新增至任務或問題的清單和報表。 此欄位會顯示已新增任務或問題的所有展示板。

如需詳細資訊，請參閱 [將現有任務或問題新增至展示板](/help/quicksilver/agile/get-started-with-boards/add-card-from-list-to-board.md).


## 登錄主板上連接的卡的時數

>[!NOTE]
>
>只有透過Workfront展示板的早期功能選擇，才能使用此功能。

您現在可以在連線卡上登錄數小時，就像處理任務或問題時一樣。 您必須擁有任務或問題的正確權限才能記錄時間。

依預設，連線的卡片上不會顯示時間記錄欄位。 您必須啟用 **小時** 在「卡片」下的「配置」區域中。

如需詳細資訊，請參閱 [在主板上使用連接的卡](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).


## 自訂卡片上的欄位顯示

>[!NOTE]
>
>只有透過Workfront展示板的早期功能選擇，才能使用此功能。


現在可自訂，以設定卡片上顯示的欄位，包括卡片開啟時的完整檢視，以及展示板上的縮合卡片檢視。 當您停用欄位時，兩個檢視中都不會顯示。 您也可以啟用完整檢視中的欄位，並在縮合檢視中隱藏該欄位。

如需詳細資訊，請參閱 [自訂卡片上顯示的欄位](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

[觀看此功能的影片示範](https://video.tv.adobe.com/v/3415710/){target=_blank}

## 為移入展示板欄的資訊卡定義預設狀態

>[!NOTE]
>
>只有透過Workfront展示板的早期功能選擇，才能使用此功能。

您現在可以在欄原則中選取自訂狀態和系統狀態，以設定預設狀態，以套用至移入特定欄的卡。 當您將資訊卡移入欄中時，Workfront會先嘗試套用自訂狀態（例如「等待意見」）。 如果自訂狀態不適用於該卡片，Workfront會改用系統狀態（例如「暫掛」）。 此外，如果連接任務或問題的狀態更改為列策略中設定的自定義或系統狀態，則卡會自動移到列。

以前，如果有多種狀態可用，系統會提示您為每個移至欄的卡片選取狀態。

如需詳細資訊，請參閱 [管理欄](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).

[觀看此功能的影片示範](https://video.tv.adobe.com/v/3415711/){target=_blank}

## 集合現在可在Adobe Workfront展示板中使用

>[!NOTE]
>
>只有透過Workfront展示板的早期功能選擇，才能使用此功能。

您現在可以在展示板控制面板上建立集合。 集合是一組用於協作工作的委員會。 為系列命名後，您可以使用一組範本將展示板新增至系列，這些範本提供預先定義的設定，例如欄名稱。 您也可以將獨立展示板移入集合中。 展示板在系列中後，可以移至其他系列，但無法變成獨立展示板。

將成員新增至集合的運作方式與將成員新增至展示板相同。 人員或團隊必須是集合的成員，才能在集合的展示板中將其新增為成員。

如需詳細資訊，請參閱 [管理集合](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md).

[觀看此功能的影片示範](https://video.tv.adobe.com/v/3415609/){target=_blank}

## 連接卡上的估計欄位映射到Workfront對象上的「文章點」欄位

>[!NOTE]
>
>只有透過Workfront展示板的早期功能選擇，才能使用此功能。

Workfront展示板中連線卡片上的「估計」欄位現在對應至相關聯Workfront物件的「動態點」欄位。

新的「動態點」欄位是可編輯、自由的表單欄位，您可將其新增至清單中的檢視，或新增至報表中，以了解工作或問題。 它不與計畫小時數或團隊分配相關聯。

之前，卡片估計是手動輸入，未對應至任務或問題上的任何欄位。

此外，臨機卡和已連線卡上的「估計」欄位不再有字元限制。 過去，字元數上限為99。

如需詳細資訊，請參閱 [在主板上使用連接的卡](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## 進氣列中的預覽卡

>[!NOTE]
>
>只有透過Workfront展示板的早期功能選擇，才能使用此功能。

您現在可以按一下進入欄中的已連線卡片，以查看其內容僅限檢視的版本。 在資訊卡從進入欄移出到展示板上的其他欄之前，您無法編輯資訊卡內容。
