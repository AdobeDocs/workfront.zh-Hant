---
title: 2023年第四季管理員增強功能
description: 2023年第四季管理員增強功能
author: Lisa
feature: Product Announcements
source-git-commit: 8488cb46b3dd9b377c59121597db5b6fe784fdab
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 0%

---

# 2023年第四季管理員增強功能

此頁面說明2023年第四季版本對「預覽」環境所做的所有管理員增強功能。 這些增強功能將在23.10版本的生產環境中提供。

如需2023年第四季版本週期目前可用的所有變更清單，請參閱 [2023年第四季版本總覽](/help/quicksilver/product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md).

## 自訂表單的計算欄位現在可以使用$$USER萬用字元

此 `$$USER` 新表單設計工具的計算自訂欄位和外部查詢欄位現在提供萬用字元。 引用 `$$USER` 在計算中新增目前使用者的ID。 您也可以將萬用字元搭配其他欄位使用。 例如， `$$USER.{name}` 會新增目前使用者的名稱。

有關計算欄位的詳細資訊，請參閱 [使用表單設計工具新增計算欄位](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

## 從外部API新增值選項至自訂表單

新的欄位型別， **外部查詢**，現在可用於自訂表單設計工具。 當資料儲存在外部系統時，此欄位型別可讓您從外部API載入選項，並根據自訂表單中的其他欄位值進行篩選。

將表單新增到物件時，從API傳回的值會出現在下拉欄位中，使用者可以選擇一個欄位。

>[!NOTE]
>
>新的 **外部查詢** 欄位型別在舊版表單產生器中無法使用。

如需詳細資訊，請參閱 [使用表單設計工具設計表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
