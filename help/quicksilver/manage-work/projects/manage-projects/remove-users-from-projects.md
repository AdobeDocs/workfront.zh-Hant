---
product-area: projects;user-management
navigation-topic: manage-projects
title: 從專案移除使用者
description: 當使用者不再參與完成專案工作時，您可以從專案中將其移除。
author: Alina
feature: Work Management
exl-id: 3a75c78d-faed-41cd-a0a4-59504bb981af
source-git-commit: afbf2e2fbfcc2c527223da008518bc7632872c23
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 0%

---

# 從專案移除使用者

當使用者不再參與完成專案工作時，您可以從專案中將其移除。 從專案中移除使用者會對任務和問題指派以及專案角色產生影響。 已移除的使用者停止接收專案團隊的通知。 如需有關專案團隊通知的詳細資訊，請參閱[事件通知型別](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md)。

與專案相關聯的使用者會列在專案的「人員」區域中。 他們代表專案團隊。 如需有關專案團隊的詳細資訊，請參閱[專案團隊概觀](../../../manage-work/projects/planning-a-project/project-team-overview.md)。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯專案的存取權</p> <p><b>附註</b>

如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理專案的許可權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 移除使用者對現有任務、問題和專案有何影響

從專案移除使用者時，指派給他們的任何任務或問題可能會受到影響，具體取決於移除使用者時任務或問題是否已完成：

* **若移除使用者時專案尚未完成：**&#x200B;若已指派工作角色，則會重新指派專案給工作角色，或指派專案給使用者正在執行的工作角色。 如果專案或使用者沒有指派工作角色，您必須手動重新指派專案。
* **如果移除使用者時專案已完成：**&#x200B;移除的使用者名稱會保留在專案上。
* **如果移除的使用者也是專案的建立者：**&#x200B;專案並未從他們的&#x200B;**我所在的專案**&#x200B;清單中移除。 該專案會從按「輸入者」欄位篩選該專案的所有其他使用者的清單中移除。
* **如果使用者是專案所有者或贊助者：**&#x200B;使用者仍會保留其專案贊助者或擁有者的角色。

## 從專案和專案團隊中移除使用者

您可以將使用者從專案團隊中移除，將使用者從專案中移除。

當使用者在專案中履行角色時，他們會成為專案團隊的一部分。

當您從使用者在專案中的角色中移除使用者時，他們仍然是專案團隊的一部分。

如需有關專案中使用者角色的資訊，請參閱[管理專案團隊](../planning-a-project/manage-project-team.md)。

若要從專案團隊中移除使用者：

1. 前往您要移除使用者的專案。

1. 按一下左側面板中的&#x200B;**人員**，然後選取您要移除的使用者。 您可能需要按一下「**顯示更多**」，然後按「**人員**」。

1. 按一下使用者清單頂端的&#x200B;**移除**&#x200B;圖示![移除專案](assets/remove-icon---x-in-circle.png)。

1. 按一下&#x200B;**是，移除選取的使用者**&#x200B;以確認移除。

   系統會將使用者從專案團隊中移除，並從其可能受指派的任何未完成任務或問題中移除。 他們不再收到專案團隊適用的通知。
