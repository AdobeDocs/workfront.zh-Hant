---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 連接器
navigation-topic: apps-and-their-modules
title: Adobe Workfront模組
description: 您可以使用Adobe Workfront Fusion Adobe Workfront連接器，將Workfront中的程式自動化。 如果您有Workfront Fusion for Work Automation and Integration授權，也可以用它來連接第三方應用程式和服務。
author: Becky
feature: Workfront Fusion, Workfront Integrations and Apps
exl-id: b84d2d41-a983-4ea3-b331-0302bfcf8a2b
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '5276'
ht-degree: 3%

---

# [!DNL Adobe Workfront] 模組

您可以使用 [!DNL Adobe Workfront Fusion] [!DNL Adobe Workfront] 連接器可在 [!DNL Workfront]. 如果您有 [!UICONTROL [!DNL Workfront Fusion] 工作自動化和整合] 授權，您也可以用它來連線至協力廠商應用程式和服務。

此 [!DNL Workfront] 連接器不會計入貴組織可用的作用中應用程式數量。 所有情況，即使它們僅使用 [!DNL Workfront] 應用程式時，請確實計入貴組織的案例總數。

如需貴組織可用應用程式和案例的詳細資訊，請參閱 [組織](../../workfront-fusion/organizations/organizations-and-teams.md#organiza2) in [[!DNL Adobe Workfront Fusion] 組織和團隊](../../workfront-fusion/organizations/organizations-and-teams.md).

如果您需要建立案例的相關指示，請參閱 [在中建立案例 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). 如需模組的相關資訊，請參閱 [中的模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## 存取需求

您必須具備下列存取權才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td>
  <td> <p>[!UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td>
   <td> <p>[!UICONTROL計畫]、[!UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 許可**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p>  <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化）</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>


若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Connect [!DNL Workfront] to [!DNL Workfront Fusion]

此 [!DNL Workfront] 連接器使用OAuth 2.0連線至 [!DNL Workfront].

您可以建立與 [!DNL Workfront] 直接從內部 [!DNL Workfront Fusion] 模組。

1. 在任何 [!DNL Workfront] 應用程式模組，按一下 **[!UICONTROL 新增]** 旁邊 [!UICONTROL 連線] 框。
1. 在URL中輸入執行個體的名稱。 範例: `https://<your instance>.my.workfront.com`.
1. 按一下 **[!UICONTROL 下一個]**.
1. 按一下 **[!UICONTROL SAML登入]** 若要建立連線，請返回模組。

   或

   輸入您的使用者名稱和密碼，然後按一下 **[!UICONTROL 登入]** 若要建立連線，請返回模組。

   >[!NOTE]
   >
   >* 如果您沒有看見SAML登入按鈕，表示您的組織尚未啟用單一登入(SSO)。 您可以使用您的使用者名稱和密碼登入。
      >   
      >   如需SSO的詳細資訊，請參閱 [單一登入概觀 [!DNL Adobe Workfront]](../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)
   >   
   >* OAuth 2.0與 [!DNL Workfront] API不再依賴API金鑰。


## [!DNL Workfront] 模組及其欄位

設定時 [!DNL Workfront] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!DNL Workfront] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

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

+++ **[!UICONTROL 觀看事件]**

在Workfront中新增、更新或刪除特定類型的物件時，此觸發程式模組會即時執行案例

模組會傳回與記錄相關聯的任何標準欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

1. 按一下 **[!UICONTROL 新增]** 至 **Webhook** 框。

1. 在 **[!UICONTROL 添加掛接]** 框。

   設定此模組時，會顯示下列欄位。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Webhook名稱]</td> 
      <td>（可選）為網頁鈎點輸入新名稱</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL連接]</td> 
      <td> <p>有關連接 [!DNL Workfront] 應用程式至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL記錄類型]</td> 
      <td>選取 [!DNL Workfront] 記錄您要讓模組觀看的項目。</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL狀態]</td> 
      <td>選取您要觀看舊狀態還是新狀態。<ul><li><p><b>[!UICONTROL新狀態]</b></p><p>記錄變更時觸發情境 <b>to</b> 指定值。</p><p>例如，如果狀態設定為[!UICONTROL新狀態]，而篩選器設定為[!UICONTROL狀態] [!UICONTROL等於] [!UICONTROL正在進行中]，則無論以前的狀態為何，當[!UICONTROL狀態]更改為[!UICONTROL正在進行中]時，Webhook都會觸發情境。 </p></li><li><p><b>[!UICONTROL舊狀態]</b></p><p>記錄變更時觸發情境 <b>從</b> 指定值。</p><p>例如，如果狀態設定為[!UICONTROL舊狀態]，而篩選器設定為[!UICONTROL狀態] [!UICONTROL等於] [!UICONTROL正在進行中]，則當當前為[!UICONTROL正在進行中]的[!UICONTROL狀態]更改為其他狀態時，Webhook將觸發情境。 </p></li></ul></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td> <p>[!UICONTROL事件篩選器]</p> </td> 
      <td> <p>您可以設定篩選條件，僅監視符合您選取之條件的記錄。</p> <p>對於每個篩選器，輸入您要篩選器評估的欄位、運算子，以及您希望篩選器允許的值。 您可以新增AND規則，以使用多個篩選器。</p> <p>注意：您無法編輯現有的篩選器 [!DNL Workfront] 網頁鈎點。 為設定不同的篩選器 [!DNL Workfront] 事件訂閱、移除目前的webhook並建立新網頁。</p> <p>如需事件篩選器的詳細資訊，請參閱 <a href="#event-subscription-filters-in-the-workfront-watch-events-modules" class="MCXref xref">中的事件訂閱篩選器 [!DNL Workfront] &gt; [!UICONTROL監看事件]模組</a> 這篇文章。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td>排除此連線發生的事件</td> 
      <td>啟用此選項，可排除使用此觸發器模組所使用的相同連接器所建立或更新的事件。 這可防止情境可能自行觸發的情況，導致其在無盡的回圈中重複。</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL記錄來源]</td> 
      <td> <p>選擇是否要監視方案 <strong>[!UICONTROL僅新記錄]</strong>, <strong>[!UICONTROL僅更新記錄]</strong>, <strong>[!UICONTROL新記錄和更新記錄]</strong>，或 <strong>[!DNL Deleted Records Only]</strong>.</p> <p>注意：如果您選擇 <strong>[!UICONTROL新記錄和更新記錄]</strong>,webhook建立會建立2個事件訂閱（針對相同的webhook位址）。</p> </td> 
     </tr> 
    </tbody> 
   </table>

建立Webhook後，您可以檢視事件所要傳送到之端點的位址。

如需詳細資訊，請參閱 [事件裝載範例](../../wf-api/general/event-subs-api.md#examples-of-event-payloads) 在 [!DNL Workfront] 說明文章 [事件訂閱API](../../wf-api/general/event-subs-api.md).

查看 [!DNL Workfront] 您可以在 [[!DNL Workfront] object types available for each [!DNL Workfront] 模組](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL 監視欄位]**

此觸發器模組會在您指定的欄位更新時執行案例。 模組會同時傳回您指定欄位的舊值和新值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Workfront] 應用程式至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL記錄類型]</td> 
   <td> <p>選取 [!DNL Workfront] 記錄您要讓模組觀看的項目。</p> <p>例如，如果要在每次任務中更新記錄欄位時開始執行方案，請選擇[!UICONTROL任務]。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL欄位]</td> 
   <td>選取您要讓模組監看更新的欄位。 這些欄位會反映您 [!DNL Workfront] 管理員已設定用於追蹤。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL輸出]</td> 
   <td>選擇要包含在此模組的輸出包中的資訊。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL限制]</td> 
   <td> <p>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>

查看 [!DNL Workfront] 您可以在 [[!DNL Workfront] object types available for each [!DNL Workfront] 模組](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL 監視記錄]**

當添加、更新或同時添加特定類型的對象時，此觸發器模組將執行一個方案。 模組會傳回與記錄或記錄相關聯的所有標準欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。 在輸出中，模組指示每個記錄是新記錄還是更新記錄。

在指定時段內新增和更新的記錄會以新記錄的形式傳回。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Workfront] 應用程式至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL篩選器]</td> 
   <td> <p>選擇是否要監視方案 <strong>[!UICONTROL僅新記錄]</strong>, <strong>[!UICONTROL僅更新記錄]</strong>，或 <strong>[!UICONTROL新記錄和更新記錄]</strong>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL記錄類型]</td> 
   <td> <p>(在您選擇 <strong>篩選</strong>.) 選取 [!DNL Workfront] 記錄您要讓模組觀看的項目。</p> <p>例如，如果您想在每次建立新專案時啟動案例，請選取[!UICONTROL專案]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸出]</td> 
   <td> <p>選擇要包含在此模組的輸出包中的資訊。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL可選篩選器]</td> 
   <td> <p>（進階）輸入API程式碼字串，以定義將調整您條件的任何其他參數或程式碼。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>

查看 [!DNL Workfront] 您可以在 [[!DNL Workfront] object types available for each [!DNL Workfront] 模組](#workfront-object-types-available-for-each-workfront-module).

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

此動作模組會進行下列其中一次轉換：

* 將問題轉換為專案
* 將問題轉換為任務
* 將任務轉換為項目

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Workfront] 應用程式至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL對象類型]</td> 
   <td> <p>選擇要轉換的對象類型。 這是物件在轉換前的類型。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL轉換為]</td> 
   <td>選擇要轉換為的對象。 這是物件在轉換後擁有的類型。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL &lt;object&gt; ID]</td> 
   <td> <p>輸入物件的ID。 </p> <p>注意：輸入對象的ID時，可以開始鍵入對象的名稱，然後從清單中選擇該名稱。 然後，模組在欄位中輸入適當的ID。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL模板ID]</td> 
   <td> <p>如果要轉換為專案，請選取您要用於專案的範本ID。</p> <p>注意：輸入對象的ID時，可以開始鍵入對象的名稱，然後從清單中選擇該名稱。 然後，模組在欄位中輸入適當的ID。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL自訂表單]</td> 
   <td>選擇要添加到新轉換對象的任何自定義表單，然後輸入自定義表單欄位的值。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL選項]</td> 
   <td> <p>在轉換物件時啟用您想要的任何選項。 視您要轉換為或從哪個物件而定，可供使用選項。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 建立記錄（附加自訂表單）]**

此動作模組會建立物件，例如專案、任務或 [!DNL Workfront]，可讓您將自訂表單新增至新物件。 模組可讓您選取模組中可用的物件欄位。

您指定記錄的ID。

模組會傳回記錄和任何相關欄位的ID，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

例如，您可以使用此模組，在 [!DNL Workfront] 當客戶端在 [!DNL Google Sheets] 需要完成的任務清單。

設定此模組時，會顯示下列欄位。

請務必提供最少的輸入欄位數。 例如，如果您想要建立問題，您必須在「專案ID」欄位中提供有效的上層專案ID，以指出問題應在Workfront中的哪個位置存在。 您可以使用映射面板來映射方案中其他模組的此資訊，或者通過鍵入名稱，然後從清單中選擇該資訊來手動輸入。

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Workfront] 應用程式至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL記錄類型]</td> 
   <td> <p>選取 [!DNL Workfront] 記錄您要建立模組。</p> <p>例如，如果要建立專案，請從下拉式清單中選取[!UICONTROL專案]，然後確定您擁有將填入專案的資料（來自案例中的先前模組）存取權。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL選擇要映射的欄位]</td> 
   <td> <p>選取您要供資料輸入使用的欄位。 這可讓您使用這些欄位，而無須捲動查看您不需要的欄位。</p> <p>對於自訂表單中的欄位，請使用 <b>[!UICONTROL附加自定義表單]</b> 欄位。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL附加自定義表單]</td> 
   <td>選擇要添加到新對象的任何自定義表單，然後為這些欄位輸入值。</td> 
  </tr> 
 </tbody> 
</table>

查看 [!DNL Workfront] 您可以在 [[!DNL Workfront] object types available for each [!DNL Workfront] 模組](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* 輸入對象的ID時，可以開始鍵入對象的名稱，然後從清單中選擇該名稱。 然後，模組在欄位中輸入適當的ID。
>* 輸入自訂欄位或 [!UICONTROL 附註] 物件（註解或回覆），您可以在 [!UICONTROL 附註文字] 欄位來建立RTF文字，例如粗體或斜體文字。
>
>  如需更新中RTF的詳細資訊，請參閱 [向工作項添加更新](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) in [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

+++

+++ **[!UICONTROL 建立記錄]**

此動作模組會建立物件，例如Workfront中的專案、任務或問題。 模組可讓您選取模組中可用的物件欄位。

您指定記錄的ID。

模組會傳回記錄和任何相關欄位的ID，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

例如，您可以使用此模組，在 [!DNL Workfront] 當用戶端在Google工作表中新增需要執行之工作的列時。

設定此模組時，會顯示下列欄位。

請務必提供最少的輸入欄位數。 例如，如果您想要建立問題，您必須在「專案ID」欄位中提供有效的上層專案ID，以指出問題應在Workfront中的哪個位置存在。 您可以使用映射面板來映射方案中其他模組的此資訊，或者通過鍵入名稱，然後從清單中選擇該資訊來手動輸入。

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Workfront] 應用程式至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL記錄類型]</td> 
   <td> <p>選取 [!DNL Workfront] 記錄您要建立模組。</p> <p>例如，如果要建立專案，請從下拉式清單中選取[!UICONTROL專案]，然後確定您擁有將填入專案的資料（來自案例中的先前模組）存取權。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL選擇要映射的欄位]</td> 
   <td>選取您要供資料輸入使用的欄位。 這可讓您使用這些欄位，而無須捲動查看您不需要的欄位。</td> 
  </tr> 
 </tbody> 
</table>

查看 [!DNL Workfront] 您可以在 [[!DNL Workfront] object types available for each [!DNL Workfront] 模組](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* 輸入對象的ID時，可以開始鍵入對象的名稱，然後從清單中選擇該名稱。 然後，模組在欄位中輸入適當的ID。
>* 輸入自訂欄位或 [!UICONTROL 附註] 物件（註解或回覆），您可以在 [!UICONTROL 附註文字] 欄位來建立RTF文字，例如粗體或斜體文字。
>
>  如需更新中RTF的詳細資訊，請參閱 [向工作項添加更新](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) in [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

+++

+++ **[!UICONTROL 自訂API呼叫]**

此動作模組可讓您對 [!DNL Workfront] API。 這樣，您就可以建立資料流自動化，而另一個無法完成 [!DNL Workfront] 模組。

模組會傳回下列資訊：

* **[!UICONTROL 狀態代碼]** （數字）:這表示HTTP要求是否成功。 這些是標準代碼，你可以在網際網路上查找。
* **[!UICONTROL 標題]** （對象）:與輸出內文無關之回應/狀態代碼的更詳細內容。 並非所有顯示在回應標題中的標題都是回應標題，因此有些標題可能對您沒有用。

   回應標題取決於您在設定模組時選擇的HTTP要求。

* **[!UICONTROL 主體]** （對象）:根據您在設定模組時選擇的HTTP要求，您可能會收到一些資料。 該資料(例如來自GET請求的資料)包含在此物件中。

您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Workfront] 應用程式至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p>輸入相對於的路徑<code> https://&lt;WORKFRONT_DOMAIN&gt;/attask/api/&lt;API_VERSION&gt;/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL API版本]</td> 
   <td>選取 [!DNL Workfront] 您要讓模組使用的API。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL方法]</td> 
   td&gt; <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL標題]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標題。 這會決定請求的內容類型。</p> <p>例如，<code> {"Content-type":"application/json"}</code></p> <p>注意：如果您收到錯誤，且很難判斷其來源，請考慮根據 [!DNL Workfront] 檔案。 如果您的自訂API呼叫傳回422 HTTP要求錯誤，請嘗試使用 <code>"Content-Type":"text/plain"</code> 頁首。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL查詢字串]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的查詢。</p> <p>例如： <code>{"name":"something-urgent"}</code></p> <p>提示：建議您透過JSON內文傳送資訊，而非以查詢參數的形式傳送。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL正文]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的內文內容。</p> <p>備註:  <p>使用條件陳述式時，例如 <code>if</code> 在JSON中，將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

查看 [!DNL Workfront] 您可以在 [[!DNL Workfront] object types available for each [!DNL Workfront] 模組](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL 刪除記錄]**

此動作模組會刪除物件，例如Workfront中的專案、任務或問題。

您指定記錄的ID。

模組會傳回記錄和任何相關欄位的ID，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Workfront] 應用程式至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL強制刪除]</td> 
   <td>啟用此選項可確保刪除記錄，即使 [!DNL Workfront] UI會要求確認刪除。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>ID</td> 
   <td> <p>輸入唯一 [!DNL Workfront] 您要刪除模組的記錄ID。</p> <p>若要取得ID，請開啟 [!DNL Workfront] 物件，並複製URL結尾"ID="之後的文字。 例如：https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL記錄類型]</td> 
   <td>選取 [!DNL Workfront] 記錄您要刪除模組。</td> 
  </tr> 
 </tbody> 
</table>

查看 [!DNL Workfront] 您可以在 [[!DNL Workfront] object types available for each [!DNL Workfront] 模組](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL 下載文件]**

此動作模組會從Workfront下載檔案。

您指定記錄的ID。

模組會傳回檔案的內容、檔案名稱、副檔名和檔案大小。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Workfront] 應用程式至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文檔ID]</td> 
   <td> <p>映射或手動輸入唯一 [!DNL Workfront] 要下載模組的文檔ID。</p> <p>若要取得ID，請開啟 [!DNL Workfront] 物件，並複製URL結尾"ID="之後的文字。 例如：https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
 </tbody> 
</table>

查看 [!DNL Workfront] 您可以在 [[!DNL Workfront] object types available for each [!DNL Workfront] 模組](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL 雜項活動]**

此動作模組可讓您對API執行動作。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Workfront] 應用程式至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL記錄類型]</td> 
   <td> <p>選取 [!DNL Workfront] 記錄您要模組與之互動的項目。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL操作]</td> 
   <td> <p>選取您要模組執行的動作。</p> <p>您可能需要根據您選擇的[!UICONTROL記錄類型]和[!UICONTROL操作]填寫其他欄位。 這兩個設定的某些組合可能只需要記錄ID，而其他組合(例如 <strong>[!UICONTROL記錄類型]</strong> 和適用於 <strong>[!UICONTROL操作]</strong>)需要其他資訊（例如物件ID和範本ID）。</p> <p>如需個別欄位的詳細資訊，請參閱 <a href="http://developer.workfront.com/">Workfront開發人員檔案</a>. </p> 
    <ol> 
     <li value="1"> <p>從的左側導覽中選取記錄類型 [!DNL Workfront] 開發人員檔案頁面。 下列類型有其專屬的頁面：</p> 
      <ul> 
       <li> <p>[!UICONTROL項目]</p> </li> 
       <li> <p>[!UICONTROL任務]</p> </li> 
       <li> <p>[!UICONTROL問題]</p> </li> 
       <li> <p>[!UICONTROL用戶]</p> </li> 
       <li> <p>[!UICONTROL文檔]</p> </li> 
      </ul> <p>對於所有其他記錄類型，請選擇 <b>[!UICONTROL其他對象和端點]</b>，然後在依字母順序排序的頁面上找到記錄類型。</p> </li> 
     <li value="2"> <p>在適當記錄類型的頁面上，搜尋（Ctrl-F或Cmd-F）動作。</p> </li> 
     <li value="3"> <p>查看所選操作下可用欄位的說明。</p> </li> 
    </ol> <p>備註:  <p>透過建立校樣時 [!DNL Workfront] [!UICONTROL雜項操作]模組，最佳做法是建立沒有任何高級選項的校樣，然後使用 [!DNL Workfront Proof] SOAP API。</p> <p>如需使用建立校樣的詳細資訊 [!DNL Workfront] API（此模組使用的），請參閱 <a href="../../wf-api/tips-tricks-and-troubleshooting/api-create-proof-options-json.md" class="MCXref xref">透過建立校樣時，新增進階校樣選項 [!DNL Adobe Workfront] API</a></p> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID]</td> 
   <td>輸入或對應唯一 [!DNL Workfront] 您要模組與之互動的記錄ID。<p>若要取得ID，請開啟 [!DNL Workfront] 物件，並複製URL結尾"ID="之後的文字。 例如：https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p></td> 
  </tr> 
 </tbody> 
</table>

查看 [!DNL Workfront] 您可以在 [[!DNL Workfront] object types available for each [!DNL Workfront] 模組](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL 閱讀記錄]**

此動作模組會從單一記錄中擷取資料。

您指定記錄的ID。 您也可以指定想要模組讀取的相關記錄。

例如，如果模組正在讀取的記錄是項目，則可以指定要讀取項目的任務。

模組會從您指定輸出的標準欄位傳回資料陣列。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL連接]</td>

<td> <p>有關連接 [!DNL Workfront] 應用程式至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL記錄類型]</td>

<td>選擇 [!DNL Workfront] 您要模組讀取的物件類型。</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL輸出]</td>

<td> <p>選擇要包含在此模組的輸出包中的資訊。</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL引用]</td>
   <td>選擇要包括在輸出中的任何引用欄位。</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL集合]</td>
   <td>選擇要包括在輸出中的任何引用欄位。</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL ID]</td>
   <td> <p>輸入唯一 [!DNL Workfront] 您要模組讀取的記錄ID。</p> <p>若要取得ID，請開啟 [!DNL Workfront] 物件，並複製URL結尾"ID="之後的文字。 例如：https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
 </tbody> 
</table>

查看 [!DNL Workfront] 您可以在 [[!DNL Workfront] object types available for each [!DNL Workfront] 模組](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL 更新記錄]**

此動作模組會更新物件，例如專案、任務或問題。 模組可讓您選取模組中可用的物件欄位。

您指定記錄的ID。

模組會傳回物件的ID和任何相關欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Workfront] 應用程式至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>輸入唯一 [!DNL Workfront] 要更新模組的記錄ID。</p> <p>若要取得ID，請開啟 [!DNL Workfront] 物件，並複製URL結尾"ID="之後的文字。 例如：https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Record Type]</td> 
   <td> <p>選取 [!DNL Workfront] 記錄您要更新模組。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!DNL Select fields to map]</td> 
   <td>選取您要供資料輸入使用的欄位。 這可讓您使用這些欄位，而無須捲動查看您不需要的欄位。</td> 
  </tr> 
 </tbody> 
</table>

查看 [!DNL Workfront] 您可以在 [[!DNL Workfront] object types available for each [!DNL Workfront] 模組](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* 輸入對象的ID時，可以開始鍵入對象的名稱，然後從清單中選擇該名稱。 然後，模組在欄位中輸入適當的ID。
>* 輸入自訂欄位或 [!UICONTROL 附註] 物件（註解或回覆），您可以在 [!UICONTROL 附註文字] 欄位來建立RTF文字，例如粗體或斜體文字。
>
>  如需更新中RTF的詳細資訊，請參閱 [向工作項添加更新](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) in [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

+++

+++ **[!UICONTROL 上傳檔案]**

此動作模組會將檔案上傳至 [!DNL Workfront] 對象，如項目、任務或問題。

可指定文檔的位置、要上載的檔案以及檔案的可選新名稱。

模組會傳回檔案的ID和任何相關欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Workfront] 應用程式至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL相關記錄ID]</td> 
   <td>輸入唯一 [!DNL Workfront] 要上載文檔的記錄ID。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL相關記錄類型]</td> 
   <td>選取 [!DNL Workfront] 記錄您要模組上傳檔案的位置。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL源檔案]</td> 
   <td> <p>從上一個模組中選擇源檔案，或映射源檔案的名稱和資料。</p> </td> 
  </tr> 
 </tbody> 
</table>

查看 [!DNL Workfront] 您可以在 [[!DNL Workfront] object types available for each [!DNL Workfront] 模組](#workfront-object-types-available-for-each-workfront-module).

+++

### 搜尋

<!--
* [Read Related Records](#read-related-records) 
* [Search](#search)
-->

+++ **[!UICONTROL 讀取相關記錄]**

此搜索模組讀取與您指定的搜索查詢（特定父對象）匹配的記錄。

您可指定要在輸出中包含哪些欄位。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Workfront] 應用程式至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL記錄類型]</td> 
   <td> <p>選擇要讀取其關聯記錄的父記錄(Workfront對象)的類型。</p> <p>查看 [!DNL Workfront] 您可以在 <a href="#object-types-available-for-each-workfront-search-module" class="MCXref xref">[!DNL Workfront] 每個 [!DNL Workfront] 模組</a> 這篇文章。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL父記錄ID]</td> 
   <td> <p>輸入或映射要讀取其關聯記錄的父記錄的ID。</p> <p>若要取得ID，請開啟 [!DNL Workfront] 物件，並複製URL結尾"ID="之後的文字。 例如：https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL集合]</td> 
   <td>選擇或映射要模組讀取的子記錄類型。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL輸出]</td> 
   <td> <p>選擇要包含在此模組的輸出包中的資訊。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 搜尋]**

此搜尋模組會在 [!DNL Workfront] 符合您指定的搜尋查詢。

您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Workfront] 應用程式至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Connect [!DNL Workfront] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL記錄類型]</td> 
   <td> <p>選取 [!DNL Workfront] 記錄您要模組搜尋的。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL結果集]</td> 
   <td>選擇一個選項，以指定您希望模組獲得與您的搜索標準匹配的第一個結果還是所有匹配的結果。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL最大]</td> 
   <td> <p>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL搜索條件]</td> 
   <td> <p>輸入要搜索的欄位、要在查詢中使用的運算子，以及要在欄位中搜索的值。</p> <p>注意：請勿使用 <code>username </code>填入。 包括 <code>username </code>在API查詢中 [!DNL Workfront] 將使用者登入Workfront，則搜尋將無法成功。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL輸出]</td> 
   <td> <p>選取您要納入此模組輸出的欄位。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL引用]</td> 
   <td>選擇要包括在搜索中的任何引用欄位。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL集合]</td> 
   <td>選擇要添加到搜索的任何集合。</td> 
  </tr> 
 </tbody> 
</table>

查看 [!DNL Workfront] 您可以在 [[!DNL Workfront] object types available for each [!DNL Workfront] 模組](#workfront-object-types-available-for-each-workfront-module).

+++

## [!DNL Workfront] 每個 [!DNL Workfront] 模組

<!-- [Object types available for each Workfront trigger module](#object-types-available-for-each-workfront-trigger-module) 
* [Object types available for each Workfront action module](#object-types-available-for-each-workfront-action-module) 
* [Object types available for each Workfront search module](#object-types-available-for-each-workfront-search-module)-->

+++**每個對象都可用的對象類型 [!DNL Workfront] 觸發模組**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>[!UICONTROL監看記錄]</th> 
   <th>[!UICONTROL監視欄位]</th> 
   <th>[!UICONTROL監看事件]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>核准流程</td> 
   <td> </td> 
   <td>✓</td> 
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
   <td>預留時間* </td> 
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

+++**每個對象都可用的對象類型 [!DNL Workfront] 動作模組**

>[!NOTE]
>
>此 [!UICONTROL 下載檔案] 模組不包含在此表格中，因為 [!DNL Workfront] 物件類型不屬於其設定。

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
   <th>[!UICONTROL建立記錄]</th> 
   <th>[!UICONTROL更新記錄]</th> 
   <th>[!UICONTROL刪除記錄]</th> 
   <th>[!UICONTROL上載文檔]</th> 
   <th>[!UICONTROL讀取記錄]</th> 
   <th>[!UICONTROL自訂API呼叫]</th> 
   <th>[!UICONTROL雜項操作]</th> 
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
   <td>預留時間* </td> 
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

+++**每個對象都可用的對象類型 [!DNL Workfront] 搜尋模組**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>[!UICONTROL搜索]</th> 
   <th>[!UICONTROL讀取相關記錄]</th> 
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
   <td>預留時間* </td> 
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

建議您仔細檢查，以確保此功能如預期般運作。

+++

## 中的事件訂閱篩選器 [!DNL Workfront] > [!UICONTROL 觀看事件] 模組

>[!NOTE]
>
>我們強烈建議您在 [!UICONTROL 觀看事件] 模組。

此 [!DNL Workfront] [!UICONTROL 觀看事件] 模組會根據webhook觸發情況，該webhook會在 [!DNL Workfront] API。 事件訂閱是一組資料，可決定要將哪些事件傳送至網頁連結。 例如，若您設定 [!UICONTROL 觀看事件] 正在觀看問題的模組，則事件訂閱只會傳送與問題相關的事件。

Fusion使用者可使用事件訂閱篩選器來建立更符合其使用案例的事件訂閱。 例如，您可以在 [!DNL Workfront] API僅將特定專案中的問題傳送至WebHook，確保 [!UICONTROL 觀看事件] 模組只會針對該專案中的問題觸發。 建立較窄觸發器的能力，透過減少無關觸發器的數量來改進情境設計。

這與在 [!DNL Workfront Fusion] 藍本。 若沒有事件訂閱篩選器，您的Webhook將接收與您選取的物件類型相關的所有事件。 這些事件大多與情境無關，必須先篩選掉，才能繼續。

>[!NOTE]
>
>您無法編輯現有的篩選器 [!DNL Workfront] 網頁鈎點。 為設定不同的篩選器 [!DNL Workfront] 事件訂閱、移除目前的webhook並建立新網頁。

>[!INFO]
>
>**範例：** 請考慮處理指派給特定使用者Ana的新問題的案例。
>
>### 使用事件訂閱篩選器篩選事件（建議）
>
>使用事件篩選器，您可以設定Webhook以在建立問題時將問題指派給Ana時觸發案例。 Ana有userID b378489d8f7cd3cee0539260720a84b7。
>
>![](assets/event-filter-watch-events-350x277.png)
>
>如果一天內建立100個問題，但只將其中兩個指派給Ana，則情境會執行兩次。
>
>### 篩選案例內的事件（不建議）
>
>若要篩選事件，以便僅處理指派給Ana的問題，您可以在 [!UICONTROL 觀看事件] 模組。
>
>![](assets/watch-events-non-event-filter-350x206.png)
>
>如果一天內建立100個問題，但只將其中兩個指派給Ana，則情境會執行100次。 98個執行會在篩選器中停止，但觸發模組仍在使用資料，並在所有執行中執行操作。

如需事件訂閱的詳細資訊，請參閱 [常見問題集 — 事件訂閱](../../wf-api/general/event-subs-faq.md).

如需Webhook的詳細資訊，請參閱 [中的即時觸發器(Webhook) [!DNL Adobe Workfront Fusion]](../../workfront-fusion/webhooks/instant-triggers-webhooks.md)

如需藍本中篩選器的詳細資訊，請參閱 [將篩選器新增至案例，於 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).
