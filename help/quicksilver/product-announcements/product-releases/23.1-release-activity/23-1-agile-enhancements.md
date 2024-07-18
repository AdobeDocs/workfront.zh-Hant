---
title: 23.1敏捷增強功能
description: 23.1敏捷增強功能
author: Courtney
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4bd041a5-a6e3-4fe3-ae23-45980701e904
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '889'
ht-degree: 0%

---

# 23.1敏捷增強功能

本頁說明預覽環境的23.1版本所做的所有敏捷增強功能。 這些增強功能將在2023年1月16日當週的生產環境中提供。

如需23.1版本可用的所有變更清單，請參閱[23.1版本總覽](/help/quicksilver/product-announcements/product-releases/23.1-release-activity/23-1-release-overview.md)。

## Workfront主機板的Scrum規劃

Adobe Workfront展示板中的新Scrum規劃功能提供彈性選項，可管理您的敏捷流程。 使用這些工具，您可以：

* 追蹤反複專案或衝刺中的工作
* 使用Velocity引導團隊承諾
* 追蹤待執行工作及完成率

在23.1版發行後，Scrum規劃功能將是「快速跟隨」。

## 卡片上的到期日對應至Workfront物件上的計畫完成日期

>[!NOTE]
>
>此功能只能透過Workfront展示板的早期功能選擇加入來使用。

Workfront面板中連線卡片的到期日現在對應至關聯Workfront物件上的計畫完成日期。 如果您更新卡片上的到期日，則任務或問題上的計畫完成日期會更新。 變更計畫完成日期也會變更卡上的到期日。 以往，卡片到期日是手動輸入，未對應至任務或問題的任何日期。

日期對應也會套用至同步至子任務的已連線檢查清單專案。

連線的卡片和臨機卡片上的到期日期現在也包含時間欄位。

如需詳細資訊，請參閱[使用主機板上的連線卡](/help/quicksilver/agile/get-started-with-boards/connected-cards.md)。

[觀看此功能的影片示範](https://video.tv.adobe.com/v/3411952/){target=_blank}

## 展示板檢查清單專案和Workfront子任務現在已連結

>[!NOTE]
>
>此功能只能透過Workfront展示板的早期功能選擇加入來使用。

當您為Workfront任務將連線的卡片新增到展示板時，任何子任務都會匯入為卡片上的清單專案。 此外，當您在已連線的卡片上建立檢查清單專案時，子任務會新增到Workfront任務中。 問題的清單專案未連線至任何Workfront物件。

以前檢查清單專案和子任務未連結。 如果您想在展示板上加入子任務，您可以將它匯入為個別的連線卡片，或手動將檢查清單專案新增到卡片。

如需詳細資訊，請參閱[在面板上使用連線的卡片](/help/quicksilver/agile/get-started-with-boards/connected-cards.md)和[管理卡片上的檢查清單專案](/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md)。

[觀看此功能的影片示範](https://video.tv.adobe.com/v/3411951/){target=_blank}

## 展示板欄上的卡片計數器

>[!NOTE]
>
>此功能只能透過Workfront展示板的早期功能選擇加入來使用。

有新的組態設定可開啟展示板上所有欄的卡片計數器。 如果您在欄上使用WIP限制，則不會新增個別的卡片計數器。

如需詳細資訊，請參閱[管理主機板資料行](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md)。

## 在面板控制面板上搜尋和排序

>[!NOTE]
>
>此功能只能透過Workfront展示板的早期功能選擇加入來使用。

您現在可以依展示板名稱或日期來排序展示板，並在清單中搜尋特定展示板。

如需詳細資訊，請參閱[使用面板儀表板](/help/quicksilver/agile/get-started-with-boards/use-boards-page.md)。

## 狀態會顯示在卡片上

>[!NOTE]
>
>此功能只能透過Workfront展示板的早期功能選擇加入來使用。

如果展示板上的卡片已指派狀態，狀態現在會顯示在卡片上，因此您不必開啟卡片即可檢視狀態。 此增強功能同時適用於ad hoc卡和連線卡。

如需詳細資訊，請參閱[在展示板上使用連線的卡片](/help/quicksilver/agile/get-started-with-boards/connected-cards.md)和[將臨機操作卡片新增到展示板](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md)。

卡片上的![狀態](/help/quicksilver/product-announcements/product-releases/assets/boards-connected-card-details-110922.png)

## 可連結卡現在可在展示板上使用

>[!NOTE]
>
>此功能只能透過Workfront展示板的早期功能選擇加入來使用。

您現在可以將特定卡片的連結傳送給其他看板使用者。 此人必須擁有檢視展示板的存取權，才能開啟連結。

當您在展示板上開啟卡片時，瀏覽器URL看起來像這樣：

```
https://<Workfront-URL>/boards/<board-id>/card/<card-id>. 
```

您可以複製完整的URL並傳送給其他人。 使用者存取連結時，會直接前往開啟的卡片。

以前展示板有連結，但特定卡片沒有連結。

如需有關卡片的資訊，請參閱[將臨機卡片新增到展示板](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md)和[使用展示板上連線的卡片](/help/quicksilver/agile/get-started-with-boards/connected-cards.md)。

## 在面板上依連線篩選

>[!NOTE]
>
>此功能只能透過Workfront展示板的早期功能選擇加入來使用。

展示板上的篩選器清單現在包含依連線篩選的選項，這會顯示特定專案的所有已連線卡片。 您也可以依未連線的卡片進行篩選。

如需詳細資訊，請參閱[在展示板中篩選和搜尋](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md)。

[觀看此功能的影片示範](https://video.tv.adobe.com/v/3412381/){target=_blank}

## 依排程從展示板封存卡片

>[!NOTE]
>
>此功能只能透過Workfront展示板的早期功能選擇加入來使用。

您可以設定展示板，讓卡片可依排程封存或「脫落」展示板。 選項可用於在特定欄中設定卡片，以在特定天數或周數中封存。 例如，您可以定義減少，讓完整欄中的卡片在欄中停留兩週後封存。

如果您想在卡片從展示板掉落後再次顯示卡片，您可以將展示板篩選器設定為顯示已封存的卡片。

如需詳細資訊，請參閱[設定卡片縮減](/help/quicksilver/agile/use-boards-agile-planning-tools/configure-card-falloff.md)。

[觀看此功能的影片示範](https://video.tv.adobe.com/v/3412323/){target=_blank}
