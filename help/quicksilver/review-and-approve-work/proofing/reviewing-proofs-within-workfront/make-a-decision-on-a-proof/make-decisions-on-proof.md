---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: 在校訂檢視器中對校訂做出決定
description: 您可以直接在校訂檢視器中對校訂做出決定。
author: Courtney
feature: Digital Content and Documents
exl-id: cf74ac54-b8c1-4404-b35f-2aa94831ecad
source-git-commit: 8af531868249f609113af6d2a8465af01edcbc3f
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 2%

---

# 在校訂檢視器中對校訂做出決定

您可以直接在校訂檢視器中對校訂做出決定。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>目前計畫：Pro或更高版本</p> <p>或</p> <p>舊版計畫：選擇或Premium</p> <p>如需有關不同方案的校訂存取許可權的詳細資訊，請參閱<a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">存取Workfront中的校訂功能</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>目前計畫：工作或計畫</p> <p>舊版計畫：任何（您必須為使用者啟用校訂）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">校樣權限設定檔 </td> 
   <td>經理或以上</td> 
  </tr> 
  <tr> 
   <td role="rowheader">校訂角色</td> 
   <td>核准者、檢閱者和核准者、作者、版主</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯檔案的存取權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、角色或校訂許可權設定檔，請連絡您的Workfront或Workfront Proof管理員。

+++

## 在校訂檢視器中對校訂做出決定

1. 前往包含檔案的專案、任務或問題，然後選取「**檔案**」。
1. 尋找您需要的校訂，然後按一下&#x200B;**開啟校訂**。

1. 按一下校訂檢視器頂端中央的&#x200B;**做出決定**。

1. 在出現的&#x200B;**校訂決定**&#x200B;方塊中，按一下下列決定之一：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">已核准</td> 
      <td>校訂已準備就緒，可移至自動化工作流程的下一個階段。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">已核准 (附帶變更)</td> 
      <td>校訂需要一些變更，但在修訂移至自動化工作流程的下一個階段之前，您不需要檢視修訂版本。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">所需變更</td> 
      <td>校訂需要變更，並且您必須先檢視其他修訂專案，才能移至自動化工作流程的下一個階段。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">不相關</td> 
      <td>證明與您無關，您不需要做出決定。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">自訂決定</td> 
      <td> <p>在「選取」與「進階」計畫上，Workfront管理員或Workfront Proof管理員可以重新命名、重新排序和隱藏決策。 如需詳細資訊，請參閱<a href="../../../../workfront-proof/wp-acct-admin/account-settings/configure-approval-decision-in-wp.md" class="MCXref xref">在Workfront Proof中設定核准決定選項</a>。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （視條件而定）如果Adobe Workfront管理員或Workfront Proof管理員已新增「原因」區段，請為您的決定選取任何適用的原因。 如需管理員如何設定決策原因的詳細資訊，請參閱  [在Workfront Proof中設定核准決定選項](../../../../workfront-proof/wp-acct-admin/account-settings/configure-approval-decision-in-wp.md)。
1. （選擇性）選取&#x200B;**傳送電子郵件確認函給我**，以接收您決定的電子郵件確認函。
1. 按一下&#x200B;**做出決定**。

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Make a decision when the proof is configured with an approval process</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can make decisions on a proof when it is configured with an approval process (within Workfront) and&nbsp;a user has sent you a document approval request, as described in <a href="../../../../review-and-approve-work/manage-approvals/request-document-approvals.md" class="MCXref xref">Request document approvals</a>.</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#make-a-workfront-approval-decision-in-a-proof" class="MCXref xref">Make a Workfront approval decision in a proof</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#change-your-workfront-approval-decision-in-a-proof" class="MCXref xref">Change your Workfront approval decision in a proof</a> </li>
  -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="make-a-workfront-approval-decision-in-a-proof">Make a Workfront approval decision in a proof</h3>
-->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Open the proof of the document that you want to make a decision on.</p>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">In the proofing viewer, select whether you want to <strong>Approve</strong>, require <strong>Changes</strong>, or <strong>Reject</strong> the approval request.</li>
   -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="change-your-workfront-approval-decision-in-a-proof">Change your Workfront approval decision in a proof</h3>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Open the proof of the document where you want to change your Workfront approval decision.</li>
<li value="2"> <p>At the top-center of the proofing viewer, click the decision you made previously.</p> </li>
<li value="3">In the <strong>Proof decision</strong> box that appears, select whether you want to <strong>Approve</strong>, require <strong>Changes</strong>, or <strong>Reject</strong> the approval request.</li>
</ol>
-->
