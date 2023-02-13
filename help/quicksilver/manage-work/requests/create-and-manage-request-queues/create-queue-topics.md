---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: 建立佇列主題
description: 排隊主題與路由規則一起工作，以自動將傳入的工作分配給用戶、作業角色、團隊，或將其放在項目上。 隊列主題定義了要實施路由規則所需存在的條件。
author: Alina
feature: Work Management
exl-id: 65a74698-011f-4caa-9739-d7510faeb66f
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '885'
ht-degree: 3%

---

# 建立佇列主題

排隊主題與路由規則一起工作，以自動將傳入的工作分配給用戶、作業角色、團隊，或將其放在項目上。 隊列主題定義了要實施路由規則所需存在的條件。

可分配給主題組或項目的隊列主題數沒有限制。 佇列主題是可報告的物件類型。

## 存取需求

<!--drafted - replace table with P&P:

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
   <td> <p>Edit access to Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
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
   <td> <p>編輯專案的存取權</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p> 管理專案的權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員

## 建立佇列主題

1. 如果您計畫將路由規則、主題組和自定義表單與隊列主題關聯，請建立該規則、主題組和自定義表單。\
   有關如何建立路由規則、主題組或自定義表單的詳細資訊，請參閱以下文章：

   * [建立路由規則](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)
   * [建立主題群組](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md)
   * [建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

1. 轉至您選擇以「說明請求佇列」形式啟用的專案，以及您要建立新佇列主題的位置。\
   有關如何將項目指定為幫助請求隊列的詳細資訊，請參閱以下文章：\
   [建立請求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)

   您可以在主題組下或直接在指定為幫助請求隊列的項目下組織相關隊列主題。 這會在提出要求時提供要求者一系列的下拉式功能表。\
   您可以直接在指定為「說明請求佇列」的專案下巢狀內嵌「佇列主題」，不含「主題群組」。

   如需建立主題群組的相關資訊，請參閱 [建立主題群組](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).

1. 按一下 **佇列主題** 中。 您可能需要按一下 **顯示更多**，然後 **佇列主題**.
1. 按一下 **新隊列主題**.
1. 在 **新隊列主題** 表單中指定以下內容：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>名稱</strong> </td> 
      <td> 隊列主題的名稱。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>說明</strong> </td> 
      <td>說明請求佇列。 當使用者在提交新請求的過程中選取佇列主題時，便會顯示說明。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>新增至主題群組</strong> </td> 
      <td> 如果專案中沒有「主題群組」，專案的名稱會預設為「主題群組」。<br>如果要從此處建立其他主題組，請選擇 <strong>建立新主題組</strong> 從下拉式功能表。<br><img src="assets/create-new-topic-group-within-queue-topic-350x203.png" alt="create_new_topic_group_within_queue_topic.png" style="width: 350;height: 203;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>自訂表單</strong> </td> 
      <td>選擇要與隊列主題關聯的任何自定義表單。 您必須先建立問題的自訂表單，才能將問題與佇列主題建立關聯。 如需建立自訂表單的相關資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">建立或編輯自訂表單</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">預設核准</td> 
      <td> <p>將批准流程與此隊列主題關聯。 此下拉式功能表中只會顯示「核准核准程式」。 提交到此隊列的所有問題都將與此批准進程關聯。 您的Adobe Workfront管理員必須先定義系統層級的核准程式，才能將它們與佇列主題建立關聯。 <span>具有管理存取權的核准程式使用者也可以建立群組專屬的核准程式。</span> 如需建立核准程式的詳細資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">建立工作項的審批流程</a>.<br></p> 
       <div> 
        <p>重要：如果項目組發生更改，附加到現有問題的特定於組的審批流程將變成一次性審批流程。 有關項目組的更改或審批流程中的更改如何影響審批設定的詳細資訊，請參閱 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">組和審批流程更改如何影響分配的審批流程</a>.</p> 
        <p>將核准程式新增至佇列主題時，請考量下列事項： </p> 
        <ul style="list-style-type: circle;"> 
         <li>清單中只會顯示作用中的核准程式。 </li> 
         <li> <p>清單中顯示系統範圍和組特定的批准流程。 與項目組以外的組相關聯的審批流程不會顯示在清單中。</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>預設期間</strong> </td> 
      <td>這是請求的預設持續時間，請求的計畫完成日期會根據此值計算。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>預設路線</strong> </td> 
      <td>指定要與「隊列主題」關聯的路由規則。 必須先建立路由規則，才能將其附加到隊列主題。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>請求類型</strong> </td> 
      <td> <p>選擇此隊列主題儲存的請求類型。 可見選項設定在 <strong>隊列詳細資訊</strong> 頁簽。 這是必填欄位。 </p> <p>注意：只有在「佇列詳細資料」和「佇列主題」頁面皆已選取「請求類型」時，「請求類型」才會顯示為「請求」區域中的選取項目。 有關設定項目的「隊列詳細資訊」區域的資訊，請參閱 <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">建立請求佇列</a>. </p> <p>從下列類型中選取：</p> 
       <ul> 
        <li>錯誤報告</li> 
        <li>變更順序</li> 
        <li>問題</li> 
        <li>請求</li> 
       </ul> <p>您的Workfront管理員可能已重新命名其中一些選項。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/new-queue-topic-box-nwe-350x375.png)

1.  
1. 按一下&#x200B;**儲存**。\
   選取「請求佇列」和「主題群組」後，佇列主題現在可供使用，並可顯示在Workfront的「請求」區域中。
