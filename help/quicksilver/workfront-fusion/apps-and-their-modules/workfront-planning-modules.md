---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Adobe Workfront規劃模組
description: 使用 [!DNL Adobe Workfront Planning] 模組，您可以啟動 [!DNL Adobe Workfront Fusion] 根據您設定之事件的案例 [!DNL Adobe] Workfront Planning帳戶、建立、讀取或更新協定與其他記錄、使用您設定的條件搜尋記錄，以及上傳檔案。
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
exl-id: 892fdaf3-935e-4e66-a01c-9e9b6e0daf3e
source-git-commit: e067c5ff34c31060ca6fd392289d845f53a5ef3a
workflow-type: tm+mt
source-wordcount: '1116'
ht-degree: 0%

---

# [!DNL Adobe Workfront Planning] 模組

使用 [!DNL Adobe Workfront Planning] 模組，則可於Workfront Planning中發生事件時觸發情境。 您也可以建立、讀取、更新和刪除記錄，或執行自訂API呼叫至 [!DNL Adobe Workfront Planning] 帳戶。

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
   <p>目前授權需求：否 [!DNL Workfront Fusion] 授權需求。</p>
   <p>或</p>
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] 適用於工作自動化與整合] </p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 計畫，您的組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述的功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 計畫。</p>
   <p>或</p>
   <p>舊版產品需求：貴組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

有關的資訊 [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 建立與的連線 [!DNL Adobe Workfront Planning]

您可以建立與您的電腦的連線， [!DNL Workfront Planning] 直接從a內的帳戶 [!DNL Workfront Fusion] 模組。

1. 在任何 [!DNL Workfront Planning] 應用程式模組，按一下 **[!UICONTROL 新增]** 在 [!UICONTROL 連線] 方塊。
1. 輸入此連線的名稱。
1. 選取您要連線至生產環境或非生產環境。
1. 選取您要連線到服務帳戶還是個人帳戶。
1. 按一下 **[!UICONTROL SAML登入]** 以建立連線並返回模組。

## [!DNL Adobe Workfront Planning] 模組及其欄位

### 觀看活動

在Workfront Planning中建立、更新或刪除記錄、記錄型別或工作區時，此觸發模組會啟動案例。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Webhook]</td>
      <td>選取您要使用的webhook，或按一下「新增」以建立新的webhook。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有關建立與的連線的指示 [!DNL Adobe Workfront Planning]，請參閱 <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >建立與的連線 [!DNL Adobe Workfront Planning]</a> 本文章內容。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL物件型別]</td>
      <td>選取您要監視記錄、記錄型別或工作區。</td>
    </tr>
     <tr data-mc-conditions=""> 
      <td> <p>[！UICONTROL事件篩選器]</p> </td> 
      <td> <p>您可以設定篩選器，只監視符合您選取條件的記錄。</p> <p>針對每個篩選器，輸入您希望篩選器評估的欄位、運運算元，以及您希望篩選器允許的值。 您可以新增AND規則來使用一個以上的篩選器。</p> <p>附註：您無法編輯現有篩選器中的 [!DNL Workfront] webhook。 若要為設定不同的篩選器 [!DNL Workfront] 事件訂閱，移除目前的webhook並建立新的訂閱。</p> <p>如需事件篩選器的詳細資訊，請參閱 <a href="/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-modules.md#event-subscription-filters-in-the-workfront--watch-events-modules" class="MCXref xref">中的事件訂閱篩選器 [!DNL Workfront] &gt; [！UICONTROL觀看活動]模組</a> 在Workfront模組文章中。</p> </td> 
     </tr> 
    <tr>
      <td role="rowheader">要觀看的[！UICONTROL物件]</td>
      <td>選取是否要監視新專案。 更新、新增和更新或刪除的記錄。</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[！UICONTROL排除此連線所做的更新]</p>
      </td>
      <td>啟用此選項可防止此模組使用的連線進行變更時觸發此案例。 如此可防止在此案例執行觸發動作時觸發另一個案例例項。</td> 
      </tr>
  </tbody>
</table>

### 刪除記錄型別

此動作模組會依據其ID刪除Workfront Planning中的單一記錄型別。

>[!WARNING]
>
>刪除Workfront Planning中的記錄型別也會刪除記錄型別表格中的所有記錄。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有關建立與的連線的指示 [!DNL Adobe Workfront Planning]，請參閱 <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >建立與的連線 [!DNL Adobe Workfront Planning]</a> 本文章內容。</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[！UICONTROL記錄型別ID]</p>
      </td>
      <td>輸入或對應您要刪除之欄位的ID。</td> 
      </tr>
  </tbody>
</table>

### 進行自訂API呼叫

此模組會對 [!DNL Adobe Workfront Planning] API。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有關建立與的連線的指示 [!DNL Adobe Workfront Planning]，請參閱 <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >建立與的連線 [!DNL Adobe Workfront Planning]</a> 本文章內容。</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[！UICONTROL路徑]</p>
      </td>
      <td>
        <p>輸入相對於https://&lt;WORKFRONT_DOMAIN&gt;/attask/api/&lt;API_VERSION&gt;/的路徑</p>
      </td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[！UICONTROL API版本]</p>
      </td>
      <td>
        <p>選取您要使用的API版本。 如果您未選取版本，則預設會使用最新版本。</p>
      </td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[！UICONTROL API路徑覆寫]</p>
      </td>
      <td>
        <p>輸入相對於https://&lt;WORKFRONT_DOMAIN&gt;/attask/api/&lt;API_VERSION&gt;/的路徑</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL方法]</p>
      </td>
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Headers]</td>
      <td>
        <p>以標準JSON物件的形式新增請求的標頭。</p>
        <p>例如， <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] 自動新增授權標頭。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL查詢字串]  </td>
      <td>
        <p>對於每個要新增至查詢字串的索引鍵/值組，按一下 <b>新增專案</b> 並輸入索引鍵和值。</p>
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

<!--

### Delete a field

This action module deletes a single field in Workfront Planning by its ID.

>[!WARNING]
>
>Deleting a field in Workfront Planning deletes it and any data in it from every object of that record type in Workfront Planning.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Workfront Planning], see <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Create a connection to [!DNL Adobe Workfront Planning]</a> in this article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Field ID]</p>
      </td>
      <td>Enter or map the ID of the record type you want to delete.</td> 
      </tr>
  </tbody>
</table>

### Get a field 


This action module retrieves a single field in Workfront Planning by its ID.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Workfront Planning], see <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Create a connection to [!DNL Adobe Workfront Planning]</a> in this article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Field ID]</p>
      </td>
      <td>Enter or map the ID of the field you want to delete.</td> 
      </tr>
  </tbody>
</table>

-->

### 建立記錄

這個動作會在Workfront Planning中建立單一記錄。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有關建立與的連線的指示 [!DNL Adobe Workfront Planning]，請參閱 <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >建立與的連線 [!DNL Adobe Workfront Planning]</a> 本文章內容。</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[！UICONTROL記錄型別ID]</p>
      </td>
      <td>輸入或對應您要建立的記錄型別。 可用的記錄型別取決於您的Workfront Planning帳戶。</td> 
      </tr>
     <tr>
      <td role="rowheader">
        <p>其他欄位</p>
      </td>
      <td>這些欄位是根據您選取的記錄型別。</td> 
      </tr>
     <tr>
  </tbody>
</table>

### 刪除記錄

此動作模組會刪除Workfront Planning中的指定記錄。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有關建立與的連線的指示 [!DNL Adobe Workfront Planning]，請參閱 <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >建立與的連線 [!DNL Adobe Workfront Planning]</a> 本文章內容。</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[！UICONTROL記錄ID]</p>
      </td>
      <td>輸入或對應您要刪除之記錄的ID。</td> 
      </tr>
  </tbody>
</table>

<!--

### Get all records

This action module retrieves all records from an [!DNL Adobe Workfront Planning] account.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Workfront Planning], see <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Create a connection to [!DNL Adobe Workfront Planning]</a> in this article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Maximum number of returned records]</p>
      </td>
      <td>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</td> 
      </tr>
  </tbody>
</table>

-->

### 取得記錄

此動作模組會從擷取單一記錄 [!DNL Adobe Workfront Planning]，以其ID指定。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有關建立與的連線的指示 [!DNL Adobe Workfront Planning]，請參閱 <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >建立與的連線 [!DNL Adobe Workfront Planning]</a> 本文章內容。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL記錄ID]</td>
      <td>輸入或對應您要擷取之記錄的ID。</td>
    </tr>
  </tbody>
</table>

### 依記錄型別取得記錄

此動作模組會擷取指定型別的所有記錄。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有關建立與的連線的指示 [!DNL Adobe Workfront Planning]，請參閱 <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >建立與的連線 [!DNL Adobe Workfront Planning]</a> 本文章內容。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Workspace]</td>
      <td>選取或對映包含您要擷取之記錄的工作區。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL記錄型別]</td>
      <td>選取您要擷取的記錄型別。</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[！UICONTROL傳回記錄的最大數量]</p>
      </td>
      <td>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</td> 
  </tbody>
</table>

### 取得記錄型別

此動作模組會擷取 [!DNL Adobe Workfront Planning] 帳戶。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有關建立與的連線的指示 [!DNL Adobe Workfront Planning]，請參閱 <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >建立與的連線 [!DNL Adobe Workfront Planning]</a> 本文章內容。</td>
    </tr>
  </tbody>
</table>

### 更新記錄

此動作會更新Workfront Planning中的單一記錄。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有關建立與的連線的指示 [!DNL Adobe Workfront Planning]，請參閱 <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >建立與的連線 [!DNL Adobe Workfront Planning]</a> 本文章內容。</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[！UICONTROL記錄ID]</p>
      </td>
      <td>輸入或對應您要更新的記錄型別。 可用的記錄型別取決於您的Workfront Planning帳戶。</td> 
      </tr>
     <tr>
      <td role="rowheader">
        <p>其他欄位</p>
      </td>
      <td>這些欄位是根據您選取的記錄型別。</td> 
      </tr>
     <tr>
  </tbody>
</table>

### 搜尋記錄

此動作模組會根據您指定的條件擷取記錄清單。

>[!NOTE]
>
>此模組正在建構中。
