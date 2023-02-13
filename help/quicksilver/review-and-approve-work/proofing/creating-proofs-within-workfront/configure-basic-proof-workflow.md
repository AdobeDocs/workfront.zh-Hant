---
product-area: documents;setup
navigation-topic: create-proofs-within-workfront
title: 使用基本工作流程建立進階校樣
description: 使用基本的工作流程，您可以讓數位審核者進行校樣，但不會分階段組織。 您新增的所有審核者都可以在建立校樣後立即存取校樣。
author: Courtney
feature: Digital Content and Documents
exl-id: 4f5d0c0e-e070-4f32-89c4-3b511a3b7fdc
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1831'
ht-degree: 1%

---

# 使用基本工作流程建立進階校樣

使用基本的工作流程，您可以讓數位審核者進行校樣，但不會分階段組織。 您新增的所有審核者都可以在建立校樣後立即存取校樣。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>當前計畫：Pro或更高</p> <p>或</p> <p>舊計畫：選擇或更高</p> <p>如需使用不同計畫校對存取權限的詳細資訊，請參閱 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">存取Workfront中的校對功能</a>.</p> </td> 
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
   <td> <p>編輯對文檔的訪問</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、角色或校樣權限設定檔，請聯絡您的Workfront或Workfront Proof管理員。

## 使用基本工作流程建立進階校樣

1. 前往您要校樣的專案、任務或問題，然後按一下 **檔案** 標籤。
1. 按一下 **新增** >校樣，上傳內容，然後逐一查看下列章節。

   或

   暫留在現有檔案上，然後按一下 **建立校樣** > **進階校樣** 並逐步完成下列章節。

## 配置工作流程並添加審核者

1. 在「工作流類型」部分中，選擇 **基本**.
1. 指定您要新增的使用者，然後選擇校樣角色。

   ![](assets/new-proof---roles-350x213.png)

1. 下表列出每個角色及其相關的權限。

   <table border="1" cellspacing="15" cellpadding="1"> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p> </p> </th> 
      <th> <p><strong>檢視校樣</strong> </p> </th> 
      <th> <p><strong>新增行銷</strong> </p> </th> 
      <th> <p><strong>添加註釋</strong> </p> </th> 
      <th> <p><strong>如果沒有回覆，請編輯自己的留言</strong> </p> </th> 
      <th> <p><strong>做出決定</strong> </p> </th> 
      <th> <p><strong>刪除其他人的評論</strong> </p> </th> 
      <th>解決注釋</th> 
      <th>將動作套用至註解</th> 
      <th> <p><strong>編輯校樣</strong> </p> </th> 
      <th>與其他人共用證明</th> 
      <th>建立新版本</th> 
      <th> <p><strong>在「首頁」區域中查看批准請求</strong> </p> </th> 
      <th>新增審核者</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p><strong>唯讀</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> </td> 
      <td>✓</td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td> </td> 
      <td> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>檢閱者</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> </td> 
      <td>✓</td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td> </td> 
      <td> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>核准者</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> </td> 
      <td>✓</td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td> </td> 
      <td> <p>✓</p> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>檢閱者和核准者</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td> </td> 
      <td>✓</td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td> </td> 
      <td> <p>✓</p> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>作者</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p> </p> </td> 
      <td>✓</td> 
      <td>✓</td> 
      <td> <p>✓</p> </td> 
      <td>✓</td> 
      <td>✓</td> 
      <td> </td> 
      <td>✓</td> 
     </tr> 
     <tr> 
      <td> <p><strong>仲裁者</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p><strong>✓</strong> </p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> </td> 
      <td> <p>✓</p> <p> </p> </td> 
      <td>✓</td> 
      <td>✓</td> 
      <td> <p>✓</p> </td> 
      <td>✓</td> 
      <td>✓</td> 
      <td>✓</td> 
      <td>✓</td> 
     </tr> 
    </tbody> 
   </table>

1. 新Workfront計畫的使用者可將作者或版主角色授與系統中的任何使用者。 舊版計畫的使用者可以將作者或版主角色授予系統中具有校樣授權的任何使用者。
1. （可選）如果下拉式功能表仍然開啟，請選取功能表底部的其他可用權限：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">解決注釋並應用操作 </td> 
      <td> <p>可讓Workfront使用者執行下列作業：</p> 
       <ul> 
        <li>在處理後解決評論，如 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/resolve-proof-comments.md" class="MCXref xref">解決校樣注釋</a>.</li> 
        <li>將動作套用至註解，如 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md" class="MCXref xref">對校樣注釋使用動作</a>. </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">透過標籤共用校樣</td> 
      <td> <p>允許審核者將任何Workfront使用者新增至校樣，如 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/tag-users-to-share-proof.md" class="MCXref xref">標籤使用者以共用校樣</a>.</p> <p>備註:  <p>如果這兩個選項不可用（暗顯），則用戶已具有允許解析注釋、將操作應用到注釋以及標籤任何用戶的權限配置檔案。 </p> <p>如果未顯示選項，則您新增的人員不是Workfront授權持有者。</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 對於您已新增至校樣的任何其他使用者，重複步驟1至3。
1. 對於您要共用的每個使用者， **電子郵件警報** 下拉式清單中，選取當使用者對校樣發表意見及做出決策時，此使用者會收到的電子郵件警報類型：

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
      <td>只有當有人明確回覆其留言時，系統才會傳送電子郵件給審閱者（這會排除其對其留言的回覆）。 這表示如果校樣上的某人發表新意見，則不會通知審核者。<p>建議您的用戶端使用此設定，以便他們不會收到關於證明的任何其他意見的通知，而且只會收到對其意見的回覆通知。</p><p>雖然具有此電子郵件警報設定的審核者不會收到其他新留言的通知，但他們仍可在校對檢視器中檢視校樣上的所有留言。</p><p>如需註解的相關資訊，請參閱 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">檢視並回覆校樣留言</a>.</p></td> 
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
      <td>Workfront只會在您自己的活動以外的日子，傳送一封電子郵件，其中列出所有留言、回覆和決策。<p>此警報是您查看專案摘要的好方法，不會在一天中多次更新。</p><p>此摘要的使用案例範例是部門主管，他想要監控專案的整體進度。</p><p>如需詳細資訊，請參閱 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">管理校樣意見和決策的通知</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">無電子郵件</td> 
      <td>Workfront不會傳送任何電子郵件警報。<br>對於只為了參考而新增至校樣，且不需要收到任何變更通知的人，這個用法很有幫助。<p>系統預設值為「每日摘要」（也顯示為「未設定」）。 如果您或您的審核者未進行任何其他更改，則所有校樣都具有此設定。</p></td> 
     </tr> 
    </tbody> 
   </table>

1. 繼續 [配置校樣的電子郵件設定](#configure-email-settings-for-the-proof) 下方。

## 配置校樣的電子郵件設定 {#configure-email-settings-for-the-proof}

1. 在 **電子郵件通知** 區段，選擇是否向您在 [使用基本工作流程建立進階校樣](#workflow) 本文的前面部分：

   <table>
   <tbody>
   <tr>
   <td>將此校樣通知收件者</td>
   <td>選取此選項可傳送電子郵件通知給使用者。 當 <strong>基本共用</strong> 在 <strong>工作流程</strong> 區段，則會在建立校樣時傳送電子郵件通知。 當 <strong>自動化工作流程</strong> 在 <strong>工作流程</strong> 區段中，當校樣進入使用者相關聯的「自動化工作流程」階段時，會傳送電子郵件通知。</td>
   </tr>
   <tr>
   <td>新增自訂訊息</td>
   <td>選取此選項，在通知中加入自訂訊息。 您可以指定主旨和訊息內文。 訊息內文可包含RTF格式，例如粗體、項目符號和超連結。</td>
   </tr>
   </tbody>
   </table>


1. 繼續 [配置校樣設定](#configure-proof-settings) 下方。

## 配置校樣設定 {#configure-proof-settings}

1. 在 **校樣設定** ，請選擇以下任一選項：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">需要登入 — 校樣只能與其他使用者共用</td> 
      <td>當此選項停用（預設）時，任何具有URL的人都能檢視校樣。 <br>選取此選項時：
       <ul>
        <li>只有Workfront校樣使用者能檢視校樣。</li>
        <li>除非使用者已新增至校樣，否則無法登入校樣。</li>
        <li>無法啟用訂閱。</li>
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader">此證明只需要一個決定</td> 
      <td>當選擇此選項時，在某個決策者作出決定後完成審查。<br>預設會停用此選項。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">需要以電子方式簽署決策</td> 
      <td>使用者在決定校樣時，必須指定其使用者名稱和密碼。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">做出所有必要決策時鎖定校樣</td> 
      <td>啟用此設定後，在做出所有決策後，會鎖定校樣狀態。 當最終批准者作出決定時，狀態會自動從解除鎖定變更為鎖定。<br>預設會停用此選項。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">下載原始檔案</td> 
      <td>選取此選項時，審閱者將能夠下載建立校樣的原始檔案。<br>取消選取此選項時，「下載」圖示將不再顯示。<br>預設會啟用此選項。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">透過公用URL或內嵌程式碼共用校樣</td> 
      <td>選取此選項時，可透過公用URL或內嵌程式碼來共用校樣。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">透過公開URL或內嵌程式碼訂閱校樣</td> 
      <td>選取此選項時，尚未明確新增至校樣的人員可訂閱校樣。 訂閱校樣的人員會獲得您在下列設定中定義的角色和電子郵件：
       <ul>
        <li><strong>訂閱者角色：</strong> 分配給訂閱校樣的所有審核者的預設校樣角色。 </li>
        <li><strong>訂閱者的電子郵件警報設定：</strong> 指派給訂閱校樣之所有審核者的預設電子郵件警報。</li>
       </ul><p>
        <ul>
         <li><strong>下列項目需要透過電子郵件連結進行校樣存取：</strong> 設定訂閱者是否收到包含校樣連結的電子郵件。 您可以選取 <strong>無電子郵件</strong> （存取校樣不需要電子郵件連結）, <strong>僅校樣通知電子郵件</strong> （訂閱者會透過電子郵件收到校樣的連結，無需任何驗證），或 <strong>驗證和校樣通知電子郵件</strong> （訂閱者會透過電子郵件收到校樣的連結，且必須按一下連結才能存取校樣，此選項的目的是確保使用者已輸入其有權存取的正確電子郵件地址）。</li>
        </ul><p>注意： 如果校樣已附加「自動化工作流程」 ，則所有訂閱都會產生確認電子郵件給校樣擁有者，讓他們決定應將人員新增至哪個階段。<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **建立校樣**.

   Workfront會開始產生所選檔案或網站的證明。 視檔案大小和類型而定，檔案上傳的延遲時間可能會有所不同。 請耐心等待，因為較大的檔案需要更長的時間才能產生。 您可以離開頁面，Workfront會繼續產生您的檔案。 檔案上傳大小上限為4GB。

1. 產生校樣後，按一下 **開啟校樣** 啟動校對檢視器。

   ![](assets/open-proof-350x132.png)

   帳戶上未啟用校樣的使用者仍可檢視檔案，並對校樣發表意見。