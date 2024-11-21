---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Adobe Acrobat Sign模組
description: 透過 [!DNL Adobe Acrobat Sign] 模組，您可以根據您 [!DNL Adobe] Acrobat Sign帳戶中的事件來啟動 [!DNL Adobe Workfront Fusion] 案例、建立、讀取或更新合約及其他記錄、使用您設定的條件搜尋記錄，以及上傳檔案。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 01158218-31a6-4c68-a9b7-6a678a8f40c9
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '6652'
ht-degree: 0%

---

# [!DNL Adobe Acrobat Sign]模組

透過[!DNL Adobe Acrobat Sign]模組，您可以根據[!DNL Adobe Acrobat Sign]帳戶中的事件來啟動[!DNL Adobe Workfront Fusion]案例、建立、讀取或更新合約及其他記錄、使用您設定的條件搜尋記錄，以及上傳檔案。

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
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]計畫，貴組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]計畫中。</p>
   <p>或</p>
   <p>舊版產品需求：您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## [!DNL Adobe Acrobat Sign] API資訊

Adobe Acrobat Sign聯結器會使用以下專案：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">API版本</td> 
   <td> v6 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API標籤</td> 
   <td>v1.35.1</td> 
  </tr>
 </tbody> 
</table>


## [!DNL Adobe Acrobat Sign]聯結器使用建議

[!DNL Adobe Sign]應用程式可讓[!DNL Fusion]中的自動化eSignature商務程式更容易、更強大。

[!DNL Adobe Sign]的新使用者應密切注意與更新合約相關的一些限制。 協定通常一經啟動便不會變更。 我們建議[!DNL Adobe Sign]的新使用者專注於使用合約建立模組來建立新合約。 這會讓[!DNL Fusion]自動化更容易，而且能更好地與[!DNL Adobe Sign]搭配使用。

[!DNL Adobe Sign]個協定需要欄位才能使用。 有幾個選項可以執行此操作，但最簡單也最常用的是上傳暫時性檔案，然後將該檔案對應至您的合約。

![](assets/adobe-sign-recommendations-350x168.png)

## [!DNL Adobe Acrobat Sign]模組及其欄位

當您設定[!DNL Adobe Acrobat Sign]模組時，[!DNL Workfront Fusion]會顯示下列欄位。 除了這些欄位以外，可能還會顯示其他[!DNL Adobe Acrobat Sign]欄位，視您在應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中將資訊從一個模組對應到另一個模組。

![](assets/map-toggle-350x74.png)

* [觸發器](#triggers)
* [動作](#actions)
* [搜尋](#searches)

### 觸發器

<!--
* [Watch for agreements](#watch-for-agreements) 
* [Watch for events](#watch-for-events)
-->

+++ **[!UICONTROL 觀看合約]**

此觸發模組會在建立或更新協定時啟動案例。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
<td>如需有關將您的[!DNL Adobe Acrobat Sign]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a></td>  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL篩選器]</td> 
   <td>選取您要監視新記錄、更新記錄或兩者。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別] </td> 
   <td>選取您要記錄觀看的記錄型別。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL尋找文字]</td> 
   <td> <p>輸入您要搜尋的字詞。 模組會傳回包含這些字詞作為欄位值的記錄。</p> <p>如需在[!DNL Adobe Acrobat Sign]中搜尋欄位的詳細資訊，請參閱<a href="https://helpx.adobe.com/sign/using/adobesign-search-users-agreements.html#HowSearchWorks">Adobe Sign搜尋中的「文字搜尋如何運作」 — 其運作方式</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL傳回協定的最大數目]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 觀看活動]**

當您選取的事件發生時，此觸發模組就會啟動案例。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Webhook]</td> 
   <td>選取您要使用的webhook，或按一下<b>[！UICONTROL新增]</b>並填入下列欄位。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Webhook名稱]</td> 
   <td> <p>輸入webhook的名稱</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Adobe Acrobat Sign]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL範圍]</td> 
   <td> 
    <ul> 
     <li> <p>[！UICONTROL帳戶]</p> </li> 
     <li> <p>[！UICONTROL群組]</p> </li> 
     <li> <p>[！UICONTROL使用者]</p> </li> 
     <li> <p>[！UICONTROL資源]</p> <p>如果您選取[！UICONTROL Resource]，請輸入資源ID和資源型別。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資源層級]</td> 
   <td> <p>選取您要觀看的資源型別。</p> 
    <ul> 
     <li> <p>[！UICONTROL合約]</p> </li> 
     <li> <p>[！UICONTROL Widget]</p> </li> 
     <li> <p>[！UICONTROL Megasigns]</p> </li> 
     <li> <p>[！UICONTROL資料庫檔案]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Webhook訂閱事件]</td> 
   <td>選取您希望模組觀看的[!DNL Adobe Sign]個事件。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL應用程式顯示名稱]</td> 
   <td>建立webhook時所使用的應用程式的顯示名稱。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL應用程式名稱]</td> 
   <td>建立webhook時所使用的應用程式的顯示名稱。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL問題通知電子郵件]</td> 
   <td> <p>此設定僅適用於管理員帳戶</p> <p>針對您想要傳送問題通知電子郵件的每個電子郵件地址，按一下<b>[！UICONTROL新增]</b>並輸入電子郵件地址。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Agreement條件引數]</td> 
   <td>如果要新增任何條件引數，請在要新增引數的記錄型別上選取<b>[！UICONTROL是]</b>，然後在要啟用的任何引數上選取<b>[！UICONTROL是]</b>。</td> 
  </tr> 
 </tbody> 
</table>

+++

### 動作

<!--
* [Create a record](#create-a-record) 
* [Create an agreement](#create-an-agreement) 
* [Create related records](#create-related-records) 
* [Custom API Call](#custom-api-call) 
* [List records](#list-records) 
* [Read a record](#read-a-record) 
* [Read related records](#read-related-records) 
* [Update a record](#update-a-record) 
* [Update related record](#update-related-record) 
* [Upload document](#upload-document)
-->

+++ **[!UICONTROL 建立記錄]**

此動作模組會建立所選型別的新記錄。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>如需有關將您的[!DNL Adobe Acrobat Sign]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers]</td> 
   <td>以標準JSON物件的形式新增請求的標頭。例如， <code>{"Content-type":"application/json"}</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別]</td> 
   <td> <p>選取您要建立的記錄型別。</p> 
    <ul> 
     <li> <p><b>[！UICONTROL群組]</b> </p> </li> 
     <li> <p><b>[！UICONTROL資料庫檔案]</b> </p> </li> 
     <li> <p><b>[！UICONTROL使用者]</b> </p> </li> 
     <li> <p><b>[！UICONTROL網頁表單] ([！UICONTROL Widget])</b> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL群組資訊]</td> 
   <td> <p>輸入或對應群組的[！UICONTROL名稱]和[！UICONTROL ID]，並指示此群組是否為帳戶的預設群組。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資料庫檔案資訊]</td> 
   <td> <p>填寫下列欄位：</p> 
    <ul> 
     <li> <p>要傳送的<b>[！UICONTROL檔案]</b> </p> <p>對於每個要新增的檔案，按一下<b>[！UICONTROL新增專案]</b>並填入欄位。</p> 
      <ul> 
       <li><b>[！UICONTROL暫時性檔案識別碼]</b> <p>輸入暫時性檔案的識別碼</p> </li> 
       <li> <p><b>[！UICONTROL URL檔案傳輸]</b> </p> <p>填寫下列欄位：</p> 
        <ul> 
         <li> <p><b>[！UICONTROL Mime-Type]</b> </p> <p>輸入原始檔案的mime型別。 多用途網際網路郵件延伸模組(MIME)型別是標籤，可讓軟體識別網際網路上共用的不同資料型別。 Web伺服器和瀏覽器會使用MIME型別來決定應該對檔案執行的操作。 例如，MIME型別為<code>text/html</code>的檔案在瀏覽器中的處理方式與MIME型別為<code>image/jpeg</code>的檔案不同。</p> </li> 
         <li> <p><b>[！UICONTROL名稱]</b> </p> <p>輸入檔案的名稱。</p> </li> 
         <li> <p><b>[！UICONTROL URL]</b> </p> <p>輸入您要傳送之檔案的URL。</p> </li> 
        </ul> </li> 
       <li> <p><b>[！UICONTROL Notarize]</b> </p> <p>選取是否需要將此檔案公證。</p> </li> 
      </ul> </li> 
     <li> <p><b>[！UICONTROL程式庫範本名稱]</b> </p> <p>輸入或對應程式庫範本的名稱</p> </li> 
     <li> <p><b>[！UICONTROL共用模式]</b> </p> <p>指定應該擁有程式庫檔案存取權的使用者。</p> </li> 
     <li> <p><b>[！UICONTROL程式庫檔案狀態]</b> </p> <p>選擇檔案是處於編寫狀態還是使用中。</p> </li> 
     <li> <p><b>[！UICONTROL程式庫範本型別]</b> </p> <p>針對您要使用的每個程式庫範本型別，按一下<b>[！UICONTROL新增專案]</b>並選取範本型別。</p> </li> 
     <li> <p><b>[！UICONTROL上次事件日期]</b> </p> <p>輸入程式庫檔案發生事件的最後日期。</p> <p>如需支援的日期和時間格式清單，請參閱<a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中鍵入強制。</p> </li> 
     <li> <p><b>[！UICONTROL資料庫檔案狀態]</b> </p> <p>選取程式庫檔案的狀態。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL使用者資訊]</td> 
   <td> <p>填寫下列欄位：</p> 
    <ul> 
     <li> <p><b>[！UICONTROL電子郵件]</b> </p> <p>輸入使用者的電子郵件地址。</p> </li> 
     <li> <p><b>[！UICONTROL是帳戶管理員]</b> </p> <p>如果建立的使用者是帳戶管理員，請核取此選項。</p> </li> 
     <li> <p><b>[！UICONTROL使用者ID]</b> </p> <p>輸入使用者的唯一識別碼</p> </li> 
     <li> <p><b>[！UICONTROL帳戶ID]</b> </p> <p>輸入與此使用者相關聯之[!DNL Adobe Acrobat Sign]帳戶的唯一識別碼。</p> </li> 
     <li> <p><b>[！UICONTROL名字]</b> </p> <p>輸入使用者的名字。</p> </li> 
     <li> <p><b>[！UICONTROL姓氏]</b> </p> <p>輸入使用者的姓氏</p> </li> 
     <li> <p><b>[！UICONTROL公司]</b> </p> <p>輸入使用者的公司名稱。</p> </li> 
     <li> <p><b>[！UICONTROL首字母]</b> </p> <p>輸入使用者的縮寫。</p> </li> 
     <li> <p><b>[！UICONTROL地區設定]</b> </p> <p>輸入使用者的地區設定。 這會決定UI的語言。 </p> </li> 
     <li> <p><b>[！UICONTROL電話]</b> </p> <p>輸入使用者的電話號碼</p> </li> 
     <li> <p><b>主要群組識別碼</b> </p> <p>輸入新增使用者的群組。 如果未輸入任何內容，則會將使用者新增至帳戶的預設群組。</p> </li> 
     <li> <p><b>[！UICONTROL工作標題]</b> </p> <p>輸入使用者的職稱。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL網頁表單資訊]</td> 
   <td> <p>填寫以下欄位</p> 
    <ul> 
     <li> <p><b>[！UICONTROL檔案資訊]</b> </p> <p>對於每個要新增至網路表單的檔案，按一下「新增」並填寫下列欄位：</p> 
      <ul> 
       <li> <p>[！UICONTROL檔案型別]</p> <p>[！UICONTROL檔案]</p> </li> 
       <li> <p>[！UICONTROL暫時性檔案]</p> </li> 
       <li> <p>[！UICONTROL URL檔案資訊]</p> </li> 
      </ul> </li> 
     <li> <p><b>[！UICONTROL網頁表單名稱]</b> </p> <p>輸入網頁表單的名稱。 此名稱用於識別電子郵件和網站等位置中的網路表單。</p> </li> 
     <li> <p><b>[！UICONTROL Web表單狀態]</b> </p> <p>選取應建立新Web表單的狀態。</p> </li> 
     <li> <p><b>[！UICONTROL Web表單參與者集資訊]</b> </p> 
      <ul> 
       <li> <p><b>[！UICONTROL成員資訊]</b> </p> <p>針對您想要新增至參與者集的每個成員，按一下<b>[！UICONTROL新增專案]</b>。 </p> 
        <ul> 
         <li> <p><b>[！UICONTROL電子郵件]</b> </p> <p>請將此選項保留空白。</p> </li> 
         <li> <p><b>[！UICONTROL安全性選項]</b> </p> <p>如果要新增安全性選項來認證此使用者，請選取<b>[！UICONTROL是]</b>，然後選取安全性選項並填寫它所需的任何欄位。</p> </li> 
        </ul> </li> 
       <li> <p><b>[！UICONTROL角色]</b> </p> <p>選取角色。 此參與者集的所有成員都會共用角色。</p> </li> 
      </ul> </li> 
     <li> <p><b>[！UICONTROL Web表單其他參與者集資訊]</b> </p> 
      <ul> 
       <li> <p><b>[！UICONTROL成員資訊]</b> </p> <p>針對您想要新增至參與者集的每個成員，按一下<b>[！UICONTROL新增專案]</b>。</p> 
        <ul> 
         <li> <p><b>[！UICONTROL電子郵件]</b> </p> <p>請將此選項保留空白。</p> </li> 
         <li> <p><b>[！UICONTROL安全性選項]</b> </p> <p>如果要新增安全性選項來認證此使用者，請選取<b>[！UICONTROL是]</b>，然後選取安全性選項並填寫它所需的任何欄位。</p> </li> 
        </ul> </li> 
       <li> <p><b>[！UICONTROL角色]</b> </p> </li> 
       <li> <p><b>[！UICONTROL網頁表單參與者識別碼] </b> </p> <p>輸入網頁表單參與者的識別碼。</p> </li> 
       <li> <p><b>[！UICONTROL順序]</b> </p> <p>指定此參與者集與網頁表單互動的順序。 例如，順序值為1的參與者群組必須先執行，2必須先執行，依此類推。 訂單編號必須以一個開頭，且序列中沒有間隙。 </p> </li> 
       <li> <p><b>[！UICONTROL提供者參與者集資訊]</b> </p> <p>如果參與者不明，請輸入提供者是否必須提供參與者的詳細資訊，然後輸入訊息，其中包含您對未知參與者所需的詳細資訊。</p> </li> 
      </ul> </li> 
     <li> <p><b>[！UICONTROL驗證失敗資訊]</b> </p> <p>如果您要為使用者提供失敗或錯誤頁面，請選取<b>[！UICONTROL是]</b>，然後填寫下列欄位：</p> 
      <ul> 
       <li> <p><b>[！UICONTROL URL]</b> </p> <p>輸入錯誤頁面的URL</p> </li> 
       <li> <p><b>[！UICONTROL框架]</b> </p> <p>如果您希望錯誤頁面顯示在網頁表單中，請啟用此選項</p> </li> 
       <li> <p><b>[！UICONTROL延遲]</b> </p> <p>輸入將使用者重新導向至錯誤頁面之前的延遲秒數。</p> </li> 
      </ul> </li> 
     <li> <p><b>[！UICONTROL CC資訊]</b> </p> <p>對於您希望在網頁表單上的最終合約簽署時收到電子郵件的每個電子郵件地址，按一下<b>[！UICONTROL新增專案]</b>並輸入電子郵件地址。</p> </li> 
     <li> <p><b>[！UICONTROL完成資訊]</b> </p> <p style="font-style: normal;">如果您要為使用者提供成功頁面，請選取<b>[！UICONTROL是]</b>，然後填寫下列欄位：</p> 
      <ul> 
       <li> <p><b>[！UICONTROL URL]</b> </p> <p>輸入成功頁面的URL</p> </li> 
       <li> <p><b>[！UICONTROL框架]</b> </p> <p>如果您希望成功頁面顯示在網頁表單中，請啟用此選項</p> </li> 
       <li> <p><b>[！UICONTROL延遲]</b> </p> <p>輸入將使用者重新導向至成功頁面之前的延遲秒數。</p> </li> 
      </ul> </li> 
     <li> <p><b>[！UICONTROL群組識別碼]</b> </p> <p>輸入網頁表單所屬群組的識別碼。 如果未輸入任何內容，則網頁表單屬於帳戶使用者的主要群組。</p> </li> 
     <li> <p><b>[！UICONTROL上次事件日期]</b> </p> <p>輸入上次事件在網路表單上發生的日期。 使用格式<code>yyyy-MM-dd'T'HH:mm:ssZ</code>。</p> </li> 
     <li> <p><b>[！UICONTROL地區設定]</b> </p> <p>輸入使用者的地區設定。 這會決定UI的語言。 </p> </li> 
     <li> <p><b>[！UICONTROL安全性選項]n</b> </p> <p>輸入用來保護檔案的密碼。 您必須個別將此密碼傳達給任何相關方。</p> </li> 
     <li> <p><b>[！UICONTROL儲存庫資訊]</b> </p> <p>如果您的帳戶設定為檔案儲存庫，且選項是為每個協定啟用，您可以啟用此選項來儲存此協定。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 建立合約]**

此動作模組會建立協定、將協定送出以索取簽名，然後傳回協定ID。

>[!NOTE]
>
>我們建議上傳檔案以簽署為暫時性檔案，然後將它對應到[!UICONTROL 建立合約]模組中的[!UICONTROL 檔案以傳送]欄位。 如需範例，請參閱本文中的「上傳檔案」。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
<td>如需有關將您的[!DNL Adobe Acrobat Sign]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a></td>  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers]</td> 
   <td>以標準JSON物件的形式新增請求的標頭。例如， <code>{"Content-type":"application/json"}</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">要傳送的[！UICONTROL檔案]</td> 
   <td> <p>針對您要在合約中加入的每個專案，按一下<b>[！UICONTROL新增專案]</b>，並填寫下列欄位：</p> 
    <ul> 
     <li> <p><b>[！UICONTROL檔案型別]</b> </p> 
      <ul> 
       <li> <p><b>[！UICONTROL檔案]</b> </p> <p>填寫下列欄位：</p> 
        <ul> 
         <li> <p><b>[！UICONTROL建立日期]</b> </p> <p>以<code>yyyy-MM-dd'T'HH:mm:ssZ</code>格式輸入或對應檔案的建立日期。 例如，<code>2016-02-25T18:46:19Z</code>代表UTC時間。</p> </li> 
         <li> <p><b>[！UICONTROL識別碼]</b> </p> <p>輸入或對映檔案的ID。</p> </li> 
         <li> <p><b>[！UICONTROL標籤]</b> </p> <p>輸入或對應檔案的唯一標籤。 在自訂工作流程中，這會將檔案對應至工作流程定義中對應的檔案元素。 若是自訂工作流程協定建立請求，則必須指定此屬性。</p> </li> 
         <li> <p><b>[！UICONTROL頁數]</b> </p> <p>輸入或對應檔案中的頁數。</p> </li> 
         <li> <p><b>[！UICONTROL Mime-Type]</b> </p> <p>輸入或對映原始檔案的mime型別。 多用途網際網路郵件延伸模組(MIME)型別是標籤，可讓軟體識別網際網路上共用的不同資料型別。 Web伺服器和瀏覽器會使用MIME型別來決定應該對檔案執行的操作。 例如，MIME型別為<code>text/html</code>的檔案在瀏覽器中的處理方式與MIME型別為<code>image/jpeg</code>的檔案不同。</p> </li> 
         <li> <p><b>[！UICONTROL名稱]</b> </p> <p>輸入或對映檔案的名稱。<br></p> </li> 
        </ul> </li> 
       <li> <p><b>[！UICONTROL資料庫檔案ID]</b> </p> <p>輸入程式庫檔案的ID</p> </li> 
       <li> <p><b>[！UICONTROL暫時性檔案識別碼]</b> </p> <p>輸入暫時性檔案的識別碼</p> </li> 
       <li> <p><b>[！UICONTROL URL檔案傳輸]</b> </p> <p>填寫下列欄位：</p> 
        <ul> 
         <li> <p><b>[！UICONTROL Mime-Type]</b> </p> <p>輸入原始檔案的mime型別。 多用途網際網路郵件延伸模組(MIME)型別是標籤，可讓軟體識別網際網路上共用的不同資料型別。 Web伺服器和瀏覽器會使用MIME型別來決定應該對檔案執行的操作。 例如，MIME型別為<code>text/html</code>的檔案在瀏覽器中的處理方式與MIME型別為<code>image/jpeg</code>的檔案不同。</p> </li> 
         <li> <p><b>[！UICONTROL名稱]</b> </p> <p>輸入檔案的名稱。</p> </li> 
         <li> <p><b>[！UICONTROL URL]</b> </p> <p>輸入您要傳送之檔案的URL。</p> </li> 
        </ul> </li> 
      </ul> </li> 
     <li> <p><b>[！UICONTROL標籤]</b> </p> <p>輸入檔案的標籤。</p> </li> 
     <li> <p><b>[！UICONTROL Notarize]</b> </p> <p>啟用此選項以指示檔案必須經過公證。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL合約名稱]</td> 
   <td>輸入新合約的名稱。 此名稱用於識別電子郵件和網站等位置中的合約。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL參與者集資訊]</td> 
   <td> <p>針對您要新增的每個參與者集，按一下<b>[！UICONTROL新增專案]</b>並填寫下列欄位。</p> 
    <ul> 
     <li> <p><b>[！UICONTROL成員]</b> </p> <p>針對您想要新增至參與者集的每個人員，按一下<b>[！UICONTROL新增專案]</b>，然後輸入該人員的電子郵件地址。</p> </li> 
     <li> <p><b>[！UICONTROL順序]</b> </p> <p>指定此參與者集簽署合約的順序。 例如，訂單值為1的參與者群組必須先簽署，2必須在下一個簽署，依此類推。 訂單編號必須以一個開頭，且序列中沒有間隙。 </p> </li> 
     <li> <p><b>[！UICONTROL角色]</b> </p> <p>選取此參與者集的角色。 集合中的所有參與者都會獲得此角色。</p> </li> 
     <li> <p><b>[！UICONTROL識別碼]</b> </p> <p>輸入或對應此參與者集的ID。</p> </li> 
     <li> <p><b>[！UICONTROL標籤]</b> </p> <p>輸入或對應參與者集的唯一標籤。 對於自訂工作流程，參與率集中指定的標籤應該將其對應至自訂工作流程中的參與率步驟。</p> </li> 
     <li> <p><b>[！UICONTROL名稱]</b> </p> <p>輸入參與者集名稱。 此名稱在合約中必須是唯一的。</p> </li> 
     <li> <p><b>[！UICONTROL私人訊息]</b> </p> <p>輸入或對應此參與者集的訊息。 集合中的所有參與者都會收到此訊息。</p> </li> 
     <li> <p><b>[！UICONTROL可見頁面]</b> </p> <p>如果為此協定啟用有限檔案可見性，請指定對此參與者集可見的檔案。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL簽章型別]</td> 
   <td> <p>選取合約所需的簽章型別。</p> 
    <ul> 
     <li> <p><b>[！UICONTROL E-sign]</b> </p> <p>合約必須以電子方式簽署。</p> </li> 
     <li> <p><b>[！UICONTROL已寫入]</b> </p> <p>合約必須手動簽署，且已簽署的合約必須掃描並上傳。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL狀態]</td> 
   <td> <p>選取此協定的狀態。</p> 
    <ul> 
     <li> <p><b>[！UICONTROL製作]</b> </p> <p>您仍然可以編輯欄位或新增欄位至此合約。</p> </li> 
     <li> <p><b>[！UICONTROL草稿]</b> </p> <p>您可以在傳送合約之前逐步建立此合約。</p> </li> 
     <li> <p><b>[！UICONTROL處理中]</b> </p> <p>此合約將立即傳送。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL CCs]</td> 
   <td> <p>您可以將此合約傳送給不需要簽署的利害關係人，例如利害關係人。 他們會在簽署程式開始時收到一封電子郵件，並在收到最終簽名時收到另一封電子郵件。 他們也會收到合約的PDF副本。 </p> <p>針對您想要在此合約上寄送副本的每個人，按一下<b>[！UICONTROL新增專案]</b>，並填寫下列欄位：</p> 
    <ul> 
     <li> <p><b>[！UICONTROL電子郵件]</b> </p> <p>輸入或對應您要在合約上寄送的電子郵件地址。</p> </li> 
     <li> <p><b>[！UICONTROL標籤]</b> </p> <p>輸入或對應此電子郵件地址的標籤，如工作流程說明所示</p> </li> 
     <li> <p><b>[！UICONTROL可見頁面]</b> </p> </li> 
     <li> <p>如果為此協定啟用有限檔案可見性，請指定對此參與者集可見的檔案。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL電子郵件選項]</td> 
   <td> <p>針對每種型別的電子郵件，選取該型別的電子郵件是傳送給所有參與者還是全部不傳送。</p> 
    <ul> 
     <li> <p><b>[！UICONTROL完成電子郵件]</b> </p> <p>在此合約完成、取消、過期或拒絕時傳送電子郵件。</p> </li> 
     <li> <p><b>[！UICONTROL小眾測試版內電子郵件]</b> </p> <p>委派或取代此合約時傳送電子郵件。</p> </li> 
     <li> <p><b>[！UICONTROL合約初始電子郵件]</b> </p> <p>建立此合約或請求對此合約執行動作時，請傳送電子郵件。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL外部ID]</td> 
   <td> <p>輸入或對應此合約的ID。 您可以在建立協定時指定此項，並用來在後續的模組或查詢中尋找協定。</p> <p>注意：所有參與者可透過API看見外部ID值，因此不應使用它來包含敏感權杖。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL合併欄位資訊]</td> 
   <td> <p>針對協定中要設定預設值的每個欄位，按一下<b>[！UICONTROL新增專案]</b>，然後輸入預設值和欄位名稱。</p> <p>可編輯欄位的值將會顯示給簽署者。對於唯讀欄位，提供的值在簽署過程中將不可編輯。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL公證資訊]</td> 
   <td> <p>填寫下列欄位：</p> 
    <ul> 
     <li> <p><b>[！UICONTROL約會]</b> </p> <p>輸入或對應約會的建議時間與日期，以公證此合約。</p> </li> 
     <li> <p><b>[！UICONTROL附註]</b> </p> <p>輸入或對應您想要包含的有關公證工作階段的任何附註。</p> </li> 
     <li> <p><b>[！UICONTROL付款]</b> </p> <p>選擇由合約的簽署者或寄件者支付公證人費用。</p> </li> 
     <li> <p><b>[！UICONTROL公證型別]</b> </p> <p>選取公證人的型別</p> 
      <ul> 
       <li> <p>[！UICONTROL Provider notary]</p> <p>公證員由公證提供者提供。</p> </li> 
       <li> <p>[！UICONTROL BYON NOTARY]</p> <p>公證人由客戶提供。</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Post sign option]</td> 
   <td> <p>選取您是否希望簽署協定後，將簽署者導向成功頁面。 如果您選取<b>[！UICONTROL是]</b>，請填入下列欄位：</p> 
    <ul> 
     <li> <p><b>[！UICONTROL重新導向延遲]</b> </p> <p>輸入或對應數字，代表將簽署者重新導向至成功頁面之前的秒數。 如果此值大於0，使用者將會先看到標準的[!DNL Adobe Sign]成功訊息，然後在延遲之後將會重新導向至您的成功頁面。</p> </li> 
     <li> <p><b>[！UICONTROL重新導向URL]</b> </p> <p>輸入或對應可公開存取的URL，使用者在成功完成簽署程式後會傳送到此URL。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL安全性選項]</td> 
   <td> <p>輸入或對應用於保護PDF檔案安全的次要密碼。 </p> <p>重要： [!DNL Adobe Sign]絕不會共用此密碼，因此您必須單獨將它傳達給任何相關人員。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL儲存庫資訊]</td> 
   <td>如果您的帳戶設定為檔案儲存庫，且選項是為每個協定啟用，您可以啟用此選項來儲存此協定。</td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 建立相關記錄]**

此動作模組會建立連結至您選取之模組的記錄。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Adobe Acrobat Sign]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標頭。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 自動新增授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別]</td> 
   <td>選取要與建立的記錄產生關聯的原始記錄的記錄型別。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Agreement]/[！UICONTROL Library document]/[！UICONTROL User]/[！UICONTROL Widget ID]</td> 
   <td>輸入或對應您想要與建立的記錄產生關聯的物件ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL合約相關欄位]</td> 
   <td> <p>選取您要建立的相關欄位型別</p> 
    <ul> 
     <li> <p><b>[！UICONTROL表單欄位]</b> </p> <p>輸入包含您要建立之欄位之範本的範本ID</p> </li> 
     <li> <p><b>[！UICONTROL提醒]</b> </p> <p>填寫下列欄位：</p> 
      <ul> 
       <li> <p><b>[！UICONTROL收件者參與者識別碼]</b> </p> <p>對於您想要收到提醒的每個參與者，請按一下[！UICONTROL新增專案]，然後輸入參與者的ID。</p> </li> 
       <li> <p><b>[！UICONTROL狀態]</b> </p> <p>對於新記錄，狀態必須為[！UICONTROL Active]。</p> </li> 
       <li> <p><b>[！UICONTROL第一個提醒延遲]</b> </p> <p>輸入傳送第一個提醒前的延遲小時數。 允許的最小值為1小時，最大值不能超過合約建立和合約到期時間（以小時為單位）的差異。 如果未設定此延遲，則會根據頻率進行第一個提醒。</p> </li> 
       <li> <p><b>[！UICONTROL提醒頻率]</b> </p> <p>設定您要傳送提醒的頻率。 如果未提供頻率，則提醒將會傳送一次。</p> </li> 
       <li> <p><b>[！UICONTROL上次傳送日期]</b> </p> <p>此欄位由系統設定。</p> </li> 
       <li> <p><b>[！UICONTROL下一個傳送日期]</b> </p> <p>此欄位必須空白或設為[！UICONTROL一次]。</p> </li> 
       <li> <p><b>[！UICONTROL附註]</b> </p> <p>輸入要包含在提醒中的備註。 這有助於告訴參與者需要其參與的原因。</p> </li> 
       <li> <p><b>[！UICONTROL開始提醒計數器來自]</b> </p> <p>選取是否根據合約建立時間（當合約可用時）來傳送提醒。</p> </li> 
      </ul> </li> 
     <li> <p><b>[！UICONTROL簽署者身分報告]</b> </p> <p>輸入用於保護PDF檔案安全的密碼。</p> </li> 
     <li> <p><b>[！UICONTROL檢視]</b> </p> <p>輸入下列欄位</p> 
      <ul> 
       <li> <p><b>[！UICONTROL名稱]</b> </p> <p>選取您要建立的檢視名稱。</p> </li> 
       <li> <p><b>[！UICONTROL自動登入使用者]</b> </p> <p>選取<b>[！UICONTROL是]</b>自動將使用者登入傳回的URL。</p> </li> 
       <li> <p><b>[！UICONTROL框架父項]</b> </p> <p>輸入或對應上層網域URL的逗號分隔清單，其中傳回的URL可能會以iframe格式顯示。 如果留空，無法在iframe中檢視[!DNL Adobe Acrobat Sign]頁面。</p> </li> 
       <li> <p><b>[！UICONTROL地區設定]</b> </p> <p>輸入您要建立檢視的語言。 </p> </li> 
       <li> <p><b>[！UICONTROL無Chrome旗標]</b> </p> <p>選取<b>[！UICONTROL是]</b>以顯示沒有導覽頁首或頁尾的內嵌頁面。</p> </li> 
       <li> <p><b>[！UICONTROL可以編輯檔案]</b> </p> <p>若要透過新增或移除檔案來編輯檔案上傳區段，請選取<b>[！UICONTROL是]</b>。 這不是存取控制機制。 預設值為[！UICONTROL是]。</p> </li> 
       <li> <p><b>[！UICONTROL資料庫檔案]</b> </p> <p>若要顯示程式庫檔案連結，請選取<b>[！UICONTROL是]</b>。 預設值為[！UICONTROL是]。</p> </li> 
       <li> <p><b>[！UICONTROL本機檔案]</b> </p> <p>若要顯示本機檔案上傳按鈕，請選取<b>[！UICONTROL是]</b>。 預設值為[！UICONTROL是]。</p> </li> 
       <li> <p><b>[！UICONTROL Web聯結器]</b> </p> <p>若要顯示連結以附加來自Web來源的檔案，請選取<b>[！UICONTROL是]</b>。 預設值為「是」。</p> </li> 
       <li> <p><b>[！UICONTROL為預覽已選取]</b> </p> <p>選取<b>[！UICONTROL是]</b>以將撰寫頁面設定為撰寫模式。</p> </li> 
      </ul> </li> 
     <li> <p><b>[！UICONTROL成員共用]</b> </p> <p>針對您想要與其共用合約的每個成員，按一下<b>[！UICONTROL新增專案]</b>，然後輸入成員的電子郵件地址和給該成員的訊息。</p> </li> 
     <li> <p>[！UICONTROL委派參與者集]</p> 
      <ul> 
       <li> <p><b>[！UICONTROL參與者集識別碼]</b> </p> <p>輸入參與者集識別碼</p> </li> 
       <li> <p><b>[！UICONTROL成員資訊]</b> </p> <p>針對您要新增的每個成員，按一下[！UICONTROL新增專案]，然後輸入成員的電子郵件地址和電話資訊。</p> </li> 
       <li> <p><b>[！UICONTROL私人訊息]</b> </p> <p>輸入訊息。 參與者集的所有成員都會收到此訊息。</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資料庫檢視資訊]</td> 
   <td> <p>填寫下列欄位：</p> 
    <ul> 
     <li> <p><b>[！UICONTROL名稱]</b> </p> <p>輸入程式庫範本的名稱。 此名稱用於電子郵件和網站。</p> </li> 
     <li> <p><b>[！UICONTROL自動登入使用者]</b> </p> <p>選取<b>[！UICONTROL是]</b>自動將使用者登入傳回的URL。</p> </li> 
     <li> <p><b>[！UICONTROL框架父項]</b> </p> <p>輸入或對應上層網域URL的逗號分隔清單，其中傳回的URL可能會以iframe格式顯示。 如果留空，無法在iframe中檢視[!DNL Adobe Acrobat Sign]頁面。</p> </li> 
     <li> <p><b>[！UICONTROL地區設定]</b> </p> <p>輸入您要建立檢視的語言。 </p> </li> 
     <li> <p><b>[！UICONTROL無Chrome旗標]</b> </p> <p>選取<b>[！UICONTROL是]</b>以顯示沒有導覽頁首或頁尾的內嵌頁面。</p> </li> 
     <li> <p><b>[！UICONTROL傳送檢視組態]</b> </p> <p>若要設定[！UICONTROL Send]檢視，請選取<b>[！UICONTROL Yes]</b>，然後填寫下列欄位。</p> 
      <ul> 
       <li> <p><b>[！UICONTROL合約名稱]</b> </p> <p>在構成頁面上輸入或對應程式庫檔案的協定名稱。</p> </li> 
       <li> <p><b>[！UICONTROL可以編輯檔案]</b> </p> <p>若要透過新增或移除檔案來編輯檔案上傳區段，請選取<b>[！UICONTROL是]</b>。 這不是存取控制機制。 預設值為[！UICONTROL是]。</p> </li> 
       <li> <p><b>[！UICONTROL本機檔案]</b> </p> <p>若要顯示程式庫檔案連結，請選取<b>[！UICONTROL是]</b>。 預設值為[！UICONTROL是]。</p> </li> 
       <li> <p><b>[！UICONTROL Web聯結器]</b> </p> <p>若要顯示連結以附加來自Web來源的檔案，請選取<b>[！UICONTROL是]</b>。 預設值為[！UICONTROL是]。</p> </li> 
       <li> <p><b>已選取預覽</b> </p> <p>選取<b>[！UICONTROL是]</b>以將撰寫頁面設定為撰寫模式。</p> </li> 
      </ul> <p> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL使用者檢視資訊]</td> 
   <td> <p>填寫以下欄位</p> 
    <ul> 
     <li> <p><b>[！UICONTROL名稱]</b> </p> <p>選取要求的使用者檢視名稱。</p> </li> 
     <li> <p><b>[！UICONTROL自動登入使用者]</b> </p> <p>選取<b>[！UICONTROL是]</b>以自動登入使用者。 選取<b>[！UICONTROL否]</b>以需要認證。 預設值為[！UICONTROL否]。</p> </li> 
     <li> <p><b>[！UICONTROL框架父項]</b> </p> <p>輸入或對應上層網域URL的逗號分隔清單，其中傳回的URL可能會以iframe格式顯示。 如果留空，無法在iframe中檢視[!DNL Adobe Acrobat Sign]頁面。</p> </li> 
     <li> <p><b>無Chrome標幟</b> </p> <p>選取<b>[！UICONTROL是]</b>以顯示沒有導覽頁首或頁尾的內嵌頁面。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Widget相關欄位]</td> 
   <td> <p>選取您要建立的相關記錄。</p> 
    <ul> 
     <li> <p>[！UICONTROL檢視]</p> <p>填寫下列欄位。</p> 
      <ul> 
       <li> <p><b>[！UICONTROL名稱]</b> </p> <p>選取要求的網頁表單檢視的名稱</p> </li> 
       <li> <p><b>[！UICONTROL自動登入使用者]</b> </p> <p>選取<b>[！UICONTROL是]</b>以自動登入使用者。 選取<b>[！UICONTROL否]</b>以需要認證。 預設值為[！UICONTROL否]。</p> </li> 
       <li> <p><b>[！UICONTROL框架父項]</b> </p> <p>輸入或對應上層網域URL的逗號分隔清單，其中傳回的URL可能會以iframe格式顯示。 如果留空，無法在iframe中檢視[!DNL Adobe Acrobat Sign]頁面。</p> </li> 
       <li> <p><b>[！UICONTROL地區設定]</b> </p> <p>輸入您要建立檢視的語言。 </p> </li> 
       <li> <p><b>[！UICONTROL無Chrome旗標]</b> </p> <p>選取<b>[！UICONTROL是]</b>以顯示沒有導覽頁首或頁尾的內嵌頁面。</p> </li> 
       <li> <p>[！UICONTROL個人化簽署檢視設定]</p> <p>如果您要設定個人化簽署檢視，請選取<b>[！UICONTROL是]</b>並填寫下列欄位：</p> 
        <ul> 
         <li> <p><b>[！UICONTROL電子郵件]</b> </p> <p>輸入接收新建立網路表單之人員的電子郵件地址</p> </li> 
         <li> <p><b>[！UICONTROL註解]</b> </p> <p>輸入描述API呼叫者如何建立簽署者身分的註解。 此資訊會顯示在[!DNL Adobe Acrobat Sign]稽核軌跡中。</p> </li> 
         <li> <p><b>[！UICONTROL到期]</b> </p> <p>輸入此網頁表單個人化的到期日。 </p> <p>如需支援的日期和時間格式清單，請參閱<a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">在[!DNL Adobe Workfront Fusion]</a>中鍵入強制。</p> </li> 
         <li> <p><b>[！UICONTROL可重複使用]</b> </p> <p>如果您希望預定簽署者能夠多次簽署表單，請選取<b>[！UICONTROL是]</b>。</p> </li> 
        </ul> </li> 
      </ul> </li> 
     <li> <p><b>[！UICONTROL成員共用]</b> </p> <p>針對您想要與其共用合約的每個成員，按一下<b>[！UICONTROL新增專案]</b>，然後輸入成員的電子郵件地址和給該成員的訊息。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 自訂API呼叫]**
此模組可讓您執行自訂API呼叫。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Adobe Acrobat Sign]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL URL]</p> </td> 
   <td> <p>輸入相對於 <code>https://api.[region].adobesign.com/api/rest/v6/</code></p> <p>注意：如需可用端點的清單，請參閱[!DNL Adobe Sign] API參考。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL方法]</p> </td> 
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP要求方法。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標頭。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 自動新增授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查詢字串] </td> 
   <td> <p>輸入請求查詢字串。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Body]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的內文內容。</p> <p>注意：  <p>在JSON中使用條件陳述式（例如<code>if</code>）時，請將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL上傳暫時性檔案]</td> 
   <td> <p>如果要上傳暫時性檔案，請輸入要上傳檔案的來源檔案。</p> <p>從先前的模組中選取來源檔案，或對應來源檔案的名稱和資料。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 清單記錄]**

此動作模組會列出該帳戶有權存取之選取型別的所有記錄。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Adobe Acrobat Sign]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標頭。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 自動新增授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別]</td> 
   <td>選取您要擷取相關記錄的記錄型別。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Locale]</td> 
   <td> <p>輸入使用者的地區設定。 這會決定UI的語言。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL外部ID]</td> 
   <td>針對您要傳回的合約，輸入或對應外部識別碼（在[!DNL Adobe Acrobat Sign]之外指派的識別碼）。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL群組ID]</td> 
   <td>輸入與您要列出之記錄關聯的群組識別碼。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL顯示隱藏的（記錄）]</td> 
   <td>若要在結果中包含隱藏的記錄，請啟用此選項。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Cursor] / [！UICONTROL開始索引]</td> 
   <td> <p>輸入模組應傳回的第一個記錄編號。 </p> <p>注意：此欄位會與[！UICONTROL Maximum number of returned records]欄位結合，以分頁。 例如，如果[！UICONTROL傳回事件數上限]為100，而[！UICONTROL開始索引]為101，模組會傳回記錄101-200，或傳回結果的第二頁。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL傳回記錄的最大數量]</td> 
   <td> <p>在每個案例執行週期中，輸入或對應您要模組至[action]的最大記錄數量。</p> <p>注意：此欄位會與[！UICONTROL Cursor]或[！UICONTROL Start Index]欄位結合，以分頁。 例如，如果[！UICONTROL傳回事件數上限]為100，而[！UICONTROL開始索引]為101，模組會傳回記錄101-200，或傳回結果的第二頁。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL父網域URL]</td> 
   <td> <p>輸入或對應上層網域URL的逗號分隔清單，其中傳回的URL可能會以iframe格式顯示。 如果留空，無法在iframe中檢視[!DNL Adobe Acrobat Sign]頁面。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 讀取記錄]**

此動作模組會從單一記錄擷取資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Adobe Acrobat Sign]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標頭。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 自動新增授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別]</td> 
   <td>選取您要擷取相關記錄的記錄型別。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄ID]</td> 
   <td>輸入或對應您要擷取之記錄的ID。</td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 讀取相關記錄]**

閱讀與單一記錄相關的其他資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Adobe Acrobat Sign]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標頭。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 自動新增授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別]</td> 
   <td>選取您要擷取相關記錄的記錄型別。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄ID] （範例：[！UICONTROL帳戶ID]）</td> 
   <td>輸入或對應您要擷取相關記錄的記錄ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL其他欄位]</td> 
   <td>根據記錄型別和相關欄位，在特定欄位中輸入資訊。</td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 更新記錄]**

此動作模組更新[!DNL Adobe Acrobat Sign]中的單一記錄。

>[!IMPORTANT]
>
>* 最佳實務是，如果您預期協定會有重大變更，建議您建立新協定，而非更新現有協定。
>* 部分更新包含必填欄位。 設定更新時，請務必填寫所有必填欄位。 [!DNL Workfront Fusion]模組中的必填欄位為粗體。
>



<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Adobe Acrobat Sign]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標頭。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 自動新增授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄ID] </td> 
   <td>輸入或對應您要更新的記錄ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別]</td> 
   <td>選取您要更新的記錄型別。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL其他欄位]</td> 
   <td> <p>根據記錄型別和相關欄位，在特定欄位中輸入資訊。</p> 
    <ul> 
     <li> <p><b>[！UICONTROL合約]</b> </p> <p>最佳實務是，如果您預期協定會有重大變更，建議您建立新協定，而非更新現有協定。</p> </li> 
     <li> <p><b>[！UICONTROL資料庫檔案]</b> </p> <p>選取要更新的欄位，然後填寫選取的欄位：</p> 
      <ul> 
       <li> <p><b>[！UICONTROL狀態]</b> </p> <p>選取程式庫檔案的新狀態。</p> </li> 
       <li> <p><b>[！UICONTROL名稱]</b> </p> <p>輸入或對應程式庫範本的名稱</p> </li> 
       <li> <p><b>[！UICONTROL共用模式]</b> </p> <p>指定應該擁有程式庫檔案存取權的使用者。</p> </li> 
       <li> <p><b>[！UICONTROL程式庫範本型別]</b> </p> <p>針對您要使用的每個程式庫範本型別，按一下<b>[！UICONTROL新增專案]</b>並選取範本型別。</p> </li> 
      </ul> </li> 
     <li> <p><b>[！UICONTROL使用者]</b> </p> <p>選取要更新的欄位，然後填寫選取的欄位：</p> 
      <ul> 
       <li> <p><b>[！UICONTROL名字]</b> </p> <p>輸入使用者的名字。</p> </li> 
       <li> <p><b>[！UICONTROL姓氏]</b> </p> <p>輸入使用者的姓氏</p> </li> 
       <li> <p><b>[！UICONTROL公司]</b> </p> <p>輸入使用者的公司名稱。</p> </li> 
       <li> <p><b>[！UICONTROL電話]</b> </p> <p>輸入使用者的電話號碼</p> </li> 
       <li> <p><b>[！UICONTROL主要群組識別碼]</b> </p> <p>輸入新增使用者的群組。 如果未輸入任何內容，則會將使用者新增至帳戶的預設群組。</p> </li> 
       <li> <p><b>[！UICONTROL工作標題]</b> </p> <p>輸入使用者的職稱。</p> </li> 
      </ul> </li> 
     <li> <p><b>[！UICONTROL網頁表單] ([！UICONTROL widget])</b> </p> <p>根據記錄型別和相關欄位，在特定欄位中輸入資訊。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 更新相關記錄]**

此動作模組會更新與特定物件相關的記錄。

>[!IMPORTANT]
>
>* 最佳實務是，如果您預期協定會有重大變更，建議您建立新協定，而非更新現有協定。
>* 部分更新包含必填欄位。 設定更新時，請務必填寫所有必填欄位。 [!DNL Workfront Fusion]模組中的必填欄位為粗體。
>



<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Adobe Acrobat Sign]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標頭。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 自動新增授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別]</td> 
   <td>選取與相關欄位關聯之記錄的記錄型別。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Agreement]/[！UICONTROL Library document]/[！UICONTROL User]/[！UICONTROL Widget ID]</td> 
   <td>輸入或對應您想要與建立的記錄產生關聯的物件ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL其他欄位]</td> 
   <td> <p>根據記錄型別和相關欄位，在特定欄位中輸入資訊。</p> 
    <ul> 
     <li> <p><b>[！UICONTROL合約]</b> </p> <p>最佳實務是，如果您預期協定會有重大變更，建議您建立新協定，而非更新現有協定。</p> </li> 
     <li> <p><b>[！UICONTROL資料庫檔案]</b> </p> <p>選取要更新的欄位，然後填寫選取的欄位：</p> 
      <ul> 
       <li> <p><b>[！UICONTROL狀態]</b> </p> <p>選取程式庫檔案的新狀態。</p> </li> 
       <li> <p><b>[！UICONTROL附註]</b> </p> <p>輸入或對映註記的文字。</p> </li> 
       <li> <p><b>[！UICONTROL可見性]</b> </p> <p>選取是否顯示或指示程式庫檔案。</p> </li> 
      </ul> </li> 
     <li> <p><b>[！UICONTROL使用者]</b> </p> <p>選取要更新的欄位，然後填寫選取的欄位：</p> 
      <ul> 
       <li> <p><b>[！UICONTROL群組資訊清單]</b> </p> <p>填寫以下欄位</p> 
        <ul> 
         <li> <p><b>[！UICONTROL狀態]</b> </p> <p>為使用者選取新狀態。</p> </li> 
         <li> <p><b>[！UICONTROL識別碼]</b> </p> <p>輸入群組的唯一識別碼</p> </li> 
         <li> <p><b>[！UICONTROL是群組管理員]</b> </p> <p>選取<b>[！UICONTROL是]</b>，讓此使用者成為群組管理員。</p> </li> 
         <li> <p><b>為主要群組</b> </p> <p>選取<b>[！UICONTROL是]</b>，將此群組更新至使用者的主要群組。</p> </li> 
         <li> <p><b>[！UICONTROL建立日期]</b> </p> <p>輸入建立群組的日期。</p> <p>如需支援的日期和時間格式清單，請參閱<a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">在[！UICONTROL Adobe Workfront Fusion]</a>中鍵入強制。</p> </li> 
         <li> <p><b>[！UICONTROL名稱]</b> </p> <p>輸入或對映群組的名稱。</p> </li> 
         <li> <p><b>[！UICONTROL資料庫檔案建立可見]</b> </p> <p>這些設定會決定使用者是否可以建立物件庫檔案</p> 
          <ul> 
           <li> <p>[！UICONTROL值]</p> <p>允許</p> </li> 
           <li> <p>[！UICONTROL Inherited]</p> <p>從群組或帳戶繼承群組設定</p> </li> 
          </ul> </li> 
         <li> <p><b>[！UICONTROL傳送限制在工作流程中]</b> </p> <p>這些設定決定使用者是否只能使用工作流程建立協定。</p> 
          <ul> 
           <li> <p>[！UICONTROL值]</p> <p>允許</p> </li> 
           <li> <p>[！UICONTROL Inherited]</p> <p>從群組或帳戶繼承群組設定</p> </li> 
          </ul> </li> 
         <li> <p><b>[！UICONTROL使用者可以傳送]</b> </p> 
          <ul> 
           <li> <p>[！UICONTROL值]</p> <p>允許</p> </li> 
           <li> <p>[！UICONTROL Inherited]</p> <p>從群組或帳戶繼承群組設定</p> </li> 
          </ul> </li> 
        </ul> </li> 
      </ul> 
      <ul> 
       <li> <p><b>[！UICONTROL狀態]</b> </p> <p>選取使用者的新狀態，然後輸入您要啟用或停用使用者的相關註解。</p> </li> 
       <li> <p><b>[！UICONTROL地區設定]</b> </p> <p>輸入使用者的地區設定。 這會決定UI的語言。 </p> </li> 
      </ul> </li> 
     <li> <p><b>[！UICONTROL網頁表單] ([！UICONTROL widget])</b> </p> <p>根據記錄型別和相關欄位，在特定欄位中輸入資訊。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL 上傳檔案]**

上傳暫時性檔案。 暫時性檔案上傳後7天內皆可使用。

>[!NOTE]
>
>我們建議上傳檔案以作為暫時性檔案簽署，然後將它對應到「建立協定」模組中的「要傳送的檔案」欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Adobe Acrobat Sign]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標頭。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 自動新增授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄ID]</td> 
   <td>輸入或對應您要更新的記錄ID</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL MIME型別]</td> 
   <td>輸入原始檔案的mime型別。 多用途網際網路郵件延伸模組(MIME)型別是標籤，可讓軟體識別網際網路上共用的不同資料型別。 Web伺服器和瀏覽器會使用MIME型別來決定應該對檔案執行的操作。 例如，MIME型別為<code>text/html</code>的檔案在瀏覽器中的處理方式與MIME型別為<code>image/jpeg</code>的檔案不同。</td> 
  </tr> 
 </tbody> 
</table>

**範例：**&#x200B;在此工作流程中，要簽署的檔案(先前從Workfront下載)會上傳為暫時性檔案。

![](assets/sign-example-1-350x308.png)

[!UICONTROL 上傳檔案]模組會提供可在後續模組參考的檔案識別碼[!DNL Adobe Acrobat Sign]。 建立合約時，上傳檔案的識別碼會包含在[!UICONTROL 要傳送的檔案]欄位中。

![](assets/sign-example-2-350x356.png)

+++

### 搜尋

+++ **[!UICONTROL 搜尋合約]**

此搜尋模組會根據您提供的條件來搜尋協定。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Adobe Acrobat Sign]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標頭。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文字篩選]</td> 
   <td> <p>搜尋合約中繼資料中的文字。 </p> 
    <ul> 
     <li> <p><b>[！UICONTROL尋找文字]</b> </p> <p>輸入要在合約中繼資料中尋找的文字。 每個字都會被視為個別的文字專案。 </p> </li> 
     <li> <p><b>[！UICONTROL在]</b>中尋找文字 </p> <p>選取您要尋找文字的中繼資料欄位。 如果您未選取任何專案，模組會搜尋所有中繼資料。</p> </li> 
    </ul> <p>模組會傳回任何包含任何選定欄位中輸入文字的協定。 範例：輸入"spring campaign"並選取Title和Note選項會傳回在Title或Note中包含"Spring"或"Campaign"字詞的任何合約。</p> <p>如需在[!DNL Adobe Acrobat Sign]中搜尋欄位的詳細資訊，請參閱<a href="https://helpx.adobe.com/sign/using/adobesign-search-users-agreements.html#HowSearchWorks">[!DNL Adobe Sign]搜尋中的「文字搜尋如何運作」 — 其運作方式</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL建立日期]</td> 
   <td>選取日期。 模組只會傳回建立的日期符合此條件的記錄。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL到期日]</td> 
   <td>選取日期。 模組只會傳回到期日符合此條件的記錄。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[！UICONTROL修改日期]</p> </td> 
   <td>選取日期。 模組只會傳回修改日期符合此條件的記錄。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL外部ID]</td> 
   <td> <p> 外部ID是傳送者指派給合約的ID，可為任何形式，但通常為「&lt;groupID&gt;：&lt;ID&gt;」的形式。</p> <p>針對您要新增的每個外部ID，按一下<b>[！UICONTROL新增]</b>，然後輸入或對應外部ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL群組ID]</td> 
   <td> <p>群組ID是建立群組時指派的識別碼。</p> <p>針對您要新增的每個外部ID，按一下<b>[！UICONTROL新增]</b>，然後輸入或對應外部ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資產ID]</td> 
   <td> <p>這是指派給特定合約的ID。 </p> <p>針對您要新增的每個外部ID，按一下<b>[！UICONTROL新增]</b>，然後輸入或對應外部ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL父系ID]</td> 
   <td> <p>這是指派給協定之父物件的ID。 </p> <p>針對您要新增的每個外部ID，按一下<b>[！UICONTROL新增]</b>，然後輸入或對應外部ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL參與者電子郵件]</td> 
   <td> <p>參與者的電子郵件地址。 </p> <p>針對您要新增的每個外部ID，按一下<b>[！UICONTROL新增]</b>，然後輸入或對應外部ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL角色]</td> 
   <td>選取您希望傳回的結果包含的角色。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL排序依據]</td> 
   <td>如果您希望模組對結果進行排序，請選取要作為結果排序依據的欄位。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL排序順序]r</td> 
   <td>如果您希望模組排序結果，請選取您想要升序排序還是降序排序。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL狀態]</td> 
   <td>選取您希望傳回的結果包含的狀態。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL型別]</td> 
   <td>選取您想要傳回結果包含的協定型別。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL子型別]</td> 
   <td>選取您想要傳回結果包含的協定子型態。 只有「物件庫」範本協定具有子型別。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL使用者ID]</td> 
   <td> <p>與共用合約之使用者的使用者ID。</p> <p>針對您要新增的每個使用者ID，按一下<b>[！UICONTROL新增]</b>，然後輸入或對映使用者ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL可見性]</td> 
   <td>選取您想要傳回結果包含的可見度層級。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL開始索引]</td> 
   <td> <p>輸入要傳回的第一個結果的位置。 將此專案與[！UICONTROL傳回結果數上限結合，以分頁結果</p> <p>範例：如果一次傳回100個結果，請輸入100以傳回結果100-200。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL傳回結果的最大數目]</td> 
   <td> <p>在每個案例執行週期中，輸入或對應您要模組至[action]的最大記錄數量。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++
