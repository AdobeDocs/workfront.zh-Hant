---
product-area: projects
navigation-topic: create-projects
title: 建立專案基準線
description: 基準線是專案快照，代表初始專案計畫或專案生命週期中任何指定時間包含的關鍵資訊。
author: Alina
feature: Work Management
exl-id: 422bd7a5-d7a0-4c24-8624-bd0fe6e79d7b
source-git-commit: 3d96d7b7073ad194f291afe370ae813d3482bc9e
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 0%

---

# 建立專案基準線

<!-- Audited: 12/2023 -->

基準線是專案快照，代表初始專案計畫或專案生命週期中任何指定時間包含的關鍵資訊。

您可以使用基準線來比較目前計畫與原始計畫或任何其他時間點的那些資訊片段，以識別問題作業、範圍潛移和其他隨時間變化的趨勢。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<!--
drafted for P&P:

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
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to the project or higher to view baselines</p> <p>Manage permissions to the project to create baselines</p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
    <td><p>新增：標準</p>
        <p>或</p>
        <p>目前：計畫 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級</td> 
   <td> <p>編輯專案的存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視專案或以上版本的許可權以檢視基準線</p> <p>管理專案的許可權以建立基準線</p> </td> 
  </tr> 
 </tbody> 
</table>

*如需此表格中資訊的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 使用基準線的注意事項

* 您可以在專案存留期內多次擷取專案進度快照，建立多個基準線。
* 您可以透過建立基準線或建立「基準線」報表，來檢視專案基準線中包含的資訊。
* 當您建立基準線時，也會擷取該基準線之基準線工作上的工作資訊。
* 您可以建立「基準線作業」報表，以檢視基準線作業的資訊。

>[!IMPORTANT]
>
>基準線會擷取專案名稱、日期和財務資訊的快照。 基準線不包含專案上自訂欄位的值。 如需基準線中包含的財務資訊，請參閱[專案基準線中包含的專案財務](../../../manage-work/projects/project-finances/project-finances-included-in-project-baselines.md)。

## 建立基準線

您可以使用下列方式建立基準線：

* **自動**：您的Workfront管理員或群組管理員會設定Workfront的專案偏好設定，以在專案變為「目前」時自動建立基準。 啟用此設定時，會在專案狀態變成「目前」時建立基準線。 未啟用此設定時，您必須手動建立基準線。

  如需有關設定專案偏好設定和設定自動建立基準線的詳細資訊，請參閱[設定全系統專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

  >[!CAUTION]
  >
  >啟用此設定會在每次專案狀態變更為目前時，自動建立專案的基準線。 第一個建立的基準線是預設基準線。 在專案存留期內，您必須手動建立所有其他基準線。

* **手動**：您可以在專案進行時，視需要為專案建立新的基準線。 然後您可以比較基準線，以檢視專案在一段時間內的進度。

若要建立基準線：

1. 前往專案。
1. 在左側面板中，按一下&#x200B;**基準線**。

   專案](assets/baselines-section-on-project-with-header.png)上的![基準線區段

1. 按一下&#x200B;**新增基準線。**
1. 指定基準線的名稱。
1. （選擇性）如果這是第一個基準線，您可以選取它作為預設值。
1. 按一下「**儲存**」。

   依預設，會顯示下列有關您建立之基準線的資訊：

   * 基準線名稱
   * 基準線輸入日期
   * 建立基準時的專案計劃開始日期
   * 建立基準時的專案預計開始日期
   * 建立基準時的專案實際期間
   * 建立基準線時專案的完成百分比
   * 顯示基準是否為專案之「預設」基準的預設基準指標

     >[!TIP]
     >
     >您無法在同一檢視或報表中同時檢視任何兩個基準的資訊。 您只能在同一個報表中檢視指定基準線與「預設」基準線的資訊。 您可以在專案存留期內隨時修改您認為是「預設」基準線的基準。

1. （選擇性）按一下&#x200B;**檢視**&#x200B;按鈕，然後建立新檢視或編輯目前檢視，將欄位新增至檢視並比較基準之間的其他資訊。 如需詳細資訊，請參閱[在Adobe Workfront中建立或編輯檢視](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md)。

## 建立基準或基準任務報告

若要檢視基準資訊，您也可以建立「基準線」或「基準線工作」報告。 這可讓您在一個檢視中顯示任何數目的基準線或基準線工作的相關欄位，以比較它們。

>[!TIP]
>
>您必須先建立基準線，才能建立「基準線」或「基準線工作」報表。

如需建立報告的詳細資訊，請參閱[建立自訂報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

我們建議您將「專案名稱」分組新增至「基準線」或「基準線任務」報告，以便於閱讀。

如需建立群組的相關資訊，請參閱[在Adobe Workfront中建立群組](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)。
