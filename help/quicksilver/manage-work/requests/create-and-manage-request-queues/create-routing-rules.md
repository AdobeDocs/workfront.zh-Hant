---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: 建立路由規則
description: 路由規則可控制Adobe Workfront在將問題提交至請求佇列時，對問題的處理方式。 如需有關建立請求佇列的詳細資訊，請參閱建立請求佇列。
author: Alina
feature: Work Management, Requests
topic: Collaboration
role: User, Admin
exl-id: 640f9054-f2f8-4594-9311-e93518f58453
source-git-commit: c5053b78dd80fe9017ba96e193e59fbd9b17e7c8
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 2%

---

# 建立路由規則

路由規則可控制Adobe Workfront在將問題提交至請求佇列時，對問題的處理方式。 如需建立「請求佇列」的詳細資訊，請參閱 [建立請求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

路由規則會將問題傳送給最能解決已提交問題或請求的特定使用者或工作角色。 路由規則通常與佇列主題相關聯，這些主題用於控制將套用至問題或請求的路由規則。

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
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯專案的存取權</p> <p><b>附註</b>

如果您仍然沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p> 管理專案的許可權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要瞭解您擁有的計畫、授權型別或存取權，請聯絡Workfront管理員

## 建立路由規則

1. 前往您要為請求新增路由規則的專案。
1. 按一下 **路由規則** 在左側面板中。 您可能需要按一下 **顯示更多**，則 **路由規則**.
1. 按一下 **新增路由規則** 以新增規則。
1. 指定「路由規則」的下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>名稱</strong> </td> 
      <td> <p>路由規則的名稱。 如果您有存取權檢視專案的這項資訊，則可以檢視路由規則。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>說明</strong> </td> 
      <td>新增路由規則的說明。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>預設受指派人*</strong> </td> 
      <td>新增應指派新問題的作用中使用者或作用中工作角色。 此欄位中只能有一個預設受指派人。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>預設團隊*</strong> </td> 
      <td>新增新問題應指派給的活躍團隊。 此欄位中只能有一個預設團隊。

   <p><b>附註</b></p>

   提交問題後，您可以編輯其指派並指派其他使用者、角色或團隊。 如需詳細資訊，請參閱  <a href="../../../manage-work/issues/manage-issues/assign-issues.md">指派問題 </a>.

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
   >*如果使用者、工作角色或團隊在與路由規則關聯後停用，請求會繼續路由到它們。 您必須定期清查所有製程規則，並將已停用的指派替換為有效指派。

   將問題路由至專案時，擁有該問題許可權的使用者會獲得在該專案上設定的許可權。 如需關於設定專案許可權的資訊，請參閱 [在Adobe Workfront中共用專案](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

   ![](assets/new-routing-rule-box-nwe-350x419.png)

1. 按一下&#x200B;**儲存**。

   此程式只會定義路由規則。 為確保問題在提交至請求佇列時能夠被路由，您必須在 **佇列詳細資訊** 標籤下的 **預設路由**.

   如需將「預設路由」新增至請求佇列的詳細資訊，請參閱 [建立請求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

   如果要將多個路由規則與請求佇列相關聯，您必須建立多個佇列主題，並將每個主題與個別的路由規則相關聯。 如需建立佇列主題的詳細資訊，請參閱 [建立佇列主題](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).
