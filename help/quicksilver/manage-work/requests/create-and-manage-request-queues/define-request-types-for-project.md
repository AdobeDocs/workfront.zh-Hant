---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: 定義專案的請求型別
description: 您可以依「請求型別」來組織登入Adobe Workfront的問題或請求型別。
author: Alina
feature: Work Management
exl-id: 627749bb-a8d7-4cc2-9d11-237811f82eb8
source-git-commit: 6311526ddf9143c4a979d8bbac96312a3b0e8151
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 2%

---

# 定義專案的請求型別

您可以依「請求型別」來組織登入Adobe Workfront的問題或請求型別。

這個組織適合用於製作報表，以及協助使用者瞭解在專案存留期內可能會發生哪些非預期工作。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

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
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>
    <p>新增：標準</p>
    <p>或</p>
    <p>目前：計畫</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯專案的存取權</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理專案的許可權</p></td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

開始之前，您必須執行下列動作：

* 擁有或建立專案

  如需有關建立專案的資訊，請參閱[建立專案](../../../manage-work/projects/create-projects/create-project.md)。

## 有關請求型別的考量事項

* 當您設定專案的&#x200B;**佇列詳細資料**&#x200B;區域時，可以指定可登入專案的問題或要求型別。
* 您不需要讓專案成為請求佇列，就能為專案定義請求型別。 為專案記錄的任何問題都可以標示為不同的請求型別。
* 如果您將佇列主題新增到專案，您必須在每個佇列主題上定義請求型別，以便在新增問題或請求時顯示它。 如需詳細資訊，請參閱[建立佇列主題](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)。

## 定義專案的問題或請求型別

{{step1-to-projects}}

1. 按一下專案名稱以開啟。
1. 在左側面板中，按一下&#x200B;**佇列詳細資料**。
1. 在&#x200B;**佇列屬性**&#x200B;區段中，選取您想要用於專案的&#x200B;**要求型別**。

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
   >您的Workfront管理員可能已重新命名其中的一些選項。 如需詳細資訊，請參閱[設定要求型別](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md)。

1. 按一下「**儲存**」。

   當您在任務或專案上輸入新問題時，或當您向專案提交新請求時（如果專案已啟用為請求佇列），您指定的請求型別將可供選取。
