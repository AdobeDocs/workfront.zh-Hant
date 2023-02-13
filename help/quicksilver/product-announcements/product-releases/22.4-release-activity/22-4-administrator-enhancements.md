---
title: 22.4管理員增強功能
description: 22.4管理員增強功能
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 1e62e7b3-14b6-4669-b3e1-ac6507343479
source-git-commit: 80fa784e15c3b4a927ee8ba2d18a80a2d84f4a91
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 0%

---

# 22.4管理員增強功能

本頁面說明在「預覽」環境的22.4版中所做的所有管理員增強功能。 這些增強功能將於2022年10月3日當周推出。

如需22.4版所有可用變更的清單，請參閱 [22.4版本概觀](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md).

## 在批准流程中使用解除鎖定狀態

>[!NOTE]
>
>此功能是在22.3版本時間範圍內，首次在「預覽」環境中推出。 It於2022年9月15日發行至生產環境。

為了讓您對系統中的核准流程和狀態擁有更多控制權，我們讓您可以根據未鎖定的系統狀態建立核准流程。 此外，您現在可以解除鎖定核准程式中已使用的任何狀態。 以前，必須鎖定核准程式中使用的系統狀態。 這使它可供所有組使用（不可能刪除或更名），因此組管理員無法簡化組的狀態清單以滿足其特定需要。

## 主菜單上的「藍圖」表徵圖現在通過佈局模板進行控制

系統管理員現在可以通過佈局模板配置來添加或刪除主菜單中的Blueprint表徵圖。 這可更好地控制誰可以瀏覽Blueprint目錄。

當出現以下情況時，「Blueprints（藍圖）」表徵圖將出現在「Main Menu（主菜單）」中：

* 用戶未分配佈局模板

* 用戶的佈局模板在「活動物料」清單中具有「藍圖」選項

* 用戶的佈局模板在「可用項目」清單中具有「藍圖」選項，該表徵圖不會顯示在主菜單中。

現有佈局模板會自動包含「Blueprint」表徵圖，管理員可以從佈局模板中刪除該表徵圖，以限制Blueprint目錄的可見性。 在22.4版之後建立的新佈局模板將在「活動項目」清單中包含「藍圖」表徵圖。

如需詳細資訊，請參閱 [配置對Blueprint的訪問](/help/quicksilver/administration-and-setup/blueprints/configure-access-to-blueprints.md).

[觀看此功能的影片示範](https://video.tv.adobe.com/v/3412382/){target=_blank}

## 問題標題自訂

身為Workfront或群組管理員，您現在可以自訂使用「配置範本」時，問題標題中顯示的欄位。

此更新包含下列增強功能：

* 從問題標題中移除或重新排列現有欄位。

* 新增不可編輯的「問題概述」欄位。 您無法新增可編輯的自訂欄位或欄位。 您也可以顯示問題標題上目前可編輯的欄位（例如狀態或完成百分比）。

* 問題標題最多可包含五個欄位。

* 您現在可以將「解決者」欄位新增至問題標題。 解決對象與問題關聯時，「解決者」欄位將更改為「解決問題」、「解決任務」或「解決項目」，具體取決於與問題關聯的對象類型。

在此版本之前，僅可自訂專案和任務標題。



如需詳細資訊，請參閱 [使用版面範本自訂物件標題](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

[觀看此功能的影片示範](https://video.tv.adobe.com/v/3412383/){target=_blank}

## 任務標題定制

身為Workfront或群組管理員，您現在可以自訂使用「配置範本」時，任務標題中顯示的欄位。

此更新包含下列增強功能：

* 從任務標題中移除或重新排列現有欄位。

* 添加新的、不可編輯的任務概述欄位。 您無法新增可編輯的自訂欄位或欄位。 您也可以顯示當前在任務題頭上的可編輯欄位（例如，狀態或完成百分比）。

* 任務標題最多可包含五個欄位。

在此版本之前，僅可自訂專案標題。

如需詳細資訊，請參閱 [使用版面範本自訂物件標題](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

[觀看此功能的影片示範。](https://video.tv.adobe.com/v/3412384/){target=_blank}

## 搶先選擇加入展示板上的最新功能

我們很高興能為搶先選擇加入功能開啟新的展示板功能。 此可選工具適用於所有組織。

只有Workfront管理員才能選擇加入早期功能。 當管理員選擇提早使用功能時，組織中的所有使用者都會選擇加入，而其他功能則會在您的生產Workfront環境中啟用。

如需詳細資訊，請參閱 [搶先選擇加入Adobe Workfront展示板的功能](/help/quicksilver/agile/get-started-with-boards/boards-early-feature-opt-in.md).

[觀看此功能的影片示範。](https://video.tv.adobe.com/v/3412386/){target=_blank}

## 自定義表單域計算編輯器顯示錯誤資訊

>[!NOTE]
>
>此功能是在22.3版本時間範圍內，首次在「預覽」環境中推出。 透過22.4版發行至生產環境。

編輯自訂欄位的計算現在更輕鬆，計算中直接指出實用的錯誤資訊。 在自訂表單中建立計算欄位時，錯誤會以粉紅色強調顯示。 將滑鼠移到醒目提示的部分上時，畫面會顯示工具提示，說明問題所在。

如需詳細資訊，請參閱 [將計算資料新增至自訂表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

[觀看此功能的影片示範。](https://video.tv.adobe.com/v/3412387/){target=_blank}

## 移轉至AdobeUnified Experience

注意：這一遷移已推遲至2023年的Q1-Q2次。 屆時，所有受影響的客戶都會收到通知。

如果貴組織已上線至Adobe Admin Console，您的Workfront執行個體將會在22.4版本中移轉至Adobe統一體驗。

Adobe統一體驗包括：

* 透過Adobe Experience Cloud為所有Adobe應用程式單次登入

* 在Workfront組織和環境之間移動的「組織切換器」

* 使用Workfront頁面、Adobe Experience Cloud偏好設定和Workfront設定檔選項進行導覽

如需詳細資訊，請參閱 [AdobeWorkfront的統一體驗](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

[觀看此功能的影片示範。](https://video.tv.adobe.com/v/3412388/){target=_blank}
