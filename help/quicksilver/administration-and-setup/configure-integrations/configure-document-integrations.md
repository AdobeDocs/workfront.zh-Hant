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
source-git-commit: ceda437684f565b91dbb8b02f6b03cbe8d27a70a
workflow-type: tm+mt
source-wordcount: '1161'
ht-degree: 1%

---

# 配置文檔整合

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

作為 [!DNL Adobe Workfront] 管理員，您可以配置文檔整合，以管理 [!UICONTROL Workfront]. 您也可以設定 [!UICONTROL Workfront] 這樣，文檔僅儲存在文檔服務應用程式中，而不儲存在 [!UICONTROL Workfront] 本身。 如需詳細資訊，請參閱 [更新並連結來自 [!UICONTROL Workfront] 外部雲提供商](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#sending-documents) in [從外部應用程式連結文檔](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

>[!NOTE]
>
>允許在 [!DNL Workfront Proof] 和 [!DNL Workfront] 伺服器，則您可能需要將特定IP位址新增至允許清單。 如需詳細資訊，請參閱 [配置防火牆的允許清單](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## 存取需求

您必須具備下列條件才能執行本文所述步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td>[!UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>您必須是 [!DNL Workfront] 管理員。 如需 [!DNL Workfront] 管理員請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 支援的整合

<!--DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

您可以設定下列整合以管理檔案：

<!--
  Experience Manager Assets Essentials </p>
  -->

* [!DNL Workfront DAM]

* [!DNL Workfront Proof]

   連結校樣來自 [!DNL Workfront Proof] 可讓您製作原本於 [!DNL Workfront Proof] 可在 [!DNL Workfront]. A [!UICONTROL Pro] [!DNL Workfront] 使用此功能需要計畫或更高版本。 如需各種可用計畫的詳細資訊，請參閱 [Workfront計畫。](https://www.workfront.com/plans)

* [!DNL Microsoft SharePoint]

   如需與整合的相關資訊 [!DNL SharePoint]，請參閱 [設定 [!DNL SharePoint] 整合](../../administration-and-setup/configure-integrations/configure-sharepoint-integration.md).

* 第三方雲文檔提供程式：

   * [!DNL Box]
   * [!DNL Dropbox]
   * [!DNL Dropbox Business]
   * [!DNL WebDAM]
   * [!DNL Microsoft OneDrive]
   * [!UICONTROL Google Drive]

      <!--Quip-->
   >[!TIP]
   >
   >您可以透過直接上傳至的校樣和核准檔案的方式，校樣並核准從外部雲端提供者連結的檔案 [!DNL Workfront].

* 其他檔案提供者（透過自訂檔案整合）。

   A [!UICONTROL Pro] [!DNL Workfront] 使用此功能需要計畫或更高版本。 如需各種可用計畫的詳細資訊，請參閱 [[!DNL Workfront] 計畫。](https://www.workfront.com/plans)

此外，您還可以 [!DNL Workfront] 透過原生數位資產管理(DAM)系統或第三方DAM整合提供檔案體驗。 管理員必須啟用這些功能，才能讓使用者將服務連結至其 [!DNL Workfront] 帳戶。 如需Workfront DAM的詳細資訊，請參閱 [使用管理文檔 [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

## 配置整合以管理文檔

1. 登入 [!DNL Workfront] 管理員。
1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **[!UICONTROL 檔案]** > **[!UICONTROL 雲端提供者].**

1. （可選）將文檔儲存在文檔服務應用程式中，而不是 [!DNL Workfront]，選取 **[!UICONTROL 阻止用戶將文檔儲存在 [!DNL Workfront]].**

1. 選取您要啟用的整合。
1. 按一下&#x200B;**[!UICONTROL 儲存]**。

如果您要設定與 [!DNL Workfront DAM]，您可以啟用 [!DNL Workfront] 包括元資料和文檔。 如需對應中繼資料的資訊，請參閱 [設定中繼資料對應](../../administration-and-setup/configure-integrations/set-up-metadata-mapping.md).

## 設定自訂檔案整合

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **)</p>
-->

自訂檔案整合可讓 [!DNL Workfront] 將檔案連結到 [!DNL Workfront] 從幾乎任何系統中，只要系統是用於 [!DNL Workfront].

若要讓自訂整合可供使用者使用，您必須先建立整合。 如需如何建立要搭配使用的整合的相關資訊 [!DNL Workfront]，請參閱 [文檔Webhook API](../../wf-api/doc-wbhks-api/docu-webhook-api.md).

建置自訂檔案整合後，您就可以讓網站上的使用者使用該整合。

1. 登入 [!DNL Workfront] 管理員。
1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **[!UICONTROL 檔案]** > **[!UICONTROL 自訂整合].**

1. 按一下 **[!UICONTROL 新增自訂整合]**.
1. 指定下列資訊以設定整合：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL名稱]</td> 
      <td>自訂整合的名稱。 這是使用者在使用Workfront中的整合時看到的名稱。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Base API URL] </td> 
      <td>API呼叫的基礎HTTP或安全HTTP URL。 例如， <a class="link-https" title="https://documentprovider.com/api/v2" href="https://documentprovider.com/api/v2">https://documentprovider.com/api/v2</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL驗證類型]</td> 
      <td> <p>對自訂整合進行授權API呼叫時要使用的驗證方法。</p> 
       <ul> 
        <li>如果您選擇 <strong>[!UICONTROL OAuth]</strong>，繼續步驟6。</li> 
        <li>如果您選擇 <strong>[!UICONTROL ApiKey]</strong>，繼續步驟7。</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. （條件性）如果您選取 **[!UICONTROL OAuth]** 驗證 **[!UICONTROL 驗證類型]**，請指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL驗證URL]</td> 
      <td>用於使用者驗證的完整URL。 [!DNL Workfront] 將使用者導覽至此位址，作為OAuth布建程式的一部分。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL令牌端點URL]</td> 
      <td>用於擷取 OAuth 權杖的完整 API URL。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL客戶端ID]</td> 
      <td>此整合的OAut用戶端ID。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL客戶端密碼]</td> 
      <td>此整合的OAut用戶端密碼。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL請求參數]</td> 
      <td> <p>指定要附加至每個API呼叫之查詢字串的選用值。 例如， access_type=offline。</p> <p>若要新增多個請求參數，請按一下 <strong>+新增請求參數</strong>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >此 [!DNL Workfront] 顯示在 [!UICONTROL 自訂整合] 頁面列出用於註冊與外部文檔提供程式的整合的URI。

1. （條件性）如果您選取 **[!UICONTROL ApiKey]** 驗證 **[!UICONTROL 驗證類型]**，指定由自訂檔案提供者核發的API金鑰。

   [!DNL Workfront] 會使用此API金鑰，對檔案提供者進行授權API呼叫。

1. 按一下 **[!UICONTROL 儲存]** 來建立整合。

## 使用檔案整合

如需使用者如何使用的資訊 [!DNL Workfront DAM]，請參閱 [使用管理文檔 [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

如需使用者如何使用校對的詳細資訊，請參閱 [建立校樣](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs--in-wf.md).

如需在您設定後，使用者如何使用協力廠商檔案整合的詳細資訊，請參閱 [從外部應用程式連結文檔](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### 設定 [!DNL Workfront] 將元資料發送到 [!UICONTROL [!DNL Workfront] DAM] {#configure-workfront-to-send-metadata-to-workfront-dam}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **) </p>
-->

從 [!DNL Workfront] to [!DNL Workfront DAM]，您也可以傳送與該檔案相關的資訊。 有關文檔的資訊將映射到 [!DNL Workfront DAM] 作為中繼資料。

資訊僅以單向方式映射，從 [!DNL Workfront] to [!DNL Workfront DAM] 而且只有在將文檔上載到 [!DNL Workfront DAM]. Workfront欄位中未來的任何變更都不會更新中繼資料欄位 [!DNL Workfront DAM] 在文檔已上載後。\
您可以對應相同的 [!DNL Workfront] 欄位 [!DNL Workfront DAM] 欄位，但您無法使用相同 [!DNL Workfront DAM] 多個欄位 [!DNL Workfront] 欄位。

如果您必須設定多個 [!DNL Workfront] 要導出為一個欄位 [!DNL Workfront DAM] 欄位，首先在中建立計算的自訂欄位 [!DNL Workfront] 以顯示物件的所有個別自訂欄位。 然後，映射計算 [!DNL Workfront] 欄位至 [!DNL Workfront DAM] 欄位。\
如需計算自訂欄位的詳細資訊，請參閱 [將計算資料新增至自訂表單](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

映射會影響任何用戶從 [!DNL Workfront] to [!UICONTROL Workfront] DAM。

As a [!DNL Workfront] 管理員，您必須啟用 [!DNL Workfront DAM] 在Workfront中，您才能對應中繼資料對應程式的欄位。 如需如何啟用的詳細資訊 [!DNL Workfront DAM]，請參閱 [設定Workfront以將中繼資料傳送至 [!DNL Workfront DAM]](#configure-workfront-to-send-metadata-to-workfront-dam).

配置 [!DNL Workfront] 將元資料發送到 [!DNL Workfront DAM]:

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 按一下 **[!UICONTROL 檔案]** > **[!UICONTROL 中繼資料對應]**.

1. 在 **[!UICONTROL 選擇要映射的源欄位]** 欄位，開始輸入您要對應的Workfront欄位名稱 [!DNL Workfront DAM]，然後在清單中看到它時選取它。
1. 在 **[!UICONTROL 選擇映射的目標欄位]**，請選取 [!DNL Workfront DAM] 填入所選 [!DNL Workfront] 欄位。

   >[!NOTE]
   >
   > 所有發送到的文檔 [!DNL Workfront DAM] 擁有此權限的使用者，會以 [!DNL Workfront] 此處映射的欄位，當它們上載到 [!DNL Workfront DAM].

1. 按一下 **[!UICONTROL 新增對應]**.

1. 繼續添加更多內容 [!UICONTROL Workfront] 欄位和對應 [!DNL Workfront DAM] 欄位。

### 刪除映射的欄位

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 展開 **[!UICONTROL 檔案]**，然後按一下 **[!UICONTROL 中繼資料對應]**.

1. 在欄位清單中，選取您要從中繼資料對應中移除的任何欄位。
1. 按一下 **[!UICONTROL 刪除]**.

   欄位會從中繼資料對應中移除，其中包含的資訊不會傳輸至 [!DNL Workfront DAM] 上傳的檔案。
