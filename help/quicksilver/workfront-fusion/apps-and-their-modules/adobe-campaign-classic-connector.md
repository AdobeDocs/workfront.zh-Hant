---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 連接器
navigation-topic: apps-and-their-modules
title: Adobe Campaign Classic模組
description: 使用 [!DNL Adobe Campaign Classic] 模組，您可以啟動 [!DNL Adobe Workfront Fusion] 情境是根據您 [!DNL Adobe Campaign Classic] 帳戶、建立、讀取或更新協定和其他記錄、使用您設定的標準搜索記錄，以及上傳文檔。
author: Becky
feature: Workfront Fusion
exl-id: 84e8fa35-0c3c-46bd-8886-88c6d8d9e1d5
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1146'
ht-degree: 1%

---

# [!DNL Adobe Campaign Classic] 模組

使用 [!DNL Adobe Campaign Classic] 模組，您可以啟動 [!DNL Adobe Workfront Fusion] 情境是根據您 [!DNL Adobe Campaign Classic] 帳戶、建立、讀取或更新記錄、使用您設定的條件搜尋記錄，以及執行自訂API呼叫。

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Connect [!DNL Adobe Campaign Classic] to [!DNL Adobe Workfront Fusion]

1. 在任何 [!DNL Adobe Campaign Classic] 模組，按一下 **[!UICONTROL 新增]** 旁邊 [!UICONTROL 連線] 欄位。
1. 輸入您用來連線至 [!DNL Adobe Campaign Classic] 例項。
1. 輸入您的使用者名稱和密碼。
1. 按一下 **[!UICONTROL 繼續]** 若要建立連線，請返回模組。

## [!DNL Adobe Campaign Classic] 模組及其欄位

設定時 [!DNL Adobe Campaign Classic] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!DNL Adobe Campaign Classic] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [觸發器](#triggers)
* [動作](#actions)
* [搜尋](#searches)

### 觸發器

#### [!UICONTROL 監看記錄]

此已排程觸發模組會在記錄變更時啟動案例。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td>有關建立連接的說明 [!DNL Adobe Campaign Classic]，請參閱 <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >建立連線至 [!DNL Adobe Campaign Classic]</a> 這篇文章。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL篩選器]</td> 
   <td>選擇您要監視新記錄、更新記錄還是兩者。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資源]</td> 
   <td>選取您要監看的資源。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL要包含在輸出中的欄位]</td> 
   <td>選取您要納入模組輸出的欄位。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL要包含在輸出中的自定義欄位]</td> 
   <td>對於要包含在輸出中的每個自訂欄位，按一下 <b>[!UICONTROL添加]</b> 並輸入自訂欄位的名稱。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL返回結果的最大數]</td> 
   <td>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</td> 
  </tr> 
 </tbody> 
</table>


### 動作

* [[!UICONTROL 建立記錄]](#create-a-record)
* [[!UICONTROL 進行自訂API呼叫]](#make-a-custom-api-call)
* [[!UICONTROL 刪除記錄]](#delete-record)
* [[!UICONTROL 執行動作]](#perform-an-action)
* [[!UICONTROL 讀取記錄]](#-read-a-record)
* [[!UICONTROL 訂閱或取消訂閱]](#subscribe-or-unsubscribe)
* [[!UICONTROL 更新記錄]](#update-record)

#### [!UICONTROL 建立記錄]

此動作模組會在 [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td>
   <td>有關建立連接的說明 [!DNL Adobe Campaign Classic]，請參閱 <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >建立連線至 [!DNL Adobe Campaign Classic]</a> 這篇文章。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資源]</td> 
   <td>選取 [!DNL Adobe Campaign Classic] 記錄。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL欄位] </td> 
   <td>選擇建立記錄時要為其設定值的欄位，然後填寫這些欄位的值。 欄位會根據您選取的記錄類型而有所不同。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL自定義欄位]</td> 
   <td> 針對您要新增至新記錄的每個自訂欄位，按一下 <b>[!UICONTROL添加項]</b> 並輸入或映射欄位的名稱和值。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 進行自訂API呼叫]

此模組會對 [!DNL Adobe Campaign Classic] API

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL連接]</td>
   <td>有關建立連接的說明 [!DNL Adobe Campaign Classic]，請參閱 <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >建立連線至 [!DNL Adobe Campaign Classic]</a> 這篇文章。</td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL操作]</td>
      <td><p>選取您要API呼叫執行的動作。</p>
      <p>[!UICONTROL執行查詢]</p>
      <p>[!UICONTROL寫入]</p>
      <p>[!UICONTROL獲取實體（如果最近）]</p>
      <p>[!UICONTROL選擇全部]</p>
      <p>[!UICONTROL推送事件]</p>
    </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL標題]</td>
      <td>
        <p>以標準JSON物件的形式新增請求的標題。</p>
        <p>例如， <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] 自動新增[!UICONTROL x-security]代號標頭。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL XML主體]</td>
   <td> <p>在XML中新增API呼叫的內文內容，不含工作階段元素。 </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL 刪除記錄]

此動作模組會從 [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td>
   <td>有關建立連接的說明 [!DNL Adobe Campaign Classic]，請參閱 <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >建立連線至 [!DNL Adobe Campaign Classic]</a> 這篇文章。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資源]</td> 
   <td>選擇要刪除的資源類型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>輸入或對應您要刪除之資源的ID。</td> 
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL 執行動作]

此動作模組會對 [!DNL Adobe Campaign Classic] API。

如需特定動作和欄位的詳細資訊，請參閱 [[!DNL Adobe Campaign] - API檔案](https://experienceleague.adobe.com/developer/campaign-api/api/p-14.html).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td>
   <td>有關建立連接的說明 [!DNL Adobe Campaign Classic]，請參閱 <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >建立連線至 [!DNL Adobe Campaign Classic]</a> 這篇文章。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL操作]</td> 
   <td><p>選取要對物件執行的動作。</p>
   <ul>
   <li><p><b>[!DNL List]</b></p><p> 如需可用欄位，請參閱 <a href="#search" class="MCXref xref" >[!UICONTROL搜索]</a> 這篇文章。 </p></li>
     <li><p><b>[!UICONTROL Get]</b></p><p> 如需可用欄位，請參閱 <a href="#search" class="MCXref xref" >[!UICONTROL搜索]</a> 這篇文章。 </p></li> 
   <li><p><b>[!UICONTROL建立]</b></p><p> 如需可用欄位，請參閱 <a href="#create-a-record" class="MCXref xref" >[!UICONTROL建立記錄]</a> 這篇文章。 </p></li>
   <li><p><b>[!UICONTROL更新]</b></p><p> 如需可用欄位，請參閱 <a href="#update-record" class="MCXref xref" >[!UICONTROL更新記錄]</a> 這篇文章。 </p></li>
   <li><p><b>[!UICONTROL刪除]</b></p><p> 如需可用欄位，請參閱 <a href="#delete-record" class="MCXref xref" >[!UICONTROL刪除記錄]</a> 這篇文章。 </p></li>
   </ul>
   </td>
</tr> 
 </tbody> 
</table>

#### [!UICONTROL 讀取記錄]

此動作模組會從 [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td>
   <td>有關建立連接的說明 [!DNL Adobe Campaign Classic]，請參閱 <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >建立連線至 [!DNL Adobe Campaign Classic]</a> 這篇文章。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資源]</td> 
   <td>選取 [!DNL Adobe Campaign Classic] 記錄你想讀的。</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL ID] </td> 
   <td>輸入要讀取的記錄的ID。</td> 
  </tr> 
 <tr> 
   <td role="rowheader">[!UICONTROL要包含在輸出中的欄位] </td> 
   <td>選取您要納入模組輸出的欄位。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL要包含在輸出中的自定義欄位]</td> 
   <td>對於要包含在輸出中的每個自訂欄位，按一下 <b>[!UICONTROL添加]</b> 並輸入自訂欄位的名稱。</td> 
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL 訂閱或取消訂閱]

此動作模組會將使用者訂閱或取消訂閱資訊服務的使用者。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td>
   <td>有關建立連接的說明 [!DNL Adobe Campaign Classic]，請參閱 <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >建立連線至 [!DNL Adobe Campaign Classic]</a> 這篇文章。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL訂閱或取消訂閱]</td> 
   <td>選擇要訂閱還是取消訂閱資訊服務。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL服務名]</td> 
   <td>選擇要訂閱或取消訂閱的服務。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL收件人電子郵件地址] </td> 
   <td>輸入或映射您要訂閱或取消訂閱資訊服務的用戶的電子郵件地址。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新記錄]

此動作模組會更新 [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td>
   <td>有關建立連接的說明 [!DNL Adobe Campaign Classic]，請參閱 <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >建立連線至 [!DNL Adobe Campaign Classic]</a> 這篇文章。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資源]</td> 
   <td>選取 [!DNL Adobe Campaign Classic] 記錄。</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL ID] </td> 
   <td>輸入要更新的記錄ID的映射。</td> 
  </tr> 
<tr> 
   <td role="rowheader">[!UICONTROL欄位] </td> 
   <td>選取您要更新值的欄位，然後填寫這些欄位的值。 欄位會根據您選取的記錄類型而有所不同。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL自定義欄位]</td> 
   <td> 針對您要更新的每個自訂欄位，按一下 <b>[!UICONTROL添加項]</b> 並輸入或映射欄位的名稱和值。 </td> 
  </tr> 
 </tbody> 
</table>

### 搜尋

#### [!UICONTROL 搜尋]

此搜尋模組會根據指定的條件傳回記錄。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td>
   <td>有關建立連接的說明 [!DNL Adobe Campaign Classic]，請參閱 <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >建立連線至 [!DNL Adobe Campaign Classic]</a> 這篇文章。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資源]</td> 
   <td>選取 [!DNL Adobe Campaign Classic] 記錄。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制] </td> 
   <td>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</td> 
  </tr> 
 </tbody> 
</table>
