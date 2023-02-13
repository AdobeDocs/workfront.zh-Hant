---
title: 21.4專案增強功能
description: 21.4專案增強功能
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 6bcd332e-bd4e-4a74-bae9-9ba507299a51
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '942'
ht-degree: 0%

---

# 21.4專案增強功能

本頁面說明在「預覽」環境中21.4版本中進行的所有專案增強功能。 這些增強功能將於2021年10月4日當周在生產環境中提供。

如需21.4版所有可用變更的清單，請參閱 [21.4版本概觀](../../../product-announcements/product-releases/21.4-release-activity/21.4-release-overview.md).

## 在更新中包括影像

在物件的「更新」標籤中，您現在可以按一下工具列上的「影像」圖示來新增影像。 您也可以將影像拖放至更新區域。 請注意，您的Workfront管理員必須先啟用新增影像，您才能看到影像圖示。

您可以在更新和回覆中新增影像。 更新中的影像縮圖表示收件者可以在瀏覽器中預覽或下載影像，而電子郵件和應用程式內通知會顯示影像已附加至更新。

以前，在Workfront中共用影像的唯一方法是將影像附加至檔案形式的物件。 在「更新」頁簽上添加的影像僅在該頁簽上可用，而不在「文檔」頁簽上。

如需詳細資訊，請參閱 [更新工作](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

Workfront使用者必須先由Adobe Workfront管理員啟用此功能，才能在更新中加入影像，如 [配置用戶更新的首選項](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).

## 更新智慧指派的演算法

我們改進了智慧分配時使用的算法。 透過新的改善，Workfront會查看登入使用者最近30次進行的指派，以在指派工作和問題時提出建議。 建議清單最多可包含50位使用者。

在此增強功能之前，Workfront在建議使用者時，曾考慮父任務上的指派以及與這些指派相關的其他使用者屬性。

有關智慧分配的資訊，請參閱 [智慧分配概述](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

## 從範本建立專案時的新體驗

為了讓您使用Workfront與新的Workfront體驗一致，我們重新設計了從範本建立專案的介面。 使用範本建立專案的功能未變更。 不過，這個新重新設計的介面有幾項改善包括：

* 附加範本資訊前先預覽範本資訊
* 在項目建立過程中將模板添加到收藏夾清單

我們已更新了在「專案」和「範本」區域建立專案時建立專案的介面。

如需資訊， [使用範本建立專案](../../../manage-work/projects/create-projects/create-project-from-template.md).

## 將範本附加至專案的新體驗

>[!NOTE]
>
>此功能僅適用於新的Adobe Workfront體驗。

為了讓您使用Workfront與新的Workfront體驗一致，我們重新設計了將範本附加至專案的介面。 附加範本的功能未變更。 不過，這個新重新設計的介面有一些改進項目，包括：

* 附加範本資訊前先預覽範本資訊
* 在附件過程中將模板添加到收藏夾清單
* 在一個連續頁面中查看管理模板和項目設定的所有選項

如需詳細資訊，請參閱 [將範本附加至專案](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

## 任務的統一持續時間和持續時間單位值

為提供更簡潔且更簡化的使用者體驗，我們已將「持續時間」欄位的值與持續時間單位合併。 在此增強功能之前，時間單位會顯示在「持續時間」欄位之後的個別下拉式欄位中。

除了「任務詳細資訊」、「編輯任務」和「新任務」框中的「持續時間」欄位之外，我們還更新以下欄位以匹配此體驗：

* 進行高級分配時的持續時間欄位
* 建立或編輯任務時調平延遲欄位
* 建立循環任務時的頻率欄位（即將推出）
* 新增前置項時的延遲欄位（即將推出）

如需詳細資訊，請參閱 [編輯任務](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

![](assets/duration-combined-field-350x139.png)

## 停用在專案中新增內嵌問題

為了確保使用者在填寫問題表單以新增問題至專案時提供正確資訊，我們推出了新的設定，可讓您管理他們是否可以內嵌新增問題至專案或其工作。 預設情況下，在「編輯項目」框的新「問題設定」區域中啟用此設定。 停用後，專案的「問題」區段中會顯示「新增更多問題」選項，因此使用者無法在清單中新增任何問題。 使用者仍可使用「問題」區段中的「新問題」選項，或是為專案設定請求佇列，將問題新增至專案。

>[!NOTE]
>
>此設定僅適用於新的Workfront體驗。 使用Workfront Classic的使用者仍可新增問題至專案或其工作，即使使用新Workfront體驗的使用者已針對專案停用此設定亦然。

如需詳細資訊，請參閱 [編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md).

## 核取方塊和選項按鈕的自訂欄位顯示改善

在自訂表單中檢視和選取核取方塊和選項按鈕選項變得更輕鬆，具有許多核取方塊或選項按鈕選項的自訂欄位現在會顯示在頁面的多個欄中。 以前，它們會以單一欄顯示，使用者需要額外捲動才能填寫表單。

這取決於如何定位自定義表單中的欄位 — 如果使用複選框或單選按鈕欄位將另一個欄位放在同一行，則選項可能只有足夠的水準空間顯示在單個列中。

如需填寫自訂表單的相關資訊，請參閱 [在自訂表單欄位中編輯資訊](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

如需在自訂表單中建立核取方塊或選項按鈕欄位的相關資訊，請參閱區段 [建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create) 和 [建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#configur) 在文章中 [建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

