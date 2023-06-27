---
title: 加寬模組
description: 在 [!DNL Adobe Workfront Fusion] 情境下，您可以自動化使用下列專案的工作流程： [!UICONTROL 加寬]，以及將其連線到多個協力廠商應用程式和服務。
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: d46935bc-4f6c-4502-bd2f-3927f33241e1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1586'
ht-degree: 1%

---

# [!DNL Widen] 模組

在 [!DNL Adobe Workfront Fusion] 情境下，您可以自動化使用下列專案的工作流程： [!UICONTROL 加寬]，以及將其連線到多個協力廠商應用程式和服務。

如果您需要建立案例的說明，請參閱 [在中建立情境 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

如需模組的相關資訊，請參閱 [中的模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

若要瞭解您擁有哪些計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

有關以下專案的資訊： [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 必要條件

使用 [!UICONTROL 加寬] 模組，您必須擁有 [!UICONTROL 加寬] 帳戶。

## Connect [!DNL Widen] 至 [!DNL Workfront Fusion] {#connect-widen-to-workfront-fusion}

您可以建立與的連線 [!DNL Widen] 直接從a內的帳戶 [!DNL Widen] 模組。

1. 在任何 [!DNL Widen] 模組，按一下 **[!UICONTROL 新增]** 旁邊 [!UICONTROL 連線] 欄位。
1. 選取 [!DNL Widen] 您要連線的網域。
1. 輸入您的Token [!DNL Widen] 帳戶。 如需尋找此Token的指示，請參閱 [[!DNL Widen] API常見問題集](https://community.widen.com/collective/s/article/API-FAQs).
1. 按一下 **[!UICONTROL 繼續]** 以建立連線並返回模組。

## [!DNL Widen] 模組及其欄位

當您設定 [!DNL Widen] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 除了這些以外， [!DNL Widen] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應至中的另一個模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [觸發器模組](#trigger-modules)
* [動作模組](#action-modules)
* [搜尋模組](#search-modules)

### 觸發器模組

#### [!UICONTROL 觀看資產]

建立或更新資產時，此觸發模組就會啟動案例。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
  <td> <p>如需有關連線您的電腦的指示， [!DNL Widen] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connect [!DNL Widen] 至 [!DNL Workfront Fusion] </a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL事件型別]</td> 
   <td> <p>選取您要觀看新資產或更新資產。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL展開]</td> 
   <td> <p>選取除了資產欄位之外，您想包含在模組輸出中的屬性。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸出]</td> 
   <td>選取您要納入模組輸出的欄位。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>輸入或對應每個案例執行週期中您希望模組使用的最大資產數量。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 動作模組

* [[!UICONTROL 自訂API呼叫]](#custom-api-call)
* [[!UICONTROL 讀取資產資訊]](#read-asset-info)
* [[!UICONTROL 將資產新增至收藏集]](#add-assets-to-collections)
* [[!UICONTROL 從集合中移除資產]](#remove-assets-from-collection)
* [[!UICONTROL 更新資產中繼資料]](#update-asset-metadata)
* [[!UICONTROL 下載檔案]](#download-file)
* [[!UICONTROL 上傳] 檔案](#upload-a-file)

#### [!UICONTROL 自訂API呼叫]

此動作模組可讓您對 [!DNL Widen] API。 如此一來，您就可以建立其他人無法完成的資料流程自動化 [!DNL Widen] 模組。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Widen] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connect [!DNL Widen] 至 [!DNL Workfront Fusion] </a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL API版本]</td> 
   <td>選取是否要使用最新版的 [!DNL Widen] API或1.0版</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL URL]</td> 
   <td>輸入或對應您API呼叫的URL。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL方法]</td> 
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL標頭]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標頭。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>[！UICONTROL Workfront Fusion]會為您新增授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查詢字串]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的查詢。</p> <p>例如： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL內文]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的正文內容。</p> <p>備註:  <p>使用條件陳述式時，例如 <code>if</code> 在JSON中，將引號放在條件陳述式之外。</p> 
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
   <td role="rowheader">[！UICONTROL連線]</td> 
  <td> <p>如需有關連線您的電腦的指示， [!DNL Widen] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connect [!DNL Widen] 至 [!DNL Workfront Fusion] </a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資產ID]</td> 
   <td> <p>輸入或對應您要讀取資訊之資產的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL展開]</td> 
   <td> <p>選取除了資產欄位之外，您想包含在模組輸出中的屬性。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸出]</td> 
   <td>選取您要納入模組輸出的欄位。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 將資產新增至收藏集]

此動作模組會將一個或多個資產新增至集合。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
  <td> <p>如需有關連線您的電腦的指示， [!DNL Widen] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connect [!DNL Widen] 至 [!DNL Workfront Fusion] </a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL集合ID]</td> 
   <td> <p>針對您想要新增資產的每個集合：</p> 
    <ol> 
     <li value="1"> <p> 按一下 <strong>[！UICONTROL新增]</strong>.</p> </li> 
     <li value="2"> <p>輸入或對應[！UICONTROL集合ID]。</p> </li> 
     <li value="3"> <p>按一下 <strong>[！UICONTROL新增專案]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資產ID]</td> 
   <td> <p>針對您想要新增至集合的每個資產：</p> 
    <ol> 
     <li value="1"> <p> 按一下 <strong>[！UICONTROL新增]</strong>.</p> </li> 
     <li value="2"> <p>輸入或對應資產ID。</p> </li> 
     <li value="3"> <p>按一下 <strong>[！UICONTROL新增專案]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>輸入或對應每個案例執行週期中您希望模組使用的最大資產數量。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 從集合中移除資產]

此動作模組會從集合中移除一個或多個資產。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
  <td> <p>如需有關連線您的電腦的指示， [!DNL Widen] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connect [!DNL Widen] 至 [!DNL Workfront Fusion] </a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL集合ID]</td> 
   <td> <p>針對您想要從中移除資產的每個集合：</p> 
    <ol> 
     <li value="1"> <p> 按一下 <strong>[！UICONTROL新增]</strong>.</p> </li> 
     <li value="2"> <p>輸入或對應「集合ID」。</p> </li> 
     <li value="3"> <p>按一下 <strong>[！UICONTROL新增專案]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">資產ID</td> 
   <td> <p>針對您要從集合中移除的每個資產：</p> 
    <ol> 
     <li value="1"> <p> 按一下 <strong>[！UICONTROL新增]</strong>.</p> </li> 
     <li value="2"> <p>輸入或對應資產ID。</p> </li> 
     <li value="3"> <p>按一下 <strong>[！UICONTROL新增專案]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>輸入或對應每個案例執行週期中您希望模組使用的最大資產數量。</p> </td> 
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
   <td role="rowheader">[！UICONTROL連線]</td> 
  <td> <p>如需有關連線您的電腦的指示， [!DNL Widen] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connect [!DNL Widen] 至 [!DNL Workfront Fusion] </a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資產ID]</td> 
   <td> <p>輸入或對應您要更新中繼資料的資產ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL中繼資料型別]</td> 
   <td> <p>選取您要更新之中繼資料的中繼資料型別。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL中繼資料]</td> 
   <td>選取您要更新的中繼資料欄位。 針對每個欄位，輸入欄位的新值。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>輸入或對應每個案例執行週期中您希望模組使用的最大資產數量。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 下載檔案]

此動作模組會從您的下載資產 [!DNL Widen] 帳戶。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
  <td> <p>如需有關連線您的電腦的指示， [!DNL Widen] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connect [!DNL Widen] 至 [!DNL Workfront Fusion] </a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資產ID]</td> 
   <td> <p>輸入或對應您要下載的資產的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 上傳檔案]

此動作模組會將檔案上傳至 [!DNL Widen] 帳戶。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
  <td> <p>如需有關連線您的電腦的指示， [!DNL Widen] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connect [!DNL Widen] 至 [!DNL Workfront Fusion] </a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL上傳設定檔]</td> 
   <td> <p>選取您要模組使用的上傳設定檔。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL上傳方法]</td> 
   <td> <p>選取您要如何上傳檔案。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL From File]</strong> </p> <p>從先前的模組選取或對應來源檔案。</p> </li> 
     <li> <p><strong>[！UICONTROL By URL]</strong> </p> <p>輸入或對應您要上傳之檔案的URL。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL檔案名稱]</td> 
   <td>輸入或對應已上傳檔案的名稱。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL中繼資料型別]</td> 
   <td>選取您要上傳之檔案的中繼資料型別。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL中繼資料]</td> 
   <td>選取要包含在檔案上傳中的中繼資料欄位。 對於每個欄位，輸入該欄位的[！UICONTROL值]。</td> 
  </tr> 
 </tbody> 
</table>

### 搜尋模組

* [[!UICONTROL 讀取集合資產]](#read-collection-assets)
* [[!UICONTROL 搜尋資產]](#search-assets)

#### [!UICONTROL 讀取集合資產]

此動作模組會擷取集合中的資產清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
  <td> <p>如需有關連線您的電腦的指示， [!DNL Widen] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connect [!DNL Widen] 至 [!DNL Workfront Fusion] </a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL集合ID]</td> 
   <td> <p>輸入或對應包含您要讀取之資產的集合ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL開始]</td> 
   <td>輸入或對映您要列出的第一個專案編號。 這是分頁記錄的方式。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL最大值]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期內傳回的最大記錄數。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL排序依據]</td> 
   <td> <p>選取您要用來排序資產的屬性。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL順序]</td> 
   <td>選取您要以遞增或遞減方式排序資產。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸出]</td> 
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
   <td role="rowheader">[！UICONTROL連線]</td> 
  <td> <p>如需有關連線您的電腦的指示， [!DNL Widen] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Connect [!DNL Widen] 至 [!DNL Workfront Fusion] </a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL搜尋查詢]</td> 
   <td> <p>輸入您要搜尋資產的條件。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL排序依據]</td> 
   <td> <p>選取您要如何排序資產。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL順序]</td> 
   <td>選取您要以遞增或遞減方式排序資產。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL包含已刪除]</td> 
   <td>啟用此選項以在搜尋中包含已刪除的資產。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL包含已封存的]</p> </td> 
   <td> <p>啟用此選項以在搜尋中包含已封存的資產。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL搜尋檔案文字]</td> 
   <td>啟用此選項可在搜尋中包含檔案文字，或啟用False僅包含標題符合搜尋條件的資產。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期內傳回的最大記錄數。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL位移]</td> 
   <td>輸入或對應您要擷取其詳細資訊的第一個專案編號。 這是分頁記錄的方式。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL捲動]</td> 
   <td>啟用此選項可允許捲動。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL展開]</td> 
   <td> <p>選取除了資產欄位之外，您想包含在模組輸出中的屬性。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸出]</td> 
   <td>選取您要納入模組輸出的欄位。</td> 
  </tr> 
 </tbody> 
</table>
