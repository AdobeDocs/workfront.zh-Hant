---
title: 配置全局批准設定
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: 身為Adobe Workfront管理員，您可以決定Workfront中核准程式的全域設定。 這些設定會影響您系統中的所有工作項目核准程式。
author: Alina, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2fb0c647-bb6d-46d0-a985-6ab820b4a7f2
source-git-commit: a3cb3d9d340d377e301c98480324bfe8bf507382
workflow-type: tm+mt
source-wordcount: '907'
ht-degree: 2%

---

# 配置全局批准設定

身為Adobe Workfront管理員，您可以決定Workfront中核准程式的全域設定。 這些設定會影響您系統中的所有工作項目核准程式。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>您必須是系統管理員或擁有具有管理權限的計畫許可證，才能管理批准流程</p> <p><b>注意</b>:如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 配置全局批准設定

1. 以Workfront管理員身分登入Workfront 。
1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **程式** > **核准** .

1. 按一下 **設定** 圖示 ![](assets/gear-icon-settings.png) 旁邊 **核准** 區域名稱。

1. 在 **核准設定** 框中，指定以下資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">新增 &lt;number&gt; 計畫完成日期的天數，以適應審批流程</td> 
      <td> <p>指定分鐘、小時、天、周或月數，以將時間添加到需要審批的任務的計畫完成日期。 選擇「已用」分鐘數、小時數、天數或周數以添加時間，這些時間包括系統工作計畫日曆中指定的任何週末、節假日和非工作小時數。</p> 
      <p>例如，如果在星期五分配了任務，且任務的持續時間為3天，則任務完成日期將設定為星期一（假設星期六和星期日是週末）。 如果任務的持續時間為3天（未過），則任務完成日期設定為星期三。</p>
      <p><b>注意</b>:啟用額外時間以適應任務審批將影響任務和項目的時間軸。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">不需要核准者加入專案團隊（用於包含角色的核准程式）</td> 
      <td> <p>如果在審批流程包含角色時不需要審批人加入項目團隊，請選擇此選項。 將批准決策指派給工作角色時，只有在專案中具有與其相關聯角色的使用者才會看到批准。 如果啟用此設定，則具有該作業角色的任何用戶無論是否在項目團隊中，都會收到批准請求。 如需編輯使用者專案角色的相關資訊，請參閱 <a href="../../../manage-work/projects/planning-a-project/manage-project-team.md" class="MCXref xref">管理專案團隊</a>. </p> 
      <p><b>筆尖</b>:將批准指派給角色和選項時 <b>不需要核准者加入專案團隊（用於包含角色的核准程式）</b> 已禁用，但項目組中沒有與批准時的角色匹配的角色，則會將批准重新分配給項目所有者。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">停用核准委派</td> 
      <td> <p>選擇此選項可禁用系統中用戶將批准委託給其他用戶的功能。 選取此選項時，從Workfront移除委派核准的選項，並停止任何現有核准委派。</p> <p>如需在Workfront中委派核准的詳細資訊，請參閱 <a href="../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md" class="MCXref xref">委派核准請求</a> .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">允許在項目、任務或問題處於等待批准狀態時編輯自定義表單</td> 
      <td> <p>選取此選項，可讓使用者在「待核准」狀態下編輯自訂的專案、工作和問題表單。 這是預設設定。</p> 
      <p>選取此選項時：</p> 
       <ul> 
       <li>所有批准者（以及任何有權編輯自定義表單的其他用戶）都可以在對象處於待批准狀態時對自定義表單進行更改，而不管當前的批准路徑或批准步驟如何。</li> 
       <li>在批准過程中對自定義表單所做的更改不會影響在更改之前作出的任何批准決定。</li> 
       <li> <p>對專案、任務或問題所做的任何變更都會以相同方式追蹤，無論此設定為何。 </p> <p>例如，如果您新增要在更新資料流上追蹤的自訂表單欄位，則會在物件的更新資料流上追蹤表單的任何變更。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">允許使用者恢復新建立的等待核准中請求</td> 
      <td> <p>選擇此選項可配置用戶是否可以撤回問題或請求以等待其第一個狀態的批准。 您可以設定請求佇列，將問題或請求的第一個狀態與核准程式建立關聯。 </p> 
      <p>如需請求佇列的詳細資訊，請參閱 <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">建立請求佇列</a>.</p> 
      <p>執行下列任一項作業：</p> 
       <ul> 
       <li>選擇此選項可讓使用者重新調用對問題或請求的第一個狀態的批准。 在此情況下，他們會看到新問題或正在等待批准狀態的請求的「召回」&lt;按鈕。 當他們選擇撤回問題時，將收到警告，說明問題也將被刪除。 在他們確認回訪後，該問題即被刪除。 </li> 
       <li> <p>取消選取此選項，以防止使用者回顧第一個狀態為等待核准的問題或請求。 他們看不到新發行或請求的Recall&lt;按鈕，必須授予批准。 這是預設選項。</p> 
       <p>有關複查等待批准的項目的詳細資訊，請參閱 <a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">查看批准 </a>.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **儲存變更。**
