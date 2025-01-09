---
title: 2025年第一季度管理員增強功能
description: 2025年第一季度管理員增強功能
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: fa24040d-0403-4799-b690-c3d172797115
source-git-commit: d2e3379e9390f2b419bb2d78b1999c8c2dd7d0d3
workflow-type: tm+mt
source-wordcount: '744'
ht-degree: 0%

---

# 2025年第一季度管理員增強功能

本頁說明2025年第一季度版本對「預覽」環境所做的所有管理員增強功能。 如上所述，這些增強功能將於生產環境中提供。

如需2025年第一季發行週期目前可用的所有變更清單，請參閱[2025年第一季發行概觀](/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-release-overview.md)。

## 比較不同環境之間的物件以進行環境升級

>[!NOTE]
>
>預覽版本： 2024年1月6日；適用於所有客戶的生產版本：搭配25.1版（2025年1月）

為了更便於確定哪些物件應包含在環境推進套件中，我們新增了跨環境比較物件的功能。 現在，您可以選取物件型別和環境。 Workfront會產生該型別物件的清單，包括它們是否存在於目標環境中，以及該物件在來源環境與目標環境之間是否有差異。 然後，您可以從此清單直接將物件加入封裝。

以前，如果使用者想要比較環境之間的物件，他們必須手動檢查這些物件。

如需詳細資訊，請參閱[比較環境間的物件](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-compare.md)。

## 更多可用於環境升級的物件

>[!NOTE]
>
>預覽版本： 2024年1月6日；適用於所有客戶的生產版本：搭配25.1版（2025年1月）

為了擴展環境推進功能的功能，我們已新增更多物件。 現在，您可以將下列物件加入至環境推進封裝：

* 位置
* 費率卡
* 指派

以前，這些物件無法用於環境升級。

如需有關可用於環境推進的物件的詳細資訊，請參閱「環境推進概述」一文中的[環境推進的支援物件](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#supported-objects-for-environment-promotion)。

## 當有記錄時數時防止移動任務

>[!NOTE]
>
>預覽版本： 2024年12月19日；適用於所有客戶的生產版本：搭配25.1版（2025年1月16日）

由於移動記錄時數的任務或問題有時會導致相容性或稽核問題，因此我們在「設定」的「任務和問題偏好設定」區域中新增了偏好設定，可讓您防止使用者移動記錄時數的任務和問題。 在此增強功能之前，使用者可以將任務和問題移動到其他專案，即使這些專案上記錄了小時數。

如需詳細資訊，請參閱[設定全系統的任務和問題偏好設定](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。

## 用於單一指派任務的專案或使用者排程的偏好設定

>[!NOTE]
>
>預覽版本： 2024年11月21日；快速發行生產：24.12版（2024年12月12日）；每季發行生產：25.1版（2025年1月16日）

作為系統或群組管理員，您現在有新的偏好設定，可指明Workfront在您指派一名使用者至任務，且專案和使用者都與排程相關聯時，是否應使用專案或使用者的排程來計算專案的時間表。 在此增強功能之前，此設定存在於多使用者指派中。 此設定現在可用於單一使用者對任務的指派。

如需詳細資訊，請參閱[設定全系統的專案偏好設定](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

## 商業規則現在支援超連結

>[!NOTE]
>
>預覽版本： 2024年11月21日；快速發行生產：24.12版（2024年12月12日）；每季發行生產：25.1版（2025年1月16日）

您現在可以在商業規則的自訂錯誤訊息中包含超連結，以指導使用者如何在規則的限制內修改其動作。 靜態URL可連結至對使用者有所幫助的檔案或其他頁面。

如需詳細資訊，請參閱[建立和編輯商業規則](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md)。

## 現起提供原生預先輸入欄位上的篩選

>[!NOTE]
>
>預覽版本： 2024年11月21日；快速發行生產：24.12版（2024年12月12日）；每季發行生產：25.1版（2025年1月16日）

當您將原生欄位參考新增至自訂表單，並且它參考預先輸入欄位(例如，Portfolio、公司或所有者)時，現在可以使用篩選器選項。 篩選器可讓您限制使用者在使用欄位時可選擇的物件。 此自訂篩選的運作方式與自訂預先輸入欄位上的篩選相同，是使用文字模式來定義篩選。

如需詳細資訊，請參閱[建立自訂表格](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

## 「移至」圖示已新增到自訂欄位

>[!NOTE]
>
>預覽版本： 2024年10月29日；快速發行生產：24.11版（2024年11月14日）；每季發行生產：25.1版（2025年1月16日）

當自訂表單包含具有多個欄位的多個區段時，透過拖放將欄位從一個區段移動到另一個區段會很困難。 每個欄位已新增「移至」圖示，可讓您選取欄位所在的區段。

如需詳細資訊，請參閱[整理並預覽表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md)。
