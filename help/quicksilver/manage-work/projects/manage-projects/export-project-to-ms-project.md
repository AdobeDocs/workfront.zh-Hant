---
product-area: projects
navigation-topic: manage-projects
title: 將專案匯出至Microsoft專案
description: 您可以將Adobe Workfront專案匯出至Microsoft專案。
author: Alina
feature: Work Management
exl-id: 3f0f3644-a763-4b72-a93a-85af8626b5b3
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 0%

---

# 將專案匯出至Microsoft專案

您可以將Adobe Workfront專案匯出至Microsoft專案。 

>[!IMPORTANT]
>
>* 並非所有Workfront欄位都在Microsoft專案檔案中轉移。\
>  如需有關Workfront與Microsoft專案之間欄位相容性的詳細資訊，請參閱文章[將Microsoft專案欄位對應到Adobe Workfront專案](../../../manage-work/projects/manage-projects/map-ms-project-fields-to-workfront.md)。
>* 我們建議您限制將專案從一個應用程式傳輸到另一個應用程式的次數。 
>

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
   <td>  <p>Current license: Light or higher</p>
   Or
   <p>Legacy license: Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> View or higher permissions to the project</p> <p>For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
您必須具有下列存取權才能執行本文中的步驟：

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
   <td> <p>評論或以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>檢視或更高專案存取權</p> <p><b>附註</b>

如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需有關存取專案的資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">授予專案的存取權</a>。 如需Workfront管理員如何變更存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。 </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p> 檢視專案或更高的許可權</p> <p>如需有關專案許可權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">在Adobe Workfront中共用專案</a>。</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 將專案從Workfront匯出至Microsoft專案

您可以從專案頁面、專案清單或報表，從Workfront匯出專案。

1. 前往您要匯出的專案，然後按一下專案名稱右側的&#x200B;**更多**&#x200B;圖示![更多功能表](assets/qs-more-menu.png)

   ![更多下拉式清單](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   或

   前往專案清單或報告，並選取專案，然後按一下清單頂端的「更多」圖示![「更多」功能表](assets/qs-more-menu.png)。

   ![其他功能表已展開](assets/more-menu-expanded-in-a-list-one-project-selected-nwe.png)

1. 按一下&#x200B;**匯出MS Project**。

   專案會下載為XML檔案至您的電腦，且已準備好匯入Microsoft專案。 
