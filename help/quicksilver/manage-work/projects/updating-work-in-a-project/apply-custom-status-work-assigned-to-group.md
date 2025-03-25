---
product-area: projects
navigation-topic: update-work-in-a-project
title: 將狀態套用至與群組相關聯的工作
description: 如果專案與群組相關聯，您可以將系統層級狀態以及與該群組相關聯的自訂狀態套用至該專案上的專案、任務或問題。
author: Alina
feature: Work Management
exl-id: 7564ab6a-8ddf-4e76-8e45-d59f9cf8d38b
source-git-commit: 15ddf6b4d82ccc694ec7a6c60d8e2d5b6b3645d6
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 0%

---

# 將狀態套用至與群組相關聯的工作

<!--
Alina, I moved this out of an admin article about statuses (Create and customize statuses)
-->

如果專案與群組相關聯，您可以將系統層級狀態以及與該群組相關聯的自訂狀態套用至專案，或套用至該專案上的任務和問題。 如需Adobe Workfront中群組狀態的詳細資訊，請參閱[建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)。

>[!TIP]
>
>您只能將專案與群組建立關聯。 問題和任務會從他們所屬的專案繼承群組。

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
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td> <p>規劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯專案的存取權</p> <p><b>附註</b>

如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理專案的許可權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 更新專案群組和狀態

當您更新專案的群組時，任務、問題或專案狀態可用的選項會變更為符合群組。

1. 移至專案或建立新專案，如[建立專案](../../../manage-work/projects/create-projects/create-project.md)中所述。
1. 按一下&#x200B;**更多**&#x200B;圖示![更多圖示](assets/more-icon.png)，然後按一下&#x200B;**編輯**。

1. 在顯示的&#x200B;**編輯專案**&#x200B;方塊中，在&#x200B;**概觀**&#x200B;區段底部附近，選取&#x200B;**群組**&#x200B;下拉式功能表中的群組。

1. 在&#x200B;**狀態**&#x200B;下拉式功能表中，選取自訂狀態。

   >[!NOTE]
   >
   >如果您在&#x200B;**群組**&#x200B;下拉式功能表中選取不同的群組，**狀態**&#x200B;功能表中的自訂狀態會自動變更，以便與新的群組建立關聯。
   >
   >
   >以專案](assets/status-drop-down-expanded-with-custom-statuses-for-project-nwe.png)的自訂狀態展開的![狀態下拉式清單   >
   >

1. 選取專案狀態。 您建立並套用至該群組的自訂狀態會顯示在清單中。
