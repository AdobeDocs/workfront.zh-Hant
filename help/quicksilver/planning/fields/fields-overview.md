---
title: 欄位概述
description: 您可以在Adobe Workfront Planning中新增反映組織生命週期的欄位。 欄位是記錄型別的屬性。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: a1ad5ada-5010-4dec-934e-a49a3e28aa5f
source-git-commit: 3667359ba2c6ea0aab3ce6845f1a537183f304ec
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 2%

---


# 欄位概述

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


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

      * 當您在記錄型別頁面的表格檢視中新增欄時。 表格的欄是與記錄型別相關聯的欄位。 它們是顯示在記錄頁面上的相同欄位。

        您無法從記錄的頁面建立欄位。

      * 當您連線記錄型別時。 當您在兩個記錄型別之間新增連線，或記錄型別和其他應用程式的物件型別之間新增連線時，可以建立連結的記錄欄位。

        如需有關連線記錄型別的詳細資訊，請參閱[連線記錄型別](/help/quicksilver/planning/architecture/connect-record-types.md)。

      * 當您從Workfront匯入現有欄位時。

        如需詳細資訊，請參閱[從Adobe Workfront匯入欄位](/help/quicksilver/planning/fields/import-fields-from-workfront.md)。


   * 自動：

      * 建立記錄型別時：

         * 姓名
         * 說明
         * 開始日期
         * 結束日期
         * 狀態。 記錄狀態的預設值為：
            * 開發
            * 計畫
            * 作用中
            * 已完成
            * 保留

        您可以新增更多值或重新命名現有值。

      * 從範本建立工作區時。

        如需詳細資訊，請參閱[建立工作區](/help/quicksilver/planning/architecture/create-workspaces.md)。

      * 當您使用Excel或CSV檔案匯入記錄型別時。

        如需詳細資訊，請參閱[建立記錄型別](/help/quicksilver/planning/architecture/create-record-types.md)。

* 無法從Workfront存取Workfront規劃欄位。

* 只有當您連線記錄型別與Workfront物件型別，並從Workfront物件新增連結或查詢欄位時，才能從Workfront Planning存取Workfront欄位。 如需詳細資訊，請參閱[連線記錄型別](/help/quicksilver/planning/architecture/connect-record-types.md)。

* 如果您擁有工作區的「管理」許可權以及該欄位所屬的記錄型別，您可以檢視和更新您或任何其他使用者建立的欄位設定。

* 一個記錄型別最多可以有500個欄位。

* 欄位名稱最多可包含250個字元。

* 刪除記錄型別或工作區時，與其關聯的所有欄位和欄位的值也會被刪除並且無法復原。<!-- this might change with a possible recycle bin solution?!-->
* 當您刪除屬於公式運算式一部分的欄位時，公式欄位會變更。
* 當您變更公式運算式，且該公式欄位被其他公式欄位參考時，其他公式也會受到影響。
