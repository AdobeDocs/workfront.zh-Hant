---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Webhook
description: webhook是由事件觸發的HTTP呼叫。 您可以使用Webhook來啟動即時觸發程式模組。 任何連線至網際網路並允許HTTP請求的應用程式都可以將Webhook傳送至Adobe Workfront Fusion。
author: Becky
feature: Workfront Fusion
exl-id: 987544a4-5840-40d4-9438-41a000aa22ee
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1437'
ht-degree: 0%

---

# Webhook

webhook是由事件觸發的HTTP呼叫。 您可以使用Webhook來啟動即時觸發程式模組。 任何連線至網際網路並允許HTTP請求的應用程式都可以將Webhook傳送至Adobe Workfront Fusion。

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

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

&#42;&#42;有關以下專案的資訊： [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 在中使用webhook [!DNL Workfront Fusion]

>[!NOTE]
>
>若要呼叫第三方webhook （傳出webhook），請使用其中一個HTTP模組。 如需詳細資訊，請參閱 [http模組](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md).

使用webhook將應用程式連線至 [!DNL Workfront Fusion]：

1. 新增 **[!UICONTROL Webhook]** >**[!UICONTROL 自訂Webhook]** 立即觸發模組至您的情境。

1. 按一下 **[!UICONTROL 新增]** 在Webhook欄位旁邊，並輸入新webhook的名稱。
1. （可選）按一下 **[!UICONTROL 進階設定]**.
1. 在 **[!UICONTROL IP限制]** 欄位中，輸入模組可接受資料的IP位址清單（以逗號分隔）。
1. 按一下 **[!UICONTROL 儲存]**

建立webhook後，會顯示唯一的URL。 這是webhook傳送資料的地址。 Workfront Fusion會驗證傳送到此位址的資料，然後將其傳遞以在情境中處理。

>[!NOTE]
>
>建立webhook後，您可以一次用於多個情境。

### 設定webhook的資料結構 {#configure-the-webhook-s-data-structure}

為了識別傳入有效負載的資料結構， [!DNL Workfront Fusion] 解析您傳送至顯示位址的範例資料。 您可以變更服務或應用程式，讓該服務或應用程式呼叫webhook，以提供範例資料。 例如，您可以移除檔案。

或者，您可以遵循以下步驟，透過以下方式傳送範例資料： [!UICONTROL HTTP] > [!UICONTROL 提出要求] 模組。

1. 使用建立新情境 **[!UICONTROL HTTP]** > **[!UICONTROL 提出要求]** 模組

1. 使用下列值設定模組：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><p>[！UICONTROL URL] </p></td> 
      <td>輸入webhook的URL。 您可以在用來設定webhook的[！UICONTROL Webhook]模組中找到此URL。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL方法] </td> 
      <td><p>[！UICONTROLPOST]</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL主體型別]</td> 
      <td><p> [！UICONTROL Raw]</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL內容型別]</td> 
      <td><p> JSON (application/json)</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL要求內容]</td> 
      <td><p>webhook中需要原始JSON</p></td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/new-scenario-set-up-like-this-350x446.png)

1. 使用開啟情境 [!UICONTROL Webhook] 在個別的瀏覽器標籤或視窗中放入模組。
1. 在webhooks模組中，按一下 **[!UICONTROL 重新決定資料結構]**.

   您不需要從Webhook模組取消連結其他模組。

1. 切換至具有的情境 [!UICONTROL HTTP] 模組並執行。
1. 切換回使用Webhooks模組的情境。

   A &quot;[!UICONTROL 已成功確定]「訊息表示模組已成功判斷資料結構。

   ![](assets/successfully-determined-350x175.png)

1. 按一下 **[!UICONTROL 確定]** 以儲存資料結構。

   webhook的專案現在可以在對應面板中使用，以便與案例中的後續模組一起使用。

## 佇列

如果webhook收到資料，而且沒有預期該資料的作用中案例，則資料會儲存在佇列中。 啟用案例後，它會依序處理佇列中所有等待的組合。

>[!IMPORTANT]
>
>Webhook佇列在使用相同webhook的情境之間共用。 如果其中一個案例停用，所有傳入資料都會保留在佇列中。

## 支援的傳入資料格式

[!DNL Workfront Fusion] 支援3種傳入資料格式： [!UICONTROL 查詢字串]， [!UICONTROL 表單資料] 和 [!UICONTROL JSON].

[!DNL Workfront Fusion] 依據選取的資料結構驗證所有傳入資料。 然後，根據情境的設定，資料會儲存在佇列中以供處理，或立即處理。

如果資料的任何部分未通過驗證， [!DNL Workfront Fusion] 會傳回400 HTTP狀態代碼，並在HTTP回應內文中指定傳入資料未通過驗證檢查的原因。 如果傳入資料的驗證成功，Workfront Fusion會傳回「[!UICONTROL 200個已接受]「狀態。

* [[!UICONTROL 查詢字串]](#query-string)
* [[!UICONTROL 表單資料]](#form-data)
* [[!UICONTROL JSON]](#json)

### [!UICONTROL 查詢字串]

```
GET https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>?name=<yourname>&job=automate
```

### [!UICONTROL 表單資料]

```
POST https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>

Content-Type: application/x-www-form-urlencoded

name=<yourname>&job=automate
```

#### 多部分表單資料

```
POST https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>


Content-Type: multipart/form-data; boundary=---generatedboundary

---generatedboundary

Content-Disposition: form-data; name="file"; filename="file.txt"


Content-Type: text/plain


Content of file.txt


---generatedboundary

Content-Disposition: form-data; name="name"

Workfront Fusion

---generatedboundary
```

為了接收以編碼的檔案 `multipart/form-data`，您必須使用設定資料結構 `collection` 包含巢狀欄位的型別欄位 `name`， `mime`、和 `data`. 欄位 `name` 是 `text` 輸入並包含已上傳檔案的名稱。 此 `mime` 是 `text` 型別並包含MIME格式的檔案。 欄位 `data` 是 `buffer` 型別並包含所傳輸檔案的二進位資料。

如需MIME格式的詳細資訊，請參閱 [mime模組](../../workfront-fusion/apps-and-their-modules/mime.md).

### [!UICONTROL JSON]

```
POST https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>

Content-Type: application/json

{"name": "Workfront Fusion", "job": "automate"}
```

>[!TIP]
>
>如果您想要存取原始JSON，請在設定webhook時啟用JSON傳遞。
>
>1. 按一下 **[!UICONTROL 新增]** 以新增新的webhook。
>1. 按一下 **[!UICONTROL 顯示進階設定]**.
>1. 按一下 **[!UICONTROL JSON傳遞]**.
>

## Webhook標頭

若要存取webhook的標頭，請在設定webhook時啟用Get要求標頭。

1. 按一下 **[!UICONTROL 新增]** 以新增新的webhook。
1. 按一下 **[!UICONTROL 顯示進階設定]**.
1. 按一下 **[!UICONTROL 取得請求標頭]**.

您可以使用以下組合來擷取特定的標頭值： `map()` 和 `get()` 函式。

>[!INFO]
>
>**範例:**
>
>以下範例顯示一個公式，用於擷取 `authorization` 標題來自 `Headers[]` 陣列。 此公式用於篩選條件，該篩選條件會將擷取的值與指定文字進行比較，以僅在有相符專案時傳遞Webhook。
>
>![](assets/set-up-a-filter-350x169.png)
>
>如需使用指定索引鍵取得陣列元素的進一步資訊，請參閱 [使用指定索引鍵對應陣列的元素](../../workfront-fusion/mapping/map-information-between-modules.md#mapping) 在文章中 [在Adobe Workfront Fusion中將資訊從一個模組對應到另一個模組](../../workfront-fusion/mapping/map-information-between-modules.md).

## 回應Webhook

webhook呼叫的預設回應是文字「已接受」。 回應會傳回至應用程式，該應用程式會在執行自訂Webhook模組期間呼叫webhook。

* [測試對webhook的回應](#test-the-response-to-a-webhook)
* [HTML回應範例](#html-response-example)
* [重新導向範例](#redirect-example)

### 測試對webhook的回應

1. 包含 **[!UICONTROL 自訂Webhook]** 模組。
1. 將新的webhook新增至模組。
1. 將webhook URL複製到剪貼簿。
1. 執行情境。

   上的閃電圖示 [!UICONTROL 自訂Webhook] 模組會變更為旋轉點。 這顯示模組現在正等候webhook呼叫。

1. 開啟新的瀏覽器視窗，將複製的URL貼到網址列並按下 **[!UICONTROL 輸入]**.

   此 [!UICONTROL 自訂Webhook] 模組已觸發，且瀏覽器會顯示新頁面。

如果要自訂webhook的回應，請採用模組Webhook回應。

模組的設定包含兩個欄位： [!UICONTROL 狀態] 和 [!UICONTROL 內文].

* 此 [!UICONTROL 狀態] 欄位包含HTTP回應狀態代碼，例如2xx for Success (例如 `200` 對於「確定」(OK)，3xx表示「重新導向」(Redirection) (例如， `307` 對於暫時重新導向)，4xx代表使用者端錯誤(例如， `400` （針對錯誤請求），依此類推。

* 此 [!UICONTROL 內文] 欄位包含webhook呼叫將接受的任何內容。 可以是簡單文字、HTML、XML、JSON等。

  >[!TIP]
  >
  >我們建議設定 `Content-Type` 標頭至對應的MIME型別： `text/plain` 如果是純文字， `text/html` 若為HTML， `application/json` 若為JSON， `application/xml` 適用於XML等。 如需MIME型別的詳細資訊，請參閱 [mime模組](../../workfront-fusion/apps-and-their-modules/mime.md).

傳送回應的逾時為40秒。 如果該期間內沒有回應，Workfront Fusion會傳回「200已接受」狀態。

### HTML回應範例

>[!INFO]
>
>**範例:**
>
>設定 [!UICONTROL Webhook回應] 模組如下：
>
><table style="table-layout:auto"> 
&gt; <col> 
&gt; <col> 
&gt; <tbody> 
&gt;  <tr> 
&gt;   <td role="rowheader">[！UICONTROL狀態] </td> 
&gt;   <td> <p>2xx成功HTTP狀態碼，例如200</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader">[！UICONTROL內文] </td> 
&gt;   <td> <p>HTML代碼</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader"> <p>[！UICONTROL自訂標頭]</p> </td> 
&gt;   <td> 
&gt;    <ul> 
&gt;     <li><strong>金鑰</strong>：內容型別</li> 
&gt;     <li><strong>值</strong>：text/html</li> 
&gt;    </ul> </td> 
&gt;  </tr> 
&gt; </tbody> 
&gt;</table>
>
>![](assets/custom-headers-350x235.png)
>
>這會產生HTML回應，並顯示在網頁瀏覽器中：
>
>![](assets/html-response-350x70.png)

### 重新導向範例

>[!INFO]
>
>**範例：** 設定 [!UICONTROL Webhook回應] 模組如下：
>
><table style="table-layout:auto"> 
&gt; <col> 
&gt; <col> 
&gt; <tbody> 
&gt;  <tr> 
&gt;   <td role="rowheader">[！UICONTROL狀態] </td> 
&gt;   <td> <p>3xx重新導向HTTP狀態代碼，例如303</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader"> <p>[！UICONTROL自訂標頭]</p> </td> 
&gt;   <td> 
&gt;    <ul> 
&gt;     <li><strong>[！UICONTROL索引鍵]</strong>：位置</li> 
&gt;     <li><strong>[！UICONTROL值]</strong>：您要重新導向的URL。</li> 
&gt;    </ul> </td> 
&gt;  </tr> 
&gt; </tbody> 
&gt;</table>
>
>![](assets/webhook-response-350x279.png)

## Webhook停用

如果符合下列任一條件，Webhook就會自動停用：

* webhook已超過5天未連線至任何案例
* webhook僅用於非使用中情境，這些情境已非使用中超過30天。

如果停用的Webhook未連線到任何情境且處於停用狀態超過30天，則會自動刪除和取消註冊。


## 疑難排解

### 對應面板中缺少專案

如果在模組之後的設定中，對應面板中缺少某些專案，請 [!UICONTROL Webhook] > [!UICONTROL 自訂Webhook] 模組，按一下 **[!UICONTROL Webhook] > [!UICONTROL 自訂Webhook]** 模組，以開啟其設定並按一下 **[!UICONTROL 重新決定資料結構]**：

![](assets/redetermine-data-structure-btn-350x195.png)

然後遵循一節中所述的步驟 [設定webhook的資料結構](#configure-the-webhook-s-data-structure) 本文章內容。
