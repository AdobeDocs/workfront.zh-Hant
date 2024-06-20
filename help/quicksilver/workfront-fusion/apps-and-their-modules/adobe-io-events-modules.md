---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: 「Adobe I/O事件模組」
description: 「使用Adobe I/O事件模組，您可以根據Adobe應用程式中的事件啟動Adobe Workfront Fusion案例。」
author: Becky
feature: Workfront Fusion, Digital Content and Documents
source-git-commit: 508f21b6860f13a9cf2a5b19713ed70aaba638c3
workflow-type: tm+mt
source-wordcount: '897'
ht-degree: 1%

---

# Adobe I/O事件模組

您可以使用「Adobe I/O事件」模組，根據沒有專用Adobe Workfront Fusion聯結器的Adobe帳戶和服務中的事件來啟動Workfront Fusion案例。

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>Pro或更高</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計畫、工作</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion授權**</td> 
   <td> <p>適用於工作自動化和整合的Workfront Fusion </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>您的組織必須購買Adobe Workfront Fusion以及Adobe Workfront，才能使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

&#42;&#42;如需Adobe Workfront Fusion授權的相關資訊，請參閱 [Adobe Workfront Fusion授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 先決條件

使用Adobe I/O事件聯結器之前，您必須確保符合下列先決條件：

* 您必須擁有使用中的Adobe帳戶。

## 建立與Adobe I/O事件的連線

若要建立「Adobe I/O事件」模組的連線：

1. 按一下「連線」方塊旁的「新增」。

1. 填寫下列欄位：

   <table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
      <tr>
        <td role="rowheader">連線名稱</td>
        <td>
          <p>輸入此連線的名稱。</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">類型</td>
        <td>
          <p>選取您要連線到服務帳戶或個人帳戶。</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">其他範圍</td>
        <td>若要新增任何其他範圍，請按一下 <b>新增專案</b> 並輸入範圍。</td>
      </tr>
      <tr>
        <td role="rowheader">用戶端 ID</td>
        <td>輸入您的Adobe使用者端ID。 您可以在Adobe Developer Console的「認證詳細資訊」區段中找到</td>
      </tr>
      <tr>
        <td role="rowheader">用戶端密碼</td>
        <td>輸入您的Adobe使用者端密碼。 您可以在Adobe Developer Console的「認證詳細資訊」區段中找到</td>
      </tr>
      </tr>
        <tr>
        <td role="rowheader">消費者組織ID</td>
        <td>輸入您的消費者組織ID。 您可以在專案的認證URL中找到此專案： <code>https://developer.adobe.com/console/projects/{consumer org ID}/ {project ID}/credentials/{credential ID}/details</code></td>
      </tr>
      <tr>
        <td role="rowheader">認證ID</td>
        <td>輸入您的認證識別碼。 您可以在專案的認證URL中找到此專案： <code>https://developer.adobe.com/console/projects/{consumer org ID}/ {project ID}/credentials/{credential ID}/details</code></td>
      </tr>
      <tr>
        <td role="rowheader">IMS組織ID</td>
        <td>輸入您的Adobe組織ID。 您可以在Adobe Developer Console的「認證詳細資訊」區段中找到</td>
      </tr>
        <tr>
        <td role="rowheader">專案識別碼</td>
        <td>輸入您的專案ID。 您可以在專案的認證URL中找到此專案： <code>https://developer.adobe.com/console/projects/{consumer org ID}/ {project ID}/credentials/{credential ID}/details</code></td>
      </tr>
      <tr>
        <td role="rowheader">工作區ID</td>
        <td>輸入您的工作區ID。 </td>
      </tr>
    </tbody>
    </table>

1. 按一下 **繼續** 以儲存連線並返回模組。

## Adobe I/O事件模組及其欄位

當您設定 [!DNL Adobe I/O Events] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 除了這些以外， [!DNL Adobe I/O Events] 欄位可能會顯示，端視您應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [在中將資訊從一個模組對應到另一個模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [觸發器](#triggers)
* [動作](#actions)
* [搜尋](#searches)

### 觸發器

#### 建立事件註冊

此動作模組使用webhook建立事件說明。 您可以在這裡設定webhook。 如果您使用現有的webhook，則此模組中的欄位為唯讀。

若要建立webhook：

1. 按一下 **新增** ，位於Webhook欄位旁。
1. 填寫下列欄位：

   <table>
     <col/>
     <col/>
     <tbody>
       <tr>
         <td role="rowheader">[！UICONTROL Webhook名稱]</td>
        <td>輸入此webhook的名稱。</td>
       </tr>
       <tr>
         <td role="rowheader">[！UICONTROL Connection]</td>
        <td>有關建立與的連線的指示 [!DNL Adobe I/O Events]，請參閱 <a href="#create-a-connection-to-adobe-io-events" class="MCXref xref" >建立與的連線 [!DNL Adobe I/O Events]</a> 本文章內容。</td>
       </tr>
       <tr>
         <td role="rowheader">
           [！UICONTROL Webhook說明]
         </td>
         <td>
           輸入此webhook的說明。
        </td>
       </tr>
       <tr>
         <td role="rowheader">
           [！UICONTROL事件提供者]
         </td>
         <td>
           選取您要建立事件的來源產品或帳戶。
         </td>
       </tr>
       <tr>
         <td role="rowheader">
           [！UICONTROL事件型別]
         </td>
         <td>
           選取您希望webhook觀看的活動。 這些事件發生時會觸發此情境。
         </td>
       </tr>
     </tbody>
   </table>

1. 按一下儲存，儲存webhook並返回模組。

### 動作

#### 從日誌取得所有事件

此搜尋模組會從日誌中擷取註冊的所有事件。

<table>
     <col/>
     <col/>
     <tbody>
       <tr>
         <td role="rowheader">[！UICONTROL Connection]</td>
        <td>有關建立與的連線的指示 [!DNL Adobe I/O Events]，請參閱 <a href="#create-a-connection-to-adobe-io-events" class="MCXref xref" >建立與的連線 [!DNL Adobe I/O Events]</a> 本文章內容。</td>
       </tr>
       <tr>
         <td role="rowheader">
           [！UICONTROL註冊ID]
         </td>
         <td>
           選取您要擷取事件的註冊。
        </td>
       </tr>
       <tr>
         <td role="rowheader">
           [！UICONTROL傳回記錄的最大數量]
         </td>
         <td>
              輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。 
         </td>
       </tr>
       <tr>
         <td role="rowheader">
           [！UICONTROL傳回發生於]之後的事件
         </td>
         <td>
         </td>
       </tr>
       <tr>
         <td role="rowheader">
           [！UICONTROL Seek]
         </td>
         <td>
         </td>
       </tr>
       <tr>
         <td role="rowheader">
           [！UICONTROL Latest]
         </td>
         <td>
         啟用此選項以傳回最新事件。
         </td>
       </tr>
     </tbody>
   </table>

#### 進行自訂API呼叫

此動作模組會對 [!DNL Adobe I/O Events] API

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[！UICONTROL Connection]</td>
        <td>有關建立與的連線的指示 [!DNL Adobe I/O Events]，請參閱 <a href="#create-a-connection-to-adobe-io-events" class="MCXref xref" >建立與的連線 [!DNL Adobe I/O Events]</a> 本文章內容。</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL路徑]</p>
      </td>
      <td>
        <p>輸入相對於 <code>https://api.adobe.io/events</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL方法]</p>
      </td>
      <td>
  <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p>  
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Headers]</td>
      <td>
        <p>以標準JSON物件的形式新增請求的標頭。</p>
        <p>例如， <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion會自動新增授權標題和x-api-key標題。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL查詢字串]  </td>
      <td>
        <p>輸入請求查詢字串。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Body]</td>
   <td> <p>以標準JSON物件的形式新增API呼叫的內文內容。</p> <p>注意：  <p>使用條件陳述式時，例如 <code>if</code> 在JSON中，將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

### 搜尋

#### 取得提供者和事件ID

此搜尋模組取得指定之提供者和事件的Adobe I/O事件ID。

<table>
     <col/>
     <col/>
     <tbody>
       <tr>
         <td role="rowheader">[！UICONTROL Connection]</td>
        <td>有關建立與的連線的指示 [!DNL Adobe I/O Events]，請參閱 <a href="#create-a-connection-to-adobe-io-events" class="MCXref xref" >建立與的連線 [!DNL Adobe I/O Events]</a> 本文章內容。</td>
       </tr>
       <tr>
         <td role="rowheader">
           [！UICONTROL事件提供者]
         </td>
         <td>
           選取您要擷取ID的提供者。
        </td>
       </tr>
       <tr>
         <td role="rowheader">
           [！UICONTROL事件型別]
         </td>
         <td>
              選取您要提供ID的事件。 根據事件提供者，可使用事件。 
         </td>
       </tr>
     </tbody>
   </table>

<!--

Watch Events

This trigger module starts a scenario when an event occurs in the chosen Adobe product or service.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">Webhook</td> 
   <td><p>Select the webhook that you want to use for this trigger, or add a new webhook. </p><p>To add a new webhook, <ol><li>Click <b>Add</b> next to the webhook field.</li><li>Enter the following: <ul><li>A name for the webhook</li><li>The connection that you want to use for this webhook</li><li>The source of the events you want to watch</li></ul></li><li>Click <b>Save</b> to save the webhook and return to the module. </td> 
   </tr> 
   </tbody> 
</table>

-->

