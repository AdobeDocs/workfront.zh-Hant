---
product-area: projects
navigation-topic: create-projects
title: 從Microsoft專案匯入專案
description: 您可以將專案從Microsoft專案匯入Adobe Workfront，並在一個應用程式中管理您的所有專案。 每次從Microsoft專案匯入專案時，都會在Workfront中建立新專案。
author: Alina
feature: Work Management
exl-id: dcc3c049-245c-4bb7-b819-b75d6d7e5b67
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/drxvgi-xQLjEt5JOL6-MxLdkmVcXxkcXMN14nwmNZvs
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 604
ht-degree: 3%

---

# 從Microsoft專案匯入專案

<!-- Audited: 10/2025 -->

您可以將專案從Microsoft專案匯入Adobe Workfront，並在一個應用程式中管理您的所有專案。 每次從Microsoft專案匯入專案時，都會在Workfront中建立新專案。

>[!IMPORTANT]
>
>並非所有Microsoft專案欄位都會轉移至Workfront。
>
>如需有關Workfront與Microsoft專案之間欄位相容性的詳細資訊，請參閱[將Microsoft專案欄位對應到Adobe Workfront專案](../../../manage-work/projects/manage-projects/map-ms-project-fields-to-workfront.md)。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 封裝</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>標準</p> 
    <p>規劃</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯專案的存取權</p> 
   <p>如果您將專案新增至投資組合或計畫，您必須擁有投資組合和計畫的編輯存取權。</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>建立專案時，您會自動收到專案的管理許可權</p>
   <p>如果您將專案新增至投資組合或方案，您必須擁有投資組合和方案的管理許可權。</p>
   </td> 
    </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--
old permissions model: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard </p> 
   Or
   <p>Current: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>Edit access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>When you create a project you automatically receive Manage permissions to the project </p> </td> 
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

   * 按一下左上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon-left-nav.png)，然後按一下&#x200B;**專案**&#x200B;並展開&#x200B;**新增專案**。
   * 移至投資組合，然後展開&#x200B;**新專案**。
   * 前往方案，然後展開&#x200B;**新專案**。
   * 如果您是群組管理員，則可以在您管理之群組的&#x200B;**專案**&#x200B;區段中建立專案。 如需詳細資訊，請參閱[建立和修改群組的專案](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md)。

1. 按一下&#x200B;**匯入MS Project**。

   ![新專案下拉式清單](assets/import-ms-project-option.png)

   **匯入MS檔案**&#x200B;方塊開啟。

1. 按一下「**選取檔案**」，然後在電腦上瀏覽您從Microsoft專案匯出的.xml檔案。
1. 匯入選取的檔案。 Workfront會開始匯入程式，並根據從Microsoft專案匯出的檔案建立新專案。

   >[!NOTE]
   >
   >Workfront對檔案上傳有15分鐘的時間限制。 如果檔案上傳時間超過此時間，我們建議您將專案分割為較小的專案，然後分別匯入這些專案。 將任務匯入Workfront後，請將任務從一個專案移動到另一個專案，以將其合併到一個專案中。 如需關於移動任務的資訊，請參閱[移動任務](../../../manage-work/tasks/manage-tasks/move-tasks.md)。

   匯入程式完成後，您會被導向新專案頁面，該頁面會顯示匯入已成功完成的確認訊息。

   >[!CAUTION]
   >
   >如果您的Workfront執行個體同時擁有檔案之Workfront和Adobe雲端儲存空間的存取權，則從MS Project匯入專案會建立舊版Workfront儲存空間專案，即使Workfront管理員將Adobe雲端儲存空間設為您系統的預設值亦然。
   >
   >如需詳細資訊，請參閱[專案和相關物件的檔案管理概觀](/help/quicksilver/manage-work/projects/manage-projects/manage-documents-on-projects.md)。


1. （選用）繼續在Workfront中編輯專案。 如需有關編輯專案的資訊，請參閱[編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md)。


   >[!NOTE]
   >
   >從範本建立的新專案狀態與您的Workfront管理員在&#x200B;**專案偏好設定**&#x200B;區域中定義的狀態相對應，或由群組管理員在&#x200B;**群組專案偏好設定**&#x200B;區域中定義。 如需有關設定專案偏好設定的資訊，請參閱[設定全系統的專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。
