---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: 管理校訂評論和決定的通知
description: 當您處理校訂時，無論您是Adobe Workfront使用者或外部共同作業人員，都可指定您想要收到哪些有關校訂上所做評論和決定的電子郵件通知。 如需詳細資訊，請參閱校訂評論和決定總覽的通知。
author: Courtney
feature: Digital Content and Documents
exl-id: c38e005c-8984-4e99-9527-94a0a6b1071d
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '978'
ht-degree: 1%

---

# 管理校訂評論和決定的通知

當您處理校訂時，無論您是Adobe Workfront使用者或外部共同作業人員，都可指定您想要收到哪些有關校訂上所做評論和決定的電子郵件通知。 如需詳細資訊，請參閱[校訂評論和決定總覽通知](../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md)。

>[!NOTE]
>
>這些通知與您可以收到的有關稽核者之間校樣流程的電子郵件警報不同。 它們也不同於您可以在Workfront中設定的電子郵件警報設定。 

## 存取需求

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

## 管理校訂評論和決定的通知

1. 開啟您要設定將接收之通知的校訂。
1. 如果左側工具列未顯示，請按一下位於Web Proofing Viewer左上角的&#x200B;**功能表**&#x200B;圖示。

   ![Menu_icon_in_Proofing_Viewer.png](assets/menu-icon-in-proofing-viewer-350x228.png)

1. 在左側工具列中按一下&#x200B;**設定**&#x200B;圖示。 ![Settings_icon.png](assets/settings-icon.png)

1. 在「**傳送關於**&#x200B;的電子郵件通知給我」下，按一下您要校訂的設定。

   您選取的設定僅對您已開啟的校樣有效。

   系統預設值為&#x200B;**每日摘要**。 如果您或您的稽核者未進行任何其他變更，則您的所有校樣都會具有此設定。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">所有活動</td> 
      <td>每次校訂上有任何活動（例如新評論、回覆或決定）時，都會傳送電子郵件給檢閱者。<br><p>這是管理校訂流程之人員的絕佳選項，因為可讓他們檢視活動發生的情形。 使用者不會收到有關其活動的電子郵件警報（例如，評論、回覆和作出的決定）。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">回覆我的評論</td> 
      <td>只有當某人明確回覆其評論時（這不包括他們自己的評論），才會傳送電子郵件給稽核者。 這表示如果校訂上的某人發表新評論，則不會通知檢閱者。<p>建議將此設定提供給校訂上的客戶，這樣他們就不會收到校訂上任何其他評論的通知，而只會在回覆他們自己的評論時收到通知。</p><p>雖然具有此電子郵件警報設定的檢閱者不會收到其他新評論的通知，但他們仍可在校訂檢視器中檢視校訂上的所有評論。<br></p><p>如需詳細資訊，請參閱<a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">檢視並回覆校訂評論</a>。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">決策</td> 
      <td>只有在有人做出決定時，才會向檢閱者傳送電子郵件。<br><p>此電子郵件警示對於管理核准流程的人員（例如專案經理）非常有用，因為它允許管理核准流程的人員監視校訂的進度，並檢視哪些使用者已做出決定。<br></p><p>除非您在提交決定時選取電子郵件確認選項，否則不會通知您自己的決定。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">最終決策</td> 
      <td>校訂做出最終決定時會傳送電子郵件（校訂的最後一位核准者做出決定時）。<br><p>設計人員經常會使用此警示，因為設計人員不需要參與實際的稽核討論。 做出最終決定時，設計人員會收到通知，然後可以對任何必要的變更採取行動。<br></p><p>此警示對於必須在複查程式完成後才收到通知的部門主管來說也很有用。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">每小時摘要</td> 
      <td>每小時會傳送電子郵件給稽核者，其中包含過去一小時內發生的所有評論、回覆和決定的摘要。<br><p>只有當您以外的活動發生在過去一小時內，才會傳送電子郵件。 如果沒有其他使用者的活動，則不會傳送電子郵件。<br></p><p>此警報是檢視專案概觀的好地方。<br></p><p>此摘要的範例使用案例是資深檢閱者，他需要專案的概觀，但不需要立即收到校訂上所有活動的通知。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">每日摘要</td> 
      <td>（預設設定）：每天都會傳送電子郵件，其中包含列出的所有評論、回覆和決定。 只有當您有其他活動時，才會傳送電子郵件。<br><p>此警報是檢視專案摘要的好方法，而不會在一天中忙於多次更新。<br></p><p>此摘要的範例使用案例是部門負責人，他想要監控專案的整體進度。<br></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">無電子郵件</td> 
      <td>不會傳送電子郵件警示。<br><p>此設定對於僅供參考而新增至校樣且不需要通知任何變更的人員非常有用。</p><p>注意： <p>此選項僅關閉您可收到的有關校訂評論和決定的電子郵件警報。 它不會關閉您可以收到的有關校訂流程的電子郵件提醒，例如新校訂或延遲校訂電子郵件。 如需有關校樣流程的電子郵件警報的詳細資訊，請參閱以下文章： </p>
        <ul>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md" class="MCXref xref">新校訂電子郵件</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-version-email.md" class="MCXref xref">新版本的電子郵件</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/late-proof-email.md" class="MCXref xref">延遲校訂電子郵件</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">校樣已製作電子郵件</a></li>
        </ul></p></td> 
     </tr> 
    </tbody> 
   </table>
