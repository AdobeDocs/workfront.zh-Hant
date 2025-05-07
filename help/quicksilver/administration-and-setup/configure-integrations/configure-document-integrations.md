---
title: 設定檔案整合
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: 作為Adobe Workfront管理員，您可以設定檔案整合以管理Workfront中的檔案。
author: Courtney, Becky
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: cf5c4e3d-b45f-46cd-a938-22e412d1c491
source-git-commit: ec0e2be036ce1298e285ce85cdeddae97cd1f144
workflow-type: tm+mt
source-wordcount: '1199'
ht-degree: 1%

---

# 設定文件整合

<!-- Audited: 12/2023 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

作為[!DNL Adobe Workfront]管理員，您可以設定檔案整合以管理[!UICONTROL Workfront]中的檔案。 您也可以設定[!UICONTROL Workfront]，讓檔案只儲存在檔案服務應用程式中，而不儲存在[!UICONTROL Workfront]本身中。 如需詳細資訊，請參閱[從外部應用程式連結檔案](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)中的[更新檔案，並將檔案從[!UICONTROL Workfront]連結到外部雲端提供者](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#update-and-link-a-document-from-workfront-to-an-external-cloud-provider)。

>[!NOTE]
>
>若要允許[!DNL Workfront Proof]與[!DNL Workfront]伺服器之間的開啟通訊，您可能需要將某些IP位址新增至允許清單。 如需詳細資訊，請參閱[設定防火牆的允許清單](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具備下列專案才能執行本文所述的步驟：

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
   <td><p>新增：[！UICONTROL Standard]</p>
       <p>或</p>
       <p>目前： [！UICONTROL計畫]</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是[!DNL Workfront]管理員。</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 支援的整合

<!--DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

您可以設定下列整合來管理檔案：

<!--
  Experience Manager Assets Essentials </p>
  -->

* [!DNL Workfront DAM]

* [!DNL Workfront Proof]

  從[!DNL Workfront Proof]連結校訂可讓您讓原本在[!DNL Workfront Proof]內建立的校訂可在[!DNL Workfront]內使用。 對於目前的計畫，需要[!UICONTROL Pro] [!DNL Workfront]計畫或更新的計畫才能使用此功能。 對於新計畫，此功能可用於所有計畫。 如需各種可用計畫的詳細資訊，請參閱[Workfront計畫](https://business.adobe.com/products/workfront/pricing.html)。

* [!DNL Microsoft SharePoint]

  如需有關與[!DNL SharePoint]整合的資訊，請參閱[設定 [!DNL SharePoint] 整合](../../administration-and-setup/configure-integrations/configure-sharepoint-integration.md)。

* 協力廠商雲端檔案提供者：

   * [!DNL Box]
   * [!DNL Dropbox]
   * [!DNL Dropbox Business]
   * [!DNL WebDAM]
   * [!DNL Microsoft OneDrive]
   * [!DNL Microsoft SharePoint]
   * [!UICONTROL Google磁碟機]
   * Quip

  >[!TIP]
  >
  >您可以校訂和核准從外部雲端提供者連結的檔案，其方式與直接上傳至[!DNL Workfront]的檔案校訂和核准方式相同。

* 其他檔案提供者（透過自訂檔案整合）。

  對於目前的計畫，需要[!UICONTROL Pro] [!DNL Workfront]計畫或更新的計畫才能使用此功能。 對於新計畫，此功能可用於所有計畫。 如需各種可用計畫的詳細資訊，請參閱[Workfront計畫](https://business.adobe.com/products/workfront/pricing.html)。

此外，您還可以使用協力廠商DAM整合來增強您的[!DNL Workfront]檔案體驗。 管理員必須啟用這些功能，使用者才能將服務連結至其[!DNL Workfront]帳戶。

## 設定整合以管理檔案

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**[!UICONTROL 檔案]** > **[!UICONTROL 雲端提供者].**

1. （選擇性）若要將檔案儲存在檔案服務應用程式中，而不是儲存在[!DNL Workfront]中，請選取&#x200B;**[!UICONTROL 防止使用者將檔案儲存在[!DNL Workfront]]。**

1. 選取要啟用的整合。
1. 按一下「**[!UICONTROL 儲存]**」。

如果您正在設定與[!DNL Workfront DAM]的整合，您可以啟用[!DNL Workfront]以包含中繼資料與檔案。 如需對應中繼資料的詳細資訊，請參閱[設定中繼資料對應](../../administration-and-setup/configure-integrations/set-up-metadata-mapping.md)。

## 設定自訂檔案整合

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **)</p>
-->

自訂檔案整合可讓[!DNL Workfront]使用者從幾乎任何系統連結檔案至[!DNL Workfront]，但前提是系統必須與[!DNL Workfront]搭配使用。

若要讓使用者可以使用自訂整合，您必須先建置整合。 如需有關如何建立與[!DNL Workfront]搭配使用的整合的資訊，請參閱[Document Webhooks API](../../wf-api/doc-wbhks-api/docu-webhook-api.md)。

建立自訂檔案整合後，您就可以將其提供給網站上的使用者。

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**[!UICONTROL 檔案]** > **[!UICONTROL 自訂整合]**。

1. 按一下&#x200B;**[!UICONTROL 新增自訂整合]**。
1. 輸入下列資訊以設定整合：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL名稱]</td> 
      <td>自訂整合的名稱。 這是使用者在Workfront中使用整合時看到的名稱。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL基本API URL] </td> 
      <td>API呼叫的基本HTTP或安全HTTP URL。 例如， <code>https://&lt;documentprovider&gt;.com/api/v2</code></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL驗證型別]</td> 
      <td> <p>對自訂整合發出授權API呼叫時所使用的驗證方法。</p> 
       <ul> 
        <li>如果您選擇<strong>[！UICONTROL OAuth]</strong>，請繼續步驟5。</li> 
        <li>如果您選擇<strong>[！UICONTROL ApiKey]</strong>，請繼續步驟6。</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. （視條件而定）如果您為&#x200B;**[!UICONTROL 驗證型別]**&#x200B;選取&#x200B;**[!UICONTROL OAuth]**&#x200B;驗證，請輸入下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL驗證URL]</td> 
      <td>用於使用者驗證的完整URL。 [!DNL Workfront]會在OAuth布建程式過程中將使用者導覽至此位址。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL權杖端點URL]</td> 
      <td>用於擷取 OAuth 權杖的完整 API URL。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL使用者端ID]</td> 
      <td>此整合的OAut使用者端ID。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL使用者端密碼]</td> 
      <td>此整合的OAut使用者端密碼。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL請求引數]</td> 
      <td> <p>輸入要附加至每個API呼叫之查詢字串的選用值。 例如，access_type=offline。</p> <p>若要新增多個請求引數，請按一下<strong>+新增請求引數</strong>。</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >顯示在[!UICONTROL 自訂整合]頁面底部的[!DNL Workfront]重新導向URI列出用來向外部檔案提供者註冊此整合的URI。

1. （視條件而定）如果您為&#x200B;**[!UICONTROL 驗證型別]**&#x200B;選取&#x200B;**[!UICONTROL ApiKey]**&#x200B;驗證，請輸入自訂檔案提供者所發出的API金鑰。

   [!DNL Workfront]使用此API金鑰對檔案提供者進行授權的API呼叫。

1. 按一下&#x200B;**[!UICONTROL 儲存]**&#x200B;以建立整合。

## 使用檔案整合

如需使用者如何使用校訂的相關資訊，請參閱[建立校訂](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs-in-wf.md)。

如需使用者在您設定協力廠商檔案整合後如何使用協力廠商檔案整合的相關資訊，請參閱[從外部應用程式連結檔案](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)。

### 設定[!DNL Workfront]將中繼資料傳送至[!UICONTROL [!DNL Workfront] DAM] {#configure-workfront-to-send-metadata-to-workfront-dam}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **) </p>
-->

從[!DNL Workfront]傳送檔案至[!DNL Workfront DAM]時，您也可以傳送與該檔案相關的資訊。 檔案的相關資訊會作為中繼資料對應至[!DNL Workfront DAM]。

資訊只會單向對應，從[!DNL Workfront]到[!DNL Workfront DAM]，而且只有在檔案上傳到[!DNL Workfront DAM]時才會傳輸資訊。 上傳檔案後，Workfront欄位中任何未來的變更都不會更新[!DNL Workfront DAM]中的中繼資料欄位。\
您可以將相同的[!DNL Workfront]欄位對應到不同的[!DNL Workfront DAM]欄位，但您無法將相同的[!DNL Workfront DAM]欄位用於多個[!DNL Workfront]欄位。

如果您必須設定多個[!DNL Workfront]欄位以匯出至一個[!DNL Workfront DAM]欄位，請先在[!DNL Workfront]中建立計算自訂欄位，以顯示物件的所有個別自訂欄位。 然後，將計算的[!DNL Workfront]欄位對應到一個[!DNL Workfront DAM]欄位。\
如需有關計算自訂欄位的詳細資訊，請參閱[將計算欄位新增至表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)。

對應會影響任何使用者從[!DNL Workfront]上傳到[!UICONTROL Workfront] DAM的所有檔案。

身為[!DNL Workfront]管理員，您必須先在Workfront中啟用[!DNL Workfront DAM]，才能對應中繼資料對應程式的欄位。

若要設定[!DNL Workfront]將中繼資料傳送至[!DNL Workfront DAM]：

{{step-1-to-setup}}

1. 按一下&#x200B;**[!UICONTROL 檔案]** > **[!UICONTROL 中繼資料對應]**。

1. 在&#x200B;**[!UICONTROL 選取要對應的Source欄位]**&#x200B;欄位中，開始輸入您要對應到[!DNL Workfront DAM]的Workfront欄位名稱，然後在清單中看到它時選取它。
1. 在&#x200B;**[!UICONTROL 選取對應目標欄位]**&#x200B;中，選取要以所選[!DNL Workfront]欄位中的資訊填入的[!DNL Workfront DAM]欄位。

   >[!NOTE]
   >
   > 有權傳送給[!DNL Workfront DAM]的使用者上傳至[!DNL Workfront DAM]時，其所有檔案的中繼資料都會更新為對應至此處的[!DNL Workfront]欄位。

1. 按一下&#x200B;**[!UICONTROL 新增對應]**。

1. 繼續新增更多[!UICONTROL Workfront]欄位和對應的[!DNL Workfront DAM]欄位。

### 刪除對應的欄位

{{step-1-to-setup}}

1. 展開&#x200B;**[!UICONTROL 檔案]**，然後按一下&#x200B;**[!UICONTROL 中繼資料對應]**。

1. 在欄位清單中，選取您要從中繼資料對應中移除的任何欄位。
1. 按一下&#x200B;**[!UICONTROL 刪除]**。

   這些欄位會從中繼資料對應中移除，而且其中包含的資訊不會隨上傳的檔案傳輸到[!DNL Workfront DAM]。


## 限制

### Google Drive整合

* 將連結資料夾新增至Workfront時，資料夾中的檔案不再自動新增。
   * 您可以將Google資料夾新增至Workfront （不含檔案），然後將個別檔案新增至Workfront。 這些檔案會自動新增至Workfront中的Google資料夾。
或
   * 您可以在Workfront中建立「檔案」資料夾，然後選取Google資料夾中的所有檔案，並將它們新增至Workfront資料夾。


* Google Drive檔案整合支援從Google Drive的「我的磁碟機」區域新增檔案。 您無法從共用磁碟機新增資料夾或影像。 深入瞭解[Google共用磁碟機](https://support.google.com/a/users/answer/7212025?hl=en)。
