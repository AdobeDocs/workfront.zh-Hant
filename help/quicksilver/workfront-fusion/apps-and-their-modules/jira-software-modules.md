---
title: Jira軟體模組
description: 在 [!DNL Adobe Workfront Fusion] 情境下，您可以自動化使用下列專案的工作流程： [!DNL Jira] 軟體，以及連線到多個協力廠商的應用程式和服務。
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 6437fe98-2c2b-4b49-97e2-f94b23da93fd
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '2085'
ht-degree: 1%

---

# [!DNL Jira Software] 模組

在 [!DNL Adobe Workfront Fusion] 情境下，您可以自動化使用下列專案的工作流程： [!DNL Jira Software]，以及將其連線到多個協力廠商應用程式和服務。

如果您需要建立案例的說明，請參閱 [在中建立情境 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

如需模組的相關資訊，請參閱 [中的模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

<!-- Bob Fix this compared to original -->

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td>
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
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 計畫，您的組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 計畫。</p>
   <p>或</p>
   <p>舊版產品需求：貴組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有哪些計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

有關以下專案的資訊： [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 必要條件

使用 [!DNL Jira] 模組必須有 [!DNL Jira] 帳戶。

## Connect [!DNL Jira Software] 至 [!DNL Workfront Fusion]

您的連線方法取決於您是否使用 [!DNL Jira Cloud] 或 [!DNL Jira Server].

* [Connect [!DNL Jira Cloud] 至Workfront Fusion](#connect-jira-cloud-to-workfront-fusion)
* [Connect [!DNL Jira Server] 至 [!DNL Workfront Fusion]](#connect-jira-server-to-workfront-fusion)

### Connect [!DNL Jira Cloud] 至 [!DNL Workfront Fusion]

Connect [!DNL Jira Cloud] 至 [!DNL Workfront Fusion]

若要連線 [!DNL Jira Software] 至 [!DNL Workfront Fusion]，您必須建立API權杖，並將其與服務URL和使用者名稱一起插入 [!UICONTROL 建立連線] 中的欄位 [!DNL Workfront Fusion].

#### 在中建立API權杖 [!DNL Jira]

1. 前往 [https://id.atlassian.com/manage/api-tokens](https://id.atlassian.com/manage/api-tokens) 並登入。
1. 按一下 **[!UICONTROL 建立API權杖]**.
1. 輸入權杖的名稱，例如 *Workfront Fusion*.
1. 使用複製權杖 **[!UICONTROL 複製到剪貼簿]** 按鈕。

   >[!IMPORTANT]
   >
   >關閉此對話方塊後，您無法再次檢視權杖。
1. 將產生的Token儲存在安全的地方。
1. 繼續使用 [設定 [!DNL Jira] 中的API權杖 [!DNL Workfront Fusion]](#configure-the-jira-api-token-in-workfront-fusion).

#### 設定 [!DNL Jira] 中的API權杖 [!DNL Workfront Fusion]

1. 在 [!DNL Workfront Fusion]，新增 [!DNL Jira] 模組至情境，以開啟 **[!UICONTROL 建立連線]** 方塊。
1. 指定下列資訊：

   * **[!UICONTROL 服務URL]**
   * **[!UICONTROL 使用者名稱]**
   * **[!UICONTROL API權杖]：** 這是您在中建立的API權杖 [在中建立API權杖 [!DNL Jira]](#create-an-api-token-in-jira) 章節。

1. 按一下 [!UICONTROL 繼續] 以建立連線並返回模組。

### Connect [!DNL Jira Server] 至 [!DNL Workfront Fusion]

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Becky: Find out and document how to find these things</p>
-->

若要授權兩者之間的連線 [!DNL Workfront Fusion] 和 [!DNL Jira Server]，您需要消費者金鑰、私密金鑰和服務URL。 您可能需要聯絡 [!DNL Jira] 管理員以取得此資訊。

* [為您的產生公開和私密金鑰 [!DNL Jira] 連線](#generate-public-and-private-keys-for-your-jira-connection)
* [將使用者端應用程式設定為中的消費者 [!DNL Jira]](#configure-the-client-app-as-a-consumer-in-jira)
* [建立與的連線 [!DNL Jira] 中的伺服器或Jira資料中心 [!DNL Workfront Fusion]](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion)

#### 為您的產生公開和私密金鑰 [!DNL Jira] 連線

取得您的私密金鑰 [!DNL Workfront Fusion Jira] 連線，您需要產生公開和私密金鑰。

1. 在終端機中，執行下列動作 `openssl` 命令。

   * `openssl genrsa -out jira_privatekey.pem 1024`

     這個指令會產生1024位元私密金鑰。

   * `openssl req -newkey rsa:1024 -x509 -key jira_privatekey.pem -out jira_publickey.cer -days 365`

     這個命令會建立X509憑證。

   * `openssl pkcs8 -topk8 -nocrypt -in jira_privatekey.pem -out jira_privatekey.pcks8`

     此命令會將私密金鑰（PKCS8格式）擷取到 `jira_privatekey.pcks8`
檔案。

   * `openssl x509 -pubkey -noout -in jira_publickey.cer  > jira_publickey.pem`

     此命令會從憑證擷取公開金鑰至 `jira_publickey.pem` 檔案。

     >[!NOTE]
     >
     >如果您使用的是Windows，您可能需要將公開金鑰儲存至 `jira_publickey.pem` 手動檔案：
     >
     >1. 在終端機中，執行下列命令：
     >   
     >   `openssl x509 -pubkey -noout -in jira_publickey.cer`
     >   
     >1. 複製終端機輸出(包括 `-------BEGIN PUBLIC KEY--------` 和 `-------END PUBLIC KEY--------`
     >   
     >1. 將終端機輸出貼到名為的檔案中 `jira_publickey.pem`.


1. 繼續至 [將使用者端應用程式設定為中的消費者 [!DNL Jira]](#configure-the-client-app-as-a-consumer-in-jira)

#### 將使用者端應用程式設定為中的消費者 [!DNL Jira]

1. 登入您的 [!DNL Jira] 執行個體。
1. 在左側導覽面板中，按一下 **[!UICONTROL [!DNL Jira]設定]** ![](assets/jira-settings-icon.png) > **[!UICONTROL 應用]**> **[!UICONTROL 應用程式連結]**.
1. 在 **[!UICONTROL 輸入您要連結之應用程式的URL]** 欄位，輸入

   ```
   https://app.workfrontfusion.com/oauth/cb/workfront-jiraserver-oauth1
   ```

1. 按一下 **[!UICONTROL 建立新連結]**. 忽略「沒有從您輸入的URL收到回應」錯誤訊息。
1. 在 **[!UICONTROL 連結應用計畫]** 視窗中，輸入值至 **[!UICONTROL 使用者金鑰]** 和 **[!UICONTROL 共用機密]** 欄位。

   您可以為這些欄位選擇值。

1. 複製以下專案的值： **[!UICONTROL 使用者金鑰]** 和 **[!UICONTROL 共用機密]** 欄位至安全位置。

   您稍後在設定程式中會需要這些值。

1. 填寫URL欄位，如下所示：

   | 欄位 | 說明 |
   |---|---|
   | [!UICONTROL 請求權杖URL] | `<Jira base url>/plugins/servlet/oauth/request-token` |
   | [!UICONTROL 授權URL] | `<Jira base url>/plugins/servlet/oauth/authorize` |
   | [!UICONTROL 存取權杖URL] | `<Jira base url>/plugins/servlet/oauth/access-token` |

1. 選取 **[!UICONTROL 建立傳入連結]** 核取方塊。
1. 按一下 **[!UICONTROL 繼續]**.
1. 在 **[!UICONTROL 連結應用計畫]** 視窗中，填寫下列欄位：

   <table style="table-layout:auto"> 
    <col data-mc-conditions=""> 
    <col data-mc-conditions=""> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[！UICONTROL使用者金鑰]</p> </td> 
      <td> 將您複製至安全位置的消費者金鑰貼上。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL消費者名稱]</td> 
      <td>輸入您選擇的名稱。 此名稱僅供您參考。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL公開金鑰]</td> 
      <td>從您的電腦貼上公開金鑰 <code>[!DNL jira_publickey.pem]</code> 檔案。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **[!UICONTROL 繼續]**.
1. 繼續至 [建立與的連線 [!DNL Jira Server] 或 [!DNL Jira Data Center] 在 [!DNL Workfront Fusion]](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion)

#### 建立與的連線 [!DNL Jira Server] 或 [!DNL Jira Data Center] 在 [!DNL Workfront Fusion]

>[!NOTE]
>
>使用 [!DNL Jira Server] 要連線的應用程式 [!DNL Jira Server] 或 [!DNL Jira Data Center].
1. 在任何 [!DNL Jira Server] 中的模組 [!DNL Workfront Fusion]，按一下 **[!UICONTROL 新增]** 旁邊 [!UICONTROL 連線] 欄位。
1. 在 [!UICONTROL 建立連線] 填入下列欄位：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[！UICONTROL連線名稱]</p> </td> 
      <td> <p>輸入連線的名稱</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL使用者金鑰]</td> 
      <td>貼入您複製至中安全位置的消費者金鑰 <a href="#configure-the-client-app-as-a-consumer-in-jira" class="MCXref xref">將使用者端應用程式設定為中的消費者 [!DNL Jira]</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Private Key]</td> 
      <td>從貼入私密金鑰 <code>[!DNL jira_privatekey.pcks8]</code> 您在中建立的檔案 <a href="#generate-public-and-private-keys-for-your-jira-connection" class="MCXref xref">為您的產生公開和私密金鑰 [!DNL Jira] 連線</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Service URL]</td> 
      <td>輸入您的 [!DNL Jira] 執行個體URL。 </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **[!UICONTROL 繼續]** 以建立連線並返回模組。

## [!DNL Jira Software] 模組及其欄位

當您設定 [!DNL Jira Software] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 除了這些以外， [!DNL Jira Software] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應至中的另一個模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

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
   <td role="rowheader">[！UICONTROL Webhook]</td> 
   <td> <p>選取您要用來監視記錄的webhook。 </p> <p>若要新增新的webhook：</p> 
    <ol> 
     <li value="1">按一下 <strong>[！UICONTROL新增]</strong></li> 
     <li value="2">輸入webhook的名稱。</li> 
     <li value="3"> <p>選取您要用於webhook的連線。 </p> <p>如需有關連線您的電腦的指示， [!DNL Jira Software] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </li> 
     <li value="4"> <p>選取您要軟體監視的記錄型別：</p> 
      <ul> 
       <li>[！UICONTROL註解] </li> 
       <li>[！UICONTROL問題]</li> 
       <li>[！UICONTROL專案] </li> 
       <li>[！UICONTROL Sprint]</li> 
      </ul> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### 動作

* [[!UICONTROL 新增問題至衝刺(sprint)]](#add-issue-to-sprint)
* [[!UICONTROL 自訂API呼叫]](#custom-api-call)
* [[!UICONTROL 建立記錄]](#create-a-record)
* [[!UICONTROL 刪除記錄]](#delete-a-record)
* [[!UICONTROL 下載附件]](#download-an-attachment)
* [[!UICONTROL 讀取記錄]](#read-a-record)
* [[!UICONTROL 更新記錄]](#update-a-record)

#### [!UICONTROL 新增問題至衝刺(sprint)]

此動作模組會將一或多個問題新增至衝刺。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Jira Software] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Sprint ID]</td> 
   <td>輸入或對應您想要新增問題的衝刺(sprint)的Sprint ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL問題ID或金鑰]</td> 
   <td>針對您想要新增至衝刺的每個問題，新增問題ID或金鑰。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立記錄]

此動作模組會在Jira中建立新記錄。

模組會傳回與記錄相關聯的任何標準欄位，以及連線存取的任何自訂欄位和值。 您可以將此資訊對應到情境中的後續模組中。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Jira Software] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別]</td> 
   <td> <p>選取您要模組建立的記錄型別。 當您選取記錄型別時，該記錄型別專屬的其他欄位會出現在模組中。</p> 
    <ul> 
     <li>[！UICONTROL附件]</li> 
     <li>[！UICONTROL註解]</li> 
     <li>[！UICONTROL問題]</li> 
     <li>[！UICONTROL專案]</li> 
     <li>[！UICONTROL Sprint] </li> 
     <li>[！UICONTROL工作記錄檔]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 自訂API呼叫]

此動作模組可讓您對 [!DNL Jira Software] API。 如此一來，您就可以建立其他人無法完成的資料流程自動化 [!DNL Jira Software] 模組。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Jira Software] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL URL]</td> 
   <td>輸入相對於<code>&lt;Instance URL>/rest/api/2/ </code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL方法]</td> 
   td&gt; <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL標頭]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標頭。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 為您新增授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查詢字串]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的查詢。</p> <p>例如： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL內文]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的正文內容。</p> <p>備註:  <p>使用條件陳述式時，例如 <code>if</code> 在JSON中，將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除記錄]

此動作模組會刪除特定記錄。

您指定記錄的ID。

模組會傳回記錄ID和任何關聯欄位，以及連線存取的任何自訂欄位和值。 您可以將此資訊對應到情境中的後續模組中。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Jira Software] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別]</td> 
   <td> <p>選取您要模組刪除的記錄型別。 </p> 
    <ul> 
     <li>[！UICONTROL附件]</li> 
     <li>[！UICONTROL註解]</li> 
     <li>[！UICONTROL問題]</li> 
     <li>[！UICONTROL專案]</li> 
     <li>[！UICONTROL Sprint] </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL ID或金鑰]</td> 
   <td>輸入或對應您要刪除之記錄的ID或金鑰。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 下載附件]

此動作模組會下載特定附件。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Jira Software] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL ID]</td> 
   <td>輸入或對應您要下載之附件的ID。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 讀取記錄]

此動作模組會從中的單一記錄讀取資料 [!DNL Jira Software].

您指定記錄的ID。

模組會傳回與記錄相關聯的任何標準欄位，以及連線存取的任何自訂欄位和值。 您可以將此資訊對應到情境中的後續模組中。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Jira Software] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別]</td> 
   <td> <p>選取型別 [!DNL Jira] 您希望模組讀取的記錄。</p> 
    <ul> 
     <li>[！UICONTROL附件]</li> 
     <li>[！UICONTROL問題]</li> 
     <li>[！UICONTROL專案]</li> 
     <li>[！UICONTROL Sprint] </li> 
     <li>[！UICONTROL使用者]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸出]</td> 
   <td>選取您要接收的輸出。 根據「[！UICONTROL記錄型別]」欄位中選取的記錄型別，可使用輸出選項。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL ID]</td> 
   <td> <p>輸入或對映唯一的 [!DNL Jira Software] 您希望模組讀取的記錄ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新記錄]

此動作模組會更新現有記錄，例如問題或專案。

您指定記錄的ID。

模組會傳回記錄ID和任何關聯欄位，以及連線存取的任何自訂欄位和值。 您可以將此資訊對應到情境中的後續模組中。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Jira Software] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別]</td> 
   <td> <p>選取您要模組更新的記錄型別。 當您選取記錄型別時，該記錄型別專屬的其他欄位會出現在模組中。</p> 
    <ul> 
     <li>[！UICONTROL註解]</li> 
     <li>[！UICONTROL問題]</li> 
     <li>[！UICONTROL專案]</li> 
     <li>[！UICONTROL Sprint] </li> 
     <li>[！UICONTROL轉換問題]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL ID或金鑰]</td> 
   <td>輸入或對應您要更新的記錄ID或金鑰。</td> 
  </tr> 
 </tbody> 
</table>

### 搜尋

* [[!UICONTROL 清單記錄]](#list-records)
* [[!UICONTROL 搜尋記錄]](#search-for-records)

#### [!UICONTROL 清單記錄]

此搜尋模組會擷取符合您的搜尋查詢的特定型別的所有專案

您可以將此資訊對應到情境中的後續模組中。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Jira Software] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別]</td> 
   <td> <p>選取您要模組列出的記錄型別。 當您選取記錄型別時，該記錄型別專屬的其他欄位會出現在模組中。</p> 
    <ul> 
     <li>[！UICONTROL註解]</li> 
     <li>[！UICONTROL問題]</li> 
     <li>[！UICONTROL專案]</li> 
     <li>[！UICONTROL Sprint問題]</li> 
     <li>[！UICONTROL工作記錄檔]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL最大結果]</p> </td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期中擷取的記錄數上限。</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Offset</td> 
    <td> Enter or map the ID of the first item you want to retrieve details for. This is a way to paginate the records. If you enter the 5000th item as the offset, the module would return items 5000-9999.</td> 
   </tr>
  --> 
 </tbody> 
</table>

#### [!UICONTROL 搜尋記錄]

此搜尋模組會在中尋找物件中的記錄 [!DNL Jira Software] 符合您指定的搜尋查詢。

您可以將此資訊對應到情境中的後續模組中。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL連線]</td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Jira Software] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Connect [!DNL Jira Software] 至 [!DNL Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別]</td> 
   <td> <p>選取您要模組搜尋的記錄型別。 當您選取記錄型別時，該記錄型別專屬的其他欄位會出現在模組中。</p> 
    <ul> 
     <li>[！UICONTROL問題]</li> 
     <li> <p>[！UICONTROL Issues by JQL （Jira查詢語言）] </p> <p>如需JQL的詳細資訊，請參閱 <a href="https://www.atlassian.com/blog/jira-software/jql-the-most-flexible-way-to-search-jira-14#:~:text=JQLstandsforJiraQuery,projectmanagers%2Candbusinessusers.">JQL</a> 在Atlassian說明網站。 </p> </li> 
     <li>[！UICONTROL專案]</li> 
     <li>[！UICONTROL專案（按問題）</li> 
     <li>[！UICONTROL使用者]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
