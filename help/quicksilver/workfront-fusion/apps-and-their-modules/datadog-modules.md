---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Datadog模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用Datadog的工作流程，並將其連線到多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: a0b4352d-a1ce-4459-a58e-71de860b8a90
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 0%

---

# [!DNL Datadog]模組

在[!DNL Adobe Workfront Fusion]案例中，您可以自動化使用[!DNL Datadog]的工作流程，並將其連線至多個協力廠商應用程式和服務。

如果您需要有關建立案例的指示，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md)中建立案例。

如需模組的相關資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md)中的[模組。

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
   <p>舊版授權需求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
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

## 先決條件

若要使用[!DNL Datadog]模組，您必須有[!DNL Datadog]帳戶。

## 將[!DNL Datadog]連線至[!DNL Workfront Fusion] {#connect-datadog-to-workfront-fusion}

### 擷取您的API金鑰和應用程式金鑰 {#retrieve-your-api-key-and-application-key}

若要將您的[!DNL Datadog]帳戶連線至[!DNL Workfront Fusion]，您必須從您的[!DNL Datadog]帳戶擷取API金鑰和應用程式金鑰。

1. 登入您的[!DNL Datadog]帳戶。
1. 在左側導覽面板中，按一下&#x200B;**[!UICONTROL 整合]**，然後按一下&#x200B;**[!UICONTROL API]**。
1. 在主畫面上，按一下&#x200B;**[!UICONTROL API金鑰]**。
1. 將滑鼠停留在紫色列上以顯示API金鑰。
1. 將API金鑰複製到安全位置。
1. 在主畫面上，按一下&#x200B;**[!UICONTROL 應用程式鍵]**。
1. 將滑鼠指標暫留在紫色列上，即可顯示應用程式索引鍵。
1. 將應用程式金鑰複製到安全位置。

### 在[!DNL Workfront Fusion]中建立與[!DNL Datadog]的連線

您可以直接從[!UICONTROL Datadog]模組內建立與您的[!DNL Datadog]帳戶的連線。

1. 在任何[!UICONTROL Datadog]模組中，按一下[!UICONTROL 連線]欄位旁的&#x200B;**[!UICONTROL 新增]**。
1. 依照以下方式填寫模組的欄位：

<table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL連線型別]</td> 
      <td> <p> 選取[！UICONTROL [!DNL Datadog] Application]選項以取得[!DNL Datadog] API的完整存取權。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL連線名稱]</td> 
      <td> <p> 輸入連線的名稱。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL網域] </td> 
      <td> <p>選取您要連線的網域（美國或歐盟）。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL API Key]</td> 
      <td> <p> 輸入您的[!DNL Datadog] API金鑰。 </p> <p>如需擷取API金鑰的指示，請參閱本文中的<a href="#retrieve-your-api-key-and-application-key" class="MCXref xref">擷取您的API金鑰和應用程式金鑰</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL應用程式鍵]</td> 
      <td> <p> 輸入您的[!DNL Datadog]應用程式金鑰。 </p> <p>如需擷取應用程式金鑰的指示，請參閱本文中的<a href="#retrieve-your-api-key-and-application-key" class="MCXref xref">擷取您的API金鑰和應用程式金鑰</a>。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**[!UICONTROL 繼續]**&#x200B;以建立連線並返回模組。

## [!DNL Datadog]模組及其欄位

當您設定[!DNL Datadog]模組時，[!DNL Workfront Fusion]會顯示下列欄位。 除了這些欄位以外，可能還會顯示其他[!DNL Datadog]欄位，視您在應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中將資訊從一個模組對應到另一個模組。

![](assets/map-toggle-350x74.png)

### 動作

* [[!UICONTROL Post時間序列點]](#post-timeseries-points)
* [[!UICONTROL 進行API呼叫]](#make-an-api-call)

#### [!UICONTROL Post時間序列點]

此模組可讓您張貼可以在[!DNL Datadog]的儀表板上繪製的時間序列資料。

壓縮有效負載的限製為3.2 MB (3200000)，而解壓縮有效負載的限製為62 MB (62914560)。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Datadog]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-datadog-to-workfront-fusion" class="MCXref xref">將[!DNL Datadog]連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Series]</td> 
   <td> <p>新增您要提交到[!DNL Datadog]的時間序列。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL量度]</strong> </p> <p>輸入時間序列的名稱。</p> </li> 
     <li> <p><strong>[！UICONTROL型別]</strong> </p> <p>選取量度型別。</p> </li> 
     <li> <p><strong>[！UICONTROL間隔]</strong> </p> <p> 如果度量的型別是「比率」或「計數」，請定義對應的間隔。</p> </li> 
     <li> <p><strong>[！UICONTROL點]</strong> </p> <p>新增與量度相關的點。</p> <p>這是JSON點陣列。 每個點的格式如下： <code>[[POSIX_timestamp, numeric_value], ...] </code></p> <p>注意：  <p>時間戳記必須以秒為單位。</p> <p>時間戳記必須是最新的。 「目前」的定義是未來不超過10分鐘，或過去不超過1小時。</p> <p> 數值格式應為浮點數值。</p> </p> <p>此欄位必須至少包含1個專案。</p> </li> 
     <li> <p><strong>[！UICONTROL主機]</strong> </p> <p>輸入產生測量結果的主機名稱。</p> </li> 
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
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Datadog]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-datadog-to-workfront-fusion" class="MCXref xref">將[!DNL Datadog]連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL URL]</td> 
   <td>輸入相對於<code>https://api.datadoghq.com/api/</code>的路徑。 範例： <code> /v1/org</code>。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL方法]</td> 
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP要求方法。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標頭。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion會為您新增授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查詢字串]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的查詢。</p> <p>例如： <code>{"name":"something-urgent"}</code></p> </td> 
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

**範例：**&#x200B;下列API呼叫傳回您[!DNL Datadog]帳戶中的所有儀表板：

URL： `/v1/dashboard`

方法： `GET`

![](assets/datadog-api-example.png)

結果可在模組的輸出中找到，位於「套件>內文>控制面板」下。

在我們的範例中，傳回3個控制面板：

![](assets/datadog-api-response-example.png)
