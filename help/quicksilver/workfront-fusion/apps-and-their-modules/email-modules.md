---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: 電子郵件模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以將電子郵件帳戶連線至多個協力廠商應用程式和服務。這可讓您透過IMAP下載電子郵件、透過SMTP傳送電子郵件、建立新草稿、將電子郵件從一個資料夾移動及複製到另一個資料夾、將電子郵件標示為已讀取或未讀取，以及刪除電子郵件。
author: Becky
feature: Workfront Fusion
exl-id: 384ba60a-d79e-4126-a247-6d67b5154ede
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: tm+mt
source-wordcount: '2626'
ht-degree: 0%

---

# 電子郵件模組

在[!DNL Adobe Workfront Fusion]案例中，您可以將電子郵件帳戶連線至多個協力廠商應用程式和服務。這可讓您透過IMAP下載電子郵件、透過SMTP傳送電子郵件、建立新草稿、將電子郵件從一個資料夾移動及複製到另一個資料夾、將電子郵件標示為已讀取或未讀取，以及刪除電子郵件。

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

## 將電子郵件連線至Workfront Fusion {#connect-your-email-to-workfront-fusion}

* [連線至Google](#connect-to-google)
* [連線到其他電子郵件服務(SMAP)](#connect-to-other-email-services-smap)

### 連線到[!DNL Google]

使用此選項來建立需要連線至您[!DNL Google]帳戶的電子郵件模組的案例。 這是具有受限制範圍的帳戶。

您可以直接從電子郵件模組內建立與您的[!DNL Google]帳戶的連線。

1. 在任何電子郵件模組中，按一下[!UICONTROL 連線]欄位旁的&#x200B;**[!UICONTROL 新增]**。
1. 選取&#x200B;**[!DNL Google]**&#x200B;作為連線型別。
1. 輸入連線的名稱。
1. （選擇性）輸入您的[!UICONTROL [!DNL Google]使用者端識別碼]和[!UICONTROL 使用者端密碼]。
1. 按一下&#x200B;**[!UICONTROL 繼續]**&#x200B;以建立連線並返回模組。

### 連線到其他電子郵件服務(SMAP)

SMAP連線可讓您從遠端存取信箱，並讀取或操作信箱中的郵件。 大部分電子郵件模組都使用SMAP連線。

1. 在任何電子郵件模組中，按一下[!UICONTROL 連線]欄位旁的&#x200B;**[!UICONTROL 新增]**。
1. 選取&#x200B;**[!UICONTROL 其他(SMTP)]**&#x200B;做為連線型別。
1. 輸入連線的&#x200B;**[!UICONTROL 名稱]**。
1. 從清單中選取您的&#x200B;**[!UICONTROL 電子郵件提供者]**。 如果您的電子郵件提供者不在清單中，請選取[其他]。
1. 輸入您的&#x200B;**[!UICONTROL 電子郵件地址]**、**[!UICONTROL 全名]**、**[!UICONTROL 使用者名稱]**&#x200B;和&#x200B;**[!UICONTROL 密碼]**。
1. （視條件而定）如果您的提供者不在清單中，請輸入您的&#x200B;**[!UICONTROL SMTP伺服器]**&#x200B;和&#x200B;**[!UICONTROL 連線埠]**，並指定是否要&#x200B;**[!UICONTROL 使用安全連線(TLS)]**。 若要尋找此資訊，請檢視您信箱的[!UICONTROL 說明]區段。 如果您無法取得此資訊，請連絡您的電子郵件服務提供者。
1. 按一下&#x200B;**[!UICONTROL 繼續]**&#x200B;以建立連線並返回模組。

## [!UICONTROL 電子郵件]模組及其欄位

當您設定[!UICONTROL 電子郵件]模組時，[!DNL Workfront Fusion]會顯示下列欄位。 除了這些以外，其他欄位可能會顯示，端視您在應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

部分電子郵件欄位可能已包含資料，因為您已在情境中的另一個模組中使用這些資料。 如需相關資訊，請參閱電子郵件說明檔案。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中將資訊從一個模組對應到另一個模組。

![](assets/map-toggle-350x74.png)

>[!NOTE]
>
>稱為&#39;[!UICONTROL 電子郵件ID (UID)]&#39;的唯一電子郵件ID是電子郵件的識別碼。 電子郵件ID是每個電子郵件資料夾專屬的。

* [觸發器](#triggers)
* [動作](#actions)
* [迭代器](#iterators)

### 觸發器

#### [!UICONTROL 觀看電子郵件]

收到新電子郵件並根據指定條件進行處理時觸發。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的電子郵件帳戶連線到[！UICONTROL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">將您的電子郵件連線到[！UICONTROL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資料夾] </td> 
   <td> <p>選取包含您要觀看之電子郵件的資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL條件]</p> </td> 
   <td> <p>選取您想用來觀看電子郵件的條件：</p> 
    <ul> 
     <li>[！UICONTROL所有電子郵件]</li> 
     <li>[！UICONTROL僅讀取電子郵件]</li> 
     <li>[！UICONTROL Only未讀取電子郵件]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL寄件者電子郵件地址] </td> 
   <td> <p>輸入要監視其電子郵件的寄件者電子郵件地址。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[！UICONTROL收件者電子郵件地址]</td> 
   <td> <p> 輸入您要觀看其電子郵件的收件者的電子郵件地址。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL主旨] </td> 
   <td> <p>輸入您要觀看之電子郵件的主旨。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL片語] </td> 
   <td> <p>輸入任何關鍵字，以僅觀看包含特定短語的電子郵件。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL擷取時將訊息標示為已讀取]</td> 
   <td> <p>啟用此選項，在擷取詳細資料後將未讀取的電子郵件標示為已讀取。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL結果數量上限]</td> 
   <td> <p> 一個案例執行週期內應該傳回的最大電子郵件數量[!DNL Workfront Fusion]。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 動作

* [[!UICONTROL 傳送電子郵件]](#send-an-email)
* [[!UICONTROL 建立草稿]](#create-a-draft)
* [[!UICONTROL 將電子郵件標示為已讀取]](#mark-an-email-as-read)
* [[!UICONTROL 將電子郵件標示為未讀取]](#mark-an-email-as-unread)
* [[!UICONTROL 移動電子郵件]](#move-an-email)
* [[!UICONTROL 複製電子郵件]](#copy-an-email)
* [[!UICONTROL 刪除電子郵件]](#delete-an-email)
* [[!UICONTROL 取得電子郵件]](#get-emails)

#### [!UICONTROL 傳送電子郵件]

傳送新電子郵件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的電子郵件帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">將您的電子郵件連線到[！UICONTROL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL傳送後儲存訊息]</td> 
   <td>電子郵件傳送後，會儲存在您的信箱中。 若要將使用[!DNL Workfront Fusion]傳送的電子郵件儲存至<i>[！UICONTROL已傳送郵件]</i>資料夾或您信箱中的其他資料夾，請啟用此選項。 有些電子郵件服務（例如[!DNL Gmail]）會自動儲存已傳送的郵件。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL至] </td> 
   <td> <p>新增您要傳送電子郵件的收件者電子郵件地址。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL主旨] </td> 
   <td> <p>輸入或對映電子郵件的主旨列。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL內容型別]</p> </td> 
   <td> <p>選取電子郵件的[！UICONTROL內容]型別：</p> 
    <ul> 
     <li>HTML</li> 
     <li>[！UICONTROL純文字]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL內容] </td> 
   <td> <p>視您在[！UICONTROL內容型別]欄位中選擇的專案而定，使用HTML標籤以HTML格式或純文字輸入或對應電子郵件內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL附件]</p> </td> 
   <td> <p>新增附件：</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL檔案名稱]</strong> </p> <p>輸入檔案名稱。 例如，sample.doc。</p> </li> 
     <li> <p><strong>[！UICONTROL資料]</strong> </p> <p>輸入要上傳附件的資料夾路徑。</p> </li> 
     <li> <p><strong>[！UICONTROL Content-ID]</strong> </p> <p>輸入[！UICONTROL內容ID]以在內容中插入附件（影像）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL副本收件者] </td> 
   <td> <p>輸入或對應您要傳送此電子郵件復本的一或多個電子郵件地址。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL密件副本收件者]</td> 
   <td> <p> 輸入或對應您要傳送此電子郵件復本的一或多個電子郵件地址，而不需要將該電子郵件地址顯示在電子郵件中。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[！UICONTROL From] </td> 
   <td> <p>輸入或對應電子郵件中[！UICONTROL寄件者]欄位中所顯示的電子郵件地址（和名稱，如有需要）。 </p> <p>重要：使用正確的語法： <code>name@email.com</code>或<code>"Name" name@email.com</code>。</p> <p>注意：通常，[!DNL Workfront Fusion]會使用您在建立連線時輸入的電子郵件地址作為寄件者地址。 如果您輸入任何其他電子郵件地址，傳送郵件時可能會發生錯誤，因為您的帳戶可能沒有許可權，無法從您自己的其他地址傳送電子郵件。 例如<code>test@mail.com</code>或''<code>John Bush" test@email.com</code>'。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL寄件者]</p> </td> 
   <td> <p>輸入或對應出現在電子郵件之[！UICONTROL Sender]欄位中的電子郵件地址。</p> <p>提示：如果您不確定要使用此欄位還是從欄位，我們建議您選擇從欄位。</p> <p>重要：使用正確的語法： <code>name@email.com</code>或 <code>"Name" name@email.com</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL回覆]</td> 
   <td> <p> 如果您要將此電子郵件的回覆傳送至「寄件者」地址以外的其他地址，請輸入您要傳送此電子郵件回覆的電子郵件地址。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL In-Reply-To]</td> 
   <td> <p> 如果您要回覆特定電子郵件，請輸入或對應您要回覆之電子郵件的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL參考] </td> 
   <td> <p>輸入對話串中所有回覆的訊息ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL優先順序]</p> </td> 
   <td> <p>選取電子郵件的優先順序：</p> 
    <ul> 
     <li>[！UICONTROL高]</li> 
     <li>[！UICONTROL Normal]</li> 
     <li>[！UICONTROL低]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Headers]</p> </td> 
   <td> <p>新增標題：</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL索引鍵]</strong> </p> <p>新增金鑰。 例如[！UICONTROL Sender]、[！UICONTROL Date]、[！UICONTROL To]等。</p> </li> 
     <li> <p><strong>[！UICONTROL值]</strong> </p> <p>輸入索引鍵的值。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立草稿]

建立新草稿並將其新增至選取的資料夾。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的電子郵件帳戶連線到[！UICONTROL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">將您的電子郵件連線到[！UICONTROL Workfront Fusion]</a>。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資料夾]</td> 
   <td>選取您要建立草稿電子郵件的資料夾。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL至] </td> 
   <td> <p>輸入或對應您要傳送電子郵件的電子郵件地址。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL主旨] </td> 
   <td> <p>輸入或對映電子郵件的主旨列。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[！UICONTROL內容型別]</p> </td> 
   <td> <p>選取電子郵件的內容型別：</p> 
    <ul> 
     <li>HTML</li> 
     <li>[！UICONTROL純文字]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL內容] </td> 
   <td> <p>視您在[！UICONTROL內容型別]欄位中選擇的專案而定，使用HTML標籤以HTML格式或純文字輸入或對應電子郵件內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL附件]</p> </td> 
   <td> <p>新增附件：</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL檔案名稱]</strong> </p> <p>輸入檔案名稱。 例如，sample.doc。</p> </li> 
     <li> <p><strong>[！UICONTROL資料]</strong> </p> <p>輸入要上傳附件的資料夾路徑。</p> </li> 
     <li> <p><strong>[！UICONTROL Content-ID]</strong> </p> <p>輸入內容ID以在內容中插入附件（影像）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL副本收件者] </td> 
   <td> <p>輸入或對應您要傳送此電子郵件復本的一或多個電子郵件地址。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL密件副本收件者]</td> 
   <td> <p> 輸入或對應您要傳送此電子郵件復本的一或多個電子郵件地址，而不需要將該電子郵件地址顯示在電子郵件中。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[！UICONTROL From] </td> 
   <td> <p>輸入或對應電子郵件中[！UICONTROL寄件者]欄位中所顯示的電子郵件地址（和名稱，如有需要）。 </p> <p>重要：使用正確的語法： <code>name@email.com</code>或<code>"Name" name@email.com</code>。</p> <p>注意：通常，[!DNL Workfront Fusion]會使用您在建立連線時輸入的電子郵件地址作為寄件者地址。 如果您輸入任何其他電子郵件地址，傳送郵件時可能會發生錯誤，因為您的帳戶可能沒有許可權，無法從您自己的其他地址傳送電子郵件。 例如<code>test@mail.com</code>或''<code>John Bush" test@email.com</code>'。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[！UICONTROL寄件者]</p> </td> 
   <td> <p>輸入或對應出現在電子郵件之[！UICONTROL Sender]欄位中的電子郵件地址。</p> <p>提示：如果您不確定要使用此欄位還是從欄位，我們建議您選擇從欄位。</p> <p>重要：使用正確的語法： <code>name@email.com</code>或 <code>"Name" name@email.com</code></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[！UICONTROL回覆]</td> 
   <td> <p> 如果您要將此電子郵件的回覆傳送至「[！UICONTROL from]」地址以外的其他地址，請輸入您要傳送此電子郵件的回覆的電子郵件地址。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[！UICONTROL In-Reply-To]</td> 
   <td> <p> 如果您要回覆特定電子郵件，請輸入或對應您要回覆之電子郵件的ID。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[！UICONTROL參考] </td> 
   <td> <p>輸入對話串中所有回覆的訊息ID。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[！UICONTROL優先順序]</p> </td> 
   <td> <p>選取電子郵件的優先順序：</p> 
    <ul> 
     <li>[！UICONTROL高]</li> 
     <li>[！UICONTROL Normal]</li> 
     <li>[！UICONTROL低]</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[！UICONTROL Headers]</p> </td> 
   <td> <p>新增標題：</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL索引鍵]</strong> </p> <p>新增金鑰。 例如，「寄件者」、「日期」、「收件者」等。</p> </li> 
     <li> <p><strong>[！UICONTROL值]</strong> </p> <p>輸入索引鍵的值。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 將電子郵件標示為已讀取]

設定[!UICONTROL 讀取]旗標，將選取資料夾中的電子郵件或草稿標示為已讀取。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的電子郵件帳戶連線到[！UICONTROL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">將您的電子郵件連線到[！UICONTROL Workfront Fusion]</a>。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資料夾]</td> 
   <td>選取您要標示為已讀取的電子郵件資料夾。 範例： Primary。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL電子郵件識別碼(UID)]</p> </td> 
   <td> <p>輸入您要標示為已讀取之電子郵件的電子郵件UID 。</p> <p>您可以使用[！UICONTROL Email] &gt;[！UICONTROL Watch Email]模組或[！UICONTROL Search Email]模組來取得電子郵件的UID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 將電子郵件標示為未讀取]

設定「未讀取」旗標，將選取資料夾中的電子郵件或草稿標示為未讀取。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的電子郵件帳戶連線到[！UICONTROL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">將您的電子郵件連線到[！UICONTROL Workfront Fusion]</a>。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資料夾]</td> 
   <td>選取您要標籤為未讀取的電子郵件資料夾。 範例： Primary。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL電子郵件識別碼(UID)]</p> </td> 
   <td> <p>輸入您要標示為未讀取之電子郵件的電子郵件UID。</p> <p>您可以使用[！UICONTROL Email] &gt;[！UICONTROL Watch Email]模組或[！UICONTROL Search Email]模組來取得電子郵件的UID。</p> </td> 
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
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的電子郵件帳戶連線到[！UICONTROL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">將您的電子郵件連線到[！UICONTROL Workfront Fusion]</a>。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Source資料夾]</td> 
   <td>選取包含您要移動電子郵件之電子郵件的資料夾。 範例： Primary。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL目的地資料夾]</td> 
   <td> <p> 選取您要新增電子郵件的資料夾。 範例：工作。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL電子郵件識別碼(UID)]</p> </td> 
   <td> <p>輸入您要移至目的地資料夾之電子郵件的電子郵件UID。</p> <p>您可以使用[！UICONTROL Email] &gt;[！UICONTROL Watch Email]模組或[！UICONTROL Search Email]模組來取得電子郵件的UID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 複製電子郵件]

將電子郵件或草稿複製到選取的資料夾。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的電子郵件帳戶連線到[！UICONTROL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">將您的電子郵件連線到[！UICONTROL Workfront Fusion]</a>。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Source資料夾]</td> 
   <td>選取您要複製電子郵件的資料夾。 範例： Primary。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL目的地資料夾]</td> 
   <td> <p> 選取您要複製電子郵件的資料夾。 範例：工作。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL電子郵件識別碼(UID)]</p> </td> 
   <td> <p>輸入您要複製到目的地資料夾之電子郵件的電子郵件UID。</p> <p>您可以使用[！UICONTROL Email] &gt;[！UICONTROL Watch Email]模組或[！UICONTROL Search Email]模組來取得電子郵件的UID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除電子郵件]

從選取的資料夾中移除電子郵件或草稿。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的電子郵件帳戶連線到[！UICONTROL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">將您的電子郵件連線到[！UICONTROL Workfront Fusion]</a>。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資料夾]</td> 
   <td>選取要刪除的電子郵件資料夾。 範例： Primary。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL電子郵件識別碼(UID)]</p> </td> 
   <td> <p>輸入您要刪除之電子郵件的電子郵件UID。</p> <p>您可以使用[！UICONTROL Email] &gt;[！UICONTROL Watch Email]模組或[！UICONTROL Search Email]模組來取得電子郵件的UID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL分段]</td> 
   <td> <p>啟用此選項可允許模組永久移除目前開啟之信箱中標示為[！UICONTROL已刪除]的所有郵件。</p> <p>注意：在[!DNL Gmail]中，此行為是由[！UICONTROL設定] &gt;[！UICONTROL轉送POP/IMAP in IMAP access]區段中的設定所驅動。</p> </td> 
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
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的電子郵件帳戶連線到[！UICONTROL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">將您的電子郵件連線到[！UICONTROL Workfront Fusion]</a>。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資料夾] </td> 
   <td> <p>選取包含您要擷取之電子郵件的資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL擷取時將訊息標示為已讀取] </td> 
   <td> <p>如果您要在擷取詳細資料後將未讀取的電子郵件標示為已讀取，請啟用此選項。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL條件]</p> </td> 
   <td> <p>選取您要擷取之電子郵件的條件：</p> 
    <ul> 
     <li>[！UICONTROL所有電子郵件]</li> 
     <li>[！UICONTROL僅讀取電子郵件]</li> 
     <li>[！UICONTROL Only未讀取電子郵件]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL寄件者電子郵件地址] </td> 
   <td> <p>輸入或對應您要擷取其電子郵件的寄件者電子郵件地址。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[！UICONTROL收件者電子郵件地址]</td> 
   <td> <p> 輸入或對應您要擷取其電子郵件的收件者的電子郵件地址。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL起始日期] </td> 
   <td> <p>輸入或對應日期，以擷取在指定日期當天或之後處理的電子郵件。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL日期之前]</td> 
   <td> <p> 輸入或對應日期，以擷取指定日期當天或之前處理的電子郵件。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL主旨] </td> 
   <td> <p>輸入或對應您要擷取之電子郵件的主旨。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL片語] </td> 
   <td> <p>輸入或對應任何關鍵字，以僅擷取包含特定片語的電子郵件。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL電子郵件識別碼(UID)]</td> 
   <td> <p> 輸入要擷取其詳細資訊之電子郵件的電子郵件ID (UID)。</p> <p>您可以使用[!DNL Workfront Fusion]的[！UICONTROL Watch Email]模組或[！UICONTROL Search Email]模組來取得電子郵件的UID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL結果數量上限]</td> 
   <td> <p> 一個案例執行週期內應該傳回的最大電子郵件數量[!DNL Workfront Fusion]。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL即使模組未傳回任何結果，仍繼續執行路由]</td> 
   <td> <p> 選取是否要在沒有傳回結果的情況下繼續執行模組。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 迭代器

#### [!UICONTROL 重複附件]

逐一反複收到附件。

電子郵件疊代器模組可讓您分別管理電子郵件附件。 例如，您可以將設定為觀看電子郵件，以反複處理包含附件的電子郵件並接收警報。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Source模組]</td> 
   <td> <p>選取輸出附有您要反複處理之附件的電子郵件的模組。</p> </td> 
  </tr> 
 </tbody> 
</table>

如需迭代器的詳細資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md)中的[迭代器模組。
