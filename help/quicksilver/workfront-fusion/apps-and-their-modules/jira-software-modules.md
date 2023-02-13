---
title: Jira軟體模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!DNL Jira] 軟體，並將其連接到多個第三方應用程式和服務。
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 6437fe98-2c2b-4b49-97e2-f94b23da93fd
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2039'
ht-degree: 1%

---

# [!DNL Jira Software] 模組

在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!DNL Jira Software]，並將其連接至多個協力廠商應用程式和服務。

如果您需要建立案例的相關指示，請參閱 [在中建立案例 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

如需模組的相關資訊，請參閱 [中的模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

<!-- Bob Fix this compared to original -->

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
   <td> <p>[!UICONTROL Workfront Fusion for Work Automation and Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 必要條件

使用 [!DNL Jira] 模組 [!DNL Jira] 帳戶。

## Connect [!DNL Jira Software] to [!DNL Workfront Fusion]

您的連線方法是根據您是否使用 [!DNL Jira Cloud] 或 [!DNL Jira Server].

* [Connect [!DNL Jira Cloud] 到Workfront Fusion](#connect-jira-cloud-to-workfront-fusion)
* [Connect [!DNL Jira Server] to [!DNL Workfront Fusion]](#connect-jira-server-to-workfront-fusion)

### Connect [!DNL Jira Cloud] to [!DNL Workfront Fusion]

Connect [!DNL Jira Cloud] to [!DNL Workfront Fusion]

連接 [!DNL Jira Software] to [!DNL Workfront Fusion]，您必須建立API Token，並將其與您的服務URL和使用者名稱插入至 [!UICONTROL 建立連線] 欄位 [!DNL Workfront Fusion].

#### 在中建立API代號 [!DNL Jira]

1. 前往 [https://id.atlassian.com/manage/api-tokens](https://id.atlassian.com/manage/api-tokens) 並登入。
1. 按一下 **[!UICONTROL 建立API代號]**.
1. 輸入代號的名稱，例如 *Workfront融合*.
1. 使用 **[!UICONTROL 複製到剪貼簿]** 按鈕。

   >[!IMPORTANT]
   >
   >關閉此對話方塊後，無法再檢視Token。
1. 將產生的代號儲存在安全位置。
1. 繼續 [設定 [!DNL Jira] 中的API代號 [!DNL Workfront Fusion]](#configure-the-jira-api-token-in-workfront-fusion).

#### 設定 [!DNL Jira] 中的API代號 [!DNL Workfront Fusion]

1. 在 [!DNL Workfront Fusion]，新增 [!DNL Jira] 模組至方案以開啟 **[!UICONTROL 建立連線]** 框。
1. 指定下列資訊：

   * **[!UICONTROL 服務URL]**
   * **[!UICONTROL 使用者名稱]**
   * **[!UICONTROL API代號]:** 這是您在 [在中建立API代號 [!DNL Jira]](#create-an-api-token-in-jira) 本文的一節。

1. 按一下 [!UICONTROL 繼續] 以建立連線並返回模組。

### Connect [!DNL Jira Server] to [!DNL Workfront Fusion]

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Becky: Find out and document how to find these things</p>
-->

授權之間的連線 [!DNL Workfront Fusion] 和 [!DNL Jira Server]，您需要您的消費者金鑰、私密金鑰和服務URL。 您可能需要聯絡 [!DNL Jira] 管理員。

* [為您的 [!DNL Jira] 連接](#generate-public-and-private-keys-for-your-jira-connection)
* [將用戶端應用程式設為 [!DNL Jira]](#configure-the-client-app-as-a-consumer-in-jira)
* [建立連線至 [!DNL Jira] 中的伺服器或Jira資料中心 [!DNL Workfront Fusion]](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion)

#### 為您的 [!DNL Jira] 連接

為您的 [!DNL Workfront Fusion Jira] 連線，您需要產生公開金鑰和私密金鑰。

1. 在您的終端機中，執行下列 `openssl` 命令。

   * `openssl genrsa -out jira_privatekey.pem 1024`

      此命令生成1024位私鑰。

   * `openssl req -newkey rsa:1024 -x509 -key jira_privatekey.pem -out jira_publickey.cer -days 365`

      此命令建立X509證書。

   * `openssl pkcs8 -topk8 -nocrypt -in jira_privatekey.pem -out jira_privatekey.pcks8`

      此命令將私鑰（PKCS8格式）提取到 `jira_privatekey.pcks8`
檔案。

   * `openssl x509 -pubkey -noout -in jira_publickey.cer  > jira_publickey.pem`

      此命令會從憑證中擷取公開金鑰至 `jira_publickey.pem` 檔案。

      >[!NOTE]
      >
      >如果您使用Windows，則可能需要將公開金鑰儲存至 `jira_publickey.pem` 檔案：
      >
      >1. 在您的終端機中，執行下列命令：
      >   
      >   `openssl x509 -pubkey -noout -in jira_publickey.cer`
      >   
      >1. 複製終端輸出(包括 `-------BEGIN PUBLIC KEY--------` 和 `-------END PUBLIC KEY--------`
      >   
      >1. 將終端輸出貼入名為 `jira_publickey.pem`.



1. 繼續 [將用戶端應用程式設為 [!DNL Jira]](#configure-the-client-app-as-a-consumer-in-jira)

#### 將用戶端應用程式設為 [!DNL Jira]

1. 登入 [!DNL Jira] 例項。
1. 在左側導覽面板中，按一下 **[!UICONTROL [!DNL Jira]設定]** ![](assets/jira-settings-icon.png) > **[!UICONTROL 應用程式]**> **[!UICONTROL 應用程式連結]**.
1. 在 **[!UICONTROL 輸入要連結的應用程式的URL]** 欄位，輸入

   ```
   https://app.workfrontfusion.com/oauth/cb/workfront-jiraserver-oauth1
   ```

1. 按一下 **[!UICONTROL 建立新連結]**. 忽略「未從您輸入的URL收到任何回應」錯誤訊息。
1. 在 **[!UICONTROL 連結應用程式]** ，請在 **[!UICONTROL 使用者金鑰]** 和 **[!UICONTROL 共用機密]** 欄位。

   您可以選擇這些欄位的值。

1. 複製 **[!UICONTROL 使用者金鑰]** 和 **[!UICONTROL 共用機密]** 欄位移至安全位置。

   您稍後會在設定程式中需要這些值。

1. 填寫URL欄位如下：

   | 欄位 | 說明 |
   |---|---|
   | [!UICONTROL 要求Token URL] | `<Jira base url>/plugins/servlet/oauth/request-token` |
   | [!UICONTROL 授權URL] | `<Jira base url>/plugins/servlet/oauth/authorize` |
   | [!UICONTROL 存取權杖URL] | `<Jira base url>/plugins/servlet/oauth/access-token` |

1. 選取 **[!UICONTROL 建立傳入連結]** 核取方塊。
1. 按一下 **[!UICONTROL 繼續]**.
1. 在 **[!UICONTROL 連結應用程式]** ，請填寫以下欄位：

   <table style="table-layout:auto"> 
    <col data-mc-conditions=""> 
    <col data-mc-conditions=""> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL使用者金鑰]</p> </td> 
      <td> 貼入您複製到安全位置的使用者金鑰。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL使用者名稱]</td> 
      <td>輸入您選擇的名稱。 此名稱僅供您參考。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL公鑰]</td> 
      <td>貼入您 <code>[!DNL jira_publickey.pem]</code> 檔案。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **[!UICONTROL 繼續]**.
1. 繼續 [建立連線至 [!DNL Jira Server] 或 [!DNL Jira Data Center] in [!DNL Workfront Fusion]](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion)

#### 建立連線至 [!DNL Jira Server] 或 [!DNL Jira Data Center] in [!DNL Workfront Fusion]

>[!NOTE]
>
>使用 [!DNL Jira Server] 連接到 [!DNL Jira Server] 或 [!DNL Jira Data Center].
1. 在任何 [!DNL Jira Server] 模組 [!DNL Workfront Fusion]，按一下 **[!UICONTROL 新增]** 旁邊 [!UICONTROL 連接] 欄位。
1. 在 [!UICONTROL 建立連線] 面板中，填入下列欄位：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL連接名]</p> </td> 
      <td> <p>輸入連接的名稱</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL使用者金鑰]</td> 
      <td>貼入您複製至安全位置的使用者金鑰，位於 <a href="#configure-the-client-app-as-a-consumer-in-jira" class="MCXref xref">將用戶端應用程式設為 [!DNL Jira]</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Private Key]</td> 
      <td>貼入 <code>[!DNL jira_privatekey.pcks8]</code> 在 <a href="#generate-public-and-private-keys-for-your-jira-connection" class="MCXref xref">為您的 [!DNL Jira] 連接</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Service URL]</td> 
      <td>輸入 [!DNL Jira] 例項URL。 </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **[!UICONTROL 繼續]** 若要建立連線，請返回模組。

## [!DNL Jira Software] 模組及其欄位

設定時 [!DNL Jira Software] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!DNL Jira Software] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [觸發器](#triggers)
* [動作](#actions)
* [搜尋](#searches)

### 觸發器

#### [!UICONTROL 留意記錄]

此觸發模組會在新增、更新或刪除記錄時啟動案例。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>選取您要用來監看記錄的網頁連結。 </p> <p>要添加新網頁鈎點：</p> 
    <ol> 
     <li value="1">按一下 <strong>[!UICONTROL添加]</strong></li> 
     <li value="2">輸入Webhook的名稱。</li> 
     <li value="3"> <p>選取您要用於網頁連結的連線。 </p> <p>有關連接 [!DNL Jira Software] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </li> 
     <li value="4"> <p>選擇要軟體監視的記錄類型：</p> 
      <ul> 
       <li>[!UICONTROL注釋] </li> 
       <li>[!UICONTROL問題]</li> 
       <li>[!UICONTROL項目] </li> 
       <li>[!UICONTROL Sprint]</li> 
      </ul> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### 動作

* [[!UICONTROL 向衝刺添加問題]](#add-issue-to-sprint)
* [[!UICONTROL 自訂API呼叫]](#custom-api-call)
* [[!UICONTROL 建立記錄]](#create-a-record)
* [[!UICONTROL 刪除記錄]](#delete-a-record)
* [[!UICONTROL 下載附件]](#download-an-attachment)
* [[!UICONTROL 讀取記錄]](#read-a-record)
* [[!UICONTROL 更新記錄]](#update-a-record)

#### [!UICONTROL 向衝刺添加問題]

此動作模組會新增一或多個問題至衝刺。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Jira Software] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sprint ID]</td> 
   <td>輸入或映射要添加問題的衝刺的衝刺ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL問題ID或密鑰]</td> 
   <td>為您要加入衝刺的每個問題新增問題ID或金鑰。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立記錄]

此動作模組在Jira中建立新記錄。

模組會傳回與記錄相關聯的任何標準欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Jira Software] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL記錄類型]</td> 
   <td> <p>選擇要模組建立的記錄類型。 選取記錄類型時，該記錄類型的其他特定欄位會出現在模組中。</p> 
    <ul> 
     <li>[!UICONTROL附件]</li> 
     <li>[!UICONTROL注釋]</li> 
     <li>[!UICONTROL問題]</li> 
     <li>[!UICONTROL項目]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL工作日誌]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 自訂API呼叫]

此動作模組可讓您對 [!DNL Jira Software] API。 這樣，您就可以建立資料流自動化，而另一個無法完成 [!DNL Jira Software] 模組。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Jira Software] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>輸入相對於的路徑<code>&lt;Instance URL>/rest/api/2/ </code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL方法]</td> 
   td&gt; <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL標題]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標題。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 為您添加授權標頭。</p> </td> 
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

#### [!UICONTROL 刪除記錄]

此動作模組會刪除特定記錄。

您指定記錄的ID。

模組會傳回記錄和任何相關欄位的ID，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Jira Software] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL記錄類型]</td> 
   <td> <p>選擇要刪除模組的記錄類型。 </p> 
    <ul> 
     <li>[!UICONTROL附件]</li> 
     <li>[!UICONTROL注釋]</li> 
     <li>[!UICONTROL問題]</li> 
     <li>[!UICONTROL項目]</li> 
     <li>[!UICONTROL Sprint] </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID或Key]</td> 
   <td>輸入或映射要刪除的記錄的ID或密鑰。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 下載附件]

此動作模組會下載特定附件。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Jira Software] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>輸入或映射要下載的附件ID。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 讀取記錄]

此動作模組會從中的單一記錄讀取資料 [!DNL Jira Software].

您指定記錄的ID。

模組會傳回與記錄相關聯的任何標準欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Jira Software] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL記錄類型]</td> 
   <td> <p>選取 [!DNL Jira] 記錄您要讀取的模組。</p> 
    <ul> 
     <li>[!UICONTROL附件]</li> 
     <li>[!UICONTROL問題]</li> 
     <li>[!UICONTROL項目]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL用戶]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸出]</td> 
   <td>選取要接收的輸出。 根據在「[!UICONTROL記錄類型]」欄位中選擇的記錄類型，可以使用輸出選項。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td> <p>輸入或對應唯一 [!DNL Jira Software] 您要模組讀取的記錄ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新記錄]

此動作模組會更新現有記錄，例如問題或專案。

您指定記錄的ID。

模組會傳回記錄和任何相關欄位的ID，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Jira Software] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL記錄類型]</td> 
   <td> <p>選擇要更新模組的記錄類型。 選取記錄類型時，該記錄類型的其他特定欄位會出現在模組中。</p> 
    <ul> 
     <li>[!UICONTROL注釋]</li> 
     <li>[!UICONTROL問題]</li> 
     <li>[!UICONTROL項目]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL轉換問題]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID或Key]</td> 
   <td>輸入或映射要更新的記錄的ID或密鑰。</td> 
  </tr> 
 </tbody> 
</table>

### 搜尋

* [[!UICONTROL 清單記錄]](#list-records)
* [[!UICONTROL 搜索記錄]](#search-for-records)

#### [!UICONTROL 清單記錄]

此搜索模組將檢索與搜索查詢匹配的特定類型的所有項目

您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Jira Software] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL記錄類型]</td> 
   <td> <p>選擇要列出模組的記錄類型。 選取記錄類型時，該記錄類型的其他特定欄位會出現在模組中。</p> 
    <ul> 
     <li>[!UICONTROL注釋]</li> 
     <li>[!UICONTROL問題]</li> 
     <li>[!UICONTROL項目]</li> 
     <li>[!UICONTROL Sprint問題]</li> 
     <li>[!UICONTROL工作日誌]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL最大結果]</p> </td> 
   <td> <p>輸入或映射您希望模組在每個方案執行週期中檢索的最大記錄數。</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Offset</td> 
    <td> Enter or map the ID of the first item you want to retrieve details for. This is a way to paginate the records. If you enter the 5000th item as the offset, the module would return items 5000-9999.</td> 
   </tr>
  --> 
 </tbody> 
</table>

#### [!UICONTROL 搜索記錄]

此搜尋模組會在 [!DNL Jira Software] 符合您指定的搜尋查詢。

您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Jira Software] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL記錄類型]</td> 
   <td> <p>選擇要模組搜索的記錄類型。 選取記錄類型時，該記錄類型的其他特定欄位會出現在模組中。</p> 
    <ul> 
     <li>[!UICONTROL問題]</li> 
     <li> <p>[!JQL的UICONTROL問題（Jira查詢語言）] </p> <p>有關JQL的詳細資訊，請參見 <a href="https://www.atlassian.com/blog/jira-software/jql-the-most-flexible-way-to-search-jira-14#:~:text=JQLstandsforJiraQuery,projectmanagers%2Candbusinessusers.">JQL</a> 在Atlassian幫助站點。 </p> </li> 
     <li>[!UICONTROL項目]</li> 
     <li>[!UICONTROL項目（按問題）]</li> 
     <li>[!UICONTROL用戶]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
