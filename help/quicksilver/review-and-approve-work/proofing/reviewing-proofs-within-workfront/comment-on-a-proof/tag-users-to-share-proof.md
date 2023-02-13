---
product-area: documents;user-management;resource-management
navigation-topic: comment-on-a-proof
title: 標籤使用者以共用校樣
description: 當您在校對檢視器中評論校樣時，可以標籤其他使用者，透過電子郵件將其注意力吸引到您的評論，並將其新增至校樣的工作流程。
author: Courtney
feature: Digital Content and Documents
exl-id: 4efbfdeb-3834-48dd-aa5b-515891bac519
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '708'
ht-degree: 0%

---

# 標籤使用者以共用校樣

當您在校對檢視器中評論校樣時，可以標籤其他使用者，透過電子郵件將其注意力吸引到您的評論，並將其新增至校樣的工作流程。

在校樣的註解中標籤使用者時，您可以標籤的使用者可能會因各種因素而異，例如個別使用者權限和您在組織中的成員資格：

* 如果您是校樣建立者、擁有者或已啟用特定權限，您可以在校樣工作流程之外標籤使用者，並與他們共用校樣。
* 如果您是以外部使用者身分新增至校樣，且您是另一個環境的成員，且有不同校樣帳戶，則您只能從原始環境中標籤這些使用者。 <!--For more information, see [Proofing collaboration limitations with people outside of your organization](../../../../review-and-approve-work/proofing/tips-tricks-and-troubleshooting/collaboration-with-members-outside-of-your-organization.md)-->

## 存取需求 {#access-requirements}

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>當前計畫：Pro或更高</p> <p>或</p> <p>舊計畫：Premium</p> <p>如需使用不同計畫校對存取權限的詳細資訊，請參閱 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">存取Workfront中的校對功能</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>當前計畫：工作或計畫</p> <p>舊計畫：任何（您必須為使用者啟用校對）</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">證明角色</td> 
   <td>作者、主持人</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">校訂權限設定檔 </td> 
   <td>主管或管理員</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對文檔的訪問</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、角色或校樣權限設定檔，請聯絡您的Workfront或Workfront Proof管理員。

## 標籤使用者以共用校樣

具有校樣權限設定檔或校樣角色的使用者，如 [存取需求](#access-requirements) 依預設，上方的區段可標籤使用者來共用校樣。 如果您是校樣擁有者或建立者，您也可以標籤使用者以共用校樣，無論「校樣權限設定檔」或「校樣」角色為何。 您可以讓具有較低「校樣權限設定檔」或「校樣」角色的使用者，在建立校樣時，標籤使用者來共用校樣。 如需詳細資訊，請參閱 [配置工作流程並添加審核者](../../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md#configur) 區段 [使用基本工作流程建立進階校樣](../../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md) 文章。

>[!NOTE]
>
>僅當以下任一條件為真時，才能使用外部協作者的電子郵件地址標籤外部協作者：>
>* 您組織的Workfront帳戶中的使用者先前已將共同作業者的電子郵件地址新增至校樣。
>* 合作者先前曾使用電子郵件地址在貴組織的Workfront帳戶中訂閱校樣。
>


在評論中標籤某人並共用校樣：

1. 在您對校樣發表評論時，請輸入at符號(@)，後面接著人員的姓名或電子郵件地址。 開始輸入時，可用名稱會顯示在下拉式清單中。
1. 在下拉式清單中看到人員名稱時，請選取該人員的名稱。

   >[!TIP]
   >
   >如果要關閉下拉式清單而不選取任何人，可以按 **Esc** 鍵，或按一下清單外的任意位置。

1. 對於要在註解中標籤的任何其他使用者，重複步驟1至2。
1. 完成注釋，然後按一下 **貼文**.
1. （條件性）如果您標籤了尚未新增至校樣的任何人，請指定 **證明角色** 和 **電子郵件警報** 針對顯示方塊中所列的每個使用者進行設定，然後按一下 **新增人員和貼文留言**.

   ![](assets/add-people-to-proof-350x220.png)

   如需校樣角色的相關資訊，請參閱。 如需校樣電子郵件警報的相關資訊，請參閱文章中的區段 [在Workfront Proof中設定電子郵件通知設定](../../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).

   如果校樣有「自動化工作流程」，則您標籤的使用者會新增至您所在的階段。 如需詳細資訊，請參閱 [自動化工作流程概觀](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

   您標籤的任何人，無論其使用的校樣電子郵件警報設定為何，都會收到有關您校樣留言的通知電子郵件：

   * 如果使用者收到每日摘要或每小時的摘要電子郵件，Workfront會個別傳送通知，並在摘要電子郵件中加入您的校樣註解相關資訊。
   * 如果使用者收到所有活動的警報，或收到對其留言的回覆，則通知會取代這些留言和回覆的通知。

如需將使用者新增至校樣的其他方式的相關資訊，請參閱 [在Adobe Workfront內共用證明](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).
