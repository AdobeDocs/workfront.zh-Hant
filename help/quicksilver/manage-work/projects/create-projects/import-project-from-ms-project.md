---
product-area: projects
navigation-topic: create-projects
title: 從Microsoft專案匯入專案
description: 您可以將專案從Microsoft專案匯入Adobe Workfront，並在一個應用程式中管理您的所有專案。 每次從Microsoft專案匯入專案時，都會在Workfront中建立新專案。
author: Alina
feature: Work Management
exl-id: dcc3c049-245c-4bb7-b819-b75d6d7e5b67
source-git-commit: 32966d4732221d73aa3397771e157b630f7d5760
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 1%

---

# 從Microsoft專案匯入專案

您可以將專案從Microsoft專案匯入Adobe Workfront，並在一個應用程式中管理您的所有專案。 每次從Microsoft專案匯入專案時，都會在Workfront中建立新專案。

>[!IMPORTANT]
>
>並非所有Microsoft專案欄位都會轉移至Workfront。
>
>如需有關Workfront與Microsoft專案之間欄位相容性的詳細資訊，請參閱 [將Microsoft專案欄位對應至Adobe Workfront專案](../../../manage-work/projects/manage-projects/map-ms-project-fields-to-workfront.md).

## 存取需求

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
   <td> <p>新授權： Standard </p> 
   或
   <p>目前授權：計畫 </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級*</td> 
   <td> <p>編輯專案的存取權</p> <p><b>附註</b>

如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需有關存取專案的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">授予專案存取權</a>. 如需有關Workfront管理員如何變更您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>建立專案時，您會自動收到專案的管理許可權 </p> <p> 如需有關專案許可權的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">在Adobe Workfront中共用專案</a>.</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

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

您可以從主要功能表的「專案」區域，或從投資組合或方案的專案區域建立專案。

1. 前往Microsoft專案，並在Workfront中開啟您要匯入的專案。
1. 按一下 **檔案**，然後 **另存為** 將專案儲存為.xml檔案。

1. 登入Workfront。
1. 執行下列任一項作業：

   * 按一下 **主要功能表** ![](assets/main-menu-icon.png)，按一下 **專案**，然後展開 **新增專案**.
   * 前往投資組合，然後展開 **新增專案**.
   * 前往程式，然後展開 **新增專案**.
   * 如果您是群組管理員，您也可以在您管理之群組的專案區段中建立專案。 如需詳細資訊，請參閱 [建立和修改群組的專案](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

1. 選擇 **匯入MS Project** 選項。

   ![](assets/new-project-dropdown-nwe-350x358.png)

1. 按一下 **選取檔案**，然後瀏覽電腦上您從Microsoft專案匯出的.xml檔案。
1. 匯入選取的檔案。

   Workfront會開始匯入程式，並根據從Microsoft專案匯出的檔案建立新專案。

   匯入程式完成後，您會被導向新專案頁面，該頁面會顯示匯入已成功完成的確認訊息。

   >[!NOTE]
   >
   >Workfront對檔案上傳有15分鐘的時間限制。 如果檔案上傳時間超過此時間，我們建議您將專案分割為較小的專案，然後分別匯入這些專案。 將任務匯入Workfront後，請將任務從一個專案移動到另一個專案，以將其合併到一個專案中。 有關移動任務的資訊，請參閱 [移動任務](../../../manage-work/tasks/manage-tasks/move-tasks.md).

1. （選用）繼續在Workfront中編輯專案。 如需有關編輯專案的資訊，請參閱 [編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md).

   從範本建立的新專案狀態與您的Workfront管理員在專案偏好設定區域中定義的狀態相對應，或由群組管理員在群組專案偏好設定區域中定義。 如需有關設定專案偏好設定的資訊，請參閱 [設定全系統專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
