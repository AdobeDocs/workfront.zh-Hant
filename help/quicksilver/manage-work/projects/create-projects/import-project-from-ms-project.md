---
product-area: projects
navigation-topic: create-projects
title: 從Microsoft專案匯入專案
description: 您可以將Microsoft專案的專案匯入Adobe Workfront，並在一個應用程式中管理所有專案。 每次您從Microsoft專案匯入專案時，都會在Workfront中建立新專案。
author: Alina
feature: Work Management
exl-id: dcc3c049-245c-4bb7-b819-b75d6d7e5b67
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 2%

---

# 從Microsoft專案匯入專案

您可以將Microsoft專案的專案匯入Adobe Workfront，並在一個應用程式中管理所有專案。 每次您從Microsoft專案匯入專案時，都會在Workfront中建立新專案。

>[!IMPORTANT]
>
>並非所有Microsoft專案欄位都會轉移至Workfront。
>
>如需Workfront與Microsoft專案之間欄位相容性的詳細資訊，請參閱 [將Microsoft專案欄位對應至Adobe Workfront專案](../../../manage-work/projects/manage-projects/map-ms-project-fields-to-workfront.md).

## 存取需求

為寶潔起草：

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
   <td> <p>當前許可證：標準 </p> 
   或
   <p>舊版授權：計畫 </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級*</td> 
   <td> <p>編輯專案的存取權</p> <p><b>附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需存取專案的相關資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">授予專案的存取權</a>. 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>建立專案時，您會自動收到專案的「管理」權限 </p> <p> 如需專案權限的相關資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">在Adobe Workfront中共用專案</a>.</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

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
   <td> <p>編輯專案的存取權</p> <p><b>附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需存取專案的相關資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">授予專案的存取權</a>. 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>建立專案時，您會自動收到專案的「管理」權限 </p> <p> 如需專案權限的相關資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">在Adobe Workfront中共用專案</a>.</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 從MS項目建立項目

您可以從「主菜單」中的「項目」區域，或從產品組合或方案的「項目」區域建立項目。

1. 前往Microsoft專案，開啟您要在Workfront中匯入的專案。
1. 按一下 **檔案**，然後 **另存新檔** 將項目另存為.xml檔案。

1. 登入Workfront。
1. 執行下列任一項作業：

   * 按一下 **主菜單** ![](assets/main-menu-icon.png)，按一下 **專案**，然後展開 **新增專案**.
   * 前往產品組合，然後展開 **新增專案**.
   * 前往程式，然後展開 **新增專案**.
   * 如果您是群組管理員，也可以在您管理之群組的「專案」區段中建立專案。 如需詳細資訊，請參閱 [建立和修改群組的專案](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

1. 選擇 **導入MS項目** 選項。

   ![](assets/new-project-dropdown-nwe-350x358.png)

1. 按一下 **選擇檔案**，然後瀏覽您從Microsoft專案匯出的電腦上的.xml檔案。
1. 匯入選取的檔案。

   Workfront會開始匯入程式，並根據從Microsoft專案匯出的檔案建立新專案。

   匯入程式完成後，您會被導向至新專案頁面，其中會顯示匯入已成功完成的確認。

   >[!NOTE]
   >
   >Workfront對檔案上傳有15分鐘的時間限制。 如果檔案上傳所花的時間超過此時間，建議您將專案分解為較小的專案，並個別匯入。 將任務匯入Workfront後，將任務從一個專案移至另一個專案，將任務合併為一個專案。 有關移動任務的資訊，請參見 [移動任務](../../../manage-work/tasks/manage-tasks/move-tasks.md).

1. （選用）繼續編輯Workfront中的專案。 如需編輯專案的相關資訊，請參閱 [編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md).

   從模板建立的新項目的狀態與「項目首選項」區域中的Workfront管理員或「組項目首選項」區域中的組管理員定義的狀態相對應。 如需設定專案偏好設定的相關資訊，請參閱 [配置系統範圍的項目首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
