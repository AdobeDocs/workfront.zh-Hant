---
title: 配置文檔整合
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: 配置文檔整合
author: Courtney, Caroline
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: cf5c4e3d-b45f-46cd-a938-22e412d1c491
source-git-commit: 456c7b21835c96912e8974063f7797283dcb4e6d
workflow-type: tm+mt
source-wordcount: '1161'
ht-degree: 1%

---

# 配置文檔整合

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

作為 [!DNL Adobe Workfront] 管理員，您可以配置文檔整合以管理 [!UICONTROL Workfront]。 您還可以配置 [!UICONTROL Workfront] 因此文檔僅儲存在文檔服務應用程式中，而不儲存在 [!UICONTROL Workfront] 本身。 有關詳細資訊，請參見 [更新並連結文檔 [!UICONTROL Workfront] 到外部雲提供程式](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#sending-documents) 在 [從外部應用程式連結文檔](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)。

>[!NOTE]
>
>允許在 [!DNL Workfront Proof] 和 [!DNL Workfront] 伺服器，您可能需要將某些IP地址添加到允許清單。 有關詳細資訊，請參見 [配置防火牆的允許清單](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)。

## 訪問要求

要執行本文中的步驟，必須具備以下條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 許可證</td> 
   <td>[!UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>你一定是 [!DNL Workfront] 管理員。 有關 [!DNL Workfront] 管理員，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用戶完全管理訪問權限</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要瞭解您擁有的計畫、許可證類型或訪問權限，請與 [!DNL Workfront] 管理員。

## 支援的整合

<!--DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

您可以配置以下整合以管理文檔：

<!--
  Experience Manager Assets Essentials </p>
  -->

* [!DNL Workfront DAM]

* [!DNL Workfront Proof]

   連結來自 [!DNL Workfront Proof] 允許您製作最初在 [!DNL Workfront Proof] 可用 [!DNL Workfront]。 A [!UICONTROL 專業] [!DNL Workfront] 使用此功能需要計畫或更高版本。 有關各種可用計畫的詳細資訊，請參閱 [Workfront計畫。](https://www.workfront.com/plans)

* [!DNL Microsoft SharePoint]

   有關與整合的資訊 [!DNL SharePoint]，請參閱 [配置 [!DNL SharePoint] 整合](../../administration-and-setup/configure-integrations/configure-sharepoint-integration.md)。

* 第三方雲文檔提供程式：

   * [!DNL Box]
   * [!DNL Dropbox]
   * [!DNL Dropbox Business]
   * [!DNL WebDAM]
   * [!DNL Microsoft OneDrive]
   * [!DNL Microsoft SharePoint]
   * [!UICONTROL Google Drive]

      <!--Quip-->
   >[!TIP]
   >
   >您可以使用直接驗證和批准上載到外部雲提供商的文檔的方法，來驗證和批准從外部雲提供商連結的文檔 [!DNL Workfront]。

* 其他文檔提供程式（通過自定義文檔整合）。

   A [!UICONTROL 專業] [!DNL Workfront] 使用此功能需要計畫或更高版本。 有關各種可用計畫的詳細資訊，請參閱 [[!DNL Workfront] 計畫。](https://www.workfront.com/plans)

此外，您還可以 [!DNL Workfront] 使用本機數字資產管理(DAM)系統或第三方DAM整合的文檔體驗。 管理員必須啟用這些功能，以便用戶將服務連結到其 [!DNL Workfront] 帳戶。 有關Workfront大壩的詳細資訊，請參見 [管理文檔 [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md)。

## 配置整合以管理文檔

1. 登錄到 [!DNL Workfront] 作為管理員。
1. 按一下 **[!UICONTROL 主菜單]** 表徵圖 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png)。

1. 在左面板中，按一下 **[!UICONTROL 文檔]** > **[!UICONTROL 雲提供程式]。**

1. （可選）將文檔儲存在文檔服務應用程式中，而不是 [!DNL Workfront]選中 **[!UICONTROL 防止用戶將文檔儲存在 [!DNL Workfront]]。**

1. 選擇要啟用的整合。
1. 按一下&#x200B;**[!UICONTROL 儲存]**。

如果要設定與 [!DNL Workfront DAM]，您可以啟用 [!DNL Workfront] 將元資料包含在文檔中。 有關映射元資料的資訊，請參見 [設定元資料映射](../../administration-and-setup/configure-integrations/set-up-metadata-mapping.md)。

## 配置自定義文檔整合

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **)</p>
-->

自定義文檔整合允許 [!DNL Workfront] 將檔案連結到 [!DNL Workfront] 只要系統與 [!DNL Workfront]。

要使自定義整合對用戶可用，您首先需要構建整合。 有關如何構建要與 [!DNL Workfront]，請參閱 [文檔Webhooks API](../../wf-api/doc-wbhks-api/docu-webhook-api.md)。

構建自定義文檔整合後，您可以將其提供給站點上的用戶。

1. 登錄到 [!DNL Workfront] 作為管理員。
1. 按一下 **[!UICONTROL 主菜單]** 表徵圖 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png)。

1. 在左面板中，按一下 **[!UICONTROL 文檔]** > **[!UICONTROL 自定義整合]。**

1. 按一下 **[!UICONTROL 添加自定義整合]**。
1. 指定以下資訊以配置整合：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL名稱]</td> 
      <td>自定義整合的名稱。 這是用戶在使用Workfront內的整合時看到的名稱。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL基API URL] </td> 
      <td>API調用的基HTTP或安全HTTP URL。 比如說， <a class="link-https" title="https://documentprovider.com/api/v2" href="https://documentprovider.com/api/v2">https://documentprovider.com/api/v2</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL身份驗證類型]</td> 
      <td> <p>對自定義整合進行授權API調用時要使用的驗證方法。</p> 
       <ul> 
        <li>如果您選擇 <strong>[!UICONTROL OAuth]</strong>，繼續步驟6。</li> 
        <li>如果您選擇 <strong>[!UICONTROL ApiKey]</strong>，繼續步驟7。</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. （條件）如果選擇 **[!UICONTROL OAuth]** 驗證 **[!UICONTROL 驗證類型]**，指定以下資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL身份驗證URL]</td> 
      <td>用於用戶驗證的完整URL。 [!DNL Workfront] 將用戶導航到此地址，作為OAuth預配過程的一部分。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL標籤終結點URL]</td> 
      <td>用於擷取 OAuth 權杖的完整 API URL。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL客戶端ID]</td> 
      <td>此整合的OAut客戶端ID。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL客戶端密鑰]</td> 
      <td>此整合的OAut客戶端密碼。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL請求參數]</td> 
      <td> <p>指定要附加到每個API調用的查詢字串的可選值。 例如，access_type=offline。</p> <p>要添加多個請求參數，請按一下 <strong>+添加請求參數</strong>。</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >的 [!DNL Workfront] 重定向顯示在 [!UICONTROL 自定義整合] 頁面列出了用於向外部文檔提供程式註冊此整合的URI。

1. （條件）如果選擇 **[!UICONTROL ApiKey]** 驗證 **[!UICONTROL 驗證類型]**，指定由自定義文檔提供程式頒發的API密鑰。

   [!DNL Workfront] 使用此API密鑰對文檔提供程式進行授權API調用。

1. 按一下 **[!UICONTROL 保存]** 的子菜單。

## 使用文檔整合

有關用戶如何使用的資訊 [!DNL Workfront DAM]，請參閱 [管理文檔 [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md)。

有關用戶如何使用校對的資訊，請參見 [建立校樣](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs--in-wf.md)。

有關用戶在配置第三方文檔整合後如何使用這些整合的資訊，請參見 [從外部應用程式連結文檔](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)。

### 配置 [!DNL Workfront] 將元資料發送到 [!UICONTROL [!DNL Workfront] 水壩] {#configure-workfront-to-send-metadata-to-workfront-dam}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **) </p>
-->

從發送文檔時 [!DNL Workfront] 至 [!DNL Workfront DAM]，您也可以發送與該文檔關聯的資訊。 有關文檔的資訊映射到 [!DNL Workfront DAM] 元資料。

僅單向映射資訊，從 [!DNL Workfront] 至 [!DNL Workfront DAM] 並且僅當文檔上載到 [!DNL Workfront DAM]。 Workfront欄位中的任何將來更改都不會更新中的元資料欄位 [!DNL Workfront DAM] 上載文檔後。\
可以映射相同 [!DNL Workfront] 各種 [!DNL Workfront DAM] 欄位，但不能使用相同 [!DNL Workfront DAM] 多個欄位 [!DNL Workfront] 的子菜單。

如果必須配置多個 [!DNL Workfront] 將欄位導出到一個 [!DNL Workfront DAM] 欄位，首先在中建立計算的自定義欄位 [!DNL Workfront] 顯示對象的所有單個自定義欄位。 然後，映射計算出的 [!DNL Workfront] 欄位為1 [!DNL Workfront DAM] 的子菜單。\
有關計算的自定義欄位的詳細資訊，請參見 [將計算資料添加到自定義窗體](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)。

映射影響任何用戶從中上載的所有文檔 [!DNL Workfront] 至 [!UICONTROL Workfront] 水壩。

作為 [!DNL Workfront] 管理員，必須啟用 [!DNL Workfront DAM] 在Workfront中，然後才能映射元資料映射進程的欄位。 有關如何啟用的詳細資訊 [!DNL Workfront DAM]，請參閱 [配置Workfront以將元資料發送到 [!DNL Workfront DAM]](#configure-workfront-to-send-metadata-to-workfront-dam)。

配置 [!DNL Workfront] 將元資料發送到 [!DNL Workfront DAM]:

1. 按一下 **[!UICONTROL 主菜單]** 表徵圖 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png)。

1. 按一下 **[!UICONTROL 文檔]** > **[!UICONTROL 元資料映射]**。

1. 在 **[!UICONTROL 選擇用於映射的源欄位]** 欄位，開始鍵入要映射到的Workfront欄位的名稱 [!DNL Workfront DAM]，然後在清單中看到它時選擇它。
1. 在 **[!UICONTROL 選擇用於映射的目標欄位]**，選擇 [!DNL Workfront DAM] 要用所選 [!DNL Workfront] 的子菜單。

   >[!NOTE]
   >
   > 所有發送到的文檔 [!DNL Workfront DAM] 具有此權限的用戶將其元資料更新為 [!DNL Workfront] 映射到此處的欄位，當它們上載到 [!DNL Workfront DAM]。

1. 按一下 **[!UICONTROL 添加映射]**。

1. 繼續添加更多 [!UICONTROL Workfront] 欄位和對應 [!DNL Workfront DAM] 的子菜單。

### 刪除映射的欄位

1. 按一下 **[!UICONTROL 主菜單]** 表徵圖 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png)。

1. 展開 **[!UICONTROL 文檔]**，然後按一下 **[!UICONTROL 元資料映射]**。

1. 在欄位清單中，選擇要從元資料映射中刪除的任何欄位。
1. 按一下 **[!UICONTROL 刪除]**。

   從元資料映射中刪除欄位，並且其中包含的資訊不會傳輸到 [!DNL Workfront DAM] 上載的檔案。
