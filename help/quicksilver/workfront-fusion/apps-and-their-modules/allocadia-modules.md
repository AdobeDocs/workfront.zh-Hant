---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: 分配模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用Allocadia的工作流程，並將其連結至多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: f1edefd1-9fe0-48fc-bea2-c3f9facf7363
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '1401'
ht-degree: 0%

---

# [!DNL Allocadia] 模組

在 [!DNL Adobe Workfront Fusion] 情境下，您可以自動化使用下列專案的工作流程： [!DNL Allocadia]，以及將其連線到多個協力廠商應用程式和服務。

如果您需要建立案例的說明，請參閱 [在中建立情境 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

如需模組的相關資訊，請參閱 [中的模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <td>
   <p>目前授權需求：否 [!DNL Workfront Fusion] 授權需求。</p>
   <p>或</p>
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] 適用於工作自動化與整合] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 計畫，您的組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 計畫。</p>
   <p>或</p>
   <p>舊版產品需求：貴組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有哪些計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

有關以下專案的資訊： [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 必要條件

使用 [!DNL Allocadia] 模組，您必須擁有 [!DNL Allocadia] 帳戶。

## Connect [!DNL Allocadia] 至 [!DNL Workfront Fusion]

您可以建立與的連線 [!DNL Allocadia] 直接從「 」內部 [!DNL Allocadia] 模組。

1. 在任何 [!DNL Allocadia] 模組，按一下 **[!UICONTROL 新增]** 旁邊 [!UICONTROL 連線] 欄位。
1. 選取您要使用北美伺服器還是歐洲伺服器。
1. 輸入您的使用者名稱和密碼。
1. 按一下 **[!UICONTROL 繼續]** 以建立連線並返回模組。

## [!DNL Allocadia] 模組及其欄位

當您設定 [!DNL Allocadia] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 除了這些以外， [!DNL Allocadia] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應至中的另一個模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [觸發器](#triggers)
* [動作](#actions)
* [搜尋](#searches)

### 觸發器

#### [!UICONTROL 觀看記錄]

此觸發模組會在新增、更新或同時新增特定型別的物件時執行案例。 模組會傳回與一個或多個記錄關聯的所有標準欄位，以及連線存取的任何自訂欄位和值。 您可以將此資訊對應到情境中的後續模組中。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> <table style="table-layout:auto"> <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[！UICONTROL連線]</p> </td> 
   <td> <p>如需有關將您的Allocadia帳戶連線至的說明 [!DNL Workfront Fusion]，請參閱 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">[！UICONTROL Connect Allocadia]至Workfront Fusion</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">篩選器</td> 
   <td> <p>選取您希望情境僅觀看「新記錄」、[！UICONTROL僅更新記錄]還是「新記錄和更新記錄」。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">實體型別</td> 
   <td>選取您希望模組觀看的Allocadia記錄型別。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">輸出</td> 
   <td> <p>選取您要納入模組輸出的欄位。 可用欄位取決於您選取的實體型別。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">限制</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期中監視的最大記錄數。</p> </td> 
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

此動作模組可讓您對 [!DNL Allocadia] API。 如此一來，您就可以建立其他人無法完成的資料流程自動化 [!DNL Allocadia] 模組。

該動作以您指定的圖元型別（Allocadia物件型別）為基礎。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL連線]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Allocadia] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connect [!DNL Allocadia] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL URL]</td> 
   <td>輸入相對於 <code>https://api-na.allocadia.com/{version}</code> 或 <code>https://api-eu.allocadia.com/{version}</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL方法]</td> 
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL標頭]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標頭。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 為您新增授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查詢字串]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的查詢。</p> <p>例如： <code>{"name":"something-urgent"}</code></p> </td> 
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

#### [!UICONTROL 讀取記錄]

此動作模組會從中的單一記錄讀取資料 [!DNL Allocadia].

您指定記錄的ID。

模組會傳回與記錄相關聯的任何標準欄位，以及連線存取的任何自訂欄位和值。 您可以將此資訊對應到情境中的後續模組中。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[！UICONTROL連線]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Allocadia] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connect [!DNL Allocadia] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL實體型別]</td> 
   <td>選取型別 [!DNL Allocadia] 您希望模組讀取的記錄。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸出]</td> 
   <td> <p>選取您要納入模組輸出的欄位。 可用欄位取決於您選取的[！UICONTROL實體型別]。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL ID]</td> 
   <td>輸入或對映唯一的 [!DNL Allocadia] 您希望模組讀取的記錄ID。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立記錄]

此動作模組會建立記錄。

模組會傳回記錄ID和任何關聯欄位，以及連線存取的任何自訂欄位和值。 您可以將此資訊對應到情境中的後續模組中。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[！UICONTROL連線]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Allocadia] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connect [!DNL Allocadia] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL實體型別]</td> 
   <td>選取您要建立以線上專案或欄選擇為基礎的新記錄。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL預算]</td> 
   <td> <p>選取您要建立記錄的預算。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Column choices]</td> 
   <td>選取要用來建立新記錄的欄。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Label]</td> 
   <td>輸入或對應新記錄的標籤</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除記錄]

此動作模組會刪除特定記錄。

您指定記錄的ID。

模組會傳回記錄ID和任何關聯欄位，以及連線存取的任何自訂欄位和值。 您可以將此資訊對應到情境中的後續模組中。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[！UICONTROL連線]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Allocadia] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connect [!DNL Allocadia] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL實體型別]</td> 
   <td> <p>選取要刪除的圖元型別。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL行專案]</strong> </p> <p>輸入明細專案識別碼</p> </li> 
     <li> <p><strong>[！UICONTROL資料行選擇]</strong> </p> <p>選取您要刪除記錄的預算，然後輸入「欄位識別碼」與「選擇識別碼」。</p> </li> 
     <li> <p><strong>[！UICONTROL預測標籤]</strong> </p> <p>選取您要從中刪除記錄的預算，然後輸入標籤ID。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新記錄]

此動作模組會更新記錄，例如行專案、使用者或欄選擇。

您指定記錄的ID。

模組會傳回記錄ID和任何關聯欄位，以及連線存取的任何自訂欄位和值。 您可以將此資訊對應到情境中的後續模組中。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL連線]</p> </td> 
   <td> <p>如需有關將您的[！UICONTROL Allocadia]帳戶連線至的說明 [!DNL Workfront Fusion]，請參閱 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connect [!DNL Allocadia] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL實體型別]</td> 
   <td>選取型別 [!DNL Allocadia] 記錄您希望模組更新的內容。 其他欄位會根據您選取的實體型別而顯示。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL預算]</td> 
   <td> <p>選取您要更新記錄的預算。 </p> </td> 
  </tr> 
 </tbody> 
</table>

### 搜尋

#### [!UICONTROL 搜尋記錄]

此搜尋模組會在中尋找物件中的記錄 [!DNL Allocadia] 符合您指定的搜尋查詢。

您可以將此資訊對應到情境中的後續模組中。

您可以指定所要的記錄型別。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[！UICONTROL連線]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Allocadia] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">Connect [!DNL Allocadia] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL實體型別]</td> 
   <td>選取型別 [!DNL Allocadia] 您要模組搜尋的記錄。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL預算]</td> 
   <td> <p>選取您要搜尋的預算。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL結果集]</td> 
   <td>選取您希望模組傳回「所有比對記錄」，還是隻傳回「第一個比對記錄」。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL最大記錄數]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期內傳回的最大記錄數。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL搜尋條件]</td> 
   <td>選取您要搜尋的欄位、選取作業，然後輸入或對應您要搜尋的值。 您可以新增 [!DNL AND] 或 [!DNL OR] 進一步篩選搜尋的規則。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸出]</td> 
   <td> <p>選取您要納入模組輸出的欄位。 可用欄位取決於您選取的實體型別。</p> </td> 
  </tr> 
 </tbody> 
</table>
