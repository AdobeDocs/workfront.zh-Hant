---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 連接器
navigation-topic: apps-and-their-modules
title: Datadog模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用Datadog的工作流程，並將其連接至多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: a0b4352d-a1ce-4459-a58e-71de860b8a90
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '795'
ht-degree: 1%

---

# [!DNL Datadog] 模組

在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!DNL Datadog]，並將其連接至多個協力廠商應用程式和服務。

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

使用 [!DNL Datadog] 模組，您必須 [!DNL Datadog] 帳戶。

## Connect [!DNL Datadog] to [!DNL Workfront Fusion] {#connect-datadog-to-workfront-fusion}

### 擷取您的API金鑰和應用程式金鑰 {#retrieve-your-api-key-and-application-key}

連接 [!DNL Datadog] 帳戶 [!DNL Workfront Fusion] 您需要從 [!DNL Datadog] 帳戶。

1. 登入 [!DNL Datadog] 帳戶。
1. 在左側導覽面板中，按一下 **[!UICONTROL 整合]**，然後按一下 **[!UICONTROL API]**.
1. 在主畫面上，按一下 **[!UICONTROL API金鑰]**.
1. 將滑鼠移到紫色列上以顯示API金鑰。
1. 將API金鑰複製到安全位置。
1. 在主畫面上，按一下 **[!UICONTROL 應用程式密鑰]**.
1. 將滑鼠指標暫留在紫色列上，以顯示應用程式金鑰。
1. 將應用程式密鑰複製到安全位置。

### 建立連線至 [!DNL Datadog] in [!DNL Workfront Fusion]

您可以建立與 [!DNL Datadog] 直接從內部 [!UICONTROL Datadog] 模組。

1. 在任何 [!UICONTROL Datadog] 模組，按一下 **[!UICONTROL 新增]** 旁邊 [!UICONTROL 連線] 欄位。
1. 依照下列方式填入模組的欄位：

<table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL連接類型]</td> 
      <td> <p> 選擇[!UICONTROL [!DNL Datadog] 應用程式]選項，以完全存取 [!DNL Datadog] API。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL連接名]</td> 
      <td> <p> 輸入連線的名稱。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL域] </td> 
      <td> <p>選取您要連線的網域（美國或歐盟）。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL API密鑰]</td> 
      <td> <p> 輸入 [!DNL Datadog] API金鑰。 </p> <p>如需擷取API金鑰的指示，請參閱 <a href="#retrieve-your-api-key-and-application-key" class="MCXref xref">擷取您的API金鑰和應用程式金鑰</a> 這篇文章。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL應用程式密鑰]</td> 
      <td> <p> 輸入 [!DNL Datadog] 應用程式金鑰。 </p> <p>有關檢索應用程式密鑰的說明，請參見 <a href="#retrieve-your-api-key-and-application-key" class="MCXref xref">擷取您的API金鑰和應用程式金鑰</a> 這篇文章。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **[!UICONTROL 繼續]** 若要建立連線，請返回模組。

## [!DNL Datadog] 模組及其欄位

設定時 [!DNL Datadog] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!DNL Datadog] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### 動作

* [[!UICONTROL 後置時間點]](#post-timeseries-points)
* [[!UICONTROL 進行API呼叫]](#make-an-api-call)

#### [!UICONTROL 後置時間點]

模組可讓您張貼可在上繪製的時間序列資料 [!DNL Datadog]的控制面板。

壓縮有效載荷的限制為3.2兆位元組(3200000)，解壓縮有效載荷的限制為62兆位元組(62914560)。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Datadog] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-datadog-to-workfront-fusion" class="MCXref xref">Connect [!DNL Datadog] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL系列]</td> 
   <td> <p>添加要提交到的時間系列 [!DNL Datadog].</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL度量]</strong> </p> <p>輸入時間序列的名稱。</p> </li> 
     <li> <p><strong>[!UICONTROL類型]</strong> </p> <p>選取量度的類型。</p> </li> 
     <li> <p><strong>[!UICONTROL間隔]</strong> </p> <p> 如果量度的類型是比率或計數，請定義對應的間隔。</p> </li> 
     <li> <p><strong>[!UICONTROL點]</strong> </p> <p>新增與量度相關的點。</p> <p>這是JSON點陣列。 每個點的格式為： <code>[[POSIX_timestamp, numeric_value], ...] </code></p> <p>備註:  <p>時間戳記必須以秒為單位。</p> <p>時間戳記必須為最新。 「目前」的定義是未來不超過10分鐘，或過去超過1小時。</p> <p> 數值格式應為浮點值。</p> </p> <p>此欄位至少必須包含1個項目。</p> </li> 
     <li> <p><strong>[!UICONTROL主機]</strong> </p> <p>輸入產生量度的主機名稱。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 進行API呼叫]

此動作模組可讓您執行自訂API呼叫。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Datadog] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-datadog-to-workfront-fusion" class="MCXref xref">Connect [!DNL Datadog] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>輸入相對於的路徑 <code>https://api.datadoghq.com/api/</code>. 範例:<code> /v1/org</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL方法]</td> 
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL標題]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標題。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion會為您新增授權標頭。</p> </td> 
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

**範例：** 下列API呼叫會傳回您 [!DNL Datadog] 帳戶：

URL: `/v1/dashboard`

方法: `GET`

![](assets/datadog-api-example.png)

結果可在模組的「輸出」中，於「套件>內文>控制面板」下找到。

在我們的範例中，傳回3個控制面板：

![](assets/datadog-api-response-example.png)
