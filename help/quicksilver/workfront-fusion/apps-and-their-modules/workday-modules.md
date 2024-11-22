---
filename: workday-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Workday模組
description: 在Adobe Workfront Fusion案例中，您可以自動化使用 [!DNL Workday]的工作流程，並將其連線至多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: 535573e0-b6ad-43a2-b7cb-ed32d1dc8d16
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '1030'
ht-degree: 1%

---

# [!DNL Workday]模組

在[!DNL Adobe Workfront Fusion]案例中，您可以自動化使用[!DNL Workday]的工作流程，並將其連線至多個協力廠商應用程式和服務。

如果您需要有關建立案例的指示，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md)中建立案例。

如需模組的相關資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md)中的[模組。

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

## 先決條件

若要使用[!DNL Workday]模組，您必須：

* 擁有[!DNL Workday]帳戶。

* 在[!DNL Workday]中建立OAuth應用程式。 如需指示，請參閱[!DNL Workday]檔案。

## Workday API資訊

Workday聯結器會使用以下專案：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">基礎URL</td> 
   <td>https://&lbrace;&lbrace;connection.servicesUrl&rbrace;&rbrace;/api</td> 
  </tr>
  <tr> 
   <td role="rowheader">API標籤</td> 
   <td>v1.6.4</td> 
  </tr>
 </tbody> 
 </table>

## 將[!DNL Workday]連線至[!DNL Workfront Fusion]

1. 在任何[!DNL Workfront Fusion]模組中，按一下[!UICONTROL 連線]欄位旁的[!UICONTROL 新增]

2. 填寫下列欄位：

   <table style="table-layout:auto"> 
        <col/>
        <col/>
        <tbody>
            <tr>
                <td role="rowheader">
                    <p role="rowheader">[！UICONTROL連線名稱]</p>
                </td>
                <td>輸入連線的名稱</td>
            </tr>
            <tr>
                <td  role="rowheader">[！UICONTROL Workday主機]</td>
                <td>輸入不含<code>https://</code>的[!DNL Workday]主機位址。 例如： <code>mycompany.workday.com</code>。</td>
            </tr>
            <tr>
                <td role="rowheader">[！UICONTROL服務URL]</td>
                <td>輸入您的[!DNL Workday]網路服務位址（不含<code>https://</code>）。 例如： <code>mycompany-services.workday.com</code>。</td>
            </tr>
            <tr>
                <td  role="rowheader">[！UICONTROL租使用者名稱稱]</td>
                <td>輸入此[!DNL Workday]帳戶的租使用者。 您的租使用者是您組織的識別碼，可在您用來登入Workday的URL中看見。 範例：在地址<code>https://www.myworkday.com/mycompany</code>中，租使用者是<code>mycompany</code>。</td>
            </tr>
            <tr>
                <td role="rowheader">[！UICONTROL使用者端ID]</td>
                <td>輸入此連線使用的[!DNL Workday]應用程式的使用者端識別碼。 當您在[!DNL Workday]中建立應用程式時，就會取得此資訊。</td>
            </tr>
            <tr>
                <td  role="rowheader">[！UICONTROL使用者端密碼]</td>
                <td>輸入此連線使用的[!DNL Workday]應用程式的使用者端密碼。 當您在[!DNL Workday]中建立應用程式時，就會取得此資訊。</td>
            </tr>
            <tr>
                <td role="rowheader">[！UICONTROL工作階段逾時（分鐘）]</td>
                <td >輸入您的授權Token過期的分鐘數。</td>
            </tr>
        </tbody>
    </table>


3. 按一下[!UICONTROL 繼續]以儲存連線並返回模組

## [!DNL Workday]模組及其欄位

當您設定[!DNL Workday]模組時，[!DNL Workfront Fusion]會顯示下列欄位。 除了這些欄位以外，可能還會顯示其他[!DNL Workday]欄位，視您在應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中將資訊從一個模組對應到另一個模組。

![](assets/map-toggle-350x74.png)

* [動作](#action)

* [搜尋](#search)


### 動作

* [[!UICONTROL 建立記錄]](#create-a-record)

* [[!UICONTROL 刪除記錄]](#delete-a-record)

* [[!UICONTROL 進行自訂API呼叫]](#make-a-custom-api-call)

* [[!UICONTROL 更新記錄]](#update-a-record)


#### [!UICONTROL 建立記錄]

此動作模組會在[!DNL Workday]中建立單一記錄。

<table style="table-layout:auto"> 
    <col/>
    <col/>
    <tbody>
        <tr>
            <td role="rowheader">[！UICONTROL Connection]</td>
            <td>如需有關將您的[!DNL Workday]帳戶連線到Workfront Fusion的說明，請參閱<a href="#Connect" class="MCXref xre[!DNL ]f" >將[!DNL Workday]連線到[!DNL Workfront Fusion]</a>。</td>
        </tr>
        <tr>
            <td  role="rowheader">[！UICONTROL記錄型別]</td>
            <td>選取您要建立的記錄型別。</td>
        </tr>
        <tr>
            <td role="rowheader">[！UICONTROL ID] </td>
            <td>輸入或對應您要建立的記錄ID。</td>
        </tr>
        <tr>
            <td role="rowheader">[！UICONTROL子資源ID]</td>
            <td >輸入或對應您要建立之子資源的ID。</td>
        </tr>
    </tbody>
</table>

#### [!UICONTROL 刪除記錄]

此動作模組會刪除[!DNL Workday]中的單一記錄。

<table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
        <tr>
            <td role="rowheader">[！UICONTROL Connection]</td>
            <td>如需有關將您的[!DNL Workday]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="#Connect" class="MCXref xre[!DNL ]f" >將[!DNL Workday]連線到[!DNL Workfront Fusion]</a>。</td>
        </tr>
        <tr>
            <td  role="rowheader">[！UICONTROL記錄型別]</td>
            <td>選取您要刪除的記錄型別。</td>
        </tr>
        <tr>
            <td role="rowheader">[！UICONTROL特定記錄型別]</td>
            <td>選取您要刪除的特定記錄型別。 這些是以您選擇的記錄型別為基礎。</td>
        </tr>
        <tr>
            <td  role="rowheader">[！UICONTROL子資源ID]</td>
            <td>輸入或對應您要刪除之子資源的ID。</td>
        </tr>
        <tr>
            <td role="rowheader">[！UICONTROL ID] </td>
            <td >輸入或對應您要刪除之記錄的ID。</td>
        </tr>
    </tbody>
</table>


### [!UICONTROL 進行自訂API呼叫]

此動作模組可讓您對[!DNL Workday] API進行自訂的已驗證呼叫。 如此一來，您就可以建立其他[!DNL Workday]模組無法完成的資料流程自動化。

當您設定此模組時，會顯示下列欄位。

模組會傳回a狀態代碼，以及API呼叫的標題和正文。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Connection]</p> </td> 
            <td>如需有關將您的[!DNL Workday]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="#Connect" class="MCXref xre[!DNL ]f" >將[!DNL Workday]連線到[!DNL Workfront Fusion]</a>。</td>
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL URL]</td> 
   <td>輸入相對於<code style="color: #ff1493;">https://&lt;tenantHostname>/api/&lt;serviceName>/&lt;version>/&lt;tenant></code>的路徑。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL方法]</td> 
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP要求方法。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標頭。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>[！UICONTROL Workfront Fusion]會為您新增授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查詢字串]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的查詢。</p> <p>例如： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Body]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的內文內容。</p> <p>注意：  <p>在JSON中使用條件陳述式（例如<code>if</code>）時，請將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新記錄]

此動作模組更新[!DNL Workday]中的單一記錄。

<table style="table-layout:auto"> 
    <col/>
    <col/>
    <tbody>
        <tr>
            <td role="rowheader">[！UICONTROL Connection]</td>
            <td>如需有關將您的[!DNL Workday]帳戶連線到Workfront Fusion的說明，請參閱<a href="#Connect" class="MCXref xref" >[！UICONTROL連線[!DNL Workday]到Workfront Fusion]</a></td>
        </tr>
        <tr>
            <td  role="rowheader">記錄類型</td>
            <td>選取您要更新的記錄型別t[！UICONTROL ]。</td>
        </tr>
        <tr>
            <td role="rowheader">[！UICONTROL ID] </td>
            <td>輸入或對應您要更新的記錄ID。</td>
        </tr>
        <tr>
            <td role="rowheader">[！UICONTROL子資源ID]</td>
            <td >輸入或對應您要更新的子資源ID。</td>
        </tr>
    </tbody>
</table>

### 搜尋

* [[!UICONTROL 讀取記錄]](#read-a-record)

* [[!UICONTROL 清單記錄]](#list-records)


#### [!UICONTROL 讀取記錄]

此動作模組會讀取單一記錄。

<table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
        <tr>
            <td role="rowheader">[！UICONTROL Connection]</td>
            <td>如需有關將您的[!DNL Workday]帳戶連線到Workfront Fusion的說明，請參閱<a href="#Connect" class="MCXref xref" >[！UICONTROL連線[!DNL Workday]到Workfront Fusion]</a></td>
        </tr>
        <tr>
            <td  role="rowheader">[！UICONTROL記錄型別]</td>
            <td>選取您要刪除的記錄型別。</td>
        </tr>
        <tr>
            <td role="rowheader">[！UICONTROL特定記錄型別]</td>
            <td>選取您要讀取的特定記錄型別。 這些是以您選擇的記錄型別為基礎。</td>
        </tr>
        <tr>
            <td role="rowheader">[！UICONTROL ID] </td>
            <td >輸入或對應您要刪除之記錄的ID。</td>
        </tr>
    </tbody>
</table>

#### [!UICONTROL 清單記錄]

此搜尋模組會擷取指定型別的記錄清單。

<table style="table-layout:auto"> 
      <col/>
      <col/>
      <tbody>
          <tr>
              <td role="rowheader">[！UICONTROL Connection]</td>
              <td>如需有關將您的[!DNL Workday]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱<a href="#Connect" class="MCXref xref" >將[!DNL Workday]連線到[!DNL Workfront Fusion]</a></td>
          </tr>
          <tr>
              <td  role="rowheader">[！UICONTROL記錄型別]</td>
              <td>選取您要擷取的記錄型別。</td>
          </tr>
          <tr>
              <td role="rowheader">[！UICONTROL限制]</td>
              <td >
                  <p>輸入或對應您希望模組在每個案例執行週期中擷取的記錄數上限。</p>
              </td>
          </tr>
      </tbody>
  </table>
