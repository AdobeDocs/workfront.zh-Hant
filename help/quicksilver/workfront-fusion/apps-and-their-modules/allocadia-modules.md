---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 連接器
navigation-topic: apps-and-their-modules
title: 分配模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用Allocadia的工作流程，並將其連接至多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: f1edefd1-9fe0-48fc-bea2-c3f9facf7363
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1354'
ht-degree: 0%

---

# [!DNL Allocadia] 模組

在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!DNL Allocadia]，並將其連接至多個協力廠商應用程式和服務。

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

使用 [!DNL Allocadia] 模組，您必須 [!DNL Allocadia] 帳戶。

## Connect [!DNL Allocadia] to [!DNL Workfront Fusion]

您可以建立與 [!DNL Allocadia] 直接從內部 [!DNL Allocadia] 模組。

1. 在任何 [!DNL Allocadia] 模組，按一下 **[!UICONTROL 新增]** 旁邊 [!UICONTROL 連線] 欄位。
1. 選擇您要使用北美伺服器還是歐洲伺服器。
1. 輸入您的使用者名稱和密碼。
1. 按一下 **[!UICONTROL 繼續]** 若要建立連線，請返回模組。

## [!DNL Allocadia] 模組及其欄位

設定時 [!DNL Allocadia] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!DNL Allocadia] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [觸發器](#triggers)
* [動作](#actions)
* [搜尋](#searches)

### 觸發器

#### [!UICONTROL 監視記錄]

當添加、更新或同時添加特定類型的對象時，此觸發器模組將執行一個方案。 模組會傳回與記錄或記錄相關聯的所有標準欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> <table style="table-layout:auto"> <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關將Allocadia帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect Allocadia]到Workfront Fusion</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">篩選器</td> 
   <td> <p>選擇是否希望方案僅監視新記錄、[!UICONTROL僅更新記錄]或新記錄和更新記錄。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">實體類型</td> 
   <td>選擇要模組監視的分配檔案記錄類型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">輸出</td> 
   <td> <p>選取您要納入模組輸出的欄位。 可用欄位取決於所選的實體類型。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">限制</td> 
   <td> <p>輸入或映射您希望模組在每個方案執行週期中監視的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 動作

* [自訂API呼叫](#custom-api-call)
* [讀取記錄](#read-record)
* [建立記錄](#create-record)
* [刪除記錄](#delete-record)
* [更新記錄](#update-record)

#### [!UICONTROL 自訂API呼叫]

此動作模組可讓您對 [!DNL Allocadia] API。 這樣，您就可以建立資料流自動化，而另一個無法完成 [!DNL Allocadia] 模組。

動作以您指定的實體類型（配置對象類型）為基礎。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Allocadia] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connect [!DNL Allocadia] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>輸入相對於的路徑 <code>https://api-na.allocadia.com/{version}</code> 或 <code>https://api-eu.allocadia.com/{version}</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL方法]</td> 
   td&gt; <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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

#### [!UICONTROL 讀取記錄]

此動作模組會從中的單一記錄讀取資料 [!DNL Allocadia].

您指定記錄的ID。

模組會傳回與記錄相關聯的任何標準欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Allocadia] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connect [!DNL Allocadia] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL實體類型]</td> 
   <td>選取 [!DNL Allocadia] 記錄您要模組讀取的內容。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸出]</td> 
   <td> <p>選取您要納入模組輸出的欄位。 可用欄位取決於您選取的[!UICONTROL實體類型]。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>輸入或對應唯一 [!DNL Allocadia] 您要模組讀取的記錄ID。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立記錄]

此動作模組會建立記錄。

模組會傳回記錄和任何相關欄位的ID，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Allocadia] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connect [!DNL Allocadia] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL實體類型]</td> 
   <td>根據行項或列選項選擇是否要建立新記錄。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL預算]</td> 
   <td> <p>選擇要建立記錄的預算。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Column choices]</td> 
   <td>選擇要用於建立新記錄的列。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Label]</td> 
   <td>輸入或映射新記錄的標籤</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除記錄]

此動作模組會刪除特定記錄。

您指定記錄的ID。

模組會傳回記錄和任何相關欄位的ID，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Allocadia] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connect [!DNL Allocadia] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL實體類型]</td> 
   <td> <p>選擇要刪除的實體類型。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL行項]</strong> </p> <p>輸入行項目ID</p> </li> 
     <li> <p><strong>[!UICONTROL列選擇]</strong> </p> <p>選擇要刪除記錄的預算，然後輸入列ID和選擇ID。</p> </li> 
     <li> <p><strong>[!UICONTROL預測標籤]</strong> </p> <p>選擇要從中刪除記錄的預算，然後輸入標籤ID。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新記錄]

此動作模組會更新記錄，例如行項目、使用者或欄選項。

您指定記錄的ID。

模組會傳回記錄和任何相關欄位的ID，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關將[!UICONTROL Allocadia]帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connect [!DNL Allocadia] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL實體類型]</td> 
   <td>選取 [!DNL Allocadia] 記錄您要更新模組。 其他欄位會根據您選取的實體類型而顯示。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL預算]</td> 
   <td> <p>選擇要更新記錄的預算。 </p> </td> 
  </tr> 
 </tbody> 
</table>

### 搜尋

#### [!UICONTROL 搜索記錄]

此搜尋模組會在 [!DNL Allocadia] 符合您指定的搜尋查詢。

您可以在案例的後續模組中對應此資訊。

您可以指定想要的記錄類型。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Allocadia] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connect [!DNL Allocadia] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL實體類型]</td> 
   <td>選取 [!DNL Allocadia] 記錄您要模組搜尋的。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL預算]</td> 
   <td> <p>選擇要搜索的預算。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL結果集]</td> 
   <td>選擇是否希望模組返回「所有匹配記錄」，還是僅返回「第一個匹配記錄」。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL記錄的最大計數]</td> 
   <td> <p>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL搜索條件]</td> 
   <td>選擇要搜索的欄位，選擇操作，然後輸入或映射要搜索的值。 您可以新增 [!DNL AND] 或 [!DNL OR] 規則來進一步篩選您的搜尋。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸出]</td> 
   <td> <p>選取您要納入模組輸出的欄位。 可用欄位取決於所選的實體類型。</p> </td> 
  </tr> 
 </tbody> 
</table>
