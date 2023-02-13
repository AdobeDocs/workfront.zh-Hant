---
title: 設定 [!DNL Workfront] with [!DNL Adobe Experience Manager] 舊連接器
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: 作為 [!DNL Adobe Workfront] 管理員，您可以整合 [!DNL Workfront] Adobe Experience Manager(AEM)資產，為貴組織提供全方位的內容管理解決方案，以便在工作流程中建立、共用及維護資產。
author: Courtney
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 024b8606-a9b7-413a-b393-8e5cdff37dd4
source-git-commit: 2f840ea68c9efb78acb4c24346c6775671ed0334
workflow-type: tm+mt
source-wordcount: '1893'
ht-degree: 0%

---

# 設定 [!DNL Workfront] with [!DNL Adobe Experience Manager] 舊連接器

作為 [!DNL Adobe Workfront] 管理員，您可以整合 [!DNL Workfront] with [!UICONTROL Adobe Experience Manager(AEM)資產] 並為您的組織提供全面的內容管理解決方案，以便在工作流程中建立、共用和維護資產。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td>[!UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>您必須是 [!DNL Workfront] 管理員。 如需 [!DNL Workfront] 管理員請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## [!DNL Workfront for AEM Assets]

此 [!DNL Workfront for AEM Assets connector] 可讓您的組織執行下列作業：

* 將AEM資產和資料夾連結至中的專案、工作、問題和請求，以共同作業及管理創意內容 [!DNL Workfront].

   如需與協力廠商應用程式整合設定檔案的詳細資訊，請參閱  [配置文檔整合](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

* 與整合 [!DNL AEM Digital Asset Managemen]t(DAM)存放庫，可讓您使用 [!DNL Workfront] 管理和共用儲存在DAM中的數位資產。

   如需連結檔案和資產資料夾的詳細資訊，請參閱   [從外部應用程式連結文檔](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

* 合併兩個應用程式的中繼資料，並套用至資產。
* 檢視資產的全包通訊資料流。 對資產所做的更新和註解，位於 [!DNL Workfront] 或 [!UICONTROL AEM Assets] 會與其他應用程式同步，以建立與資產所進行通訊的完整記錄。

   如需在 [!DNL Workfront]，請參閱 [向文檔添加更新](../../documents/managing-documents/add-update-documents.md).

## 安裝的必要條件 [!DNL AEM Assets] 連接器

安裝之前 [!DNL Workfront] 連接器 [!UICONTROL AEM Assets]，請確定已符合下列必要條件：

* [!UICONTROL AEM Assets] 已安裝並設定6.5版或更新版本。 有關安裝的資訊 [!UICONTROL AEM Assets]，請參閱 [[!DNL Adobe Experience Manager] 檔案](https://experienceleague.adobe.com/docs/experience-manager.html).
* （條件性）如果防火牆規則未如預期允許流量，請將叢集的IP位址和/或網域新增至允許清單。 如需詳細資訊，請參閱 [配置防火牆的允許清單](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## 安裝 [!DNL Workfront for AEM Assets] 連接器封裝 {#install-the-workfront-for-aem-assets-connector-package}

>[!IMPORTANT]
>
>下列指示適用於 [!DNL Workfront with AEM Assets] 舊連接器，已由 [[!DNL Workfront for Experience Manager] 增強型連接器](../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/workfront-for-aem-enhanced-connector.md). 如需詳細資訊，請連絡您的客戶代表。

若要安裝 [!DNL Workfront for AEM Assets] 連接器，您必須使用 [!UICONTROL CRX封裝管理器].

1. 在您已安裝AEM的工作站上，下載 [!DNL Workfront for AEM Assets] 連接器安裝檔案。

   您可以取得 [!DNL Workfront for AEM Assets] 連接器 [!DNL Workfront] 代表。

1. 使用管理員帳戶登入AEM。
1. 按一下 **[!UICONTROL 工具]** > **[!UICONTROL 部署]** > **[!UICONTROL 套件]**.

   此 [!UICONTROL CRX封裝管理器] 開啟。

1. 按一下 **[!UICONTROL 上傳套件].**

1. 在 [!UICONTROL 上傳套件] 對話框，瀏覽並選擇 [!UICONTROL Workfront Connector] 封裝，然後按一下 **[!UICONTROL 確定]**.\
   套件會顯示在 [!UICONTROL CRX封裝管理器].

1. 按一下 **[!UICONTROL 安裝].**

1. 在 [!UICONTROL 套件] 對話框，忽略高級設定，然後按一下 **[!UICONTROL 安裝]**.
1. （可選）若要確認連接器已成功安裝，請確定下列陳述式顯示在 [!UICONTROL 活動記錄]:

   ```
   Package installed in <time>
   ```

1. 關閉 [!UICONTROL CRX封裝管理器].

   連接器已安裝，您現在可以設定 [!DNL AEM Assets] 整合 [!DNL Workfront].

1. 繼續 [設定 [!DNL AEM Assets] 整合 [!DNL Workfront]](#configure-aem-assets-to-integrate-with-workfront).

## 設定 [!DNL AEM Assets] 整合 [!DNL Workfront] {#configure-aem-assets-to-integrate-with-workfront}

安裝連接器後，請將連接器封裝匯入至AEM，並設定AEM以與中的檔案連結 [!DNL Workfront].

有關安裝連接器的資訊，請參閱  [安裝 [!DNL Workfront for AEM Assets] 連接器封裝](#install-the-workfront-for-aem-assets-connector-package).

* [必要條件](#prerequisites)
* [將AEM與 [!DNL Workfront]](#integrate-aem-with-workfront)
* [設定 [!UICONTROL AEM Externalizer]](#configure-the-aem-externalizer)

### 必要條件 {#prerequisites}

開始之前，必須為workfront-service啟用權限：

1. 在AEM中，前往 **[!UICONTROL 工具]**> **[!UICONTROL 安全性]**> **[!UICONTROL 權限]**.
1. 在左上角，選擇 **[!UICONTROL 使用者]**&#x200B;，然後輸入 *[!UICONTROL 工作前服務]* 在 **[!UICONTROL 搜尋]**&#x200B;欄位。 選取 [!UICONTROL 工作前服務] 使用者。
1. 在畫面的右側，選取 **[!UICONTROL 添加ACE]** 建立新條目。
1. 在&#x200B;**[!UICONTROL 新增參加項目]**&#x200B;，請選取 **[!UICONTROL 路徑]**&#x200B;欄位，然後選擇資料夾： */conf*
1. 在權限欄位中輸入： *jcr:read*
1. 選擇 **[!UICONTROL 新增]**&#x200B;右上角
1. （選用）重複步驟以建立更多項目。

### 將AEM與 [!DNL Workfront] {#integrate-aem-with-workfront}

1. 以管理員身分登入AEM Assets。
1. 按一下 **[!UICONTROL 工具]** >**[!UICONTROL Cloud Services]**>**[!UICONTROL Workfront整合設定]** >**[!UICONTROL 全球 — Workfront].**&#x200B;**&#x200B;**

1. （條件性）如果您尚未這麼做，請建立 [!DNL Workfront] 雲端設定檔案。

   1. 按一下  **[!UICONTROL 建立]** 在 [!DNL Global-Workfront] 頁面。
   1. 在 **[!UICONTROL Workfront URL]** 框中，指定 [!DNL Workfront] 例項。

      例如， [!DNL https]://`<account>`.my.workfront.com，其中 `<account>` 是您用於與AEM整合的帳戶。

   1. 在&#x200B;**[!UICONTROL 基本資料夾]** 欄位中，選取核取方塊圖示，然後在下拉式選單中選取連結至檔案的路徑 [!DNL Workfront] 對象被儲存。
   1. 在顯示的AEM強制回應視窗中，使用連線至的檔案，依照資料夾的路徑進行 [!DNL Workfront] 對象。 選擇資料夾並按 **[!UICONTROL 選擇]**&#x200B;在右上角。

      您可以連結至根/content/dam/底下的任何資料夾。

   1. 在 **[!UICONTROL Workfront API密鑰]** 框，指定 [!UICONTROL Workfront] API金鑰。

      若要擷取 [!DNL Workfront] API密鑰：

      1. 開啟瀏覽器標籤，然後登入您的 [!DNL Workfront] 帳戶作為 [!DNL Workfront] 管理員。
      1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

      1. 按一下 **[!UICONTROL 系統]** >**[!UICONTROL 客戶資訊]**.

         如果您已產生API金鑰，則您的 [!DNL Workfront] API金鑰會顯示在您使用者的API金鑰標籤下。

      1. （視條件而定）如果您尚未產生API金鑰，則需要產生一個：

         1. 在 **[!UICONTROL API金鑰設定]** 一節，請確定 **[!UICONTROL 建立後，API金鑰的過期時間為]** 選項設定為「無」。

            如果您選取過期時間，API金鑰過期後，連接器就會停止運作。 之後，您需要重新產生API金鑰並更新您的 [!DNL Workfront] 設定。

         1. 在 **[!UICONTROL 您的使用者API金鑰]** 標籤，按一下 **[!UICONTROL 產生API金鑰]**.

            適用於 [!DNL Workfront] 產生並顯示。
      1. 將API金鑰複製到剪貼簿。
      1. 開啟AEM Connector的瀏覽器標籤，並在 **[!DNL Workfront API Key]** 框中，貼上您複製的API密鑰。
   1. （條件性）按一下 **[!UICONTROL 進階]** 標籤 [!UICONTROL [!DNL Workfront] 整合設定] ，並選取下列選項（如果適用）:

      **[!UICONTROL 允許集合瀏覽]:**&#x200B;如果貴組織允許，請選取此選項 [!DNL Workfront] 將AEM Assets集合連結至 [!DNL Workfront] 對象。

      **[!UICONTROL 使用者Federated ID]:** 如果貴組織在登入Workfront時使用Federated ID或單一登入(SSO)，請選取此選項。

      **[!UICONTROL 忽略電子郵件域]:** 如果您的AEM使用者的使用者ID中未使用網域名稱，請選取此選項。

      **[!UICONTROL 限制存取]:** 選取此選項以指定適當的 [!DNL Workfront] 需要新增至允許清單的IP位址。 如需允許清單的詳細資訊，請參閱 [配置防火牆的允許清單](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

   1. 按一下 **[!UICONTROL 基本]** 標籤，然後按一下「 Workfront整合設定」頁面的左上角 **[!UICONTROL Connect]**.

      >[!NOTE]
      >
      >變更可能需要一些時間才能套用。 重新啟動套件組合可能會加速程式。



1. （條件性）如果您已建立 [!DNL Workfront] 雲配置檔案，選擇 **[!UICONTROL 全球 —[!DNL Workfront]]**，然後在左上角按一下 **[!UICONTROL 屬性]**.

1. 按一下「 」，產生AEM API金鑰 **[!UICONTROL 產生金鑰],** 然後將AEM API金鑰複製到剪貼簿。

   您稍後進行設定時將需要AEM API金鑰 [!UICONTROL Workfront] 整合 [!UICONTROL AEM Assets]. 如需詳細資訊，請參閱 [設定Workfront以與AEM資產整合](#configure-workfront-to-integrate-with-aem-assets).

1. 在右上角，按一下 **[!UICONTROL 儲存]**.

   此 [!UICONTROL 全球 — [!DNL Workfront]] 視窗。

   ![屬性.png](assets/properties-350x117.png)

1. （選用）同步AEM與 [!DNL Workfront].

   1. 按一下 **[!UICONTROL 全球 — [!DNL Workfront]].**
   1. 在視窗的左上角，按一下 **[!UICONTROL 屬性]**.

      此 [!UICONTROL [!DNL Workfront] 整合設定] 頁面。

      ![屬性2.png](assets/properties2-350x444.png)

   1. （可選）啟用同步注釋之間 [!UICONTROL AEM Assets] 和 [!DNL Workfront]，按一下 **[!UICONTROL 啟用注釋同步]**.

      >[!IMPORTANT]
      >
      >您必須啟用 [!UICONTROL 文檔同步] 同步資產。

   1. （可選）要關閉注釋同步，請按一下 **[!UICONTROL 禁用注釋同步].**

      或

      刪除 [!UICONTROL 附註建立] 已註冊至AEM例項的事件訂閱。

      如需事件訂閱的詳細資訊，請參閱 [事件訂閱API](../../wf-api/general/event-subs-api.md).

1. 繼續 [設定 [!UICONTROL AEM Externalizer]](#configure-the-aem-externalizer).

### 設定 [!UICONTROL AEM Externalizer] {#configure-the-aem-externalizer}

此 [!UICONTROL AEM Externalizer] 可讓AEM以可用於 [!DNL Workfront]. 如果未正確配置， [!DNL Workfront] 無法呼叫AEM API，且連結Workfront中AEM檔案的URL將無法運作。

1. 在AEM中，按一下 **[!UICONTROL 工具]** > **[!UICONTROL 操作]** >**[!UICONTROL Web主控台]**.

1. 按一下 **[!UICONTROL OSGI]**，然後按一下 **[!UICONTROL 設定]** 的下拉式清單。

1. 在設定清單中，選&#x200B;取&#x200B;**[!UICONTROL Day CQ Link Externalizer].**

   此 [!UICONTROL 外置器] 頁面。

1. 在 **[!UICONTROL 網域]** 一節，請確定 [!UICONTROL 作者] 欄位是AEM使用者可從外部存取的網域名稱。

   中的網域名稱 [!UICONTROL 作者] 欄位應符合AEM例項URL行中列出的網域。

   ![[!DNL Extenalizer].png](assets/extenalizer-350x128.png)

1. （條件性）如有需要，請更新 [!UICONTROL 作者] 欄位。
1. 按一下&#x200B;**[!UICONTROL 儲存]**。

   [!UICONTROL AEM Assets] 現在已設定為將檔案連結至 [!DNL Workfront]

1. 繼續 [設定 [!DNL Workfront] 整合 [!DNL AEM assets]](#configure-workfront-to-integrate-with-aem-assets).

## 設定 [!DNL Workfront] 整合 [!DNL AEM assets] {#configure-workfront-to-integrate-with-aem-assets}

安裝 [!UICONTROL Workfront for AEM Assets] 連接器(如 [安裝 [!UICONTROL Workfront for AEM Assets] 連接器封裝](#install-the-workfront-for-aem-assets-connector-package))和 [!UICONTROL AEM Assets] (如 [設定[!UICONTROL  AEM Assets] 整合 [!DNL Workfront]](#configure-aem-assets-to-integrate-with-workfront))，您需要設定 [!DNL Workfront] 將文檔連結到 [!DNL Workfront] 和 [!DNL AEM Assets].

1. 登入 [!DNL Workfront] as a [!UICONTROL Workfront] 管理員。

   >[!TIP]
   >
   >[!UICONTROL Workfront] 建議建立 [!UICONTROL Workfront] 僅專用於您的AEM整合的管理員。 如需指派 [!UICONTROL Workfront] 管理員對用戶的訪問級別，請參閱 [授予用戶對特定區域的管理訪問權限](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 按一下 **[!UICONTROL 檔案]**> **[!UICONTROL 自訂整合].**

1. 按一下 **[!UICONTROL 新增自訂整合]**.
1. 在 **[!UICONTROL 名稱]** 方塊，指定自訂整合的名稱。

   這是使用者在中使用整合時看到的名稱 [!UICONTROL Workfront];例如，您可以在 *&quot;[!DNL AEM Assets]&quot;* 名稱。

1. 在 **[!UICONTROL 基本API URL]** 框中，指定AEM實例的URL。

   基礎API URL包含AEM例項的URL，及其後面的路徑：/bin/webhooks/api/

   ![mceclip3.png](assets/mceclip3-350x130.png)

1. 在 **[!UICONTROL 驗證類型]** 下拉式功能表，選取 **[!UICONTROL ApiKey].**

1. 在&#x200B;**[!UICONTROL API金鑰]** 方塊中，貼上您在設定時複製的AEM API金鑰 [!UICONTROL AEM Assets].
1. 按一下&#x200B;**[!UICONTROL 儲存]**。
1. （選用）確認已標示整合 [!UICONTROL 作用中].\
   ![aem_custom_integration_active.png](assets/aem-custom-integration-active-350x81.png)

   [!DNL Workfront] 現在已設定為可搭配使用 [!DNL AEM Assets].

   若要存取AEM中的資產，請 [!DNL Workfront] 需要使用連接器的使用者必須在AEM中設定為使用者。 如需建立使用者的詳細資訊，請參閱  [設定使用者以使用連接器](#set-up-users-to-use-the-connector).

## 設定使用者以使用連接器 {#set-up-users-to-use-the-connector}

使用者若要存取連接器，必須在AEM中擁有使用者設定檔，且屬於 [!DNL Workfront] 具有包含 [!UICONTROL 建立] 和 [!UICONTROL 刪除] 權限。

如需 [!DNL Workfront] 權限，請參閱 [建立或修改自訂存取層級](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* [在 [!DNL AEM assets]](#set-up-users-in-aem-assets)

### 在 [!DNL AEM assets] {#set-up-users-in-aem-assets}

1. 登入 [!DNL AEM Assets] as a [!DNL Workfront] 管理員。
1. 按一下 **[!UICONTROL 工具]** >**&#x200B;**&#x200B;**[!UICONTROL 安全性]** >**[!UICONTROL 使用者]**.

1. （條件性）如果使用者在AEM中沒有使用者設定檔，請建立AEM使用者設定檔。

   1. 按一下 **[!UICONTROL 建立使用者].**
   1. 輸入用戶的個人資訊。

      ![64NewUser.png](assets/64newuser-350x524.png)

      唯一的必填欄位是ID欄位。 使用者的AEM ID必須符合 [!DNL Workfront] ID，即使用者的 [!DNL Workfront] 電子郵件地址。

      如果您選取 [!UICONTROL 忽略電子郵件域] 選項(若您已設定AEM，則整合 [!DNL Workfront]，則AEM ID將不符合 [!DNL Workfront] 電子郵件地址。

1. （條件性）如果使用者有AEM設定檔，請開啟使用者的AEM設定檔。

   1. 按一&#x200B;下&#x200B;**[!UICONTROL 使用者].**

      此 [!UICONTROL 使用者管理] 頁面。

   1. 按一下您要新增的使用者，然後按一下 **[!UICONTROL 屬性]**.

      使用者的設定頁面隨即顯示。

1. 按一下 **[!UICONTROL 群組]** 標籤。

   ![](assets/groupstab.png)

1. 確保用戶至少屬於一個 [!DNL Workfront] 具有包含 [!UICONTROL 建立] 和 [!UICONTROL 刪除] 權限。

   1. 若要將使用者新增至現有群組，請開始在 **[!UICONTROL 類型組名稱]** 框中，然後選擇顯示在下拉菜單中的組。

      或

      要選擇用戶所屬的組，請在 **[!UICONTROL 此用戶所屬的組]** 區段。

1. 按一下&#x200B;**[!UICONTROL 儲存]。**
