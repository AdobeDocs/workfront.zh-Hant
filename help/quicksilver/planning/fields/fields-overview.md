---
title: 欄位概述
description: 您可以在Adobe Workfront Planning中新增反映組織生命週期的欄位。 欄位是記錄型別的屬性。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: a1ad5ada-5010-4dec-934e-a49a3e28aa5f
source-git-commit: 78a54ec94dd5a5746144e99e14c622e8b3a7ea71
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 2%

---


# 欄位概述

{{planning-important-intro}}

您可以在Adobe Workfront Planning中新增反映組織生命週期的欄位。 欄位是記錄型別的屬性。


## 有關Adobe Workfront Planning欄位的考量事項

* 您只能從記錄型別頁面的表格檢視建立欄位。 欄位在表格檢視中顯示為欄。 與記錄型別關聯的所有欄位也會顯示在記錄頁面中。

  如需有關管理資料表資料行（或記錄欄位）的資訊，請參閱[管理資料表檢視](/help/quicksilver/planning/views/manage-the-table-view.md)。

  如需有關管理欄位的資訊，另請參閱下列文章：

   * [編輯欄位設定](/help/quicksilver/planning/fields/edit-fields.md)
   * [刪除欄位](/help/quicksilver/planning/fields/delete-fields.md)

* 與記錄型別相關聯的欄位可與該型別的所有記錄相關聯。<!--will this change and will the fields be available for other record types, too?! Also, the next bullet might need to change too if this one changes -->

* 無法將與記錄型別關聯的欄位新增到其他記錄型別。<!-- this will change when they open the Field library tab when creating a field-->

* 您可以透過下列方式手動或自動建立欄位：

   * 手動：

      * 在記錄型別頁面的表格檢視中新增欄。 表格的欄是與記錄型別相關聯的欄位。 它們是顯示在記錄頁面上的相同欄位。

        您無法從記錄的頁面建立欄位。

      * 藉由連線記錄型別。 當您在兩個記錄型別之間新增連線，或記錄型別和其他應用程式的物件型別之間新增連線時，可以建立連結的記錄欄位。

        <!--* Importing record types with fields using a CSV or an Excel file. - this is not available yet-->

        如需有關連線記錄型別的詳細資訊，請參閱[連線記錄型別](/help/quicksilver/planning/architecture/connect-record-types.md)。

     <!--* By importing record types using an Excel or CSV file. For more information, see [Create record types](/help/quicksilver/planning/architecture/create-record-types.md). -->

   * 自動：

     以下是預設為每種新記錄型別建立的標準欄位：

      * 姓名
      * 說明
      * 開始日期
      * 結束日期
      * 狀態。 記錄狀態的預設值為：
         * 開發
         * 計畫
         * 啟用中
         * 已完成
         * 保留

        您可以新增更多值或重新命名現有值。

     當您從範本建立工作區時，Workfront Planning會為記錄型別建立欄位。 如需詳細資訊，請參閱[建立工作區](/help/quicksilver/planning/architecture/create-workspaces.md)。

* 無法從Workfront存取Workfront規劃欄位。

* 只有當您連線記錄型別與Workfront物件型別，並從Workfront物件新增連結或查詢欄位時，才能從Workfront Planning存取Workfront欄位。 如需詳細資訊，請參閱[連線記錄型別](/help/quicksilver/planning/architecture/connect-record-types.md)。

* 如果您擁有欄位所屬工作區的管理許可權，您可以檢視和更新您或任何其他使用者建立的欄位設定。

* 一個記錄型別最多可以有500個欄位。

* 欄位名稱最多可包含250個字元。

* 刪除記錄型別或工作區時，與其關聯的所有欄位和欄位的值也會被刪除並且無法復原。<!-- this might change with a possible recycle bin solution?!-->
