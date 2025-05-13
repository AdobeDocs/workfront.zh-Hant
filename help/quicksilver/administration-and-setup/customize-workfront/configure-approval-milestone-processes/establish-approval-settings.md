---
title: 設定全域核准設定
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: 作為Adobe Workfront管理員，您可以決定Workfront中核准流程的全域設定。 這些設定會影響您系統中的所有工作專案核准流程。
author: Alina, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2fb0c647-bb6d-46d0-a985-6ab820b4a7f2
source-git-commit: 1397702a6b50953e7abcfe491b95aeb8b981df5b
workflow-type: tm+mt
source-wordcount: '879'
ht-degree: 2%

---

# 設定全域核准設定

作為Adobe Workfront管理員，您可以決定Workfront中核准流程的全域設定。 這些設定會影響您系統中的所有工作專案核准流程。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td>規劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>您必須是系統管理員或擁有對核准流程具有管理存取權的計畫授權</p> <p><b>注意</b>：如果您還是沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

+++

## 設定全域核准設定

{{step-1-to-setup}}

1. 按一下&#x200B;**處理序** > **核准**。

1. 按一下&#x200B;**核准**&#x200B;區域名稱旁的&#x200B;**設定**&#x200B;圖示![齒輪設定圖示](assets/gear-icon-settings.png)。

1. 在出現的&#x200B;**核准設定**&#x200B;方塊中，指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">新增&lt;number&gt;天數至計畫完成日期，以配合核准流程</td> 
      <td> <p>指定分鐘、小時、天、周或月數，以將時間新增至需要核准之任務的計畫完成日期。 選取「經過的時間」分鐘、小時、天或周，以新增時間，包括系統工作排程行事曆中指定的任何週末、假日及非工作小時。</p> 
      <p>例如，如果任務指派在星期五且持續時間為3天，則任務完成日期設定為星期一（假設星期六和星期日是週末）。 如果任務的持續時間為3天（未過），則任務完成日期設定為星期三。</p>
      <p><b>注意</b>：啟用新增額外時間以因應任務核准將會影響任務與專案的時間表。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">當核准程式包含角色時，專案團隊中不需要有核准者</td> 
      <td> <p>如果核准流程包含角色時，不需要專案團隊中的核准者，請選取此選項。 不論使用者是否屬於專案團隊，擁有該工作角色的任何使用者都會收到核准請求，但不會自動授予他們專案的存取權。 如需有關編輯使用者專案角色的資訊，請參閱<a href="../../../manage-work/projects/planning-a-project/manage-project-team.md" class="MCXref xref">管理專案團隊</a>。 </p> 
      <p><b>秘訣</b>：當您指派核准給角色，且專案團隊中不需要有選項<b>核准者（針對包含角色的核准程式）</b>已停用，但專案團隊中沒有符合核准角色的角色，核准就會重新指派給專案所有者。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">停用核准委派</td> 
      <td> <p>選取此選項可停用系統中的使用者將核准委派給其他使用者的功能。 選取此選項時，會從Workfront移除委派核准的選項，並停止任何現有的核准委派。</p> <p>如需在Workfront中委託核准的詳細資訊，請參閱<a href="../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md" class="MCXref xref">委託核准要求</a> 。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">允許在專案、任務或問題處於未決核准狀態時編輯自訂表單</td> 
      <td> <p>選擇此選項可允許使用者在處於未決核准狀態時編輯專案、任務和問題的自訂表單。 這是預設設定。</p> 
      <p>選取此選項時：</p> 
       <ul> 
       <li>物件處於未決核准狀態時，無論目前的核准路徑或核准步驟為何，所有核准者（以及有權編輯自訂表單的任何其他使用者）都可以變更自訂表單。</li> 
       <li>在核准流程期間對自訂表單進行的變更不會影響變更前所做的任何核准決定。</li> 
       <li> <p>無論此設定為何，對專案、任務或問題所做的任何變更都會以相同的方式進行追蹤。 </p> <p>例如，如果您新增要在更新流上追蹤的自訂表單欄位，對表單的任何變更都會在物件的更新流上追蹤。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">允許使用者恢復新建立的等待核准中請求</td> 
      <td> <p>選取此選項可設定使用者是否可以撤回問題，或針對其第一個狀態而等待核准的請求。 您可以設定請求佇列，將問題或請求的第一個狀態與核准流程相關聯。 </p> 
      <p>如需請求佇列的詳細資訊，請參閱<a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">建立請求佇列</a>。</p> 
      <p>執行下列其中一項：</p> 
       <ul> 
       <li>選取此選項可讓使用者恢復對問題或請求的第一個狀態的核准。 在這種情況下，他們可以在新問題或處於未決核准狀態的請求上看到「撤消」&lt;按鈕。 當他們選擇召回問題時，將會收到警告訊息，指出問題也會被刪除。 問題在確認他們將其召回後即會刪除。 </li> 
       <li> <p>取消選取此選項可防止使用者重新呼叫第一個狀態為未決核准的問題或請求。 他們看不到新問題或請求上的「撤消」&lt;按鈕，且必須獲得核准。 這是預設選項。</p> 
       <p>如需複查等待核准之專案的詳細資訊，請參閱<a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">檢視核准</a>。</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**儲存變更。**
