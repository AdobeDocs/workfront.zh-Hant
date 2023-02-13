---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: 項目、任務和問題的預計完成日期概覽
description: 預計完成日期是即時計算的指標，用於指明項目、任務或問題何時完成。 當項目、任務或問題標籤為已完成時，預計完成日期將更改為實際完成日期的日期。
author: Alina
feature: Work Management
exl-id: dde400e6-189f-4431-8f2f-7142ce424826
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '876'
ht-degree: 0%

---

# 項目、任務和問題的預計完成日期概覽

預計完成日期是即時計算的指標，用於指明項目、任務或問題何時完成。 當項目、任務或問題標籤為已完成時，預計完成日期將更改為實際完成日期的日期。

以下各節介紹如何為項目、任務和問題確定預計完成日期，以及如何確定它。

## 存取需求

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   <p>For current licenses: 
   <ul><li><p>Contributor or higher to view the Projected Completion Date in a report</p></li> <li><p>A Standard license to create a report</p></li> </ul>
   
   <p>For legacy licenses: 
   <ul><li><p>Review or higher to view the Projected Completion Date in a report</p></li> 
   <li><p>A Plan license to create a report</p> </li></ul>
      </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects</p> <p>You must have Edit access to Reports, Dashboards, Calendars to create a report</p> <p>You must have Edit access to Filters, Views, Groupings to create a report or modify a list view</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
   <td> <p>複查或更新以查看報表中的預計完成日期</p> <p>建立報表的計畫授權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>檢視或更高權限存取專案</p> <p>您必須擁有「編輯」存取權，才能建立報表、控制面板、日曆</p> <p>您必須擁有「編輯」存取權，才能建立報表或修改清單檢視</p> <p><b>附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>檢視專案的或更高權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## Adobe Workfront如何確定預計完成日期

預計完成日期是計算欄位，無法人工更改。

用於確定預計完成日期的標準會因您正在查看的對象而有所不同：

* **專案：** 項目的預計完成日期等於項目上最近任務的預計完成日期。
* **任務：** 任務的預計完成日期根據以下標準確定：

   * **任務受讓人對任務進行的進度更新：** 進度更新包括完成百分比的更改和任務狀態的更改。
   * **提交日期：** 如果任務受託人指定了提交日期，則預計完成日期將更改為與提交日期匹配。

      有關「提交日期」的詳細資訊，請參閱文章 [提交日期概述](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

   * **前置任務：** 如果前置任務沒有延遲，則預計完成日期應與計畫完成日期匹配。 當延遲發生時，相依任務顯示的預計完成日期大於計畫完成日期。

      有關任務的計畫完成日期的詳細資訊，請參閱 [任務計畫完成日期概覽](../../../manage-work/tasks/task-information/task-planned-completion-date.md).
   >[!IMPORTANT]
   >
   >當任務的前置任務具有實際完成日期時，從屬任務將接收預計完成日期，如以下方案所述：
   >
   >
   >如果項目具有任務A、任務B和任務C，並且任務B是任務A的後繼任務，則任務C是任務B的後繼任務，並且實際完成日期將添加到任務A中，則系統會自動為任務B重新計算預計完成日期(前提是 **更新類型** 項目的「自動」和「更改時」設定為「自動」，但不會為任務C重新計算。目前，Workfront會基於效能原因計算從更新任務上下一個層的任務的「預計完成日期」。 

* **問題：**問題預計完成日期最初設定為與問題計畫完成日期匹配。

   如果問題受託人指定了提交日期，則「預計完成日期」和「計畫完成日期」都將更改，以與「提交日期」匹配。

   有關「提交日期」的詳細資訊，請參閱文章 [提交日期概述](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## 查看預計完成日期

您可以查看報表中項目、任務和問題的預計完成日期。 您可以查看Workfront其他區域中項目和任務的預計完成日期。 

* [查看項目的預計完成日期](#view-the-projected-completion-date-of-a-project)
* [查看任務的預計完成日期](#view-the-projected-completion-date-of-a-task)
* [查看問題的預計完成日期](#view-the-projected-completion-date-of-an-issue)

### 查看項目的預計完成日期 {#view-the-projected-completion-date-of-a-project}

1. 轉到要查看預計完成日期的項目。
1. 按一下 **專案詳細資料** 中。
1. 找出 **預計完成日期** 欄位 **概述** 區段。

### 查看任務的預計完成日期 {#view-the-projected-completion-date-of-a-task}

1. 轉到要查看預計完成日期的任務。
1. 按一下 **任務詳細資訊** 中。
1. 找出 **預計完成日期** 欄位 **概述** 區段。

### 查看問題的預計完成日期 {#view-the-projected-completion-date-of-an-issue}

您只能在問題報表或清單視圖中查看問題的預計完成日期。 建立清單檢視類似於在報表中建立檢視。

要建立包含預計完成日期的問題報表，請執行以下操作：

1. 建立問題報告，如文章所述 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. 選取 **欄（檢視）** 標籤。
1. 按一下 **添加列**，然後開始輸入 **預計完成日期** 在 **顯示於此欄中：** 欄位。

1. 當它出現在清單中時，請在 **問題** 物件。 
1. 按一下 **儲存+關閉**.

   此 **預計完成日期** 欄填入。 

   ![](assets/issue-projected-completion-date-in-view-nwe-350x148.png)
