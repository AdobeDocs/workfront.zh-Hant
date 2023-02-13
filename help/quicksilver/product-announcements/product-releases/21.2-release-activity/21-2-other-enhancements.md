---
content-type: release-notes
keywords: 附註，每季，更新，發行
navigation-topic: 2021-2-release-activity
title: 21.2其他增強功能
description: 本頁面說明在「預覽」環境中21.2版所做的所有其他增強功能。 這些增強功能將於2021年5月10日當周在生產環境中提供。 如需21.2版所有可用變更的清單，請參閱21.2版本概觀。
author: Luke
feature: Product Announcements
exl-id: f136c08b-63c0-4e1e-a048-09eb84a0ed54
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 0%

---

# 21.2其他增強功能

本頁面說明在「預覽」環境中21.2版所做的所有其他增強功能。 這些增強功能將於2021年5月10日當周在生產環境中提供。 如需21.2版所有可用變更的清單，請參閱 [21.2版本概觀](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## 我們現在正式成為Adobe Workfront

Workfront已經改名為Adobe Workfront。

Adobe Workfront應用程式和我們面向客戶的網站中最顯眼的區域現已更新。 其他方面即將更新。

**更新區域**

* 登入畫面、頂端導覽、校對
* 版面範本UI、主功能表、自訂Forms匯出(僅適用於新的Adobe Workfront體驗)
* Workfront行動應用程式(iOS和Android)

區域即將更新

* 適用於案頭和行動裝置的校對應用程式
* PDF匯出清單和報表
* 瀏覽器標籤中的Favicon圖示

**區域更新時間較晚**

* 電子郵件通知

## 電子郵件允許清單驗證

>[!NOTE]
>
>僅適用於新的Adobe Workfront體驗。

如果您使用電子郵件允許清單，則新的和更新的使用者電子郵件地址現在會根據允許清單驗證。 當您新增新使用者或編輯現有使用者，並輸入未列在允許清單中的電子郵件網域時，訊息會通知您使用者不會收到電子郵件訊息。 您仍可以儲存使用者設定檔，但您應將網域新增至允許清單，讓使用者收到電子郵件。

如需詳細資訊，請參閱 [編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## 物件標題的全新外觀

>[!NOTE]
>
>此功能已於2020年3月10日發行至生產環境。
>
>此功能僅適用於新的Adobe Workfront體驗。

為了進一步強化資訊的階層關係並協助使用者更清楚了解其所在的頁面，每個物件標題現在都有：

* 每種對象類型的彩色、更現代表徵圖
* 對象名稱上方列出的對象類型
* 更新的字型樣式和文字大小
* 其他微幅樣式變更

以前，物件標題的右側沒有圖示和具有物件名稱的徽章。

新Workfront體驗中區域（例如增強分析、資源管理等）的頁面標題也具有此更新的外觀。

若要進一步了解新Workfront體驗中的新物件標題，請參閱 [新物件標題](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

![](assets/product-announcement-object-header-350x179.png)

## 對象狀態搜索響應的更新

Workfront現在以新方式儲存物件狀態。

這些變更不會影響狀態搜尋請求的提出方式。 不過，包含物件狀態搜尋的API請求會傳回不完整的群組狀態清單。

如需詳細資訊，請參閱 [核心API變更：狀態搜索響應](../../../wf-api/api/api-changes-search.md) .

## 已更新事件訂閱裝載，納入以ID結尾的所有欄位

所有事件訂閱裝載現在都包含以「ID」結尾的每個欄位。

請務必注意，每個物件都有其專屬的關聯欄位集，其中包含以ID結尾的一組唯一關聯欄位。 這表示，雖然每個裝載包含該物件以ID結尾的所有相關聯欄位，但每個物件都有以ID結尾的不同欄位集。

## Blueprint測試版現在可預覽

>[!NOTE]
>
>在今年晚些時候的21.3版本之前，此功能將無法在生產環境中正常使用。 僅適用於新的Adobe Workfront體驗。

Blueprint提供了基本的構建塊，幫助您建立一個隨您而增長的工作管理系統。 系統管理員可以瀏覽藍圖目錄並安裝可供使用的項目模板。

如需詳細資訊，請參閱 [藍圖](../../../administration-and-setup/blueprints/blueprints.md).
