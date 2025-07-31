---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: 建立佇列主題
description: 「佇列主題」可與「路由規則」搭配使用，以自動將內送工作指派給使用者、工作角色、專案團隊，或將其置於專案上。 「佇列主題」定義要實作「路由規則」所需存在的條件。
author: Alina
feature: Work Management, Requests
role: User, Admin
exl-id: 65a74698-011f-4caa-9739-d7510faeb66f
source-git-commit: 81b40eda8536d1a63c38a297d92158a12f9d350e
workflow-type: tm+mt
source-wordcount: '937'
ht-degree: 2%

---

# 建立佇列主題

<!-- Audited: 12/2023 -->

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它只能在「預覽Sandbox」環境中使用。</span>

「佇列主題」可與「路由規則」搭配使用，以自動將內送工作指派給使用者、工作角色、專案團隊，或將其置於專案上。 「佇列主題」定義要實作「路由規則」所需存在的條件。

可指派給主題群組或專案的佇列主題數量沒有限制。 佇列主題是可報告的物件型別。

您可以為個別專案或專案範本建立佇列主題。

建立後，您無法將佇列主題從一個專案或範本移動到另一個專案或範本。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

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

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 建立佇列主題

1. 建立路由規則、主題群組和自訂表單（如果您計畫將它們與佇列主題相關聯）。\
   如需如何建立路由規則、主題群組或自訂表單的詳細資訊，請參閱下列文章：

   * [建立路由規則](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)
   * [建立主題群組](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md)
   * [建立自訂表格](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)

1. 移至您選擇啟用為「說明要求佇列」的專案或範本，以及您想要建立新佇列主題的位置。\
   如需如何將專案指定為說明要求佇列的詳細資訊，請參閱[建立要求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)。

   您可以在「主題群組」下組織相關的「佇列主題」。 這會在提出要求時，為要求者提供一系列下拉式功能表。

   或

   您可以直接在指定為「說明請求佇列」的專案下巢狀內嵌佇列主題，而不需要主題群組。

   如需有關建立主題群組的資訊，請參閱[建立主題群組](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md)。

1. 按一下左側面板中的&#x200B;**佇列主題**。
1. 按一下&#x200B;**新增佇列主題**。
1. 在&#x200B;**新佇列主題**&#x200B;表單上，輸入下列內容：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>名稱</strong> </td> 
      <td> 佇列主題的名稱。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>說明</strong> </td> 
      <td>說明請求佇列。 使用者在提交新請求的過程中選取佇列主題時，便會顯示說明。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>新增至主題群組</strong> </td> 
      <td> 如果專案中沒有「主題群組」，專案名稱會預設為「主題群組」。<br>如果您想要在這裡建立其他主題群組，請從下拉式功能表中選取<strong>建立新主題群組</strong>。<br><img src="assets/create-new-topic-group-within-queue-topic-350x203.png" alt="create_new_topic_group_within_queue_topic.png" style="width: 350;height: 203;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>自訂表單</strong> </td> 
      <td>選取您要與佇列主題關聯的任何自訂表單。 您必須先建立問題的自訂表單，然後才能將其與佇列主題相關聯。 如需建立自訂表單的相關資訊，請參閱<a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">建立自訂表單</a>。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>預設核准</strong></td> 
      <td> <p>將核准流程與此佇列主題相關聯。 此下拉式選單中只會顯示問題核准流程。 提交至此佇列的所有問題都將與此核准流程相關聯。 您的Adobe Workfront管理員必須定義系統層級的核准流程，然後才能將其與佇列主題相關聯。 <span>擁有核准流程管理存取許可權的使用者也可以建立群組特定的核准流程。</span>如需建立核准流程的詳細資訊，請參閱<a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">建立工作專案的核准流程</a>。<br></p> 
       <div> 
        <p>重要：如果專案的群組變更，則附加至現有問題的群組特定核准流程會變成單一使用核准流程。 如需關於專案群組的變更或核准程式變更如何影響核准設定的詳細資訊，請參閱<a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">群組和核准程式變更如何影響指派的核准程式</a>。</p> 
        <p>將核准流程新增至佇列主題時，請考量下列事項： </p> 
        <ul style="list-style-type: circle;"> 
         <li>清單中只會顯示有效的核准流程。 </li> 
         <li> <p>系統範圍及群組特定的核准程式會顯示在清單中。 與專案群組以外的群組相關聯的核准程式不會顯示在清單中。</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>預設期間</strong> </td> 
      <td>這是請求的預設持續時間，系統會根據此值計算請求的「計畫完成日期」。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>預設路由</strong> </td> 
      <td>指定您要與「佇列主題」關聯的路由規則。 您必須先建立路由規則，才能將其附加至佇列主題。 如需詳細資訊，請參閱<a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md">建立路由規則</a>。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>要求型別</strong> </td> 
      <td> <p>選擇此佇列主題儲存的請求型別。 可見的選項是在專案的<strong>佇列詳細資料</strong>索引標籤上設定的。 這是必填欄位。 </p> 
       <p><b>附註</b>：</p>
      <p>只有在「佇列詳細資訊」和「佇列主題」頁面中同時選取「請求型別」時，「型別」才會顯示為「請求」區域的選取專案。 如需有關設定專案佇列詳細資料區域的資訊，請參閱<a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">建立請求佇列</a>。 </p> <p>從下列型別中選取：</p> 
       <ul> 
        <li>錯誤報告</li> 
        <li>變更順序</li> 
        <li>問題</li> 
        <li>請求</li> 
       </ul> <p>您的Workfront管理員可能已重新命名其中的一些選項。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![新佇列主題方塊](assets/new-queue-topic-box.png)

1. 按一下「**儲存**」。\
   佇列主題現在可供使用，並在選取請求佇列和主題群組後，顯示在Workfront的請求區域中。

## 編輯佇列主題

編輯現有的佇列主題：

1. 移至包含您要編輯之佇列主題的專案或範本。
1. 按一下左側面板中的&#x200B;**佇列主題**。
1. 在生產環境中，選取您要編輯的佇列主題。 在開啟的詳細資訊頁面上，按一下&#x200B;**編輯佇列主題**。
   <!--1. <span class="preview">In the Preview environment, select the Queue Topic that you want to edit, then click the Edit icon ![Edit icon](assets/edit-icon.png).</span>-->

