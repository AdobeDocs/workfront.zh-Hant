---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: 從校對檢視器共用校樣
description: 如果校樣擁有者或建立者已啟用共用，您可以從校樣檢視器共用校樣。
author: Courtney
feature: Digital Content and Documents
exl-id: 20bd2d94-1401-4a38-9042-335d0cb32a3d
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1512'
ht-degree: 0%

---

# 從校對檢視器共用校樣

如果校樣擁有者或建立者已啟用共用，您可以從校樣檢視器共用校樣。

>[!IMPORTANT]
>
>必須啟用「允許透過公用URL或內嵌程式碼共用校樣」設定。

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
   <td> <p>編輯對文檔的訪問</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、角色或校樣權限設定檔，請聯絡您的Workfront或Workfront Proof管理員。

## 共用URL

如果擁有者已設定要共用的校樣，您可以透過URL來共用校樣。 校樣擁有者可隨時更新共用設定。 如需詳細資訊，請參閱 [編輯校樣設定](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md).

1. 如果未顯示左圖示功能表，請按一下 **功能表** 表徵圖。

   ![](assets/menu-icon-in-proofing-viewer-350x188.png)

1. 在校對檢視器的左側圖示功能表中，按一下 **共用** 表徵圖。

   ![Share_btn_in_viewer.png](assets/share-btn-in-viewer.png)

1. 在 **共用校樣** 顯示的選項，請確保 **取得分享連結** 中所有規則的URL。

1.  執行下列任一操作：

   * 若要將連結複製到剪貼簿，請按一下 **複製連結**.

      您現在可以透過協力廠商工具（例如聊天或電子郵件應用程式）來分發連結。

   * 若要直接從Adobe Workfront以電子郵件傳送連結，請執行下列動作：

      1. 在 **或以電子郵件連結至** 欄位，開始輸入並選取收件者的名稱。 或指定您要共用之外部使用者的電子郵件地址。

         >[!NOTE]
         >
         >如果您在共用校樣時看到別名電子郵件，如果相應的別名電子郵件存在，則不要輸入原始電子郵件來建立新的來賓用戶。

      1. 從下列選項中選取：

         <table style="table-layout:auto">
          <col>
          <col>
          <tbody>
           <tr>
            <td role="rowheader">傳送公開連結</td>
            <td><p>在電子郵件通知中包含一個按鈕，可將使用者引導至其使用的校對檢視器內的校樣，並授予檢視存取權。</p><p>若 <strong>透過公開URL或內嵌程式碼訂閱校樣</strong> 為了校樣而關閉，使用者可以使用其Workfront登入憑證登入，以為校樣新增註解。 如果開啟，則提供其電子郵件地址和名稱（無需密碼）的任何人都可以簽名，並在校樣中添加註釋。</p></td>
           </tr>
           <tr>
            <td role="rowheader">傳送下載連結</td>
            <td>在電子郵件通知中包含一個按鈕，可將使用者引導至下載頁面，該頁面提供檔案詳細資訊、檔案名稱和檔案大小，並內嵌顯示檔案。 使用者可以按一下下載頁面中的下載連結來下載檔案。</td>
           </tr>
           <tr>
            <td role="rowheader">新增自訂訊息</td>
            <td>可讓您指定電子郵件通知的自訂主旨和內文。</td>
           </tr>
          </tbody>
         </table>

      1. 按一下 **傳送**.

         您的收件者會收到電子郵件通知，其中包含您選擇加入的校樣和按鈕的相關資訊。

         ![](assets/proof-share-email-350x87.png)

## 共用內嵌程式碼

如果校樣擁有者已為此設定校樣，您可以透過內嵌程式碼來共用校樣。

若要透過內嵌程式碼共用校樣：

1. 在校對檢視器左側的工具列中，按一下 **共用** 表徵圖。

   ![Share_btn_in_viewer__1_.png](assets/share-btn-in-viewer--1-.png)

1. 在 **共用校樣** 顯示的選項，按一下 **取得內嵌程式碼**，然後按一下 **複製**.

## 新增使用者以共用校樣

如果您有下列任一權限，可在檢閱校樣時將使用者新增至校樣：

* 主管或管理員權限
* 管理員權限，您是校樣建立者或擁有者
* 具有作者或協調者校樣角色的管理員權限

如果校樣具有「自動化工作流程」，您可以將使用者新增至個別階段。 如需詳細資訊，請參閱 [自動化工作流程概觀](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

依預設，您會新增至校樣的使用者：

* 接收包含校樣連結的電子郵件通知。
* 可以從「首頁」或「我的工作」區域對校樣進行批准決策，如 [核准工作](../../../../review-and-approve-work/manage-approvals/approving-work.md).
* 不需要啟用校樣即可檢閱校樣。

啟用「自動化工作流程」且您新增使用者至未在Workfront中啟用校樣的校樣時，「自動化工作流程」中會建立新階段。 當您新增的使用者第一次檢視校樣時，就會自動新增至此新階段。 如需詳細資訊，請參閱 [自動化工作流程概觀](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

若要與個別使用者共用校樣：

1. 在校對檢視器左側的工具列中，按一下 **共用** 表徵圖。

   ![Share_btn_in_viewer__2_.png](assets/share-btn-in-viewer--2-.png)

1. 按一下 **新增收件者** 在左邊的清單里。
1. 在 **新校樣收件者**，開始輸入您要共用校樣的使用者名稱，然後在下拉式清單中出現時按一下名稱。
1. （可選）將任何審核者選項更改為人員名稱右側：

   * **證明角色**:如需詳細資訊，請參閱 [在Workfront校樣中管理校樣角色](../../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

   * **階段**:（只有校樣具有自動化工作流程時才可用）。 如需詳細資訊，請參閱  [自動化工作流階段概觀](../../../../review-and-approve-work/proofing/proofing-overview/stages.md).

   * **電子郵件警報**：選取下列其中一個選項，以指定將如何通知人員校樣上的活動。

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">所有活動</td> 
        <td>Workfront會在每次校樣有任何活動（例如新留言、回覆或決定）時，傳送電子郵件給審核者。 <p>對於管理校對程式的人員來說，這是絕佳選項，因為這可讓他們查看活動發生的時間。 </p><p>使用者不會收到有關其自身活動的電子郵件警報。</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">對我評論的答復</td> 
        <td>只有當有人明確回覆其留言時，系統才會傳送電子郵件給審閱者（這會排除其對其留言的回覆）。 這表示如果校樣上的某人發表新意見，則不會通知審核者。<p>建議您的用戶端使用此設定，以便他們不會收到關於證明的任何其他意見的通知，而且只會收到對其意見的回覆通知。</p><p>雖然具有此電子郵件警報設定的審核者不會收到其他新留言的通知，但他們仍可在校對檢視器中檢視校樣上的所有留言。</p><p>如需註解的相關資訊，請參閱 <a href="../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">檢視並回覆校樣留言</a>.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">決策</td> 
        <td>Workfront僅在有人作出決定時，才會傳送電子郵件給審核者。<p>這對於管理審批流程的人員（如項目經理）來說非常有用，他們需要監控校樣的進度，並查看哪些用戶已做出決策。</p><p>除非您在提交決策時選取電子郵件確認選項，否則系統不會通知您自己的決策。</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">最終決定</td> 
        <td>Workfront會在校樣的最後核准者做出決定時傳送電子郵件。<p>此警報常由設計人員使用，他們通常不需要參與實際的審閱討論。 當做出最終決定時，設計人員會收到通知，然後可以對任何必要的變更採取行動。</p><p>此警報對於只有在審核流程完成時才需要通知的部門主管也很有用。</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">每小時摘要</td> 
        <td>Workfront每小時會傳送電子郵件給審核者，內含該小時內發生的所有留言、回覆和決定的摘要。<p>只有在過去一小時內發生您自己以外的活動時，才會傳送電子郵件。 </p><p>此警報是查看專案概覽的好方法。</p><p>此摘要的範例使用案例是需要專案概覽但不需要立即收到校樣上所有活動的通知的資深審核者。</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">每日摘要</td> 
        <td>Workfront只會在您自己的活動以外的日子，傳送一封電子郵件，其中列出所有留言、回覆和決策。<p>此警報是您查看專案摘要的好方法，不會在一天中多次更新。</p><p>此摘要的使用案例範例是部門主管，他想要監控專案的整體進度。</p><p>如需詳細資訊，請參閱 <a href="../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">管理校樣意見和決策的通知</a>.</p></td> 
       </tr> 
       <tr data-mc-conditions=""> 
        <td role="rowheader">無電子郵件</td> 
        <td>Workfront不會傳送任何電子郵件警報。<br>對於只為了參考而新增至校樣，且不需要收到任何變更通知的人，這個用法很有幫助。<p>系統預設值為「每日摘要」（也顯示為「未設定」）。 如果您或您的審核者未進行任何其他更改，則所有校樣都具有此設定。</p></td> 
       </tr> 
      </tbody> 
     </table>

1. （選用）重複前述兩個步驟，將多個使用者新增至校樣。 
1. （選用）設定 **截止時間** 供審核者使用（只有校樣沒有自動化工作流程時才可用）。
1. （選用）選取 **傳送電子郵件通知給新收件者** 讓他們知道您已將他們加入證明。
1. 將使用者新增到校樣後，按一下 **完成。**
