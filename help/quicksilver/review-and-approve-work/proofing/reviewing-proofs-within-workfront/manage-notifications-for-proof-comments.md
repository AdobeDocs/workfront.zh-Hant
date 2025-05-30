---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: 管理校訂評論和決定的通知
description: 當您處理校訂時，無論您是Adobe Workfront使用者或外部共同作業人員，都可指定您想要收到哪些有關校訂上所做評論和決定的電子郵件通知。 如需詳細資訊，請參閱校訂評論和決定總覽的通知。
author: Courtney
feature: Digital Content and Documents
exl-id: c38e005c-8984-4e99-9527-94a0a6b1071d
source-git-commit: c79d030ff2d05487e5f7e3457bf98df591822a80
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 2%

---

# 管理校訂評論和決定的通知

<!-- Audited: 4/2025 -->

當您處理校訂時，無論您是Adobe Workfront使用者或外部共同作業人員，都可指定您想要收到哪些有關校訂上所做評論和決定的電子郵件通知。 如需詳細資訊，請參閱[校訂評論和決定總覽通知](../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md)。

>[!NOTE]
>
>這些通知不同於您可收到的有關稽核者之間校樣流程的電子郵件警報，以及可在Workfront中設定的電子郵件警報設定。

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
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯檔案的存取權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、角色或校訂許可權設定檔，請連絡您的Workfront或Workfront Proof管理員。

+++

## 管理校訂評論和決定的通知

1. 開啟您要設定通知的校訂。
1. 如果左側工具列未顯示，請按一下Web Proofing Viewer左上角的&#x200B;**功能表**&#x200B;圖示。

   ![Menu_icon_in_Proofing_Viewer.png](assets/menu-icon-in-proofing-viewer-350x228.png)

1. 在左側工具列中按一下&#x200B;**設定**&#x200B;圖示![設定_圖示.png](assets/settings-icon.png) 。

1. 在&#x200B;**傳送關於**&#x200B;的電子郵件通知給我，選取此校訂的通知設定。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">所有活動</td> 
      <td>每次校訂上有任何活動（例如新評論、回覆或決定）時，都會傳送電子郵件給檢閱者。<br><p>建議將此設定提供給管理校訂流程的人員，因為其可讓他們檢視活動發生的情形。 使用者不會收到有關其活動的電子郵件警報（例如評論、回覆或決策）。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">回覆我的評論</td> 
      <td>只有當某人直接回覆其評論（排除其回覆自己的評論）時，才會傳送電子郵件給稽核者。<p>建議您的使用者端使用此設定，如此一來，雖然他們仍可在校訂檢視器中檢視所有評論，但系統僅會通知他們已回覆自己的評論，而不會通知他們對校訂所做的任何其他評論。</p>
      <p>如需詳細資訊，請參閱<a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">檢視並回覆校訂評論</a>。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">決策</td> 
      <td>只有在有人做出決定時，才會向檢閱者傳送電子郵件。<br><p>此電子郵件警報對管理核准流程的人十分實用，因為它可讓管理核准流程的人監控校訂進度並檢視哪些使用者已做出決定。<br></p><p>除非您在提交決定時選取電子郵件確認選項，否則不會通知您自己的決定。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">最終決策</td> 
      <td>當對校訂做出最終決定時會傳送電子郵件。<br><p>設計人員經常會使用此警示，因為設計人員不需要參與實際的稽核討論。 做出最終決定時，設計人員會收到通知，然後可以對任何必要的變更採取行動。<br></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">每小時摘要</td> 
      <td>每小時會傳送電子郵件給稽核者，其中包含過去一小時內發生的所有評論、回覆和決定的摘要。<br><p>只有當您以外的活動發生在過去一小時內，才會傳送電子郵件。 如果沒有其他使用者的活動，則不會傳送電子郵件。<br></p><p>此警報有助於您在專案進行時檢視專案概述。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">每日摘要</td> 
      <td>（預設設定）：每天都會傳送電子郵件，其中包含列出的所有評論、回覆和決定。 這只有在您有活動以外的活動時才會傳送。<br><p>此警報是檢視專案摘要的好方法，而不會在一天中忙於多次更新。<br></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">無電子郵件</td> 
      <td>不會傳送電子郵件警示。<br><p>此設定對於僅供參考而新增至校樣且不需要通知任何變更的人員非常有用。</p><p>注意： <p>此選項只會關閉有關校訂評論和決定的電子郵件警示；它不會關閉您收到的有關校訂流程的電子郵件警示，例如新校訂或延遲校訂電子郵件。 如需詳細資訊，請參閱下列文章： </p>
        <ul>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md" class="MCXref xref">新校訂電子郵件</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-version-email.md" class="MCXref xref">新版本的電子郵件</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/late-proof-email.md" class="MCXref xref">延遲校訂電子郵件</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">校樣已製作電子郵件</a></li>
        </ul></p></td> 
     </tr> 
    </tbody> 
   </table>
