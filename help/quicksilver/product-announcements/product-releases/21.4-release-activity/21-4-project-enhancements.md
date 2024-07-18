---
title: 21.4專案增強功能
description: 21.4專案增強功能
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6bcd332e-bd4e-4a74-bae9-9ba507299a51
source-git-commit: dd718ff8f497065018cdfb9592ff0804d7668bf8
workflow-type: tm+mt
source-wordcount: '911'
ht-degree: 0%

---

# 21.4專案增強功能

本頁說明21.4版對預覽環境所做的所有專案增強功能。 這些增強功能將在2021年10月4日當週的生產環境中提供。

如需21.4版本可用的所有變更清單，請參閱[21.4版本總覽](../../../product-announcements/product-releases/21.4-release-activity/21-4-release-overview.md)。

## 在更新中包含影像

在物件的「更新」標籤上，您現在可以按一下工具列上的「影像」圖示來新增影像。 您也可以將影像拖放至更新區域。 請注意，您必須先啟用Workfront管理員新增影像，才能看到影像圖示。

您可以在更新與回覆中新增影像。 更新中的影像縮圖表示收件者可以在瀏覽器中預覽或下載影像，而電子郵件和應用程式內通知會顯示影像已附加至更新。

之前，在Workfront中共用影像的唯一方式是將影像作為檔案附加至物件。 在「更新」標籤上新增的影像只能在該標籤上使用，不能在「檔案」標籤上使用。

如需詳細資訊，請參閱[更新工作](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)。

在Workfront使用者可以在更新中包含影像之前，此功能必須先由Adobe Workfront管理員啟用，如[設定使用者更新的偏好設定](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md)中所述。

## 已更新智慧型指派的演演算法

我們已改善進行智慧型指派時使用的演演算法。 透過新的改進，Workfront會檢視登入使用者最近進行的30個指派，以在他們指派任務和問題時提供建議。 建議清單最多可包含50位使用者。

在此增強功能之前，Workfront在建議使用者時，會考慮父系任務上的指派以及與這些指派相關的其他使用者屬性。

如需智慧指派的相關資訊，請參閱[智慧指派總覽](../../../manage-work/tasks/assign-tasks/smart-assignments.md)。

## 從範本建立專案時的新體驗

為了讓您使用Workfront與新的Workfront體驗一致，我們重新設計了介面，用於從範本建立專案。 使用範本建立專案的功能並未變更。 不過，這個全新重新設計的介面有以下幾項改善專案：

* 附加範本資訊之前先預覽範本資訊
* 在專案建立過程中將範本新增至我的最愛清單

當您從專案和範本區域建立專案時，我們已更新用於建立專案的介面。

如需詳細資訊，[使用範本](../../../manage-work/projects/create-projects/create-project-from-template.md)建立專案。

## 將範本附加到專案時的新體驗

>[!NOTE]
>
>此功能僅在新的Adobe Workfront體驗中可用。

為了讓您使用Workfront與新的Workfront體驗一致，我們重新設計了介面以將範本附加到專案。 附加範本的功能未變更。 不過，這個全新重新設計的介面有一些改良功能，包括下列專案：

* 附加範本資訊之前先預覽範本資訊
* 在附件程式期間將範本新增至我的最愛清單
* 在一個連續頁面中檢視用於管理範本和專案設定的所有選項

如需詳細資訊，請參閱[將範本附加至專案](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md)。

## 任務的統一持續時間和持續單位值

為了提供更乾淨且更精簡的使用者體驗，我們已將「持續時間」欄位的值與持續時間單位合併。 在此增強功能之前，時間單位會顯示在持續時間欄位後面的個別下拉式欄位中。

除了「任務詳細資訊」、「編輯任務」和「新任務」方塊中的「工期」欄位外，我們也會更新下列欄位以符合此體驗：

* 進行進階指派時的期間欄位
* 建立或編輯任務時平準延遲欄位
* 建立週期性任務時的頻率欄位（即將推出）
* 新增前置任務時的延遲欄位（即將推出）

如需詳細資訊，請參閱[編輯工作](../../../manage-work/tasks/manage-tasks/edit-tasks.md)。

![](assets/duration-combined-field-350x139.png)

## 停用在專案上新增內嵌問題

為確保使用者完成問題表單以將問題新增至專案時可提供準確資訊，我們引入了一項新設定，可讓您管理使用者是否可以將問題新增至專案或其內嵌任務。 此設定預設在編輯專案方塊的新問題設定區域中啟用。 若停用此專案，專案問題區段中的新增更多問題選項會變暗，因此使用者無法在清單中新增任何其他問題。 使用者仍然可以透過使用問題區段中的新問題選項或使用請求佇列（如果為專案配置了請求佇列）將問題新增到專案。

>[!NOTE]
>
>此設定僅在新的Workfront體驗中可用。 即使使用新Workfront體驗的使用者已針對專案停用此設定，使用Workfront Classic的使用者仍可在專案或其任務中新增內嵌問題。

如需詳細資訊，請參閱[編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md)。

## 核取方塊和選項按鈕的自訂欄位顯示改善

在自訂表單中檢視及選取核取方塊和選項按鈕選項變得更加容易 — 包含許多核取方塊或選項按鈕選項的自訂欄位現在顯示在頁面的多個欄中。 以前，它們會顯示在單一欄中，使用者填寫表單時需要進行額外的捲動。

這取決於您在自訂表單中放置欄位的方式 — 如果您將另一個欄位與核取方塊或選項按鈕欄位放在同一列，則選項可能只有足夠的水準空間可顯示在單一欄中。

如需填寫自訂表單的相關資訊，請參閱[編輯自訂表單欄位中的資訊](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md)。

