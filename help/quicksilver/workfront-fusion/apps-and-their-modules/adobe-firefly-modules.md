---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Adobe Firefly模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動化使用 [!DNL Adobe Firefly]的工作流程，並將其連線到多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 1e131c27-571d-4099-9243-69572bdb3f5a
source-git-commit: f6b00b98d3375e5660d684f1fad682fa721517aa
workflow-type: tm+mt
source-wordcount: '1315'
ht-degree: 0%

---

# [!DNL Adobe Firefly]模組

在[!DNL Adobe Workfront Fusion]案例中，您可以自動化使用[!DNL Adobe Firefly]的工作流程，並將其連線至多個協力廠商應用程式和服務。

如果您需要有關建立案例的指示，請參閱[建立案例](../../workfront-fusion/scenarios/create-a-scenario.md)。

如需模組的相關資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md)中的[模組。

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td> <p>新增：[！UICONTROL Standard]</p><p>或</p><p>目前： [！UICONTROL Work]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 授權**</td> 
   <td>
   <p>目前：無[!DNL Workfront Fusion]授權需求。</p>
   <p>或</p>
   <p>舊版：任何 </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>新增：</p> <ul><li>[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Workfront]計畫：您的組織必須購買[!DNL Adobe Workfront Fusion]。</li><li>已包含[！UICONTROL Ultimate] [!DNL Workfront]計畫： [!DNL Workfront Fusion]。</li></ul>
   <p>或</p>
   <p>目前：您的組織必須購買[!DNL Adobe Workfront Fusion]。</p>
   </td> 
  </tr>
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 先決條件

使用[!DNL Adobe Firefly]聯結器之前，您必須確定符合下列先決條件：

* 您必須擁有使用中的[!DNL Adobe Firefly]帳戶。

## Adobe Campaign API資訊

Adobe Campaign聯結器會使用以下專案：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">API標籤</td> 
   <td>v1.4.24</td> 
  </tr>
 </tbody> 
 </table>

## 建立與[!DNL Adobe Firefly]的連線

若要為您的[!DNL Adobe Firefly]模組建立連線：

1. 按一下[連線]方塊旁的&#x200B;**[!UICONTROL 新增]**。

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
          <p>輸入此連線的名稱。</p>
        </td>
        </tr>
        <tr>
        <td role="rowheader">[！UICONTROL環境]</td>
        <td>選取您要連線到生產或非生產環境。</td>
        </tr>
        <tr>
        <td role="rowheader">[！UICONTROL型別]</td>
        <td>選取您要連線到服務帳戶還是個人帳戶。</td>
        </tr>
        <tr>
        <td role="rowheader">[！UICONTROL使用者端ID]</td>
        <td>輸入您的[！UICONTROLAdobe] [！UICONTROL使用者端ID]。 這可以在[!DNL Adobe Developer Console]的[！UICONTROL Credentials]詳細資訊區段中找到。</td>
        </tr>
        <tr>
        <td role="rowheader">[！UICONTROL使用者端密碼]</td>
        <td>輸入您的[!DNL Adobe] [！UICONTROL使用者端密碼]。 這可以在[!DNL Adobe Developer Console]的[！UICONTROL Credentials]詳細資訊區段中找到。</td>
        </tr>
      </tbody>
    </table>

1. 按一下&#x200B;**[!UICONTROL 繼續]**&#x200B;以儲存連線並返回模組。

## [!DNL Adobe Firefly]模組及其欄位

當您設定[!DNL Adobe Firefly]模組時，[!DNL Workfront Fusion]會顯示下列欄位。 除了這些欄位以外，可能還會顯示其他[!DNL Adobe Firefly]欄位，視您在應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中將資訊從一個模組對應到另一個模組。

![](assets/map-toggle-350x74.png)

### 進行自訂API呼叫

此動作模組會對Firefly API進行自訂呼叫。

如需特定可用的API，請參閱Adobe Developer檔案中的[Adobe FireflyAPI](https://developer.adobe.com/firefly-services/docs/firefly-api/)。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>如需建立[!DNL Adobe Firefly]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >建立與[!DNL Adobe Firefly]</a>的連線。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL URL]</td>
      <td>
        <p>輸入相對於<code>https://firefly-api-enterprise-stage.adobe.io/</code>的路徑。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL方法]</p>
      </td>
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP要求方法。</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Headers]</td>
      <td>
        <p>以標準JSON物件的形式新增請求的標頭。</p>
        <p>例如， <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] 自動新增授權標頭。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Body]</td>
   <td> <p>以標準JSON物件的形式新增API呼叫的內文內容。</p> <p>注意：  <p>在JSON中使用條件陳述式（例如<code>if</code>）時，請將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

### 展開影像

此動作模組會展開影像，選擇性地從您提供的提示中展開內容。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需建立[!DNL Adobe Campaign]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >建立與[!DNL Adobe Firefly]</a>的連線。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL提示]</td> 
   <td>針對您要展開影像的內容輸入或對應提示。 如果未提供提示，影像將會展開並包含符合原始影像的內容。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL變化數]</td> 
   <td>輸入介於1-4之間的數字。 模組會產生此數量的展開影像變數。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL展開影像格式]</td> 
   <td>選取將儲存展開影像的檔案格式。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Source檔案]</td> 
   <td>  <p>從先前的模組中選取來源檔案，或對應來源檔案的影像檔案名稱和影像檔案（資料）。</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL大小]</td> 
   <td>選取您想要的展開影像大小。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL種子]</td> 
   <td>輸入或對應整數。 您可以在其他展開影像模組中使用相同的種子，以產生具有不同樣式的類似影像。 </td> 
  </tr> 
 </tbody> 
</table>

## 填滿影像

此動作模組會填滿影像的遮色區域，選擇性地使用您提供的提示內容。


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需建立[!DNL Adobe Campaign]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >建立與[!DNL Adobe Firefly]</a>的連線。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL提示]</td> 
   <td>針對您要填滿影像的內容，輸入或對應提示。 如果未提供提示，則會以符合原始影像的內容來填滿影像。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL變化數]</td> 
   <td>輸入介於1-4之間的數字。 模組會產生此數量的填入影像變數。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL填色影像格式]</td> 
   <td>選取將儲存填色影像的檔案格式。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Image]</td> 
   <td>  <p> 按一下<b>新增影像</b>。 從先前的模組中選取來源檔案，或對應來源檔案的影像檔案名稱和影像資料。</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL遮罩]</td> 
   <td>  <p> 按一下<b>新增遮罩</b>。 從先前的模組中選取來源檔案，或對應來源檔案的「遮罩」檔案名稱和「遮罩」資料。 遮色片檔案代表將會填滿產生內容的自訂遮色片。</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL大小]</td> 
   <td>選取您想要填色影像的大小。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL種子]</td> 
   <td>針對模組將產生的每個影像，按一下<b>新增專案<b>並輸入或對應整數。 您可以在其他展開影像模組中使用相同的種子，以產生具有不同樣式的類似影像。 您新增的種子數必須等於「變化數」欄位。</td> 
  </tr> 
 </tbody> 
</table>

## 產生影像

此動作模組會根據您提供的提示產生和影像。 您也可以提供選用的參考影像，產生的影像將與參考影像的樣式相符。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需建立[!DNL Adobe Campaign]連線的說明，請參閱本文中的<a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >建立與[!DNL Adobe Firefly]</a>的連線。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL提示]</td> 
   <td>輸入或對應您要建立之影像的提示。 提示中更詳細的內容可讓您更能控制影像中顯示的內容。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL變化數]</td> 
   <td>輸入介於1-4之間的數字。 模組會產生此數量的影像變數。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL產生的影像格式]</td> 
   <td>選取將儲存展開影像的檔案格式。 如果您選取「預設」，如果沒有提供參照影像，檔案格式將會JPEG。 如果提供參考影像，則產生影像的檔案格式將與參考影像相同。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Source檔案]</td> 
   <td>  <p>從先前的模組中選取來源檔案，或對應來源檔案的「參照」影像檔案名稱和「參照」影像檔案（資料）。 將建立產生的影像以符合參考影像的樣式。</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL預設集]</td> 
   <td>如果要使用預設樣式，請按一下「新增專案」，然後輸入或對應您要使用的樣式。<p>如需預設樣式清單，請參閱Adobe開發人員檔案中的<a href="https://developer.adobe.com/firefly-services/docs/firefly-api/guides/concepts/style-presets/" >影像模型樣式</a>。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL負面提示]</td> 
   <td>在產生的內容中輸入或對應您要避免的文字。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL內容類別]</td> 
   <td>選取您希望產生的影像更像是像片，還是更像是建立的圖案。 <ul><li><b>相片</b><p>輸入「光圈」、「快門速度」（以秒為單位）和「視野」（以毫米為單位）的值。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL種子]</td> 
   <td>輸入或對應整數。 您可以在其他展開影像模組中使用相同的種子，以產生具有不同樣式的類似影像。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL大小]</td> 
   <td>選取您希望產生的影像的大小。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL強度]</td> 
   <td>輸入或對應整數，該整數代表產生的影像與預設樣式或參考影像的樣式相符的強度。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL視覺強度]</td> 
   <td>輸入或對應整數，代表像片現有視覺特性的整體強度。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Locale]</td> 
   <td>如果提供了地區設定，模組會產生與指定地區設定更相關的內容。 <p>地區必須以ISO 639-1語言代碼和ISO 3166-1區域提供。</p><p> 範例： <code>en-US</code></p></td> 
  </tr> 
 </tbody> 
</table>
