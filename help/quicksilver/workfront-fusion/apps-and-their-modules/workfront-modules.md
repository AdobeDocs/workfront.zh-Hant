---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Adobe Workfront模組
description: 您可以使用Adobe Workfront Fusion Adobe Workfront聯結器在Workfront中自動化您的流程。 如果您有Workfront Fusion for Work Automation and Integration授權，也可以使用它來連線至協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion, Workfront Integrations and Apps
exl-id: b84d2d41-a983-4ea3-b331-0302bfcf8a2b
source-git-commit: 2a49e8f1947d39efa85bb8b8bdb7aee5054f8d33
workflow-type: tm+mt
source-wordcount: '5378'
ht-degree: 3%

---

# [!DNL Adobe Workfront] 模組

您可以使用 [!DNL Adobe Workfront Fusion] [!DNL Adobe Workfront] 聯結器可自動化您的流程，在 [!DNL Workfront]. 如果您擁有 [!UICONTROL [!DNL Workfront Fusion] 適用於工作自動化與整合] 授權，您也可以用它來連線至協力廠商的應用程式和服務。

此 [!DNL Workfront] connector不會計入貴組織可用的作用中應用程式數量。 所有情境，即使只使用 [!DNL Workfront] 應用程式，確實會針對貴組織的案例總數計算。

如需貴組織可用應用程式和情境的詳細資訊，請參閱 [組織](../../workfront-fusion/organizations/organizations-and-teams.md#organiza2) 在 [[!DNL Adobe Workfront Fusion] 組織和團隊](../../workfront-fusion/organizations/organizations-and-teams.md).

如果您需要建立案例的說明，請參閱 [在中建立情境 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). 如需模組的相關資訊，請參閱 [中的模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td>
  <td> <p>[！UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td>
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 授權**</td> 
   <td> <p>[！UICONTROL [!DNL Workfront Fusion] 適用於工作自動化與整合] </p>  <p>[！UICONTROL [!DNL Workfront Fusion] 工作自動化專用]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述功能。</td> 
  </tr> 
 </tbody> 
</table>


若要瞭解您擁有哪些計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

有關以下專案的資訊： [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Connect [!DNL Workfront] 至 [!DNL Workfront Fusion]

此 [!DNL Workfront] 聯結器使用OAuth 2.0連線至 [!DNL Workfront].

您可以建立與的連線 [!DNL Workfront] 直接從a內的帳戶 [!DNL Workfront Fusion] 模組。

1. 在任何 [!DNL Workfront] 應用程式模組，按一下 **[!UICONTROL 新增]** 旁邊 [!UICONTROL 連線] 方塊。
1. 在URL中輸入執行個體的名稱。 範例: `https://<your instance>.my.workfront.com`.
1. 按一下 **[!UICONTROL 下一個]**.
1. 按一下 **[!UICONTROL SAML登入]** 以建立連線並返回模組。

   或

   輸入您的使用者名稱和密碼，然後按一下 **[!UICONTROL 登入]** 以建立連線並返回模組。

   >[!NOTE]
   >
   >* 如果您沒有看到SAML登入按鈕，表示貴組織尚未啟用單一登入(SSO)。 您可以使用您的使用者名稱和密碼登入。
   >   
   >   如需有關SSO的詳細資訊，請參閱 [單一登入概觀 [!DNL Adobe Workfront]](../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)
   >   
   >* OAuth 2.0與的連線 [!DNL Workfront] API不再依賴API金鑰。

## [!DNL Workfront] 模組及其欄位

當您設定 [!DNL Workfront] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 除了這些以外， [!DNL Workfront] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應至中的另一個模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

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

模組會傳回與記錄相關聯的任何標準欄位，以及連線存取的任何自訂欄位和值。 您可以將此資訊對應到情境中的後續模組中。

1. 按一下 **[!UICONTROL 新增]** 右側 **Webhook** 方塊。

1. 在中設定webhook **[!UICONTROL 新增鉤點]** 方塊中顯示的方塊。

   當您設定此模組時，會顯示下列欄位。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[！UICONTROL Webhook名稱]</td> 
      <td>（選用）為webhook輸入新名稱</td> 
     </tr> 
     <tr> 
      <td>[！UICONTROL連線]</td> 
      <td> <p>如需有關連線您的電腦的指示， [!DNL Workfront] 應用程式至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
     </tr> 
     <tr> 
      <td>[！UICONTROL記錄型別]</td> 
      <td>選取型別 [!DNL Workfront] 錄製您想要模組觀看的影片。</td> 
     </tr> 
     <tr> 
      <td>[！UICONTROL狀態]</td> 
      <td>選取您要觀看舊狀態還是新狀態。<ul><li><p><b>[！UICONTROL新狀態]</b></p><p>記錄變更時觸發情境 <b>至</b> 指定值。</p><p>例如，如果狀態設為[！UICONTROL New State]，而篩選條件設為[！UICONTROL Status] [！UICONTROL Equals] [！UICONTROL In Progress]，則webhook會在[！UICONTROL Status]變更為[！UICONTROL In Progress]時觸發案例，無論狀態之前為何。 </p></li><li><p><b>[！UICONTROL舊狀態]</b></p><p>記錄變更時觸發情境 <b>從</b> 指定值。</p><p>例如，如果狀態設為[！UICONTROL Old State]，而篩選條件設為[！UICONTROL Status] [！UICONTROL Equals] [！UICONTROL In Progress]，webhook會在目前為[！UICONTROL Status]的[！UICONTROL In Progress]變更為其他狀態時觸發情境。 </p></li></ul></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td> <p>[！UICONTROL事件篩選器]</p> </td> 
      <td> <p>您可以設定篩選條件，以只監視符合您選取條件的記錄。</p> <p>對於每個篩選器，輸入您希望篩選器評估的欄位、運運算元，以及您希望篩選器允許的值。 您可以新增AND規則來使用多個篩選器。</p> <p>注意：您無法編輯現有篩選器中的篩選器 [!DNL Workfront] webhook。 若要為設定不同的篩選器 [!DNL Workfront] 事件訂閱，移除目前的webhook並建立新的訂閱。</p> <p>如需事件篩選器的詳細資訊，請參閱 <a href="#event-subscription-filters-in-the-workfront-watch-events-modules" class="MCXref xref">中的事件訂閱篩選器 [!DNL Workfront] &gt; [！UICONTROL觀看活動]模組</a> 本文章內容。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td>排除此連線造成的事件</td> 
      <td>啟用此選項可排除使用此觸發模組使用的相同聯結器建立或更新的事件。 這可防止案例可能自我觸發，導致其在無限回圈中重複的情況。</td> 
     </tr> 
     <tr> 
      <td>[！UICONTROL記錄來源]</td> 
      <td> <p>選擇是否要觀看情境 <strong>[！UICONTROL僅限新記錄]</strong>， <strong>[！UICONTROL僅更新記錄]</strong>， <strong>[！UICONTROL新記錄和更新的記錄]</strong>，或 <strong>[!DNL Deleted Records Only]</strong>.</p> <p>附註：如果您選擇 <strong>[！UICONTROL新記錄和更新的記錄]</strong>，webhook建立會建立2個事件訂閱（針對相同的webhook位址）。</p> </td> 
     </tr> 
    </tbody> 
   </table>

建立webhook後，您可以檢視事件傳送到的端點位址。

如需詳細資訊，請參閱區段 [事件裝載範例](../../wf-api/general/event-subs-api.md#examples-of-event-payloads) 在 [!DNL Workfront] 說明文章 [事件訂閱API](../../wf-api/general/event-subs-api.md).

檢視 [!DNL Workfront] 您可在其中使用此模組的物件型別 [[!DNL Workfront] object types available for each [!DNL Workfront] 模組](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL 觀看欄位]**

當您指定的欄位更新時，此觸發模組會執行案例。 模組會傳回您指定欄位的舊值和新值。 您可以將此資訊對應到情境中的後續模組中。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Workfront] 應用程式至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL記錄型別]</td> 
   <td> <p>選取型別 [!DNL Workfront] 錄製您希望模組觀看的影片。</p> <p>例如，如果您要在每次更新任務中的記錄欄位時開始執行案例，請選取[！UICONTROL任務]。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL欄位]</td> 
   <td>選取您希望模組監視更新的欄位。 這些欄位反映 [!DNL Workfront] 管理員已設定追蹤。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL輸出]</td> 
   <td>選取要包含在此模組輸出組合中的資訊。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL限制]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期內傳回的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>

檢視 [!DNL Workfront] 您可在其中使用此模組的物件型別 [[!DNL Workfront] object types available for each [!DNL Workfront] 模組](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL 觀看記錄]**

此觸發模組會在新增、更新或同時新增特定型別的物件時執行案例。 模組會傳回與一個或多個記錄關聯的所有標準欄位，以及連線存取的任何自訂欄位和值。 您可以將此資訊對應到情境中的後續模組中。 在輸出中，模組會指出每個記錄是新的還是更新的。

在指定時段新增和更新的記錄會以新記錄傳回。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Workfront] 應用程式至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL篩選器]</td> 
   <td> <p>選擇是否要觀看情境 <strong>[！UICONTROL僅限新記錄]</strong>， <strong>[！UICONTROL僅更新記錄]</strong>，或 <strong>[！UICONTROL新記錄和更新的記錄]</strong>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別]</td> 
   <td> <p>(在您選擇之後顯示 <strong>篩選</strong>.) 選取型別 [!DNL Workfront] 錄製您想要模組觀看的影片。</p> <p>例如，如果您要在每次建立新專案時啟動此案例，請選取[！UICONTROL專案]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸出]</td> 
   <td> <p>選取要包含在此模組輸出組合中的資訊。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇性篩選器]</td> 
   <td> <p>（進階）輸入API程式碼字串，以定義將縮小條件範圍的任何其他引數或程式碼。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期內傳回的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>

檢視 [!DNL Workfront] 您可在其中使用此模組的物件型別 [[!DNL Workfront] object types available for each [!DNL Workfront] 模組](#workfront-object-types-available-for-each-workfront-module).

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

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Workfront] 應用程式至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL物件型別]</td> 
   <td> <p>選取您要轉換的物件型別。 這是轉換前物件的型別。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL轉換為]</td> 
   <td>選取您要將其轉換為的物件。 這是物件在轉換後的型別。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL &lt;object&gt; ID]</td> 
   <td> <p>輸入物件的ID。 </p> <p>附註：輸入物件的識別碼時，您可以開始輸入物件的名稱，然後從清單中選取它。 模組接著在欄位中輸入適當的ID。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL範本ID]</td> 
   <td> <p>如果您要轉換為專案，請選取要用於專案的範本ID。</p> <p>附註：輸入物件的識別碼時，您可以開始輸入物件的名稱，然後從清單中選取它。 模組接著在欄位中輸入適當的ID。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL自訂表單]</td> 
   <td>選取您要新增至新轉換物件的任何自訂表單，然後輸入自訂表單欄位的值。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL選項]</td> 
   <td> <p>啟用轉換物件時所需的任何選項。 選項是否可用取決於您要將物件轉換為哪一個或哪一個物件。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 建立記錄（附加自訂表單）]**

此動作模組會建立物件，例如中的專案、任務或問題 [!DNL Workfront]，並可讓您將自訂表單新增至新物件。 模組可讓您選取可在模組中取得哪些物件欄位。

您指定記錄的ID。

模組會傳回記錄ID和任何關聯欄位，以及連線存取的任何自訂欄位和值。 您可以將此資訊對應到情境中的後續模組中。

例如，您可以使用此模組來建立任務 [!DNL Workfront] 當使用者端在中新增一列時 [!DNL Google Sheets] 需要完成的工作清單。

當您設定此模組時，會顯示下列欄位。

請務必提供最小輸入欄位數。 例如，如果您想要建立問題，則需要在「專案ID」欄位中提供有效的父專案ID，以指出問題應存在於Workfront中的哪個位置。 您可以使用對應面板從情境中的另一個模組對應此資訊，也可以輸入名稱，然後從清單中選取它，以手動輸入。

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Workfront] 應用程式至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL記錄型別]</td> 
   <td> <p>選取型別 [!DNL Workfront] 您要模組建立的記錄。</p> <p>例如，如果您想要建立專案，請從下拉式清單中選取[！UICONTROL專案]，然後確定您有權存取將填入專案的資料（來自案例中先前模組）。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL選取要對應的欄位]</td> 
   <td> <p>選取您想要可供資料輸入的欄位。 這可讓您使用這些欄位，而不必捲動瀏覽不需要的欄位。</p> <p>對於自訂表單中的欄位，請使用 <b>[！UICONTROL附加自訂表單]</b> 欄位。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL附加自訂表單]</td> 
   <td>選取您要新增至新物件的任何自訂表單，然後輸入這些欄位的值。</td> 
  </tr> 
 </tbody> 
</table>

檢視 [!DNL Workfront] 您可在其中使用此模組的物件型別 [[!DNL Workfront] object types available for each [!DNL Workfront] 模組](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* 輸入物件的ID時，您可以開始輸入物件的名稱，然後從清單中選取它。 模組接著在欄位中輸入適當的ID。
>* 輸入自訂欄位的文字或 [!UICONTROL 注意] HTML物件（註解或回覆），您可在 [!UICONTROL 附註文字] 欄位以建立RTF文字，例如粗體或斜體文字。
>
>  如需更新中RTF文字的詳細資訊，請參閱 [將更新新增至工作專案](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) 在 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
>

+++

+++ **[!UICONTROL 建立記錄]**

此動作模組會建立物件，例如Workfront中的專案、任務或問題。 模組可讓您選取可在模組中取得哪些物件欄位。

您指定記錄的ID。

模組會傳回記錄ID和任何關聯欄位，以及連線存取的任何自訂欄位和值。 您可以將此資訊對應到情境中的後續模組中。

例如，您可以使用此模組來建立任務 [!DNL Workfront] 當使用者端在Google工作表中新增需要完成的工作清單時。

當您設定此模組時，會顯示下列欄位。

請務必提供最小輸入欄位數。 例如，如果您想要建立問題，則需要在「專案ID」欄位中提供有效的父專案ID，以指出問題應存在於Workfront中的哪個位置。 您可以使用對應面板從情境中的另一個模組對應此資訊，也可以輸入名稱，然後從清單中選取它，以手動輸入。

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Workfront] 應用程式至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL記錄型別]</td> 
   <td> <p>選取型別 [!DNL Workfront] 您要模組建立的記錄。</p> <p>例如，如果您想要建立專案，請從下拉式清單中選取[！UICONTROL專案]，然後確定您有權存取將填入專案的資料（來自案例中先前模組）。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL選取要對應的欄位]</td> 
   <td>選取您想要可供資料輸入的欄位。 這可讓您使用這些欄位，而不必捲動瀏覽不需要的欄位。</td> 
  </tr> 
 </tbody> 
</table>

檢視 [!DNL Workfront] 您可在其中使用此模組的物件型別 [[!DNL Workfront] object types available for each [!DNL Workfront] 模組](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* 輸入物件的ID時，您可以開始輸入物件的名稱，然後從清單中選取它。 模組接著在欄位中輸入適當的ID。
>* 輸入自訂欄位的文字或 [!UICONTROL 注意] HTML物件（註解或回覆），您可在 [!UICONTROL 附註文字] 欄位以建立RTF文字，例如粗體或斜體文字。
>
>  如需更新中RTF文字的詳細資訊，請參閱 [將更新新增至工作專案](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) 在 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
>

+++

+++ **[!UICONTROL 自訂API呼叫]**

此動作模組可讓您對 [!DNL Workfront] API。 如此一來，您就可以建立其他人無法完成的資料流程自動化 [!DNL Workfront] 模組。

模組會傳回下列資訊：

* **[!UICONTROL 狀態代碼]** （數字）：這表示HTTP要求成功或失敗。 這些是您可在網際網路上查閱的標準程式碼。
* **[!UICONTROL 標頭]** （物件）：與輸出內文無關之回應/狀態代碼的更詳細內容。 並非所有顯示在回應標頭中的標頭都是回應標頭，因此某些標頭可能對您並無用處。

  回應標頭取決於您在設定模組時選擇的HTTP請求。

* **[!UICONTROL 內文]** （物件）：根據您在設定模組時選擇的HTTP請求，您可能會收到傳回的一些資料。 該資料(例如來自GET請求的資料)包含在此物件中。

您可以將此資訊對應到情境中的後續模組中。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Workfront] 應用程式至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p>輸入相對於<code> https://&lt;WORKFRONT_DOMAIN&gt;/attask/api/&lt;API_VERSION&gt;/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL API版本]</td> 
   <td>選取 [!DNL Workfront] 您希望模組使用的API。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL方法]</td> 
   td&gt; <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL標頭]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標頭。 這會決定請求的內容型別。</p> <p>例如，<code> {"Content-type":"application/json"}</code></p> <p>注意：如果您收到錯誤且難以判斷其來源，請考慮根據 [!DNL Workfront] 說明檔案。 如果您的自訂API呼叫傳回422 HTTP請求錯誤，請嘗試使用 <code>"Content-Type":"text/plain"</code> 標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查詢字串]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的查詢。</p> <p>例如： <code>{"name":"something-urgent"}</code></p> <p>提示：建議您透過JSON內文傳送資訊，而非查詢引數。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL內文]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的正文內容。</p> <p>備註:  <p>使用條件陳述式時，例如 <code>if</code> 在JSON中，將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

檢視 [!DNL Workfront] 您可在其中使用此模組的物件型別 [[!DNL Workfront] object types available for each [!DNL Workfront] 模組](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL 刪除記錄]**

此動作模組會刪除物件，例如Workfront中的專案、任務或問題。

您指定記錄的ID。

模組會傳回記錄ID和任何關聯欄位，以及連線存取的任何自訂欄位和值。 您可以將此資訊對應到情境中的後續模組中。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Workfront] 應用程式至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL強制刪除]</td> 
   <td>啟用此選項以確保刪除記錄，即使 [!DNL Workfront] UI會要求確認刪除。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>ID</td> 
   <td> <p>輸入唯一 [!DNL Workfront] 您要模組刪除的記錄ID。</p> <p>若要取得ID，請開啟 [!DNL Workfront] 物件，並複製URL結尾「ID=」後的文字。 例如： https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL記錄型別]</td> 
   <td>選取型別 [!DNL Workfront] 您要模組刪除的記錄。</td> 
  </tr> 
 </tbody> 
</table>

檢視 [!DNL Workfront] 您可在其中使用此模組的物件型別 [[!DNL Workfront] object types available for each [!DNL Workfront] 模組](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL 下載文件]**

此動作模組會從Workfront下載檔案。

您指定記錄的ID。

模組會傳回檔案的內容、檔案名稱、副檔名和檔案大小。 您可以將此資訊對應到情境中的後續模組中。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Workfront] 應用程式至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL檔案ID]</td> 
   <td> <p>對應或手動輸入唯一 [!DNL Workfront] 您希望模組下載的檔案ID。</p> <p>若要取得ID，請開啟 [!DNL Workfront] 物件，並複製URL結尾「ID=」後的文字。 例如： https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
 </tbody> 
</table>

檢視 [!DNL Workfront] 您可在其中使用此模組的物件型別 [[!DNL Workfront] object types available for each [!DNL Workfront] 模組](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL 其他動作]**

此動作模組可讓您對API執行動作。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Workfront] 應用程式至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL記錄型別]</td> 
   <td> <p>選取型別 [!DNL Workfront] 記錄您希望模組與之互動。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL動作]</td> 
   <td> <p>選取您希望模組執行的動作。</p> <p>視您選擇的[！UICONTROL記錄型別]和[！UICONTROL動作]而定，您可能需要填寫其他欄位。 這兩個設定的某些組合可能只需要記錄ID，而其他設定(例如的Project <strong>[！UICONTROL記錄型別]</strong> 和[！UICONTROL附加範本] <strong>[！UICONTROL動作]</strong>)需要其他資訊（例如物件ID和範本ID）。</p> <p>如需個別欄位的詳細資訊，請參閱 <a href="http://developer.workfront.com/">Workfront開發人員檔案</a>. </p> 
    <ol> 
     <li value="1"> <p>從左側導覽選擇記錄型別 [!DNL Workfront] 開發人員檔案頁面。 下列型別有自己的頁面：</p> 
      <ul> 
       <li> <p>[！UICONTROL專案]</p> </li> 
       <li> <p>[！UICONTROL工作]</p> </li> 
       <li> <p>[！UICONTROL問題]</p> </li> 
       <li> <p>[！UICONTROL使用者]</p> </li> 
       <li> <p>[！UICONTROL檔案]</p> </li> 
      </ul> <p>對於所有其他記錄型別，請選取 <b>[！UICONTROL其他物件和端點]</b>，並在依字母順序排序的頁面上找到記錄型別。</p> </li> 
     <li value="2"> <p>在適當記錄型別的頁面上，搜尋動作（Ctrl-F或Cmd-F）。</p> </li> 
     <li value="3"> <p>檢視所選動作下可用欄位的說明。</p> </li> 
    </ol> <p>備註:  <p>透過建立校訂時 [!DNL Workfront] [！UICONTROL雜湊動作]模組，最佳實務是在沒有任何進階選項的情況下建立校訂，然後使用 [!DNL Workfront Proof] SOAP API。</p> <p>如需有關使用建立校訂的詳細資訊 [!DNL Workfront] API （此模組使用此API），請參閱 <a href="../../wf-api/tips-tricks-and-troubleshooting/api-create-proof-options-json.md" class="MCXref xref">透過建立校訂時新增進階校訂選項 [!DNL Adobe Workfront] API</a></p> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL ID]</td> 
   <td>輸入或對映唯一的 [!DNL Workfront] 您希望模組與之互動的記錄ID。<p>若要取得ID，請開啟 [!DNL Workfront] 物件，並複製URL結尾「ID=」後的文字。 例如： https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p></td> 
  </tr> 
 </tbody> 
</table>

檢視 [!DNL Workfront] 您可在其中使用此模組的物件型別 [[!DNL Workfront] object types available for each [!DNL Workfront] 模組](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL 讀取記錄]**

此動作模組會從單一記錄擷取資料。

您指定記錄的ID。 您也可以指定您希望模組讀取哪些相關記錄。

例如，如果模組正在讀取的記錄是專案，您可以指定您希望專案的任務讀取。

模組會針對您指定的輸出，從標準欄位傳回資料陣列。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[！UICONTROL連線]</td>

<td> <p>如需有關連線您的電腦的指示， [!DNL Workfront] 應用程式至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
    <td>[！UICONTROL記錄型別]</td>

<td>選擇 [!DNL Workfront] 您希望模組讀取的物件型別。</td> 
  </tr> 
  <tr> 
    <td>[！UICONTROL輸出]</td>

<td> <p>選取要包含在此模組輸出組合中的資訊。</p> </td> 
  </tr> 
  <tr> 
    <td>[！UICONTROL參考]</td>
   <td>選取您要包含在輸出中的任何參考欄位。</td> 
  </tr> 
  <tr> 
    <td>[！UICONTROL集合]</td>
   <td>選取您要包含在輸出中的任何參考欄位。</td> 
  </tr> 
  <tr> 
    <td>[！UICONTROL ID]</td>
   <td> <p>輸入唯一 [!DNL Workfront] 您希望模組讀取的記錄ID。</p> <p>若要取得ID，請開啟 [!DNL Workfront] 物件，並複製URL結尾「ID=」後的文字。 例如： https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
 </tbody> 
</table>

檢視 [!DNL Workfront] 您可在其中使用此模組的物件型別 [[!DNL Workfront] object types available for each [!DNL Workfront] 模組](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL 更新記錄]**

此動作模組會更新物件，例如專案、任務或問題。 模組可讓您選取可在模組中取得哪些物件欄位。

您指定記錄的ID。

模組會傳回物件的ID和任何關聯欄位，以及連線存取的任何自訂欄位和值。 您可以將此資訊對應到情境中的後續模組中。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Workfront] 應用程式至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL ID]</td> 
   <td> <p>輸入唯一 [!DNL Workfront] 您要模組更新的記錄ID。</p> <p>若要取得ID，請開啟 [!DNL Workfront] 物件，並複製URL結尾「ID=」後的文字。 例如： https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Record Type]</td> 
   <td> <p>選取型別 [!DNL Workfront] 記錄您希望模組更新的內容。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!DNL Select fields to map]</td> 
   <td>選取您想要可供資料輸入的欄位。 這可讓您使用這些欄位，而不必捲動瀏覽不需要的欄位。</td> 
  </tr> 
 </tbody> 
</table>

檢視 [!DNL Workfront] 您可在其中使用此模組的物件型別 [[!DNL Workfront] object types available for each [!DNL Workfront] 模組](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* 輸入物件的ID時，您可以開始輸入物件的名稱，然後從清單中選取它。 模組接著在欄位中輸入適當的ID。
>* 輸入自訂欄位的文字或 [!UICONTROL 注意] HTML物件（註解或回覆），您可在 [!UICONTROL 附註文字] 欄位以建立RTF文字，例如粗體或斜體文字。
>
>  如需更新中RTF文字的詳細資訊，請參閱 [將更新新增至工作專案](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) 在 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
>

+++

+++ **[!UICONTROL 上傳檔案]**

此動作模組會將檔案上傳至 [!DNL Workfront] 物件，例如專案、任務或問題。

您可以指定檔案的位置、要上傳的檔案，以及檔案的可選新名稱。

模組會傳回檔案ID和任何關聯欄位，以及連線存取的任何自訂欄位和值。 您可以將此資訊對應到情境中的後續模組中。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Workfront] 應用程式至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL相關記錄ID]</td> 
   <td>輸入唯一 [!DNL Workfront] 您要上傳檔案的記錄ID。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL相關記錄型別]</td> 
   <td>選取型別 [!DNL Workfront] 紀錄您希望模組上傳檔案的位置。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL來源檔案]</td> 
   <td> <p>從先前的模組中選取來源檔案，或對應來源檔案的名稱和資料。</p> </td> 
  </tr> 
 </tbody> 
</table>

檢視 [!DNL Workfront] 您可在其中使用此模組的物件型別 [[!DNL Workfront] object types available for each [!DNL Workfront] 模組](#workfront-object-types-available-for-each-workfront-module).

+++

### 搜尋

<!--
* [Read Related Records](#read-related-records) 
* [Search](#search)
-->

+++ **[!UICONTROL 讀取相關記錄]**

此搜尋模組會讀取符合您指定之搜尋查詢的記錄（在特定父物件中）。

您可以指定要包含在輸出中的欄位。 您可以將此資訊對應到情境中的後續模組中。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Workfront] 應用程式至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL記錄型別]</td> 
   <td> <p>選取您要讀取其關聯記錄的父記錄型別(Workfront物件)。</p> <p>檢視 [!DNL Workfront] 您可在其中使用此模組的物件型別 <a href="#object-types-available-for-each-workfront-search-module" class="MCXref xref">[!DNL Workfront] 每個專案可用的物件型別 [!DNL Workfront] 模組</a> 本文章內容。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL父記錄ID]</td> 
   <td> <p>輸入或對應您要讀取其關聯記錄的父記錄ID。</p> <p>若要取得ID，請開啟 [!DNL Workfront] 物件，並複製URL結尾「ID=」後的文字。 例如： https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
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

此搜尋模組會在中尋找物件中的記錄 [!DNL Workfront] 符合您指定的搜尋查詢。

您可以將此資訊對應到情境中的後續模組中。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Workfront] 應用程式至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL記錄型別]</td> 
   <td> <p>選取型別 [!DNL Workfront] 您要模組搜尋的記錄。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL結果集]</td> 
   <td>選取一個選項，以指定您希望模組取得符合您搜尋條件的第一個結果，還是所有符合該條件的結果。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Maximal]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期內傳回的最大記錄數。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL搜尋條件]</td> 
   <td> <p>輸入您要搜尋的欄位、要在查詢中使用的運運算元，以及要在欄位中搜尋的值。</p> <p>注意：請勿使用 <code>username </code>在您的搜尋條件中。 包含 <code>username </code>在API查詢中 [!DNL Workfront] 將使用者登入Workfront，搜尋將不會成功。</p> <p>注意： <code>In</code> 和 <code>NotIn</code>使用陣列。 輸入的格式應為陣列。</p></td> 
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

檢視 [!DNL Workfront] 您可在其中使用此模組的物件型別 [[!DNL Workfront] object types available for each [!DNL Workfront] 模組](#workfront-object-types-available-for-each-workfront-module).

+++

## [!DNL Workfront] 每個專案可用的物件型別 [!DNL Workfront] 模組

<!-- [Object types available for each Workfront trigger module](#object-types-available-for-each-workfront-trigger-module) 
* [Object types available for each Workfront action module](#object-types-available-for-each-workfront-action-module) 
* [Object types available for each Workfront search module](#object-types-available-for-each-workfront-search-module)-->

+++**每個專案可用的物件型別 [!DNL Workfront] 觸發模組**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>[！UICONTROL觀看記錄]</th> 
   <th>[！UICONTROL監看欄位]</th> 
   <th>[！UICONTROL觀看活動]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>核准流程</td> 
   <td> </td> 
   <td>✓ (N)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>指派</td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>基準線</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> 付費記錄 </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>帳單費率</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>公司</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>儀表板</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>文件</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>文件資料夾</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>文件要求</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>文件版本</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>費用</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>費用類型</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>群組</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>時數</td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>時數類型</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>問題</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>反覆項目</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>職務角色</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>日誌輸入項目</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>里程碑</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>里程碑路徑</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>備註</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>附註標籤</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>專案組合</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>方案</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>專案</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>專案使用者</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>保留時間* </td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>報告</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
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
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>任務</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>團隊</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>範本</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>範本任務</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>時程表</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>使用者</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
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

+++**每個專案可用的物件型別 [!DNL Workfront] 動作模組**

>[!NOTE]
>
>此 [!UICONTROL 下載檔案] 此表格中未包含模組，因為 [!DNL Workfront] 物件型別不屬於其設定。

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
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>指派</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>付費記錄</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>帳單費率</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>公司</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>文件</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>文件資料夾</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>文件版本</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>費用</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>費用類型</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>群組</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>時數</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>時數類型</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>問題</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>反覆項目</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>職務角色</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>日誌輸入項目</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>里程碑</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>里程碑路徑</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>備註</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>附註標籤</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>專案組合</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>方案</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>專案</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>專案使用者</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>保留時間* </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>風險</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>風險類型</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>步驟核准者</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>任務</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>團隊</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>範本</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>範本任務</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>時程表</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>使用者</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>更新</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**每個專案可用的物件型別 [!DNL Workfront] 搜尋模組**

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
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>指派</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>付費記錄</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>帳單費率</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>公司</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>文件</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>文件資料夾</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>文件版本</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>費用</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>費用類型</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>群組</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>時數</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>時數類型</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>問題</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>反覆項目</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>職務角色</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>日誌輸入項目</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>里程碑</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>里程碑路徑</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>備註</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>附註標籤</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>專案組合</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>方案</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>專案</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>專案使用者</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>保留時間* </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>風險</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>風險類型</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>步驟核准者</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>任務</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>團隊</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>範本</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>範本任務</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>時程表</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>使用者</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>使用者委派</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

建議您仔細檢查，確保此功能的運作方式與預期一致。

+++

## 中的事件訂閱篩選器 [!DNL Workfront] > [!UICONTROL 觀看活動] 模組

>[!NOTE]
>
>強烈建議您在中使用事件訂閱篩選器 [!UICONTROL 觀看活動] 模組。

此 [!DNL Workfront] [!UICONTROL 觀看活動] 模組會根據webhook觸發案例，該案例會在 [!DNL Workfront] API。 事件訂閱是一組資料，可決定要將哪些事件傳送到webhook。 例如，如果您設定 [!UICONTROL 觀看活動] 監視問題的模組，則事件訂閱只會傳送與問題相關的事件。

透過使用事件訂閱篩選器，Fusion使用者可建立更適合其使用案例的事件訂閱。 例如，您可以在 [!DNL Workfront] API僅將特定專案中的問題傳送至webhook，確保 [!UICONTROL 觀看活動] 模組將只會為該專案中的問題觸發。 建立較窄觸發器的功能可減少不相關觸發器的數量，進而改善情境設計。

這與在中設定篩選器不同 [!DNL Workfront Fusion] 情境。 若沒有事件訂閱篩選器，您的webhook會接收與您選取的物件型別相關的所有事件。 這些事件大多與情境無關，必須篩選掉，情境才能繼續。

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
   * 使用時 `Changed`，選取 **僅更新事件** 在 **記錄來源** 欄位。

>[!IMPORTANT]
>
>您無法編輯現有篩選器中的篩選器 [!DNL Workfront] webhook。 若要為設定不同的篩選器 [!DNL Workfront] 事件訂閱，移除目前的webhook並建立新的訂閱。

>[!INFO]
>
>**範例：** 請考量處理指派給特定使用者Ana之新問題的情境。
>
>### 使用事件訂閱篩選條件來篩選事件（建議使用）
>
>使用事件篩選器，您可以設定webhook以在建立問題時將問題指派給Ana時觸發情境。 Ana具有userID b378489d8f7cd3cee0539260720a84b7。
>
>![](assets/event-filter-watch-events-350x277.png)
>
>如果一天內建立100個問題，但只有兩個問題指派給Ana，則案例會執行兩次。
>
>### 篩選案例中的事件（不建議）
>
>若要篩選事件，以便只處理指派給Ana的問題，您可以在 [!UICONTROL 觀看活動] 模組。
>
>![](assets/watch-events-non-event-filter-350x206.png)
>
>如果一天內建立100個問題，但只有兩個問題指派給Ana，則案例將執行100次。 98個執行會在篩選後停止，但觸發模組仍在使用所有執行的資料並執行操作。

如需事件訂閱的詳細資訊，請參閱 [常見問題集 — 事件訂閱](../../wf-api/general/event-subs-faq.md).

如需Webhook的詳細資訊，請參閱 [中的即時觸發器(Webhook) [!DNL Adobe Workfront Fusion]](../../workfront-fusion/webhooks/instant-triggers-webhooks.md)

如需情境中篩選器的詳細資訊，請參閱 [將篩選器新增至中的情境 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).
