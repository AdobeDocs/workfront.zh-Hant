---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: 設定 [!DNL Adobe Workfront for Jira]
description: 您可以使用 [!DNL Adobe Workfront for Jira] 整合 [!DNL Jira] 和 [!DNL Workfront] 系統。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 959adc88-5201-4945-96c4-ea890f0bd371
source-git-commit: d2c366a69b986bd8d559a18994810011c6d33441
workflow-type: tm+mt
source-wordcount: '2413'
ht-degree: 0%

---

# 設定 [!DNL Adobe Workfront for Jira]

您可以使用 [!DNL Adobe Workfront for Jira] 整合 [!DNL Jira] 和 [!DNL Workfront] 系統。

安裝附加元件後，您可以定義要建立的工作流程 [!DNL Jira] 自動發生 [!DNL Workfront] 工作項目隨即建立。 兩個應用程式中的項都會被連結，並且它們的某些資訊會在兩個系統中自動更新。

中的所有使用者 [!DNL Workfront] 和 [!DNL Jira] 可從這項整合中獲益。 他們只需要系統的許可證，而不是兩個系統。

此附加元件適用於 [!UICONTROL 伺服器] 和 [!UICONTROL OnDemand] (或 [!UICONTROL 雲])版本 [!DNL Jira] 軟體。

若需 [!DNL Jira] 版本 [!DNL Workfront for Jira] 目前支援，請參閱 [[!DNL Workfront for Jira]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview) at [!DNL Atlassian Marketplace].

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] 計劃]</a>*</td> 
   <td> <p>[!UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] 授權概述</a>*</td> 
   <td> <p>[!UICONTROL計畫]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] 存取</td> 
   <td> <p>系統管理員存取</p> <p>重要：建議您在 [!DNL Jira] 和 [!DNL Workfront] 以專用於此整合，而非使用可能附加至使用者的現有整合。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>您必須是 [!DNL Workfront] 管理員。 如需 [!DNL Workfront] 管理員請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>.</p> <p>注意：如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可修改您的存取層級，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 必要條件

設定之前 [!DNL Workfront for Jira]，您必須

* 安裝 [!DNL Workfront for Jira]\
   安裝說明 [!DNL Workfront for Jira]，請參閱 [安裝 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## 設定 [!DNL Workfront for Jira]

透過設定 [!DNL Workfront for Jira] 您可以：

* 定義要建立的觸發器 [!DNL Jira] 項目發生時 [!DNL Workfront] 項目。
* 指定在連結之間的項目之間應同步的欄位 [!DNL Jira] 和 [!DNL Workfront].

>[!NOTE]
>
>* 設定後 [!DNL Workfront for Jira] 在 [!DNL Jira] 環境，全部 [!DNL Jira] 使用者可看見 [!DNL Workfront] 右面板 [!DNL Jira] 項目。 面板包含可能連結的項目的相關資訊 [!DNL Workfront] 或指定否 [!DNL Workfront] 項目連結至 [!DNL Jira] 項目。
>* 使用 [!DNL Jira Server] 安裝時，只有與已識別為Workfront整合觸發器的專案相關的問題才會顯示「Workfront」面板。 如需為設定觸發器的詳細資訊 [!DNL Workfront to Jira] 工作流程，請參閱 [設定自動連結項目的觸發器 [!DNL Jira] 和 [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).
>




配置 [!DNL Workfront for Jira]:

1. 登入 [!DNL Jira] as a [!DNL Jira] 管理員。
1. 按一下 **[!UICONTROL 設定]** 在 [!DNL Jira] 功能表。
1. 按一下 **[!UICONTROL 附加元件]**，然後按一下 **[!UICONTROL 管理附加元件]**.

1. 展開 **[!DNL Workfront]** 附加元件。
1. 按一下 **[!UICONTROL 設定]**.
1. 按照提示登錄 [!DNL Workfront].

   >[!NOTE]
   >
   >使用者必須具備有效 `apiKey` in [!UICONTROL Workfront] 來建立成功的連線。

   您必須登入 [!DNL Workfront] as a [!DNL Workfront] 管理員繼續配置。

   >[!NOTE]
   >
   >* [!UICONTROL Workfront] 連接 [!DNL Jira] 使用OAuth 2.0，此標準供大部分網頁型整合用來驗證和授權使用者。
   >* 當系統提示您輸入 [!DNL Workfront] 帳戶，請使用此格式輸入： *yourCompany&#39;sDomain.my.workfront.com*. 您公司的網域通常是您公司的名稱。
   >* 增強驗證必須在 [!DNL Workfront] 管理員會啟用此整合。



1. 選取 **[!UICONTROL 觸發器]** 標籤來設定自動建立 [!DNL Jira] 新項目 [!DNL Workfront] 項目。

   如需設定觸發器的詳細資訊，請參閱「 Workfront [!DNL Jira] 工作流程，請參閱 [設定自動連結項目的觸發器 [!DNL Jira] 和 [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).

1. 選取 **[!UICONTROL 設定]** 頁簽，以配置連結之間的欄位同步 [!DNL Jira] 和 [!DNL Workfront] 項目。

   有關設定欄位同步的詳細資訊，請參閱 [!DNL Jira] 和 [!DNL Workfront]，請參閱 [在 [!DNL Jira] 和 [!DNL Workfront] 項目](#configure-field-synchronization-between-jira-and-workfront-items).

   >[!NOTE]
   >
   >在您定義觸發器並同步兩個應用程式之間的欄位後，任何 [!DNL Workfront] 可以建立任務或問題的用戶可能會觸發在 [!DNL Jira]. 如果使用者所建立項目的條件符合中的觸發器，則使用者可以建立項目 [!DNL Jira]，即使使用者沒有 [!DNL Jira] 授權。 此外， [!DNL Jira] 使用者可以立即開始使用 [!DNL Jira] 項目，且其更新會顯示在 [!DNL Workfront]，卻沒有 [!DNL Workfront] 授權。 中的任何更新 [!DNL Workfront] 也會顯示在 [!DNL Jira] 項目。

1. （選用）選取 **[!UICONTROL 活動記錄]** 標籤，檢閱整合期間可能發生的任何錯誤。

   如需 [!UICONTROL 活動記錄]，請參閱 [檢視 [!DNL Jira] [!UICONTROL 活動記錄]](../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md).

## 設定自動連結項目的觸發器 [!DNL Jira] 和 [!DNL Workfront]

作為 [!DNL Jira] 系統管理員，您可以定義觸發器，以自動在 [!DNL Jira] 當 [!DNL Workfront] 符合某些標準。

>[!NOTE]
>
>整合最多可能需要10分鐘，才能在 [!DNL Jira].

設定觸發建立時，請考量下列事項 [!DNL Jira] 項目為 [!DNL Workfront] 項目已建立：

* 整合是單向的：您只能觸發在中建立的項目 [!DNL Workfront] 自動建立於 [!DNL Jira]. 您無法觸發在中建立的項目 [!DNL Jira] 自動建立 [!DNL Workfront].
* 您可以擁有的觸發器數量沒有限制。
* 如果您在 [!DNL Workfront] 符合多個觸發器，則只會在中建立一個項目 [!DNL Jira]. 項目是在 [!DNL Jira] 根據第一個觸發(依定義於 [!DNL Jira])。 所有其他觸發器則會遭忽略。
* 中只有一個項目 [!DNL Workfront] 可連結至Jira中的一個項目。 您永遠無法連結 [!DNL Workfront] 項目至多個 [!DNL Jira] 問題或 [!DNL Jira] 問題至多個 [!DNL Workfront] 項目。

配置觸發器以在中自動建立項目 [!DNL Jira]:

1. 登入 [!DNL Jira] 作為系統管理員。
1. 按一下 **[!UICONTROL 設定]** 在 [!DNL Jira] 功能表。
1. 按一下 **[!UICONTROL 附加元件]**，然後 **[!UICONTROL 管理附加元件]**.

1. 展開 **[!DNL Workfront]** 附加元件。
1. 按一下 **[!UICONTROL 設定]**.
1. 登入 [!DNL Workfront] 作為系統管理員。

   此 **[!UICONTROL 觸發器]** 標籤。

1. 按一下 **[!UICONTROL 新增觸發程式]** 以新增觸發器。
1. 在 **[!UICONTROL Workfront團隊/使用者/角色]** 欄位，指定 [!DNL Workfront] 團隊、使用者或工作角色，然後按一下以在清單中顯示時加以選取。

   >[!NOTE]
   >
   >同一團隊、使用者或角色不能有多個觸發器。

   當某人建立任務或問題，並將其指派給其中一個實體時，系統會在[!DNL中自動建立問題 [!DNL Jira]]。

1. 在 **[!UICONTROL [!DNL Jira]專案]** 欄位，開始鍵入 [!DNL Jira] 專案，然後按一下以在清單中顯示時選取。

   當 [!DNL Jira] 問題會建立，並放置在您在此指定的專案上。

1. 選取 **我[!UICONTROL ssue類型]** 從下拉式功能表。

   這表示在中建立的問題類型 [!DNL Jira] 當符合此觸發器的條件時，會根據您針對 [!DNL Jira].

1. 按一下&#x200B;**[!UICONTROL 儲存]**。

   使用此設定時，每次 [!DNL Workfront] 使用者會建立符合指定觸發器的項目，而 [!DNL Jira].

## 在 [!DNL Jira] 和 [!DNL Workfront] 項目

作為 [!DNL Jira] 管理員，您可以定義應針對在之間連結的項目自動同步的欄位 [!DNL Workfront] 和吉拉。 某些欄位可從 [!DNL Workfront] 到 [!DNL Jira] 項目，而其他項目則從Jira同步至Workfront。

要定義在兩個應用程式之間連結的項目上自動同步的欄位，請執行以下操作：

1. 登入 [!DNL Jira] Jira管理員。
1. 按一下 **[!UICONTROL 設定]** 在 [!DNL Jira] 功能表。
1. 按一下 **[!UICONTROL 附加元件]**，然後 **[!UICONTROL 管理附加元件]**.

1. 展開 **[!DNL Workfront]** 附加元件。
1. 按一下 **[!UICONTROL 設定]**.
1. 登入 [!DNL Workfront] 身為Workfront管理員。
1. 按一下 **[!UICONTROL 設定]** 標籤。

1. 在 **[!UICONTROL 從Jira同步到Workfront]** 區段中，選擇要更新的欄位 [!DNL Jira] 在Workfront中更新時。

   1. 選擇與欄位同步的以下任何頻率：

      <table style="table-layout:auto">
         <tr>
              <td>[!UICONTROL建立時]</td>
              <td>您指定的欄位會在連結的Workfront和 [!DNL Jira] 在Workfront中建立項目時顯示的項目。</td>
          </tr>
          <tr>
              <td>[!UICONTROL Always]</td>
              <td>您指定的欄位會在連結的Workfront和 [!DNL Jira] 在Workfront中更新欄位時顯示的項目。 </td>
          </tr>
          <tr>
              <td>[!UICONTROL從不]</td>
              <td>您指定的欄位不會在連結的 [!DNL Workfront] 和 [!DNL Jira] 項目。 在 [!DNL Jira] 欄位已更新於 [!DNL Workfront]. </td>
          </tr>
      </table>

   1. 選取，從 [!DNL Workfront] to [!DNL Jira]:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL名稱]</td>
         <td><p>中的任務或問題的名稱 [!DNL Workfront] 會成為其連結的問題名稱 [!DNL Jira].</p><p>注意：在中建立新項目時 [!DNL Jira] 自動， [!DNL Workfront] 名稱一律會更新 [!DNL Jira] 項目，無論此欄位是否啟用。 當 [!DNL Jira] 項目會手動連結至 [!DNL Workfront] 項目，名稱 [!DNL Workfront] 僅更新項目 [!DNL Jira] 選擇 <strong>一律</strong> 同步此欄位。 如需手動或自動連結項目的詳細資訊，請參閱 <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md" class="MCXref xref">在 [!DNL Adobe Workfront] 和 [!DNL Jira]</a>.</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL描述]</td>
         <td>中的任務或問題的說明 [!DNL Workfront] 會成為連結問題的說明 [!DNL Jira].</td>
        </tr>
        <tr>
         <td role="rowheader">文件</td>
         <td><p>附加至任務或問題的文檔 [!DNL Workfront] 也附於Jira中與之連結的問題。 新文檔版本來自 [!DNL Workfront] 作為單獨的文檔添加到Jira中，並附加 <i>_v&lt;version number=""&gt;</i> 以在Workfront中指出編號版本。 </p><p>例如，如果 [!DNL Workfront] is <strong>主要廣告</strong>，並在 [!DNL Workfront]，則新版本會轉移至 [!DNL Jira] 作為名稱為的新文檔 <strong>主Ad_v2</strong>.</p><p>重要: <p>同步檔案時，請考慮下列事項：</p>
           <ul>
            <li><p>大於5MB的文檔不同步。 如果檔案同步因檔案過大而失敗，則會在活動記錄中記錄錯誤， </p><p>如需活動記錄的詳細資訊，請參閱 <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md" class="MCXref xref">查看Jira活動日誌</a>.</p></li>
            <li><p>連結至來自外部伺服器的任務和問題的檔案不會傳輸至 [!DNL Jira] 項目。 僅直接上傳至任務或 [!DNL Workfront] 會轉移至 [!DNL Jira].</p></li>
            <li><p>要從文檔建立校樣，必須在 [!DNL Workfront]. </p><p>如需產生校樣的詳細資訊，請參閱 <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md#create" class="MCXref xref">為現有文檔建立校樣 </a>in <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md" class="MCXref xref">為文檔建立校樣</a>.<br></p></li>
           </ul></p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL計畫完成日期]</td>
         <td><p>任務或問題的[!UICONTROL計畫完成日期] [!DNL Workfront] 變成連結至的問題的[!UICONTROL到期日] [!DNL Jira].</p><p>注意：確保顯示 <strong>[!UICONTROL到期日]</strong> on [!DNL Jira] 問題，以便同步此值。</p></td>
        </tr>
       </tbody>
      </table>

1. 在 **[!UICONTROL 從同步 [!DNL Jira] to[!DNL Workfront]]** 區段中，選擇要更新的欄位 [!DNL Workfront] 當 [!DNL Jira].

   1. 選擇與欄位同步的以下任何頻率：

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Always]</td>
         <td>您指定的欄位一律會在連結的 [!DNL Workfront] 和 [!DNL Jira] 項目 [!DNL Jira]. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL從不]</td>
         <td><p>您指定的欄位不會在連結的 [!DNL Workfront] 和 [!DNL Jira] 項目。 在 [!DNL Workfront] 欄位已更新於 [!DNL Jira]. </p><p>注意：選擇「從不」時， [!DNL Workfront] 欄位仍可手動從 [!DNL Jira] 左邊 [!DNL Workfront] 面板 [!DNL Jira] 問題。 這些更新只會顯示在 [!DNL Workfront] 項目 [!DNL Jira] 和 [!DNL Workfront] 不開啟 [!DNL Jira] 項目。</p></td>
        </tr>
       </tbody>
      </table>

   1. 選取，從 [!DNL Jira] to [!DNL Workfront]:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL狀態]</td>
         <td>中問題的[!UICONTROL狀態] [!DNL Jira] 會成為連結任務或問題的[!UICONTROL狀態] [!DNL Workfront].<br>如需 [!DNL Workfront] statuses，請參閱 <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">建立或編輯狀態</a>.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL受託人]</td>
         <td><p>中問題的[!UICONTROL受託人] [!DNL Jira] 會成為連結任務或問題的[!UICONTROL受託人] [!DNL Workfront].</p><p>重要：當您在 [!DNL Jira] 使用者 [!DNL Workfront] 帳戶時，整合會在 [!DNL Workfront] 只有在 <strong>在中自動建立使用者 [!DNL Workfront] 若 [!DNL Jira] 使用者沒有 [!DNL Workfront] 帳戶</strong> 設為 <strong>[!UICONTROL Always]</strong>. 此使用者未佔用 [!DNL Workfront] 授權。 可以為中的工作項目指派活躍的使用者 [!DNL Workfront]，但無法納入更新中。 </p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL附件]</td>
         <td>中問題的附件 [!DNL Jira] 也會附加至連結至的任務或問題 [!DNL Workfront]. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL注釋]</td>
         <td><p>關於 [!DNL Jira] 問題也發佈在連結的 [!DNL Workfront] 項目。 反之，在[!UICONTROL更新]區域中張貼的評論 [!DNL Workfront] 任務或問題同步到 [!DNL Jira]連結問題的原生注釋流。 </p><p>此值已設為 <strong>[!UICONTROL Always]</strong> 依預設。 如果您選取 <strong>[!UICONTROL從不]</strong> 在此，您仍可以在 [!DNL Workfront] 或 [!DNL Jira].</p></td>
        </tr>
       </tbody>
      </table>

1. 在 **[!UICONTROL 其他]** 區段中，選取應在連結項目之間更新的其他欄位。

   1. 選取選項，以決定您指定的欄位 **[!UICONTROL 一律]** 或 **[!UICONTROL 從不]** 更新 [!DNL Jira] 或 [!DNL Workfront] 的子句。

   1. 從下列欄位和更新中選取：

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL副本 [!DNL Workfront] 中右側面板的自訂資料 [!DNL Jira]]</td>
         <td><p>顯示 [!DNL Workfront] 中項目的自訂資料 [!DNL Workfront] 右面板。</p><p>注意：「自訂表單」區段會顯示在 [!DNL Workfront] 右側面板，其存取層級為 [!DNL Workfront] 系統管理員。</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL副本 [!DNL Workfront] 在的右側面板中，優先順序 [!DNL Jira]]</td>
         <td>顯示 [!DNL Workfront] 項目的優先順序 [!DNL Workfront] 右面板。</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL在 [!DNL Workfront] 「更新」標籤中的「到期日」變更 [!DNL Jira]]</td>
         <td>在 [!DNL Workfront] 項目 [!DNL Jira] 項目。</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL在中自動建立用戶 [!DNL Workfront] 若 [!DNL Jira] 使用者沒有 [!DNL Workfront] account]</td>
         <td><p>存在下列情況：</p>
          <ul>
           <li>選取 <strong>[!UICONTROL Always]</strong> 您可以啟用整合，以在每次 [!DNL Jira] 沒有 [!DNL Workfront] 帳戶會對連結的 [!DNL Jira] 問題：
            <ul>
             <li>已指派給 [!DNL Jira] 問題</li>
             <li><p>將時間記錄到 [!DNL Jira] 問題</p><p>此新使用者不會佔用 [!DNL Workfront] 授權。 預設設定為「一律」。 使用者在 [!DNL Workfront] 名稱中新增了「[!UICONTROL Jira]」。</p></li>
            </ul></li>
           <li>選取 <strong>[!UICONTROL從不]</strong>，會發生下列情況：
            <ul>
             <li>您看不到任何 [!DNL Jira] 分配 [!DNL Workfront] 項目。 在此情況下，僅執行 [!DNL Workfront] 顯示於 [!DNL Workfront] 項目。</li>
             <li>記錄到連結的時間 [!DNL Jira] 使用者的問題 [!DNL Workfront] 帳戶不會自動轉移至已連結的 [!DNL Workfront] 項目。 您仍可在 [!DNL Workfront] 項目 [!DNL Jira] 問題。</li>
            </ul></li>
          </ul></td>
        </tr>
       </tbody>
      </table>

1. 按一下&#x200B;**[!UICONTROL 儲存]**。

   現在，每當使用者更新此設定中針對其中一個項目所指定的任何欄位時 [!DNL Jira] 或 [!DNL Workfront]，也會更新其他應用程式中的連結項目。

## 疑難排解

### 無法在中建立項目 [!DNL Jira] 因為標有「[!UICONTROL 找不到]&quot;

#### 問題

當 [!DNL Workfront for Jira] 應用程式， [!DNL Workfront] 禁用觸發器以防止進一步併發症。 當這些觸發器停用時，會顯示為「[!UICONTROL 找不到]」。

#### 解決方案

找出停用觸發器的錯誤。 您可以在 [!DNL Workfront for Jira] &quot;[!UICONTROL 活動記錄]」。

此行為最常見的原因是錯誤「[!UICONTROL 無法設定「duedate」欄位。 不在適當的畫面中，或未知。]&quot;

此錯誤表示您正嘗試同步「[!UICONTROL 計畫完成日期]從 [!DNL Workfront] to [!DNL Jira]. 若要這麼做，您必須確保 [!DNL Jira] 對象具有名為「[!UICONTROL 到期日]」。 如果他們沒有這個欄位， [!DNL Workfront] 無法同步計畫完成日期，從 [!DNL Workfront] 和停用您的觸發器。

若要解決此錯誤，請嘗試下列其中一項操作：

* 詢問 [!DNL Jira] 管理員以更新受影響的 [!DNL Jira] 物件，確保其具有到期日欄位。
* 停用 [!DNL Workfront]Workfront中的計畫完成日期「[!UICONTROL 設定]「 」頁面
