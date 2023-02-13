---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 連接器
navigation-topic: apps-and-their-modules
title: Microsoft Dynamics 365模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用Microsoft Dynamics 365的工作流程，並將其連接至多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: 116df088-20a7-40a8-8880-9f422dc37632
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1541'
ht-degree: 0%

---

# [!DNL Microsoft Dynamics 365 modules]

在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!DNL Microsoft Dynamics 365]，並將其連接至多個協力廠商應用程式和服務。

>[!NOTE]
>
>此 [!DNL Microsoft Dynamics 365] 連接器不支援 [!DNL Dynamics Finance and Operations].

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

使用 [!DNL Microsoft Dynamics] 365，你必須有 [!DNL Microsoft Dynamics 365] 帳戶。

## 將Microsoft Dynamics 365連接至Workfront Fusion

您可以建立與 [!DNL Microsoft Dynamics 365] 直接從內部 [!DNL Microsoft Dynamics 365] 模組。

1. 在任何 [!DNL Microsoft Dynamics 365] 模組，按一下 **[!UICONTROL 新增]** 旁邊 [!UICONTROL 連線] 欄位。
1. 輸入連線的名稱。
1. 在 **[!UICONTROL 資源]** 欄位，輸入 [!DNL Dynamics 365] 帳戶，不 `https://`.
1. 按一下 **[!UICONTROL 繼續]** 若要建立連線，請返回模組。

>[!NOTE]
>
>註冊時 [!DNL Workfront Fusion] 在 [!DNL Microsoft Azure] 入口，使用以下重定向URI:
>
>* `https://app.workfrontfusion.com/oauth/cb/workfront-microsoft-dynamics2`



## [!DNL Microsoft Dynamics 365] 模組及其欄位

設定時 [!DNL Microsoft Dynamics 365] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!DNL Microsoft Dynamics 365] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL 監看記錄（已排程）]](#watch-records-scheduled)
* [[!UICONTROL 監看記錄（即時）]](#watch-records-real-time)
* [[!UICONTROL 建立記錄]](#create-record)
* [[!UICONTROL 進行API呼叫]](#make-an-api-call)
* [[!UICONTROL 刪除記錄]](#delete-record)
* [[!UICONTROL 讀取記錄]](#read-records)
* [[!UICONTROL 更新記錄]](#update-record)
* [[!UICONTROL 搜索記錄]](#search-records)

### [!UICONTROL 監看記錄（已排程）]

當您在指定的物件中的記錄在上次排程執行後建立或更新時，此排程觸發程式模組會執行情境 [!DNL Dynamics 365].

模組的輸出指示其找到的記錄是新記錄還是更新記錄（如果在時段內同時新增和更新，則標籤為新記錄）。 您可以在案例的後續模組中對應此資訊。

這會以您指定的定期排程間隔進行。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
  <td> <p>有關連接 [!DNL Microsoft Dynamics 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] to [!DNL Workfront Fusion]</a> 這篇文章。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Include]</td> 
   <td>選取是否要讓模組觀看 <strong>[!UICONTROL僅新記錄]</strong>, <strong>[!UICONTROL僅更新記錄]</strong>，或 <strong>[!UICONTROL新記錄和所有更改]</strong>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL實體類型]</td> 
   <td>選擇您希望藍本觀看的[!UICONTROL Microsoft Dynamics 365]記錄類型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸出]</td> 
   <td> <p>選擇要包含在此模組的輸出包中的資訊。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL最大記錄數]</td> 
   <td> <p>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 監看記錄（即時）]

此即時觸發模組會在您指定的記錄（物件）建立或更新於 [!DNL Dynamics 365].

此模組中需要Webhook。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>選取您要用於此模組的網頁連結。 </p> <p>要添加新網頁鈎點：</p> 
    <ol> 
     <li value="1"> <p>按一下 <strong>[!UICONTROL添加]</strong> 在Webhook欄位的右側</p> </li> 
     <li value="2"> <p>在 <strong>[!UICONTROL Webhook]</strong> 名稱欄位，為webhook輸入描述性名稱。</p> </li> 
     <li value="3"> <p>在 <strong>[!UICONTROL連接]</strong> 欄位中，選擇要使用的連接</p> <p>有關連接 [!DNL Microsoft Dynamics 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] to [!DNL Workfront Fusion]</a> 這篇文章。 </p> </li> 
     <li value="4"> <p>按一下 <strong>[!UICONTROL保存]</strong> 以儲存webhook並返回模組。</p> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 建立記錄]

此操作模組建立實體，如約會或任務。

您可以指定要建立的實體的相關資訊。

模組會傳回新實體和任何相關欄位的ID，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Microsoft Dynamics 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] to [!DNL Workfront Fusion]</a> 這篇文章。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL實體類型]</td> 
   <td>選取要模組建立的實體類型。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL屬性欄位]</td> 
   <td>在這些欄位中，輸入您希望工作項對給定屬性具有的值。 可用欄位取決於實體類型。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 進行API呼叫]

此動作模組可讓您對 [!DNL Microsoft Dynamics 365] API。 這樣，您就可以建立資料流自動化，而另一個無法完成 [!DNL Microsoft Dynamics 365] 模組。

模組會傳回狀態代碼、標題和內文的相關資訊。 您可以在案例的後續模組中對應此資訊。

若要進一步了解，請參閱 [!DNL Microsoft] 關於使用 [!DNL Dynamics 365 Customer Engagement Web API].

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
  <td> <p>有關連接 [!DNL Microsoft Dynamics 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] to [!DNL Workfront Fusion]</a> 這篇文章。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>輸入相對於的路徑 <code>&lt;Instance URL>/api/data/v9.1/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL方法]</td> 
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> <p>如需</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL標題]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標題。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 為您添加授權標頭。</p> </td> 
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

### [!UICONTROL 刪除記錄]

此動作模組會刪除實體。

您可指定實體的ID。

模組會傳回實體的ID和任何相關欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
  <td> <p>有關連接 [!DNL Microsoft Dynamics 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] to [!DNL Workfront Fusion]</a> 這篇文章。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL實體類型]</td> 
   <td> <p>選取您要模組刪除的實體類型。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td> <p>輸入或對應唯一 [!DNL Microsoft Dynamics 365] 您要刪除模組的記錄ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 讀取記錄]

此動作模組會從中的單一實體讀取資料 [!DNL Microsoft Dynamics 365].

您可指定實體的ID。

模組會傳回實體的ID和任何相關欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
  <td> <p>有關連接 [!DNL Microsoft Dynamics 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] to [!DNL Workfront Fusion]</a> 這篇文章。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL實體類型]</td> 
   <td>選取您要模組讀取的實體類型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸出]</td> 
   <td> <p>選擇要包含在此模組的輸出包中的資訊。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>輸入或對應唯一 [!DNL Microsoft Dynamics 365] 您要模組讀取的記錄ID。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 更新記錄]

此動作模組會更新實體。

您可指定實體的ID。

模組會傳回更新記錄和任何相關欄位的ID，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
  <td> <p>有關連接 [!DNL Microsoft Dynamics 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] to [!DNL Workfront Fusion]</a> 這篇文章。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL實體類型]</td> 
   <td>選取要模組更新的實體類型。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL屬性欄位]</td> 
   <td>在這些欄位中，輸入您希望工作項對給定屬性具有的值。 可用欄位取決於實體類型。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>輸入或對應唯一 [!DNL Microsoft Dynamics] 希望模組更新的記錄ID為365。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 搜索記錄]

此搜尋模組會在 [!DNL Microsoft Dynamics 365] 符合您指定的搜尋查詢。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
  <td> <p>有關連接 [!DNL Microsoft Dynamics 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] to [!DNL Workfront Fusion]</a> 這篇文章。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL實體類型]</td> 
   <td>選取要模組更新的實體類型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL篩選器]</td> 
   <td> <p>選取要用於此搜尋的篩選器。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL標準篩選器]</strong> </p> <p>選取欄位和運算子，然後輸入或對應您要搜尋的值，以設定篩選器。 您可以對篩選器使用AND或OR規則。</p> </li> 
     <li> <p><strong>[!UICONTROL查詢函式]</strong> </p> <p>輸入 [!DNL Dynamics 365] 要用來搜尋的網頁API查詢函式。 </p> <p>有關查詢函式的詳細資訊，請參閱 <a href="https://docs.microsoft.com/en-us/dynamics365/customer-engagement/web-api/queryfunctions?view=dynamics-ce-odata-9">Web API查詢函式參考</a> 在 [!DNL Microsoft] 檔案。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL排序]</td> 
   <td> <p>指定項目傳回的順序。 您可以添加多個排序。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL欄位]</strong> </p> <p>指定要依據哪個欄位來排序結果。</p> </li> 
     <li> <p><strong>[!UICONTROL方向]</strong> </p> <p>指定排序方向（遞增或遞減）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL最大記錄數]</td> 
   <td> <p>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸出]</td> 
   <td> <p>選擇要包含在此模組的輸出包中的資訊。</p> </td> 
  </tr> 
 </tbody> 
</table>
