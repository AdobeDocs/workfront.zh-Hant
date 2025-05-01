---
product-area: projects
navigation-topic: create-projects
title: 從Microsoft專案匯入專案
description: 您可以將專案從Microsoft專案匯入Adobe Workfront，並在一個應用程式中管理您的所有專案。 每次從Microsoft專案匯入專案時，都會在Workfront中建立新專案。
author: Alina
feature: Work Management
exl-id: dcc3c049-245c-4bb7-b819-b75d6d7e5b67
source-git-commit: b38c98ec79617a78c76510bcb109da2ff83247af
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 1%

---

# 從Microsoft專案匯入專案

<!-- Audited: 4/2025 -->

您可以將專案從Microsoft專案匯入Adobe Workfront，並在一個應用程式中管理您的所有專案。 每次從Microsoft專案匯入專案時，都會在Workfront中建立新專案。

>[!IMPORTANT]
>
>並非所有Microsoft專案欄位都會轉移至Workfront。
>
>如需有關Workfront與Microsoft專案之間欄位相容性的詳細資訊，請參閱[將Microsoft專案欄位對應到Adobe Workfront專案](../../../manage-work/projects/manage-projects/map-ms-project-fields-to-workfront.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>新增：標準 </p> 
   或
   <p>目前：計畫 </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級</td> 
   <td> <p>編輯專案的存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>建立專案時，您會自動收到專案的管理許可權 </p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--old permissions model: 

You must have the following access to perform the steps in this article:

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>When you create a project you automatically receive Manage permissions to the project </p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

## 從MS Project建立專案

您可以從&#x200B;**主功能表**&#x200B;中的&#x200B;**專案**&#x200B;區域，或投資組合或方案的&#x200B;**專案**&#x200B;區域建立專案。

1. 登入Microsoft專案，並在Workfront中開啟您要匯入的專案。
1. 按一下&#x200B;**檔案**，然後按&#x200B;**另存新檔**，將專案儲存為.xml檔案。

1. 登入Workfront。
1. 執行下列其中一項：

   * 按一下Workfront右上角的&#x200B;**主功能表** ![主功能表圖示](assets/main-menu-icon.png)，或按一下左上角的&#x200B;**主功能表** ![主功能表行](assets/lines-main-menu.png)。如果可用，請按一下&#x200B;**專案**，然後展開&#x200B;**新專案**。
   * 移至投資組合，然後展開&#x200B;**新專案**。
   * 前往方案，然後展開&#x200B;**新專案**。
   * 如果您是群組管理員，則可以在您管理之群組的&#x200B;**專案**&#x200B;區段中建立專案。 如需詳細資訊，請參閱[建立和修改群組的專案](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md)。

1. 按一下&#x200B;**匯入MS Project**。 **匯入MS檔案**&#x200B;對話方塊就會顯示。

   ![新專案下拉式清單](assets/import-ms-project-option.png)

1. 按一下「**選取檔案**」，然後在電腦上瀏覽您從Microsoft專案匯出的.xml檔案。
1. 匯入選取的檔案。 Workfront會開始匯入程式，並根據從Microsoft專案匯出的檔案建立新專案。

   匯入程式完成後，您會被導向新專案頁面，該頁面會顯示匯入已成功完成的確認訊息。

   >[!NOTE]
   >
   >Workfront對檔案上傳有15分鐘的時間限制。 如果檔案上傳時間超過此時間，我們建議您將專案分割為較小的專案，然後分別匯入這些專案。 將任務匯入Workfront後，請將任務從一個專案移動到另一個專案，以將其合併到一個專案中。 如需關於移動任務的資訊，請參閱[移動任務](../../../manage-work/tasks/manage-tasks/move-tasks.md)。

1. （選用）繼續在Workfront中編輯專案。 如需有關編輯專案的資訊，請參閱[編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md)。


   >[!NOTE]
   >
   >從範本建立的新專案狀態與您的Workfront管理員在&#x200B;**專案偏好設定**&#x200B;區域中定義的狀態相對應，或由群組管理員在&#x200B;**群組專案偏好設定**&#x200B;區域中定義。 如需有關設定專案偏好設定的資訊，請參閱[設定全系統的專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。
