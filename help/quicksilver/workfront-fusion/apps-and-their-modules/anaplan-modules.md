---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Anaplan模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動化使用Anaplan的工作流程，並將其連線到多個第三方應用程式和服務。
author: Becky
feature: Workfront Fusion, Workfront Integrations and Apps
exl-id: 03bcd0a4-c8ec-4f44-b1e1-b57e79595309
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '1844'
ht-degree: 1%

---

# [!DNL Anaplan] 模組

在 [!DNL Adobe Workfront Fusion] 情境下，您可以自動化使用下列專案的工作流程： [!DNL Anaplan]，以及將其連線到多個協力廠商應用程式和服務。

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

開始使用 [!DNL Anaplan] 聯結器時，您必須確保符合下列先決條件：

* 您必須有使用中 [!UICONTROL Anaplan] 帳戶。
* 您必須設定工作區、模型及其他 [!DNL Anaplan] 中的物件 [!UICONTROL Anaplan] 之前帳戶 [!DNL Workfront Fusion] 可以與他們互動。

## Connect [!DNL Anaplan] 至 [!DNL Workfront Fusion] {#connect-anaplan-to-workfront-fusion}

若要為建立連線，請執行下列步驟： [!DNL Anaplan] 模組：

1. 按一下 **[!UICONTROL 新增]** 旁邊 [!UICONTROL 連線] 方塊。
1. 選取連線型別。

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!DNL Anaplan] [！UICONTROL Basic]</td> 
      <td> <p>一個 [!DNL Anaplan] [！UICONTROL Basic]連線只需要電子郵件地址和密碼即可建立連線。 </p> <p>輸入連線的名稱，然後輸入您的電子郵件地址和密碼 [!DNL Anaplan] 帳戶。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Anaplan] [！UICONTROL CA憑證]</td> 
      <td> <p>一個 [!DNL Anaplan] [！UICONTROL CA Certificate]連線需要[！UICONTROL憑證金鑰]、[！UICONTROL編碼資料]和[！UICONTROL編碼已簽署資料]。 您可在以下位置產生這些： [!DNL Anaplan] 帳戶。 如需指示，請參閱 [!DNL Anaplan] 說明檔案。</p> <p>輸入連線的名稱，然後輸入您在中產生的[！UICONTROL憑證金鑰]、[！UICONTROL編碼資料]和[！UICONTROL編碼簽署資料]。 [!DNL Anaplan] 帳戶。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **[!UICONTROL 繼續]** 以儲存連線並返回模組。

## [!DNL Anaplan] 模組及其欄位

當您設定 [!DNL Anaplan] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 除了這些以外， [!DNL Anaplan] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應至中的另一個模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [觸發器](#triggers)
* [動作](#actions)
* [搜尋](#searches)

### 觸發器

#### [!DNL Watch records]

建立或更新所選型別的記錄時，此觸發模組就會啟動案例。

>[!NOTE]
>
>此模組會傳回新記錄的資料。 它不會傳回已修改現有記錄的資料。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td>如需建立連線的相關指示，請前往 [!DNL Anaplan]，請參閱 <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect [!DNL Anaplan] 至 [!DNL Workfront Fusion]</a> 本文章內容。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">要觀看的物件型別</td> 
   <td>選取您要觀看的專案型別。 建立或更新此型別的記錄時，此案例就會開始。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">&lt;object&gt; ID</td> 
   <td>在Anaplan中輸入與您要觀看的物件相關聯的物件ID，例如模型或模組</td> 
  </tr> 
  <tr> 
   <td role="rowheader">限制</td> 
   <td> <p>在每個案例執行週期中，輸入或對應您希望模組在[action]的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 動作

* [[!UICONTROL 建立清單專案]](#create-a-list-item)
* [[!UICONTROL 進行自訂API呼叫]](#make-a-custom-api-call)
* [[!UICONTROL 讀取記錄]](#read-a-record)
* [[!UICONTROL 執行動作]](#run-an-action)
* [[!UICONTROL 更新記錄]](#update-a-record)
* [[!UICONTROL 上傳檔案]](#upload-a-file)

#### [!UICONTROL 建立清單專案]

此動作模組會將新專案新增至Anaplan中的清單。

<table style="table-layout:auto">
    <tr>
        <td>[！UICONTROL連線]</td>
        <td>如需建立連線的相關指示，請前往 [!DNL Anaplan]，請參閱 <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect [!DNL Anaplan] 至 [!DNL Workfront Fusion]</a> 本文章內容。</td>
    </tr>
    <tr>
        <td>[！UICONTROL工作區ID]</td>
        <td>選取或對應包含您要新增專案之清單的Anaplan Workspace的ID。</td>
    </tr>
    <tr>
        <td>[！UICONTROL模型ID]</td>
        <td>選取或對應包含您要新增專案之清單的模型ID。</td>
    </tr>
    <tr>
        <td>[！UICONTROL清單ID]</td>
        <td>選取或對應您要建立專案之清單的ID。</td>
    </tr>
    <tr>
        <td>[！UICONTROL名稱]</td>
        <td>輸入新專案的名稱。</td>
    </tr>
    <tr>
        <td>[！UICONTROL程式碼]</td>
        <td>輸入新料號的代碼。 代碼是使用者產生的代碼，可讓您區分具有相同名稱的明細專案。</td>
    </tr>
    <tr>
        <td>[！UICONTROL Parent]</td>
        <td>輸入您要在其下建立新專案的上階專案名稱。</td>
    </tr>
    <tr>
        <td>[！UICONTROL屬性]</td>
        <td>如果您要新增專案的清單具有自訂屬性，請選取您要新增值的屬性，然後新增值。</td>
    </tr>
    <tr>
        <td>[！UICONTROL子集]</td>
        <td>如果要新增專案的清單有自訂子集，請選取要新增專案的子集，然後選取 <b>[！UICONTROL是]</b> 將新專案新增至該子集。</td>
    </tr>
</table>

#### [!UICONTROL 進行自訂API呼叫]

此模組可讓您對執行自訂API呼叫 [!DNL Anaplan] API。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td>如需建立連線的相關指示，請前往 [!DNL Anaplan]，請參閱 <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect [!DNL Anaplan] 至 [!DNL Workfront Fusion]</a> 本文章內容。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL URL]</p> </td> 
   <td> <p>輸入相對於 <code>https://api.anaplan.com/2/0/</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL方法]</p> </td> 
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL標頭]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標頭。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 自動新增授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查詢字串] </td> 
   <td> <p>輸入請求查詢字串。</p> </td> 
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

#### [!UICONTROL 刪除記錄]

此動作模組會刪除現有記錄。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td>如需建立連線的相關指示，請前往 [!DNL Anaplan]，請參閱 <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect [!DNL Anaplan] 至 [!DNL Workfront Fusion]</a> 本文章內容。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL工作區ID]</td> 
   <td>選取或對應包含您要刪除之物件的Anaplan Workspace的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL模型ID]</td> 
   <td>輸入或對應包含您要刪除之物件的模型ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">刪除</td> 
   <td> <p>選取要刪除的物件型別。</p> 
    <ul> 
     <li> <p><b>動作</b> </p> <p>選取或對映要刪除的動作。</p> </li> 
     <li> <p><b>清單專案</b> </p> <p>選取您要從中刪除專案的清單，然後輸入或對應您要刪除之專案的ID或代碼</p>  </li> 
     <li> <p><b>[！UICONTROL檔案]</b> </p> <p>選取或對應要刪除的檔案。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 讀取記錄]

此動作模組讀取單一記錄。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td>如需建立連線的相關指示，請前往 [!DNL Anaplan]，請參閱 <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect [!DNL Anaplan] 至 [!DNL Workfront Fusion]</a> 本文章內容。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別]</td> 
   <td> <p>選取要讀取的記錄型別。</p> 
    <ul> 
     <li> <p><b>模型</b> </p> <p>選取或對應您要讀取的模型ID</p> </li> 
     <li> <p><b>模型清單</b> </p> <p>選取或對應包含您要讀取之清單的工作區和模型的ID，然後選取清單。 在[！UICONTROL資料型別]欄位中，選取您要讀取資料還是中繼資料。</p> </li> 
     <li> <p><b>模型版本</b> </p> <p>選取或對應您要讀取的模型ID。</p> </li> 
     <li> <p><b>使用者</b> </p> <p>選取您是否要傳回正在使用的帳戶擁有者或其他使用者的相關資料。 如果您選取其他使用者，請選取該使用者的名稱。</p> </li> 
     <li> <p><b>工作區</b> </p> <p>選取或對應您要讀取的工作區的ID。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 執行動作]

此動作模組會匯入、匯出、刪除或處理動作。

<table style="table-layout:auto"> 
     <col/>
     <col/>
     <tbody>
      <tr>
        <td role="rowheader">[！UICONTROL連線]</td>
        <td>如需建立連線的相關指示，請前往 [!DNL Anaplan]，請參閱 <a href="#Connect" class="MCXref xref" >[！UICONTROL Connect Anaplan至Workfront Fusion]</a> 本文章內容。</td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL工作區ID]</td>
        <td>選擇或對應 [!DNL Anaplan] 您要執行動作的工作區</td>
      </tr>
      <tr >
        <td role="rowheader">[！UICONTROL模型ID]</td>
        <td>選取或對應您要執行動作之模型的ID。</td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL動作型別]</td>
        <td>
          <p>選取您要執行的動作</p>
            <ul>
              <li>
                <p><b>[！UICONTROL Delete]</b>
                </p>
                <p>輸入或對應您要刪除之動作的ID。</p>
              </li>
              <li>
                <p><b>[！UICONTROL匯出]</b>
                </p>
                <p>輸入或對應您要使用之匯出定義的ID。 您可以匯出為下列檔案格式：</p>
                  <ul>
                    <li>
                      <p>XLS</p>
                    </li>
                    <li>
                      <p>XLSX</p>
                    </li>
                    <li>
                      <p>CSV</p>
                    </li>
                  </ul>
                </li>
                <li>
                  <p><b>[！UICONTROL匯入] </b>
                  </p>
                  <p style="font-weight: normal;">輸入或對應您要使用的匯入定義ID。</p>
                </li>
                <li>
                 <p><b>[！UICONTROL程式]</b>
                 </p>
                  <p>輸入或對應您要使用的程式ID。 </p>
                </li>
              </ul>
            </td>
          </tr>
        </tbody>
      </table>


#### [!UICONTROL 更新記錄]

此動作模組會更新中的單一記錄 [!UICONTROL Anaplan].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td>如需建立連線的相關指示，請前往 [!DNL Anaplan]，請參閱 <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect [!DNL Anaplan] 至 [!DNL Workfront Fusion]</a> 本文章內容。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別]</td> 
   <td> <p>選取您要更新的記錄型別。</p> 
    <ul> 
     <li> <p><b>[！UICONTROL清單專案]</b> </p> <p>如需欄位，請參閱 <a href="#create-a-list-item" class="MCXref xref">建立清單專案</a> 本文章內容。</p> </li> 
     <li> <p><b>[！UICONTROL模組儲存格資料]</b> </p> <p>當您更新儲存格資料時，使用該資料的所有下游計算也會更新。</p> <p>填寫下列欄位：</p> 
      <ul> 
       <li> <p><b>[！UICONTROL模型ID]</b> </p> <p>選取或對應包含您要更新之儲存格的模型。</p> </li> 
       <li> <p><b>[！UICONTROL模組ID]</b> </p> <p>選取或對應包含您要更新之儲存格的模組</p> </li> 
       <li> <p><b>[！UICONTROL行專案名稱]</b> </p> <p>選取或對應您要更新的儲存格的行專案</p> </li> 
       <li> <p style="font-weight: bold;">[！UICONTROLDimensionID]</p> <p>選取或對應行專案上的維度。</p> 
       <p><b>備註: </b> 
       <ul>
       <li> Dimension索引鍵（值）必須為 <code>dimensionName</code> （下一個）或 <code>dimensionId</code> (ID)。</li>
       <li>專案索引鍵（值）必須是 <code>itemName</code> （文字）， <code>itemCode</code> （文字），或 <code>itemId</code> (ID)。</li>
       <li>Dimension和專案索引鍵必須是相同的型別（文字或ID）。
       </ul>
        </p> 
        <p>Dimension如需維度的相關資訊，請搜尋 [!DNL Anaplan Anapedia].</p> </li> 
       <li> <p><b>[！UICONTROL值]</b> </p> <p>輸入或對應儲存格的新值。</p> </li> 
      </ul> </li> 
     <li> <p><b>[！UICONTROL模型目前會計年度]</b> </p> <p>輸入您要更新其會計年度之模型的「工作區ID」和「模型ID」，然後輸入或對映模型的新年度。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 上傳檔案]

此動作模組會將檔案上傳至Anaplan。 檔案必須已上傳至Anaplan。 您可以使用此模組將其上傳至Anaplan中的其他位置。
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">[！UICONTROL連線]</td>
<td>如需建立連線的相關指示，請前往 [!DNL Anaplan]，請參閱 <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect [!DNL Anaplan] 至 [!DNL Workfront Fusion]</a> 本文章內容。</td>
</tr>
<tr>
<td role="rowheader">[！UICONTROL工作區ID]</td>
<td>選擇或對應 [!DNL Anaplan] 您要上傳檔案的工作區。</td>
</tr>
<tr>
<td role="rowheader">[！UICONTROL模型ID]</td>
<td>選取或對應您要上傳檔案的模型ID。</td>
</tr>
<tr>
<td role="rowheader">[！UICONTROL檔案ID]</td>
<td>選取或對應您要上傳之檔案的ID。</td>
</tr>
</tbody>
</table>
</div>

### 搜尋

#### [!UICONTROL 取得記錄]

此搜尋模組會傳回所選型別的所有可存取記錄。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td>如需建立連線的相關指示，請前往 [!DNL Anaplan]，請參閱 <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect [!DNL Anaplan] 至 [!DNL Workfront Fusion]</a> 本文章內容。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別]</td> 
   <td> <p>選取您要擷取的記錄型別。</p> 
      <ul> 
       <li> <p><b>[！UICONTROL工作區]</b> </p> </li> 
       <li> <p><b>[！UICONTROL模型]</b> </p> </li> 
       <li> <p><b>[！UICONTROL行專案]</b> </p> <p>選取或對應包含 [!DNL line] 要擷取的專案。</p> </li> 
       <li> <p><b>[！UICONTROL模型清單]</b> </p> <p>選取或對應包含您要擷取之模型清單的工作區ID和模型ID。</p> </li> 
       <li> <p><b>[！UICONTROL模型行事曆]</b> </p> <p>選取或對應包含您要擷取之模型行事曆的工作區的ID。</p> </li> 
       <li> <p><b>模型版本</b> </p> </li> 
       <li> <p>選取或對應包含您要擷取之模型版本的模型ID [！UICONTROL ]。</p> </li> 
       <li> <p><b>[！UICONTROL使用者]</b> </p> </li> 
       <li> <p><b>[！UICONTROL檢視]</b> </p> <p>選取您要選擇「依模組」或「依模型」檢視，然後選取或對應包含您要擷取之檢視的「模組」或「模型」ID。</p> </li> 
      </ul> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL傳回工作區大小]</td> 
   <td>啟用此選項可傳回工作區目前大小的預估值。 此估計值是根據工作區中包含的所有模組大小而定。</td> 
  </tr> 
 </tbody> 
</table>
