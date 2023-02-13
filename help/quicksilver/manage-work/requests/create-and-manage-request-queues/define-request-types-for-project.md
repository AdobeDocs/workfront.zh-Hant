---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: 定義專案的請求類型
description: 您可以依請求類型來組織登入Adobe Workfront的問題或請求類型。
author: Alina
feature: Work Management
exl-id: 627749bb-a8d7-4cc2-9d11-237811f82eb8
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 2%

---

# 定義專案的請求類型

您可以依請求類型來組織登入Adobe Workfront的問題或請求類型。

此組織有助於回報原因，並協助使用者了解專案生命週期中可能發生的意外工作類型。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront計畫</a>*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FAdministration_and_Setup%2FAdd_users%2FAccess_levels_and_object_permissions%2Fwf-licenses.html&amp;_LANG=en" target="_blank">Adobe Workfront授權</a>*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯專案的存取權</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理專案的權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

開始之前，您必須

* 擁有或建立專案

   如需建立專案的相關資訊，請參閱 [建立專案](../../../manage-work/projects/create-projects/create-project.md).

## 請求類型的考量事項

* 您可以指定在設定 **隊列詳細資訊** 區域。
* 您不必讓專案成為請求佇列，就能定義專案的請求類型。 針對專案記錄的任何問題，都可以以不同的「請求類型」加上標籤。
* 如果您將佇列主題新增至專案，您必須在每個佇列主題上定義「請求類型」，才能在新增問題或請求時顯示。 如需詳細資訊，請參閱 [建立佇列主題](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

## 定義專案的問題或請求類型

1. 按一下 **專案** 的下限。 ![](assets/main-menu-icon.png)

1. 按一下專案的名稱以開啟它。
1. 在左側面板中，按一下 **隊列詳細資訊**.
1. 在 **隊列屬性** 區段，選取 **請求類型** 你想要這個項目。

   >[!NOTE]
   >
   >您至少必須選取一個請求類型。 您可以選取多個請求類型。

   從下列類型中選取：

   * 錯誤報告
   * 變更順序
   * 問題
   * 請求

   >[!TIP]
   >
   >您的Workfront管理員可能已重新命名其中一些選項。 如需詳細資訊，請參閱 [設定請求類型](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. 按一下&#x200B;**儲存**。

   您指定的請求類型將可用於選擇何時在任務或項目上輸入新問題，或者在將新請求提交到項目時（如果項目作為請求隊列啟用）。
