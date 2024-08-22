---
title: 使用 [!DNL Adobe Experience Manager] 舊版聯結器設定 [!DNL Workfront]
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: 作為 [!DNL Adobe Workfront] 管理員，您可以整合 [!DNL Workfront] 與Adobe Experience Manager (AEM) Assets，並為您的組織提供全方位的內容管理解決方案，以建立、共用及維護工作流程中的資產。
author: Courtney
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 024b8606-a9b7-413a-b393-8e5cdff37dd4
source-git-commit: 55c8a3e5d0041a0e975bfd979a2d2e38930fea8d
workflow-type: tm+mt
source-wordcount: '1875'
ht-degree: 0%

---

# 使用[!DNL Adobe Experience Manager]舊版聯結器設定[!DNL Workfront]

作為[!DNL Adobe Workfront]管理員，您可以整合[!DNL Workfront]與[!UICONTROL Adobe Experience Manager (AEM) Assets]，並為您的組織提供完整的內容管理解決方案，以建立、共用及維護工作流程中的資產。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td>[！UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>您必須是[!DNL Workfront]管理員。 如需[!DNL Workfront]管理員的相關資訊，請參閱<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整管理存取權</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

+++

## [!DNL Workfront for AEM Assets]

[!DNL Workfront for AEM Assets connector]可讓您的組織執行下列動作：

* 在[!DNL Workfront]中將AEM資產和資料夾連結至專案、工作、問題和請求，以進行共同作業和管理創意內容。

  如需有關設定檔案與協力廠商應用程式整合的詳細資訊，請參閱[設定檔案整合](../../administration-and-setup/configure-integrations/configure-document-integrations.md)。

* 與[!DNL AEM Digital Asset Managemen]t (DAM)存放庫整合，可讓您使用[!DNL Workfront]管理和共用儲存在DAM中的數位資產。

  如需連結檔案和資產資料夾的詳細資訊，請參閱   [從外部應用程式連結檔案](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)。

* 將來自兩個應用程式的中繼資料合併並套用至資產。
* 檢視資產的包含所有內容通訊資料流。 在[!DNL Workfront]或[!UICONTROL AEM Assets]中對資產所做的更新和註解會同步處理至其他應用程式，以建立對資產進行通訊的完整歷史記錄。

  如需在[!DNL Workfront]中發表評論的詳細資訊，請參閱[將更新新增至檔案](../../documents/managing-documents/add-update-documents.md)。

## 安裝[!DNL AEM Assets]聯結器的先決條件

在安裝[!UICONTROL AEM Assets]的[!DNL Workfront]聯結器之前，請確定您符合下列必要條件：

* [!UICONTROL 已安裝並設定AEM Assets] 6.5版或更新版本。 如需有關安裝[!UICONTROL AEM Assets]的資訊，請參閱[[!DNL Adobe Experience Manager] 檔案](https://experienceleague.adobe.com/docs/experience-manager.html)。
* （視條件而定）如果防火牆規則未如預期允許流量，請將叢集的IP位址和/或網域新增至允許清單。 如需詳細資訊，請參閱[設定防火牆的允許清單](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)。

## 安裝[!DNL Workfront for AEM Assets]聯結器封裝 {#install-the-workfront-for-aem-assets-connector-package}

>[!IMPORTANT]
>
>下列指示適用於[!DNL Workfront with AEM Assets]舊版聯結器，此聯結器已由[[!DNL Workfront for Experience Manager] 增強型聯結器](../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/workfront-for-aem-enhanced-connector.md)取代。 如需詳細資訊，請聯絡您的客戶代表。

若要安裝[!DNL Workfront for AEM Assets]聯結器，您必須使用[!UICONTROL CRX封裝管理員]，將聯結器匯入AEM做為封裝。

1. 在已安裝AEM的工作站上，下載[!DNL Workfront for AEM Assets]聯結器安裝檔案。

   您可以從您的[!DNL Workfront]代表取得[!DNL Workfront for AEM Assets]聯結器。

1. 使用管理員帳戶登入AEM。
1. 按一下「**[!UICONTROL 工具]**」>「**[!UICONTROL 部署]**」>「**[!UICONTROL 封裝]**」。

   [!UICONTROL CRX封裝管理員]開啟。

1. 按一下&#x200B;**[!UICONTROL 上傳封裝]。**

1. 在[!UICONTROL 上傳封裝]對話方塊中，瀏覽並選取[!UICONTROL Workfront聯結器]封裝，然後按一下&#x200B;**[!UICONTROL 確定]**。\
   封裝會顯示在[!UICONTROL CRX封裝管理員]中。

1. 按一下&#x200B;**[!UICONTROL 安裝].**

1. 在[!UICONTROL 封裝]對話方塊中，忽略進階設定，然後按一下&#x200B;**[!UICONTROL 安裝]**。
1. （選擇性）若要確認聯結器已成功安裝，請確定[!UICONTROL 活動記錄]中顯示下列陳述式：

   ```
   Package installed in <time>
   ```

1. 關閉[!UICONTROL CRX封裝管理員]。

   聯結器已安裝，您現在可以設定[!DNL AEM Assets]與[!DNL Workfront]整合。

1. 繼續進行[設定 [!DNL AEM Assets] 以與 [!DNL Workfront]](#configure-aem-assets-to-integrate-with-workfront)整合。

## 設定[!DNL AEM Assets]以與[!DNL Workfront]整合 {#configure-aem-assets-to-integrate-with-workfront}

安裝聯結器後，請將聯結器封裝匯入至AEM並設定AEM與[!DNL Workfront]中的檔案連結。

如需有關安裝聯結器的資訊，請參閱[安裝 [!DNL Workfront for AEM Assets] 聯結器封裝](#install-the-workfront-for-aem-assets-connector-package)。

* [先決條件](#prerequisites)
* [將AEM與 [!DNL Workfront]整合](#integrate-aem-with-workfront)
* [設定[!UICONTROL AEM外部化程式]](#configure-the-aem-externalizer)

### 先決條件 {#prerequisites}

開始之前，您必須啟用Workfront服務的許可權：

1. 在AEM中，移至&#x200B;**[!UICONTROL 工具]**> **[!UICONTROL 安全性]**> **[!UICONTROL 許可權]**。
1. 在左上角，在下拉式選單中選擇&#x200B;**[!UICONTROL 使用者]**&#x200B;，並在&#x200B;**[!UICONTROL 搜尋]**&#x200B;欄位中輸入&#x200B;*[!UICONTROL workfront-service]*&#x200B;。 選取[!UICONTROL workfront-service]使用者。
1. 在熒幕右側，選取&#x200B;**[!UICONTROL 新增ACE]**&#x200B;以建立新專案。
1. 在{&#x200B;0}新增專案&#x200B;]**視窗&#x200B;中，選取**[!UICONTROL &#x200B;路徑&#x200B;]**欄&#x200B;位中的核取方塊圖示，然後選擇資料夾： */conf***[!UICONTROL 
1. 在[許可權]欄位中輸入： *jcr：read*
1. 選取右上角的&#x200B;**[!UICONTROL 新增]**&#x200B;
1. （選用）重複步驟以建立更多專案。

### 將AEM與[!DNL Workfront]整合 {#integrate-aem-with-workfront}

1. 以管理員身分登入AEM Assets。
1. 按一下&#x200B;**[!UICONTROL 工具]** >**[!UICONTROL Cloud Service]**>**[!UICONTROL Workfront整合組態]** >**[!UICONTROL 全域Workfront]。**&#x200B;**{&#x200B;10}**

1. （視條件而定）如果您尚未這樣做，請建立[!DNL Workfront]雲端設定檔。

   1. 按一下[!DNL Global-Workfront]頁面右上角的&#x200B;**[!UICONTROL 建立]**。
   1. 在&#x200B;**[!UICONTROL Workfront URL]**&#x200B;方塊中，指定您[!DNL Workfront]執行個體的URL。

      例如，[!DNL https]：//`<account>`.my.workfront.com，其中`<account>`是您用來與AEM整合的帳戶。

   1. 在{&#x200B;0}基本資料夾&#x200B;]**欄位中，選取核取方塊圖示，然後在下拉式功能表中選取連結至[!DNL Workfront]物件的檔案儲存路徑。**[!UICONTROL 
   1. 在出現的AEM強制回應視窗中，將連結至[!DNL Workfront]物件的檔案置於資料夾的路徑之後。 選擇資料夾，然後按右上角的&#x200B;**[!UICONTROL &#x200B;選取]**。

      您可以連結至根/content/dam/下的任何資料夾。

   1. 在&#x200B;**[!UICONTROL Workfront API金鑰]**&#x200B;方塊中，指定您的[!UICONTROL Workfront] API金鑰。

      若要擷取您的[!DNL Workfront] API金鑰：

      1. 開啟瀏覽器索引標籤，並以[!DNL Workfront]管理員身分登入您的[!DNL Workfront]帳戶。

      {{step-1-to-setup}}

      1. 按一下&#x200B;**[!UICONTROL 系統]** >**[!UICONTROL 客戶資訊]**。

         如果您已產生API金鑰，您的[!DNL Workfront] API金鑰會顯示在使用者的API金鑰標籤下方。

      1. （視條件而定）如果您尚未產生API金鑰，則需要產生金鑰：

         1. 在&#x200B;**[!UICONTROL API金鑰設定]**&#x200B;區段中，確定&#x200B;**[!UICONTROL 建立後，API金鑰於]**&#x200B;內到期選項設定為「無」。

            如果您選取有效期間，聯結器將在API金鑰過期後停止運作。 然後，您需要重新產生API金鑰並更新您的[!DNL Workfront]設定。

         1. 在&#x200B;**[!UICONTROL 您使用者的API金鑰]**&#x200B;標籤下，按一下&#x200B;**[!UICONTROL 產生API金鑰]**。

            [!DNL Workfront]的API金鑰會產生並顯示。
      1. 將API金鑰複製到剪貼簿。
      1. 開啟AEM Connector的瀏覽器標籤，並在&#x200B;**[!DNL Workfront API Key]**&#x200B;方塊中貼上您複製的API金鑰。
   1. （視條件而定）按一下「[!UICONTROL [!DNL Workfront]整合組態]」頁面左上角的「**[!UICONTROL 進階]**」標籤，並選取下列適用的選項：

      **[!UICONTROL 允許集合瀏覽]：**&#x200B;如果您的組織允許[!DNL Workfront]位使用者將AEM Assets集合連結至[!DNL Workfront]物件，請選取此選項。

      **[!UICONTROL 使用者Federated ID]：**&#x200B;如果您的組織在登入Workfront時使用Federated ID或單一登入(SSO)，請選取此選項。

      **[!UICONTROL 忽略電子郵件網域]：**&#x200B;如果您的AEM使用者未在其使用者ID中使用網域名稱，請選取此選項。

      **[!UICONTROL 限制存取]：**&#x200B;選取此選項以指定需要新增至允許清單的適當[!DNL Workfront] IP位址。 如需允許清單的詳細資訊，請參閱[設定防火牆的允許清單](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)。

   1. 按一下「Workfront整合設定」頁面左上角的「**[!UICONTROL 基本]**」標籤，然後按一下「**[!UICONTROL 連線]**」。

      >[!NOTE]
      >
      >套用變更可能需要一些時間。 重新啟動該套件組合可能會加快處理速度。



1. （視條件而定）如果您已建立[!DNL Workfront]雲端設定檔，請選取&#x200B;**[!UICONTROL 全域 —[!DNL Workfront]]**，然後在左上角按一下&#x200B;**[!UICONTROL 屬性]**。

1. 按一下&#x200B;**[!UICONTROL 產生金鑰]，**&#x200B;產生AEM API金鑰，然後將AEM API金鑰複製到剪貼簿。

   稍後當您設定[!UICONTROL Workfront]與[!UICONTROL AEM Assets]整合時，將需要AEM API金鑰。 如需詳細資訊，請參閱[設定Workfront以與AEM資產整合](#configure-workfront-to-integrate-with-aem-assets)。

1. 按一下右上角的&#x200B;**[!UICONTROL 儲存]**。

   顯示[!UICONTROL 全域 — [!DNL Workfront]]視窗。

   ![屬性.png](assets/properties-350x117.png)

1. （選用）同步處理AEM與[!DNL Workfront]之間的雙向通訊。

   1. 按一下&#x200B;**[!UICONTROL 全域 — [!DNL Workfront]].**
   1. 在視窗的左上角，按一下&#x200B;**[!UICONTROL 屬性]**。

      顯示[!UICONTROL [!DNL Workfront]整合組態]頁面。

      ![屬性2.png](assets/properties2-350x444.png)

   1. （選擇性）若要在[!UICONTROL AEM Assets]和[!DNL Workfront]之間啟用評論同步處理，請按一下&#x200B;**[!UICONTROL 啟用評論同步處理]**。

      >[!IMPORTANT]
      >
      >您必須啟用[!UICONTROL Document Sync]才能同步資產。

   1. （選擇性）若要關閉評論同步處理，請按一下&#x200B;**[!UICONTROL 停用評論同步處理]。**

      或

      刪除在您的AEM執行個體上註冊的[!UICONTROL NOTE CREATE]事件訂閱。

      如需有關活動訂閱的資訊，請參閱[活動訂閱API](../../wf-api/general/event-subs-api.md)。

1. 繼續[設定[!UICONTROL AEM Externalizer]](#configure-the-aem-externalizer)。

### 設定[!UICONTROL AEM外部化程式] {#configure-the-aem-externalizer}

[!UICONTROL AEM Externalizer]允許AEM以可用於[!DNL Workfront]的格式傳遞URL。 如果未正確設定，[!DNL Workfront]將無法呼叫AEM API，而且在Workfront中連結AEM檔案的URL將無法運作。

1. 在AEM中，按一下&#x200B;**[!UICONTROL 工具]** > **[!UICONTROL 作業]** >**[!UICONTROL 網頁主控台]**。

1. 按一下&#x200B;**[!UICONTROL OSGI]**，然後在下拉式功能表中按一下&#x200B;**[!UICONTROL 組態]**。

1. 在設定清單中，選取&#x200B;**[!UICONTROL &#x200B;Day CQ Link Externalizer].**

   顯示[!UICONTROL Externalizer]頁面。

1. 在&#x200B;**[!UICONTROL 網域]**&#x200B;區段中，確認[!UICONTROL 作者]欄位中所列的網域是AEM使用者可從外部存取的網域名稱。

   [!UICONTROL 作者]欄位中的網域名稱應該符合AEM執行個體的URL行中所列的網域。

   ![[!DNL Extenalizer].png](assets/extenalizer-350x128.png)

1. （條件式）如有必要，請更新[!UICONTROL 作者]欄位中的網域。
1. 按一下「**[!UICONTROL 儲存]**」。

   [!UICONTROL AEM Assets]現已設定為連結檔案與[!DNL Workfront]

1. 繼續進行[設定 [!DNL Workfront] 以與 [!DNL AEM assets]](#configure-workfront-to-integrate-with-aem-assets)整合。

## 設定[!DNL Workfront]以與[!DNL AEM assets]整合 {#configure-workfront-to-integrate-with-aem-assets}

安裝[!UICONTROL Workfront for AEM Assets]聯結器後(如[安裝[!UICONTROL Workfront for AEM Assets]聯結器套件](#install-the-workfront-for-aem-assets-connector-package)中所述)，並設定[!UICONTROL AEM Assets] (如[設定[!UICONTROL  AEM Assets]以與 [!DNL Workfront]](#configure-aem-assets-to-integrate-with-workfront)整合)後，您需要設定[!DNL Workfront]以連結介於[!DNL Workfront]和[!DNL AEM Assets]之間的檔案。

1. 以[!UICONTROL Workfront]管理員身分登入[!DNL Workfront]。

   >[!TIP]
   >
   >[!UICONTROL Workfront]建議建立專屬於您AEM整合的[!UICONTROL Workfront]管理員。 如需將[!UICONTROL Workfront]管理員存取層級指派給使用者的詳細資訊，請參閱[授予使用者對特定區域的管理存取權](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)。

{{step-1-to-setup}}

1. 按一下&#x200B;**[!UICONTROL 檔案]**> **[!UICONTROL 自訂整合]。**

1. 按一下&#x200B;**[!UICONTROL 新增自訂整合]**。
1. 在&#x200B;**[!UICONTROL 名稱]**&#x200B;方塊中，指定自訂整合的名稱。

   這是使用者在[!UICONTROL Workfront]內使用整合時看到的名稱；例如，您可以為名稱輸入&#x200B;*&quot;[!DNL AEM Assets]&quot;*。

1. 在&#x200B;**[!UICONTROL 基本API URL]**&#x200B;方塊中，指定您AEM執行個體的URL。

   基本API URL包含您的AEM執行個體的URL，後面跟有路徑：/bin/webhooks/api/

   ![mceclip3.png](assets/mceclip3-350x130.png)

1. 在&#x200B;**[!UICONTROL 驗證型別]**&#x200B;下拉式功能表中，選取&#x200B;**[!UICONTROL ApiKey].**

1. 在{&#x200B;0}API金鑰&#x200B;]**方塊中，貼上您設定[!UICONTROL AEM Assets]時複製的AEM API金鑰。**[!UICONTROL 
1. 按一下「**[!UICONTROL 儲存]**」。
1. （選擇性）確定整合已標籤為[!UICONTROL 使用中]。\
   ![aem_custom_integration_active.png](assets/aem-custom-integration-active-350x81.png)

   [!DNL Workfront]現在已設定為搭配[!DNL AEM Assets]使用。

   為了存取AEM中的資產，必須將需要使用聯結器的每個[!DNL Workfront]使用者設定為AEM中的使用者。 如需建立使用者的詳細資訊，請參閱[設定使用者以使用聯結器](#set-up-users-to-use-the-connector)。

## 設定使用聯結器的使用者 {#set-up-users-to-use-the-connector}

使用者若要存取聯結器，必須在AEM中擁有使用者設定檔，且必須屬於[!DNL Workfront]群組，該群組的存取層級包含[!UICONTROL 建立]和[!UICONTROL 刪除]許可權。

如需[!DNL Workfront]許可權的詳細資訊，請參閱[建立或修改自訂存取層級](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

* [在 [!DNL AEM assets]中設定使用者](#set-up-users-in-aem-assets)

### 在[!DNL AEM assets]中設定使用者 {#set-up-users-in-aem-assets}

1. 以[!DNL Workfront]管理員身分登入[!DNL AEM Assets]。
1. 按一下&#x200B;**[!UICONTROL 工具]** >**{&#x200B;3}{&#x200B;4}安全性]** >**[!UICONTROL 使用者]**。****[!UICONTROL 

1. （視條件而定）如果使用者在AEM中沒有使用者設定檔，請建立AEM使用者設定檔。

   1. 按一下&#x200B;**[!UICONTROL 建立使用者].**
   1. 輸入使用者的個人資訊。

      ![64NewUser.png](assets/64newuser-350x524.png)

      唯一的必填欄位是ID欄位。 使用者的AEM ID必須符合其[!DNL Workfront] ID，也就是使用者的[!DNL Workfront]電子郵件地址。

      如果您在設定AEM與[!DNL Workfront]整合時選取[!UICONTROL 忽略電子郵件網域]選項，則AEM ID將不會符合[!DNL Workfront]電子郵件地址。

1. （視條件而定）如果使用者有AEM設定檔，請開啟使用者的AEM設定檔。

   1. 按一下&#x200B;**[!UICONTROL 使用者].**

      顯示[!UICONTROL 使用者管理]頁面。

   1. 按一下您要新增的使用者，然後按一下&#x200B;**[!UICONTROL 內容]**。

      使用者的設定頁面隨即顯示。

1. 按一下「**[!UICONTROL 群組]**」標籤。

   ![](assets/groupstab.png)

1. 確定使用者至少屬於一個存取層級包含[!UICONTROL 建立]和[!UICONTROL 刪除]許可權的[!DNL Workfront]群組。

   1. 若要將使用者新增至現有群組，請在&#x200B;**[!UICONTROL 輸入群組名稱]**&#x200B;方塊中開始輸入群組名稱，然後在群組出現在下拉式功能表中時選取該群組。

      或

      若要選取使用者為其成員的群組，請在&#x200B;**[!UICONTROL 群組中，選取此使用者為]**&#x200B;區段成員的群組。

1. 按一下&#x200B;**[!UICONTROL 儲存]。**
