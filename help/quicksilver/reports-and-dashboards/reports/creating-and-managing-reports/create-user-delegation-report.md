---
product-area: reporting
keywords: 用戶，委派，報告，委派，批准
navigation-topic: create-and-manage-reports
title: 建立使用者委派報表
description: 建立使用者委派報表
author: Nolan
feature: Reports and Dashboards
exl-id: c860574b-0488-499e-8d36-d0f3f85aac2d
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 4%

---

# 建立使用者委派報表

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: consider moving this to the Custom&nbsp;View, Filter, Grouping Samples section as an example of a report)</p>
-->

在Adobe Workfront中，使用者可以委派專案、工作並核發核准給其他使用者，以確保在他們不在辦公室時可管理其核准。 擁有計畫許可證的用戶可以建立「用戶委派」報告，以查看：

* 已將其任務、問題和項目批准委託給其他用戶
* 哪些用戶已將任務、問題和項目批准分配給他們

* 委託的開始和結束日期

若要進一步了解委派核准，請參閱 [委派核准請求](../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">DRAFTED: To learn more about delegating work, see <a href="../../../workfront-basics/manage-your-account-and-profile/manage-time-off/personal-time-off.md" class="MCXref xref">Log personal time off and delegate your work</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">DRAFTED: To learn how to manage delegated work in Home, see [future link here].</p>
-->

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
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對報表、控制面板、日曆的存取</p> <p>編輯對篩選器、檢視、群組的存取</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>查看其批准被委派的項目的權限，以及對參與委派的用戶的權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 建立使用者委派報表

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **報表**.

1. 按一下 **新增報表**，然後選取 **使用者委派**.\
   ![](assets/classic-new-report-user-delegation-350x644.png)

   依預設，此報表會顯示下列欄位：

   | 欄位 | 說明 |
   |---|---|
   | **自使用者** | 這是將其任務、問題和項目批准委派給其他用戶的用戶。 |
   | **至使用者** | 這是具有委派給他們的任務、問題和項目批准的用戶。 |
   | **開始** | 這是進行委派的用戶的休假時間的開始。 |
   | **結束** | 這是已授權用戶的休假時間的結束。 |

   {style=&quot;table-layout:auto&quot;}

1. （選用）在Report Builder中，修改下列項目：

   * 欄
   * 群組
   * 篩選器
   * 圖表

   若要進一步了解這些功能，請參閱 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. 完成報表建置後，按一下 **儲存+關閉**.

1. 在 **報表名稱** 欄位，然後按一下 **儲存報表**.

   報表隨即顯示。
