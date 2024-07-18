---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Split.io模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動化使用 [!DNL Split.io]的工作流程，並將其連線到多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: 4576a2e4-b495-430e-a9de-4e1ec7379ab8
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1801'
ht-degree: 0%

---

# [!DNL Split.io]模組

在[!DNL Adobe Workfront Fusion]案例中，您可以自動化使用[!DNL Split.io]的工作流程，並將其連線至多個協力廠商應用程式和服務。

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
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]計畫，您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]計畫中。</p>
   <p>或</p>
   <p>舊版產品需求：您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 先決條件

若要使用[!DNL Split.io]模組，您必須有[!DNL Split.io]帳戶。

## 將[!DNL Split.io]連線至[!DNL Workfront Fusion] {#connect-split-io-to-workfront-fusion}

您可以直接從[!DNL Split.io]模組內建立與您的[!DNL Split.io]帳戶的連線。

1. 在任何[!DNL Split.io]模組中，按一下[!UICONTROL 連線]欄位旁的&#x200B;**[!UICONTROL 新增]**。
1. 輸入連線的名稱。
1. 輸入您的[!DNL Split.io] API金鑰。

   如需[!DNL Split.io] API金鑰的詳細資訊，請參閱[!DNL Split.io]檔案中的[API金鑰](https://help.split.io/hc/en-us/articles/360019916211-API-keys)。

1. 按一下&#x200B;**[!UICONTROL 繼續]**&#x200B;以建立連線並返回模組。

## [!DNL Split.io]模組及其欄位

當您設定[!DNL split.io]模組時，[!DNL Workfront Fusion]會顯示下列欄位。 除了這些欄位以外，可能還會顯示其他[!DNL split.io]欄位，視您在應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中將資訊從一個模組對應到另一個模組。

![](assets/map-toggle-350x74.png)

* [動作](#actions)
* [搜尋](#searches)

### 動作

* [[!UICONTROL 自訂API呼叫]](#custom-api-call)
* [[!UICONTROL 取得分割]](#get-split)
* [[!UICONTROL 在環境中取得分割定義]](#get-split-definition-in-environment)
* [[!UICONTROL 建立分割]](#create-split)
* [[!UICONTROL 刪除分割]](#delete-split)
* [[!UICONTROL 在環境中建立分割定義]](#create-split-definition-in-environment)
* [[!UICONTROL 從環境中移除分割定義]](#remove-split-definition-from-environment)
* [[!UICONTROL 在環境中部分更新分割定義]](#partial-update-split-definition-in-environment)
* [[!UICONTROL 關聯標籤]](#associate-tags)

#### [!UICONTROL 自訂API呼叫]

此動作模組可讓您對[!DNL split.io] API進行自訂的已驗證呼叫。 如此一來，您就可以建立其他[!DNL split.io]模組無法完成的資料流程自動化。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Split.io]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">將[!DNL Split.io]連線到[！UICONTROL Workfront Fusion] </a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL URL]</td> 
   <td>輸入相對於<code>https://api.split.io/internal/api/v2/</code>的路徑。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL方法]</td> 
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP要求方法。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標頭。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion會為您新增授權標頭。</p> </td> 
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
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td>輸入或對應您希望模組在每個案例執行週期中處理的最大記錄數量。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得分割]

此動作模組會擷取拆分。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Split.io]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">將[!DNL Split.io]連線到[！UICONTROL Workfront Fusion] </a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Workspace ID]</td> 
   <td>選取或對應包含您要擷取之分割的工作區。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL分割名稱]</td> 
   <td> <p>輸入或對映您要擷取的分割名稱。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 在環境中取得分割定義]

此動作模組會從指定的環境中擷取特定的分割定義。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Split.io]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">將[!DNL Split.io]連線到[！UICONTROL Workfront Fusion] </a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Workspace ID]</td> 
   <td>選取或對應包含您要擷取之分割定義的工作區。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL環境名稱或ID]</td> 
   <td>選取或對應包含您要擷取之分割定義的環境。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL分割名稱]</td> 
   <td> <p>輸入或對應您要擷取分割定義的分割名稱。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立分割]

在指定流量型別時，此動作模組會在您的組織中建立新的分割。

>[!NOTE]
>
>API不會在任何環境中設定分割。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Split.io]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">將[!DNL Split.io]連線到[！UICONTROL Workfront Fusion] </a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Workspace ID]</td> 
   <td>選取或對應您要建立分割的工作區。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL流量型別ID或名稱]</td> 
   <td>選取或對應您要用來建立分割的流量型別。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL分割名稱]</td> 
   <td> <p>輸入或對應您要建立的分割名稱。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL分割說明]</td> 
   <td>為您要建立的分割輸入或對映[！UICONTROL split]說明。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除分割]

此動作模組會從您的組織刪除分割。 這會從所有環境中自動取消設定分割定義。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Split.io]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">將[!DNL Split.io]連線到[！UICONTROL Workfront Fusion] </a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Workspace ID]</td> 
   <td>選取或對應您要刪除分割的工作區。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL分割名稱]</td> 
   <td> <p>輸入或對映您要刪除的分割名稱。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 在環境中建立分割定義]

此動作模組會為特定環境設定分割定義。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Split.io]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">將[!DNL Split.io]連線到[！UICONTROL Workfront Fusion] </a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Workspace ID]</td> 
   <td>選取或對應您要建立分割定義的工作區。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL環境名稱或ID]</td> 
   <td>選取或對應您要建立分割定義的環境。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL分割名稱]</td> 
   <td> <p>輸入或對應您要建立定義的分割名稱。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL註解]</td> 
   <td>輸入或對應您要新增至分割定義的任何註解。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL規則]</td> 
   <td> <p>針對您想要新增至定義的每個目標規則，按一下<b>[！UICONTROL新增專案]</b>，然後輸入或對應規則。</p> <p>如需鎖定目標規則的詳細資訊，請參閱[!DNL Split.io]檔案中的<a href="https://docs.split.io/reference#create-split-definition-in-environment">在環境中建立分割定義</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL預設規則]</td> 
   <td> <p>輸入或對映您要分割用於不符合其他規則規格的流量的規則。</p> <p>如需鎖定目標規則的詳細資訊，請參閱[!DNL Split.io]檔案中的<a href="https://docs.split.io/reference#create-split-definition-in-environment">在環境中建立分割定義</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL預設處理]</td> 
   <td> <p>輸入或對應分割要使用的處理方式（如果分割已終止或客戶未包含在流量分配中）。</p> <p>如需處理的詳細資訊，請參閱[!DNL Split.io]檔案中的<a href="https://docs.split.io/reference#create-split-definition-in-environment">在環境中建立分割定義</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Threads]</td> 
   <td> <p>針對您想要新增至定義的每個處理，按一下<b>[！UICONTROL新增專案]</b>，然後輸入或對應處理。</p> <p>如需處理的詳細資訊，請參閱[!DNL Split.io]檔案中的<a href="https://docs.split.io/reference#create-split-definition-in-environment">在環境中建立分割定義</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 從環境中移除分割定義]

此動作模組會取消設定特定環境的分割定義。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Split.io]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">將[!DNL Split.io]連線到[！UICONTROL Workfront Fusion] </a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Workspace ID]</td> 
   <td>選取或對應您要移除分割定義的工作區。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL環境名稱或ID]</td> 
   <td>選取或對應您要移除分割定義的環境。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL分割名稱]</td> 
   <td> <p>輸入或對應您要移除其定義的分割名稱。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL註解]</td> 
   <td>輸入或對應您要新增至分割定義的任何註解。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 在環境中部分更新分割定義]

此動作模組會更新特定環境的分割定義。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Split.io]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">將[!DNL Split.io]連線到[！UICONTROL Workfront Fusion] </a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Workspace ID]</td> 
   <td>選取或對應您要更新分割定義的工作區。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL環境名稱或ID]</td> 
   <td>選取或對應您要更新分割定義的環境。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL分割名稱]</td> 
   <td> <p>輸入或對應您要更新其定義的分割名稱。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL更新內容]</td> 
   <td> <p>針對您要更新的分割的每個屬性，按一下<b>[！UICONTROL新增專案]</b>，然後輸入或對應所需的變更。</p> <p>如需詳細資訊，請參閱[!DNL Split.io]檔案中的<a href="https://docs.split.io/reference#partial-update-split-definition-in-environment">環境</a>中的部分更新分割定義。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL註解]</td> 
   <td>輸入或對應您要新增至分割定義的任何註解。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 關聯標籤]

此動作模組會將標籤新增至指定的物件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Split.io]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">將[!DNL Split.io]連線到[！UICONTROL Workfront Fusion] </a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Workspace ID]</td> 
   <td>選取或對應您要新增標籤的工作區。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL物件名稱]</td> 
   <td>輸入或對應您要新增標籤的物件名稱，</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL物件型別]</td> 
   <td> <p>輸入或對應您要新增標籤的物件型別。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL標籤]</td> 
   <td> <p>針對您要新增的每個標籤，按一下<b>[！UICONTROL新增專案]</b>，然後輸入或對應標籤。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 搜尋

* [[!UICONTROL 取得工作區]](#get-workspaces)
* [[!UICONTROL 取得環境]](#get-environments)
* [[!UICONTROL 取得分割]](#get-splits)
* [[!UICONTROL 列出環境中的分割定義]](#list-split-definitions-in-an-environment)
* [[!UICONTROL 取得流量型別]](#get-traffic-types)

#### [!UICONTROL 取得工作區]

此搜尋模組會擷取組織的工作區。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Split.io]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">將[!DNL Split.io]連線到[！UICONTROL Workfront Fusion] </a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td>輸入或對應您希望模組在每個案例執行週期中擷取的最大工作區數量。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得環境]

此搜尋模組會擷取環境清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Split.io]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">將[!DNL Split.io]連線到[！UICONTROL Workfront Fusion] </a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Workspace ID]</td> 
   <td>選取或對應包含您要列出之環境的工作區。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得分割]

此搜尋模組會擷取分割清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Split.io]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">將[!DNL Split.io]連線到[！UICONTROL Workfront Fusion] </a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Workspace ID]</td> 
   <td>選取或對映包含您要列出之分割的工作區。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td>輸入或對應您希望模組在每個案例執行週期中擷取的最大分割數。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出環境中的分割定義]

此搜尋模組會擷取指定環境中分割定義的清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Split.io]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">將[!DNL Split.io]連線到[！UICONTROL Workfront Fusion] </a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Workspace ID]</td> 
   <td>選取或對應包含您要列出之分割定義的工作區。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL環境名稱或ID]</td> 
   <td>選取或對應包含您要列出之分割定義的環境。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td>輸入或對應您希望模組在每個案例執行週期中擷取的最大分割定義數目。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得流量型別]

此搜尋模組會擷取流量型別清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Split.io]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">將[!DNL Split.io]連線到[！UICONTROL Workfront Fusion] </a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Workspace ID]</td> 
   <td>選取或對應包含您要列出之流量型別的工作區。</td> 
  </tr> 
 </tbody> 
</table>
