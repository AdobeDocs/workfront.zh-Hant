---
product-area: documents;user-management;resource-management
navigation-topic: comment-on-a-proof
title: 標籤要共用校訂的使用者
description: 當您在校訂檢視器中對校訂發表評論時，您可以標籤其他使用者，以透過電子郵件提請他們注意您的評論，並將他們新增到校訂的工作流程中。
author: Courtney
feature: Digital Content and Documents
exl-id: 4efbfdeb-3834-48dd-aa5b-515891bac519
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 0%

---

# 標籤要共用校訂的使用者

當您在校訂檢視器中對校訂發表評論時，您可以標籤其他使用者，以透過電子郵件提請他們注意您的評論，並將他們新增到校訂的工作流程中。

在校訂的評論中標籤使用者時，您可以標籤的使用者可能會因各種因素而異，例如個別使用者許可權和您在組織中的成員資格：

* 如果您是校訂建立者、擁有者或已啟用特定許可權，您可以在校訂工作流程之外標籤使用者並與他們共用校訂。
* 如果您是以外部使用者的身分新增到校訂中，並且您是另一個環境的成員，具有不同的校訂帳戶，則您只能標籤來自原始環境的那些使用者。<!--For more information, see [Proofing collaboration limitations with people outside of your organization](../../../../review-and-approve-work/proofing/tips-tricks-and-troubleshooting/collaboration-with-members-outside-of-your-organization.md)-->

## 存取需求 {#access-requirements}

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td><p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>任何</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">校訂角色</td> 
   <td>作者，版主</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">校樣權限設定檔</td> 
   <td>監督員或管理員</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯檔案的存取權</p></td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 標籤要共用校訂的使用者

擁有上述[存取需求](#access-requirements)區段中概述之校訂許可權設定檔或校訂角色的使用者，預設可標籤使用者以共用校訂。 如果您是校訂擁有者或建立者，則無論校訂許可權設定檔或校訂角色為何，您都可以標籤使用者以共用校訂。 您可以讓擁有較低校訂許可權設定檔或校訂角色的使用者在建立校訂時標籤使用者以共用校訂。 如需詳細資訊，請參閱[使用基本工作流程建立進階校訂](../../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md#configur)文章中的[設定工作流程並新增檢閱者](../../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)區段。

>[!NOTE]
>
>只有符合下列其中一項條件時，您才能使用外部共同作業人員的電子郵件地址來標籤該人員：
>
>* 貴組織Workfront帳戶中的使用者先前已將共同作業人員的電子郵件地址新增至校訂。
>* 共同作業人員先前曾使用電子郵件地址在您組織的Workfront帳戶中訂閱校訂。

若要在評論中標籤某人並共用校訂：

1. 當您註解校訂時，輸入at sign (@)，後接人員名稱或電子郵件地址。 當您開始輸入時，可用的名稱會出現在下拉式清單中。
1. 當您在下拉式清單中看到人員時，請選取該人員的名稱。

   >[!TIP]
   >
   >如果您要關閉下拉式清單而不選取任何人，可以按&#x200B;**Esc**&#x200B;鍵或按一下清單之外的任何位置。

1. 對您要在註解中標籤的任何其他使用者重複步驟1至2。
1. 完成註解，然後按一下&#x200B;**貼文**。
1. （視條件而定）如果您已標籤尚未新增至校訂的任何人，請為顯示的方塊中列出的每個使用者指定&#x200B;**校訂角色**&#x200B;和&#x200B;**電子郵件警示**&#x200B;設定，然後按一下&#x200B;**新增人員並張貼評論**。

   ![新增人員到校訂](assets/add-people-to-proof-350x220.png)

   如需校訂角色的相關資訊，請參閱。 如需有關校訂電子郵件警示的資訊，請參閱文章[在Workfront Proof中設定電子郵件通知設定](../../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md)中的章節。

   如果校樣具有自動化工作流程，則您標籤的使用者會新增至您所在的階段。 如需詳細資訊，請參閱[自動化工作流程總覽](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md)。

   您標籤的任何人都會收到有關校樣評論的通知電子郵件，無論他們使用何種校樣電子郵件警報設定：

   * 如果使用者收到每日摘要或每小時摘要電子郵件，Workfront會單獨傳送通知，並在摘要電子郵件中包含有關您的校樣評論的資訊。
   * 如果使用者收到所有活動的警示或對其評論的回覆，則通知會取代有關這些評論和回覆的通知。

如需其他將使用者新增至校訂方式的相關資訊，請參閱[在Adobe Workfront中共用校訂](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)。
