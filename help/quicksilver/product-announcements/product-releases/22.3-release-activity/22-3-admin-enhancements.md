---
title: 22.3管理員增強功能
description: 22.3管理員增強功能
author: Luke
draft: false
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4607703a-d70e-432c-9fa2-bd43af5a870e
source-git-commit: dd718ff8f497065018cdfb9592ff0804d7668bf8
workflow-type: tm+mt
source-wordcount: '767'
ht-degree: 0%

---

# 22.3管理員增強功能

本頁說明22.3版對預覽環境所做的所有管理員增強功能。 這些增強功能已在2022年7月11日當週推出。 如需22.3版本可用的所有變更清單，請參閱[22.3版本總覽](/help/quicksilver/product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md)。

## 將Adobe Workfront與JumpSeat整合

您現在可以將JumpSeat與Workfront整合，為使用者建立自訂的產品內指南。 您必須擁有Adobe Workfront企業授權和使用中的JumpSeat訂閱才能啟用整合。

如需詳細資訊，請參閱[設定JumpSeat整合](/help/quicksilver/administration-and-setup/configure-integrations/configure-jumpseat.md)。

## 校訂預設設定已移至Workfront

您現在可以在Workfront設定區域中編輯以下校訂設定：

* 校訂預設設定

* 校訂決定設定

如需詳細資訊，請參閱[設定預設校訂設定](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/configure-default-proof-settings.md)。

## 在核准流程中使用解除鎖定狀態

**注意：**&#x200B;已從22.3生產版本中移除。 此功能計畫於2022年9月15日發佈到生產環境。

為了讓您更能掌控系統中的核准程式和狀態，我們讓您能夠根據解鎖的系統狀態來建立核准程式。 此外，您現在可以解除鎖定核准程式中已使用的任何狀態。

以前，必須鎖定核准流程中使用的系統狀態。 這使得它可供所有群組使用 — 無法將其移除或重新命名 — 因此群組管理員無法簡化其群組狀態清單以符合其特定需求。

如需詳細資訊，請參閱下列文章：

* [建立工作專案的核准流程](/help/quicksilver/administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)

* [建立或編輯狀態](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)

* [鎖定和未鎖定的系統層級狀態](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md)


## 將PDF檔案新增至自訂表單

我們持續協助您使用可新增的新資產小工具（例如影像和視訊），讓自訂表單更視覺化且資訊更豐富。 現在您可以將PDF檔案的連結新增至自訂表格。 當表單附加到物件時，使用物件的使用者可以從表單內檢視並與PDF互動。

## 自訂表單欄位計算編輯器顯示錯誤資訊

>[!NOTE]
>
>此功能暫時無法使用。 當此功能可用時，將會更新此頁面。

編輯自訂欄位的計算現在更容易，並在計算中直接指示有用的錯誤資訊。 當您在自訂表單中建立計算欄位時，錯誤會以粉紅色反白顯示。 當您將滑鼠停留在醒目提示的部分上時，會顯示工具提示來說明問題所在。

## 專案標題自訂

作為Workfront或群組管理員，您現在可以自訂當您使用版面配置範本時專案標題中顯示的欄位。

此更新包含下列增強功能：

* 從專案標題中移除現有欄位。

* 新增不可編輯的新專案概述欄位。 您無法新增可編輯的自訂欄位或欄位。 目前位於專案標題上的可編輯欄位可以保留在標題上。

* 物件標頭最多可包含五個欄位。


在此版本之前，無法自訂物件標題中的欄位。

如需詳細資訊，請參閱[使用配置範本自訂物件標頭](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)。

## 控制建立空白專案

作為系統或群組管理員，您現在可以控制使用者是否可以在不使用範本的情況下建立空白專案。 我們在「設定」的「專案偏好設定」區域中引入了一項新設定，可讓您停用在下列區域建立空白專案：

* 從專案清單中的新專案選項

* 從問題頁面將問題轉換為專案時


新的設定是「允許使用者在不使用範本的情況下建立專案」，預設為啟用。

**注意：**&#x200B;使用者仍然可以將任務轉換為空白專案。

如需詳細資訊，請參閱[設定全系統的專案偏好設定](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

## 從群組頁面停用群組

最近，我們新增了停用及重新啟用群組的功能。 為了更快、更輕鬆地進行該動作，我們將其新增到群組的頁面。 現在，在您按一下群組名稱以移至其頁面後，您可以選取群組名稱旁邊的[更多]功能表![](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/assets/main-menu-icon.png)，然後選取[停用]或[重新啟用]。

過去，您只能使用群組「詳細資訊」頁面上的「作用中」核取方塊來停用或重新啟用群組。

如需詳細資訊，請參閱[停用或重新啟用群組](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md)。

## 新增視訊至自訂表格

現在，您可以新增視訊，為自訂表單提供全新的資訊、視覺趣味和創意模式。 當表單附加到物件時，使用物件的使用者可以隨時播放視訊。

以前，您只能將文字欄位和影像新增到自訂表單中。

