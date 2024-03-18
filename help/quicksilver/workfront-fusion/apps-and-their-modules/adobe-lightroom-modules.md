---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Adobe Lightroom模組
description: 透過Adobe Lightroom模組，您可以根據Adobe Lightroom帳戶中的事件啟動Adobe Workfront Fusion案例。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
source-git-commit: e99bd69c712a7685512eecc7fccc8211013a259d
workflow-type: tm+mt
source-wordcount: '2244'
ht-degree: 0%

---

# [!DNL Adobe Lightroom] 模組

<!--Add Connection info-->

在 [!DNL Adobe Workfront Fusion] 情境中，您可以使用自動化工作流程 [!DNL Adobe Lightroom]，並連結至多個協力廠商應用程式和服務。

如果您需要有關建立情境的指示，請參閱 [建立情境](../../workfront-fusion/scenarios/create-a-scenario.md).

如需模組的相關資訊，請參閱 [中的模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td>
      <td>
        <p>[！UICONTROL Pro]或更高版本</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] 授權*</td>
      <td>
        <p>[！UICONTROL計畫]，[！UICONTROL工作]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] 授權**</td>
      <td >
        <p>[！UICONTROL Workfront Fusion for Work Automation and Integration]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">產品</td>
      <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述的功能。</td>
    </tr>
    </tr>
  </tbody>
</table>


&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

&#42;&#42;有關的資訊 [!DNL Adobe Workfront Fusion] 授權，請參閱 [!DNL [Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 先決條件

開始使用 [!DNL Adobe Lightroom] 聯結器時，您必須確定符合下列先決條件：

* 您必須擁有使用中 [!DNL Adobe Lightroom] 帳戶。

## 建立與Adobe Lightroom的連線



## Adobe Lightroom模組及其欄位

當您設定 [!DNL Adobe Lightroom] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 除了這些以外， [!DNL Adobe Lightroom] 欄位可能會顯示，端視您應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [在中將資訊從一個模組對應到另一個模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [其他](#other)
* [資產](#assets)
* [相簿](#albums)

### 其他

* [健康情況檢查](#health-check)
* [擷取使用者目錄中繼資料](#retrieve-user-catalog-metadata)

#### 健康情況檢查

此動作模組會擷取Lightroom伺服器版本ID，以證明Lightroom服務目前是否執行。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有關建立與的連線的指示 [!DNL Adobe Lightroom]，請參閱 <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >建立與的連線 [!DNL Adobe Lightroom]</a> 本文章內容。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL認證]</td>
      <td>
        <p>如果要提供特定認證以確保特定伺服器正在執行，請按一下「新增專案」並輸入認證。</p><p>授權標頭會自動新增。</p>
      </td>
    </tr>
  </tbody>
</table>

#### 擷取使用者目錄中繼資料

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有關建立與的連線的指示 [!DNL Adobe Lightroom]，請參閱 <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >建立與的連線 [!DNL Adobe Lightroom]</a> 本文章內容。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL認證]</td>
      <td>
        <p>如果您想提供特定認證，以確保可以存取正確的使用者帳戶，請按一下[新增專案]並輸入認證。</p><p>授權標頭會自動新增。</p>
      </td>
    </tr>
  </tbody>
</table>

### 資產

* [建立資產原始檔案](#create-an-asset-external-xmp-develop-setting-file)
* [建立資產](#create-an-asset)
* [建立資產外部XMP開發設定檔案](#create-an-asset-external-xmp-develop-setting-file)
* [產生原始檔案的轉譯](#generate-renditions-for-an-original-file)
* [取得目錄資產](#get-a-catalog-asset)
* [取得最新的資產外部XMP開發設定](#get-the-latest-asset-external-xmp-develop-setting-file)
* [取得最新的資產轉譯](#get-the-latest-asset-rendition)
* [擷取資產](#retrieve-assets)

#### 建立資產原始檔案

此動作模組會為資產建立和上傳原始檔案。


<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有關建立與的連線的指示 [!DNL Adobe Lightroom]，請參閱 <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >建立與的連線 [!DNL Adobe Lightroom]</a> 本文章內容。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL目錄ID]</td>
      <td>
        <p>輸入或對應包含資產的目錄ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL資產ID]</td>
      <td>
        <p>輸入或對應您要建立及上傳檔案的資產ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL內容長度（位元組）]</td>
      <td>
        <p>輸入或對應內容的長度（位元組）。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL位元組範圍]</td>
      <td>
        <p>輸入或對應要求的位元組範圍，包括第一個和最後一個位元組，以及如RFC 2616所定義的實體長度。 只有在資料太大而無法透過單一呼叫上傳時，才應包含此專案。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL內容型別]</td>
      <td>
        <p>選取新檔案的內容型別。</p>
      </td>
    </tr>
  </tbody>
</table>

#### 建立資產

此動作模組會使用初始中繼資料和匯入資訊建立新資產。


<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有關建立與的連線的指示 [!DNL Adobe Lightroom]，請參閱 <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >建立與的連線 [!DNL Adobe Lightroom]</a> 本文章內容。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL目錄ID]</td>
      <td>
        <p>輸入或對映將建立資產的目錄ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL資產ID]</td>
      <td>
        <p>輸入或對映新資產的ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL資產型別]</td>
      <td>
        <p>選取資產為影像或影片。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL日期時間使用者已建立]</td>
      <td>
        <p>輸入或對應格式的日期 <code>YYYY-MM-DDT00:00:00-00:00</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL日期時間使用者已更新]</td>
      <td>
        <p>輸入或對應格式的日期 <code>YYYY-MM-DDT00:00:00-00:00</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL擷取日期]</td>
      <td>
        <p>輸入或對應格式的日期 <code>YYYY-MM-DDT00:00:00-00:00</code>.</p>
      </td>
    </tr>
  </tbody>
</table>

#### 建立資產外部XMP開發設定檔案

此動作模組支援兩個工作流程。 第一個工作流程是上傳資產的外部XMP開發設定檔案。 第二個工作流程是複製其他資產的外部xmp開發設定檔案，以建立外部XMP開發設定檔案。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有關建立與的連線的指示 [!DNL Adobe Lightroom]，請參閱 <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >建立與的連線 [!DNL Adobe Lightroom]</a> 本文章內容。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL內容長度（位元組）]</td>
      <td>
        <p>輸入或對應內容的長度（位元組）。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL上傳新的或複製XMP/develop檔案]</td>
      <td>
        <p>選取您是上傳新檔案，還是從現有資產複製檔案。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL目錄ID]</td>
      <td>
        <p>輸入或對應包含資產的目錄ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL資產ID]</td>
      <td>
        <p>輸入或對應您要上傳或複製檔案的資產ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL XMP/develop file]連結</td>
      <td>
        <p>輸入或對應連結至您要上傳或複製的檔案。</p><p>如果複製檔案，則此檔案必須為JSON；如果上傳檔案，則必須為XML。</p>
      </td>
    </tr>
  </tbody>
</table>

#### 產生原始檔案的轉譯

此動作模組會非同步產生原始檔案的轉譯。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有關建立與的連線的指示 [!DNL Adobe Lightroom]，請參閱 <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >建立與的連線 [!DNL Adobe Lightroom]</a> 本文章內容。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL轉譯型別（以分號分隔）]</td>
      <td>
        <p>輸入您要建立之轉譯的轉譯型別。 如果輸入多個型別，請以分號(；)分隔。 <p>可能的型別：</p><ul><li><code>fullsize</code></li><li><code>2560</code></li></ul></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL內容長度（位元組）]</td>
      <td>
        <p>輸入或對應內容的長度（位元組）。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL目錄ID]</td>
      <td>
        <p>輸入或對應包含資產的目錄ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL資產ID]</td>
      <td>
        <p>輸入或對應您要為其建立檔案轉譯的資產ID。</p>
      </td>
    </tr>
  </tbody>
</table>

#### 取得目錄資產

此動作模組會擷取目錄中單一資產的相關資訊。 目錄必須由使用者擁有，該使用者的認證會顯示在此模組所使用的連線中。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有關建立與的連線的指示 [!DNL Adobe Lightroom]，請參閱 <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >建立與的連線 [!DNL Adobe Lightroom]</a> 本文章內容。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL目錄ID]</td>
      <td>
        <p>輸入或對應包含資產的目錄ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL資產ID]</td>
      <td>
        <p>輸入或對應您要擷取資訊之資產的ID。</p>
      </td>
    </tr>
  </tbody>
</table>


#### 取得最新資產外部XMP開發設定檔案

此動作模組會擷取最新的資產外部XMP設定檔案。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有關建立與的連線的指示 [!DNL Adobe Lightroom]，請參閱 <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >建立與的連線 [!DNL Adobe Lightroom]</a> 本文章內容。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL目錄ID]</td>
      <td>
        <p>輸入或對應包含資產的目錄ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL資產ID]</td>
      <td>
        <p>輸入或對應與XMP開發設定檔案相關聯的資產ID。</p>
      </td>
    </tr>
  </tbody>
</table>

#### 取得最新的資產轉譯

此動作模組會擷取指定型別的最新資產轉譯。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有關建立與的連線的指示 [!DNL Adobe Lightroom]，請參閱 <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >建立與的連線 [!DNL Adobe Lightroom]</a> 本文章內容。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL目錄ID]</td>
      <td>
        <p>輸入或對應包含資產的目錄ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL資產ID]</td>
      <td>
        <p>輸入或對應與XMP開發設定檔案相關聯的資產ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL轉譯型別]</td>
      <td>
        <p>選取您要擷取的轉譯型別。</p>
      </td>
    </tr>
  </tbody>
</table>

#### 擷取資產

此動作模組會擷取此模組所用連線中，憑證由所代表之使用者所擁有的資產。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有關建立與的連線的指示 [!DNL Adobe Lightroom]，請參閱 <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >建立與的連線 [!DNL Adobe Lightroom]</a> 本文章內容。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL目錄ID]</td>
      <td>
        <p>輸入或對應包含資產的目錄ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL開始時間戳記]</td>
      <td>
        <p>輸入或對應時間戳記。 模組會傳回在此時間戳記之後更新的記錄。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL傳回之前擷取的資產]</td>
      <td>
        <p>以格式輸入日期 <code>YYYY-MM-DDT00:00:00</code>. 模組會傳回在此日期之前擷取的結果。</p><p> 此欄位無法與欄位搭配使用 <code>Return assets captured after</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL傳回資產的最大數量]</td>
      <td>
        <p>設定符合以下條件的資產數量上限： [!DNL Workfront Fusion] 將會在一個執行週期中傳回。 此數字必須小於或等於100。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL SHA256原始檔案的雜湊值]</td>
      <td>
        <p></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL隱藏棧疊內的資產？」]</td>
      <td>
        <p></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Asset子型別值]</td>
      <td>
        <p></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL資產ID]</td>
      <td>
        <p>輸入或對應最多100個資產ID，以逗號分隔。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL要排除的資產型別]</td>
      <td>
        <p>選取是否要排除完整或不完整的資產。 若要包含所有資產，請將此欄位留空。</p>
      </td>
    <tr>
      <td role="rowheader">[！UICONTROL群組值]</td>
      <td>
        <p></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL名稱值]</td>
      <td>
        <p></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL我的最愛狀態]</td>
      <td>
        <p></p>
      </td>
    </tr>
    </tr>
  </tbody>
</table>

### 相簿

* [將資產新增至相簿](#add-assets-to-an-album)
* [建立相簿](#create-an-album)
* [刪除相簿](#delete-an-album)
* [取得相簿](#get-an-album)
* [列出相簿的資產](#list-assets-of-an-album)
* [擷取相簿](#retrieve-albums)
* [更新相簿](#update-album)

#### 將資產新增至相簿

此動作模組會將一或多個資產新增至指定的相簿。 在一個執行週期最多可新增50個資產。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有關建立與的連線的指示 [!DNL Adobe Lightroom]，請參閱 <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >建立與的連線 [!DNL Adobe Lightroom]</a> 本文章內容。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL目錄ID]</td>
      <td>
        <p>輸入或對應目錄ID，該目錄包含您要新增資產的相簿。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL相簿ID]</td>
      <td>
        <p>輸入或對應您要新增資產的相簿識別碼。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Assets]</td>
      <td>
        <p>針對您想要新增至相簿的每個資產，按一下 <b>新增專案</b> 並輸入下列欄位。</p>
      </td>
    <tr>
      <td role="rowheader">[！UICONTROL資產ID]</td>
      <td>
        <p>輸入或對應您要新增至相簿的資產ID</p>
      </td>
    <tr>
      <td role="rowheader">[！UICONTROL此資產是否為專輯封面？]</td>
      <td>
        <p>選取是否要將此資產顯示為代表相簿的影像。</p>
      </td>
    <tr>
      <td role="rowheader">[！UICONTROL順序]</td>
      <td>
        <p></p>
      </td>
    <tr>
      <td role="rowheader">[！UICONTROL中繼資料]</td>
      <td>
        <p>輸入或對應您要納入資產的任何中繼資料。 這必須是單一文字字串，最大長度為1-24個字元。</p>
      </td>
    <tr>
      <td role="rowheader">[！UICONTROL遠端ID]</td>
      <td>
        <p>輸入資產的識別碼。</p>
      </td>
    </tr>
  </tbody>
</table>

#### 建立相簿

此動作模組會在Lightroom中建立新相簿。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有關建立與的連線的指示 [!DNL Adobe Lightroom]，請參閱 <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >建立與的連線 [!DNL Adobe Lightroom]</a> 本文章內容。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL目錄ID]</td>
      <td>
        <p>輸入或對應您要建立相簿的目錄ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL相簿ID]</td>
      <td>
        <p>輸入或對應新相簿的ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Subtype]</td>
      <td>
        <p>選取相簿的子型別。</p>
      </td>
    <tr>
      <td role="rowheader">[！UICONTROL API金鑰]</td>
      <td>
        <p>輸入建立相簿之服務的API金鑰。</p>
      </td>
    <tr>
      <td role="rowheader">[！UICONTROL日期時間使用者已建立]</td>
      <td>
        <p>輸入或對應格式的日期 <code>YYYY-MM-DDT00:00:00-00:00Z</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL日期時間使用者已更新]</td>
      <td>
        <p>輸入或對應格式的日期 <code>YYYY-MM-DDT00:00:00-00:00Z</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL專輯名稱]</td>
      <td>
        <p>輸入或對應新相簿的名稱。</p>
      </td>
    <tr>
      <td role="rowheader">[！UICONTROL封面ID]</td>
      <td>
        <p>輸入或對應要當作此相簿封面的資產ID。</p>
      </td>
    <tr>
      <td role="rowheader">[！UICONTROL遠端ID]</td>
      <td>
        <p>輸入資產的識別碼。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL建立日期]</td>
      <td>
        <p>輸入或對應格式的日期 <code>YYYY-MM-DDT00:00:00-00:00Z</code>.</p>
      </td>
    <tr>
      <td role="rowheader">[！UICONTROL更新日期]</td>
      <td>
        <p>輸入或對應格式的日期 <code>YYYY-MM-DDT00:00:00-00:00Z</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL專輯已刪除嗎？]</td>
      <td>
        <p>如果刪除了外部附屬內容，則啟用此選項。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL URL of location to edit ailiated content]</td>
      <td>
        <p>如果有使用者可以編輯此相簿內容的URL，請在此輸入URL。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL URL of location to view affiliated content]</td>
      <td>
        <p>如果有使用者可以檢視此相簿內容的URL，請在此輸入URL。</p>
      </td>
    </tr>
  </tbody>
</table>

#### 刪除相簿

此動作模組會刪除相簿。

已刪除的相簿必須由目前要刪除該相簿的相同使用者端應用程式建立，而且必須是子型別 `project` 或 `project_set`.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有關建立與的連線的指示 [!DNL Adobe Lightroom]，請參閱 <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >建立與的連線 [!DNL Adobe Lightroom]</a> 本文章內容。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL目錄ID]</td>
      <td>
        <p>輸入或對應包含要刪除之相簿的目錄ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL相簿ID]</td>
      <td>
        <p>輸入或對應您要刪除的相簿識別碼。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL刪除子專輯？]</td>
      <td>
        <p>選取是否要刪除已刪除相簿的子相簿。</p>
      </td>
    </tr>
  </tbody>
</table>

### 取得相簿

此動作模組會擷取指定的相簿

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有關建立與的連線的指示 [!DNL Adobe Lightroom]，請參閱 <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >建立與的連線 [!DNL Adobe Lightroom]</a> 本文章內容。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL目錄ID]</td>
      <td>
        <p>輸入或對應包含您要擷取之相簿的目錄ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL相簿ID]</td>
      <td>
        <p>輸入或對應您要擷取的相簿ID。</p>
      </td>
    </tr>
  </tbody>
</table>

#### 列出相簿的資產

此動作模組會擷取指定相簿中的資產清單。



#### 擷取相簿

此動作模組會擷取指定目錄中的相簿清單。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有關建立與的連線的指示 [!DNL Adobe Lightroom]，請參閱 <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >建立與的連線 [!DNL Adobe Lightroom]</a> 本文章內容。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL目錄ID]</td>
      <td>
        <p>輸入或對應包含您要擷取之相簿的目錄ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL子型別]</td>
      <td>
        <p>輸入或對應您要擷取的相簿ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL目前結果前面的相簿名稱]</td>
      <td>
        <p>如果您要分頁結果，請輸入或對應上一頁最後一張相簿的名稱。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL傳回專輯的最大數量]</td>
      <td>
        <p>設定符合以下條件的資產數量上限： [!DNL Workfront Fusion] 將會在一個執行週期中傳回。 此欄位的預設值為100。如果限制邊界有多個相簿相同，則此模組傳回的相簿可能會超過此限制 <code>name_after</code> 值。</p>
      </td>
    </tr>
  </tbody>
</table>

#### 更新相簿

此動作模組會更新指定的相簿。

更新的相簿必須是由目前進行更新的相同使用者端應用程式所建立，而且必須是子型別 `project` 或 `project_set`.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有關建立與的連線的指示 [!DNL Adobe Lightroom]，請參閱 <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >建立與的連線 [!DNL Adobe Lightroom]</a> 本文章內容。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL目錄ID]</td>
      <td>
        <p>輸入或對應包含要更新之相簿的目錄ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL相簿ID]</td>
      <td>
        <p>輸入或對應您要更新的相簿識別碼。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">其他欄位</td>
      <td>
      <td>如需此模組中其他欄位的說明，請參閱 <a href="#create-an-album" class="MCXref xref" >建立相簿</a> 本文章內容。</td>
      </td>
    </tr>
  </tbody>
</table>










