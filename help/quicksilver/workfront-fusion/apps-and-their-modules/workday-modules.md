---
filename: workday-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 連接器
navigation-topic: apps-and-their-modules
title: Workday模組
description: 在Adobe Workfront Fusion案例中，您可以自動執行使用 [!DNL Workday]，並將其連接至多個協力廠商應用程式和服務。
author: Becky
exl-id: 535573e0-b6ad-43a2-b7cb-ed32d1dc8d16
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '965'
ht-degree: 1%

---

# [!DNL Workday] 模組

在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!DNL Workday]，並將其連接至多個協力廠商應用程式和服務。

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

若要使用 [!DNL Workday] 模組，您必須：

* 有 [!DNL Workday] 帳戶。

* 在 [!DNL Workday]. 如需指示，請參閱 [!DNL Workday] 檔案。

## Connect [!DNL Workday] to [!DNL Workfront Fusion]

1. 在任何 [!DNL Workfront Fusion] 模組，按一下 [!UICONTROL 新增] 旁邊 [!UICONTROL 連線] 欄位

2. 填寫下列欄位：

   <table style="table-layout:auto"> 
        <col/>
        <col/>
        <tbody>
            <tr>
                <td role="rowheader">
                    <p role="rowheader">[!UICONTROL連接名]</p>
                </td>
                <td>輸入連接的名稱</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Workday主機]</td>
                <td>輸入 [!DNL Workday] 主機無 <code>https://</code>. 例如： <code>mycompany.workday.com</code>.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL服務URL]</td>
                <td>輸入 [!DNL Workday] 網站服務 <code>https://</code>. 例如： <code>mycompany-services.workday.com</code>.</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL租戶名稱]</td>
                <td>輸入此的租用戶 [!DNL Workday] 帳戶。 您的租用戶是貴組織的識別碼，可在您用來登入Workday的URL中看到。 範例：地址 <code>https://www.myworkday.com/mycompany</code>，租用戶為 <code>mycompany</code>.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL客戶端ID]</td>
                <td>輸入 [!DNL Workday] 此連接使用的應用程式。 在中建立應用程式時，即可取得此資訊 [!DNL Workday].</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL客戶端密碼]</td>
                <td>輸入 [!DNL Workday] 此連接使用的應用程式。 在中建立應用程式時，即可取得此資訊 [!DNL Workday].</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL會話超時（分鐘）]</td>
                <td >輸入授權Token過期的分鐘數。</td>
            </tr>
        </tbody>
    </table>


3. 按一下 [!UICONTROL 繼續] 儲存連線並返回模組

## [!DNL Workday] 模組及其欄位

設定時 [!DNL Workday] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!DNL Workday] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [動作](#action)

* [搜尋](#search)


### 動作

* [[!UICONTROL 建立記錄]](#create-a-record)

* [[!UICONTROL 刪除記錄]](#delete-a-record)

* [[!UICONTROL 進行自訂API呼叫]](#make-a-custom-api-call)

* [[!UICONTROL 更新記錄]](#update-a-record)


#### [!UICONTROL 建立記錄]

此動作模組會在 [!DNL Workday].

<table style="table-layout:auto"> 
    <col/>
    <col/>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL連接]</td>
            <td>有關連接 [!DNL Workday] 帳戶至Workfront Fusion，請參閱 <a href="#Connect" class="MCXref xre[!DNL ]f" >Connect [!DNL Workday] to [!DNL Workfront Fusion]</a>.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL記錄類型]</td>
            <td>選擇要建立的記錄類型。</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td>輸入或映射要建立的記錄ID。</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL子資源ID]</td>
            <td >輸入或對應您要建立之子資源的ID。</td>
        </tr>
    </tbody>
</table>

#### [!UICONTROL 刪除記錄]

此動作模組會刪除 [!DNL Workday].

<table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL連接]</td>
            <td>有關連接 [!DNL Workday] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#Connect" class="MCXref xre[!DNL ]f" >Connect [!DNL Workday] to [!DNL Workfront Fusion]</a>.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL記錄類型]</td>
            <td>選擇要刪除的記錄類型。</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL特定記錄類型]</td>
            <td>選擇要刪除的特定記錄類型。 這些是根據您選擇的記錄類型而定。</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL子資源ID]</td>
            <td>輸入或對應您要刪除的子資源的ID。</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td >輸入或映射要刪除的記錄ID。</td>
        </tr>
    </tbody>
</table>


### [!UICONTROL 進行自訂API呼叫]

此動作模組可讓您對 [!DNL Workday] API。 這樣，您就可以建立資料流自動化，而另一個無法完成 [!DNL Workday] 模組。

設定此模組時，會顯示下列欄位。

模組會傳回狀態代碼，以及API呼叫的標題和內文。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Connection]</p> </td> 
            <td>有關連接 [!DNL Workday] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#Connect" class="MCXref xre[!DNL ]f" >Connect [!DNL Workday] to [!DNL Workfront Fusion]</a>.</td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>輸入相對於的路徑 <code style="color: #ff1493;">https://&lt;tenantHostname>/api/&lt;serviceName>/&lt;version>/&lt;tenant></code>.</td> 
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

#### [!UICONTROL 更新記錄]

此動作模組會更新 [!DNL Workday].

<table style="table-layout:auto"> 
    <col/>
    <col/>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL連接]</td>
            <td>有關連接 [!DNL Workday] 帳戶至Workfront Fusion，請參閱 <a href="#Connect" class="MCXref xref" >[!UICONTROL連接 [!DNL Workday] 到Workfront聚變]</a></td>
        </tr>
        <tr>
            <td  role="rowheader">記錄類型</td>
            <td>選擇要更新的記錄t[!UICONTROL ]的類型。</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td>輸入或映射要更新的記錄ID。</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL子資源ID]</td>
            <td >輸入或映射要更新的子資源的ID。</td>
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
            <td role="rowheader">[!UICONTROL連接]</td>
            <td>有關連接 [!DNL Workday] 帳戶至Workfront Fusion，請參閱 <a href="#Connect" class="MCXref xref" >[!UICONTROL連接 [!DNL Workday] 到Workfront聚變]</a></td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL記錄類型]</td>
            <td>選擇要刪除的記錄類型。</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL特定記錄類型]</td>
            <td>選擇要讀取的特定記錄類型。 這些是根據您選擇的記錄類型而定。</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td >輸入或映射要刪除的記錄ID。</td>
        </tr>
    </tbody>
</table>

#### [!UICONTROL 清單記錄]

此搜索模組檢索指定類型的記錄清單。

<table style="table-layout:auto"> 
      <col/>
      <col/>
      <tbody>
          <tr>
              <td role="rowheader">[!UICONTROL連接]</td>
              <td>有關連接 [!DNL Workday] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#Connect" class="MCXref xref" >Connect [!DNL Workday] to [!DNL Workfront Fusion]</a></td>
          </tr>
          <tr>
              <td  role="rowheader">[!UICONTROL記錄類型]</td>
              <td>選擇要檢索的記錄類型。</td>
          </tr>
          <tr>
              <td role="rowheader">[!UICONTROL限制]</td>
              <td >
                  <p>輸入或映射您希望模組在每個方案執行週期中檢索的最大記錄數。</p>
              </td>
          </tr>
      </tbody>
  </table>
