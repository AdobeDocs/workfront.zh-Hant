---
product-area: reporting
keywords: 使用者，委派，報告，委派，核准
navigation-topic: create-and-manage-reports
title: 建立使用者委派報告
description: 建立使用者委派報告
author: Nolan
feature: Reports and Dashboards
exl-id: c860574b-0488-499e-8d36-d0f3f85aac2d
source-git-commit: 394eb1aed6508399b6459430acec7c0729036edc
workflow-type: tm+mt
source-wordcount: '326'
ht-degree: 2%

---

# 建立使用者委派報告

<!--Audited: 10/2024-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: consider moving this to the Custom&nbsp;View, Filter, Grouping Samples section as an example of a report)</p>
-->

在Adobe Workfront中，使用者可以將專案、任務和問題核准委派給其他使用者，以確保當他們不在辦公室時，他們的核准受到管理。 擁有「計畫」授權的使用者可以建立「使用者委派」報告，以檢視：

* 誰已將其任務、問題和專案核准委派給其他使用者
* 哪些使用者已委派任務、問題和專案核准給他們

* 委派開始和結束的日期

若要深入瞭解委託核准，請參閱[委託核准要求](../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md)。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">DRAFTED: To learn more about delegating work, see <a href="../../../workfront-basics/manage-your-account-and-profile/manage-time-off/personal-time-off.md" class="MCXref xref">Log personal time off and delegate your work</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">DRAFTED: To learn how to manage delegated work in Home, see [future link here].</p>
-->

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
      <td> 
      <p>新增：</p>
         <ul>
         <li><p>標準</p></li>
         </ul>
      <p>目前：</p>
         <ul>
         <li><p>規劃</p></li>
         </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權</p> <p>編輯對篩選器、檢視、群組的存取權</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視其核准已委派之專案以及參與委派之使用者的許可權</p></td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 建立使用者委派報告

1. 按一下Adobe Workfront右上角的&#x200B;**主要功能表**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下&#x200B;**報表**。

1. 按一下&#x200B;**新報告**，然後選取&#x200B;**使用者委派**。

   ![](assets/classic-new-report-user-delegation-350x644.png)

   下列欄位預設會顯示在此報表中：

   | 欄位 | 說明 |
   |---|---|
   | **來自使用者** | 這是將其任務、問題和專案核准委派給其他使用者的使用者。 |
   | **至使用者** | 這是具有委派給他們的任務、問題和專案核准的使用者。 |
   | **開始日期** | 這是進行委派的使用者離開辦公室時間的開始。 |
   | **結束日期** | 這是進行委派的使用者結束外出時間。 |

   {style="table-layout:auto"}

1. （選用）在Report Builder中，修改下列專案：

   * 欄（檢視）
   * 群組
   * 篩選器
   * 圖表

   若要深入瞭解這些功能，請參閱[建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

1. 完成報表建置後，請按一下&#x200B;**儲存+關閉**。

   報表隨即顯示。
