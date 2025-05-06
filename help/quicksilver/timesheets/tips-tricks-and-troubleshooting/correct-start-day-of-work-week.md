---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: 修正時程表的工作週開始日期
description: 我時程表上星期的開始日期與我預期的每週開始日期不符。
author: Alina
feature: Timesheets
exl-id: 5c6c100f-2a04-4a6b-9f95-acc8de3a90f1
source-git-commit: ae3fc73e93474c75fd03144b66af23f7142867c0
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---

# 修正時程表的工作週開始日期

<!--Audited: 5/2025-->

## 問題

我時程表上星期的開始日期與我預期的每週開始日期不符。

這通常發生在您未被指派到時程表設定檔並且您的時程表是手動建立。


## 解決方案

您的Workfront管理員應該建立時間表設定檔，並將所有人指派給設定檔，如[建立、編輯和指派時間表設定檔](/help/quicksilver/timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)中所述。 您的Workfront管理員可將時程表的開始日期定義為預期每週開始日期以外的日期。 請和他們聯絡，以瞭解您的時程表設定檔的時程表開始日期。

如果您的時程表是手動建立的，時程表中一週的開始日期將使用您使用者設定檔中的電子郵件地區設定設定，如[設定我的設定](/help/quicksilver/workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md)一文所述。

例如，在「電子郵件地區設定」設定為「英文（美國）」時，時程表中的周開始於星期日。 或者，在「電子郵件地區設定」設定為「英文（英國）」時，時程表中的一週會從星期一開始。


<!--This is the old content for this article but I found this was not working this way at all, so I changed it to what it is today: 

## Problem

The start day of the week on my timesheet does not match the start day of the week that is configured on my timesheet profile (as described in [Create, edit, and assign timesheet profiles](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).).

## Solution

The start day of the week of a timesheet in Adobe Workfront uses the language and locale settings in your browser to determine the day of the week. Because of this, you need to update the language and locale settings for your browser. 

For example, with the browser language set to English and the locale set to United States, the week starts on Sunday. Alternatively, the browser language set to English and the locale set to United Kingdom, the start day is Monday.

This setting also affects the start day of the week in the pop-up calendars across the system.

The locale change does not affect the start day of the week on the Resource Grid (or resource grid view). The week always starts on Sunday.

Following are the directions for changing language and locale settings for various browsers that are supported with Workfront.

* **Chrome:** Copy and paste the following link into your Chrome browser: `chrome://settings/languages` then go to Languages.
* **Firefox:**Copy and paste the following link into your Firefox browser: `about:preferences#content` then go to Languages.
* **IE 11:** Tools -> Internet Options -> General -> Languages
* **Safari:** Unfortunately, Safari does not allow changing web browsing languages without also changing your entire operating system language. It is probably easier to simply install another browser like Chrome or Firefox.

-->


