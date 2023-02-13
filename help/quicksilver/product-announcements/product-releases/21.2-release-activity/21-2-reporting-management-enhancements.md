---
content-type: release-notes
keywords: 附註，每季，更新，發行
navigation-topic: 2021-2-release-activity
title: 21. 2報表增強功能
description: 本頁說明在「預覽」環境中21.2版所做的所有報表增強功能。 這些增強功能將於2021年5月10日當周在生產環境中提供。 如需21.2版所有可用變更的清單，請參閱21.2版本概觀。
author: Luke
feature: Product Announcements
exl-id: 1d5f76ef-bea7-4630-8051-454b0d109341
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 0%

---

# 21. 2報表增強功能

本頁說明在「預覽」環境中21.2版所做的所有報表增強功能。 這些增強功能將於2021年5月10日當周在生產環境中提供。 如需21.2版所有可用變更的清單，請參閱 [21.2版本概觀](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## 限制在專案和報表中編輯小時

為了在專案和「小時」報表的「小時」索引標籤上，提供更多時間編輯控制，我們新增了一項設定，可讓Workfront管理員將小時編輯限制在小時擁有者和系統管理員。

以前，在訪問級別啟用工時單和工時的用戶可以編輯工時。

如需詳細資訊，請參閱 [配置工時單和小時首選項](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## 更新清單和報表中「工作總攬」欄位的新外觀和風格

>[!NOTE]
>
>此功能僅適用於新的Adobe Workfront體驗。

為了符合新Workfront體驗中其他區域的現代外觀，更新清單和報表中「工作總攬」欄位的樣式已變更。 這項重新設計包括：

* 使用者設定檔圖片、工作角色和團隊的四捨五入頭像
* 不帶配置檔案圖片的用戶的縮寫顯示
* 新的作業角色表徵圖
* 高級分配的新「人員」表徵圖
* 新的「限制存取」圖示
* 其他微幅設計變更

有關清單中的分配的詳細資訊，請參閱 [指派任務](../../../manage-work/tasks/assign-tasks/assign-tasks.md) 或 [指派問題](../../../manage-work/issues/manage-issues/assign-issues.md).

![](assets/assignments-updates-350x193.png)

## 更新清單和報表中預先輸入欄位的新外觀

>[!NOTE]
>
>2021年5月20日暫時從生產環境中移除。

>[!NOTE]
>
>此功能僅適用於新的Adobe Workfront體驗。

為符合新Workfront體驗中其他區域的現代外觀，更新清單和報表中的字型預先欄位樣式已變更。 這些變更包括：

* 已從欄位中移除Typeahead圖示。
* 按一下「預先輸入」欄位時，現在會在您輸入文字之前顯示建議功能表。
* 建議功能表對值長度的回應更快，現在當符合字元限制時，這些值會在結尾處截斷，而非在值的中間。

如需更新清單的資訊，請參閱 [更新後的清單與舊版清單之間的差異](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md#updated) 文章一節 [開始使用Adobe Workfront中的清單](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

![](assets/typeahead-updates-350x336.png)

## 系統更新報告

新的「日記帳分錄」報表允許您鑽取到系統更新，從而為您提供更高的可審計性，包括：

* 項目、任務或問題的狀態更改
* 已刪除的任務或問題
* 自訂欄位中的值
* 計畫完成日期
* 專案擁有者變更

例如，您可以設定此報表以顯示特定自訂欄位周圍的活動，包括自訂欄位的專案、首次輸入值時的值、該值是什麼、更新欄位時的值、先前的值是什麼、新輸入的值是什麼、使用者完成了這些動作等。

過去，您只能透過Workfront API回報系統更新。

若要深入了解此報表，以及您可以使用它的項目，請參閱 [更新區域報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

