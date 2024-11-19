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
source-git-commit: 34d7edb6a3f9cb1e818f6c234a8dda88d01c5fc4
workflow-type: tm+mt
source-wordcount: '1449'
ht-degree: 0%

---

# Webhook



<!--This information moved to the webhooks article in the create scenarios folders in the new repo-->

webhook是由事件觸發的HTTP呼叫。 您可以使用Webhook來啟動即時觸發程式模組。 任何連線至網際網路並允許HTTP請求的應用程式都可以將Webhook傳送至Adobe Workfront Fusion。

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

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

&#42;&#42;如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 在[!DNL Workfront Fusion]中使用webhook

>[!NOTE]
>
>若要呼叫第三方webhook （傳出webhook），請使用其中一個HTTP模組。 如需詳細資訊，請參閱[HTTP模組](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md)。

若要使用webhook將應用程式連線到[!DNL Workfront Fusion]：

1. 將&#x200B;**[!UICONTROL Webhook]** >**[!UICONTROL 自訂Webhook]**&#x200B;即時觸發模組新增至您的情境。

1. 按一下Webhook欄位旁的&#x200B;**[!UICONTROL 新增]**，然後輸入新webhook的名稱。
1. （選擇性）按一下&#x200B;**[!UICONTROL 進階設定]**。
1. 在&#x200B;**[!UICONTROL IP限制]**&#x200B;欄位中，輸入模組可以接受資料的IP位址清單（以逗號分隔）。
1. 按一下&#x200B;**[!UICONTROL 儲存]**

建立webhook之後，會顯示唯一的URL。 這是webhook傳送資料的地址。 Workfront Fusion會驗證傳送到此位址的資料，然後傳遞它以用於案例中的處理。

>[!NOTE]
>
>建立webhook後，您可以一次用於多個情境。

### 設定webhook的資料結構 {#configure-the-webhook-s-data-structure}

為了識別傳入裝載的資料結構，[!DNL Workfront Fusion]會剖析您傳送至顯示位址的範例資料。 您可以變更服務或應用程式，讓該服務或應用程式呼叫webhook，以提供範例資料。 例如，您可以移除檔案。

或者，您可以依照下列步驟，透過[!UICONTROL HTTP] > [!UICONTROL 提出要求]模組傳送範例資料。

1. 使用&#x200B;**[!UICONTROL HTTP]** > **[!UICONTROL 提出要求]**&#x200B;模組建立新情境

1. 使用下列值設定模組：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><p>[！UICONTROL URL] </p></td> 
      <td>輸入webhook的URL。 您可以在用來設定webhook的[！UICONTROL Webhooks]模組中找到此URL。</td> 
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

1. 在單獨的瀏覽器標籤或視窗中開啟具有[!UICONTROL Webhooks]模組的情境。
1. 在webhooks模組中，按一下&#x200B;**[!UICONTROL 重新決定資料結構]**。

   您不需要從webhooks模組取消連結其他模組。

1. 切換至具有[!UICONTROL HTTP]模組的情境並執行它。
1. 切換回使用Webhooks模組的情境。

   「[!UICONTROL 已成功判定]」訊息表示模組已成功判定資料結構。

   ![](assets/successfully-determined-350x175.png)

1. 按一下&#x200B;**[!UICONTROL 確定]**&#x200B;以儲存資料結構。

   webhook的專案現在可以在對應面板中使用，以便與案例中的後續模組一起使用。

## webhook佇列

如果webhook收到資料，而且沒有作用中案例需要該資料，則資料會儲存在佇列中。 啟用情境後，它會依序處理佇列中等待的所有組合。

>[!IMPORTANT]
>
>Webhook佇列在使用相同webhook的情境之間共用。 如果其中一個案例已停用，所有傳入資料都會保留在佇列中。

## 支援的傳入資料格式

[!DNL Workfront Fusion]支援3種傳入資料格式： [!UICONTROL 查詢字串]、[!UICONTROL 表單資料]和[!UICONTROL JSON]。

[!DNL Workfront Fusion]會根據選取的資料結構驗證所有傳入的資料。 然後，根據情境的設定，資料會儲存在佇列中以供處理，或立即處理。

如果資料的任何部分未通過驗證，[!DNL Workfront Fusion]會傳回400 HTTP狀態代碼，並在HTTP回應的內文中指定傳入資料未通過驗證檢查的原因。 如果傳入資料的驗證成功，Workfront Fusion會傳回&quot;[!UICONTROL 200 Accepted]&quot;狀態。

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

若要接收以`multipart/form-data`編碼的檔案，您必須使用`collection`型別欄位來設定資料結構，該欄位包含巢狀欄位`name`、`mime`和`data`。 欄位`name`是`text`型別，包含上傳檔案的名稱。 `mime`是`text`型別，並包含MIME格式的檔案。 欄位`data`是`buffer`型別，包含正在傳輸之檔案的二進位資料。

如需MIME格式的詳細資訊，請參閱[MIME模組](../../workfront-fusion/apps-and-their-modules/mime.md)。

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
>1. 按一下&#x200B;**[!UICONTROL [新增]**]以新增新的webhook。
>1. 按一下&#x200B;**[!UICONTROL 顯示進階設定]**。
>1. 按一下&#x200B;**[!UICONTROL JSON傳遞]**。
>

## Webhook標題

若要存取webhook的標頭，請在設定webhook時啟用Get要求標頭。

1. 按一下&#x200B;**[!UICONTROL [新增]**]以新增新的webhook。
1. 按一下&#x200B;**[!UICONTROL 顯示進階設定]**。
1. 按一下&#x200B;**[!UICONTROL 取得要求標題]**。

您可以使用`map()`和`get()`函式的組合來擷取特定的標頭值。

>[!INFO]
>
>**範例：**
>
>下列範例顯示從`Headers[]`陣列中擷取`authorization`標頭值的公式。 此公式會用於比較擷取值與指定文字的篩選中，以便只傳遞符合的Webhook。
>
>![](assets/set-up-a-filter-350x169.png)
>
>如需有關使用指定索引鍵取得陣列元素的進一步資訊，請參閱文章[在Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md)中將資訊從一個模組對應到另一個模組[將具有指定索引鍵](../../workfront-fusion/mapping/map-information-between-modules.md#mapping)的陣列元素對應。

## 回應Webhook

webhook呼叫的預設回應是文字「已接受」。 回應會傳回至應用程式，該應用程式會在執行自訂Webhook模組期間呼叫webhook。

* [測試對webhook的回應](#test-the-response-to-a-webhook)
* [HTML回應範例](#html-response-example)
* [重新導向範例](#redirect-example)

### 測試對webhook的回應

1. 在您的情境中加入&#x200B;**[!UICONTROL 自訂Webhook]**&#x200B;模組。
1. 將新的webhook新增至模組。
1. 將webhook URL複製到剪貼簿。
1. 執行情境。

   [!UICONTROL 自訂Webhook]模組上的閃電圖示會變更為旋轉的點。 這顯示模組現在正等候webhook呼叫。

1. 開啟新的瀏覽器視窗，將複製的URL貼到網址列，然後按&#x200B;**[!UICONTROL Enter]**。

   已觸發[!UICONTROL 自訂Webhook]模組，瀏覽器將顯示新頁面。

如果要自訂webhook的回應，請採用模組Webhook回應。

模組的設定包含兩個欄位： [!UICONTROL 狀態]和[!UICONTROL 內文]。

* [!UICONTROL Status]欄位包含HTTP回應狀態代碼，例如，2xx代表Success （例如，`200`代表OK）、3xx代表Redirection （例如，`307`代表Temporary Redirect）、4xx代表Client errors （例如，`400`代表Bad Request）等等。

* [!UICONTROL Body]欄位包含webhook呼叫將接受的任何內容。 可以是簡單文字、HTML、XML、JSON等。

  >[!TIP]
  >
  >建議將`Content-Type`標頭設定為對應的MIME型別： `text/plain`用於純文字，`text/html`用於HTML，`application/json`用於JSON，`application/xml`用於XML等等。 如需MIME型別的詳細資訊，請參閱[MIME模組](../../workfront-fusion/apps-and-their-modules/mime.md)。

傳送回應的逾時為40秒。 如果在該期間內沒有回應，Workfront Fusion會傳回「200已接受」狀態。

### HTML回應範例

>[!INFO]
>
>**範例：**
>
>設定[!UICONTROL Webhook回應]模組，如下所示：
>
><table style="table-layout:auto"> 
&gt; <col> 
&gt; <col> 
&gt; <tbody> 
&gt;  <tr> 
&gt;   <td role="rowheader">[！UICONTROL狀態] </td> 
&gt;   <td> <p>2xx成功HTTP狀態代碼，例如200</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader">[！UICONTROL Body] </td> 
&gt;   <td> <p>HTML代碼</p> </td> 
&gt;  </tr> 
&gt;  <tr> 
&gt;   <td role="rowheader"> <p>[！UICONTROL自訂標頭]</p> </td> 
&gt;   <td> 
&gt;    <ul> 
&gt;     <li><strong>索引鍵</strong>： Content-type</li> 
&gt;     <li><strong>值</strong>： text/html</li> 
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
>**範例：**&#x200B;設定[!UICONTROL Webhook回應]模組，如下所示：
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
* webhook僅用於非使用中情況，這些情況已非使用中超過30天。

如果停用的Webhook未連線至任何情境且處於停用狀態超過30天，則會自動刪除和取消註冊。


## 疑難排解

### 對應面板中缺少專案

如果遵循[!UICONTROL Webhooks] > [!UICONTROL 自訂Webhook]模組的模組設定中的對應面板遺漏某些專案，請按一下&#x200B;**[!UICONTROL Webhooks] > [!UICONTROL 自訂Webhook]**&#x200B;模組以開啟其設定，然後按一下&#x200B;**[!UICONTROL 重新決定資料結構]**：

![](assets/redetermine-data-structure-btn-350x195.png)

然後遵循本文中[設定webhook的資料結構](#configure-the-webhook-s-data-structure)一節中所述的步驟。
