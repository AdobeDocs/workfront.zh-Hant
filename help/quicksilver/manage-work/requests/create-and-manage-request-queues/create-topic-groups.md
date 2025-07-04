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
source-git-commit: 0da05d048d0dab1c2f06870e589c1349c48ccc58
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# 建立主題群組

<!-- Audited: 2/2024 -->

主題群組與請求佇列相關聯。 您可以使用主題群組，根據請求的性質，將請求佇列分為多個類別。

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
   <td role="rowheader"> <p role="rowheader">Adobe Workfront授權</p> </td> 
   <td>   
      <p>新增：標準</p>
      <p>或</p> 
      <p>目前：計畫</p>
 </td> 
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

## 主題群組概觀

例如，如果您有行銷請求的請求佇列，您可以有「母親節行銷活動」的主題群組、第二層級主題群組「數位媒體」以及額外的第二層級主題群組「印刷媒體」。 然後，您可以在每個主題群組中擁有多個佇列主題。 例如，「橫幅廣告」和「部落格」可以是「數位媒體」主題群組的佇列主題。

如需有關如何建立請求佇列的詳細資訊，請參閱[建立請求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)。

使用主題群組時，請考量下列事項：

* 您可以在請求佇列中建立最多10層主題群組。
* 可與主題群組相關聯的佇列主題數目沒有限制。
* 主題群組是可報告的物件。
* 您無法將主題群組從一個專案移動到另一個專案。

## 建立主題群組

建議您先建立主題群組，再建立佇列主題。 不過，主題群組可在佇列主題產生器中建立。 如需建立佇列主題的詳細資訊，請參閱[建立佇列主題](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)。

若要建立主題群組：

1. 移至您以「說明要求佇列」形式發佈的專案。\
   如需將專案發佈為說明要求佇列的詳細資訊，請參閱[建立要求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)。

1. 按一下左側面板中的&#x200B;**主題群組**。
1. 按一下&#x200B;**新增主題群組**。

   <!--   ![](assets/new-topic-group-box-nwe-350x306.png) -->

1. 指定下列資訊：

   * **名稱**：向此請求佇列提交請求的使用者可以看到此名稱。
   * **描述**：當使用者在提交新請求的過程中選取主題群組時，會顯示描述。
   * **新增至主題群組**：您可以將新的主題群組新增至現有主題群組，也可以直接新增至以「說明要求佇列」形式發佈的專案。

1. 按一下「**儲存**」。\
   這會在您的請求佇列中建立新的主題群組。 您現在可以從「請求佇列」下的第一個下拉式功能表中選取其他類別。\
   如需有關提交請求的詳細資訊，請參閱[建立並提交Adobe Workfront請求](../../../manage-work/requests/create-requests/create-submit-requests.md)。
1. 若要編輯現有的主題群組，請從「主題群組」清單中選取「主題群組」，然後在開啟的視窗中編輯詳細資訊。 按一下[儲存]儲存變更。**&#x200B;**
