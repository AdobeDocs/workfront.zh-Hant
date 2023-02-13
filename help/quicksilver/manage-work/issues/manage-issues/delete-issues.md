---
product-area: projects
navigation-topic: manage-issues
title: 刪除問題
description: 如果您有正確的存取權和權限，可以刪除Adobe Workfront中的問題或請求。
author: Alina
feature: Work Management
exl-id: 31cc802f-7fa6-420c-8494-a45313df1f10
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 1%

---

# 刪除問題

如果您有正確的存取權和權限，可以刪除Adobe Workfront中的問題或請求。

>[!TIP]
>
>「Issues」和「requests」在Workfront中可互換使用。 您可以記錄項目和任務中的問題，以指明需要解決的未預見的工作。 您也可以提交記錄為問題的請求，此問題會列在指定為「請求佇列」的專案上。

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
   <td> <p>要求或更高版本</p> <p>檢閱或取得更高授權，以刪除專案「問題」區段中的問題。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯問題的存取權</p> <p>查看或更高程度地訪問項目和任務</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需存取層級問題的相關資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">授予問題的存取權</a>. 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理問題的權限</p> <p>對專案或任務貢獻或更高權限</p> <p> 如需授予問題權限的相關資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">共用問題 </a></p> <p>如需要求其他權限的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 刪除問題的考量事項

* 您的Workfront管理員或群組管理員必須在「專案偏好設定」區域中，啟用刪除狀態為「完成」的專案問題。 有關設定項目首選項的資訊，請參閱 [配置系統範圍的項目首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* 如果問題記錄了小時，Workfront管理員或群組管理員必須允許在Workfront執行個體中設定「任務和問題偏好設定」 ，以刪除這些問題。 當您嘗試刪除登入時數發生問題的專案時，也會套用此方法。

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">(this is not possible in classic)</span>
  </MadCap:conditionalText>
  -->

   如需有關啟用刪除記錄小時數的問題的詳細資訊，請參閱 [配置全系統任務和問題首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## 刪除問題的影響

刪除問題時，會影響連結到問題的其他對象。

刪除問題時，也會刪除與問題相關聯的下列物件：

* 文件

   無法刪除已附加簽出文檔的問題。 有關簽出文檔的詳細資訊，請參閱 [簽出文檔](../../../documents/managing-documents/check-out-documents.md).

* 附註
* 核准

視您的Workfront或群組管理員在 **時間表和小時首選項** 在您的Workfront例項中，刪除問題時，系統會以下列其中一種方式處理問題的記錄時數：

* 移至專案，如果問題稍後還原，則無法復原。
* 如果問題稍後還原，則會刪除並還原。

   當您嘗試刪除已登入數小時之任務的專案時，也會套用此方法。

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">(this is not possible in classic)</span>
  </MadCap:conditionalText>
  -->

   如需針對記錄問題的數小時設定刪除偏好設定的詳細資訊，請參閱 [配置工時單和小時首選項](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* 指派給核發或核發核准的使用者仍保留在專案團隊中。\
   如需專案團隊的詳細資訊，請參閱 [專案團隊概觀](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## 刪除問題

* [同時刪除專案中的多個問題](#delete-multiple-issues-in-a-project-simultaneously)
* [刪除單一問題](#delete-a-single-issue)

### 同時刪除專案中的多個問題  {#delete-multiple-issues-in-a-project-simultaneously}

1. 前往 **主菜單**.
1. 按一下 **專案**.
1. 按一下包含您要刪除之問題的專案名稱。
1. 按一下 **問題** 中。
1. 選取問題，然後按一下 **刪除** 圖示 ![](assets/delete.png) 清單頂端。

1. 如果允許刪除，請按一下 **是，刪除它**.\
   您的Workfront管理員可能不允許刪除記錄小時的問題。\
   如需刪除問題所需的存取權和權限詳細資訊，請參閱 [刪除問題](#access-and-permissions-needed).

### 刪除單一問題 {#delete-a-single-issue}

1. 按一下 **主要** 功能表。
1. 按一下 **專案**.
1. 按一下包含您要刪除之問題的專案名稱。
1. 按一下 **問題** 中。

   ![](assets/qs-issues-icon-highlighted-on-project-350x278.png)

1. 按一下您要刪除的問題名稱。
1. 按一下 **更多** 功能表。

   ![](assets/qs-issue-more-menu-highlighted-350x469.png)

1. 按一下 **刪除**.
1. 如果允許刪除，請按一下 **是，刪除它**.

   您的Workfront管理員可能不允許刪除記錄小時的問題。\
   如需刪除問題所需的存取權和權限詳細資訊，請參閱 [刪除問題](#access-and-permissions-needed).

## 還原已刪除的問題

Workfront或群組管理員可在問題刪除後30天內還原。 如需在Workfront中還原項目的詳細資訊，請參閱 [還原已刪除的項](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
