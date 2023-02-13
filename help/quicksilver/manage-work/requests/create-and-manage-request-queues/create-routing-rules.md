---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: 建立路由規則
description: 路由規則控制Adobe Workfront在將問題提交至請求佇列時會如何處理。 如需建立請求佇列的詳細資訊，請參閱建立請求佇列。
author: Alina
feature: Work Management
exl-id: 640f9054-f2f8-4594-9311-e93518f58453
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 2%

---

# 建立路由規則

路由規則可控制Adobe Workfront在將問題提交至請求佇列時會如何處理的問題。 如需建立請求佇列的詳細資訊，請參閱 [建立請求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

路由規則將問題發送給最適合解決提交問題或請求的特定用戶或作業角色。 路由規則通常與隊列主題關聯，隊列主題用於控制將應用於問題或請求的路由規則。

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
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯專案的存取權</p> <p><b>附註</b>

如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p> 管理專案的權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員

## 建立工藝路線規則

1. 轉到要為請求添加路由規則的項目。
1. 按一下 **路由規則** 中。 您可能需要按一下 **顯示更多**，然後 **路由規則**.
1. 按一下 **新的路由規則** 來新增新規則。
1. 為工藝路線規則指定以下資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>名稱</strong> </td> 
      <td> <p>路由規則的名稱。 如果您有權查看項目上的此資訊，則可以查看工藝路線規則。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>說明</strong> </td> 
      <td>為路由規則添加說明。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>預設受指派人*</strong> </td> 
      <td>新增應指派新問題的作用中使用者或作用中工作角色。 此欄位中只能有一個預設受託人。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>預設團隊*</strong> </td> 
      <td>新增應指派新問題的作用中團隊。 此欄位中只能有一個預設團隊。

   <p><b>附註</b></p>

   提交問題後，您可以編輯其分配並指派其他用戶、角色或團隊。 如需詳細資訊，請參閱  <a href="../../../manage-work/issues/manage-issues/assign-issues.md">指派問題 </a>.

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
   >*如果使用者、工作角色或團隊在與路由規則相關聯後被停用，則請求會繼續路由至這些請求。 您必須定期清點所有工藝路線規則，並將停用的分配替換為有效分配。

   將問題路由至專案時，擁有問題權限的使用者會收到該專案所設定的權限。 如需關於設定專案權限的資訊，請參閱 [在Adobe Workfront中共用專案](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

   ![](assets/new-routing-rule-box-nwe-350x419.png)

1. 按一下&#x200B;**儲存**。

   此過程僅定義路由規則。 為確保問題在提交至請求佇列時已路由，您必須在 **隊列詳細資訊** 標籤 **預設路由**.

   有關將預設路由添加到請求隊列的資訊，請參閱 [建立請求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

   如果要將多個路由規則與請求隊列關聯，必須建立多個隊列主題，並將每個隊列主題與單獨的路由規則關聯。 如需建立佇列主題的詳細資訊，請參閱 [建立佇列主題](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).
