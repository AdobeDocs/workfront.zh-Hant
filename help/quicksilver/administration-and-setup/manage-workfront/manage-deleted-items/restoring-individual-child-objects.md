---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: 還原單個子對象
description: 本檔案說明如何取得協助，以復原在30天前從Adobe Workfront生產或預覽環境中刪除的個別子物件。
feature: System Setup and Administration
role: Admin
exl-id: e2e4fbb7-5433-4d88-8e36-d82f4cc8a194
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '575'
ht-degree: 0%

---

# 還原單個子對象

本檔案說明如何取得協助，以復原在30天前從Adobe Workfront生產或預覽環境中刪除的個別子物件。

Workfront管理員可以還原每個Workfront例項中的專案、工作、問題和檔案，如 [還原已刪除的項](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md). 但只有Workfront資料庫團隊可以獨立於其父對象，恢復對象，如任務、問題、文檔、自定義表單、小時和注釋。

來自您即時環境的資料可在「預覽沙箱」中使用，最多7天。 這表示您可以使用下列方法，從「預覽沙箱」環境匯出獨立資料：

* Kick-Start
* 建立報表並匯出結果

如需從Workfront匯出資料的詳細資訊，請參閱 [匯出資料](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

您可以透過下列方式匯入匯出的資料：

* 手動，如果您使用匯出的報表
* 如果您使用Kick-Starts，則大量

   如需使用Kick-Starts將資料匯入Workfront的詳細資訊，請參閱 [使用Kick-Start範本將資料匯入Adobe Workfront](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

週末的維護期間會重新整理「預覽沙箱」環境。

如需預覽沙箱環境維護期間的詳細資訊，請參閱 [trust.workfront.com](https://trust.workfront.com/).

>[!IMPORTANT]
>
>文檔是這些恢複方法的例外。 您可以從預覽環境手動下載，然後重新上傳至生產環境。 如果您想要大量下載和上傳檔案，需要向Workfront要求資料還原。

## 資料還原所需的資訊

一旦確定刪除的對象需要由我們的資料庫團隊進行還原後，收集與此相關的資訊就越多。 我們的資料庫管理員需要以下資訊才能查找對象並啟動還原：

* 物件名稱
* 對象類型（任務、問題、項目等）
* 預計刪除日期和時間
* 對象GUID（如果可能）

   找到物件的GUID時，請參閱下列資訊：

   * GUID可透過參考與物件互動所觸發的電子郵件通知（指派給、註解等）來找到
   * URL結尾處的GUID範例： `yourdomain.my.workfront.com/issue/view?ID=568bfa96011220154c8ca4c4e691556b`

收集完此資訊或需要幫助後，請致電844-306-HELP(4357)，或線上提交票證。

## 資料還原過程

1. 我們的客戶支援團隊收到您的資訊後，會將資訊呈報給我們的客戶支援團隊。
1. 我們的客戶支援團隊將聯繫我們的資料庫團隊。
1. 一旦資料庫團隊有機會審查要還原的資料，就可以提供ETA的更準確估計。 恢復通常需要三天，但所需時間可能更長，具體取決於要恢復的資料的類型和數量。
1. 資料庫團隊會將資訊還原到您的預覽沙箱環境，您將有機會檢閱還原的資料。 我們的客戶支援團隊會在資料可在預覽沙箱中找到時通知您。
1. 在您對沙箱中的還原感到滿意後，請通知我們的客戶支援團隊，他們將聯繫我們的資料庫團隊，通知他們可以將資料還原到您的生產環境。
1. 請求關閉前，您將有機會檢閱已還原的資料。
