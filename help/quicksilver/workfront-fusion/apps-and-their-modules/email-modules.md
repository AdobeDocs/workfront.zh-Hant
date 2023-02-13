---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 連接器
navigation-topic: apps-and-their-modules
title: 電子郵件模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以將電子郵件帳戶連接到多個第三方應用程式和服務。這允許您通過IMAP下載電子郵件、通過SMTP發送電子郵件、建立新草稿、將電子郵件從一個資料夾移動並複製到另一個資料夾、將電子郵件標籤為已讀或未讀，以及刪除電子郵件。
author: Becky
feature: Workfront Fusion
exl-id: 384ba60a-d79e-4126-a247-6d67b5154ede
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2613'
ht-degree: 0%

---

# 電子郵件模組

在 [!DNL Adobe Workfront Fusion] 案例中，您可以將電子郵件帳戶連接到多個第三方應用程式和服務。這允許您通過IMAP下載電子郵件、通過SMTP發送電子郵件、建立新草稿、將電子郵件從一個資料夾移動並複製到另一個資料夾、將電子郵件標籤為已讀或未讀，以及刪除電子郵件。

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

## 將您的電子郵件連結至Workfront Fusion {#connect-your-email-to-workfront-fusion}

* [連線至Google](#connect-to-google)
* [連線至其他電子郵件服務(SMAP)](#connect-to-other-email-services-smap)

### 連線至 [!DNL Google]

使用此選項建立具有需要與您的 [!DNL Google] 帳戶。 這是一個有受限範圍的帳戶。

您可以建立與 [!DNL Google] 帳戶（直接從電子郵件模組內）。

1. 在任何電子郵件模組中，按一下 **[!UICONTROL 新增]** 旁邊 [!UICONTROL 連線] 欄位。
1. 選擇 **[!DNL Google]** 作為連接類型。
1. 輸入連線的名稱。
1. （選用）輸入 [!UICONTROL [!DNL Google] 用戶端ID] 和 [!UICONTROL 用戶端密碼].
1. 按一下 **[!UICONTROL 繼續]** 若要建立連線，請返回模組。

### 連線至其他電子郵件服務(SMAP)

SMAP連接允許您遠程訪問郵箱以及讀取或操作郵箱中的郵件。 SMAP連線供大部分的電子郵件模組使用。

1. 在任何電子郵件模組中，按一下 **[!UICONTROL 新增]** 旁邊 [!UICONTROL 連線] 欄位。
1. 選擇 **[!UICONTROL 其他(SMTP)]** 作為連接類型。
1. 輸入 **[!UICONTROL 名稱]** 連線。
1. 選取 **[!UICONTROL 電子郵件提供者]** 從清單中。 如果您的電子郵件提供者不在清單中，請選取「其他」。
1. 輸入 **[!UICONTROL 電子郵件地址]**, **[!UICONTROL 您的全名]**，您的 **[!UICONTROL 使用者名稱]**，和 **[!UICONTROL 密碼]**.
1. （條件性）如果您的提供者不在清單中，請輸入 **[!UICONTROL SMTP伺服器]** 和 **[!UICONTROL 埠]**，並指定您是否 **[!UICONTROL 使用安全連線(TLS)]**. 若要尋找此資訊，請檢查 [!UICONTROL 說明] 區段。 如果您沒有此資訊可用，請聯絡您的電子郵件服務提供者。
1. 按一下 **[!UICONTROL 繼續]** 若要建立連線，請返回模組。

## [!UICONTROL 電子郵件] 模組及其欄位

設定時 [!UICONTROL 電子郵件] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 除了這些欄位，還可能會根據應用程式或服務中的存取層級等因素顯示其他欄位。 模組中的粗體標題表示必填欄位。

有些電子郵件欄位可能已包含資料，因為您已在案例的其他模組中使用這些欄位。 如果您需要相關資訊，請參閱電子郵件說明檔案。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

>[!NOTE]
>
>唯一電子郵件ID稱為「[!UICONTROL 電子郵件ID(UID)]&#39;是電子郵件的識別碼。 電子郵件ID是每個電子郵件資料夾的專屬ID。

* [觸發器](#triggers)
* [動作](#actions)
* [迭代器](#iterators)

### 觸發器

#### [!UICONTROL 觀看電子郵件]

收到新電子郵件以根據指定條件進行處理時觸發。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>如需將您的電子郵件帳戶連結至[!UICONTROL Workfront Fusion]的指示，請參閱 <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">將您的電子郵件連結至[!UICONTROL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資料夾] </td> 
   <td> <p>選取包含您要監看之電子郵件的資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL條件]</p> </td> 
   <td> <p>選取您要透過哪個條件來監看電子郵件：</p> 
    <ul> 
     <li>[!UICONTROL所有電子郵件]</li> 
     <li>[!UICONTROL僅讀電子郵件]</li> 
     <li>[!UICONTROL僅未讀電子郵件]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL發件人電子郵件地址] </td> 
   <td> <p>輸入要監視其電子郵件的發件人的電子郵件地址。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL收件人電子郵件地址]</td> 
   <td> <p> 輸入您要監視其電子郵件的收件人的電子郵件地址。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主題] </td> 
   <td> <p>輸入您要觀看的電子郵件主旨。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL短語] </td> 
   <td> <p>輸入任何關鍵字以僅監視那些包含特定片語的電子郵件。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL將郵件標籤為讀取時讀取]</td> 
   <td> <p>啟用此選項，可在擷取詳細資料後，將未讀電子郵件標示為已讀。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL結果的最大數]</td> 
   <td> <p> 電子郵件數上限 [!DNL Workfront Fusion] 應會在一個案例執行週期期間傳回。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 動作

* [[!UICONTROL 傳送電子郵件]](#send-an-email)
* [[!UICONTROL 建立草稿]](#create-a-draft)
* [[!UICONTROL 將電子郵件標示為已讀取]](#mark-an-email-as-read)
* [[!UICONTROL 將電子郵件標示為未讀]](#mark-an-email-as-unread)
* [[!UICONTROL 移動電子郵件]](#move-an-email)
* [[!UICONTROL 複製電子郵件]](#copy-an-email)
* [[!UICONTROL 刪除電子郵件]](#delete-an-email)
* [[!UICONTROL 取得電子郵件]](#get-emails)
* [[!UICONTROL 傳送電子郵件給我]](#send-me-an-email)

#### [!UICONTROL 傳送電子郵件]

傳送新電子郵件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關將您的電子郵件帳戶連接到 [!DNL Workfront Fusion]，請參閱 <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">將您的電子郵件連結至[!UICONTROL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL在發送後保存消息]</td> 
   <td>電子郵件訊息傳送後，會儲存在您的信箱中。 如果您想要儲存使用 [!DNL Workfront Fusion] 到 <i>[!UICONTROL已發送郵件]</i> 檔案夾或郵箱中的其他檔案夾。 某些電子郵件服務，例如 [!DNL Gmail]，自動儲存已傳送的訊息。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL To] </td> 
   <td> <p>新增您要傳送電子郵件的電子郵件地址。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主題] </td> 
   <td> <p>輸入或對應電子郵件的主旨行。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL內容類型]</p> </td> 
   <td> <p>選取電子郵件的[!UICONTROL content]類型：</p> 
    <ul> 
     <li>HTML</li> 
     <li>[!UICONTROL Plaintext]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL內容] </td> 
   <td> <p>根據您在[!UICONTROL內容類型]欄位中選擇的內容，使用HTML標籤或純文字輸入或映射HTML格式的電子郵件內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL附件]</p> </td> 
   <td> <p>添加附件：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL檔案名]</strong> </p> <p>輸入檔案名。 例如，sample.doc。</p> </li> 
     <li> <p><strong>[!UICONTROL資料]</strong> </p> <p>輸入要上傳附件的資料夾路徑。</p> </li> 
     <li> <p><strong>[!UICONTROL Content-ID]</strong> </p> <p>輸入[!UICONTROL內容ID]以在內容中插入附件（影像）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL複製收件人] </td> 
   <td> <p>輸入或映射要向其發送此電子郵件副本的一個或多個電子郵件地址。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL盲副本收件人]</td> 
   <td> <p> 輸入或對應一或多個電子郵件地址，以便將此電子郵件的副本發送到這些電子郵件地址，而不讓電子郵件中顯示該電子郵件地址。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL從] </td> 
   <td> <p>輸入或對應出現在電子郵件中[!UICONTROL From]欄位中的電子郵件地址（如有需要，請輸入或對應名稱）。 </p> <p>重要：使用正確的語法： <code>name@email.com</code> 或 <code>"Name" name@email.com</code>.</p> <p>注意：通常， [!DNL Workfront Fusion] 使用您在建立連線時輸入的電子郵件地址做為寄件者地址。 如果您輸入任何其他電子郵件地址，則在傳送訊息時可能會發生錯誤，因為您的帳戶可能沒有從您自己的不同地址傳送電子郵件的權限。 例如 <code>test@mail.com</code> 或<code>John Bush" test@email.com</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL發件人]</p> </td> 
   <td> <p>輸入或對應電子郵件中[!UICONTROL寄件者]欄位中顯示的電子郵件地址。</p> <p>提示：如果您不確定要使用此欄位還是「從」欄位，建議選擇「從」欄位。</p> <p>重要：使用正確的語法： <code>name@email.com</code> 或 <code>"Name" name@email.com</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL回復]</td> 
   <td> <p> 如果您想要將此電子郵件的回覆傳送至與「寄件者」地址不同的位址，請輸入您要回覆此電子郵件的電子郵件地址。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL回復]</td> 
   <td> <p> 如果您正在回覆特定電子郵件，請輸入或對應您回覆之電子郵件的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL引用] </td> 
   <td> <p>輸入線程中所有回復的消息ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL優先順序]</p> </td> 
   <td> <p>選取電子郵件的優先順序：</p> 
    <ul> 
     <li>[!UICONTROL高]</li> 
     <li>[!UICONTROL標準]</li> 
     <li>[!UICONTROL低]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL標題]</p> </td> 
   <td> <p>新增標題：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL密鑰]</strong> </p> <p>新增金鑰。 例如，[!UICONTROL發送者]、[!UICONTROL日期]、[!UICONTROL目標]等。</p> </li> 
     <li> <p><strong>[!UICONTROL值]</strong> </p> <p>輸入鍵的值。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立草稿]

建立新拔模並將其添加到選定資料夾。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>如需將您的電子郵件帳戶連結至[!UICONTROL Workfront Fusion]的指示，請參閱 <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">將您的電子郵件連結至[!UICONTROL Workfront Fusion]</a> 這篇文章。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資料夾]</td> 
   <td>選取您要建立草稿電子郵件的資料夾。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL To] </td> 
   <td> <p>輸入或對應您要傳送電子郵件的電子郵件地址。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主題] </td> 
   <td> <p>輸入或對應電子郵件的主旨行。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL內容類型]</p> </td> 
   <td> <p>選取電子郵件的內容類型：</p> 
    <ul> 
     <li>HTML</li> 
     <li>[!UICONTROL純文字檔案]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL內容] </td> 
   <td> <p>根據您在[!UICONTROL內容類型]欄位中選擇的內容，使用HTML標籤或純文字輸入或映射HTML格式的電子郵件內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL附件]</p> </td> 
   <td> <p>添加附件：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL檔案名]</strong> </p> <p>輸入檔案名。 例如，sample.doc。</p> </li> 
     <li> <p><strong>[!UICONTROL資料]</strong> </p> <p>輸入要上傳附件的資料夾路徑。</p> </li> 
     <li> <p><strong>[!UICONTROL Content-ID]</strong> </p> <p>輸入內容ID以在內容中插入附件（影像）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL複製收件人] </td> 
   <td> <p>輸入或映射要向其發送此電子郵件副本的一個或多個電子郵件地址。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL盲副本收件人]</td> 
   <td> <p> 輸入或對應一或多個電子郵件地址，以便將此電子郵件的副本發送到這些電子郵件地址，而不讓電子郵件中顯示該電子郵件地址。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL從] </td> 
   <td> <p>輸入或對應出現在電子郵件中[!UICONTROL From]欄位中的電子郵件地址（如有需要，請輸入或對應名稱）。 </p> <p>重要：使用正確的語法： <code>name@email.com</code> 或 <code>"Name" name@email.com</code>.</p> <p>注意：通常， [!DNL Workfront Fusion] 使用您在建立連線時輸入的電子郵件地址做為寄件者地址。 如果您輸入任何其他電子郵件地址，則在傳送訊息時可能會發生錯誤，因為您的帳戶可能沒有從您自己的不同地址傳送電子郵件的權限。 例如 <code>test@mail.com</code> 或<code>John Bush" test@email.com</code>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL發件人]</p> </td> 
   <td> <p>輸入或對應電子郵件中[!UICONTROL寄件者]欄位中顯示的電子郵件地址。</p> <p>提示：如果您不確定要使用此欄位還是「從」欄位，建議選擇「從」欄位。</p> <p>重要：使用正確的語法： <code>name@email.com</code> 或 <code>"Name" name@email.com</code></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL回復]</td> 
   <td> <p> 如果您希望將此電子郵件的回復發送到「[!UICONTROL from]」地址以外的其他地址，請輸入要向其發送此電子郵件的回復的電子郵件地址。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL回復]</td> 
   <td> <p> 如果您正在回覆特定電子郵件，請輸入或對應您回覆之電子郵件的ID。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL引用] </td> 
   <td> <p>輸入線程中所有回復的消息ID。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL優先順序]</p> </td> 
   <td> <p>選取電子郵件的優先順序：</p> 
    <ul> 
     <li>[!UICONTROL高]</li> 
     <li>[!UICONTROL標準]</li> 
     <li>[!UICONTROL低]</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL標題]</p> </td> 
   <td> <p>新增標題：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL密鑰]</strong> </p> <p>新增金鑰。 例如，「寄件者」、「日期」、「結束日期」等。</p> </li> 
     <li> <p><strong>[!UICONTROL值]</strong> </p> <p>輸入鍵的值。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 將電子郵件標示為已讀取]

在選取的資料夾中，將電子郵件或草稿標示為已讀取，方法是設定 [!UICONTROL 閱讀] 標籤。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>如需將您的電子郵件帳戶連結至[!UICONTROL Workfront Fusion]的指示，請參閱 <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">將您的電子郵件連結至[!UICONTROL Workfront Fusion]</a> 這篇文章。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資料夾]</td> 
   <td>選取您要標示為已讀取之電子郵件的資料夾。 範例：主要。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL電子郵件ID(UID)]</p> </td> 
   <td> <p>輸入您要標示為已讀取之電子郵件的電子郵件UID。</p> <p>您可以使用[!UICONTROL Email] &gt;[!UICONTROL Watch Email]模組或[!UICONTROL Search Email]模組來取得電子郵件的UID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 將電子郵件標示為未讀]

設定「未讀」標幟，將所選資料夾中的電子郵件或草稿標示為未讀。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>如需將您的電子郵件帳戶連結至[!UICONTROL Workfront Fusion]的指示，請參閱 <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">將您的電子郵件連結至[!UICONTROL Workfront Fusion]</a> 這篇文章。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資料夾]</td> 
   <td>選取您要標示為未讀的電子郵件資料夾。 範例：主要。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL電子郵件ID(UID)]</p> </td> 
   <td> <p>輸入要標籤為未讀的電子郵件的電子郵件UID。</p> <p>您可以使用[!UICONTROL Email] &gt;[!UICONTROL Watch Email]模組或[!UICONTROL Search Email]模組來取得電子郵件的UID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 移動電子郵件]

將選取的電子郵件或草稿移至選取的資料夾。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>如需將您的電子郵件帳戶連結至[!UICONTROL Workfront Fusion]的指示，請參閱 <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">將您的電子郵件連結至[!UICONTROL Workfront Fusion]</a> 這篇文章。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL源資料夾]</td> 
   <td>選取包含您要移動電子郵件之電子郵件的資料夾。 範例：主要。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL目標資料夾]</td> 
   <td> <p> 選取您要新增電子郵件的資料夾。 範例：工作。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL電子郵件ID(UID)]</p> </td> 
   <td> <p>輸入您要移至目的地資料夾之電子郵件的電子郵件UID。</p> <p>您可以使用[!UICONTROL Email] &gt;[!UICONTROL Watch Email]模組或[!UICONTROL Search Email]模組來取得電子郵件的UID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 複製電子郵件]

將電子郵件或草稿複製至選取的資料夾。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>如需將您的電子郵件帳戶連結至[!UICONTROL Workfront Fusion]的指示，請參閱 <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">將您的電子郵件連結至[!UICONTROL Workfront Fusion]</a> 這篇文章。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL源資料夾]</td> 
   <td>選取您要從中複製電子郵件的資料夾。 範例：主要。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL目標資料夾]</td> 
   <td> <p> 選取您要將電子郵件複製到的資料夾。 範例：工作。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL電子郵件ID(UID)]</p> </td> 
   <td> <p>輸入要複製到目標資料夾之電子郵件的電子郵件UID。</p> <p>您可以使用[!UICONTROL Email] &gt;[!UICONTROL Watch Email]模組或[!UICONTROL Search Email]模組來取得電子郵件的UID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除電子郵件]

從選取的資料夾移除電子郵件或草稿。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>如需將您的電子郵件帳戶連結至[!UICONTROL Workfront Fusion]的指示，請參閱 <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">將您的電子郵件連結至[!UICONTROL Workfront Fusion]</a> 這篇文章。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資料夾]</td> 
   <td>選取您要刪除之電子郵件的資料夾。 範例：主要。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL電子郵件ID(UID)]</p> </td> 
   <td> <p>輸入您要刪除之電子郵件的電子郵件UID。</p> <p>您可以使用[!UICONTROL Email] &gt;[!UICONTROL Watch Email]模組或[!UICONTROL Search Email]模組來取得電子郵件的UID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL擴展]</td> 
   <td> <p>啟用此選項可允許模組永久刪除當前開啟的郵箱中標籤為[!UICONTROL Deleted]的所有郵件。</p> <p>注意：在 [!DNL Gmail]，此行為是由[!UICONTROL設定] &gt;[!UICONTROL轉發POP/IMAP in IMAP access]部分中的設定驅動的。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得電子郵件]

傳回符合指定條件的電子郵件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>如需將您的電子郵件帳戶連結至[!UICONTROL Workfront Fusion]的指示，請參閱 <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">將您的電子郵件連結至[!UICONTROL Workfront Fusion]</a> 這篇文章。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資料夾] </td> 
   <td> <p>選取包含您要擷取之電子郵件的資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL將郵件標籤為讀取時讀取] </td> 
   <td> <p>如果您想在擷取詳細資料後，將未讀電子郵件標示為已讀，請啟用此選項。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL條件]</p> </td> 
   <td> <p>選取您要擷取之電子郵件的條件：</p> 
    <ul> 
     <li>[!UICONTROL所有電子郵件]</li> 
     <li>[!UICONTROL僅讀電子郵件]</li> 
     <li>[!UICONTROL僅未讀電子郵件]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL發件人電子郵件地址] </td> 
   <td> <p>輸入或映射要檢索其電子郵件的發件人的電子郵件地址。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL收件人電子郵件地址]</td> 
   <td> <p> 輸入或映射要檢索其電子郵件的收件人的電子郵件地址。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL開始日期] </td> 
   <td> <p>輸入或對應日期，以擷取在指定日期或之後處理的電子郵件。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL日期之前]</td> 
   <td> <p> 輸入或對應日期，以擷取在指定日期或之前處理的電子郵件。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主題] </td> 
   <td> <p>輸入或對應您要擷取之電子郵件的主旨。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL短語] </td> 
   <td> <p>輸入或對應任何關鍵字，以僅擷取包含特定片語的電子郵件。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL電子郵件ID(UID)]</td> 
   <td> <p> 輸入要檢索其詳細資訊的電子郵件的電子郵件ID(UID)。</p> <p>您可以透過 [!DNL Workfront Fusion]s[!UICONTROL Watch Email]模組或[!UICONTROL Search Email]模組。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL結果的最大數]</td> 
   <td> <p> 電子郵件數上限 [!DNL Workfront Fusion] 應會在一個案例執行週期期間傳回。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL即使模組未返回任何結果，仍繼續執行路由]</td> 
   <td> <p> 即使沒有返回任何結果，選擇是否繼續運行模組。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 傳送電子郵件給我]

傳送新電子郵件至您的電子郵件地址。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL主題] </td> 
   <td> <p>輸入或對應電子郵件的主旨行。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL內容] </td> 
   <td> <p>輸入電子郵件的內文。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 迭代器

#### [!UICONTROL 迭代附件]

逐個反覆收到附件。

電子郵件迭代程式模組可讓您個別管理電子郵件附件。 例如，您可以設定監視電子郵件，反覆查詢附件的電子郵件並接收警報。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL源模組]</td> 
   <td> <p>選取會輸出包含您要反覆查看之附件之電子郵件的模組。</p> </td> 
  </tr> 
 </tbody> 
</table>

如需迭代程式的詳細資訊，請參閱 [中的迭代器模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).
