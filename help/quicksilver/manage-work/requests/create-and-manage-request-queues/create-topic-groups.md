---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: 建立主題群組
description: 主題群組與請求佇列相關聯。 它們可讓您根據請求的性質，將請求佇列分為多個類別。
author: Alina
feature: Work Management, Requests
topic: Collaboration
role: User, Admin
exl-id: 7c5959f4-f33f-4f5e-b031-748dbe1a24a5
source-git-commit: c5053b78dd80fe9017ba96e193e59fbd9b17e7c8
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# 建立主題群組

主題群組與請求佇列相關聯。 它們可讓您根據請求的性質，將請求佇列分為多個類別。

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
   <td role="rowheader"> <p role="rowheader">Adobe Workfront授權*</p> </td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯專案的存取權</p> <p>注意：如果您仍然沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p> 管理專案的許可權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡Workfront管理員

## 主題群組概觀

例如，如果您有行銷請求的請求佇列，您可以有一個「母親節行銷活動」主題群組、一個二級主題群組「數位媒體」，以及一個額外的二級主題群組「印刷媒體」。 然後，您可以在每個主題群組中擁有多個佇列主題。 例如，「橫幅廣告」和「部落格」可以是「數位媒體」主題群組的佇列主題。

如需有關如何建立請求佇列的詳細資訊，請參閱 [建立請求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

>[!TIP]
>
>* 您可以在請求佇列中建立最多10層主題群組。
>* 可與主題群組相關聯的佇列主題數目沒有限制。
>* 主題群組是可報告的物件。
>

## 建立主題群組

建議您先建立主題群組，再建立佇列主題。 不過，您可在佇列主題產生器中建立主題群組。 如需建立「佇列主題」的詳細資訊，請參閱 [建立佇列主題](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

若要建立主題群組：

1. 前往您以「說明請求佇列」形式發佈的專案。\
   如需將專案發佈為說明請求佇列的詳細資訊，請參閱 [建立請求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. 按一下 **主題群組** 在左側面板中。 您可能需要按一下 **顯示更多**，則 **主題群組**.
1. 按一下 **新增主題群組**.

   ![](assets/new-topic-group-box-nwe-350x306.png)

1. 指定下列資訊：

   * **名稱**：向此請求佇列提交請求的使用者可看見該名稱。
   * **說明**：使用者在提交新請求的過程中選取主題群組時，系統會顯示說明。
   * **新增至主題群組**：您可以將新的主題群組新增至現有主題群組，也可以直接新增至作為說明請求佇列發佈的專案。

1. 按一下&#x200B;**儲存**。\
   這會在您的請求佇列中建立新的主題群組。 您現在可以從「請求佇列」下方的第一個下拉式選單中選取其他類別。\
   如需提交請求的詳細資訊，請參閱 [建立並提交Adobe Workfront請求](../../../manage-work/requests/create-requests/create-submit-requests.md).
