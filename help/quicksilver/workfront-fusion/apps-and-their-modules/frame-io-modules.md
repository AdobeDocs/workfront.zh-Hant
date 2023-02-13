---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 連接器
navigation-topic: apps-and-their-modules
title: Frame.io模組
description: 此 [!DNL Adobe Workfront Fusion Frame].io modules enable you to monitor, create, update, retrieve, or delete assets and comments in your [!DNL Frame.io] 帳戶。
author: Becky
feature: Workfront Fusion
exl-id: 373a86f6-fbba-4914-b08d-a3a035ac0ae4
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2263'
ht-degree: 0%

---

# [!DNL Frame.io] 模組

此 [!DNL Adobe Workfront Fusion] [!DNL Frame.io] 模組可讓您監視、建立、更新、擷取或刪除您 [!DNL Frame.io] 帳戶。

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

使用 [!DNL Frame.io] 模組，您必須 [!DNL Frame.io] 帳戶

## Connect [!DNL Frame.io] to [!UICONTROL Adobe Workfront融合]

您可以連線至 [!DNL Frame.io] 使用API代號，或使用OAuth 2.0。

[連線至 [!DNL Frame.io] 使用API代號](#connect-to-frameio-using-an-api-token)

[連線至 [!DNL Frame.io] 使用OAuth 2.0 PKCE](#connect-to-frameio-using-oauth-20-pkce)

### 連線至 [!DNL Frame.io] 使用API代號

連接 [!DNL Frame.io] 帳戶 [!DNL Workfront Fusion] 您必須使用API代號，在 [!DNL Frame.io] 帳戶並插入 [!DNL Workfront Fusion] [!DNL Frame.io] [!UICONTROL 建立連線] 對話框。

1. 登入 [!DNL Frame.io] 帳戶。
1. 前往 **[!UICONTROL 代號]** 頁面 [!DNL Frame.io] 開發人員。
1. 按一下 **[!UICONTROL 新增]**.
1. 輸入令牌的名稱，選擇要使用的作用域，然後按一下 **[!UICONTROL 建立]**.
1. 複製提供的Token。
1. 前往 [!DNL Workfront Fusion] 然後開啟 [!DNL Frame.io] 模組 **[!UICONTROL 建立連線]** 對話框。
1. 在 **[!UICONTROL 連線類型]** 欄位，選擇 **[!DNL Frame.io]**.
1. 輸入您在步驟5中複製到 **[!UICONTROL 您的 [!DNL Frame.io] API金鑰]** 欄位，按一下 **[!UICONTROL 繼續]** 建立連接。

已建立連接。 您可以繼續設定模組。

### 連線至 [!DNL Frame.io] 使用OAuth 2.0 PKCE

您可以建立連線至 [!DNL Frame.io] 使用OAuth 2.0 PKCE搭配選用的用戶端ID。 如果您想在連線中加入用戶端ID，您必須在您的 [!DNL Frame.io] 帳戶。

* [連線至 [!DNL Frame.io] 使用OAuth 2.0 PKCE（不含用戶端ID）](#connect-to-frameio-using-using-oauth-20-pkce-without-client-id)
* [連線至 [!DNL Frame.io] 使用OAuth 2.0 PKCE（搭配用戶端ID）](#connect-to-frameio-using-using-oauth-20-pkce-with-client-id)

#### 連線至 [!DNL Frame.io] 使用OAuth 2.0 PKCE（不含用戶端ID）

1. 前往 [!DNL Workfront Fusion] 然後開啟 [!DNL Frame.io] 模組 **[!UICONTROL 建立連線]** 對話框。
1. 在 **[!UICONTROL 連線類型]** 欄位，選擇 **[!UICONTROL [!DNL Frame.io]OAuth 2.0 PKCE]**.
1. 在 **[!UICONTROL 連線名稱]** 欄位。
1. 按一下 **[!UICONTROL 繼續]** 建立連接。

已建立連接。 您可以繼續設定模組。

#### 連線至 [!DNL Frame.io] 使用OAuth 2.0 PKCE（搭配用戶端ID）

1. 在中建立OAuth 2.0應用程式 [!DNL Frame.io]. 如需指示，請參閱 [!DNL Frame.io] 檔案 [!UICONTROL OAuth 2.0程式碼授權流程].

   >[!IMPORTANT]
   >
   >在中建立OAuth 2.0應用程式時 [!DNL Frame.io]:
   >
   >* 輸入以下內容作為重定向URI:
   >   
   >  美洲/亞太地區 `https://app.workfrontfusion.com/oauth/cb/frame-io5`
   >
   >  歐洲、中東和非洲 `https://app-eu.workfrontfusion.com/oauth/cb/frame-io5`
   >
   >* 啟用PCKE選項。



1. 複製提供的 `client_id`.
1. 前往 [!DNL Workfront Fusion] 然後開啟 [!DNL Frame.io] 模組 **[!UICONTROL 建立連線]** 對話框。
1. 在 **[!UICONTROL 連線類型]** 欄位，選擇 **[!UICONTROL [!DNL Frame.io]OAuth 2.0 PKCE]**.
1. 在 **[!UICONTROL 連線名稱]** 欄位。
1. 按一下 **[!UICONTROL 顯示高級設定]**.
1. 輸入 `client_id` 您在步驟2中複製到 **[!UICONTROL 用戶端ID]** 欄位。
1. 按一下 **[!UICONTROL 繼續]** 建立連接。

已建立連接。 您可以繼續設定模組。

## [!DNL Frame.io] 模組及其欄位

設定時 [!DNL Frame.io] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!DNL Frame.io] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [資產](#assets)
* [註解](#comments)
* [專案](#projects)
* [其他](#other)

### 資產

* [[!UICONTROL 建立資產]](#create-an-asset)
* [[!UICONTROL 刪除資產]](#delete-an-asset)
* [[!UICONTROL 取得資產]](#get-an-asset)
* [[!UICONTROL 列出資產]](#list-assets)
* [[!UICONTROL 更新資產]](#update-an-asset)
* [[!UICONTROL 已刪除監看資產]](#watch-asset-deleted)
* [[!UICONTROL 已更新監看資產標籤]](#watch-asset-label-updated)
* [[!UICONTROL 觀看新資產]](#watch-new-asset)

#### [!UICONTROL 建立資產]

此動作模組會建立新資產。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td>有關建立連接的說明 [!DNL Frame.io]，請參閱 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> 這篇文章。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL團隊ID] </td> 
   <td> <p>選取或對應擁有您要建立資產之專案的團隊。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL項目ID] </td> 
   <td> <p>選取您要建立資產的專案ID，或對應該項目的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資料夾ID] </td> 
   <td> <p>選取要在中建立資產的資料夾ID，或對應該在其中建立資產的資料夾ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL類型] </td> 
   <td> <p>選擇要建立資料夾還是檔案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL名稱] </td> 
   <td> <p>輸入新檔案或資料夾的名稱。</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">File Type </td> 
    <td> <p>Select the type of file you want to upload.</p> </td> 
   </tr>
  --> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">File Size </td> 
    <td> <p>The file size in bytes.</p> </td> 
   </tr>
  --> 
  <tr> 
   <td role="rowheader">[!UICONTROL源URL] </td> 
   <td> <p>輸入要上傳之檔案的URL。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL描述] </td> 
   <td> <p>輸入資產的簡短說明。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除資產]

此動作模組會刪除指定的資產。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL連接] </td> 
   <td>有關建立連接的說明 [!DNL Frame.io]，請參閱 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> 這篇文章。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL團隊ID] </td> 
   <td> <p>選擇或映射擁有包含您要刪除資產之專案的團隊。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL項目ID]</td> 
   <td> <p> 選取包含您要刪除資產的專案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資料夾ID] </td> 
   <td> <p>選取包含您要刪除資產的資料夾</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資產ID] </td> 
   <td> <p>選取或對應您要刪除的資產。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得資產]

此動作模組會擷取資產詳細資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL連接] </td> 
   <td>有關建立連接的說明 [!DNL Frame.io]，請參閱 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> 這篇文章。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL團隊ID] </td> 
   <td> <p>選擇或映射擁有項目的團隊，該項目包含您要檢索相關詳細資訊的資產。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL項目ID]</td> 
   <td> <p> 選取包含您要擷取其詳細資訊之資產的專案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資料夾ID] </td> 
   <td> <p>選取包含您要擷取其詳細資訊之資產的資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資產ID] </td> 
   <td> <p>選取要擷取相關詳細資訊之資產的ID，或對應該該資產的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出資產]

此搜尋模組會擷取指定專案資料夾中的所有資產。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL連接] </td> 
   <td>有關建立連接的說明 [!DNL Frame.io]，請參閱 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> 這篇文章。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL團隊ID] </td> 
   <td> <p>選取或對應擁有專案的團隊，該專案包含您要擷取資產的資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL項目ID]</td> 
   <td> <p> 選取包含您要擷取資產之資料夾的專案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資料夾ID] </td> 
   <td> <p>選取要列出資產的資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制] </td> 
   <td> <p>設定資產數上限 [!DNL Workfront Fusion] 會在一個執行週期期間傳回。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### `[!UICONTROL Update an Asset]`

此動作模組可讓您更新現有資產的名稱、說明或自訂欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL連接] </td> 
   <td>有關建立連接的說明 [!DNL Frame.io]，請參閱 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> 這篇文章。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL團隊ID] </td> 
   <td> <p>選取或對應擁有您要更新資產之專案的團隊。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL項目ID] </td> 
   <td> <p>選取您要更新資產的專案ID，或對應該項目的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資料夾ID] </td> 
   <td> <p>選取要更新資產的資料夾ID，或將其對應。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL名稱] </td> 
   <td> <p>輸入更新檔案的名稱。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL描述] </td> 
   <td> <p>輸入更新資產的簡短說明。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 已刪除監看資產]

此觸發器模組會在資產刪除時啟動案例。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook名稱]</td> 
   <td> <p> 輸入Webhook的名稱，例如已刪除資產。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL連接] </td> 
   <td>有關建立連接的說明 [!DNL Frame.io]，請參閱 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> 這篇文章。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL團隊ID] </td> 
   <td> <p>選擇為此Webhook建立的團隊。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 已更新監看資產標籤]

此觸發模組會在資產的狀態設定、變更或移除時啟動案例。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook名稱]</td> 
   <td> <p> 輸入Webhook的名稱，例如資產狀態已更新。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL連接] </td> 
   <td>有關建立連接的說明 [!DNL Frame.io]，請參閱 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> 這篇文章。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL團隊ID] </td> 
   <td> <p>選擇為此Webhook建立的團隊。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 觀看新資產]

此觸發模組會在建立新資產時啟動案例。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook名稱]</td> 
   <td> <p> 輸入網頁連結的名稱，例如已建立資產。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL連接] </td> 
   <td>有關建立連接的說明 [!DNL Frame.io]，請參閱 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> 這篇文章。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL團隊ID] </td> 
   <td> <p>選擇為此Webhook建立的團隊。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 註解

* [[!UICONTROL 建立注釋]](#create-a-comment)
* [[!UICONTROL 刪除注釋]](#delete-a-comment)
* [[!UICONTROL 取得意見]](#get-a-comment)
* [[!UICONTROL 列出注釋]](#list-comments)
* [[!UICONTROL 更新注釋]](#update-a-comment)
* [[!UICONTROL 已更新Watch注釋]](#watch-comment-updated)
* [[!UICONTROL 觀看新留言]](#watch-new-comment)

#### [!UICONTROL 建立注釋]

此動作模組會新增註解或回覆至資產。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL連接] </td> 
   <td>有關建立連接的說明 [!DNL Frame.io]，請參閱 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> 這篇文章。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL類型] </td> 
   <td> <p>選擇要建立評論還是回覆評論。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL團隊ID] </td> 
   <td> <p>選擇或映射擁有項目的團隊，該項目包含您要添加評論的資產。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL項目ID] </td> 
   <td> <p>選取專案，或對應包含您要新增註解之資產的專案ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資料夾ID] </td> 
   <td> <p>選取資料夾，或對應包含您要新增註解之資產的資料夾ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資產ID] </td> 
   <td> <p>選取或對應您要新增註解的資產。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL注釋ID] </td> 
   <td> <p>選擇或映射要添加回復的評論。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL文本]</td> 
   <td> <p> 輸入評論或回覆的文本內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL時間戳] </td> 
   <td> <p>在評論應連結的視訊中輸入幀號。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除注釋]

此動作模組會刪除現有的註解。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL連接] </td> 
   <td>有關建立連接的說明 [!DNL Frame.io]，請參閱 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> 這篇文章。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL團隊ID]</td> 
   <td> <p> 選擇或映射擁有項目的團隊，該項目包含您要刪除評論的資產。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL項目ID]</td> 
   <td> <p> 選取專案或對應包含您要刪除註解之資產的專案ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資料夾ID]</td> 
   <td> <p> 選取包含您要刪除註解之資產的資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資產ID] </td> 
   <td> <p>選取包含您要刪除之註解的資產。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL注釋ID] </td> 
   <td> <p>選擇要刪除的注釋。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得意見]

此動作模組會擷取指定留言的詳細資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL連接] </td> 
   <td>有關建立連接的說明 [!DNL Frame.io]，請參閱 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> 這篇文章。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL團隊ID] </td> 
   <td> <p>選取或對應擁有專案的團隊，該專案包含您要從中擷取資產的資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL項目ID] </td> 
   <td> <p>選取包含您要擷取資產之資料夾的專案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資料夾ID] </td> 
   <td> <p>選取要列出資產的資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資產ID] </td> 
   <td> <p>選取包含您要擷取之註解的資產。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL注釋ID] </td> 
   <td> <p>選擇要檢索有關的詳細資訊的注釋。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出注釋]

此搜尋模組會擷取指定資產的所有註解。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL連接] </td> 
   <td>有關建立連接的說明 [!DNL Frame.io]，請參閱 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> 這篇文章。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL團隊ID] </td> 
   <td> <p>選擇或映射擁有包含要從中檢索注釋的資料夾的項目的團隊。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL項目ID] </td> 
   <td> <p>選擇包含要從中檢索注釋的資料夾的項目。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資料夾ID] </td> 
   <td> <p>選取包含您要列出註解之資產的資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資產ID] </td> 
   <td> <p>選取您要列出備注的資產。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制] </td> 
   <td> <p>設定注釋的最大數量 [!DNL Workfront Fusion] 會在一個執行週期期間傳回。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新注釋]

此動作模組會編輯現有的註解。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL連接] </td> 
   <td>有關建立連接的說明 [!DNL Frame.io]，請參閱 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> 這篇文章。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL團隊ID] </td> 
   <td> <p>選擇或映射擁有項目的團隊，該項目包含您要更新評論的資產。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL項目ID] </td> 
   <td> <p>選取包含您要更新註解之資產的專案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資料夾ID] </td> 
   <td> <p>選取包含您要更新註解之資產的資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資產ID] </td> 
   <td> <p>選取您要更新註解的資產。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL注釋ID] </td> 
   <td> <p>選擇要更新的注釋。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL文本]</td> 
   <td> <p> 輸入注釋的文本內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL時間戳] </td> 
   <td> <p>在評論連結的視頻中輸入幀號。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 已更新Watch注釋]

編輯註解時，此觸發模組會啟動案例。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook名稱] </td> 
   <td> <p>輸入Webhook的名稱，例如「已編輯注釋」。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL連接] </td> 
   <td>有關建立連接的說明 [!DNL Frame.io]，請參閱 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> 這篇文章。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL團隊ID] </td> 
   <td> <p>選擇為此Webhook建立的團隊。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 觀看新留言]

建立新留言或回覆時，此觸發模組就會啟動案例。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook名稱] </td> 
   <td> <p>輸入Webhook的名稱，例如「新注釋」。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL連接] </td> 
   <td>有關建立連接的說明 [!DNL Frame.io]，請參閱 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> 這篇文章。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL團隊ID] </td> 
   <td> <p>選擇為此Webhook建立的團隊。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 專案

#### [!UICONTROL 列出專案]

此搜尋模組會擷取指定團隊的所有專案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL連接] </td> 
   <td>有關建立連接的說明 [!DNL Frame.io]，請參閱 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> 這篇文章。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL團隊ID] </td> 
   <td> <p>選擇或映射要為其檢索項目的團隊。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制] </td> 
   <td> <p>設定專案的最大數量 [!DNL Workfront Fusion] 會在一個執行週期期間傳回。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 其他

#### [!UICONTROL 進行API呼叫]

此模組可讓您執行自訂API呼叫。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL連接] </td> 
   <td>有關建立連接的說明 [!DNL Frame.io]，請參閱 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Frame.io] to [!DNL Adobe Workfront Fusion]</a> 這篇文章。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>輸入相對於的路徑 <code>https://api.frame.io</code>. 範例: <code> /v2/teams</code></p> <p>注意：如需可用端點的清單，請參閱 [!DNL Frame.io] API參考。</p> </td> 
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
   <td> <p>輸入請求查詢字串。 針對您要納入查詢字串的每個參數，按一下 <b>[!UICONTROL添加項]</b> 並輸入欄位的名稱和所需值。</p> </td> 
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

**範例：** 下列API呼叫會傳回所有團隊，並在 [!DNL Frame.io] 帳戶：

URL: `/v2/teams`

方法: `GET`

![](assets/api-call-example.png)

結果可在模組的「輸出」(Output)下的「捆綁」(Bundle)>「主體」(Body)下找到。

在我們的範例中，傳回1個團隊的詳細資料：

![](assets/api-call-output.png)
