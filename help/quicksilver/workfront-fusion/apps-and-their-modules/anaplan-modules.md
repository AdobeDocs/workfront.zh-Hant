---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 連接器
navigation-topic: apps-and-their-modules
title: Anaplan模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用Anaplan的工作流程，並將其連接到多個第三方應用程式和服務。
author: Becky
feature: Workfront Fusion, Workfront Integrations and Apps
exl-id: 03bcd0a4-c8ec-4f44-b1e1-b57e79595309
source-git-commit: 8963acee01aac6117a731147d9288fddbe3e812f
workflow-type: tm+mt
source-wordcount: '1796'
ht-degree: 1%

---

# [!DNL Anaplan] 模組

在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!DNL Anaplan]，並將其連接至多個協力廠商應用程式和服務。

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

您可以使用 [!DNL Anaplan] 連接器，您必須確保符合下列必要條件：

* 您必須具有活動 [!UICONTROL 阿納普蘭] 帳戶。
* 必須配置工作區、模型和其他 [!DNL Anaplan] 對象 [!UICONTROL 阿納普蘭] 帳戶之前 [!DNL Workfront Fusion] 能與他們互動。

## Connect [!DNL Anaplan] to [!DNL Workfront Fusion] {#connect-anaplan-to-workfront-fusion}

為 [!DNL Anaplan] 模組：

1. 按一下 **[!UICONTROL 新增]** 旁邊 [!UICONTROL 連線] 框。
1. 選擇連接類型。

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!DNL Anaplan] [!UICONTROL Basic]</td> 
      <td> <p>安 [!DNL Anaplan] [!UICONTROL Basic]連接僅需要電子郵件地址和密碼才能建立連接。 </p> <p>輸入連線的名稱，然後輸入您的電子郵件地址和密碼 [!DNL Anaplan] 帳戶。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Anaplan] [!UICONTROL CA證書]</td> 
      <td> <p>安 [!DNL Anaplan] [!UICONTROL CA Certificate]連接需要[!UICONTROL證書密鑰]、[!UICONTROL編碼資料]和[!UICONTROL編碼簽名資料]。 您可以在 [!DNL Anaplan] 帳戶。 如需指示，請參閱 [!DNL Anaplan] 檔案。</p> <p>輸入連線的名稱，然後輸入您在 [!DNL Anaplan] 帳戶。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **[!UICONTROL 繼續]** 以儲存連線並返回模組。

## [!DNL Anaplan] 模組及其欄位

設定時 [!DNL Anaplan] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!DNL Anaplan] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [觸發器](#triggers)
* [動作](#actions)
* [搜尋](#searches)

### 觸發器

#### [!DNL Watch records]

此觸發模組會在建立或更新所選類型的記錄時啟動案例。

>[!NOTE]
>
>此模組返回新記錄的資料。 它不會傳回已修改之現有記錄的資料。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td>有關建立連接的說明 [!DNL Anaplan]，請參閱 <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect [!DNL Anaplan] to [!DNL Workfront Fusion]</a> 這篇文章。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">要監視的對象類型</td> 
   <td>選擇要監視的項目類型。 當建立或更新此類型的記錄時，將開始情況。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">&lt;object&gt; ID</td> 
   <td>在Anaplan中輸入對象的ID，如與要監視的對象關聯的模型或模組</td> 
  </tr> 
  <tr> 
   <td role="rowheader">限制</td> 
   <td> <p>輸入或映射在每個方案執行週期中希望模組執行[action]的記錄數上限。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 動作

* [[!UICONTROL 建立清單項目]](#create-a-list-item)
* [[!UICONTROL 進行自訂API呼叫]](#make-a-custom-api-call)
* [[!UICONTROL 讀取記錄]](#read-a-record)
* [[!UICONTROL 執行動作]](#run-an-action)
* [[!UICONTROL 更新記錄]](#update-a-record)
* [[!UICONTROL 上傳檔案]](#upload-a-file)

#### [!UICONTROL 建立清單項目]

此操作模組將新項添加到Anaplan中的清單。

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL連接]</td>
        <td>有關建立連接的說明 [!DNL Anaplan]，請參閱 <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect [!DNL Anaplan] to [!DNL Workfront Fusion]</a> 這篇文章。</td>
    </tr>
    <tr>
        <td>[!UICONTROL Workspace ID]</td>
        <td>選擇或映射包含要添加項的清單的Anaplan Workspace的ID。</td>
    </tr>
    <tr>
        <td>[!UICONTROL模型ID]</td>
        <td>選擇或映射包含要添加項的清單的模型的ID。</td>
    </tr>
    <tr>
        <td>[!UICONTROL清單ID]</td>
        <td>選擇或映射要建立項的清單的ID。</td>
    </tr>
    <tr>
        <td>[!UICONTROL名稱]</td>
        <td>輸入新項的名稱。</td>
    </tr>
    <tr>
        <td>[!UICONTROL代碼]</td>
        <td>輸入新項的代碼。 代碼是用戶生成的代碼，使您能夠區分具有相同名稱的行項目。</td>
    </tr>
    <tr>
        <td>[!UICONTROL父級]</td>
        <td>輸入要在下建立新項的父項的名稱。</td>
    </tr>
    <tr>
        <td>[!UICONTROL屬性]</td>
        <td>如果要向其中添加項目的清單具有自定義屬性，請選擇要為其添加值的屬性，然後添加值。</td>
    </tr>
    <tr>
        <td>[!UICONTROL子集]</td>
        <td>如果要向中添加項的清單具有自定義子集，請選擇要向中添加項的子集，然後選擇 <b>[!UICONTROL是]</b> 將新項目新增至該子集。</td>
    </tr>
</table>

#### [!UICONTROL 進行自訂API呼叫]

此模組可讓您對 [!DNL Anaplan] API。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td>有關建立連接的說明 [!DNL Anaplan]，請參閱 <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect [!DNL Anaplan] to [!DNL Workfront Fusion]</a> 這篇文章。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>輸入相對於的路徑 <code>https://api.anaplan.com/2/0/</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL方法]</p> </td> 
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL標題]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標題。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 自動添加授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL查詢字串] </td> 
   <td> <p>輸入請求查詢字串。</p> </td> 
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

#### [!UICONTROL 刪除記錄]

此動作模組會刪除現有記錄。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td>有關建立連接的說明 [!DNL Anaplan]，請參閱 <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect [!DNL Anaplan] to [!DNL Workfront Fusion]</a> 這篇文章。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>選擇或映射包含要刪除的對象的Anaplan Workspace的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL模型ID]</td> 
   <td>輸入或映射包含要刪除的對象的模型的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">刪除</td> 
   <td> <p>選擇要刪除的對象類型。</p> 
    <ul> 
     <li> <p><b>動作</b> </p> <p>選取或對應要刪除的動作。</p> </li> 
     <li> <p><b>清單項目</b> </p> <p>選擇要刪除項的清單，然後輸入或映射要刪除的項的ID或代碼</p>  </li> 
     <li> <p><b>[!UICONTROL檔案]</b> </p> <p>選取或對應要刪除的檔案。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 讀取記錄]

此動作模組會讀取單一記錄。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td>有關建立連接的說明 [!DNL Anaplan]，請參閱 <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect [!DNL Anaplan] to [!DNL Workfront Fusion]</a> 這篇文章。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL記錄類型]</td> 
   <td> <p>選擇要讀取的記錄類型。</p> 
    <ul> 
     <li> <p><b>模型</b> </p> <p>選擇或映射要讀取的模型的ID</p> </li> 
     <li> <p><b>模型清單</b> </p> <p>選擇或映射包含要讀取的清單的工作區和模型的ID，然後選擇清單。 在[!UICONTROL資料類型]欄位中，選擇您要讀取資料還是元資料。</p> </li> 
     <li> <p><b>模型版本</b> </p> <p>選擇或映射要讀取的模型的ID。</p> </li> 
     <li> <p><b>使用者</b> </p> <p>選取您要傳回所使用帳戶擁有者的相關資料，還是其他使用者。 如果您選取其他使用者，請選取使用者的名稱。</p> </li> 
     <li> <p><b>工作區</b> </p> <p>選取或對應您要讀取之工作區的ID。</p> </li> 
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
        <td role="rowheader">[!UICONTROL連接]</td>
        <td>有關建立連接的說明 [!DNL Anaplan]，請參閱 <a href="#Connect" class="MCXref xref" >[!UICONTROL將Anaplan連接到Workfront Fusion]</a> 這篇文章。</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Workspace ID]</td>
        <td>選取或對應 [!DNL Anaplan] 您要執行動作的工作區</td>
      </tr>
      <tr >
        <td role="rowheader">[!UICONTROL模型ID]</td>
        <td>選擇或映射要執行操作的模型的ID。</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL操作類型]</td>
        <td>
          <p>選取要執行的動作</p>
            <ul>
              <li>
                <p><b>[!UICONTROL刪除]</b>
                </p>
                <p>輸入或對應您要刪除之動作的ID。</p>
              </li>
              <li>
                <p><b>[!UICONTROL導出]</b>
                </p>
                <p>輸入或映射要使用的導出定義的ID。 您可以匯出為下列檔案格式：</p>
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
                  <p><b>[!UICONTROL匯入] </b>
                  </p>
                  <p style="font-weight: normal;">輸入或映射要使用的導入定義的ID。</p>
                </li>
                <li>
                 <p><b>[!UICONTROL進程]</b>
                 </p>
                  <p>輸入或映射要使用的流程的ID。 </p>
                </li>
              </ul>
            </td>
          </tr>
        </tbody>
      </table>


#### [!UICONTROL 更新記錄]

此動作模組會更新 [!UICONTROL 阿納普蘭].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td>有關建立連接的說明 [!DNL Anaplan]，請參閱 <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect [!DNL Anaplan] to [!DNL Workfront Fusion]</a> 這篇文章。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL記錄類型]</td> 
   <td> <p>選擇要更新的記錄類型。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL清單項]</b> </p> <p>如需欄位，請參閱 <a href="#create-a-list-item" class="MCXref xref">建立清單項目</a> 這篇文章。</p> </li> 
     <li> <p><b>[!UICONTROL模組單元格資料]</b> </p> <p>更新儲存格資料時，所有使用該資料的下游計算也會更新。</p> <p>填寫下列欄位：</p> 
      <ul> 
       <li> <p><b>[!UICONTROL模型ID]</b> </p> <p>選擇或映射包含要更新的單元格的模型。</p> </li> 
       <li> <p><b>[!UICONTROL模組ID]</b> </p> <p>選擇或映射包含要更新的單元格的模組</p> </li> 
       <li> <p><b>[!UICONTROL行項目名]</b> </p> <p>選擇或映射要更新的單元格的行項</p> </li> 
       <li> <p style="font-weight: bold;">[!UICONTROLDimensionID]</p> <p>選取或對應行項目上的維度。</p> 
       <p><b>備註: </b> 
       <ul>
       <li> Dimension鍵（值）必須是 <code>dimensionName</code> （下一個）或 <code>dimensionId</code> (ID)。</li>
       <li>項目鍵（值）必須 <code>itemName</code> （文本）, <code>itemCode</code> （文字），或 <code>itemId</code> (ID)。</li>
       <li>Dimension和項目索引鍵必須是相同的類型（文字或ID）。
       </ul>
        </p> 
        <p>如需維度的相關資訊，請在 [!DNL Anaplan Anapedia].</p> </li> 
       <li> <p><b>[!UICONTROL值]</b> </p> <p>輸入或映射儲存格的新值。</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL當前會計年度模型]</b> </p> <p>輸入要更新會計年度的模型的工作區ID和模型ID，然後輸入或映射模型的新年度。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 上傳檔案]

此操作模組將檔案上載到Anaplan。 檔案必須已上載到Anaplan。 您可以使用此模組將其上傳至Anaplan內的其他位置。
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">[!UICONTROL連接]</td>
<td>有關建立連接的說明 [!DNL Anaplan]，請參閱 <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect [!DNL Anaplan] to [!DNL Workfront Fusion]</a> 這篇文章。</td>
</tr>
<tr>
<td role="rowheader">[!UICONTROL Workspace ID]</td>
<td>選取或對應 [!DNL Anaplan] 上傳檔案的工作區。</td>
</tr>
<tr>
<td role="rowheader">[!UICONTROL模型ID]</td>
<td>選擇或映射要上載檔案的模型的ID。</td>
</tr>
<tr>
<td role="rowheader">[!UICONTROL檔案ID]</td>
<td>選取或對應您要上傳之檔案的ID。</td>
</tr>
</tbody>
</table>
</div>

### 搜尋

#### [!UICONTROL 獲取記錄]

此搜索模組返回所選類型的所有可訪問記錄。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td>有關建立連接的說明 [!DNL Anaplan]，請參閱 <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect [!DNL Anaplan] to [!DNL Workfront Fusion]</a> 這篇文章。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL記錄類型]</td> 
   <td> <p>選擇要檢索的記錄類型。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL工作區]</b> </p> </li> 
       <li> <p><b>[!UICONTROL模型]</b> </p> </li> 
       <li> <p><b>[!UICONTROL行項]</b> </p> <p>選擇或映射包含 [!DNL line] 要檢索的項目。</p> </li> 
       <li> <p><b>[!UICONTROL模型清單]</b> </p> <p>選擇或映射包含要檢索的模型清單的工作區和模型ID的ID。</p> </li> 
       <li> <p><b>[!UICONTROL模型日曆]</b> </p> <p>選擇或映射包含要檢索的模型日曆的工作區的ID。</p> </li> 
       <li> <p><b>模型版本</b> </p> </li> 
       <li> <p>選擇或映射[!UICONTROL ]包含要檢索的模型版本的模型的ID。</p> </li> 
       <li> <p><b>[!UICONTROL用戶]</b> </p> </li> 
       <li> <p><b>[!UICONTROL視圖]</b> </p> <p>選擇要按模組還是按模型選擇視圖，然後選擇或映射包含要檢索的視圖的模組或模型的ID。</p> </li> 
      </ul> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL返回工作區大小]</td> 
   <td>啟用此選項可傳回工作區目前大小的預估值。 此預估是根據工作區中所包含所有模組的大小。</td> 
  </tr> 
 </tbody> 
</table>
