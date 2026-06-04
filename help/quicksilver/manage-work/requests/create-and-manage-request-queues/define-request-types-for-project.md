---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: 定義專案的請求型別
description: 您可以依「請求型別」來組織登入Adobe Workfront的問題或請求型別。
author: Alina
feature: Work Management
exl-id: 627749bb-a8d7-4cc2-9d11-237811f82eb8
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/fOdoie2wI-EHoKmQTHy0cDaVipi6XYE1JgMHdX6-Tbo
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: c10f2e93-7a58-4212-aa24-684c265ebe76
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 354
ht-degree: 7%

---

# 定義專案的請求型別

<!-- Audited: 6/2025 -->

您可以依「請求型別」來組織登入Adobe Workfront的問題或請求型別。 這對於報告原因，以及協助使用者瞭解在專案存留期內可能會發生哪些意外工作非常有用。

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
   <td>
    <p>標準</p>
    <p>規劃</p></td>  
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

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

開始之前，您必須執行下列動作：

* 擁有或建立專案。

  如需有關建立專案的資訊，請參閱[建立專案](../../../manage-work/projects/create-projects/create-project.md)。

## 有關請求型別的考量事項

* 您可以在設定專案的佇列詳細資料區域時，指定可記錄在專案上的問題或請求型別。
* 您不需要讓專案成為請求佇列，就能為專案定義請求型別。 為專案記錄的任何問題都可以標示為不同的請求型別。
* 如果您將佇列主題新增到專案，您必須在每個佇列主題上定義請求型別，以便在新增問題或請求時顯示它。 如需詳細資訊，請參閱[建立佇列主題](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)。

## 定義專案的問題或請求型別

{{step1-to-projects}}

1. 在&#x200B;**專案**&#x200B;頁面上，選取專案。
1. 在左側面板中，按一下&#x200B;**佇列詳細資料**。
1. 在&#x200B;**佇列屬性**&#x200B;區段中，選取您想要用於專案的&#x200B;**要求型別**：
   * 錯誤報告
   * 變更順序
   * 問題
   * 請求

   >[!NOTE]
   >
   >* 您必須至少選取一個請求型別。 您可以選取多種型別。
   >* 您的Workfront管理員可能已重新命名其中的一些選項。 如需詳細資訊，請參閱[設定要求型別](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md)。

1. 按一下「**儲存**」。 當您在任務或專案上輸入新問題，或在向專案提交新請求時（如果專案已啟用為請求佇列），您指定的請求型別將可供選取。
