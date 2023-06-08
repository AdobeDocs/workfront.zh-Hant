---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: 定義專案的請求型別
description: 您可以依「請求型別」組織登入Adobe Workfront的問題或請求型別。
author: Alina
feature: Work Management
exl-id: 627749bb-a8d7-4cc2-9d11-237811f82eb8
source-git-commit: 9b6552fe496a1602786cdc6b6050d02cd367a531
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 2%

---

# 定義專案的請求型別

您可以依「請求型別」組織登入Adobe Workfront的問題或請求型別。

這個組織適合用於製作報表，以及協助使用者瞭解在專案存留期內可能會發生哪些非預期的工作。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront計畫</a>*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md">授權總覽</a>*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯專案的存取權</p> <p><b>附註</b>

如果您仍然沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理專案的許可權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 必要條件

在開始之前，您必須執行下列動作：

* 擁有或建立專案

  如需關於建立專案的資訊，請參閱 [建立專案](../../../manage-work/projects/create-projects/create-project.md).

## 請求型別的相關考量事項

* 您可以指定在設定時可登入專案的問題或請求型別。 **佇列詳細資訊** 專案區域。
* 您不需要讓專案成為請求佇列，就能為專案定義請求型別。 為專案記錄的任何問題都可以標示為不同的請求型別。
* 如果您將佇列主題新增至專案，您必須在每個佇列主題上定義請求型別，以便在新增問題或請求時顯示它。 如需詳細資訊，請參閱 [建立佇列主題](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

## 定義專案的問題或請求型別

1. 按一下 **專案** 在主要功能表中。 ![](assets/main-menu-icon.png)

1. 按一下專案名稱以開啟。
1. 在左側面板中，按一下 **佇列詳細資訊**.
1. 在 **佇列屬性** 區段，選取 **請求型別** 您想要專案的。

   >[!NOTE]
   >
   >您必須至少選取一個請求型別。 您可以選取多個請求型別。

   從下列型別中選取：

   * 錯誤報告
   * 變更順序
   * 問題
   * 請求

   >[!TIP]
   >
   >您的Workfront管理員可能已重新命名其中的一些選項。 如需詳細資訊，請參閱 [設定請求型別](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. 按一下&#x200B;**儲存**。

   當您在任務或專案中輸入新問題時，或當您向專案提交新請求時（如果專案已啟用為請求佇列），您指定的請求型別將可供選取。
