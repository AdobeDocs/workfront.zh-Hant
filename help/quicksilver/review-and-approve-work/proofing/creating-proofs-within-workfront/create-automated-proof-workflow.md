---
product-area: documents;setup
navigation-topic: create-proofs-within-workfront
title: 使用自動化工作流程建立進階校訂
description: 如果您的程式複雜，或您定期傳送內容給相同的人員審查，自動化工作流程可讓您更輕鬆地管理審查程式。 校訂從一個階段移動到另一個階段，當輪到每個使用者檢閱時，Adobe Workfront會通知他們。 如需自動化工作流程的詳細資訊，請參閱自動化工作流程概觀。
author: Courtney
feature: Digital Content and Documents
exl-id: 977fe1bc-458f-4301-8056-dc51c61edb6c
source-git-commit: 84c5772d130be78d9f9b9aef342c57183d5ec985
workflow-type: tm+mt
source-wordcount: '1831'
ht-degree: 0%

---

# 使用自動化工作流程建立進階校訂

<!-- Audited: 2/2024 -->

如果您的程式複雜，或您定期傳送內容給相同的人員審查，自動化工作流程可讓您更輕鬆地管理審查程式。 校訂從一個階段移動到另一個階段，當輪到每個使用者檢閱時，Adobe Workfront會通知他們。 如需自動化工作流程的詳細資訊，請參閱 [自動化工作流程總覽](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>新增：任何</p><p>目前計畫：Pro或更高版本</p><p>舊版計畫：選取或更高</p> <p>如需有關校訂不同方案的存取許可權的詳細資訊，請參閱 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">存取Workfront中的校訂功能</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>新增：標準</p><p>目前計畫：工作或計畫</p> <p>舊版計畫：任何（您必須為使用者啟用校訂）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">校樣權限設定檔 </td> 
   <td>經理或以上</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯檔案的存取權</p></td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## 使用自動化工作流程建立進階校訂

1. 前往您想要校訂的專案、任務或問題，然後按一下 **檔案** 標籤。
1. 按一下 **新增** >校訂，上傳內容，然後完成以下列出的區段。

   或

   將滑鼠停留在現有檔案上，然後按一下 **建立校訂** > **進階校訂** 並逐步說明下列章節。

## 設定校訂階段

1. 在「工作流程型別」區段中，選擇 **自動化**.
1. （選用）如果您想使用Workfront管理員建立並共用給您的自動工作流程範本，請按一下 **新增範本**，在出現的方塊中選取範本，然後按一下 **新增範本**.

   >[!NOTE]
   >
   >使用自動化工作流程範本時，請考量下列事項：
   >   
   >* 自動化工作流程範本的設定會決定您可以使用自動化工作流程做哪些事來校訂。 例如，如果範本中停用「新增階段」按鈕，當您使用校訂的「自動化工作流程」設定時，將無法看到該按鈕。
   >* 當有人在自動化工作流程範本中新增到頁面，但已經在校樣上作為稽核者出現時，套用範本會從階段中移除稽核者。 如果您未將其他稽核者新增至階段，則會出現一則訊息，提示您新增稽核者。
   >* 您修改自動化工作流程範本的能力取決於Workfront管理員設定的範本設定，如所述。 如果修改範本的功能已停用，則只有範本的擁有者可以修改它。

1. 設定自動化工作流程的第一階段：

   1. （選擇性）如果要建立第一個階段的名稱，請按一下 **階段1**，然後輸入名稱。
   1. 在 **收件者** 部分，新增稽核者至階段。

      >[!NOTE]
      >
      >將稽核者新增至階段時，請考量下列事項：
      >   
      >* 您可以將外部使用者新增至具有電子郵件地址的階段。
      >* 將使用者新增到階段後，您可以在校訂上為該使用者設定設定。
      >* 您可以將使用者直接拖曳到另一個舞台，也可以將使用者拖曳到 **階段** 圖表。 若要選取多個使用者，請按Shift+Ctrl鍵（在Windows上）或Shift+Command鍵(在Mac上)。
      >* 您只能將稽核者新增到校訂一次，這表示您無法將同一個人新增到校訂上的多個階段。
      >* 未新增至私人階段的稽核者在校訂上無法看到該階段，也無法在該階段中做出評論。
      >* 根據預設，將使用者新增到階段會授予該使用者從建立校訂開始檢視校訂的存取權。 在工作流程進入新增使用者的階段之前，您的Workfront管理員可以限制使用者存取校訂。

   1. 按一下 **中繼設定**.
   1. 按一下 **啟用階段** 用來指示您想要舞台啟動方式的選項。

      對於第一個階段，您只能選取 **建立校訂時**， **在特定日期和時間**，或 **手動**.

   1. （視條件而定）如果您已選取 **在特定日期和時間** 在上一個步驟中，選取您要在中啟動階段的日期和時間 **啟用日期** 方塊。

   1. 使用下列任一選項來進一步設定舞台。

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">設定階段期限</td>
         <td><p>若要設定階段的截止日期，請按一下 <strong>截止日期選項</strong> 下拉式清單。 然後，在 <strong>期限</strong>，請執行下列任一項作業：</p>
          <ul>
           <li>如果您選擇 <strong>設定特定日期</strong>：選取您想要的截止日期和時間。</li>
           <li>如果您選擇 <strong>從階段啟用日期計算</strong>：選取要新增至階段啟用日期的工作日數以決定截止日期。</li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">鎖定階段</td>
         <td>指定可以鎖定舞台的時間。 </td>
        </tr>
        <tr>
         <td role="rowheader">將主要決定權轉移至</td>
         <td><p>選取階段上的主要決策者（只有在您將至少一個具有「核准者」或更高證明「 」角色的人新增到階段後，才能使用）。 如果您選取主要決策者， <strong>只需要一個決定</strong> 選項已在此階段停用。</p></td>
        </tr>
        <tr>
         <td role="rowheader">此階段只需要一個決定</td>
         <td>當其中一位決策者做出決定時，結束整個稽核程式。<p>如果您在中指定使用者，則此選項不可用 <strong>主要決策者</strong>下拉式功能表。</p></td>
        </tr>
        <tr>
         <td role="rowheader">將此階段設為私人</td>
         <td>僅允許下列人員檢視在此階段中作出的評論和決定：主管、Workfront管理員和Workfront Proof管理員</td>
        </tr>
       </tbody>
      </table>

1. 若要新增及設定另一個階段：

   1. 按一下 **新階段**.
   1. （選擇性）如果要建立第一個階段的名稱，請按一下 **階段2** (或 **階段3**， **階段4**，依此類推)，然後輸入名稱。

   1. 按一下 **啟用階段**，然後選取選項以指定舞台是自動啟動還是手動啟動。

      除了選項 **建立校訂時**， **在特定日期和時間**，或 **手動**，您可以選取一個選項，該選項取決於前一步驟中發生的情況：

      ![](assets/activate-stage-options-for-stage-2-plus-350x177.png)

   1. 如果您選取的啟動階段選項取決於上一步驟中所發生的情況，請使用顯示的選項來設定啟動設定。

      例如，如果您選取 **當上一個階段狀態變更時**，選取 **上一個階段**，然後在 **狀態已變更為** 方塊。

1. 視需要重複上一步驟以新增更多階段。

   當您新增階段至「自動化工作流程」時，畫面上的圖表會呈現這些階段：

   ![](assets/stages-diagram-350x213.png)

1. 繼續使用 [設定校訂的電子郵件設定](#configure-email-settings-for-the-proof) 底下。

## 設定校訂的電子郵件設定 {#configure-email-settings-for-the-proof}

1. 在 **電子郵件通知** 區段，選取是否傳送電子郵件通知及自訂訊息給您在中選取的使用者 [使用自動化工作流程建立進階校訂](#workflow) 本文前文：

   <table>
      <tbody>
      <tr>
      <td>將此校訂通知收件者</td>
      <td>選取此選項即可傳送電子郵件通知給使用者。 時間 <strong>基本共用</strong> 已選取的 <strong>工作流程</strong> 區段，建立校樣時會傳送電子郵件通知。 時間 <strong>自動化工作流程</strong> 已選取的 <strong>工作流程</strong> 區段，當校樣進入使用者關聯的自動化工作流程階段時，會傳送電子郵件通知。</td>
      </tr>
      <tr>
      <td>新增自訂訊息</td>
      <td>選取此選項以在通知中包含自訂訊息。 您可以指定主旨和訊息內文。 訊息內文可包含RTF格式，例如粗體、專案符號和超連結。</td>
      </tr>
      </tbody>
      </table>


1. 繼續使用 [設定校訂設定](#configure-proof-settings) 底下。

## 設定校訂設定 {#configure-proof-settings}

1. 在 **校訂設定** 部分，選取下列任一選項：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">需要登入 — 校訂只能與其他使用者共用</td> 
      <td>停用此選項（預設）時，具有URL的任何人都能夠檢視校訂。 <br>選取此選項時：
       <ul>
        <li>只有Workfront Proof使用者能檢視校訂。</li>
        <li>使用者無法登入校訂，除非他們已新增到校訂中。</li>
        <li>無法啟用訂閱。</li>
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader">此證明只需一個決定</td> 
      <td>選取此選項時，稽核會在其中一位決策者做出決定後完成。<br>此選項預設為停用。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">需要以電子方式簽署決策</td> 
      <td>使用者必須在就校訂做出決定時指定其使用者名稱和密碼。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">完成所有必要的決定時鎖定校訂</td> 
      <td>啟用此設定時，完成所有決定後才會鎖定校訂狀態。 當最終核准者做出決定時，狀態會自動從已解除鎖定變更為已鎖定。<br>此選項預設為停用。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">下載原始檔案</td> 
      <td>選取此選項時，稽核者可下載從中建立校訂的原始檔案。<br>取消選取此選項時，不再顯示「下載」圖示。<br>此選項預設為啟用。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">透過公開URL或內嵌代碼共用校訂</td> 
      <td>選取此選項時，可透過公用URL或內嵌程式碼共用校訂。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">透過公開URL或內嵌程式碼訂閱校訂</td> 
      <td>選取此選項時，未明確新增到校訂的人員可以訂閱校訂。 訂閱校訂的人員會獲得您在以下設定中定義的角色和電子郵件：
       <ul>
        <li><strong>訂閱者角色：</strong> 為訂閱校訂的所有檢閱者指派的預設校訂角色。</li>
        <li><strong>訂閱者的電子郵件警示設定：</strong> 指派給所有訂閱校訂的稽核者的預設電子郵件警報。</li>
       </ul><p>
        <ul>
         <li><strong>以下專案需要透過電子郵件連結的校訂存取權：</strong> 設定訂閱者是否收到包含校訂連結的電子郵件。 您可以選取 <strong>無電子郵件</strong> （存取校樣不需要電子郵件連結）， <strong>僅校訂通知電子郵件</strong> （訂閱者會透過電子郵件收到校訂連結，無需任何驗證），或 <strong>驗證和校訂通知電子郵件</strong> （訂閱者會透過電子郵件收到校訂連結，必須按一下連結才能存取校訂，此選項的目的是確保人員輸入了他們有權存取的正確電子郵件地址）。</li>
        </ul><p><strong>注意：</strong> 如果校訂已附加自動化工作流程，則所有訂閱都將向校訂所有者產生確認電子郵件，以便他們決定應將人員新增到哪個階段。<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **建立校訂**.

   Workfront開始產生所選檔案或網站的校訂。 根據檔案大小和型別，檔案上傳的延遲時間可能會有所不同。 請耐心等候，因為產生較大的檔案需要更長的時間。 您可以離開頁面，Workfront會繼續產生您的檔案。 檔案上傳大小上限為4GB。

1. 產生校訂後，按一下 **未完成的校訂** 以啟動校訂檢視器。

   ![](assets/open-proof-350x132.png)

   未在其帳戶中啟用校訂的使用者仍可檢視檔案並對校訂進行評論 [.](../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md)
