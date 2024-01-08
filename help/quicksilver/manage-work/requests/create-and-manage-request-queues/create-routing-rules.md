---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: 建立路由規則
description: 路由規則可控制Adobe Workfront在將問題提交至「請求佇列」時如何處理問題。 如需有關建立請求佇列的詳細資訊，請參閱建立請求佇列。
author: Alina
feature: Work Management, Requests
topic: Collaboration
role: User, Admin
exl-id: 640f9054-f2f8-4594-9311-e93518f58453
source-git-commit: 16a34e4315d508e31859e962edd01026d01ee193
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 1%

---

# 建立路由規則

<!-- Audited: 12/2023 -->

路由規則可控制將Adobe Workfront的問題提交至請求佇列時，該如何處理問題。 如需建立「請求佇列」的詳細資訊，請參閱 [建立請求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

路由規則會將問題傳送給最能解決已提交問題或請求的特定使用者或工作角色。 路由規則通常與佇列主題相關聯，這些主題可用於控制將套用至問題或請求的路由規則。

## 存取需求

<!--drafted - replace the table at P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何 </p> </td> 
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
   <td> <p>編輯專案的存取權</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p> 管理專案的許可權</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 建立路由規則

1. 移至您要為請求新增路由規則的專案。
1. 按一下 **路由規則** 在左側面板中。 您可能需要按一下 **顯示更多**，然後 **路由規則**.
1. 按一下 **建立路由規則** 以新增規則。
1. 輸入「路由規則」的下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>名稱</strong> </td> 
      <td>路由規則的名稱。 如果您有權檢視專案的這項資訊，則可以檢視路由規則。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>說明</strong> </td> 
      <td>新增路由規則的描述。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>預設受指派人*</strong> </td> 
      <td>新增應指派新問題的作用中使用者或作用中工作角色。 此欄位中只能有一個預設受指派人。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>預設團隊*</strong> </td> 
      <td>新增應指派新問題的作用中團隊。 此欄位中只能有一個預設團隊。

   <p><b>附註</b></p>

   提交問題後，您可以編輯其指派並指派其他使用者、角色或團隊。 如需詳細資訊，請參閱  <a href="../../../manage-work/issues/manage-issues/assign-issues.md">指派問題</a>.

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>專案路線</strong> </td> 
      <td>這是新增問題的專案。</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >*如果使用者、工作角色或團隊在與路由規則關聯後停用，請求會繼續路由給它們。 您必須定期清查所有路由規則，並將已停用的指派取代為有效指派。

   將問題路由至專案時，擁有問題許可權的使用者會收到在該專案上設定的許可權。 如需關於設定專案許可權的資訊，請參閱 [在Adobe Workfront中共用專案](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

   ![新路由規則方塊](assets/new-routing-rule-box.png)

1. 按一下「**儲存**」。

   此程式只會定義「路由規則」。 為確保問題在提交至請求佇列時路由傳送，您必須在 **佇列詳細資訊** 標籤下的 **預設路由**.

   如需有關將「預設路由」新增至請求佇列的資訊，請參閱 [建立請求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

   如果要將多個路由規則與請求佇列相關聯，您必須建立多個佇列主題，並將每個主題與個別的路由規則相關聯。 如需有關建立佇列主題的詳細資訊，請參閱 [建立佇列主題](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).
