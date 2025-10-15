---
navigation-topic: business-case-and-scorecards
title: 核准業務案例
description: 在您完成並提交專案要求的業務案例後，業務案例必須獲得核准。 這取決於您組織中的工作流程。 專案可以不經業務案例核准而開始，但您的Adobe Workfront管理員和專案所有者可能認為不宜這樣做。
author: Becky
feature: Work Management
exl-id: 60abb054-5cb0-4dd6-9091-c9dcd635a630
source-git-commit: aa3ae2a5d92420f4adcedb60a4f7404533eaa59b
workflow-type: tm+mt
source-wordcount: '682'
ht-degree: 0%

---

# 核准業務案例

<!--Audit: 6/2025-->

在您完成並提交專案要求的業務案例後，業務案例必須獲得核准。 這取決於您組織中的工作流程。 專案可以不經業務案例核准而開始，但您的Adobe Workfront管理員和專案所有者可能認為不宜這樣做。

如需有關完成和提交業務案例的詳細資訊，請參閱文章[為專案建立業務案例](../../../manage-work/projects/define-a-business-case/create-business-case.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront套件</p></td> 
   <td> 
   <p>Prime或更新版本</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> 
   <p>標準 </p> 
   <p>規劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯專案的存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>物件許可權</p></td> 
   <td> <p>管理專案的許可權</p> <p>檢視或更高的投資組合許可權</p>  </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 業務案例核准概要

核准專案的業務案例時，請考量下列事項：

* 您必須擁有專案的管理許可權才能核准其業務案例。
* 您將無法透過首頁中的我的核准Widget看到正在等待業務案例核准的專案。
* 您必須手動前往需要業務案例核准的個別專案，以檢視他們處於未決核准。 沒有Workfront通知機制會提醒某人他們必須核准專案的業務案例。
* 您可以透過建立專案報告或存取與其相關聯的投資組合，找到等待業務案例核准的專案。

  如需關於產品組合的詳細資訊，請參閱文章[&#x200B; Adobe Workfront中的Portfolio概觀](../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md)。

## 建立專案報告以核准業務案例

您可以建立專案報告，以檢視哪些專案需要其業務案例核准。

若要為擱置核准其業務案例的專案建立報告：

1. 建立專案報告。

   如需有關建立報告的詳細資訊，請參閱文章[建立自訂報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

1. 選取報告的&#x200B;**檢視**&#x200B;標籤，然後按一下&#x200B;**新增欄**。

1. 開始在&#x200B;*顯示在此欄*&#x200B;欄位中輸入&#x200B;**狀態**，並在此欄位出現在清單中時選取它。

   此欄將顯示專案狀態。

1. 選取報告的&#x200B;**篩選器**&#x200B;標籤，然後按一下&#x200B;**新增篩選器規則**。

1. 開始在&#x200B;*只為我顯示……*&#x200B;欄位中的專案輸入&#x200B;**狀態**，並在它出現在清單中時選取它。
1. 針對篩選修飾元選取&#x200B;**等於**。
1. 在可用欄位中開始輸入&#x200B;*Requested*。

   這可確保報表僅包含處於請求狀態的專案。

   ![requested_projects_filter.png](assets/requested-projects-filter-350x14.png)

1. （選擇性）按一下&#x200B;**新增其他篩選規則**。

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

   以顯示您指定為Portfolio管理員的位置。

1. 按一下&#x200B;**儲存+關閉**。

   請注意，報表中的所有專案都處於&#x200B;**已要求**&#x200B;的狀態。

1. 按一下報告中的專案名稱以開啟。
1. 按一下左側面板中的&#x200B;**業務案例**。
1. 按一下業務案例摘要區域中的&#x200B;**核准**&#x200B;或&#x200B;**拒絕**，以核准或拒絕業務案例。

<!-- ![Business case](assets/business-case-summary-with-rp-information--1-.png) -->

若業務案例已核准，專案狀態會變更為&#x200B;**已核准**。

若業務案例被拒絕，專案狀態會變更為&#x200B;**已拒絕**。

>[!NOTE]
>
>沒有通知可提醒提交業務案例核准的使用者其專案請求是否核准或拒絕。

## 存取投資組合中請求的專案以核准業務案例

如需有關檢閱請求的專案的詳細資訊，請參閱文章[檢閱請求的專案](../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md)。
