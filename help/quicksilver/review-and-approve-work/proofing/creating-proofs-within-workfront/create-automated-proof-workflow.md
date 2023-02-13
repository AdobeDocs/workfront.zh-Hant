---
product-area: documents;setup
navigation-topic: create-proofs-within-workfront
title: 使用自動化工作流程建立進階校樣
description: 如果您的流程複雜，或您定期將內容傳送給相同的人員進行審核，自動化工作流程可讓您更輕鬆地管理審核流程。 校樣會從舞台移至舞台，Adobe Workfront會在每位使用者需要檢閱時通知他們。 如需自動化工作流程的詳細資訊，請參閱自動化工作流程概觀。
author: Courtney
feature: Digital Content and Documents
exl-id: 977fe1bc-458f-4301-8056-dc51c61edb6c
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1856'
ht-degree: 0%

---

# 使用自動化工作流程建立進階校樣

如果您的流程複雜，或您定期將內容傳送給相同的人員進行審核，自動化工作流程可讓您更輕鬆地管理審核流程。 校樣會從舞台移至舞台，Adobe Workfront會在每位使用者需要檢閱時通知他們。 如需自動化工作流程的詳細資訊，請參閱 [自動化工作流程概觀](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

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

## 使用自動化工作流程建立進階校樣

1. 前往您要校樣的專案、任務或問題，然後按一下 **檔案** 標籤。
1. 按一下 **新增** >校樣，上傳內容，然後逐一查看下列章節。

   或

   暫留在現有檔案上，然後按一下 **建立校樣** > **進階校樣** 並逐步完成下列章節。

## 配置校樣階段

1. 在「工作流類型」部分中，選擇 **自動**.
1. （選用）如果您想要使用Workfront管理員建立並與您共用的「自動化工作流程」範本，請按一下 **新增範本**，在出現的方塊中選取範本，然後按一下 **新增範本**.

   >[!NOTE]
   >
   >使用「自動化工作流程」範本時，請考量下列事項：
   >   
   >* 「自動化工作流程」範本的設定決定了您可以對「自動化工作流程」執行哪些校樣。 例如，如果在範本中停用了「新增階段」按鈕，當您使用校樣的「自動化工作流程」設定時，該按鈕將不會顯示。
   * 將人員添加到「自動化工作流」模板中的某個頁面，但同時已作為校樣的審閱者出現時，應用模板會將審閱者從舞台中刪除。 如果您未將另一個審核者添加到舞台，則會出現一條消息提示您添加一個審核者。
   * 您修改「自動化工作流程」範本的能力取決於Workfront管理員所設定的範本設定，如中所述。 如果禁用了修改模板的功能，則只有模板的所有者才能修改它。


1. 設定自動化工作流程的第一階段：

   1. （可選）如果要建立第一個階段的名稱，請按一下 **第1階段**，然後輸入名稱。
   1. 在 **收件者** 節，將審核者添加到舞台。

      >[!NOTE]
      將審核者添加到階段時，請考慮以下事項：
      * 您可以使用電子郵件地址將外部使用者新增至預備。
      * 將使用者新增到舞台後，您可以在校樣上設定該使用者的設定。
      * 您可以直接將使用者拖曳至另一個階段，或將使用者拖曳至 **階段** 圖表。 要選擇多個用戶，請按Shift + Ctrl（在Windows上）或Shift + Command(在Mac上)。
      * 只能將審核者添加到校樣一次，這意味著您不能將同一人添加到校樣的多個階段。
      * 未添加到私人舞台的審閱者無法看到該舞台上在該舞台上所做的校樣或評論。
      * 依預設，將使用者新增至階段會授予使用者從建立校樣開始即可檢視校樣的存取權。\
         您的Workfront管理員可以限制使用者存取校樣，直到工作流程進入新增使用者的階段為止。


   1. 按一下 **舞台設定**.
   1. 按一下 **啟動階段** 選項，指明要如何激活舞台。

      對於第一階段，您只能選取 **論校樣建立**, **在特定日期和時間**，或 **手動**.

   1. （條件性）如果您選取 **在特定日期和時間** 在上一步中，選取要在 **於啟用** 框中。

   1. 使用下面的任何選項進一步配置舞台。

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">設定階段截止期</td>
         <td><p>若要設定階段的截止時間，請按一下 <strong>期限選項</strong> 下拉式清單。 然後，在 <strong>截止時間</strong>，執行下列其中一項操作：</p>
          <ul>
           <li>如果您選擇 <strong>設定特定日期</strong>:選擇所需的截止日期和時間。</li>
           <li>如果您選擇 <strong>從階段激活日期計算</strong>:選擇要添加到階段激活日期的工作天數，以確定截止日期。</li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">鎖台</td>
         <td>指定何時可以鎖定舞台。 </td>
        </tr>
        <tr>
         <td role="rowheader">將主要決策權轉讓至</td>
         <td><p>在舞台上選擇主決策者（僅在向舞台上添加至少一個具有「批准者」或更高「證明」角色的人員後可用）。 如果選擇主決策者，則 <strong>只需一個決定</strong> 選項。</p></td>
        </tr>
        <tr>
         <td role="rowheader">此階段只需要一個決策</td>
         <td>當某個決策者做出決策時，結束整個審查過程。<p>如果您在 <strong>主要決策者</strong>下拉式功能表。</p></td>
        </tr>
        <tr>
         <td role="rowheader">將此階段設為私人</td>
         <td>僅允許以下人員查看此階段中做出的評論和決策：監事、Workfront管理員和Workfront Proof管理員</td>
        </tr>
       </tbody>
      </table>

1. 要添加和配置另一個階段：

   1. 按一下 **新階段**.
   1. （可選）如果要建立第一個階段的名稱，請按一下 **第2階段** (或 **第3階段**, **第4階段**、等)，然後輸入名稱。

   1. 按一下 **啟動階段**，然後選擇一個選項以指定是否自動激活舞台或手動激活舞台。

      除了 **論校樣建立**, **在特定日期和時間**，或 **手動**，您可以選取與前一個步驟中發生的內容相依的選項：

      ![](assets/activate-stage-options-for-stage-2-plus-350x177.png)

   1. 如果您選取了與前一個步驟發生的內容相關的「啟動」階段選項，請使用顯示的選項來配置啟動設定。

      例如，若您選取 **上一階段狀態更改時**，請選取 **上一階段**，然後選取 **狀態已變更為** 框。

1. 視需要重複上一步，以新增更多階段。

   將階段新增至自動化工作流程時，畫面上會顯示圖表，以表示這些階段：

   ![](assets/stages-diagram-350x213.png)

1. 繼續 [配置校樣的電子郵件設定](#configure-email-settings-for-the-proof) 下方。

## 配置校樣的電子郵件設定 {#configure-email-settings-for-the-proof}

1. 在 **電子郵件通知** 區段，選擇是否向您在 [使用自動化工作流程建立進階校樣](#workflow) 本文的前面部分：

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
        </ul><p><strong>注意：</strong> 如果校樣已附加「自動化工作流程」 ，則所有訂閱都會產生確認電子郵件給校樣擁有者，讓他們決定應將人員新增至哪個階段。<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **建立校樣**.

   Workfront會開始產生所選檔案或網站的證明。 視檔案大小和類型而定，檔案上傳的延遲時間可能會有所不同。 請耐心等待，因為較大的檔案需要更長的時間才能產生。 您可以離開頁面，Workfront會繼續產生您的檔案。 檔案上傳大小上限為4GB。

1. 產生校樣後，按一下 **開啟校樣** 啟動校對檢視器。

   ![](assets/open-proof-350x132.png)

   帳戶中未啟用校對功能的使用者，仍可檢視檔案並對校樣發表意見 [.](../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md)
