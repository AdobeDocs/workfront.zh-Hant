---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: 設定 [!DNL Adobe Workfront for Jira]
description: 您可以使用 [!DNL Adobe Workfront for Jira] 若要整合您的 [!DNL Jira] 和 [!DNL Workfront] 系統。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 959adc88-5201-4945-96c4-ea890f0bd371
source-git-commit: 9ff647ba4eca31e6d2d06a8c9b787badaf965477
workflow-type: tm+mt
source-wordcount: '2427'
ht-degree: 0%

---

# 設定 [!DNL Adobe Workfront for Jira]

您可以使用 [!DNL Adobe Workfront for Jira] 若要整合您的 [!DNL Jira] 和 [!DNL Workfront] 系統。

安裝附加元件後，您可以定義要建立的工作流程 [!DNL Jira] 發生以下情況時自動問題： [!DNL Workfront] 工作專案已建立。 兩個應用程式中的專案會變成連結，而且其部分資訊會在兩個系統中自動更新。

中的所有使用者 [!DNL Workfront] 和 [!DNL Jira] 可受惠於這項整合。 他們只需要最常使用的系統授權，而不需要兩個系統的授權。

此附加元件同時適用於 [!UICONTROL 伺服器] 和 [!UICONTROL 隨選] (或 [!UICONTROL 雲端])個版本的 [!DNL Jira] 軟體。

針對清單 [!DNL Jira] 版本為 [!DNL Workfront for Jira] 目前支援，請參閱 [[!DNL Workfront for Jira]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview) 在 [!DNL Atlassian Marketplace].

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL [!DNL Adobe Workfront] 計畫]*</td> 
   <td><p>新計畫： [！UICONTROL Prime]或更高版本</p>
       <p>或</p>
       <p>目前計畫： [！UICONTROL Pro]或更高版本</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td><p>新計畫： [！UICONTROL Standard] </p>
       <p>或</p> 
       <p>目前計畫： [！UICONTROL計畫] </p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] 存取</td> 
   <td> <p>系統管理員存取權</p> <p>重要：建議您在中建立個別的系統管理員帳戶 [!DNL Jira] 和 [!DNL Workfront] 以專門用於此整合，而不使用可能附加至使用者的現有整合。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>您必須是 [!DNL Workfront] 管理員。 有關的資訊 [!DNL Workfront] 管理員，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整管理存取權</a>.</p> <p>注意：如果您還是沒有存取權，請詢問您的 [!DNL Workfront] 管理員是否對您的存取層級設定其他限制。 如需瞭解如何 [!DNL Workfront] 管理員可以修改您的存取層級，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 必要條件

設定之前 [!DNL Workfront for Jira]，您必須：

* 安裝 [!DNL Workfront for Jira].
有關安裝的指示 [!DNL Workfront for Jira]，請參閱 [安裝 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## 設定 [!DNL Workfront for Jira]

透過設定 [!DNL Workfront for Jira]，您可以：

* 定義將建立的觸發器 [!DNL Jira] 專案時間 [!DNL Workfront] 專案隨即建立。
* 指定哪些欄位應在連結於其間的專案之間同步 [!DNL Jira] 和 [!DNL Workfront].

>[!NOTE]
>
>* 在您設定之後 [!DNL Workfront for Jira] 在您的 [!DNL Jira] 環境，全部 [!DNL Jira] 使用者看到 [!DNL Workfront] 全部的右側面板 [!DNL Jira] 個專案。 面板包含可能連結之專案的相關資訊 [!DNL Workfront] 或指定否 [!DNL Workfront] 專案已連結至 [!DNL Jira] 個專案。
>* 使用時 [!DNL Jira Server] 安裝時，只有與識別為Workfront整合觸發程式的專案相關的問題，才會顯示Workfront面板。 如需關於設定觸發器的詳細資訊， [!DNL Workfront to Jira] 工作流程，請參閱 [設定觸發程式以自動連結以下專案之間的專案： [!DNL Jira] 和 [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).
>

進行設定 [!DNL Workfront for Jira]：

1. 登入 [!DNL Jira] as a [!DNL Jira] 管理員。
1. 按一下 **[!UICONTROL 設定]** 在主要 [!DNL Jira] 功能表。
1. 按一下 **[!UICONTROL 附加元件]**，然後按一下 **[!UICONTROL 管理附加元件]**.

1. 展開 **[!DNL Workfront]** 附加元件。
1. 按一下 **[!UICONTROL 設定]**.
1. 依照提示登入 [!DNL Workfront].

   >[!NOTE]
   >
   >使用者必須具備有效的 `apiKey` 在 [!UICONTROL Workfront] 以建立成功的連線。

   您必須登入 [!DNL Workfront] as a [!DNL Workfront] 管理員以繼續設定。

   >[!NOTE]
   >
   >* [!UICONTROL Workfront] 連線到 [!DNL Jira] 使用OAuth 2.0，大部分網頁型整合所使用的標準，來驗證及授權使用者。
   >* 當提示您輸入您的網域時 [!DNL Workfront] 帳戶，請以此格式輸入： *yourCompany&#39;sDomain.my.workfront.com*. 您公司的網域通常是您公司的名稱。
   >* 增強式驗證必須等到 [!DNL Workfront] 管理員會為此整合啟用它。

1. 在Jira中，選取 **[!UICONTROL 觸發器]** 標籤以設定自動建立 [!DNL Jira] 個專案為新專案 [!DNL Workfront] 專案隨即建立。

   如需為Workfront設定觸發器的詳細資訊，請參閱 [!DNL Jira] 工作流程，請參閱 [設定觸發程式以自動連結以下專案之間的專案： [!DNL Jira] 和 [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).

1. 選取 **[!UICONTROL 設定]** 索引標籤以設定連結欄位之間的同步化 [!DNL Jira] 和 [!DNL Workfront] 個專案。

   如需關於設定兩者之間的欄位同步化的詳細資訊， [!DNL Jira] 和 [!DNL Workfront]，請參閱 [設定欄位同步處理介於 [!DNL Jira] 和 [!DNL Workfront] 專案](#configure-field-synchronization-between-jira-and-workfront-items).

   >[!NOTE]
   >
   >定義觸發程式以及兩個應用程式之間的欄位同步後， [!DNL Workfront] 可以建立任務或問題的使用者可能會觸發在中建立專案 [!DNL Jira]. 如果使用者建立的專案條件符合中的觸發條件，則使用者可以建立專案 [!DNL Jira]，即使使用者沒有 [!DNL Jira] 授權。 此外，任何 [!DNL Jira] 使用者可以立即開始使用 [!DNL Jira] 專案，及其更新可見於 [!DNL Workfront]，但沒有設定索引標籤。 [!DNL Workfront] 授權。 中的任何更新 [!DNL Workfront] 也會顯示在 [!DNL Jira] 個專案。

1. （可選）選取 **[!UICONTROL 活動記錄]** 標籤來檢閱整合期間可能發生的任何錯誤。

   如需關於的詳細資訊 [!UICONTROL 活動記錄]，請參閱 [檢視 [!DNL Jira] [!UICONTROL 活動記錄]](../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md).

## 設定觸發程式以自動連結以下專案之間的專案： [!DNL Jira] 和 [!DNL Workfront]

作為 [!DNL Jira] 系統管理員，您可以定義會在以下位置自動建立問題的觸發器： [!DNL Jira] 當專案位於 [!DNL Workfront] 符合特定准則。

>[!NOTE]
>
>整合最多可能需要10分鐘，才能在中建立新問題 [!DNL Jira].

設定觸發建立時，請考慮下列事項 [!DNL Jira] 專案為 [!DNL Workfront] 已建立專案：

* 整合是單向的：您只能觸發您在中建立的專案 [!DNL Workfront] 自動建立於 [!DNL Jira]. 您無法觸發在中建立的專案 [!DNL Jira] 自動建立於 [!DNL Workfront].
* 您可以使用的觸發器數量沒有限制。
* 如果您在中建立的專案 [!DNL Workfront] 符合多個觸發程式，在中只建立一個專案 [!DNL Jira]. 專案建立於 [!DNL Jira] 根據第一個觸發器（依照下列定義它們的順序）： [!DNL Jira])。 忽略所有其他觸發程式。
* 中只有一個專案 [!DNL Workfront] 可連結至Jira中的一個專案。 您永遠無法連結一個 [!DNL Workfront] 專案至多個 [!DNL Jira] 問題或一個 [!DNL Jira] 問題轉換為多個 [!DNL Workfront] 個專案。

若要設定自動建立專案的觸發程式，請執行下列步驟： [!DNL Jira]：

1. 登入 [!DNL Jira] 作為系統管理員。
1. 按一下 **[!UICONTROL 設定]** 在主要 [!DNL Jira] 功能表。
1. 按一下 **[!UICONTROL 附加元件]**，然後 **[!UICONTROL 管理附加元件]**.
1. 展開 **[!DNL Workfront]** 附加元件。
1. 按一下 **[!UICONTROL 設定]**.
1. 登入 [!DNL Workfront] 作為系統管理員。

   此 **[!UICONTROL 觸發器]** Jira中預設會選取索引標籤。

1. 按一下 **[!UICONTROL 新增觸發器]** 以新增觸發器。
1. 在 **[!UICONTROL Workfront團隊/使用者/角色]** 欄位，指定 [!DNL Workfront] 團隊、使用者或工作角色，然後按一下以在清單中顯示時選取它。

   >[!NOTE]
   >
   >同一個團隊、使用者或角色不能有多個觸發程式。

   當有人建立任務或問題並將其指派給其中一個實體時，問題會自動在[！DNL]中建立 [!DNL Jira]]。

1. 在 **[!UICONTROL [!DNL Jira]專案]** 欄位，開始輸入 [!DNL Jira] 專案，然後按一下以在清單中顯示時選取專案。

   當 [!DNL Jira] 問題建立後，會放置在您在此處選擇的專案上。

1. 選取 **I[!UICONTROL 問題型別]** （從下拉式功能表）。

   這表示在中建立的問題型別 [!DNL Jira] 當滿足此觸發器的條件時，根據您對中的特定專案的設定 [!DNL Jira].

1. 按一下&#x200B;**[!UICONTROL 儲存]**。

   透過此設定，每次 [!DNL Workfront] 使用者建立符合指定觸發器的專案，新問題建立於 [!DNL Jira].

## 設定欄位同步處理介於 [!DNL Jira] 和 [!DNL Workfront] 專案

作為 [!DNL Jira] 管理員，您可以定義哪些欄位應該自動同步處理連結在之間的專案 [!DNL Workfront] 和Jira。 某些欄位可從 [!DNL Workfront] 至 [!DNL Jira] 專案和其他專案會從Jira同步至Workfront。

若要定義應在兩個應用程式之間連結的專案上自動同步化的欄位：

1. 登入 [!DNL Jira] 身為Jira管理員。
1. 按一下 **[!UICONTROL 設定]** 在主要 [!DNL Jira] 功能表。
1. 按一下 **[!UICONTROL 附加元件]**，然後 **[!UICONTROL 管理附加元件]**.
1. 展開 **[!DNL Workfront]** 附加元件。
1. 按一下 **[!UICONTROL 設定]**.
1. 登入 [!DNL Workfront] Workfront管理員。
1. 在Jira中，按一下 **[!UICONTROL 設定]** 標籤。
1. 在 **[!UICONTROL 從Workfront同步至Jira]** 區段，選取您要更新的欄位 [!DNL Jira] 在Workfront中更新時。

   1. 選取下列任何與欄位同步化的頻率：

      <table style="table-layout:auto">
         <tr>
              <td>[！UICONTROL建立時]</td>
              <td>您指定的欄位會在連結的Workfront與之間同步 [!DNL Jira] 在Workfront中建立專案時顯示的專案。</td>
          </tr>
          <tr>
              <td>[！UICONTROL Always]</td>
              <td>您指定的欄位會在連結的Workfront與之間同步 [!DNL Jira] 在Workfront中更新欄位時的專案。 </td>
          </tr>
          <tr>
              <td>[！UICONTROL從不]</td>
              <td>您指定的欄位不會在連結的欄位之間同步 [!DNL Workfront] 和 [!DNL Jira] 個專案。 沒有任何指示 [!DNL Jira] 欄位已更新的位置 [!DNL Workfront]. </td>
          </tr>
      </table>

   1. 選取下列任一項以同步化欄位 [!DNL Workfront] 至 [!DNL Jira]：

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[！UICONTROL名稱]</td>
         <td><p>中任務或問題的名稱 [!DNL Workfront] 會成為與其連結之問題的名稱 [!DNL Jira].</p><p>附註：在中建立新專案時 [!DNL Jira] 自動 [!DNL Workfront] 名稱一律會更新於 [!DNL Jira] 專案，無論此處是否啟用此欄位。 當 [!DNL Jira] 專案已手動連結至 [!DNL Workfront] 專案，此專案的名稱： [!DNL Workfront] 專案僅更新 [!DNL Jira] 當您選取 <strong>一直</strong> 同步此欄位。 如需手動或自動連結專案的詳細資訊，請參閱 <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md" class="MCXref xref">連結專案介於 [!DNL Adobe Workfront] 和 [!DNL Jira]</a>.</p></td>
        </tr>
        <tr>
         <td role="rowheader">[！UICONTROL說明]</td>
         <td>中任務或問題的說明 [!DNL Workfront] 會成為其所連結問題的說明 [!DNL Jira].</td>
        </tr>
        <tr>
         <td role="rowheader">文件</td>
         <td><p>附加到中任務或問題的檔案 [!DNL Workfront] 也會附加至在Jira中連結的問題。 新檔案版本來源 [!DNL Workfront] 新增為Jira的獨立檔案，並附加 <i>_v&lt;version number=""&gt;</i> 表示Workfront中的編號版本。 </p><p>例如，如果檔名稱位於 [!DNL Workfront] 是 <strong>主要廣告</strong>，並在中新增新版本 [!DNL Workfront]，則新版本將會轉移至 [!DNL Jira] 作為具有名稱的新檔案 <strong>主要Ad_v2</strong>.</p><p>重要： <p>同步檔案時，請考量下列事項：</p>
           <ul>
            <li><p>大於5MB的檔案不會同步。 如果檔案同步因為檔案太大而失敗，活動記錄中會記錄一個錯誤。 </p><p>如需活動記錄的詳細資訊，請參閱 <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md" class="MCXref xref">檢視Jira活動記錄</a>.</p></li>
            <li><p>連結至外部伺服器任務和問題的檔案不會傳輸至 [!DNL Jira] 個專案。 僅直接在任務上傳的檔案或中的問題 [!DNL Workfront] 已轉移到中的已連結問題 [!DNL Jira].</p></li>
            <li><p>若要從檔案建立校訂，您必須在中產生校訂 [!DNL Workfront]. </p><p>如需產生校訂的詳細資訊，請參閱 <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md#create-a-proof-for-an-existing-document" class="MCXref xref">為現有檔案建立校訂 </a>在 <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md" class="MCXref xref">為檔案建立校訂</a>.<br></p></li>
           </ul></p></td>
        </tr>
        <tr>
         <td role="rowheader">[！UICONTROL計畫完成日期]</td>
         <td><p>中任務或問題的[！UICONTROL規劃完成日期] [!DNL Workfront] 會成為它所連結之問題的[！UICONTROL到期日] [!DNL Jira].</p><p>注意：請確定您顯示 <strong>[！UICONTROL到期日期]</strong> 於 [!DNL Jira] 問題，此值無法同步。</p></td>
        </tr>
       </tbody>
      </table>

1. 在 **[!UICONTROL 同步來源 [!DNL Jira] 至[!DNL Workfront]]** 區段，選取您要更新的欄位 [!DNL Workfront] 當它們更新於 [!DNL Jira].

   1. 選取下列任何與欄位同步化的頻率：

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[！UICONTROL Always]</td>
         <td>您指定的欄位一律會在連結的欄位之間同步 [!DNL Workfront] 和 [!DNL Jira] 欄位更新時的專案 [!DNL Jira]. </td>
        </tr>
        <tr>
         <td role="rowheader">[！UICONTROL從不]</td>
         <td><p>您指定的欄位不會在連結的欄位之間同步 [!DNL Workfront] 和 [!DNL Jira] 個專案。 沒有任何指示 [!DNL Workfront] 欄位已更新的位置 [!DNL Jira]. </p><p>附註：選取「永不」時， [!DNL Workfront] 欄位仍然可以從手動更新 [!DNL Jira] 在左側 [!DNL Workfront] 面板 [!DNL Jira] 問題。 這些更新只會顯示在 [!DNL Workfront] 中的專案 [!DNL Jira] 和 [!DNL Workfront] 且未開啟 [!DNL Jira] 個專案。</p></td>
        </tr>
       </tbody>
      </table>

   1. 選取以同步處理以下任何欄位 [!DNL Jira] 至 [!DNL Workfront]：

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[！UICONTROL狀態]</td>
         <td>中的問題[！UICONTROL狀態] [!DNL Jira] 會成為它所連結之任務或問題的[！UICONTROL狀態] [!DNL Workfront].<br>有關詳細資訊 [!DNL Workfront] 狀態，請參閱 <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">建立或編輯狀態</a>.</td>
        </tr>
        <tr>
         <td role="rowheader">[！UICONTROL受託人]</td>
         <td><p>中的[！UICONTROL問題受指派人] [!DNL Jira] 會成為其所連結之任務或問題的[！UICONTROL受指派人] [!DNL Workfront].</p><p>重要：當您在中指派專案時 [!DNL Jira] 給沒有 [!DNL Workfront] 帳戶，整合會在中建立新的作用中使用者 [!DNL Workfront] 僅當 <strong>自動在中建立使用者 [!DNL Workfront] 如果 [!DNL Jira] 使用者沒有 [!DNL Workfront] 帳戶</strong> 設為 <strong>[！UICONTROL Always]</strong>. 此使用者未佔用 [!DNL Workfront] 授權。 可將作用中的使用者指派給中的工作專案 [!DNL Workfront]，但不能包含在更新中。 </p></td>
        </tr>
        <tr>
         <td role="rowheader">[！UICONTROL附件]</td>
         <td>中的問題附件 [!DNL Jira] 也會附加到連結至的任務或問題 [!DNL Workfront]. </td>
        </tr>
        <tr>
         <td role="rowheader">[！UICONTROL註解]</td>
         <td><p>評論 [!DNL Jira] 問題也會張貼在連結的 [!DNL Workfront] [！UICONTROL更新]區域中的專案。 相反地，在[！UICONTROL更新]區域張貼的評論 [!DNL Workfront] 任務或問題同步至 [!DNL Jira]的原生註解串流。 </p><p>此設定為 <strong>[！UICONTROL Always]</strong> 依預設。 如果您選取 <strong>[！UICONTROL從不]</strong> 在此，您仍然可以在中手動在連結專案上張貼註解 [!DNL Workfront] 或 [!DNL Jira].</p></td>
        </tr>
       </tbody>
      </table>

1. 在 **[!UICONTROL 其他]** 區段，選取連結專案之間應更新哪些其他欄位。

   1. 選取選項以決定您指定的欄位是否為 **[!UICONTROL 一直]** 或 **[!UICONTROL 從不]** 更新位置 [!DNL Jira] 或 [!DNL Workfront] 當它們被修改時。

   1. 從下列欄位和更新中選取：

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[！UICONTROL副本 [!DNL Workfront] 中的右側面板中的自訂資料 [!DNL Jira]]</td>
         <td><p>顯示 [!DNL Workfront] 中的專案自訂資料 [!DNL Workfront] 右側面板。</p><p>注意：自訂表單區段會顯示在 [!DNL Workfront] 右側面板，其存取層級為 [!DNL Workfront] 系統管理員。</p></td>
        </tr>
        <tr>
         <td role="rowheader">[！UICONTROL副本 [!DNL Workfront] 中右側面板的優先順序 [!DNL Jira]]</td>
         <td>顯示 [!DNL Workfront] 中專案的優先順序 [!DNL Workfront] 右側面板。</td>
        </tr>
        <tr>
         <td role="rowheader">[！UICONTROL在 [!DNL Workfront] 有關到期日期變更的更新索引標籤 [!DNL Jira]]</td>
         <td>在的[！UICONTROL Update]索引標籤中新增註解 [!DNL Workfront] 當連結中的[！UICONTROL到期日]變更時的專案 [!DNL Jira] 個專案。</td>
        </tr>
        <tr>
         <td role="rowheader">[！UICONTROL在中自動建立使用者 [!DNL Workfront] 如果 [!DNL Jira] 使用者沒有 [!DNL Workfront] 帳戶]</td>
         <td><p>存在下列情況：</p>
          <ul>
           <li>當您選取 <strong>[！UICONTROL Always]</strong>Workfront ，您可啟用整合，以便在每次 [!DNL Jira] 沒有 [!DNL Workfront] 帳戶會對連結的執行下列動作 [!DNL Jira] 問題：
            <ul>
             <li>指派至 [!DNL Jira] 問題</li>
             <li><p>將時間記錄到 [!DNL Jira] 問題</p><p>此新使用者未佔用 [!DNL Workfront] 授權。 預設設定為「一律」。 使用者在中以這種方式建立 [!DNL Workfront] 「[！UICONTROL Jira]」已新增至其名稱。</p></li>
            </ul></li>
           <li>當您選取 <strong>[！UICONTROL從不]</strong>，會發生下列情況：
            <ul>
             <li>您看不到任何 [!DNL Jira] 任務位於 [!DNL Workfront] 個專案。 在此情況下，僅指派於 [!DNL Workfront] 顯示於 [!DNL Workfront] 個專案。</li>
             <li>記錄至連結的時間 [!DNL Jira] 由沒有 [!DNL Workfront] 帳戶不會自動轉移到已連結的 [!DNL Workfront] 個專案。 您仍然可以將時間登入 [!DNL Workfront] 「 」右側面板中的專案 [!DNL Jira] 問題。</li>
            </ul></li>
          </ul></td>
        </tr>
       </tbody>
      </table>

1. 按一下&#x200B;**[!UICONTROL 儲存]**。

   現在，每次使用者更新此設定中指定的任何欄位（在中的專案上） [!DNL Jira] 或 [!DNL Workfront]，另一個應用程式中的連結專案也會更新。

## 疑難排解

### 無法在中建立專案 [!DNL Jira] 因為觸發欄位標示為&quot;[!UICONTROL 找不到]&quot;

#### 問題

當與發生錯誤時 [!DNL Workfront for Jira] 應用程式， [!DNL Workfront] 停用觸發程式以避免進一步複雜化。 這些觸發程式停用時，會顯示為&quot;[!UICONTROL 找不到].」

#### 解決方案

找出停用觸發程式的錯誤。 您可以在下列位置找到錯誤： [!DNL Workfront for Jira] [!UICONTROL 活動記錄].

發生此行為的最常見原因是錯誤&quot;[!UICONTROL 無法設定&#39;duedate&#39;欄位。 不在適當的熒幕上，或未知。]&quot;

此錯誤表示您正嘗試同步&quot;[!UICONTROL 計畫完成日期]&quot;從 [!DNL Workfront] 至 [!DNL Jira]. 若要這麼做，您必須確保 [!DNL Jira] 物件有一個欄位稱為&quot;[!UICONTROL 到期日期].」 如果他們沒有此欄位， [!DNL Workfront] 無法從同步計畫完成日期 [!DNL Workfront] 和會停用您的觸發程式。

若要解決此錯誤，請嘗試下列方法之一：

* 詢問您的 [!DNL Jira] 管理員以更新受影響的 [!DNL Jira] 物件以確保它們有到期日欄位。
* 停用同步 [!DNL Workfront]的Workfront計畫完成日期 [!UICONTROL 設定] 頁面。
