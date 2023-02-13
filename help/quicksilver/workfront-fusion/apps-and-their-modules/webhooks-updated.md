---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Webhook
description: 網頁連結是由事件觸發的HTTP呼叫。 您可以使用Webhook來啟用即時觸發模組。 任何連線至網際網路且允許HTTP要求的應用程式都可將Webhook傳送至Adobe Workfront Fusion。
author: Becky
feature: Workfront Fusion
exl-id: 987544a4-5840-40d4-9438-41a000aa22ee
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1391'
ht-degree: 0%

---

# Webhook

網頁連結是由事件觸發的HTTP呼叫。 您可以使用Webhook來啟用即時觸發模組。 任何連線至網際網路且允許HTTP要求的應用程式都可將Webhook傳送至Adobe Workfront Fusion。

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
   <td> <p>[!UICONTROL Workfront Fusion for Work Automation and Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr>
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

&#42;&#42;如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 在中使用網頁鈎 [!DNL Workfront Fusion]

>[!NOTE]
>
>要調用第三方Webhook（傳出Webhook），請使用其中一個HTTP模組。 如需詳細資訊，請參閱 [HTTP模組](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md).

使用網頁連結將應用程式連結至 [!DNL Workfront Fusion]:

1. 新增 **[!UICONTROL Webhook]** >**[!UICONTROL 自訂Webhook]** 即時觸發模組至您的案例。

1. 按一下 **[!UICONTROL 新增]** 在「Webhook」欄位旁，輸入新Webhook的名稱。
1. （選用）按一下 **[!UICONTROL 進階設定]**.
1. 在 **[!UICONTROL IP限制]** 欄位中，輸入模組可接受資料的IP位址清單（以逗號分隔）。
1. 按一下 **[!UICONTROL 儲存]**

建立網頁連結後，會顯示唯一URL。 這是Webhook傳送資料的位址。 Workfront Fusion會驗證傳送至此位址的資料，然後傳遞給該位址，以便在案例中處理。

>[!NOTE]
>
>建立網頁連結後，您一次可以在多個案例中使用。

### 配置Webhook的資料結構 {#configure-the-webhook-s-data-structure}

為了識別傳入有效負載的資料結構， [!DNL Workfront Fusion] 剖析您傳送至顯示地址的範例資料。 您可以在服務或應用程式中進行變更，讓該服務或應用程式呼叫網頁鈎點，以便提供範例資料。 例如，您可以移除檔案。

或者，您可以依照下列步驟，透過 [!UICONTROL HTTP] > [!UICONTROL 提出請求] 模組。

1. 使用 **[!UICONTROL HTTP]** > **[!UICONTROL 提出請求]** 模組

1. 使用下列值設定模組：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><p>[!UICONTROL URL] </p></td> 
      <td>輸入網頁連結的URL。 您可以在您用來設定Webhook的[!UICONTROL Webhooks]模組中找到此URL。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL方法] </td> 
      <td><p>[!UICONTROLPOST]</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL主體類型]</td> 
      <td><p> [!UICONTROL Raw]</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL內容類型]</td> 
      <td><p> JSON(application/json)</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL要求內容]</td> 
      <td><p>網頁鈎點中應有原始JSON</p></td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/new-scenario-set-up-like-this-350x446.png)

1. 使用 [!UICONTROL Webhook] 模組（在個別的瀏覽器標籤或視窗中）。
1. 在Webhook模組中，按一下 **[!UICONTROL 重新確定資料結構]**.

   您不需要將其他模組與Webhook模組取消連結。

1. 切換至案例，並搭配 [!UICONTROL HTTP] 模組並執行。
1. 切換回使用Webhook模組的案例。

   A &quot;[!UICONTROL 已成功確定]「訊息表示模組已成功判斷資料結構。

   ![](assets/successfully-determined-350x175.png)

1. 按一下 **[!UICONTROL 確定]** 以儲存資料結構。

   Webhook的項目現在可在對應面板中使用，以便與案例中的後續模組搭配使用。

## 佇列

如果Webhook收到資料，且沒有預期該資料的作用中案例，則資料會儲存在佇列中。 一旦您啟動案例，它就會依序處理佇列中等待的所有套件組合。

>[!IMPORTANT]
>
>Webhook隊列在採用相同Webhook的方案之間共用。 如果禁用了其中一個方案，則所有傳入資料都會保留在隊列中。

## 支援的傳入資料格式

[!DNL Workfront Fusion] 支援3種傳入資料格式： [!UICONTROL 查詢字串], [!UICONTROL 表單資料] 和 [!UICONTROL JSON].

[!DNL Workfront Fusion] 根據所選資料結構驗證所有傳入資料。 然後，根據情境的設定，資料會儲存在佇列中以供處理，或是立即處理。

如果資料的任何部分未通過驗證， [!DNL Workfront Fusion] 傳回400 HTTP狀態代碼，並在HTTP回應內文中指定傳入資料失敗驗證檢查的原因。 如果傳入資料的驗證成功，Workfront Fusion會傳回「[!UICONTROL 200個已接受]」狀態。

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

為了接收以 `multipart/form-data`，您必須使用 `collection` 包含巢狀欄位的類型欄位 `name`, `mime`，和 `data`. 欄位 `name` 是 `text` 輸入並包含已上傳檔案的名稱。 此 `mime` 是 `text` 類型並包含MIME格式的檔案。 欄位 `data` 是 `buffer` 輸入並包含要傳輸的檔案的二進位資料。

如需MIME格式的詳細資訊，請參閱 [MIME模組](../../workfront-fusion/apps-and-their-modules/mime.md).

### [!UICONTROL JSON]

```
POST https://app.workfrontfusion.com/wh/<yourunique32characterslongstring>

Content-Type: application/json

{"name": "Workfront Fusion", "job": "automate"}
```

>[!TIP]
>
>如果您想要存取原始JSON，請在設定網頁連結時啟用JSON傳遞。
>
>1. 按一下 **[!UICONTROL 新增]** 來新增網頁連結。
>1. 按一下 **[!UICONTROL 顯示高級設定]**.
>1. 按一下 **[!UICONTROL JSON傳遞]**.

>


## 網頁鈎頭

若要存取網頁連結的標題，請在設定網頁連結時啟用「取得請求標題」 。

1. 按一下 **[!UICONTROL 新增]** 來新增網頁連結。
1. 按一下 **[!UICONTROL 顯示高級設定]**.
1. 按一下 **[!UICONTROL 取得要求標題]**.

您可以使用 `map()` 和 `get()` 函式。

>[!INFO]
>
>**範例:**
>
>以下範例顯示可擷取 `authorization` 標題 `Headers[]` 陣列。 此公式用於篩選器，該篩選器會將擷取的值與指定文字進行比較，以在有相符項目時僅傳遞Webhook。
>
>![](assets/set-up-a-filter-350x169.png)
>
>有關使用給定鍵獲取陣列元素的詳細資訊，請參見 [使用指定的鍵映射陣列的元素](../../workfront-fusion/mapping/map-information-between-modules.md#mapping) 在文章中 [在Adobe Workfront Fusion中，將資訊從一個模組對應至另一個模組](../../workfront-fusion/mapping/map-information-between-modules.md).

## 回應Webhook

網頁連結呼叫的預設回應為「已接受」文字。 回應會傳回至在執行自訂Webhook模組期間呼叫Webhook的應用程式。

* [測試對Webhook的回應](#test-the-response-to-a-webhook)
* [HTML回應範例](#html-response-example)
* [重新導向範例](#redirect-example)

### 測試對Webhook的回應

1. 納入 **[!UICONTROL 自訂Webhook]** 模組。
1. 將新網頁連結新增至模組。
1. 將網頁連結URL複製到剪貼簿。
1. 執行案例。

   閃電表徵圖 [!UICONTROL 自訂Webhook] 模組變更為旋轉點。 這表示模組現在正在等候Webhook呼叫。

1. 開啟新的瀏覽器視窗，將複製的URL貼到網址列，然後按 **[!UICONTROL 輸入]**.

   此 [!UICONTROL 自訂Webhook] 模組隨即觸發，瀏覽器將顯示新頁面。

如果您要自訂Webhook的回應，請使用模組Webhook回應。

模組的設定包含兩個欄位： [!UICONTROL 狀態] 和 [!UICONTROL 主體].

* 此 [!UICONTROL 狀態] 欄位包含HTTP回應狀態代碼，例如「成功」為2xx(例如 `200` （例如OK）、3xx(例如 `307` 若為暫時重新導向)，則為用戶端錯誤(例如 `400` Bad Request)等。

* 此 [!UICONTROL 主體] 欄位包含webhook呼叫將接受的任何內容。 它可以是簡單的文字、HTML、XML、JSON等。

   >[!TIP]
   >
   >建議您將 `Content-Type` 標題到相應的MIME類型： `text/plain` 為了純文字， `text/html` HTML, `application/json` 若為JSON, `application/xml` XML等。 如需MIME類型的詳細資訊，請參閱 [MIME模組](../../workfront-fusion/apps-and-their-modules/mime.md).

傳送回應的逾時為40秒。 如果此回應在該期間內無法使用，Workfront Fusion會傳回「200個接受」狀態。

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
&gt;   <td role="rowheader">[!UICONTROL狀態] </td> 
&gt;   <td> <p>2xx成功HTTP狀態代碼，例如200</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader">[!UICONTROL正文] </td> 
&gt;   <td> <p>HTML代碼</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader"> <p>[!UICONTROL自訂標題]</p> </td> 
&gt;   <td> 
&gt;    <ul> 
&gt;     <li><strong>金鑰</strong>:內容類型</li> 
&gt;     <li><strong>值</strong>:文字/html</li> 
&gt;    </ul> </td> 
&gt;  </tr> 
&gt; </tbody> 
&gt;</table>
>
>![](assets/custom-headers-350x235.png)
>
>這會產生顯示於網頁瀏覽器的HTML回應：
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
&gt;   <td role="rowheader">[!UICONTROL狀態] </td> 
&gt;   <td> <p>3xx重定向HTTP狀態代碼，例如303</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader"> <p>[!UICONTROL自訂標題]</p> </td> 
&gt;   <td> 
&gt;    <ul> 
&gt;     <li><strong>[!UICONTROL密鑰]</strong>:位置</li> 
&gt;     <li><strong>[!UICONTROL值]</strong>:您要重新導向至的URL。</li> 
&gt;    </ul> </td> 
&gt;  </tr> 
&gt; </tbody> 
&gt;</table>
>
>![](assets/webhook-response-350x279.png)

## Webhook停用

如果下列任一情況適用，Webhook就會自動停用：

* Webhook已超過5天未連接到任何情況
* Webhook僅用於已停用超過30天的非作用中案例。

如果停用的WebHook未連線至任何案例，且已停用30天以上，系統就會自動刪除並取消註冊。


## 疑難排解

### 映射面板中缺少項

如果在模組設定中的對應面板中缺少某些項目，則遵循 [!UICONTROL Webhook] > [!UICONTROL 自訂Webhook] 模組，按一下 **[!UICONTROL Webhook] > [!UICONTROL 自訂Webhook]** 模組，開啟其設定，然後按一下 **[!UICONTROL 重新確定資料結構]**:

![](assets/redetermine-data-structure-btn-350x195.png)

然後，請依照 [配置Webhook的資料結構](#configure-the-webhook-s-data-structure) 這篇文章。
