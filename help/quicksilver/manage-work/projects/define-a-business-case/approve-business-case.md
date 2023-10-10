---
navigation-topic: business-case-and-scorecards
title: 核准業務案例
description: 在您完成並提交專案要求的業務案例後，業務案例必須獲得核准。 這取決於您組織中的工作流程。 專案可以不經業務案例核准而開始，但您的Adobe Workfront管理員和專案所有者可能認為不宜這樣做。
author: Alina
feature: Work Management
exl-id: 60abb054-5cb0-4dd6-9091-c9dcd635a630
source-git-commit: f4ef463ebdc9a4a7a0802e5394d7820ebc447aa9
workflow-type: tm+mt
source-wordcount: '733'
ht-degree: 0%

---

# 核准業務案例

在您完成並提交專案要求的業務案例後，業務案例必須獲得核准。 這取決於您組織中的工作流程。 專案可以不經業務案例核准而開始，但您的Adobe Workfront管理員和專案所有者可能認為不宜這樣做。 

如需完成和提交業務案例的詳細資訊，請參閱文章 [為專案建立業務案例](../../../manage-work/projects/define-a-business-case/create-business-case.md).

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>Pro或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯專案的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理專案的許可權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 業務案例核准概要

核准專案的業務案例時，請考量下列事項：

* 您必須擁有專案的管理許可權才能核准其業務案例。 
* 您將無法在首頁的[核准]下看到等待業務案例核准的專案。
* 您必須手動前往需要業務案例核准的個別專案，以檢視他們處於未決核准。 沒有Workfront通知機制會提醒某人他們必須核准專案的業務案例。
* 您可以透過建立專案報告或存取與其相關聯的投資組合，找到等待業務案例核准的專案。 

  如需Portfolio的詳細資訊，請參閱文章 [Adobe Workfront中的Portfolio概觀](../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

## 建立專案報告以核准業務案例

您可以建立專案報告，以檢視哪些專案需要其業務案例核准。 

若要為擱置核准其業務案例的專案建立報告：

1. 建立專案報告。

   如需建立報表的詳細資訊，請參閱文章 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. 選取 **檢視** 索引標籤中，然後按一下 **新增欄**.

1. 開始在「 」中輸入「狀態」 **顯示在此欄中** 欄位，並在此欄位出現在清單中時選取它。

    此欄將顯示專案狀態。

1. 選取 **篩選器** 索引標籤中，然後按一下 **新增篩選器規則**.

1. 開始在「 」中輸入「狀態」 **只為我顯示其中的……** 欄位，並在清單中出現時選取它。
1. 選取 **等於** （篩選修飾元）。
1. 開始在可用欄位中輸入「已要求」。 

   這可確保報表僅包含處於請求狀態的專案。

     ![requested_projects_filter.png](assets/requested-projects-filter-350x14.png)

1. （選用）按一下 **新增另一個篩選器規則**.

   您可以新增其他篩選器，以僅顯示您是專案所有者、專案贊助者或Portfolio所有者的專案。

   例如，您可以使用以下篩選陳述式： 

   ```
   Project Sponsor ID Equals $$USER.ID
   ```

   顯示您指定為專案贊助者的專案

   ```
   Project Owner ID Equals $$USER.ID
   ```

   顯示您指定為專案所有者的專案

   ```
   Project Portfolio Owner ID Equals $$USER. ID
   ```

   以顯示您被指定為「Portfolio管理員」的位置。 

1. 按一下 **儲存+關閉**.

   請注意，報表中的所有專案都處於 **已要求**.

1. 按一下報告中的專案名稱以開啟。
1. 按一下 **業務案例** 在左側面板中。
1. 按一下 **核准** 或 **拒絕** 在「業務案例摘要」區域中，以核准或拒絕業務案例。

   ![](assets/business-case-summary-with-rp-information--1-.png)

   專案狀態已變更為 **已核准** 業務案例是否核准。

   專案狀態已變更為 **已拒絕** 若業務案例遭拒絕。

   >[!NOTE]
   >
   >沒有通知可提醒提交業務案例核准的使用者其專案請求是否核准或拒絕。

## 存取投資組合中請求的專案以核准業務案例

如需有關檢閱請求的專案的詳細資訊，請參閱文章 [檢閱請求的專案](../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md).
