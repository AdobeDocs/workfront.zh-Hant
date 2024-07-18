---
title: 2023年第四季管理員增強功能
description: 2023年第四季管理員增強功能
author: Lisa
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 7ed37978-b821-488e-9ca1-b81825255be3
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---

# 2023年第四季管理員增強功能

此頁面說明2023年第四季版本對「預覽」環境所做的所有管理員增強功能。 這些增強功能已在23.10版本的生產環境中提供。

如需2023年第四季版本週期目前可用的所有變更清單，請參閱[2023年第四季版本概觀](/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md)。

## 舊版授權模式客戶可用的校訂和檔案決策

尚未轉換至新Adobe Workfront授權模式的舊版客戶，現在可以在單一報表中檢視每個使用者每月校訂/檔案決策數量的資料。 當您執行使用者決定報表時，即可使用此資料。

如需詳細資訊，請參閱[瞭解Adobe Workfront中的物件](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)和[檢視所有使用者的校訂和檔案決策數目](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/view-number-of-decisions-for-users.md)。

## 自訂表單的計算欄位現在可以使用$$USER萬用字元

`$$USER`萬用字元現在可用於新表單設計工具的計算自訂欄位和外部查閱欄位中。 在計算中參照`$$USER`會新增目前使用者的識別碼。 您也可以將萬用字元搭配其他欄位使用。 例如，`$$USER.{name}`會新增目前使用者的名稱。

如需有關計算欄位的詳細資訊，請參閱[使用表單設計工具新增計算欄位](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)。

## 從外部API新增值選項至自訂表單

自訂表單設計工具現在提供新的欄位型別&#x200B;**外部查詢**。 當資料儲存在外部系統時，此欄位型別可讓您從外部API載入選項，並根據自訂表單中的其他欄位值進行篩選。

將表單新增到物件時，從API傳回的值會出現在下拉欄位中，使用者可以選擇一個欄位。

>[!NOTE]
>
>舊版表單產生器沒有新的&#x200B;**外部查詢**&#x200B;欄位型別。

如需詳細資訊，請參閱[使用表單設計工具](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)設計表單。
