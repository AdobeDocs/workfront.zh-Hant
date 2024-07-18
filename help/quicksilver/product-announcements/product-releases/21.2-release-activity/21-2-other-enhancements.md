---
content-type: release-notes
keywords: 備註，每季，更新，發行
navigation-topic: 2021-2-release-activity
title: 21.2其他增強功能
description: 本頁說明21.2版對預覽環境所做的所有其他增強功能。 這些增強功能將在2021年5月10日當週的生產環境中提供。 如需21.2版所有可用變更的清單，請參閱21.2版總覽。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: f136c08b-63c0-4e1e-a048-09eb84a0ed54
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '610'
ht-degree: 0%

---

# 21.2其他增強功能

本頁說明21.2版對預覽環境所做的所有其他增強功能。 這些增強功能將在2021年5月10日當週的生產環境中提供。 如需21.2版本可用的所有變更清單，請參閱[21.2版本概觀](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md)。

## 我們現在正式改稱Adobe Workfront

Workfront已更名為Adobe Workfront。

Adobe Workfront應用程式中最顯眼的區域和我們面向客戶的網站現在都已更新。 其他區域即將更新。

**已更新區域**

* 登入畫面、頂端導覽、校樣
* 版面配置範本UI、主功能表、自訂Forms匯出(僅在新的Adobe Workfront體驗中可用)
* Workfront行動應用程式(iOS和Android)

區域即將更新

* 適用於桌上型電腦和行動裝置的校訂應用程式
* 清單和報告的PDF匯出
* 瀏覽器標籤中的Favicon圖示

**區域稍後更新**

* 電子郵件通知

## 電子郵件允許清單驗證

>[!NOTE]
>
>僅於新的Adobe Workfront體驗中提供。

如果您使用電子郵件允許清單，新和更新的使用者電子郵件地址現在會根據允許清單進行驗證。 當您新增使用者或編輯現有使用者，並輸入不在允許清單中的電子郵件網域時，訊息會通知您使用者將不會收到電子郵件訊息。 您仍然可以儲存使用者設定檔，但您應該將網域新增到允許清單，以便使用者會收到電子郵件。

如需詳細資訊，請參閱[編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

## 物件標題的新外觀

>[!NOTE]
>
>此功能於2020年3月10日發佈到生產環境。
>
>此功能僅在新的Adobe Workfront體驗中可用。

為了進一步強化資訊的階層，並幫助使用者更清楚瞭解他們所在的頁面，每個物件標頭現在都有：

* 每種物件型別都有色彩鮮豔、更現代的圖示
* 物件名稱上方列出的物件型別
* 更新的字型樣式和文字大小
* 其他次要樣式變更

過去，物件標題的右側不會出現圖示，而是出現一個具有物件名稱的徽章。

新Workfront體驗中區域的頁面標頭（例如增強型分析、資源管理等）也有此更新的外觀。

若要進一步瞭解新Workfront體驗中的新物件標頭，請參閱[新物件標頭](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md)。

![](assets/product-announcement-object-header-350x179.png)

## 物件狀態搜尋回應的更新

Workfront現在以新的方式儲存物件狀態。

這些變更不會影響進行狀態搜尋請求的方式。 不過，包含物件狀態搜尋的API請求將傳回不完整的群組狀態清單。

如需詳細資訊，請參閱[核心API變更：狀態搜尋回應](../../../wf-api/api/api-changes-search.md) 。

## 事件訂閱裝載已更新，以包含所有以ID結尾的欄位

所有事件訂閱裝載現在都包含以「ID」結尾的每個欄位。

請務必注意，每個物件有其專屬的相關欄位集，其中包括以ID結尾的唯一相關欄位集。 這表示雖然每個裝載都包含該物件所有以ID結尾的關聯欄位，但每個物件都有一組以ID結尾的不同欄位。

## Blueprint測試版現在可在預覽中使用

>[!NOTE]
>
>直到21.3版本（今年晚些時候）才會在生產環境中正式提供此功能。 僅於新的Adobe Workfront體驗中提供。

藍圖提供基本的建置組塊，協助您建立隨您成長的工作管理系統。 系統管理員可以瀏覽Blueprint目錄並安裝現成的專案範本。

如需詳細資訊，請參閱[藍圖](../../../administration-and-setup/blueprints/blueprints.md)。
