---
title: 23.1敏捷增強功能
description: 23.1敏捷增強功能
author: Courtney
draft: Probably
feature: Product Announcements
exl-id: 4bd041a5-a6e3-4fe3-ae23-45980701e904
source-git-commit: f0e21f9b2846c5665474903a2910ce9f41cdf810
workflow-type: tm+mt
source-wordcount: '882'
ht-degree: 0%

---

# 23.1敏捷增強功能

本頁說明在「預覽」環境中23.1版所進行的所有敏捷增強功能。 這些增強功能將於2023年1月16日當周在生產環境中提供。

如需23.1版所有可用變更的清單，請參閱 [23.1版本概觀](/help/quicksilver/product-announcements/product-releases/23.1-release-activity/23-1-release-overview.md).

## Workfront展示板的掃描規劃

Adobe Workfront展示板中新的Scrum規劃功能提供彈性的選項，以管理您敏捷的流程。 使用這些工具，您可以：

* 在迭代或約束中跟蹤工作
* 使用velocity來指導團隊承諾
* 跟蹤燃耗和完成率

第23.1發行版本後，Scrum規劃功能將是「快速跟進」。

## 卡片的到期日對應至Workfront物件的計畫完成日期

>[!NOTE]
>
>只有透過Workfront展示板的早期功能選擇，才能使用此功能。

Workfront主板中連線卡的到期日現在對應至關聯Workfront物件的計畫完成日期。 如果更新卡上的到期日，則計畫完成日期將在任務或問題上更新。 變更計畫完成日期也會變更卡片上的到期日。 之前，卡片到期日是手動輸入，未對應至任務或問題上的任何日期。

日期對應也適用於同步至子任務的已連線檢查清單項目。

連線卡和臨機卡的到期日現在也包含時間欄位。

如需詳細資訊，請參閱 [在主板上使用連接的卡](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

[觀看此功能的影片示範](https://video.tv.adobe.com/v/3411952/){target=_blank}

## 現在已連結展示板檢查清單項目和Workfront子任務

>[!NOTE]
>
>只有透過Workfront展示板的早期功能選擇，才能使用此功能。

當您將已連線的資訊卡新增至Workfront工作的展示板時，任何子任務都會匯入為資訊卡上的檢查清單項目。 此外，當您在連線的資訊卡上建立檢查清單項目時，會將子任務新增至Workfront任務。 問題的檢查清單項目未與任何Workfront物件連結。

以前未連結檢查清單項目和子任務。 如果您想在展示板上包含子任務，可以將其作為單獨的連接卡導入，或手動將檢查清單項添加到資訊卡。

如需詳細資訊，請參閱 [在主板上使用連接的卡](/help/quicksilver/agile/get-started-with-boards/connected-cards.md) 和 [管理卡上的檢查清單項目](/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md).

[觀看此功能的影片示範](https://video.tv.adobe.com/v/3411951/){target=_blank}

## 板上的卡計數器

>[!NOTE]
>
>只有透過Workfront展示板的早期功能選擇，才能使用此功能。

新的組態設定可用來開啟展示板上所有欄的卡片計數器。 如果您在欄上使用WIP限制，則不會新增個別的卡片計數器。

如需詳細資訊，請參閱 [管理展示板欄](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).

## 在展示板控制面板上搜尋及排序

>[!NOTE]
>
>只有透過Workfront展示板的早期功能選擇，才能使用此功能。

您現在可以依展示板名稱或日期來排序展示板控制面板，並在清單中搜尋特定展示板。

如需詳細資訊，請參閱 [使用展示板控制面板](/help/quicksilver/agile/get-started-with-boards/use-boards-page.md).

## 狀態會顯示在資訊卡上

>[!NOTE]
>
>只有透過Workfront展示板的早期功能選擇，才能使用此功能。

如果展示板上的資訊卡獲派狀態，狀態現在會顯示在資訊卡上，因此您不必開啟資訊卡即可查看狀態。 此增強功能適用於臨機和已連線的資訊卡。

如需詳細資訊，請參閱 [在主板上使用連接的卡](/help/quicksilver/agile/get-started-with-boards/connected-cards.md) 和 [新增臨機卡至展示板](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md).

![卡片狀態](/help/quicksilver/product-announcements/product-releases/assets/boards-connected-card-details-110922.png)

## 可連結卡現在可在板上使用

>[!NOTE]
>
>只有透過Workfront展示板的早期功能選擇，才能使用此功能。

您現在可以將特定資訊卡的連結傳送給其他展示板使用者。 人員必須擁有檢視展示板的存取權，才能開啟連結。

當您在展示板上開啟資訊卡時，瀏覽器URL看起來會像這樣：

```
https://<Workfront-URL>/boards/<board-id>/card/<card-id>. 
```

您可以複製完整的URL並傳送給其他人。 當使用者存取連結時，會直接前往開啟的資訊卡。

過去，展示板可使用連結，但無法使用特定資訊卡。

如需資訊卡，請參閱 [新增臨機卡至展示板](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md) 和 [在主板上使用連接的卡](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## 在展示板上依連線篩選

>[!NOTE]
>
>只有透過Workfront展示板的早期功能選擇，才能使用此功能。

展示板上的篩選器清單現在包含可依連線篩選的選項，可顯示特定專案的所有已連線卡片。 您也可以依未連線的卡片來篩選。

如需詳細資訊，請參閱 [在展示板中篩選和搜尋](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

[觀看此功能的影片示範](https://video.tv.adobe.com/v/3412381/){target=_blank}

## 依排程從展示板封存資訊卡

>[!NOTE]
>
>只有透過Workfront展示板的早期功能選擇，才能使用此功能。

您可以設定展示板，讓資訊卡依排程封存或「流失」展示板。 可使用選項在特定欄中設定卡片，以在特定天數或周內封存。 例如，您可以定義衰退，讓「完成」欄中的卡片在欄中存放兩週後即進行封存。

如果您想在資訊卡從展示板掉下來後再次顯示，您可以設定展示板篩選來顯示已封存的資訊卡。

如需詳細資訊，請參閱 [設定卡片流失](/help/quicksilver/agile/use-boards-agile-planning-tools/configure-card-falloff.md).

[觀看此功能的影片示範](https://video.tv.adobe.com/v/3412323/){target=_blank}
