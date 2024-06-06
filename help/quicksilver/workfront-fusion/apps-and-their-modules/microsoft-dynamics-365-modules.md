---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Microsoft Dynamics 365模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動化使用Microsoft Dynamics 365的工作流程，並將其連結至多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: 116df088-20a7-40a8-8880-9f422dc37632
source-git-commit: 46c282062ed737be860aeb4af96ac5f5efe9360d
workflow-type: tm+mt
source-wordcount: '1633'
ht-degree: 0%

---

# [!DNL Microsoft Dynamics 365 modules]

在 [!DNL Adobe Workfront Fusion] 情境中，您可以使用自動化工作流程 [!DNL Microsoft Dynamics 365]，並連結至多個協力廠商應用程式和服務。

>[!NOTE]
>
>此 [!DNL Microsoft Dynamics 365] 聯結器不支援 [!DNL Dynamics Finance and Operations].

如果您需要有關建立情境的指示，請參閱 [在中建立情境 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

如需模組的相關資訊，請參閱 [中的模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <p>目前授權需求：否 [!DNL Workfront Fusion] 授權需求。</p>
   <p>或</p>
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] 適用於工作自動化與整合] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 計畫，您的組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述的功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 計畫。</p>
   <p>或</p>
   <p>舊版產品需求：貴組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述的功能。</p>
   </td> 
  </tr>
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

有關的資訊 [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 先決條件

使用 [!DNL Microsoft Dynamics] 365，您必須擁有 [!DNL Microsoft Dynamics 365] 帳戶。

## 將Microsoft Dynamics 365連線至Workfront Fusion

您可以建立與您的電腦的連線， [!DNL Microsoft Dynamics 365] 直接從 [!DNL Microsoft Dynamics 365] 模組。

1. 在任何 [!DNL Microsoft Dynamics 365] 模組，按一下 **[!UICONTROL 新增]** 在 [!UICONTROL 連線] 欄位。
1. 輸入連線的名稱。
1. 在 **[!UICONTROL 資源]** 欄位，輸入您的網址 [!DNL Dynamics 365] 帳戶，不含 `https://`.
1. 按一下 **[!UICONTROL 繼續]** 以建立連線並返回模組。

>[!NOTE]
>
>註冊時 [!DNL Workfront Fusion] 在您的 [!DNL Microsoft Azure] 入口網站，請使用以下重新導向URI：
>
>* `https://app.workfrontfusion.com/oauth/cb/workfront-microsoft-dynamics2`


## [!DNL Microsoft Dynamics 365] 模組及其欄位

當您設定 [!DNL Microsoft Dynamics 365] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 除了這些以外， [!DNL Microsoft Dynamics 365] 欄位可能會顯示，端視您應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [在中將資訊從一個模組對應到另一個模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL 觀看記錄（已排程）]](#watch-records-scheduled)
* [[!UICONTROL 觀看記錄（即時）]](#watch-records-real-time)
* [[!UICONTROL 建立記錄]](#create-record)
* [[!UICONTROL 進行API呼叫]](#make-an-api-call)
* [[!UICONTROL 刪除記錄]](#delete-record)
* [[!UICONTROL 讀取記錄]](#read-records)
* [[!UICONTROL 更新記錄]](#update-record)
* [[!UICONTROL 搜尋記錄]](#search-records)

### [!UICONTROL 觀看記錄（已排程）]

當您指定的物件中的記錄是在中上次排定的執行之後建立或更新時，此排定的觸發模組會執行一個案例 [!DNL Dynamics 365].

模組的輸出指出它找到的記錄是新的還是更新的（如果它在時段中同時新增和更新，則標籤為新）。 您可以在情境中的後續模組中對應此資訊。

這會以您指定的定期排程間隔發生。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
  <td> <p>如需有關連線您的電腦的指示 [!DNL Microsoft Dynamics 365] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">連線 [!DNL Microsoft Dynamics 365] 至 [!DNL Workfront Fusion]</a> 本文章內容。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Include]</td> 
   <td>選取是否要讓模組觀看 <strong>[！UICONTROL僅限新記錄]</strong>， <strong>[！UICONTROL僅更新記錄]</strong>，或 <strong>[！UICONTROL新記錄和所有變更]</strong>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL實體型別]</td> 
   <td>選擇要讓情境觀看的[！UICONTROL Microsoft Dynamics 365]記錄型別。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸出]</td> 
   <td> <p>選取要包含在此模組輸出組合中的資訊。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL最大記錄數]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 觀看記錄（即時）]

此即時觸發模組會在您指定的記錄（物件）建立或更新時執行情境 [!DNL Dynamics 365].

此模組需要webhook。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Webhook]</td> 
   <td> <p>選取您要用於此模組的webhook。 </p> <p>若要新增webhook：</p> 
    <ol> 
     <li value="1"> <p>按一下 <strong>[！UICONTROL新增]</strong> 在Webhook欄位右側</p> </li> 
     <li value="2"> <p>在 <strong>[！UICONTROL Webhook]</strong> 名稱欄位，輸入webhook的描述性名稱。</p> </li> 
     <li value="3"> <p>在 <strong>[！UICONTROL Connection]</strong> 欄位中，選取您要使用的連線已選取</p> <p>如需有關連線您的電腦的指示 [!DNL Microsoft Dynamics 365] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">連線 [!DNL Microsoft Dynamics 365] 至 [!DNL Workfront Fusion]</a> 本文章內容。 </p> </li> 
     <li value="4"> <p>按一下 <strong>[！UICONTROL儲存]</strong> 以儲存webhook並返回模組。</p> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 建立記錄]

此動作模組會建立實體，例如約會或任務。

您可以指定要建立的圖元相關資訊。

模組會傳回新實體的ID及任何關聯欄位，連同連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL Microsoft Dynamics 365] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">連線 [!DNL Microsoft Dynamics 365] 至 [!DNL Workfront Fusion]</a> 本文章內容。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL實體型別]</td> 
   <td>選取您要模組建立的實體型別。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇要對應的欄位]</td> 
   <td>選取建立記錄時您想要包含值的欄位。 可用欄位取決於實體型別。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[！UICONTROL屬性欄位]</td> 
   <td> 這些是您選取的欄位。 輸入您要讓記錄擁有指定屬性的值。 </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 進行API呼叫]

此動作模組可讓您對 [!DNL Microsoft Dynamics 365] API。 如此一來，您就可以建立其他人無法完成的資料流程自動化 [!DNL Microsoft Dynamics 365] 模組。

模組會傳回狀態代碼、標題和本文的相關資訊。 您可以在情境中的後續模組中對應此資訊。

若要進一步瞭解，請參閱 [!DNL Microsoft] 有關使用的檔案 [!DNL Dynamics 365 Customer Engagement Web API].

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
  <td> <p>如需有關連線您的電腦的指示 [!DNL Microsoft Dynamics 365] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">連線 [!DNL Microsoft Dynamics 365] 至 [!DNL Workfront Fusion]</a> 本文章內容。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL URL]</td> 
   <td> <p>輸入相對於 <code>&lt;Instance URL>/api/data/v9.1/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL方法]</td> 
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> <p>有關詳細資訊</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標頭。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 為您新增授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查詢字串]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的查詢。</p> <p>例如： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Body]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的內文內容。</p> <p>注意：  <p>使用條件陳述式時，例如 <code>if</code> 在JSON中，將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 刪除記錄]

此動作模組會刪除實體。

您可以指定實體的ID。

模組會傳回實體ID及任何關聯欄位，連同連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
  <td> <p>如需有關連線您的電腦的指示 [!DNL Microsoft Dynamics 365] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">連線 [!DNL Microsoft Dynamics 365] 至 [!DNL Workfront Fusion]</a> 本文章內容。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL實體型別]</td> 
   <td> <p>選取您要讓模組刪除的實體型別。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL ID]</td> 
   <td> <p>輸入或對映唯一的 [!DNL Microsoft Dynamics 365] 您要模組刪除的記錄ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 讀取記錄]

此動作模組會從中的單一實體讀取資料 [!DNL Microsoft Dynamics 365].

您可以指定實體的ID。

模組會傳回實體ID及任何關聯欄位，連同連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
  <td> <p>如需有關連線您的電腦的指示 [!DNL Microsoft Dynamics 365] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">連線 [!DNL Microsoft Dynamics 365] 至 [!DNL Workfront Fusion]</a> 本文章內容。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL實體型別]</td> 
   <td>選取您希望模組讀取的實體型別。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸出]</td> 
   <td> <p>選取要包含在此模組輸出組合中的資訊。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL ID]</td> 
   <td>輸入或對映唯一的 [!DNL Microsoft Dynamics 365] 您希望模組讀取的記錄ID。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 更新記錄]

此動作模組會更新實體。

您可以指定實體的ID。

模組會傳回更新記錄的ID和任何關聯欄位，以及連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
  <td> <p>如需有關連線您的電腦的指示 [!DNL Microsoft Dynamics 365] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">連線 [!DNL Microsoft Dynamics 365] 至 [!DNL Workfront Fusion]</a> 本文章內容。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[！UICONTROL實體型別]</td> 
   <td>選取您希望模組更新的實體型別。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選擇要對應的欄位]</td> 
   <td>選取建立記錄時您想要包含值的欄位。 可用欄位取決於實體型別。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[！UICONTROL屬性欄位]</td> 
   <td>這些是您選取的欄位。 輸入您要讓記錄擁有指定屬性的值。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[！UICONTROL ID]</td> 
   <td>輸入或對映唯一的 [!DNL Microsoft Dynamics] 您希望模組更新的記錄365 ID。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 搜尋記錄]

此搜尋模組會在中尋找物件中的記錄 [!DNL Microsoft Dynamics 365] 符合您指定的搜尋查詢。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
  <td> <p>如需有關連線您的電腦的指示 [!DNL Microsoft Dynamics 365] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">連線 [!DNL Microsoft Dynamics 365] 至 [!DNL Workfront Fusion]</a> 本文章內容。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL實體型別]</td> 
   <td>選取您希望模組更新的實體型別。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL篩選器]</td> 
   <td> <p>選取要用於此搜尋的篩選器。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL標準篩選器]</strong> </p> <p>選取欄位和運運算元，然後輸入或對應您要搜尋的值，以設定篩選。 您可以使用AND或OR規則來篩選篩選器。</p> </li> 
     <li> <p><strong>[！UICONTROL查詢函式]</strong> </p> <p>輸入 [!DNL Dynamics 365] 您要用來搜尋的網頁API查詢函式。 </p> <p>如需查詢函式的詳細資訊，請參閱 <a href="https://docs.microsoft.com/en-us/dynamics365/customer-engagement/web-api/queryfunctions?view=dynamics-ce-odata-9">Web API查詢函式參考</a> 在 [!DNL Microsoft] 檔案。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL排序]</td> 
   <td> <p>指定專案傳回的順序。 您可以新增多個排序。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL欄位]</strong> </p> <p>指定您要排序結果的欄位。</p> </li> 
     <li> <p><strong>[！UICONTROL方向]</strong> </p> <p>指定排序方向（升序或降序）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL最大記錄數]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸出]</td> 
   <td> <p>選取要包含在此模組輸出組合中的資訊。</p> </td> 
  </tr> 
 </tbody> 
</table>
