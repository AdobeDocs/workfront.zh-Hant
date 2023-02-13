---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: 建立主題群組
description: 主題組與請求隊列關聯。 它們可讓您根據請求的性質，將請求佇列分層為多個類別。
author: Alina
feature: Work Management
exl-id: 7c5959f4-f33f-4f5e-b031-748dbe1a24a5
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# 建立主題群組

主題組與請求隊列關聯。 它們可讓您根據請求的性質，將請求佇列分層為多個類別。

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

## 主題群組概觀

例如，如果您有行銷請求的請求佇列，則可以有「母親日促銷活動」的主題群組、第二層主題群組「數位媒體」，以及另一層主題群組「列印媒體」。 然後，每個主題組內可以有多個隊列主題。 例如，「橫幅廣告」和「部落格」可以是「數位媒體」主題群組的佇列主題。

如需如何建立請求佇列的詳細資訊，請參閱 [建立請求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

>[!TIP]
>
>* 您可以在「請求佇列」中建立最多10層的「主題群組」。
>* 可與主題組關聯的隊列主題數沒有限制。
>* 主題組是可報告的對象。
>


## 建立主題群組

建議您先建立主題群組，再建立佇列主題。 不過，您可以在佇列主題產生器中建立主題群組。 如需建立佇列主題的詳細資訊，請參閱 [建立佇列主題](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

建立主題組：

1. 前往您以「說明請求佇列」形式發佈的專案。\
   如需將專案發佈為「說明請求佇列」的詳細資訊，請參閱 [建立請求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. 按一下 **主題群組** 中。 您可能需要按一下 **顯示更多**，然後 **主題群組**.
1. 按一下 **新主題組**.

   ![](assets/new-topic-group-box-nwe-350x306.png)

1. 指定下列資訊：

   * **名稱**:向此請求佇列提交請求的使用者可以看到名稱。
   * **說明**:當使用者在提交新請求的過程中選取主題群組時，便會顯示說明。
   * **添加到主題組**:您可以將新主題組添加到現有主題組，也可以直接將其添加到作為幫助請求隊列發佈的項目。

1. 按一下&#x200B;**儲存**。\
   這會在您的請求佇列中建立新的主題群組。 您現在可以從「請求佇列」下的第一個下拉式功能表選取其他類別。\
   如需提交請求的詳細資訊，請參閱 [建立及提交Adobe Workfront請求](../../../manage-work/requests/create-requests/create-submit-requests.md).
