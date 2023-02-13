---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: 管理校樣意見和決策的通知
description: 當您處理校樣時，無論您是Adobe Workfront用戶還是外部協作者，都可以指定要接收哪些電子郵件通知，以了解您對校樣所做的評論和決策。 如需詳細資訊，請參閱校樣意見和決策概觀的通知。
author: Courtney
feature: Digital Content and Documents
exl-id: c38e005c-8984-4e99-9527-94a0a6b1071d
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '983'
ht-degree: 0%

---

# 管理校樣意見和決策的通知

當您處理校樣時，無論您是Adobe Workfront用戶還是外部協作者，都可以指定要接收哪些電子郵件通知，以了解您對校樣所做的評論和決策。 如需詳細資訊，請參閱 [校樣意見和決策通知概述](../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md).

>[!NOTE]
>
>這些通知與您收到的審核者校樣流程的電子郵件警報不同。 它們也與您可在Workfront中設定的電子郵件警報設定不同。 

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
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對文檔的訪問</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、角色或校樣權限設定檔，請聯絡您的Workfront或Workfront Proof管理員。

## 管理校樣意見和決策的通知

1. 開啟您要設定接收通知的校樣。
1. 如果左側工具列未顯示，請按一下 **功能表** 表徵圖，位於Web校對查看器的左上角。

   ![Menu_icon_in_Pooking_Viewer.png](assets/menu-icon-in-proofing-viewer-350x228.png)

1. 在左側工具列中，按一下 **設定** 表徵圖。 ![Settings_icon.png](assets/settings-icon.png)

1. 在 **傳送有關**，按一下您要進行校樣的設定。

   您選取的設定僅對已開啟的校樣有效。

   系統預設值為 **每日摘要**. 如果您或您的審核者未進行任何其他更改，則所有校樣都具有此設定。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">所有活動</td> 
      <td>每次校樣上有任何活動（例如新留言、回覆或決定）時，都會傳送電子郵件給審核者。<br><p>對於管理校對程式的人員來說，這是絕佳選項，因為這可讓他們查看活動發生的時間。 使用者不會收到有關其自身活動（例如留言、回覆和所做決策）的電子郵件警報。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">對我評論的答復</td> 
      <td>只有當有人明確回覆其留言時，系統才會傳送電子郵件給審閱者（這會排除其對其留言的回覆）。 這表示如果校樣上的某人發表新意見，則不會通知審核者。<p>建議您的用戶端使用此設定，以便他們不會收到關於證明的任何其他意見的通知，而且只會收到對其意見的回覆通知。</p><p>雖然具有此電子郵件警報設定的審核者不會收到其他新留言的通知，但他們仍可在校對檢視器中檢視校樣上的所有留言。<br></p><p>如需詳細資訊，請參閱 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">檢視並回覆校樣留言</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">決策</td> 
      <td>只有在有人作出決定時，才會傳送電子郵件給審核者。<br><p>此電子郵件警報對於管理核准流程的人員（如項目經理）非常有用，因為它允許管理核准流程的人員監視校樣的進度，並查看哪些用戶做出了決策。<br></p><p>除非您在提交決策時選取電子郵件確認選項，否則系統不會通知您自己的決策。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">最終決定</td> 
      <td>當對校樣做出最終決定時（當校樣的最後核准者做出決定時），就會傳送電子郵件。<br><p>此警報常被設計人員使用，因為設計人員不需要參與實際的審閱討論。 當做出最終決定時，設計人員會收到通知，然後可以對任何必要的變更採取行動。<br></p><p>此警報對於只有在審核流程完成時才需要通知的部門主管也很有用。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">每小時摘要</td> 
      <td>每小時會傳送電子郵件給審核者，其中包含最後一小時內發生的所有留言、回覆和決策的摘要。<br><p>只有在過去一小時內發生您自己以外的活動時，才會傳送電子郵件。 如果沒有其他使用者的活動，則不會傳送任何電子郵件。<br></p><p>此警報是查看專案概覽的好方法。<br></p><p>此摘要的範例使用案例是需要專案概覽但不需要立即收到校樣上所有活動的通知的資深審核者。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">每日摘要</td> 
      <td>（預設設定）:每天都會傳送電子郵件，列出所有意見、回覆和決策。 只有在您自己的活動以外還有活動時，才會傳送電子郵件。<br><p>此警報是您查看專案摘要的好方法，不會在一天中多次更新。<br></p><p>此摘要的使用案例範例是部門主管，他想要監控專案的整體進度。<br></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">無電子郵件</td> 
      <td>不會傳送電子郵件警報。<br><p>此設定適用於只為了參考而新增至校樣，且不需要收到任何變更通知的人。</p><p>備註: <p>此選項只會關閉您可接收有關證明留言和決策的電子郵件警報。 它不會關閉您可接收有關校樣流程的電子郵件警報，例如「新校樣」或「延遲校樣」電子郵件。 如需有關校樣流程的電子郵件警報的詳細資訊，請參閱下列文章： </p>
        <ul>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md" class="MCXref xref">新校樣電子郵件</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-version-email.md" class="MCXref xref">新版本電子郵件</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/late-proof-email.md" class="MCXref xref">延遲校樣電子郵件</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">校樣製作的電子郵件</a></li>
        </ul></p></td> 
     </tr> 
    </tbody> 
   </table>
