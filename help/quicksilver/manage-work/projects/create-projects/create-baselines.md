---
product-area: projects
navigation-topic: create-projects
title: 建立專案基線
description: 基線是項目快照，表示初始項目計畫中包含的關鍵資訊，或在項目生命期內的任何給定時間。
author: Alina
feature: Work Management
exl-id: 422bd7a5-d7a0-4c24-8624-bd0fe6e79d7b
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 0%

---

# 建立專案基線

基線是項目快照，表示初始項目計畫中包含的關鍵資訊，或在項目生命期內的任何給定時間。

您可以使用基線來比較從當前計畫到原始計畫或任何其他時間點的這些資訊，以確定問題任務、範圍蠕變和隨時間變化的其他趨勢。

## 存取需求

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
   <td role="rowheader">存取層級*</td> 
   <td> <p>編輯專案的存取權</p> <p><b>注意</b>
   如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需存取專案的相關資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">授予專案的存取權</a>. 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>檢視專案或以上版本的權限以檢視基線</p> <p>管理專案的權限以建立基線</p> <p> 如需專案權限的相關資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">在Adobe Workfront中共用專案</a>.</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 使用基線的考量事項

* 您可以在項目的生命週期內多次捕獲項目進度的快照，從而建立多個基線。
* 您可以建立基線或建立基線報表，以檢視包含在專案基線中的資訊。
* 建立基線時，也會根據該基線的基線任務捕獲任務資訊。
* 通過構建「基線任務」報告，可以查看基線任務的資訊。

>[!IMPORTANT]
>
>基線會拍攝項目名稱、日期和財務資訊的快照。 基線不包含專案上自訂欄位的值。 有關基線中包括的財務資訊的資訊，請參見 [項目基線中包含的項目財務](../../../manage-work/projects/project-finances/project-finances-included-in-project-baselines.md).

## 建立基線

可以通過以下方式建立基線：

* **自動**:您的Workfront管理員或群組管理員會設定Workfront的專案偏好設定，以在專案變成「目前」時自動建立基線。 啟用此設定時，當項目狀態變為「當前」時，將建立基線。 未啟用此設定時，您必須手動建立基線。

   有關配置項目首選項和設定自動基線建立的詳細資訊，請參閱 [配置系統範圍的項目首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   >[!CAUTION]
   >
   >啟用此設定會在每次項目狀態更改為「當前」時自動為項目建立基線。 第一個建立的基線是預設的基線。 在項目生效期間，必須手動建立所有其他基線。

* **手動**:您可以視需要隨著專案進行，為專案建立新基線。 然後，您可以比較基線，以查看專案在一段時間內的進展情形。

要建立基線：

1. 導覽至專案。
1. 在左側面板中，按一下 **基線**.

   或

   按一下 **顯示更多**，然後按一下 **基線**.

   ![](assets/nwe-baselines-section-on-project-with-header-350x78.png)

1. 按一下 **新基線。**
1. 指定基線的名稱。
1. （可選）如果這是第一個基線，則可選擇它作為預設基線。
1. 按一下&#x200B;**儲存**。

   依預設，會顯示您建立之基線的下列資訊：

   * 基線名稱
   * 基準錄入日期
   * 計畫起始日期建立基準時的項目起始日期
   * 預計起始日期建立基準時的項目日期
   * 建立基線時的項目實際持續時間
   * 建立基線時項目完成%
   * 顯示基線是否為項目的預設基線的預設基線指標

      >[!TIP]
      >
      >不能在同一個視圖或報告中同時查看任何兩個基線的資訊。 您只能在同一報告中查看給定基線和預設基線的資訊。 在項目生命期內，可以隨時修改您認為是預設基線的基線。

1. （選用）按一下「檢視」旁的下拉式箭頭，然後 **自訂檢視** 將欄位新增至檢視，並比較基線之間的其他資訊。

## 建立基線或基線任務報告

要查看基線資訊，還可以建立基線或基線任務報告。 這可讓您顯示任何數量的基線或基線任務相關欄位，以便在一個檢視中比較這些欄位。

>[!TIP]
>
>必須先建立基線，然後才能建立基線或基線任務報告。

如需建立報表的相關資訊，請參閱 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

建議您將「專案名稱」分組新增至「基線」或「基線」報表，以方便閱讀。

如需建立分組的相關資訊，請參閱 [在Adobe Workfront中建立群組](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).
