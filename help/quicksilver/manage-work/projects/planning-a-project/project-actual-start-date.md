---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: 項目實際起始日期概覽
description: 專案、工作和問題在Adobe Workfront中有實際開始日期。 對於任務和問題，這是標籤為「進行中」的日期。 對於項目，這是項目上第一個任務被標籤為「正在執行」或已完成的日期。
author: Alina
feature: Work Management
exl-id: 4357b072-24f6-4f89-b624-f066f8af0722
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 0%

---

# 項目實際起始日期概覽

專案、工作和問題在Adobe Workfront中有實際開始日期。 對於任務和問題，這是標籤為「進行中」的日期。 對於項目，這是項目上第一個任務被標籤為「正在執行」或已完成的日期。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>審核或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>檢視或更高權限存取專案</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>檢視專案的或更高權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 關於Workfront中實際開始日期的考量事項

* 「實際起始日期」位於項目、任務和問題的「詳細資訊」部分。 
* 建立這些項目時，不會填入項目、任務或問題的實際起始日期。
* 當項目、任務或問題上的實際工作開始時，會填入實際開始日期。
* 如果項目上的工作尚未開始，則「項目詳細資訊」頁簽上不會顯示實際起始日期。

   如果「任務」和「問題詳細資訊」頁簽上的工作尚未開始，則「實際開始日期」將顯示為空。

* 您可以人工修改任務或問題的實際起始日期，但不能修改項目的實際起始日期。

## 關於專案實際開始日期的考量事項

* Workfront會在發生下列任一情況時自動設定專案的實際日期：

   * 任務受託人將任務的狀態從 *新增* 不等於 *新增*.

   * 任務受託人更改任務的「完成百分比」。

      >[!IMPORTANT]
      >
      >將項目標籤為「當前」時，不會填入項目實際起始日期。 實際工作必須在項目填充的實際開始日期之前開始。

      在這些情況下，項目的實際起始日期設定為項目上最早任務發生這些活動的日期和時間。 這表示專案實際是在此日期和時間開始。

## 找出專案的實際開始日期

您可以在以下區域找到專案的實際開始日期：

* 在專案的「詳細資訊」區段中。
* 在項目報表或視圖中，在報表中添加對象項目的實際開始日期時。

   如需建立報表的相關資訊，請參閱文章 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

要在項目的「詳細資訊」部分中找到實際起始日期，請執行以下操作：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Workfront的右上角，然後按一下 **專案**.
1. 按一下要查看實際開始日期的項目。
1. 按一下 **專案詳細資料** 在左側面板中，然後前往 **概述** 區段。

   實際開始日期會與其他專案日期一起顯示。

   ![](assets/nwe-project-actual-start-date--highlighted-350x367.png)

 
