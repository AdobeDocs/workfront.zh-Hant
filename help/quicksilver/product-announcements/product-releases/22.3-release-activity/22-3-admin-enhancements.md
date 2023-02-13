---
title: 22.3管理員增強功能
description: 22.3管理員增強功能
author: Luke
draft: false
feature: Product Announcements
exl-id: 4607703a-d70e-432c-9fa2-bd43af5a870e
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '805'
ht-degree: 0%

---

# 22.3管理員增強功能

本頁面說明在「預覽」環境中22.3版中進行的所有管理員增強功能。 這些增強功能已於2022年7月11日當周推出。 如需22.3版所有可用變更的清單，請參閱 [22.3版本概觀](/help/quicksilver/product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## 將Adobe Workfront與JumpSeat整合

您現在可以整合JumpSeat與Workfront，為使用者建立自訂的產品內指引。 您必須擁有Adobe Workfront企業授權和有效的JumpSeat訂閱，才能啟用整合。

如需詳細資訊，請參閱 [配置JumpSeat整合](/help/quicksilver/administration-and-setup/configure-integrations/configure-jumpseat.md).

## 校樣預設設定已移至Workfront

您現在可以在Workfront設定區域內編輯下列校樣設定：

* 校樣預設設定

* 校樣決策設定

如需詳細資訊，請參閱 [配置預設校樣設定](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/configure-default-proof-settings.md).

## 在批准流程中使用解除鎖定狀態

**注意：** 從22.3生產版本中移除。 此功能預計於2022年9月15日發行至生產環境。

為了讓您對系統中的核准流程和狀態擁有更多控制權，我們讓您可以根據未鎖定的系統狀態建立核准流程。 此外，您現在可以解除鎖定核准程式中已使用的任何狀態。

以前，必須鎖定核准程式中使用的系統狀態。 這使它可供所有組使用（不可能刪除或更名），因此組管理員無法簡化組的狀態清單以滿足其特定需要。

如需詳細資訊，請參閱下列文章：

* [建立工作項的審批流程](/help/quicksilver/administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)

* [建立或編輯狀態](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)

* [鎖定和解除鎖定系統級狀態](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md)


## 將PDF檔案新增至自訂表單

我們持續協助您透過可新增的新資產小工具（例如影像和影片），讓自訂表單更加視覺化，提供更多資訊。 現在，您可以將連結新增至PDF檔案至自訂表單。 表單附加至物件時，使用物件的使用者可以從表單內檢視與PDF互動。

如需詳細資訊，請參閱 [在自訂表單中新增或編輯影像或其他資產介面工具集](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## 自定義表單域計算編輯器顯示錯誤資訊

>[!NOTE]
>
>此功能暫時無法使用。 此頁面將在功能可用時更新。

編輯自訂欄位的計算現在更輕鬆，計算中直接指出實用的錯誤資訊。 在自訂表單中建立計算欄位時，錯誤會以粉紅色強調顯示。 將滑鼠移到醒目提示的部分上時，畫面會顯示工具提示，說明問題所在。

如需詳細資訊，請參閱 [將計算資料新增至自訂表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## 專案標題自訂

身為Workfront或群組管理員，您現在可以在使用「配置範本」時，自訂專案標題中顯示的欄位。

此更新包含下列增強功能：

* 從專案標題中移除現有欄位。

* 新增不可編輯的專案概述欄位。 您無法新增可編輯的自訂欄位或欄位。 目前位於專案標題上的可編輯欄位可保留在標題上。

* 物件標題最多可包含五個欄位。


在此版本之前，無法自訂物件標題中的欄位。

如需詳細資訊，請參閱 [使用版面範本自訂物件標題](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

## 控制建立空白專案

身為系統或群組管理員，您現在可以控制使用者是否可以建立空白專案，而不需使用範本。 我們已在「設定」的「專案偏好設定」區域導入新設定，可讓您在下列區域停用建立空白專案：

* 從項目清單中的「新建項目」選項

* 從問題頁面將問題轉換為專案時


新設定為「允許使用者建立專案而不使用範本」，預設為啟用。

**注意：** 使用者仍可將任務轉換為空白專案。

如需詳細資訊，請參閱 [配置系統範圍的項目首選項](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## 從「群組」頁面停用群組

最近，我們新增了停用和重新啟用群組的功能。 為了讓動作更快更輕鬆，我們已將其新增至群組的頁面。 現在，按一下群組名稱以前往其頁面後，您可以選取「更多」功能表 ![](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/assets/main-menu-icon.png) 在群組名稱旁，選取「停用」或「重新啟用」。

以前，您只能使用群組詳細資訊頁面上的「使用中」核取方塊，以停用或重新啟用群組。

如需詳細資訊，請參閱 [停用或重新啟用群組](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

## 將影片新增至自訂表單

現在，您可以新增影片，為自訂表單提供新的資訊、視覺興趣和創意模式。 表單附加至物件時，使用物件的使用者隨時都可以播放視訊。

以前，您只能將文字欄位和影像新增至自訂表單。

如需詳細資訊，請參閱 [在自訂表單中新增或編輯影像或視訊資產介面工具集](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

