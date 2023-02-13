---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 連接器
navigation-topic: apps-and-their-modules
title: Split.io模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!DNL Split.io]，並將其連接至多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: 4576a2e4-b495-430e-a9de-4e1ec7379ab8
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1773'
ht-degree: 0%

---

# [!DNL Split.io] 模組

在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!DNL Split.io]，並將其連接至多個協力廠商應用程式和服務。

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

使用 [!DNL Split.io] 模組，您必須 [!DNL Split.io] 帳戶。

## Connect [!DNL Split.io] to [!DNL Workfront Fusion] {#connect-split-io-to-workfront-fusion}

您可以建立與 [!DNL Split.io] 直接從內部 [!DNL Split.io] 模組。

1. 在任何 [!DNL Split.io] 模組，按一下 **[!UICONTROL 新增]** 旁邊 [!UICONTROL 連線] 欄位。
1. 輸入連線的名稱。
1. 輸入 [!DNL Split.io] API金鑰。

   如需 [!DNL Split.io] API金鑰，請參閱 [API金鑰](https://help.split.io/hc/en-us/articles/360019916211-API-keys) 在 [!DNL Split.io] 檔案。

1. 按一下 **[!UICONTROL 繼續]** 若要建立連線，請返回模組。

## [!DNL Split.io] 模組及其欄位

設定時 [!DNL split.io] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!DNL split.io] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [動作](#actions)
* [搜尋](#searches)

### 動作

* [[!UICONTROL 自訂API呼叫]](#custom-api-call)
* [[!UICONTROL 分割]](#get-split)
* [[!UICONTROL 在環境中獲取拆分定義]](#get-split-definition-in-environment)
* [[!UICONTROL 建立拆分]](#create-split)
* [[!UICONTROL 刪除拆分]](#delete-split)
* [[!UICONTROL 在環境中建立拆分定義]](#create-split-definition-in-environment)
* [[!UICONTROL 從環境中刪除拆分定義]](#remove-split-definition-from-environment)
* [[!UICONTROL 環境中的部分更新拆分定義]](#partial-update-split-definition-in-environment)
* [[!UICONTROL 關聯標籤]](#associate-tags)

#### [!UICONTROL 自訂API呼叫]

此動作模組可讓您對 [!DNL split.io] API。 這樣，您就可以建立資料流自動化，而另一個無法完成 [!DNL split.io] 模組。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Split.io] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] 到[!UICONTROL Workfront Fusion] </a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>輸入相對於的路徑 <code>https://api.split.io/internal/api/v2/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL方法]</td> 
   <td> <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL標題]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標題。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion會為您新增授權標頭。</p> </td> 
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
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td>輸入或映射在每個方案執行週期中希望模組使用的最大記錄數。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 分割]

此動作模組會擷取分割。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Split.io] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] 到[!UICONTROL Workfront Fusion] </a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>選擇或映射包含要檢索的拆分的工作區。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL拆分名稱]</td> 
   <td> <p>輸入或映射要檢索的拆分的名稱。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 在環境中獲取拆分定義]

此動作模組會從指定環境中擷取特定的分割定義。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Split.io] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] 到[!UICONTROL Workfront Fusion] </a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>選擇或映射包含要檢索的拆分定義的工作區。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL環境名稱或ID]</td> 
   <td>選擇或映射包含要檢索的拆分定義的環境。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL拆分名稱]</td> 
   <td> <p>輸入或映射要檢索拆分定義的拆分的名稱。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立拆分]

在流量類型下，此動作模組會在您的組織中建立新的分割。

>[!NOTE]
>
>API不會在任何環境中設定分割。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Split.io] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] 到[!UICONTROL Workfront Fusion] </a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>選擇或映射要建立分割的工作區。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL流量類型ID或名稱]</td> 
   <td>選取或對應您要用來建立分割的流量類型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL拆分名稱]</td> 
   <td> <p>輸入或映射要建立的拆分的名稱。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL拆分說明]</td> 
   <td>輸入或映射要建立的拆分的[!UICONTROL拆分]說明。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除拆分]

此動作模組會從您的組織中刪除分割。 這會自動從所有環境中取消配置拆分定義。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Split.io] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] 到[!UICONTROL Workfront Fusion] </a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>選擇或映射要刪除分割的工作區。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL拆分名稱]</td> 
   <td> <p>輸入或映射要刪除的拆分的名稱。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 在環境中建立拆分定義]

此動作模組會為特定環境設定分割定義。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Split.io] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] 到[!UICONTROL Workfront Fusion] </a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>選擇或映射要建立拆分定義的工作區。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL環境名稱或ID]</td> 
   <td>選擇或映射要建立拆分定義的環境。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL拆分名稱]</td> 
   <td> <p>輸入或映射要為其建立定義的拆分的名稱。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL注釋]</td> 
   <td>輸入或映射要添加到拆分定義的任何注釋。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL規則]</td> 
   <td> <p>針對您要新增至定義的每個定位規則，按一下 <b>[!UICONTROL添加項]</b>，然後輸入或對應規則。</p> <p>如需鎖定規則的詳細資訊，請參閱 <a href="https://docs.split.io/reference#create-split-definition-in-environment">在環境中建立分割定義</a> 在 [!DNL Split.io] 檔案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL預設規則]</td> 
   <td> <p>輸入或映射您希望拆分用於不符合其他規則的規範的流量的規則。</p> <p>如需鎖定規則的詳細資訊，請參閱 <a href="https://docs.split.io/reference#create-split-definition-in-environment">在環境中建立分割定義</a> 在 [!DNL Split.io] 檔案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL預設處理]</td> 
   <td> <p>輸入或映射在拆分被終止或客戶未包含在流量分配中時，您希望拆分使用的處理。</p> <p>有關處理的詳細資訊，請參見 <a href="https://docs.split.io/reference#create-split-definition-in-environment">在環境中建立分割定義</a> 在 [!DNL Split.io] 檔案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL處理]</td> 
   <td> <p>對於要添加到定義中的每種處理，按一下 <b>[!UICONTROL添加項]</b>，然後輸入或映射處理。</p> <p>有關處理的詳細資訊，請參見 <a href="https://docs.split.io/reference#create-split-definition-in-environment">在環境中建立分割定義</a> 在 [!DNL Split.io] 檔案。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 從環境中刪除拆分定義]

此動作模組會取消設定特定環境的分割定義。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Split.io] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] 到[!UICONTROL Workfront Fusion] </a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>選擇或映射要刪除拆分定義的工作區。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL環境名稱或ID]</td> 
   <td>選擇或映射要刪除拆分定義的環境。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL拆分名稱]</td> 
   <td> <p>輸入或映射要刪除定義的拆分的名稱。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL注釋]</td> 
   <td>輸入或映射要添加到拆分定義的任何注釋。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 環境中的部分更新拆分定義]

此動作模組會更新特定環境的分割定義。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Split.io] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] 到[!UICONTROL Workfront Fusion] </a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>選擇或映射要更新分割定義的工作區。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL環境名稱或ID]</td> 
   <td>選擇或映射要更新拆分定義的環境。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL拆分名稱]</td> 
   <td> <p>輸入或映射要更新定義的拆分的名稱。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL更新內容]</td> 
   <td> <p>對於要更新的拆分的每個屬性，按一下 <b>[!UICONTROL添加項]</b> 並輸入或對應所需的變更。</p> <p>如需詳細資訊，請參閱 <a href="https://docs.split.io/reference#partial-update-split-definition-in-environment">環境中的部分更新拆分定義</a> 在 [!DNL Split.io] 檔案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL注釋]</td> 
   <td>輸入或映射要添加到拆分定義的任何注釋。</td> 
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
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Split.io] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] 到[!UICONTROL Workfront Fusion] </a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>選取或對應您要新增標籤的工作區。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL對象名稱]</td> 
   <td>輸入或映射要添加標籤的對象的名稱，</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL對象類型]</td> 
   <td> <p>輸入或映射要添加標籤的對象類型。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL標籤]</td> 
   <td> <p>針對您要新增的每個標籤，按一下 <b>[!UICONTROL添加項]</b> 並輸入或對應標籤。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 搜尋

* [[!UICONTROL 取得工作區]](#get-workspaces)
* [[!UICONTROL 取得環境]](#get-environments)
* [[!UICONTROL 獲取拆分]](#get-splits)
* [[!UICONTROL 在環境中列出拆分定義]](#list-split-definitions-in-an-environment)
* [[!UICONTROL 取得流量類型]](#get-traffic-types)

#### [!UICONTROL 取得工作區]

此搜尋模組會擷取組織的工作區。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Split.io] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] 到[!UICONTROL Workfront Fusion] </a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td>輸入或映射您希望模組在每個方案執行週期期間擷取的最大工作區數。</td> 
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
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Split.io] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] 到[!UICONTROL Workfront Fusion] </a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>選取或對應包含您要列出之環境的工作區。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 獲取拆分]

此搜尋模組會擷取分割清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Split.io] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] 到[!UICONTROL Workfront Fusion] </a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>選取或對應包含您要列出之分割的工作區。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td>輸入或映射您希望模組在每個方案執行週期期間擷取的最大分割數。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 在環境中列出拆分定義]

此搜尋模組會擷取指定環境中的分割定義清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Split.io] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] 到[!UICONTROL Workfront Fusion] </a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>選擇或映射包含要列出的拆分定義的工作區。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL環境名稱或ID]</td> 
   <td>選擇或映射包含要列出的拆分定義的環境。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td>輸入或映射您希望模組在每個方案執行週期中檢索的最大拆分定義數。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得流量類型]

此搜尋模組會擷取流量類型清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Split.io] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] 到[!UICONTROL Workfront Fusion] </a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>選取或對應包含您要列出之流量類型的工作區。</td> 
  </tr> 
 </tbody> 
</table>
