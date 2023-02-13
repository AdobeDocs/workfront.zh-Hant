---
title: 擴展模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!UICONTROL 擴展]，並將其連接至多個協力廠商應用程式和服務。
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: d46935bc-4f6c-4502-bd2f-3927f33241e1
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1538'
ht-degree: 1%

---

# [!DNL Widen] 模組

在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!UICONTROL 擴展]，並將其連接至多個協力廠商應用程式和服務。

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

使用 [!UICONTROL 擴展] 模組，您必須 [!UICONTROL 擴展] 帳戶。

## Connect [!DNL Widen] to [!DNL Workfront Fusion] {#connect-widen-to-workfront-fusion}

您可以建立與 [!DNL Widen] 直接從內部 [!DNL Widen] 模組。

1. 在任何 [!DNL Widen] 模組，按一下 **[!UICONTROL 新增]** 旁邊 [!UICONTROL 連線] 欄位。
1. 選取 [!DNL Widen] 要連接的域。
1. 輸入您的 [!DNL Widen] 帳戶。 如需找到此代號的指示，請參閱 [[!DNL Widen] API常見問題集](https://community.widen.com/collective/s/article/API-FAQs).
1. 按一下 **[!UICONTROL 繼續]** 若要建立連線，請返回模組。

## [!DNL Widen] 模組及其欄位

設定時 [!DNL Widen] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!DNL Widen] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [觸發模組](#trigger-modules)
* [動作模組](#action-modules)
* [搜尋模組](#search-modules)

### 觸發模組

#### [!UICONTROL 監看資產]

此觸發器模組會在資產建立或更新時啟動案例。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
  <td> <p>有關連接 [!DNL Widen] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connect [!DNL Widen] to [!DNL Workfront Fusion] </a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL事件類型]</td> 
   <td> <p>選取您要觀看新資產或更新的資產。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL展開]</td> 
   <td> <p>除了資產欄位，請選取您要納入模組輸出的屬性。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸出]</td> 
   <td>選取您要納入模組輸出的欄位。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>輸入或對應您希望模組在每個方案執行週期期間使用的資產數量上限。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 動作模組

* [[!UICONTROL 自訂API呼叫]](#custom-api-call)
* [[!UICONTROL 讀取資產資訊]](#read-asset-info)
* [[!UICONTROL 新增資產至集合]](#add-assets-to-collections)
* [[!UICONTROL 從集合中移除資產]](#remove-assets-from-collection)
* [[!UICONTROL 更新資產中繼資料]](#update-asset-metadata)
* [[!UICONTROL 下載檔案]](#download-file)
* [[!UICONTROL 上傳] 檔案](#upload-a-file)

#### [!UICONTROL 自訂API呼叫]

此動作模組可讓您對 [!DNL Widen] API。 這樣，您就可以建立資料流自動化，而另一個無法完成 [!DNL Widen] 模組。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Widen] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connect [!DNL Widen] to [!DNL Workfront Fusion] </a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL API版本]</td> 
   <td>選取您是否要使用 [!DNL Widen] API或1.0版</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>輸入或對應API呼叫的URL。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL方法]</td> 
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL標題]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標題。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>[!UICONTROL Workfront Fusion]為您添加授權標頭。</p> </td> 
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

#### [!UICONTROL 讀取資產資訊]

此動作模組會依其唯一ID擷取個別資產。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
  <td> <p>有關連接 [!DNL Widen] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connect [!DNL Widen] to [!DNL Workfront Fusion] </a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資產ID]</td> 
   <td> <p>輸入或對應您要讀取資訊的資產ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL展開]</td> 
   <td> <p>除了資產欄位，請選取您要納入模組輸出的屬性。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸出]</td> 
   <td>選取您要納入模組輸出的欄位。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 新增資產至集合]

此動作模組會新增一或多個資產至集合。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
  <td> <p>有關連接 [!DNL Widen] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connect [!DNL Widen] to [!DNL Workfront Fusion] </a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL集合ID]</td> 
   <td> <p>針對您要新增資產的每個集合：</p> 
    <ol> 
     <li value="1"> <p> 按一下 <strong>[!UICONTROL添加]</strong>.</p> </li> 
     <li value="2"> <p>輸入或映射[!UICONTROL集合ID]。</p> </li> 
     <li value="3"> <p>按一下 <strong>[!UICONTROL添加項]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資產ID]</td> 
   <td> <p>針對您要新增至集合的每個資產：</p> 
    <ol> 
     <li value="1"> <p> 按一下 <strong>[!UICONTROL添加]</strong>.</p> </li> 
     <li value="2"> <p>輸入或對應資產ID。</p> </li> 
     <li value="3"> <p>按一下 <strong>[!UICONTROL添加項]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>輸入或對應您希望模組在每個方案執行週期期間使用的資產數量上限。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 從集合中移除資產]

此動作模組會從集合中移除一或多個資產。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
  <td> <p>有關連接 [!DNL Widen] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connect [!DNL Widen] to [!DNL Workfront Fusion] </a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL集合ID]</td> 
   <td> <p>針對您要從中移除資產的每個集合：</p> 
    <ol> 
     <li value="1"> <p> 按一下 <strong>[!UICONTROL添加]</strong>.</p> </li> 
     <li value="2"> <p>輸入或對應收集ID。</p> </li> 
     <li value="3"> <p>按一下 <strong>[!UICONTROL添加項]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">資產ID</td> 
   <td> <p>針對您要從集合中移除的每個資產：</p> 
    <ol> 
     <li value="1"> <p> 按一下 <strong>[!UICONTROL添加]</strong>.</p> </li> 
     <li value="2"> <p>輸入或對應資產ID。</p> </li> 
     <li value="3"> <p>按一下 <strong>[!UICONTROL添加項]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>輸入或對應您希望模組在每個方案執行週期期間使用的資產數量上限。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新資產中繼資料]

此動作模組會更新資產的中繼資料欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
  <td> <p>有關連接 [!DNL Widen] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connect [!DNL Widen] to [!DNL Workfront Fusion] </a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資產ID]</td> 
   <td> <p>輸入或對應您要更新中繼資料之資產的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL元資料類型]</td> 
   <td> <p>選取您要更新之中繼資料的中繼資料類型。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL元資料]</td> 
   <td>選取您要更新的中繼資料欄位。 對於每個欄位，輸入欄位的新值。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>輸入或對應您希望模組在每個方案執行週期期間使用的資產數量上限。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 下載檔案]

此動作模組會從 [!DNL Widen] 帳戶。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
  <td> <p>有關連接 [!DNL Widen] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connect [!DNL Widen] to [!DNL Workfront Fusion] </a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資產ID]</td> 
   <td> <p>輸入或對應您要下載的資產ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 上傳檔案]

此動作模組會將檔案上傳至您的 [!DNL Widen] 帳戶。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
  <td> <p>有關連接 [!DNL Widen] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connect [!DNL Widen] to [!DNL Workfront Fusion] </a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL上載配置檔案]</td> 
   <td> <p>選取您要模組使用的上傳設定檔。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL上載方法]</td> 
   <td> <p>選取要如何上傳檔案。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL從檔案]</strong> </p> <p>從上一個模組選擇或映射源檔案。</p> </li> 
     <li> <p><strong>[!UICONTROL（按URL）]</strong> </p> <p>輸入或對應您要上傳之檔案的URL。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL檔案名]</td> 
   <td>輸入或映射已上載檔案的名稱。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL元資料類型]</td> 
   <td>選取您要上傳之檔案的中繼資料類型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL元資料]</td> 
   <td>選取您要納入檔案上傳的中繼資料欄位。 對於每個欄位，為欄位輸入[!UICONTROL值]。</td> 
  </tr> 
 </tbody> 
</table>

### 搜尋模組

* [[!UICONTROL 讀取集合資產]](#read-collection-assets)
* [[!UICONTROL 搜尋資產]](#search-assets)

#### [!UICONTROL 讀取集合資產]

此動作模組會擷取集合內的資產清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
  <td> <p>有關連接 [!DNL Widen] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connect [!DNL Widen] to [!DNL Workfront Fusion] </a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL集合ID]</td> 
   <td> <p>輸入或對應包含您要讀取之資產的集合ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL開始]</td> 
   <td>輸入或映射要列出的第一個項目的編號。 這是為記錄分頁的方法。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL最大值]</td> 
   <td> <p>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL排序依據]</td> 
   <td> <p>選取要依據哪個屬性來排序資產。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL順序]</td> 
   <td>選取您要以遞增或遞減方式排序資產。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸出]</td> 
   <td>選取您要納入模組輸出的欄位。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 搜尋資產]

此搜尋模組會擷取符合特定搜尋條件的資產清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
  <td> <p>有關連接 [!DNL Widen] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connect [!DNL Widen] to [!DNL Workfront Fusion] </a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL搜索查詢]</td> 
   <td> <p>輸入要依據哪個條件來搜尋資產。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL排序依據]</td> 
   <td> <p>選取要如何排序資產。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL順序]</td> 
   <td>選取您要以遞增或遞減方式排序資產。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！已刪除UICONTROL包含]</td> 
   <td>啟用此選項，將刪除的資產包含在搜尋中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL包含已存檔]</p> </td> 
   <td> <p>啟用此選項，將封存的資產包含在搜尋中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL搜索文檔文本]</td> 
   <td>啟用此選項可在搜尋中包含檔案文字，或啟用false以僅包含標題符合搜尋條件的資產。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL偏移]</td> 
   <td>輸入或映射要檢索詳細資訊的第一個項目的編號。 這是為記錄分頁的方法。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL滾動]</td> 
   <td>啟用此選項以允許滾動。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL展開]</td> 
   <td> <p>除了資產欄位，請選取您要納入模組輸出的屬性。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸出]</td> 
   <td>選取您要納入模組輸出的欄位。</td> 
  </tr> 
 </tbody> 
</table>
