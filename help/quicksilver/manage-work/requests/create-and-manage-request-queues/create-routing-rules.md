---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: 建立路由規則
description: 路由規則可控制Adobe Workfront在將問題提交至「請求佇列」時如何處理問題。
author: Alina
feature: Work Management, Requests
topic: Collaboration
role: User, Admin
exl-id: 640f9054-f2f8-4594-9311-e93518f58453
source-git-commit: 8ec279ece400c10a37e67664b77b1e0df6639724
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 1%

---

# 建立路由規則

<!-- Audited: 12/2023 -->

路由規則可控制將Adobe Workfront的問題提交至請求佇列時，該如何處理問題。 如需有關建立請求佇列的詳細資訊，請參閱[建立請求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)。

路由規則會將問題傳送給最能解決已提交問題或請求的特定使用者或工作角色。 路由規則通常與佇列主題相關聯，這些主題可用於控制將套用至問題或請求的路由規則。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront計畫</p></td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>新授權： Standard </p> 
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

*如需此表格中資訊的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 建立路由規則

1. 前往您要為請求新增路由規則的專案。
1. 按一下左側面板中的&#x200B;**路由規則**。 您可能需要按一下&#x200B;**顯示更多**，然後按一下&#x200B;**路由規則**。
1. 按一下&#x200B;**新增路由規則**&#x200B;以新增規則。 **新路由規則**&#x200B;方塊開啟。

   ![新路由規則方塊](assets/new-routing-rule-box.png)
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

   提交問題後，您可以編輯其指派並指派其他使用者、角色或團隊。 如需詳細資訊，請參閱<a href="../../../manage-work/issues/manage-issues/assign-issues.md">指派問題</a>。

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>專案路由</strong> </td> 
      <td>這是新增問題的專案。</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >*如果使用者、工作角色或團隊在與路由規則關聯後停用，請求會繼續路由給它們。 您必須定期清查所有路由規則，並將已停用的指派取代為有效指派。

   將問題路由至專案時，擁有問題許可權的使用者會收到在該專案上設定的許可權。 如需有關設定專案許可權的資訊，請參閱[在Adobe Workfront中共用專案](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md)。

1. 按一下「**儲存**」。

   此程式只會定義「路由規則」。 為了確保問題在提交至請求佇列時能夠路由傳送，您必須在&#x200B;**預設路由**&#x200B;下的&#x200B;**佇列詳細資料**&#x200B;索引標籤上選取路由規則。

   如需新增預設路由至要求佇列的詳細資訊，請參閱[建立要求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)。

   如果要將多個路由規則與請求佇列相關聯，您必須建立多個佇列主題，並將每個主題與個別的路由規則相關聯。 如需建立佇列主題的詳細資訊，請參閱[建立佇列主題](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)。
