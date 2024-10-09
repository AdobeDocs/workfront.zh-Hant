---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Adobe Workfront模組
description: 您可以使用Adobe Workfront Fusion Adobe Workfront聯結器在Workfront中自動化您的流程。 如果您有Workfront Fusion for Work Automation and Integration授權，也可以用它來連線至協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion, Workfront Integrations and Apps
exl-id: b84d2d41-a983-4ea3-b331-0302bfcf8a2b
source-git-commit: 38b6fef43157f47c93dcd9cf543f1001142d86dd
workflow-type: tm+mt
source-wordcount: '6621'
ht-degree: 2%

---

# [!DNL Adobe Workfront]模組

您可以使用[!DNL Adobe Workfront Fusion] [!DNL Adobe Workfront]聯結器在[!DNL Workfront]內自動化您的程式。 如果您有[!UICONTROL [!DNL Workfront Fusion]的Work Automation與Integration]授權，也可以用它來連線到協力廠商的應用程式和服務。

[!DNL Workfront]聯結器不會計入您的組織可用的作用中應用程式數目。 所有情境（即使只使用[!DNL Workfront]應用程式）都會計入貴組織的情境總數。

如需貴組織可用應用程式和情境的詳細資訊，請參閱[[!DNL Adobe Workfront Fusion] 組織和團隊](../../workfront-fusion/organizations/organizations-and-teams.md)中的[組織](../../workfront-fusion/organizations/organizations-and-teams.md#organiza2)。

如果您需要有關建立案例的指示，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md)中建立案例。 如需模組的相關資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md)中的[模組。

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td>
  <td> <p>[！UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td>
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 授權**</td> 
   <td>
   <p>目前授權需求：無[!DNL Workfront Fusion]授權需求。</p>
   <p>或</p>
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]，[！UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]計畫，您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]計畫中。</p>
   <p>或</p>
   <p>舊版產品需求：您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>


若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 將[!DNL Workfront]連線至[!DNL Workfront Fusion]

[!DNL Workfront]聯結器使用OAuth 2.0連線至[!DNL Workfront]。

您可以直接從[!DNL Workfront Fusion]模組內建立與您的[!DNL Workfront]帳戶的連線。

1. 在任何Adobe Workfront模組中，按一下[連線]欄位旁的&#x200B;**新增**。
1. 填寫下列欄位：

   <table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
      <tr>
        <td role="rowheader">[！UICONTROL連線名稱]</td>
        <td>
          <p>輸入新連線的名稱。</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL環境]</td>
        <td>
          <p>選取要連線到生產或非生產環境。</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL連線型別]</td>
        <td>
          <p>選取您要連線到服務帳戶還是個人帳戶。</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL使用者端ID]</td>
        <td>輸入您的[!DNL Workfront]使用者端識別碼。 您可在Workfront中「設定」區域的「OAuth2應用程式」區域中找到此專案。 開啟您要連線的特定應用程式以檢視使用者端ID。</td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL使用者端密碼]</td>
        <td>輸入您的[!DNL Workfront]使用者端識別碼。 您可在Workfront中「設定」區域的「OAuth2應用程式」區域中找到此專案。 開啟您要連線的特定應用程式以檢視使用者端ID。</td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL驗證URL]</td>
        <td>這可以維持預設值，或者您可以輸入Workfront執行個體的URL，然後輸入<code>/integrations/oauth2</code>。 <p>範例： <code>https://mydomain.my.workfront.com/integrations/oauth2</code></p></td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL主機前置詞]</td>
        <td>在大多數情況下，此值應該是<code>origin</code>。
      </tr>
    </tbody>
    </table>

1. 按一下&#x200B;**[!UICONTROL 繼續]**&#x200B;以儲存連線並返回模組。




<!--1. Enter the name of your instance into the URL. Example: `https://<your instance>.my.workfront.com`.
1. Click **[!UICONTROL Next]**.
1. Click **[!UICONTROL SAML log in]** to create the connection and go back to the module.

   Or

   Enter your Username and Password, then click **[!UICONTROL Log in]** to create the connection and go back to the module.-->

>[!NOTE]
>
>* 如果您沒有看到SAML登入按鈕，表示您的組織尚未啟用單一登入(SSO)。 您可以使用您的使用者名稱和密碼登入。
>   
>   如需有關SSO的詳細資訊，請參閱[單一登入概述 [!DNL Adobe Workfront]](../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)
>   
>* [!DNL Workfront] API的OAuth 2.0連線不再依賴API金鑰。
>* 若要建立與Workfront沙箱環境的連線，您必須在該環境中建立OAuth2應用程式，然後在您的連線中使用該應用程式產生的使用者端ID和使用者端密碼。
>
>   如需在Workfront中建立OAuth2應用程式的指示，請參閱為Workfront整合建立OAuth2應用程式一文中的[使用使用者認證（授權代碼流程）建立OAuth2應用程式](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md#create-an-oauth2-application-using-user-credentials-authorization-code-flow)。

## [!DNL Workfront]模組及其欄位

當您設定[!DNL Workfront]模組時，[!DNL Workfront Fusion]會顯示下列欄位。 除了這些欄位以外，可能還會顯示其他[!DNL Workfront]欄位，視您在應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中將資訊從一個模組對應到另一個模組。


![](assets/map-toggle-350x74.png)

>[!NOTE]
>
>* 如果您在Workfront模組中未看到最新欄位，可能是因為快取問題。 請等待一小時，然後再試一次。
>* 來自Adobe Workfront的HTTP 429狀態程式碼不應導致停用，而會在案例中觸發短暫的執行暫停。

* [觸發器](#triggers)
* [動作](#actions)
* [搜尋](#searches)

### 觸發器

<!--
* [Watch Events](#watch-events) 
* [Watch Record](#watch-record) 
* [Watch Field](#watch-field)
-->

+++ **[!UICONTROL 觀看活動]**

在Workfront中新增、更新或刪除特定型別的物件時，此觸發模組會即時執行案例

模組會傳回與記錄相關聯的任何標準欄位，以及連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

1. 按一下&#x200B;**Webhook**&#x200B;方塊右側的&#x200B;**[!UICONTROL [新增]**]。

1. 在顯示的&#x200B;**[!UICONTROL 新增連結]**&#x200B;方塊中設定webhook。

   當您設定此模組時，會顯示下列欄位。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[！UICONTROL Webhook名稱]</td> 
      <td>（可選）為webhook輸入新名稱</td> 
     </tr> 
     <tr> 
      <td>[！UICONTROL Connection]</td> 
      <td> <p>如需有關將[!DNL Workfront]應用程式連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">將[!DNL Workfront]連線到[!DNL Workfront Fusion]</a>。</p> </td> 
     </tr> 
     <tr> 
      <td>[！UICONTROL記錄型別]</td> 
      <td>選取您希望模組觀看的[!DNL Workfront]記錄型別。</td> 
     </tr> 
     <tr> 
      <td>[！UICONTROL狀態]</td> 
      <td>選取您要觀看舊狀態還是新狀態。<ul><li><p><b>[！UICONTROL新狀態]</b></p><p>當記錄將指定值<b>變更為</b>時觸發案例。</p><p>例如，如果狀態設為[！UICONTROL New State]，而篩選條件設為[！UICONTROL Status] [！UICONTROL Equals] [！UICONTROL In Progress]，則webhook會在[！UICONTROL Status]變更為[！UICONTROL In Progress]時觸發案例，無論狀態之前為何。 </p></li><li><p><b>[！UICONTROL舊狀態]</b></p><p>當記錄從</b>變更指定值時，觸發案例<b>。</p><p>例如，如果狀態設為[！UICONTROL Old State]，而篩選條件設為[！UICONTROL Status] [！UICONTROL Equals] [！UICONTROL In Progress]，則當[！UICONTROL Status]目前為[！UICONTROL In Progress]的狀態變更為其他狀態時，webhook會觸發一個情境。 </p></li></ul></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td> <p>[！UICONTROL事件篩選器]</p> </td> 
      <td> <p>您可以設定篩選器，只監視符合您選取條件的記錄。</p> <p>針對每個篩選器，輸入您希望篩選器評估的欄位、運運算元，以及您希望篩選器允許的值。 您可以新增AND規則來使用一個以上的篩選器。</p> <p>注意：您無法編輯現有[!DNL Workfront] Webhook中的篩選器。 若要為[!DNL Workfront]個事件訂閱設定不同的篩選器，請移除目前的webhook並建立新的篩選器。</p> <p>如需事件篩選的詳細資訊，請參閱本文中[!DNL Workfront] &gt; [！UICONTROL觀看事件]模組</a>中的<a href="#event-subscription-filters-in-the-workfront-watch-events-modules" class="MCXref xref">事件訂閱篩選。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td>排除此連線造成的事件</td> 
      <td>啟用此選項可排除使用此觸發模組使用的相同聯結器建立或更新的事件。 這可防止案例可能觸發自身的情況，導致其在無限回圈中重複。<p><b>注意</b>指派記錄型別不包含此選項。</p></td> 
     </tr> 
     <tr> 
      <td>[！UICONTROL記錄來源]</td> 
      <td> <p>選擇您希望案例僅觀看<strong>[！UICONTROL新記錄]</strong>、<strong>[！UICONTROL僅更新記錄]</strong>、<strong>[！UICONTROL新記錄和更新記錄]</strong>或<strong>[!DNL Deleted Records Only]</strong>。</p> <p>注意：如果您選擇<strong>[！UICONTROL新增和更新的記錄]</strong>，webhook建立會建立2個事件訂閱（針對相同的webhook位址）。</p> </td> 
     </tr> 
    </tbody> 
   </table>

建立webhook後，您可以檢視事件傳送到的端點位址。

如需詳細資訊，請參閱[!DNL Workfront]說明文章[事件訂閱API](../../wf-api/general/event-subs-api.md)中的[事件裝載範例](../../wf-api/general/event-subs-api.md#examples-of-event-payloads)小節。

檢視您可以在每個 [!DNL Workfront] 模組](#workfront-object-types-available-for-each-workfront-module)可用的[[!DNL Workfront] 物件型別中使用此模組的[!DNL Workfront]物件型別清單。

+++

+++ **[!UICONTROL 觀看欄位]**

當您指定的欄位更新時，此觸發模組會執行情境。 模組會傳回您指定之欄位的舊值和新值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
   <td> <p>如需有關將[!DNL Workfront]應用程式連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">將[!DNL Workfront]連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL記錄型別]</td> 
   <td> <p>選取您希望模組觀看的[!DNL Workfront]記錄型別。</p> <p>例如，如果您要在每次更新任務中的記錄欄位時開始執行案例，請選取[！UICONTROL任務]。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL欄位]</td> 
   <td>選取您希望模組監視更新的欄位。 這些欄位反映[!DNL Workfront]管理員已設定用於追蹤的欄位。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL輸出]</td> 
   <td>選取要包含在此模組輸出組合中的資訊。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL限制]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>

檢視您可以在每個 [!DNL Workfront] 模組](#workfront-object-types-available-for-each-workfront-module)可用的[[!DNL Workfront] 物件型別中使用此模組的[!DNL Workfront]物件型別清單。

+++

+++ **[!UICONTROL 觀看記錄]**

此觸發模組會在新增、更新特定型別的物件或兩者同時進行時，執行案例。 模組會傳回與一個或多個記錄相關聯的所有標準欄位，以及連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。 在輸出中，模組會指出每個記錄是新的還是更新的。

在指定時段新增和更新的記錄會傳回為新記錄。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將[!DNL Workfront]應用程式連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">將[!DNL Workfront]連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL篩選器]</td> 
   <td> <p>選擇您希望案例僅觀看<strong>[！UICONTROL新記錄]</strong>、<strong>[！UICONTROL僅更新記錄]</strong>或<strong>[！UICONTROL新記錄和更新記錄]</strong>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別]</td> 
   <td> <p>（在您選擇<strong>篩選器</strong>之後顯示。） 選取您希望模組觀看的[!DNL Workfront]記錄型別。</p> <p>例如，如果您要在每次建立新專案時啟動情境，請選取[！UICONTROL專案]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸出]</td> 
   <td> <p>選取要包含在此模組輸出組合中的資訊。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選用篩選器]</td> 
   <td> <p>（進階）輸入API程式碼字串，以定義將縮小條件範圍的任何其他引數或程式碼。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>

檢視您可以在每個 [!DNL Workfront] 模組](#workfront-object-types-available-for-each-workfront-module)可用的[[!DNL Workfront] 物件型別中使用此模組的[!DNL Workfront]物件型別清單。

+++


### 動作

<!--
* [Convert object](#convert-object) 
* [Create a record (attaching custom forms)](#create-a-record-attaching-custom-forms) 
* [Create a record](#create-a-record) 
* [Custom API Call](#custom-api-call) 
* [Delete Record](#delete-record) 
* [Download Document](#download-document) 
* [Misc Action](#misc-action) 
* [Read a Record](#read-a-record) 
* [Update Record](#update-record) 
* [Upload Document](#upload-document)
-->

+++ **[!UICONTROL 轉換物件]**

此動作模組會進行下列其中一個轉換：

* 將問題轉換為專案
* 將問題轉換為任務
* 將任務轉換為專案

>[!NOTE]
>
>自2024年7月起，轉換物件時可包含自訂表單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
   <td> <p>如需有關將[!DNL Workfront]應用程式連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">將[!DNL Workfront]連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL物件型別]</td> 
   <td> <p>選取您要轉換的物件型別。 這是轉換前物件的型別。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL轉換為]</td> 
   <td>選取您想要將它轉換成的物件。 這是物件在轉換後的型別。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL &lt;物件&gt; ID]</td> 
   <td> <p>輸入物件的ID。 </p> <p>附註：輸入物件識別碼時，您可以開始輸入物件的名稱，然後從清單中選取它。 模組接著在欄位中輸入適當的ID。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL範本ID]</td> 
   <td> <p>如果要轉換為專案，請選取要用於專案的範本ID。</p> <p>附註：輸入物件識別碼時，您可以開始輸入物件的名稱，然後從清單中選取它。 模組接著在欄位中輸入適當的ID。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL自訂表單]</td> 
   <td>選取您要新增至新轉換物件的任何自訂表單，然後輸入自訂表單欄位的值。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL Options]</td> 
   <td> <p>啟用轉換物件時所需的任何選項。 選項是否可用取決於您轉換至哪個物件或轉換自哪個物件。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL複製原生欄位]</td> 
   <td> <p>啟用此選項可將任何原生欄位從原始物件複製到新物件。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL複製自訂表單]</td> 
   <td> <p>啟用此選項可將任何原生欄位從原始物件複製到新物件。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 建立記錄（附加自訂表格）]**

此動作模組會在[!DNL Workfront]中建立專案、任務或問題等物件，並允許您將自訂表單新增到新物件。 模組可讓您選取可在模組中取得哪些物件欄位。

您指定記錄的ID。

模組會傳回記錄ID及任何關聯欄位，連同連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

例如，當使用者端在需要完成的工作清單[!DNL Google Sheets]中新增一列時，您可以使用此模組在[!DNL Workfront]中建立工作。

當您設定此模組時，會顯示下列欄位。

請務必提供最小輸入欄位數。 例如，如果您想建立問題，則需要在「專案ID」欄位中提供有效的父專案ID，以指出問題應存在於Workfront中的何處。 您可以使用對應面板從情境中的另一個模組對應此資訊，或是輸入名稱，然後從清單中選取它，以手動方式輸入資訊。

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
   <td> <p>如需有關將[!DNL Workfront]應用程式連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">將[!DNL Workfront]連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL記錄型別]</td> 
   <td> <p>選取您要模組建立的[!DNL Workfront]記錄型別。</p> <p>例如，如果您想要建立專案，請從下拉式清單中選取[！UICONTROL專案]，然後確定您有權存取將填入專案的資料（來自案例中先前模組）。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL選擇要對應的欄位]</td> 
   <td> <p>選取您想用於資料輸入的欄位。 這可讓您使用這些欄位，而無需捲動瀏覽您不需要的欄位。</p> <p>對於自訂表單中的欄位，請使用<b>[！UICONTROL附加自訂表單]</b>欄位。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL附加自訂表單]</td> 
   <td>選取您要新增至新物件的任何自訂表單，然後輸入這些欄位的值。</td> 
  </tr> 
 </tbody> 
</table>

檢視您可以在每個 [!DNL Workfront] 模組](#workfront-object-types-available-for-each-workfront-module)可用的[[!DNL Workfront] 物件型別中使用此模組的[!DNL Workfront]物件型別清單。

>[!NOTE]
>
>* 輸入物件的ID時，您可以開始輸入物件的名稱，然後從清單中選取它。 模組接著在欄位中輸入適當的ID。
>* 輸入自訂欄位或[!UICONTROL Note]物件（註解或回覆）的文字時，您可以使用[!UICONTROL Note文字]欄位中的HTML標籤來建立RTF文字，例如粗體或斜體文字。
>
>  如需更新中RTF文字的詳細資訊，請參閱[更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)中的[將更新新增至工作專案](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add)。
>

+++

+++ **[!UICONTROL 建立記錄]**

此動作模組會建立物件，例如Workfront中的專案、任務或問題。 模組可讓您選取可在模組中取得哪些物件欄位。

您指定記錄的ID。

模組會傳回記錄ID及任何關聯欄位，連同連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

例如，當使用者端在Google工作表清單中新增需要完成的工作時，您可以使用此模組在[!DNL Workfront]中建立工作。

當您設定此模組時，會顯示下列欄位。

請務必提供最小輸入欄位數。 例如，如果您想建立問題，則需要在「專案ID」欄位中提供有效的父專案ID，以指出問題應存在於Workfront中的何處。 您可以使用對應面板從情境中的另一個模組對應此資訊，或是輸入名稱，然後從清單中選取它，以手動方式輸入資訊。

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
   <td> <p>如需有關將[!DNL Workfront]應用程式連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">將[!DNL Workfront]連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL記錄型別]</td> 
   <td> <p>選取您要模組建立的[!DNL Workfront]記錄型別。</p> <p>例如，如果您想要建立專案，請從下拉式清單中選取[！UICONTROL專案]，然後確定您有權存取將填入專案的資料（來自案例中先前模組）。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL選擇要對應的欄位]</td> 
   <td>選取您想用於資料輸入的欄位。 這可讓您使用這些欄位，而無需捲動瀏覽您不需要的欄位。</td> 
  </tr> 
 </tbody> 
</table>

檢視您可以在每個 [!DNL Workfront] 模組](#workfront-object-types-available-for-each-workfront-module)可用的[[!DNL Workfront] 物件型別中使用此模組的[!DNL Workfront]物件型別清單。

>[!NOTE]
>
>* 輸入物件的ID時，您可以開始輸入物件的名稱，然後從清單中選取它。 模組接著在欄位中輸入適當的ID。
>* 輸入自訂欄位或[!UICONTROL Note]物件（註解或回覆）的文字時，您可以使用[!UICONTROL Note文字]欄位中的HTML標籤來建立RTF文字，例如粗體或斜體文字。
>
>  如需更新中RTF文字的詳細資訊，請參閱[更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)中的[將更新新增至工作專案](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add)。
>

+++

+++ **[!UICONTROL 自訂API呼叫]**

此動作模組可讓您對[!DNL Workfront] API進行自訂的已驗證呼叫。 如此一來，您就可以建立其他[!DNL Workfront]模組無法完成的資料流程自動化。

模組會傳回下列資訊：

* **[!UICONTROL 狀態碼]** （數字）：這表示您的HTTP要求成功或失敗。 這些是您可在網際網路上查閱的標準程式碼。
* **[!UICONTROL Headers]** （物件）：與輸出本文無關之回應/狀態代碼的更詳細內容。 並非顯示在回應標題中的所有標題都是回應標題，因此某些標題可能對您並不實用。

  回應標題取決於您在設定模組時選擇的HTTP請求。

* **[!UICONTROL 內文]** （物件）：根據您在設定模組時所選擇的HTTP要求，您可能會收到一些傳回的資料。 該資料(例如來自GET請求的資料)包含在此物件中。

您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將[!DNL Workfront]應用程式連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">將[!DNL Workfront]連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p>輸入相對於<code> https://&lt;WORKFRONT_DOMAIN&gt;/attask/api/&lt;API_VERSION&gt;/</code>的路徑。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL API版本]</td> 
   <td>選取您希望模組使用的[!DNL Workfront] API版本。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL方法]</td> 
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP要求方法。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標頭。 這會決定請求的內容型別。</p> <p>例如，<code> {"Content-type":"application/json"}</code></p> <p>注意：如果您收到錯誤且難以判斷其來源，請考慮根據[!DNL Workfront]檔案修改標題。 如果您的自訂API呼叫傳回422 HTTP請求錯誤，請嘗試使用<code>"Content-Type":"text/plain"</code>標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查詢字串]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的查詢。</p> <p>例如： <code>{"name":"something-urgent"}</code></p> <p>提示：建議您透過JSON內文傳送資訊，而非查詢引數。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Body]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的內文內容。</p> <p>注意：  <p>在JSON中使用條件陳述式（例如<code>if</code>）時，請將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

檢視您可以在每個 [!DNL Workfront] 模組](#workfront-object-types-available-for-each-workfront-module)可用的[[!DNL Workfront] 物件型別中使用此模組的[!DNL Workfront]物件型別清單。

+++

+++ **[!UICONTROL 刪除記錄]**

此動作模組會刪除物件，例如Workfront中的專案、任務或問題。

您指定記錄的ID。

模組會傳回記錄ID及任何關聯欄位，連同連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
   <td> <p>如需有關將[!DNL Workfront]應用程式連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">將[!DNL Workfront]連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL強制刪除]</td> 
   <td>啟用此選項以確保刪除記錄，即使[!DNL Workfront] UI要求確認刪除。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>ID</td> 
   <td> <p>輸入您要模組刪除之記錄的唯一[!DNL Workfront]識別碼。</p> <p>若要取得ID，請在瀏覽器中開啟[!DNL Workfront]物件，並在"ID="後複製URL結尾的文字。 例如： https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL記錄型別]</td> 
   <td>選取您要模組刪除的[!DNL Workfront]記錄型別。</td> 
  </tr> 
 </tbody> 
</table>

檢視您可以在每個 [!DNL Workfront] 模組](#workfront-object-types-available-for-each-workfront-module)可用的[[!DNL Workfront] 物件型別中使用此模組的[!DNL Workfront]物件型別清單。

>[!NOTE]
>
>我們建議使用下列案例設定，以避免因非同步操作而無法刪除記錄的可能性。
>
>1. 同步刪除記錄。
>1. 新增錯誤處理至刪除記錄模組，以忽略40秒逾時造成的錯誤。


+++

+++ **[!UICONTROL 下載檔案]**

此動作模組會從Workfront下載檔案。

您指定記錄的ID。

模組會傳回檔案的內容、檔案名稱、副檔名和檔案大小。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
   <td> <p>如需有關將[!DNL Workfront]應用程式連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">將[!DNL Workfront]連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL檔案ID]</td> 
   <td> <p>對應或手動輸入您要模組下載之檔案的唯一[!DNL Workfront] ID。</p> <p>若要取得ID，請在瀏覽器中開啟[!DNL Workfront]物件，並在"ID="後複製URL結尾的文字。 例如： https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
 </tbody> 
</table>

檢視您可以在每個 [!DNL Workfront] 模組](#workfront-object-types-available-for-each-workfront-module)可用的[[!DNL Workfront] 物件型別中使用此模組的[!DNL Workfront]物件型別清單。

+++

+++ **[!UICONTROL 其他動作]**

此動作模組可讓您對API執行動作。

>[!NOTE]
>
>截至2024年7月，`convertToProject`動作包含欄位`copyCategories`。 設定為`TRUE`時，所有自訂表單都將包含在問題轉換為的專案中。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
   <td> <p>如需有關將[!DNL Workfront]應用程式連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">將[!DNL Workfront]連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL記錄型別]</td> 
   <td> <p>選取您希望模組與之互動的[!DNL Workfront]記錄型別。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL動作]</td> 
   <td> <p>選取您希望模組執行的動作。</p> <p>視您選擇的[！UICONTROL記錄型別]和[！UICONTROL動作]而定，您可能需要填寫其他欄位。 這兩個設定的某些組合可能只需要記錄ID，而其他設定（例如<strong>[！UICONTROL記錄型別]</strong>的Project和<strong>[！UICONTROL動作]</strong>的[！UICONTROL附加範本]）則需要其他資訊（例如物件ID和範本ID）。</p> <p>如需個別欄位的詳細資訊，請參閱<a href="http://developer.workfront.com/">Workfront開發人員檔案</a>。 <p><strong>注意</strong>：開發人員檔案網站僅包含透過API版本14的資訊，但仍包含API呼叫的重要資訊。 </p> 
    <ol> 
     <li value="1"> <p>從[!DNL Workfront]開發人員檔案頁面的左側導覽選取記錄型別。 下列型別有自己的頁面：</p> 
      <ul> 
       <li> <p>[！UICONTROL專案]</p> </li> 
       <li> <p>[！UICONTROL工作]</p> </li> 
       <li> <p>[！UICONTROL問題]</p> </li> 
       <li> <p>[！UICONTROL使用者]</p> </li> 
       <li> <p>[！UICONTROL檔案]</p> </li> 
      </ul> <p>針對所有其他記錄型別，選取<b>[！UICONTROL Other objects and endpoints]</b>，然後在依字母順序排序的頁面上尋找記錄型別。</p> </li> 
     <li value="2"> <p>在適當記錄型別的頁面上，搜尋動作（Ctrl-F或Cmd-F）。</p> </li> 
     <li value="3"> <p>檢視所選動作下可用欄位的說明。</p> </li> 
    </ol> <p>注意：  <p>透過[!DNL Workfront] [！UICONTROL雜湊動作]模組建立校訂時，最佳實務是建立不含任何進階選項的校訂，然後使用[!DNL Workfront Proof] SOAP API更新校訂。</p> <p>如需使用[!DNL Workfront] API （此模組使用）建立校訂的詳細資訊，請參閱<a href="../../wf-api/tips-tricks-and-troubleshooting/api-create-proof-options-json.md" class="MCXref xref">透過[!DNL Adobe Workfront] API建立校訂時新增進階校訂選項</a></p> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL ID]</td> 
   <td>輸入或對應您希望模組與其互動之記錄的唯一[!DNL Workfront]識別碼。<p>若要取得ID，請在瀏覽器中開啟[!DNL Workfront]物件，並在"ID="後複製URL結尾的文字。 例如： https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p></td> 
  </tr> 
 </tbody> 
</table>

檢視您可以在每個 [!DNL Workfront] 模組](#workfront-object-types-available-for-each-workfront-module)可用的[[!DNL Workfront] 物件型別中使用此模組的[!DNL Workfront]物件型別清單。

+++

+++ **[!UICONTROL 讀取記錄]**

此動作模組會從單一記錄擷取資料。

您指定記錄的ID。 您也可以指定要讓模組讀取哪些相關記錄。

例如，如果模組正在讀取的記錄是專案，您可以指定您要讀取專案任務。

模組會針對您指定的輸出，從標準欄位傳回資料陣列。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[！UICONTROL Connection]</td>

<td> <p>如需有關將[!DNL Workfront]應用程式連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">將[!DNL Workfront]連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
    <td>[！UICONTROL記錄型別]</td>

<td>選擇您希望模組讀取的[!DNL Workfront]物件型別。</td> 
  </tr> 
  <tr> 
    <td>[！UICONTROL輸出]</td>

<td> <p>選取要包含在此模組輸出組合中的資訊。</p> </td> 
  </tr> 
  <tr> 
    <td>[！UICONTROL參考]</td>
   <td>選取您要納入輸出的任何參考欄位。</td> 
  </tr> 
  <tr> 
    <td>[！UICONTROL集合]</td>
   <td>選取您要納入輸出的任何參考欄位。</td> 
  </tr> 
  <tr> 
    <td>[！UICONTROL ID]</td>
   <td> <p>輸入您希望模組讀取之記錄的唯一[!DNL Workfront]識別碼。</p> <p>若要取得ID，請在瀏覽器中開啟[!DNL Workfront]物件，並在"ID="後複製URL結尾的文字。 例如： https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
 </tbody> 
</table>

檢視您可以在每個 [!DNL Workfront] 模組](#workfront-object-types-available-for-each-workfront-module)可用的[[!DNL Workfront] 物件型別中使用此模組的[!DNL Workfront]物件型別清單。

+++

+++ **[!UICONTROL 更新記錄]**

此動作模組會更新物件，例如專案、任務或問題。 模組可讓您選取可在模組中取得哪些物件欄位。

您指定記錄的ID。

模組會傳回物件ID及任何關聯欄位，以及連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
   <td> <p>如需有關將[!DNL Workfront]應用程式連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">將[!DNL Workfront]連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL ID]</td> 
   <td> <p>輸入您希望模組更新的記錄的唯一[!DNL Workfront]識別碼。</p> <p>若要取得ID，請在瀏覽器中開啟[!DNL Workfront]物件，並在"ID="後複製URL結尾的文字。 例如： https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Record Type]</td> 
   <td> <p>選取您希望模組更新的[!DNL Workfront]記錄型別。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!DNL Select fields to map]</td> 
   <td>選取您想用於資料輸入的欄位。 這可讓您使用這些欄位，而無需捲動瀏覽您不需要的欄位。</td> 
  </tr> 
 </tbody> 
</table>

檢視您可以在每個 [!DNL Workfront] 模組](#workfront-object-types-available-for-each-workfront-module)可用的[[!DNL Workfront] 物件型別中使用此模組的[!DNL Workfront]物件型別清單。

>[!NOTE]
>
>* 輸入物件的ID時，您可以開始輸入物件的名稱，然後從清單中選取它。 模組接著在欄位中輸入適當的ID。
>* 輸入自訂欄位或[!UICONTROL Note]物件（註解或回覆）的文字時，您可以使用[!UICONTROL Note文字]欄位中的HTML標籤來建立RTF文字，例如粗體或斜體文字。
>
>  如需更新中RTF文字的詳細資訊，請參閱[更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)中的[將更新新增至工作專案](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add)。
>

+++

+++ **[!UICONTROL 上傳檔案]**

此動作模組會將檔案上傳到[!DNL Workfront]物件，例如專案、任務或問題。 此模組會以區塊上傳檔案，讓Workfront的上傳程式更順暢。

您可以指定檔案的位置、要上傳的檔案，以及檔案的可選新名稱。

模組會傳回檔案ID和任何關聯欄位，以及連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
   <td> <p>如需有關將[!DNL Workfront]應用程式連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">將[!DNL Workfront]連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL相關記錄ID]</td> 
   <td>輸入您要將檔案上傳到其中之記錄的唯一[!DNL Workfront]識別碼。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL相關記錄型別]</td> 
   <td>選取您希望模組上傳檔案的[!DNL Workfront]記錄型別。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL資料夾ID]</td> 
   <td>視相關記錄的型別而定，您可能需要輸入或對映資料夾ID。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Source檔案]</td> 
   <td> <p>從先前的模組中選取來源檔案，或對應來源檔案的名稱和資料。</p> </td> 
  </tr> 
 </tbody> 
</table>

檢視您可以在每個 [!DNL Workfront] 模組](#workfront-object-types-available-for-each-workfront-module)可用的[[!DNL Workfront] 物件型別中使用此模組的[!DNL Workfront]物件型別清單。

+++

+++ **[!UICONTROL 上傳檔案（舊版）]**

此動作模組會將檔案上傳到[!DNL Workfront]物件，例如專案、任務或問題。 它會一次上傳整個檔案。

您可以指定檔案的位置、要上傳的檔案，以及檔案的可選新名稱。

模組會傳回檔案ID和任何關聯欄位，以及連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
   <td> <p>如需有關將[!DNL Workfront]應用程式連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">將[!DNL Workfront]連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL相關記錄ID]</td> 
   <td>輸入您要將檔案上傳到其中之記錄的唯一[!DNL Workfront]識別碼。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL相關記錄型別]</td> 
   <td>選取您希望模組上傳檔案的[!DNL Workfront]記錄型別。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL資料夾ID]</td> 
   <td>視相關記錄的型別而定，您可能需要輸入或對映資料夾ID。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Source檔案]</td> 
   <td> <p>從先前的模組中選取來源檔案，或對應來源檔案的名稱和資料。</p> </td> 
  </tr> 
 </tbody> 
</table>

檢視您可以在每個 [!DNL Workfront] 模組](#workfront-object-types-available-for-each-workfront-module)可用的[[!DNL Workfront] 物件型別中使用此模組的[!DNL Workfront]物件型別清單。

+++

### 搜尋

<!--
* [Read Related Records](#read-related-records) 
* [Search](#search)
-->

+++ **[!UICONTROL 讀取相關記錄]**

此搜尋模組會讀取符合您指定之搜尋查詢的記錄（在特定父物件中）。

您可以指定要包含在輸出中的欄位。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
   <td> <p>如需有關將[!DNL Workfront]應用程式連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">將[!DNL Workfront]連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL記錄型別]</td> 
   <td> <p>選取您要讀取其關聯記錄的父記錄型別(Workfront物件)。</p> <p>檢視[!DNL Workfront]物件型別的清單，您可以針對此清單在本文章中每個[!DNL Workfront]模組</a>可用的<a href="#object-types-available-for-each-workfront-search-module" class="MCXref xref">[!DNL Workfront]物件型別中使用此模組。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL父記錄ID]</td> 
   <td> <p>輸入或對應您要讀取其關聯記錄的父記錄識別碼。</p> <p>若要取得ID，請在瀏覽器中開啟[!DNL Workfront]物件，並在"ID="後複製URL結尾的文字。 例如： https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL集合]</td> 
   <td>選取或對應您希望模組讀取的子記錄型別。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL輸出]</td> 
   <td> <p>選取要包含在此模組輸出組合中的資訊。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 搜尋]**

此搜尋模組會在[!DNL Workfront]中尋找符合您指定之搜尋查詢的物件記錄。

您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
   <td> <p>如需有關將[!DNL Workfront]應用程式連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">將[!DNL Workfront]連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL記錄型別]</td> 
   <td> <p>選取您要模組搜尋的[!DNL Workfront]記錄型別。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL結果集]</td> 
   <td>選取選項以指定您希望模組取得符合搜尋條件的第一個結果，還是所有符合該條件的結果。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Maximal]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL搜尋條件欄位]</td> 
   <td> <p>選取您要用於搜尋條件的欄位。 這些欄位隨後將顯示在搜尋條件下拉式清單中。</p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL搜尋條件]</td> 
   <td> <p>輸入您要搜尋的欄位、要在查詢中使用的運運算元，以及要在欄位中搜尋的值。</p> <p>注意：請勿在您的搜尋條件中使用<code>username </code>。 在對[!DNL Workfront]的API查詢中包含<code>username </code>會將使用者登入Workfront，搜尋將不會成功。</p> <p>注意： <code>In</code>和<code>NotIn</code>可搭配陣列使用。 輸入的格式應為陣列。</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL輸出]</td> 
   <td> <p>選取您要包含在此模組輸出中的欄位。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL參考]</td> 
   <td>選取您要納入搜尋的任何參考欄位。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL集合]</td> 
   <td>選取您要新增至搜尋的任何集合。</td> 
  </tr> 
 </tbody> 
</table>
+++

+++ **[!UICONTROL 搜尋（舊版）]**

此搜尋模組會在[!DNL Workfront]中尋找符合您指定之搜尋查詢的物件記錄。

您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
   <td> <p>如需有關將[!DNL Workfront]應用程式連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">將[!DNL Workfront]連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL記錄型別]</td> 
   <td> <p>選取您要模組搜尋的[!DNL Workfront]記錄型別。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL結果集]</td> 
   <td>選取選項以指定您希望模組取得符合搜尋條件的第一個結果，還是所有符合該條件的結果。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Maximal]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL搜尋條件]</td> 
   <td> <p>輸入您要搜尋的欄位、要在查詢中使用的運運算元，以及要在欄位中搜尋的值。</p> <p>注意：請勿在您的搜尋條件中使用<code>username </code>。 在對[!DNL Workfront]的API查詢中包含<code>username </code>會將使用者登入Workfront，搜尋將不會成功。</p> <p>注意： <code>In</code>和<code>NotIn</code>可搭配陣列使用。 輸入的格式應為陣列。</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL輸出]</td> 
   <td> <p>選取您要包含在此模組輸出中的欄位。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL參考]</td> 
   <td>選取您要納入搜尋的任何參考欄位。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL集合]</td> 
   <td>選取您要新增至搜尋的任何集合。</td> 
  </tr> 
 </tbody> 
</table>

檢視您可以在每個 [!DNL Workfront] 模組](#workfront-object-types-available-for-each-workfront-module)可用的[[!DNL Workfront] 物件型別中使用此模組的[!DNL Workfront]物件型別清單。

+++

## 每個[!DNL Workfront]模組都有[!DNL Workfront]個可用的物件型別

<!-- [Object types available for each Workfront trigger module](#object-types-available-for-each-workfront-trigger-module) 
* [Object types available for each Workfront action module](#object-types-available-for-each-workfront-action-module) 
* [Object types available for each Workfront search module](#object-types-available-for-each-workfront-search-module)-->

+++每個[!DNL Workfront]觸發程式模組都有&#x200B;**可用的物件型別**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>[！UICONTROL監看紀錄]</th> 
   <th>[！UICONTROL監視欄位]</th> 
   <th>[！UICONTROL觀看活動]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>核准流程</td> 
   <td> </td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>指派</td> 
   <td> </td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>基準線</td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> 計費記錄 </td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>計費率</td> 
   <td> </td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>公司</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>儀表板</td> 
   <td> </td> 
   <td> </td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>文件</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>文件資料夾</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>文件要求</td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>文件版本</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>費用</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>費用類型</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>群組</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>小時</td> 
   <td> </td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>時數類型</td> 
   <td> </td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>問題</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>反覆項目</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>職務角色</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>日誌輸入項目</td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>里程碑</td> 
   <td> </td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>里程碑路徑</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>備註</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>附註標籤</td> 
   <td> </td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>專案組合</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>方案</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>專案</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>專案使用者</td> 
   <td> </td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>校樣核准</td> 
   <td> </td> 
   <td> </td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>保留時間* </td> 
   <td> </td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>報告</td> 
   <td> </td> 
   <td> </td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>風險</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>風險類型</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>步驟核准者</td> 
   <td> </td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>任務</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>團隊</td> 
   <td> </td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>範本</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>範本任務</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>時程表</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>使用者</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>更新</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++每個[!DNL Workfront]動作模組都有&#x200B;**可用的物件型別**

>[!NOTE]
>
>[!UICONTROL 下載檔案]模組未包含在此資料表中，因為[!DNL Workfront]物件型別不是其組態的一部分。

<table style="table-layout:auto"> 
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
   <th> </th> 
   <th>[！UICONTROL建立記錄]</th> 
   <th>[！UICONTROL更新記錄]</th> 
   <th>[！UICONTROL刪除記錄]</th> 
   <th>[！UICONTROL上傳檔案]</th> 
   <th>[！UICONTROL讀取記錄]</th> 
   <th>[！UICONTROL自訂API呼叫]</th> 
   <th>[！UICONTROL其他動作]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>核准流程</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>指派</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>基準線</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
   <tr> 
   <td>計費記錄</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>計費率</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>公司</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>文件</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>文件資料夾</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>文件版本</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>匯率</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>費用</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>費用類型</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>外部檔案</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>群組</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>小時</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>時數類型</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>問題</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>反覆項目</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>職務角色</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>日誌輸入項目</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>里程碑</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>里程碑路徑</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>備註</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>附註標籤</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>專案組合</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>方案</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>專案</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>專案使用者</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>保留時間* </td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>風險</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>風險類型</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>步驟核准者</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>任務</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>團隊</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>範本</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>範本任務</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>時程表</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>使用者</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>更新</td> 
   <td> </td> 
   <td>✓ (A)</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++每個[!DNL Workfront]搜尋模組都有&#x200B;**可用的物件型別**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>[！UICONTROL搜尋]</th> 
   <th>[！UICONTROL讀取相關記錄]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>核准流程</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>指派</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>計費記錄</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>計費率</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>公司</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>文件</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>文件資料夾</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>文件版本</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>費用</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>費用類型</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>群組</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>小時</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>時數類型</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>問題</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>反覆項目</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>職務角色</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>日誌輸入項目</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>里程碑</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>里程碑路徑</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>備註</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>附註標籤</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>專案組合</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>方案</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>專案</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>專案使用者</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>保留時間* </td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>風險</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>風險類型</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>步驟核准者</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>任務</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>團隊</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>範本</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>範本任務</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>時程表</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>使用者</td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td>使用者委派</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

建議您仔細檢查，確保此功能的運作方式與預期的一樣。

+++

## [!DNL Workfront] > [!UICONTROL 觀看活動]模組中的活動訂閱篩選器

>[!NOTE]
>
>我們強烈建議您在您的[!UICONTROL 觀看活動]模組中使用事件訂閱篩選器。

[!DNL Workfront] [!UICONTROL 觀看事件]模組會根據webhook觸發案例，該案例會在[!DNL Workfront] API中建立事件訂閱。 事件訂閱是一組資料，可決定要將哪些事件傳送到webhook。 例如，如果您設定監視問題的[!UICONTROL 監視事件]模組，則事件訂閱只會傳送與問題相關的事件。

透過使用事件訂閱篩選器，Fusion使用者可建立更適合其使用案例的事件訂閱。 例如，您可以在[!DNL Workfront] API中設定事件訂閱，以僅將特定專案中的問題傳送至webhook，確保[!UICONTROL 觀看事件]模組將只會觸發該專案中的問題。 建立較窄觸發器的功能可減少不相關觸發器的數量，進而改善情境設計。

這與在[!DNL Workfront Fusion]情境中設定篩選器不同。 如果沒有事件訂閱篩選器，您的webhook會接收與您選取的物件型別相關的所有事件。 這些事件大多與情境無關，必須先篩選掉，情境才能繼續。

「Workfront >關注事件」篩選器中提供下列運運算元：

* 等於
* 不等於
* 大於
* 小於
* 大於或等於
* 小於或等於
* 包含
* 存在
   * 此運運算元不需要值，而且值欄位不存在。
* 不存在
   * 此運運算元不需要值，而且值欄位不存在。
* 已變更
   * 此運運算元不需要值，而且值欄位不存在。
   * 此運運算元會忽略狀態列位。
   * 使用`Changed`時，請在&#x200B;**記錄來源**&#x200B;欄位中選取&#x200B;**僅更新事件**。

>[!IMPORTANT]
>
>您無法編輯現有[!DNL Workfront] Webhook中的篩選器。 若要為[!DNL Workfront]個事件訂閱設定不同的篩選器，請移除目前的webhook並建立新的篩選器。

>[!INFO]
>
>**範例：**&#x200B;考慮處理指派給特定使用者Ana之新問題的案例。
>
>### 使用事件訂閱篩選器來篩選事件（建議使用）
>
>使用事件篩選器，您可以設定webhook以在建立問題時將問題指派給Ana時觸發情境。 Ana具有userID b378489d8f7cd3cee0539260720a84b7。
>
>![](assets/event-filter-watch-events-350x277.png)
>
>如果一天內建立100個問題，但只有兩個問題指派給Ana，則案例會執行兩次。
>
>### 篩選案例中的事件（不建議）
>
>若要篩選事件，以便只處理指派給Ana的問題，您可以在[!UICONTROL 觀看事件]模組之後建立篩選器。
>
>![](assets/watch-events-non-event-filter-350x206.png)
>
>如果一天內建立100個問題，但只有兩個問題指派給Ana，則案例將執行100次。 98個執行會在篩選後停止，但觸發模組仍在所有執行中使用資料並執行操作。

如需有關活動訂閱的詳細資訊，請參閱[常見問題集 — 活動訂閱](../../wf-api/general/event-subs-faq.md)。

如需Webhook的詳細資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/webhooks/instant-triggers-webhooks.md)中的[即時觸發器(Webhook)

如需情境中篩選的詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md)中將篩選新增至情境。

