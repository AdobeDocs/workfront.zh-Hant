---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Microsoft Dynamics 365財務與營運模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用Microsoft Dynamics 365 Finance and Operations的工作流程，以及將其連線到多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion
source-git-commit: 130437dd44db5db2a94914fb0e42fd35a7c14291
workflow-type: tm+mt
source-wordcount: '995'
ht-degree: 0%

---

# [!DNL Microsoft Dynamics 365 Finance and Operations modules]

在[!DNL Adobe Workfront Fusion]案例中，您可以自動化使用[!DNL Microsoft Dynamics 365]的工作流程，並將其連線至多個協力廠商應用程式和服務。

>[!NOTE]
>
>[!DNL Microsoft Dynamics 365 Finance and Operations]聯結器不支援[!DNL Dynamics 365]。
>
>若為Microsoft Dynamics 365模組，請參閱[[!DNL Microsoft Dynamics 365 modules]](/help/quicksilver/workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md)。

如果您需要有關建立案例的指示，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md)中建立案例。

如需模組的相關資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md)中的[模組。

## 建立連線

若要建立Microsoft Dynamics 365 Finance and Operations模組的連線：

1. 在任何Microsoft Dynamics 365 Finance and Operations模組中，按一下[連線]方塊旁的[新增]。****

1. 填寫下列欄位：

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
        <td role="rowheader">[！UICONTROL連線型別]</td>
        <td>
          <p>選取您要建立標準的Dynamics Finance and Operations連線，或使用授權碼建立連線。</p>
        </td>
        </tr>
        <tr>
        <td role="rowheader">[！UICONTROL連線名稱]</td>
        <td>
          <p>輸入此連線的名稱。</p>
        </td>
        </tr>
        <tr>
        <td role="rowheader">[！UICONTROL使用者端ID]</td>
        <td>輸入您的Dynamics Finance and Operations [！UICONTROL使用者端ID]。</td>
        </tr>
        <tr>
        <td role="rowheader">[！UICONTROL使用者端密碼]</td>
        <td>輸入您的Dynamics Finance and Operations [！UICONTROL使用者端密碼]。 </td>
        </tr>
        <tr>
        <td role="rowheader">[！UICONTROL租使用者ID]</td>
        <td>輸入您的Dynamics Finance and Operations租使用者ID。</td>
        </tr>
        <tr>
        <td role="rowheader">資源</td>
        <td>輸入Dynamics Finance and Operations帳戶的URL (不含https://)</td>
        </tr>
      </tbody>
    </table>

1. 按一下&#x200B;**[!UICONTROL 繼續]**&#x200B;以儲存連線並返回模組。



## Microsoft Dynamics 365 Finance and Operations模組及其欄位

>[!IMPORTANT]
>
>透過Dynamics 365 F&amp;O API提供的資料實體可能會因執行個體而異。 如果您不確定哪些實體可透過API使用，則使用「data」端點來檢視例項中的實體會很有用。 Dynamics 365 Finance and Operations中的「資料」端點是用於存取OData服務的根URL。 此端點可讓您使用標準OData通訊協定，與系統公開的各種資料實體互動。
>
>您可以使用自訂API呼叫模組擷取這些實體。
>
><!--For more information -->



### 建立實體專案

此動作模組會在Microsoft Dynamics 365 Finance and Operations中建立新的實體專案。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[！UICONTROL Connection]</td>
    <td> <p>如需有關將Microsoft Dynamics 365 Finance and Operations連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#create-a-connection" class="MCXref xref">建立連線</a>。</p> </td> 
  </tr> 
  <tr> 
    <td>[！UICONTROL實體]</td>
     <td>輸入或對應您要建立的Dynamics Finance and Operations實體型別。</td> 
  </tr> 
  <tr> 
    <td>[！UICONTROL Body]</td>
     <td> <p>輸入或對應包含您要納入新實體專案之資料的JSON內文。</p> </td> 
  </tr> 
 </tbody> 
</table>



### 刪除實體專案

此動作模組會從Dynamics Finance and Operations刪除實體專案。 專案由其主索引鍵欄位識別。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[！UICONTROL Connection]</td>
    <td> <p>如需有關將Microsoft Dynamics 365 Finance and Operations連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#create-a-connection" class="MCXref xref">建立連線</a>。</p> </td> 
  </tr> 
  <tr> 
    <td>[！UICONTROL實體]</td>
     <td>輸入或對應您要刪除的Dynamics Finance and Operations實體型別。</td> 
  </tr> 
  <tr> 
    <td>[！UICONTROL主鍵欄位]</td>
     <td> 主索引鍵欄位可識別專案。 針對您想要提供的每個主索引鍵欄位，按一下<b>新增專案</b>，然後輸入或對應識別該專案的唯一索引鍵和值。 </td> 
  </tr> 
 </tbody> 
</table>

### 進行自訂API呼叫

此動作模組會對Dynamics Finance and Operations API進行自訂呼叫。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
    <td> <p>如需有關將Microsoft Dynamics 365 Finance and Operations連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#create-a-connection" class="MCXref xref">建立連線</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p>輸入相對於Dynamics Finance and Operations URL的路徑。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL方法]</td> 
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP要求方法。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標頭。 這會決定請求的內容型別。</p> <p>例如，<code> {"Content-type":"application/json"}</code></p> <p>注意：如果您收到錯誤且難以判斷其來源，請考慮根據[!DNL Workfront]檔案修改標題。 如果您的自訂API呼叫傳回422 HTTP請求錯誤，請嘗試使用<code>"Content-Type":"text/plain"</code>標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查詢字串]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的查詢。</p> <p>例如： <code>{"name":"something-urgent"}</code></p> <p>提示：建議您透過JSON內文傳送資訊，而非查詢引數。</p> </td> 
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



### 讀取實體專案

此動作模組會從實體專案傳回資料。 專案由其主索引鍵欄位識別。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[！UICONTROL Connection]</td>
    <td> <p>如需有關將Microsoft Dynamics 365 Finance and Operations連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#create-a-connection" class="MCXref xref">建立連線</a>。</p> </td> 
  </tr> 
  <tr> 
    <td>[！UICONTROL實體]</td>
     <td>輸入或對應您要讀取的Dynamics Finance and Operations實體型別。</td> 
  </tr> 
  <tr> 
    <td>[！UICONTROL主鍵欄位]</td>
     <td> 主索引鍵欄位可識別專案。 針對您想要提供的每個主索引鍵欄位，按一下<b>新增專案</b>，然後輸入或對應識別該專案的唯一索引鍵和值。 </td> 
  </tr> 
 </tbody> 
</table>

### 更新實體專案

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[！UICONTROL Connection]</td>
    <td> <p>如需有關將Microsoft Dynamics 365 Finance and Operations連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#create-a-connection" class="MCXref xref">建立連線</a>。</p> </td> 
  </tr> 
  <tr> 
    <td>[！UICONTROL實體]</td>
     <td>輸入或對應您要更新的Dynamics Finance and Operations實體型別。</td> 
  </tr>  
  <tr> 
    <td>[！UICONTROL主鍵欄位]</td>
     <td> 主索引鍵欄位可識別專案。 針對您想要提供的每個主索引鍵欄位，按一下<b>新增專案</b>，然後輸入或對應識別該專案的唯一索引鍵和值。 </td> 
  </tr> 
  <tr> 
    <td>[！UICONTROL Body]</td>
     <td> <p>輸入或對應包含您要納入新實體專案之資料的JSON內文。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 搜尋

此搜尋模組會根據您指定的條件傳回結果。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection]</td> 
   <td> <p>如需有關將[!DNL Workfront]應用程式連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">將[!DNL Workfront]連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL實體]</td> 
   <td>輸入或對應您要搜尋的Dynamics Finance and Operations實體型別。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL搜尋條件]</td> 
   <td> <p>輸入您要搜尋的欄位、要在查詢中使用的運運算元，以及要在欄位中搜尋的值。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL限制]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL排序依據]</td> 
   <td> <p>輸入或對應您要排序結果的欄位。</p> </td> 
  </tr> 
 </tbody> 
</table>


<!--

### List All

This module lists all records for a given entity.  The item is identified by its Primary key fields.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection]</td>
    <td> <p>For instructions about connecting Microsoft Dynamics 365 Finance and Operations to [!DNL Workfront Fusion], see <a href="#create-a-connection" class="MCXref xref">Create a connection</a> in this article.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Record Type]</td>
     <td>Choose the Dynamics Finance and Operations entity type that you want the module to list.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Outputs]</td>
     <td> <p>Select the information you want included in the output bundle for this module.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Watch Record

This trigger module starts a scenario when a record of the given type is created or updated.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
    <td> <p>For instructions about connecting Microsoft Dynamics 365 Finance and Operations to [!DNL Workfront Fusion], see <a href="#create-a-connection" class="MCXref xref">Create a connection</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Select the type of [!DNL Workfront] record that you want the module to watch.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>Enter the field that you want to search by, the operator you want to use in your query, and the value that you are searching for in the field.</p> <p>Note: Do not use <code>username </code>in your search criteria. Including <code>username </code>in an API query to [!DNL Workfront] logs the user into Workfront, and the search will not be successful.</p> <p>Note: <code>In</code> and <code>NotIn</code>work with arrays. The inputs should be in array format.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Select the information you want included in the output bundle for this module.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->
