---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: 從校訂檢視器共用校訂
description: 如果校訂擁有者或建立者啟用共用，則您可以從校訂檢視器共用校訂。
author: Courtney
feature: Digital Content and Documents
exl-id: 20bd2d94-1401-4a38-9042-335d0cb32a3d
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1501'
ht-degree: 0%

---

# 從校訂檢視器共用校訂

如果校訂擁有者或建立者啟用共用，則您可以從校訂檢視器共用校訂。

>[!IMPORTANT]
>
>必須啟用「允許透過公開URL或內嵌程式碼共用校訂」設定。

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
   <td> <p>編輯檔案的存取權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、角色或校訂許可權設定檔，請連絡您的Workfront或Workfront Proof管理員。

## 共用URL

如果擁有者已設定要共用的校訂，您可以透過URL共用校訂。 校訂擁有者可隨時更新共用設定。 如需詳細資訊，請參閱[編輯校訂設定](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md)。

1. 如果未顯示左圖示功能表，請按一下校訂檢視器左上角的&#x200B;**功能表**&#x200B;圖示。

   ![](assets/menu-icon-in-proofing-viewer-350x188.png)

1. 在校訂檢視器的左側圖示功能表中，按一下&#x200B;**共用**&#x200B;圖示。

   ![Share_btn_in_viewer.png](assets/share-btn-in-viewer.png)

1. 在出現的&#x200B;**共用校訂**&#x200B;選項中，確定已選取&#x200B;**取得可共用連結**。

1.  執行下列任一項作業：

   * 若要將連結複製到剪貼簿，請按一下[複製連結]。****

     您現在可以透過第三方工具（例如聊天或電子郵件應用程式）發佈連結。

   * 若要直接從Adobe Workfront透過電子郵件傳送連結，請執行下列動作：

      1. 在&#x200B;**或電子郵件連結至**&#x200B;欄位中，開始輸入並選取收件者的名稱。 或指定要與其共用的外部使用者的電子郵件地址。

         >[!NOTE]
         >
         >如果您在共用校訂時看到別名電子郵件，請勿在存在對應的別名電子郵件時輸入原始電子郵件來建立新的訪客使用者。

      1. 從下列選項中選取：

         <table style="table-layout:auto">
          <col>
          <col>
          <tbody>
           <tr>
            <td role="rowheader">傳送公開連結</td>
            <td><p>在電子郵件通知中包含一個按鈕，可將使用者導向到他們使用的校訂檢視器內的校訂並授予檢視存取權。</p><p>如果<strong>透過公開URL或內嵌程式碼訂閱校訂</strong>已針對校訂關閉，使用者可以使用其Workfront登入認證登入，以在校訂中加入註解。 如果已開啟，則提供其電子郵件地址和名稱（不需要密碼）的任何人都可以簽署並在校訂中新增註解。</p></td>
           </tr>
           <tr>
            <td role="rowheader">傳送下載連結</td>
            <td>在電子郵件通知中包含一個按鈕，可將使用者引導至下載頁面，其中提供檔案詳細資訊、檔案名稱和檔案大小，並內嵌顯示檔案。 使用者可以從下載頁面按一下下載連結來下載檔案。</td>
           </tr>
           <tr>
            <td role="rowheader">新增自訂訊息</td>
            <td>可讓您指定電子郵件通知的自訂主旨與內文。</td>
           </tr>
          </tbody>
         </table>

      1. 按一下「**傳送**」。

         收件者會收到電子郵件通知，其中包含有關校樣和您選擇加入之按鈕的資訊。

         ![](assets/proof-share-email-350x87.png)

## 共用內嵌程式碼

如果校訂擁有者已為此設定，您可以透過內嵌程式碼共用校訂。

若要透過內嵌程式碼共用校樣：

1. 在校訂檢視器左側的工具列中，按一下&#x200B;**共用**&#x200B;圖示。

   ![Share_btn_in_viewer__1_.png](assets/share-btn-in-viewer--1-.png)

1. 在出現的&#x200B;**共用校訂**&#x200B;選項中，按一下&#x200B;**取得內嵌程式碼**，然後按一下&#x200B;**複製**。

## 新增使用者以共用校訂

如果您擁有下列任一許可權，您可以在檢閱校訂時將使用者新增到校訂中：

* 監督員或管理員許可權
* 管理員許可權且您是校訂建立者或所有者
* 具有作者或版主校訂角色的管理者許可權

如果校訂有自動化工作流程，您可以將使用者新增到個別階段。 如需詳細資訊，請參閱[自動化工作流程總覽](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md)。

根據預設，您新增到校訂的使用者：

* 接收內含證明連結的電子郵件通知。
* 可以根據[核准工作](../../../../review-and-approve-work/manage-approvals/approving-work.md)中所述，從首頁或我的工作區域對校訂進行核准決定。
* 不需要啟用校訂即可檢閱校訂。

當啟用自動工作流程且您將使用者新增到Workfront中未啟用校訂的校訂時，會在自動工作流程中建立新階段。 您新增的使用者第一次檢視校訂時，會自動新增到此新階段。 如需詳細資訊，請參閱[自動化工作流程總覽](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md)。

若要與個別使用者共用校訂：

1. 在校訂檢視器左側的工具列中，按一下&#x200B;**共用**&#x200B;圖示。

   ![Share_btn_in_viewer__2_.png](assets/share-btn-in-viewer--2-.png)

1. 按一下左側清單中的&#x200B;**新增收件者**。
1. 在&#x200B;**新校訂收件者**&#x200B;下方，開始輸入您要與其共用校訂的使用者名稱，然後在其出現在下拉式清單中時按一下該名稱。
1. （可選）變更人員名稱右邊的任何檢閱者選項：

   * **校訂角色**：如需詳細資訊，請參閱[在Workfront Proof中管理校訂角色](../../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)。

   * **階段**： （只有在校訂具有自動化工作流程時才可用）。 如需詳細資訊，請參閱  [自動化工作流程階段概觀](../../../../review-and-approve-work/proofing/proofing-overview/stages.md)。

   * **電子郵件警示**：選取下列其中一個選項，以指定如何通知人員有關校訂活動的通知。

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">所有活動</td> 
        <td>每次校訂上發生任何活動（例如新評論、回覆或決定）時，Workfront都會傳送電子郵件給檢閱者。 <p>這是管理校訂流程之人員的絕佳選項，因為可讓他們檢視活動發生的情形。 </p><p>使用者不會收到有關其活動的電子郵件警報。</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">回覆我的評論</td> 
        <td>只有當某人明確回覆其評論時（這不包括他們自己的評論），才會傳送電子郵件給稽核者。 這表示如果校訂上的某人發表新評論，則不會通知檢閱者。<p>建議將此設定提供給校訂上的客戶，這樣他們就不會收到校訂上任何其他評論的通知，而只會在回覆他們自己的評論時收到通知。</p><p>雖然具有此電子郵件警報設定的檢閱者不會收到其他新評論的通知，但他們仍可在校訂檢視器中檢視校訂上的所有評論。</p><p>如需有關註解的資訊，請參閱<a href="../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">檢視並回覆校訂註解</a>。</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">決策</td> 
        <td>Workfront只會在有人做出決定時，才會傳送電子郵件給稽核者。<p>這對於管理核准流程的人員（例如專案經理）非常有用，他們需要監視校訂的進度並檢視哪些使用者已做出決定。</p><p>除非您在提交決定時選取電子郵件確認選項，否則不會通知您自己的決定。</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">最終決策</td> 
        <td>當校訂的最後一位核准者做出決定時，Workfront會傳送電子郵件。<p>設計人員經常會使用此警示，他們通常不需要參與實際的稽核討論。 做出最終決定時，設計人員會收到通知，然後可以對任何必要的變更採取行動。</p><p>此警示對於必須在複查程式完成後才收到通知的部門主管來說也很有用。</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">每小時摘要</td> 
        <td>Workfront每小時會傳送電子郵件給稽核者，其中包含該小時發生的所有評論、回覆和決定的摘要。<p>只有當您以外的活動發生在過去一小時內，才會傳送電子郵件。 </p><p>此警報是檢視專案概觀的好地方。</p><p>此摘要的範例使用案例是資深檢閱者，他需要專案的概觀，但不需要立即收到校訂上所有活動的通知。</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">每日摘要</td> 
        <td>Workfront會傳送一封電子郵件，其中包含所有評論、回覆和決定，且僅限於您擁有活動以外的日期。<p>此警報是檢視專案摘要的好方法，而不會在一天中忙於多次更新。</p><p>此摘要的範例使用案例是部門負責人，他想要監控專案的整體進度。</p><p>如需詳細資訊，請參閱<a href="../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">管理校訂評論和決定的通知</a>。</p></td> 
       </tr> 
       <tr data-mc-conditions=""> 
        <td role="rowheader">無電子郵件</td> 
        <td>Workfront不會傳送任何電子郵件警示。<br>這對於僅供參考而新增到校訂中且不需要通知任何變更的人員非常有用。<p>系統預設值為「每日」摘要（亦顯示為「未設定」）。 如果您或您的稽核者未進行任何其他變更，則您的所有校樣都會具有此設定。</p></td> 
       </tr> 
      </tbody> 
     </table>

1. （選用）重複前兩個步驟，將多位使用者新增至校訂中。 
1. （選用）為稽核者設定&#x200B;**期限** （僅在校訂沒有自動化工作流程時可用）。
1. （選擇性）選取&#x200B;**傳送電子郵件通知給新收件者**，讓他們知道您已將其新增至校訂中。
1. 當您完成新增使用者到校訂時，請按一下&#x200B;**完成。**
