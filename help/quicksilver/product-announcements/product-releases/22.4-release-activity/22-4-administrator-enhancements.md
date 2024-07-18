---
title: 22.4管理員增強功能
description: 22.4管理員增強功能
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1e62e7b3-14b6-4669-b3e1-ac6507343479
source-git-commit: 0876d4d47aad701d5ffadc88868217ebae7e4790
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 0%

---

# 22.4管理員增強功能

本頁說明22.4版對預覽環境所做的所有管理員增強功能。 這些增強功能將在2022年10月3日當週提供。

如需22.4版本可用的所有變更清單，請參閱[22.4版本總覽](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md)。

## 在核准流程中使用解除鎖定狀態

>[!NOTE]
>
>此功能於22.3發行時間範圍內首次引入預覽環境。 It於2022年9月15日發行至生產環境。

為了讓您更能掌控系統中的核准程式和狀態，我們讓您能夠根據解鎖的系統狀態來建立核准程式。 此外，您現在可以解除鎖定核准程式中已使用的任何狀態。 以前，必須鎖定核准流程中使用的系統狀態。 這使得它可供所有群組使用 — 無法將其移除或重新命名 — 因此群組管理員無法簡化其群組狀態清單以符合其特定需求。

## 主選單上的藍圖圖示現在透過版面配置範本控制

系統管理員現在可以透過版面配置範本設定，新增或移除主選單上的藍圖圖示。 這可讓您更能掌控誰可以瀏覽Blueprint目錄。

藍圖圖示會出現在主功能表中，當：

* 使用者未指派任何版面配置範本

* 使用者的版面配置範本在「使用中專案」清單中有「藍圖」選項

* 使用者的版面配置範本在「可用專案」清單中有「藍圖」選項，圖示不會出現在主功能表中。

現有版面範本會自動包含藍圖圖示，管理員可以從版面範本中移除圖示以限制藍圖目錄的可見度。 在22.4版之後建立的新版面範本將包含「使用中專案」清單中的「藍圖」圖示。

如需詳細資訊，請參閱[設定Blueprint的存取權](/help/quicksilver/administration-and-setup/blueprints/configure-access-to-blueprints.md)。

[觀看此功能的影片示範](https://video.tv.adobe.com/v/3412382/){target=_blank}

## 問題標題自訂

作為Workfront或群組管理員，您現在可以自訂當您使用版面配置範本時問題標題中顯示的欄位。

此更新包含下列增強功能：

* 從問題標題中移除或重新排列現有欄位。

* 新增不可編輯的問題概述欄位。 您無法新增可編輯的自訂欄位或欄位。 您還可以顯示問題標題上當前的可編輯欄位（例如，狀態或完成百分比）。

* 問題標題最多可包含五個欄位。

* 您現在可以新增「解決者」欄位到問題標題。 當解決物件與問題相關聯時，「解決者」欄位將變更為「解決問題」、「解決任務」或「解決專案」，具體取決於與問題相關聯的物件型別。

在此版本之前，只能自訂專案和任務標題。



如需詳細資訊，請參閱[使用配置範本自訂物件標頭](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)。

[觀看此功能的影片示範](https://video.tv.adobe.com/v/3412383/){target=_blank}

## 任務標題自訂

作為Workfront或群組管理員，您現在可以自訂當您使用版面配置範本時顯示在任務標題中的欄位。

此更新包含下列增強功能：

* 從任務標題中移除或重新排列現有欄位。

* 新增不可編輯的任務概述欄位。 您無法新增可編輯的自訂欄位或欄位。 您也可以顯示目前位於任務標題上的可編輯欄位（例如，「狀態」或「完成百分比」）。

* 任務標題最多可包含五個欄位。

在此版本之前，只能自訂專案標題。

如需詳細資訊，請參閱[使用配置範本自訂物件標頭](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)。

[觀看此功能的影片示範。](https://video.tv.adobe.com/v/3412384/){target=_blank}

## 面板最新功能的早期功能選擇加入

我們很高興能開啟新的主機板功能，供您及早選擇加入功能。 此選用工具適用於所有組織。

只有Workfront管理員可以選擇加入早期功能。 當管理員選擇加入早期功能時，組織中的所有使用者都會選擇加入，而額外功能會在您的生產Workfront環境中啟用。

如需詳細資訊，請參閱[Adobe Workfront主機板的早期功能選擇加入](/help/quicksilver/agile/get-started-with-boards/boards-early-feature-opt-in.md)。

[觀看此功能的影片示範。](https://video.tv.adobe.com/v/3412386/){target=_blank}

## 自訂表單欄位計算編輯器顯示錯誤資訊

>[!NOTE]
>
>此功能於22.3發行時間範圍內首次引入預覽環境。 它會在第22.4發行版本中發行至生產環境。

編輯自訂欄位的計算現在更容易，並在計算中直接指示有用的錯誤資訊。 當您在自訂表單中建立計算欄位時，錯誤會以粉紅色反白顯示。 當您將滑鼠停留在醒目提示的部分上時，會顯示工具提示來說明問題所在。

[觀看此功能的影片示範。](https://video.tv.adobe.com/v/3412387/){target=_blank}

## 移轉至Adobe Unified Experience

注意：此移轉已延遲至2023年第1季至第2季。 屆時所有受影響的客戶都會收到通知。

如果您的組織已上線Adobe Admin Console，您的Workfront執行個體將會移轉至Adobe Unified Experience 22.4版。

Adobe Unified Experience包括：

* 透過Adobe Experience Cloud對所有Adobe應用程式執行單一登入

* 可在Workfront組織和環境之間移動的「組織切換器」

* 包含Workfront頁面、Adobe Experience Cloud偏好設定和您的Workfront設定檔選項的導覽

如需詳細資訊，請參閱[Workfront的Adobe統一體驗](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md)。

[觀看此功能的影片示範。](https://video.tv.adobe.com/v/3412388/){target=_blank}
