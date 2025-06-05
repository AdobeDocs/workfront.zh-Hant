---
product-area: projects
navigation-topic: manage-issues
title: 刪除問題
description: 如果您有正確的存取權和許可權，可以刪除Adobe Workfront中的問題或請求。
author: Alina
feature: Work Management
exl-id: 31cc802f-7fa6-420c-8494-a45313df1f10
source-git-commit: aa2bef064df3ff7dd9e4fd896ac7482df3c55e32
workflow-type: tm+mt
source-wordcount: '716'
ht-degree: 1%

---

# 刪除問題

<!--Audited: 05/2025-->

如果您有正確的存取權和許可權，可以刪除Adobe Workfront中的問題或請求。

>[!TIP]
>
>在Workfront中，「問題」和「要求」可互換使用。 您可以同時記錄專案和任務的問題，以指出需要解決的無法預見的工作。 您也可以在指定為「請求佇列」的專案上提交記錄為問題的請求。

## 存取需求

+++ 展開以檢視存取需求。

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
   <td> <p>新增：投稿人或更高版本</p>
   <p>目前：要求或以上</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯問題的存取權</p> <p>檢視專案和任務的或更高存取權</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理問題的許可權</p> <p>專案或任務的貢獻或較高許可權</p> </td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 刪除問題的考量

* 您的Workfront管理員或群組管理員必須在您的專案偏好設定區域中啟用刪除狀態為「完成」的專案中的問題。

  如需有關設定專案偏好設定的資訊，請參閱[設定全系統的專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

* 如果問題已記錄時數，Workfront管理員或群組管理員必須透過在您的Workfront執行個體中設定任務和問題偏好設定，以允許刪除這些問題。 當您嘗試刪除有記錄時數問題的專案時，這也適用。

  如需有關啟用刪除記錄時數之問題的詳細資訊，請參閱[設定系統範圍的任務和問題偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)中的「刪除」一節。


## 刪除問題的影響

當您刪除問題時，會影響連結至問題的其他物件。

當您刪除問題時，也會刪除附加到問題的下列物件：

* 文件

  您無法刪除檔案已簽出並附加於其上的問題。 如需簽出檔案的詳細資訊，請參閱[簽出檔案](../../../documents/managing-documents/check-out-documents.md)。

* 附註
* 核准

視您的Workfront或群組管理員在Workfront執行個體的&#x200B;**時程表和小時偏好設定**&#x200B;中設定專案、任務或問題刪除偏好設定的方式而定，在刪除問題時，會以下列其中一種方式處理問題的記錄小時：

* 移至專案，日後若問題恢復，將無法還原問題。
* 將予以刪除，如果問題在稍後時間恢復，則會在問題上恢復。

  當您嘗試刪除擁有已記錄時數任務的專案時，這也適用。

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">(this is not possible in classic)</span>
  </MadCap:conditionalText>
  -->

  如需有關為登入問題時數設定刪除偏好設定的詳細資訊，請參閱[設定時程表和時數偏好設定](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)。

* 指派給問題或問題核准的使用者仍保留在專案團隊中。\
  如需專案團隊的詳細資訊，請參閱[專案團隊概述](../../../manage-work/projects/planning-a-project/project-team-overview.md)。

## 刪除問題

### 同時刪除專案中的多個問題  {#delete-multiple-issues-in-a-project-simultaneously}

1. 移至&#x200B;**主功能表**。
1. 按一下&#x200B;**專案**。
1. 按一下包含您要刪除之問題的專案名稱。
1. 按一下左側面板中的&#x200B;**問題**。

   與所選專案相關的問題清單會在右側顯示。
1. 在清單中選取一或多個問題，然後按一下清單頂端的&#x200B;**刪除**&#x200B;圖示![刪除圖示](assets/delete.png)。

1. 如果允許刪除，請按一下&#x200B;**刪除**。

   您的Workfront管理員可能不允許刪除記錄時數的問題。\
   如需有關刪除問題所需的存取權和許可權的詳細資訊，請參閱本文中的[刪除問題的考量事項](#considerations-for-deleting-issues)一節。

### 刪除單一問題 {#delete-a-single-issue}

{{step1-to-projects}}

1. 按一下包含您要刪除之問題的專案名稱。
1. 按一下左側面板中的&#x200B;**問題**。

   左側面板中的![問題區段](assets/qs-issues-icon-highlighted-on-project-350x278.png)

1. 按一下您要刪除的問題名稱。
1. 按一下問題名稱右側的&#x200B;**更多**&#x200B;功能表。

   ![問題更多功能表](assets/qs-issue-more-menu-highlighted-350x469.png)

1. 按一下&#x200B;**刪除問題**。
1. 如果允許刪除，請按一下&#x200B;**刪除**。

   您的Workfront管理員可能不允許刪除記錄時數的問題。\
   如需有關刪除問題所需的存取權和許可權的詳細資訊，請參閱本文中的[刪除問題的考量事項](#considerations-for-deleting-issues)一節。

## 還原已刪除的問題

Workfront或群組管理員可在問題刪除後30天內將其還原。

如需有關在Workfront中還原專案的詳細資訊，請參閱[還原已刪除的專案](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md)。
