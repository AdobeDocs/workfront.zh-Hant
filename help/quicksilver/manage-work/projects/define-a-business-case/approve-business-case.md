---
navigation-topic: business-case-and-scorecards
title: 批准業務案例
description: 完成並提交項目請求的業務案例後，必須批准該業務案例。 這取決於您組織中的工作流程。 專案可以在不需要核准業務案例的情況下開始，但您的Adobe Workfront管理員和專案擁有者可能不認為是理想的作法。
author: Alina
feature: Work Management
exl-id: 60abb054-5cb0-4dd6-9091-c9dcd635a630
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '733'
ht-degree: 0%

---

# 批准業務案例

完成並提交項目請求的業務案例後，必須批准該業務案例。 這取決於您組織中的工作流程。 專案可以在不需要核准業務案例的情況下開始，但您的Adobe Workfront管理員和專案擁有者可能不認為是理想的作法。 

有關填寫和提交業務案例的詳細資訊，請參閱文章 [為項目建立業務案例](../../../manage-work/projects/define-a-business-case/create-business-case.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>Pro或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯專案的存取權</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理專案的權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 業務案例審批概述

批准項目的「業務案例」時，請考慮以下事項：

* 您必須擁有專案的「管理」權限，才能核准其商業案例。 
* 您將看不到在「首頁批准」下等待業務案例獲得批准的項目。
* 您必須手動轉到需要Business Case批准的個別項目，以查看它們是否在等待批准。 沒有Workfront通知機制可提醒某人必須核准專案的業務案例。
* 您可以通過構建項目報告或訪問與其關聯的產品組合，找到等待業務案例批准的項目。 

   如需Portfolio的詳細資訊，請參閱文章 [PortfolioAdobe Workfront概觀](../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

## 建立專案報表以核准業務案例

您可以為專案建立報表，查看哪些專案需要核准其業務案例。 

要為等待其業務案例批准的項目建立報告，請執行以下操作：

1. 建立專案的報表。

   如需建立報表的詳細資訊，請參閱文章 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. 選取 **檢視** ，然後按一下 **添加列**.

1. 開始在 **顯示在此列中** 欄位，並在此欄位出現在清單中時選擇它。

    此欄會顯示專案的狀態。

1. 選取 **篩選器** ，然後按一下 **新增篩選規則**.

1. 開始在 **僅顯示……** 欄位，並在清單中出現時選取它。
1. 選擇 **等於** （針對篩選修飾詞）。
1. 開始在可用欄位中鍵入「已請求」。 

   這可確保報告僅包括處於「請求」狀態的項目。

     ![requested_projects_filter.png](assets/requested-projects-filter-350x14.png)

1. （選用）按一下 **新增其他篩選規則**.

   您可以新增其他篩選條件，只顯示您是專案擁有者、專案贊助者或Portfolio擁有者的專案。

   例如，您可以使用下列篩選陳述式： 

   ```
   Project Sponsor ID Equals $$USER.ID
   ```

   顯示指定您作為項目贊助商的項目

   ```
   Project Owner ID Equals $$USER.ID
   ```

   顯示指定為「項目」所有者的項目

   ```
   Project Portfolio Owner ID Equals $$USER. ID
   ```

   顯示指定您為「Portfolio管理員」的位置。 

1. 按一下 **儲存並關閉**.

   請注意，報表中的所有專案都處於 **已請求**.

1. 按一下報表中專案的名稱以開啟它。
1. 按一下 **業務案例** 中。
1. 按一下 **核准** 或 **拒絕** 在「業務案例匯總」區域中批准或拒絕業務案例。 

   ![](assets/business-case-summary-with-rp-information--1-.png)

   專案狀態已變更為 **已核准** 如果業務案例被批准。

   專案狀態已變更為 **已拒絕** 如果Business案例被拒絕。

   >[!NOTE]
   >
   >沒有通知會提醒提交業務案例批准的用戶其項目請求是否被批准或拒絕。

## 通過訪問產品組合中的請求項目來批准業務案例

有關審核請求的項目的詳細資訊，請參閱文章 [審查請求的項目](../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md).
