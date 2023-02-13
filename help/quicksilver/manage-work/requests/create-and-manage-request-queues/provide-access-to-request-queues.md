---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: 提供對請求隊列的訪問
description: 當您提供請求佇列的存取權時，可決定組織中的哪些人可以在Adobe Workfront的「請求」區域中檢視請求佇列。
author: Alina
feature: Work Management
exl-id: eb88c32a-f8b8-42d3-9a3a-72c62fd1dc3a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# 提供對請求隊列的訪問

當您提供請求佇列的存取權時，可決定組織中的哪些人可以在Adobe Workfront的「請求」區域中檢視請求佇列。

您可以根據不同的使用者是專案團隊、專案群組或專案公司的成員，提供「請求佇列」的不同存取權。 您也可以提供系統中每個人對請求佇列的存取權。 

在邀請外部利害關係人加入Workfront且希望限制使用者存取特定區域的組織中，這個用法很有用，在此情況下，請求佇列會僅開放給與公司或專案群組相關聯的使用者，而局限外部利害關係人可見。 讓任何人都能存取，讓內部和外部持份者都能查看要求。

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯專案的存取權</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p> 管理專案的權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員

## 必要條件

在「請求」區域中的「請求佇列」可供使用者使用前，您必須先建立專案，並具備下列設定：

* 將其指定為請求佇列。 如需建立請求佇列的詳細資訊，請參閱 [建立請求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
* 將項目的狀態更新為當前狀態。

## 提供請求佇列的存取權

1. 前往您要提供請求佇列存取權的專案。

   >[!NOTE]
   >
   >「請求」區域中只會顯示狀態為「目前」的專案。

1. 按一下 **隊列詳細資訊** 中。 您可能需要按一下 **顯示更多**，然後 **隊列詳細資訊**.
1. 選擇 **發佈為說明請求佇列** 將專案指定為「請求佇列」。
1. 從下列選項中選取：

   * **任何人**:任何使用者都可以檢視請求，以及將請求新增至請求佇列。
   * **有權查看此項目的人員**：擁有專案檢視權限的使用者可以檢視請求，以及將請求新增至請求佇列。 
   * **此項目公司的人員**：與專案公司相關聯的使用者可以檢視及新增請求。 與項目關聯的公司列在此選項旁的括弧中。 
   * **此項目組中的人員**：與專案群組相關聯的使用者可以檢視及新增請求。 與項目關聯的組列在此選項旁的括弧中。

      若有幾個部門共用Workfront帳戶以達成獨特的組織目標，群組佇列就十分實用。 每個部門可能都有自己的隊列，其他組的成員不能看到這些隊列。

      如需誰擁有專案權限的相關資訊，請參閱 [在Adobe Workfront中共用專案](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).\
      編輯專案時，群組和公司可與專案相關聯。 如需編輯專案的詳細資訊，請參閱 [編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md).

1. 按一下&#x200B;**儲存**。
