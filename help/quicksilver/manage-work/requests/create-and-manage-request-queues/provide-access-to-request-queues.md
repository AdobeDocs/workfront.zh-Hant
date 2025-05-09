---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: 提供請求佇列的存取權
description: 提供請求佇列的存取權時，您可決定組織中的哪個人員可以在Adobe Workfront的「請求」區域中檢視請求佇列。
author: Alina
feature: Work Management
exl-id: eb88c32a-f8b8-42d3-9a3a-72c62fd1dc3a
source-git-commit: 3d96d7b7073ad194f291afe370ae813d3482bc9e
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 0%

---

# 提供請求佇列的存取權

提供請求佇列的存取權時，您可決定組織中的哪個人員可以在Adobe Workfront的「請求」區域中檢視請求佇列。

您可以根據使用者是專案團隊、專案群組或專案公司的一員，提供不同使用者對請求佇列的存取權。 您也可以讓系統中的每個人都能存取請求佇列。

在邀請外部利益關係人加入Workfront並希望限制使用者對特定區域的存取的組織中，這會很有用；在此情況下，僅對與專案公司或群組相關聯的使用者開放的請求佇列會限制外部利益關係人的可見度。 將存取權授與任何人，會讓內部和外部利害關係人都看到請求。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> 
   <p>新授權： Standard </p>
   或
   <p>目前授權：計畫 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯專案的存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p> 管理專案的許可權</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

在請求區域中使用者可以使用請求佇列之前，您必須建立具有以下設定的專案：

* 將其指定為請求佇列。 如需有關建立請求佇列的詳細資訊，請參閱[建立請求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)。
* 將專案狀態更新為目前。

## 提供請求佇列的存取權

1. 前往您想要提供請求佇列存取權的專案。

   >[!NOTE]
   >
   >請求區域中只會顯示具有目前狀態的專案。

1. 按一下左側面板中的&#x200B;**佇列詳細資料**。
1. 選取&#x200B;**發佈為說明要求佇列**，將專案指定為要求佇列。
1. 從下列選項中選取：

   * **任何人**：任何使用者都可以檢視及新增要求至要求佇列。
   * **擁有此專案檢視存取許可權的人員**：擁有專案檢視許可權的使用者可以檢視及新增要求佇列。
   * **此專案的公司中的人員**：與專案的公司相關聯的使用者可以檢視及新增要求。 與此專案相關聯的公司會列在此選項旁的括弧中。
   * **此專案群組的人員**：與專案群組相關聯的使用者可以檢視及新增要求。 與此專案關聯的群組會列在此選項旁的括弧中。

     當多個部門共用一個Workfront帳戶以實現獨特的組織目標時，群組佇列會很有用。 每個部門可能有自己的佇列，其他群組的成員應該看不到這些佇列。

     如需關於誰擁有專案許可權的資訊，請參閱[在Adobe Workfront中共用專案](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md)。\
     編輯專案時，群組和公司可以與專案相關聯。 如需有關編輯專案的詳細資訊，請參閱[編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md)。

1. 按一下「**儲存**」。
