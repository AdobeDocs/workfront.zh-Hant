---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: 在校對檢視器中決定校樣
description: 您可以直接在校樣檢視器中對校樣進行決策。
author: Courtney
feature: Digital Content and Documents
exl-id: cf74ac54-b8c1-4404-b35f-2aa94831ecad
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 3%

---

# 在校對檢視器中決定校樣

您可以直接在校樣檢視器中對校樣進行決策。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>當前計畫：Pro或更高</p> <p>或</p> <p>舊計畫：Select或Premium</p> <p>如需使用不同計畫校對存取權限的詳細資訊，請參閱 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">存取Workfront中的校對功能</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>當前計畫：工作或計畫</p> <p>舊計畫：任何（您必須為使用者啟用校對）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">校訂權限設定檔 </td> 
   <td>管理員或更高</td> 
  </tr> 
  <tr> 
   <td role="rowheader">證明角色</td> 
   <td>核准者、審核者與核准者、作者、協調者</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對文檔的訪問</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、角色或校樣權限設定檔，請聯絡您的Workfront或Workfront Proof管理員。

## 在校對檢視器中決定校樣

1. 轉到包含文檔的項目、任務或問題，然後選擇 **檔案**.
1. 找到您需要的校樣，然後按一下 **開啟校樣**.

1. 按一下 **決策** 在校對檢視器的頂端。

1. 在 **證明決策** 框中，按一下以下任一決策：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">已核准</td> 
      <td>校樣已準備好移至自動化工作流程的下一個階段。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">已核准，但有變更</td> 
      <td>校樣需要一些變更，但您不需要先查看修訂版本，再將其移至自動化工作流程的下一個階段。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">所需變更</td> 
      <td>校樣需要變更，而您必須先查看其他修訂版本，才能移至自動化工作流程的下一個階段。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">不相關</td> 
      <td>證明與您無關，您不需要做出決定。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">自訂決策</td> 
      <td> <p>在Select和Premium計畫上，Workfront管理員或Workfront校樣管理員可以更名、重新排序和隱藏決策。 如需詳細資訊，請參閱 <a href="../../../../workfront-proof/wp-acct-admin/account-settings/configure-approval-decision-in-wp.md" class="MCXref xref">在Workfront Proof中設定核准決策選項</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （條件性）如果Adobe Workfront管理員或Workfront校樣管理員已新增「原因」區段，請選取您決定的任何適用原因。 如需管理員如何設定決策原因的詳細資訊，請參閱  [在Workfront Proof中設定核准決策選項](../../../../workfront-proof/wp-acct-admin/account-settings/configure-approval-decision-in-wp.md).
1. （選用）選取 **發送電子郵件確認** 接收您的決定的電子郵件確認。
1. 按一下 **決策**.

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
