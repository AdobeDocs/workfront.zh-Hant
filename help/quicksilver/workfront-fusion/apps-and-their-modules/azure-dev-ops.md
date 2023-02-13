---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 連接器
navigation-topic: apps-and-their-modules
title: Azure DevOps模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!DNL Azure DevOps]，並將其連接至多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: ecaa93c9-47bb-4fe1-87b4-d2e117cc68ae
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1749'
ht-degree: 0%

---

# [!DNL Azure DevOps] 模組

在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!DNL Azure DevOps]，並將其連接至多個協力廠商應用程式和服務。

如果您需要建立案例的相關指示，請參閱 [在中建立案例 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

如需模組的相關資訊，請參閱 [中的模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 必要條件

使用 [!DNL Azure DevOps] 模組，您必須 [!DNL Azure] DevOps帳戶。

## Connect [!DNL Azure DevOps] to [!DNL Workfront Fusion] {#connect-azure-devops-to-workfront-fusion}

1. 新增 [!DNL Azure DevOps] 模組至您的案例。
1. 按一下 **[!UICONTROL 新增]** 旁邊 [!UICONTROL 連線] 欄位。
1. 在 [!UICONTROL 連線類型] 欄位，選擇 **[!DNL Azure DevOps]**.

   >[!IMPORTANT]
   >
   >此 [!UICONTROL [!DNL Azure DevOps] （請求所有範圍）] 不久後將會淘汰連線類型。 因此，我們不建議使用它。

1. 填寫下列欄位：

   <table style="table-layout:auto">
        <tr>
            <td>[!UICONTROL連接名]</td>
            <td>輸入要建立的連接的名稱。</td>
        </tr>
      <tr>
            <td>[!UICONTROL組織]</td>
            <td>輸入建立您的 [!DNL Azure DevOps] 應用程式。</td>
        </tr>
    </table>

1. 按一下 **[!UICONTROL 繼續]** 完成連接設定並繼續建立方案。

## [!UICONTROL Azure DevOps] 模組及其欄位

設定時 [!DNL Azure DevOps] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!DNL Azure DevOps] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [觸發器](#triggers)
* [動作](#actions)
* [搜尋](#searches)

### 觸發器

#### [!UICONTROL 關注工作項目]

此即時觸發模組會在記錄新增、更新或刪除時執行情境 [!UICONTROL Azure DevOps].

模組會傳回與記錄相關聯的任何標準欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>選取或新增模組的網頁連結。</p> <p>如需觸發模組中Webhook的詳細資訊，請參閱 <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">中的即時觸發器(Webhook) [!DNL Adobe Workfront Fusion]</a>.</p> <p>如需如何建立網頁連結的資訊，請參閱 <a href="../../workfront-fusion/apps-and-their-modules/webhooks-updated.md" class="MCXref xref">Webhook</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 動作

* [自訂API呼叫](#custom-api-call)
* [讀取記錄](#read-record)
* [建立記錄](#create-a-record)
* [更新工作項](#update-a-work-item)
* [[!UICONTROL 上傳附件]](#upload-an-attachment)
* [下載附件](#download-an-attachment)
* [連結工作項]([!UICONTROL #link-work-items])

#### [!UICONTROL 自訂API呼叫]

此動作模組可讓您對 [!DNL Azure DevOps] API。 這樣，您就可以建立資料流自動化，而另一個無法完成 [!DNL Azure DevOps] 模組。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Azure DevOps] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] 到[!UICONTROL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL基URL]</td> 
   <td> <p>選取或對應您用來連線至 [!DNL Azure DevOps] 帳戶</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL相對URL]</td> 
   <td> <p>輸入您要針對此API呼叫連線的相對URL。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>範例: </b></span></span><code>{organization}/_apis[/{area}]/{resource}</code> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL API版本]</td> 
   <td>選取或對應 [!DNL Azure DevOps] 您要針對此API呼叫連線的API。 如果未選取版本， [!DNL Workfront Fusion] 連接 [!DNL Azure DevOps] API 5.1版。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL方法]</td> 
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL標題]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標題。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL查詢字串]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的查詢。</p> <p>例如： <code>{"name":"something-urgent"}</code></p> </td> 
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

#### [!UICONTROL 讀取記錄]

此動作模組會從中的單一記錄讀取資料 [!DNL Azure DevOps].

您指定記錄的ID。

模組會傳回記錄和任何相關欄位的ID，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Azure DevOps] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] 到[!UICONTROL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL記錄類型]</td> 
   <td> <p>選擇要讀取項目還是工作項</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL項目]</strong>:選取您要讀取的專案。</p> </li> 
     <li> <p><strong>[!UICONTROL工作項]</strong>:選擇包含要讀取的工作項的項目，然後選擇工作項類型。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸出]</td> 
   <td>選擇要包含在此模組的輸出包中的資訊。 可用欄位取決於工作項目類型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>輸入或映射要讀取的記錄的ID。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立記錄]

此操作模組將建立新項目或工作項。

模組會輸出新建立工作項的對象ID，或新建立項目的URL和狀態代碼。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Azure DevOps] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] 到[!UICONTROL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL記錄類型]</td> 
   <td> <p>選擇要建立工作項還是項目。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL項目]</strong> </p> <p>填寫下列欄位：</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL名稱]</strong>：輸入或映射新項目的名稱。</p> </li> 
       <li> <p><strong>[!UICONTROL描述]</strong>：輸入或映射新項目的說明。 </p> </li> 
       <li> <p><strong>[!UICONTROL可見性]</strong>:選取您的專案是公開還是私人專案。 使用者必須已登入您的組織，且必須已獲得專案的存取權，才能與私人專案互動。 未登入您組織的使用者可看到公用專案。</p> </li> 
       <li> <p><strong>[!UICONTROL版本控制]</strong>:選取是否要使用專案 [!DNL Git] 或[!UICONTROL Team Foundation Version Control(TFCV)]（用於版本控制）。</p> </li> 
       <li> <p><strong>[!UICONTROL工作項進程]</strong>:選擇要用於項目的工作流程。 選項包括[!UICONTROL Basic]、[!UICONTROL Scrum]、[!UICONTROL功能成熟度模型整合(CMMI)]和[!UICONTROL Agile]。</p> <p>如需 [!DNL Azure DevOps] 進程，請參閱 <a href="https://docs.microsoft.com/en-us/azure/devops/boards/work-items/guidance/choose-process?view=azure-devops&amp;tabs=basic-process">選擇流程</a> 在 [!DNL Azure DevOps] 檔案。</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL工作項]</strong> </p> <p>填寫下列欄位：</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL項目]</strong>:選擇要建立工作項的項目。</p> </li> 
       <li> <p><strong>[!UICONTROL工作項類型]</strong>:選擇要建立的工作項的類型。</p> </li> 
       <li> <p><strong>[!UICONTROL其他欄位]</strong>：在這些欄位中，輸入您希望工作項對指定屬性具有的值。 可用欄位取決於工作項目類型。</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新工作項]

此動作模組會使用其ID更新現有的工作項目。

模組會傳回更新後工作項目的ID。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Azure DevOps] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] 到[!UICONTROL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL項目]</td> 
   <td>選擇包含要更新的工作項的項目。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL工作項類型]</td> 
   <td> <p>選擇要更新的工作項的類型。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL其他欄位]</td> 
   <td>在每個欄位中，輸入您希望工作項對給定屬性具有的值。 可用欄位取決於工作項目類型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL工作項ID]</td> 
   <td>輸入或映射要更新的工作項的ID。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 上傳附件]

此動作模組會上傳檔案並將其附加至工作項目。

模組會傳回附件ID和附件的下載URL。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Azure DevOps] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] 到[!UICONTROL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL項目] </td> 
   <td> <p>選取您要上傳附件的專案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL工作項ID]</td> 
   <td> <p>輸入或映射要上載附件的工作項的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL注釋]</td> 
   <td>輸入要添加到已上載附件的注釋文本。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL源檔案] </td> 
   <td>從上一個模組中選擇源檔案，或輸入或映射源檔案的名稱和內容。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 下載附件]

此動作模組會下載附件。

模組會傳回附件的檔案內容。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Azure DevOps] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] 到[!UICONTROL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL附件URL]</td> 
   <td> <p>輸入或映射要下載的附件的URL。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 連結工作項]

此動作模組會連結兩個工作項目並定義它們之間的關係。

該模組返回主要工作項和任何關聯欄位的ID，以及連接訪問的任何自定義欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Azure DevOps] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] 到[!UICONTROL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL工作項ID]</td> 
   <td>輸入或映射要連結另一個工作項的主要工作項的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL連結的工作項ID]</td> 
   <td>輸入或映射要連結到主要工作項的工作項的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL連結類型]</td> 
   <td> <p>定義要連結的工作項目之間的關係。</p> <p>如需詳細資訊，請參閱 <a href="https://docs.microsoft.com/en-us/azure/devops/boards/queries/link-type-reference?view=azure-devops">連結類型參考</a> 在[!UICONTROL Azure DevOps]檔案中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL注釋]</td> 
   <td>輸入或映射注釋的文本。 這有助於解釋連結的推理或意圖。</td> 
  </tr> 
 </tbody> 
</table>

### 搜尋

#### [!UICONTROL 列出工作項]

此動作模組會擷取 [!DNL Azure DevOps] 專案。

該模組返回主要工作項和任何關聯欄位的ID，以及連接訪問的任何自定義欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Azure DevOps] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] 到[!UICONTROL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL項目]</td> 
   <td>選擇要從中檢索工作項的項目。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL工作項類型]</td> 
   <td> <p>選擇要檢索的工作項的類型。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸出]</td> 
   <td>選取您要在模組輸出中顯示的屬性。 可用欄位取決於您要擷取的工作項目類型。 您至少必須選取一個屬性。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td>輸入或映射工作項的最大數量 [!DNL Workfront Fusion] 在一個執行週期中傳回。</td> 
  </tr> 
 </tbody> 
</table>
