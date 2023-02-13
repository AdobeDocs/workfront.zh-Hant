---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 連接器
navigation-topic: apps-and-their-modules
title: Microsoft Office 365電子郵件
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用Microsoft Office 365電子郵件的工作流程，並將其連接到多個第三方應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: 29b69e8c-a889-441e-a052-287f1db2052d
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1838'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Email]

在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!UICONTROL Microsoft Office 365電子郵件]，並將其連接至多個協力廠商應用程式和服務。

為了使用 [!UICONTROL Office 365電子郵件] with [!DNL Adobe Workfront Fusion]，則必須有 [!UICONTROL Office 365帳戶]. 您可以在www.office.com建立一個。

有關連接 [!UICONTROL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 [建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示](../../workfront-fusion/connections/connect-to-fusion-general.md)

授與同意後，系統會將您重新導向回 [!UICONTROL Workfront融合] 「管理」頁面，您可以在此處繼續建立案例。

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

使用 [!DNL Microsoft Office 365 Email] 模組，您必須 [!DNL Microsoft Office 365 Email] 帳戶。

## [!DNL Microsoft Office 365 Email] 模組及其欄位

設定時 [!DNL Microsoft Office 365 Email] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!DNL Microsoft Office 365 Email] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [訊息](#message)
* [草稿訊息](#draft-message)
* [附件](#attachment)
* [其他](#other)

### 訊息

* [[!UICONTROL 監看訊息]](#watch-messages)
* [[!UICONTROL 搜尋訊息]](#search-messages)
* [[!UICONTROL 取得訊息]](#get-a-message)
* [[!UICONTROL 建立和傳送訊息]](#create-and-send-a-message)
* [[!UICONTROL 移動訊息]](#move-a-message)
* [[!UICONTROL 刪除訊息]](#delete-a-message)

#### [!UICONTROL 監看訊息]

傳送或接收新電子郵件時觸發。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL監看消息]</p> </td> 
   <td> <p>選擇要監視的消息：</p> 
    <ul> 
     <li>[!UICONTROL僅未讀]</li> 
     <li>[!UICONTROL只讀]</li> 
     <li>[!UICONTROL全部]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL郵件資料夾]</td> 
   <td> <p>選取包含您要監看之訊息的資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL搜索]</td> 
   <td>輸入您的搜索查詢。 有關如何編寫搜索查詢的資訊，請參閱 [!DNL Microsoft] 支援文章 <a href="https://support.microsoft.com/en-us/office/search-mail-and-people-in-outlook-com-88108edf-028e-4306-b87e-7400bbb40aa7?ui=en-us&amp;rs=en-us&amp;ad=us">在中搜索郵件和人員 [!DNL Outlook.com]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制] </td> 
   <td> <p>輸入最大消息數 [!DNL Workfront Fusion] 應會在一個案例執行週期期間傳回。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 搜尋訊息]

根據特定條件搜尋訊息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL郵件資料夾]</td> 
   <td> <p>選取包含您要搜尋之訊息的資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL搜索]</td> 
   <td>輸入您的搜索查詢。 有關如何編寫搜索查詢的資訊，請參閱 [!DNL Microsoft] 支援文章 <a href="https://support.microsoft.com/en-us/office/search-mail-and-people-in-outlook-com-88108edf-028e-4306-b87e-7400bbb40aa7?ui=en-us&amp;rs=en-us&amp;ad=us">在中搜索郵件和人員 [!DNL Outlook.com]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL順序依]</td> 
   <td> <p>選擇要如何排序結果：</p> 
    <ul> 
     <li>[!UICONTROL主體（升序或降序）]</li> 
     <li>[!UICONTROL建立的日期時間（遞增或遞減）]</li> 
     <li>[!UICONTROL上次修改的日期時間（升序或降序）]</li> 
     <li>[!UICONTROL接收日期時間（升序或降序）]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>輸入最大消息數 [!DNL Workfront Fusion] 應會在一個案例執行週期期間傳回。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得訊息]

獲取特定消息的元資料

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL消息ID]</td> 
   <td> <p> 選取或對應您要擷取中繼資料之訊息的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL獲取MIME內容]</td> 
   <td>啟用此選項可檢索有關郵件MIME內容的資料。 [!UICONTROL MIME]內容可能包括影像、音訊、視訊或其他類型的檔案。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立和傳送訊息]

建立並傳送電子郵件訊息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主題]</td> 
   <td> <p>輸入或映射消息的主題行。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL主體內容類型]</td> 
   <td>選取訊息的內文內容為HTML或文字。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL內文]</td> 
   <td> <p>輸入或映射電子郵件的郵件正文文本。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL重要性]</td> 
   <td> <p>選取電子郵件的重要性</p> 
    <ul> 
     <li>[!UICONTROL低]</li> 
     <li>[!UICONTROL標準]</li> 
     <li>[!UICONTROL高]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL對收件者]</p> </td> 
   <td> <p>新增您要傳送訊息的電子郵件地址：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL名稱]</strong> </p> <p>輸入聯繫人的姓名</p> </li> 
     <li> <p><strong>[!UICONTROL電子郵件地址]</strong> </p> <p>輸入聯繫人的電子郵件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC收件者]</p> </td> 
   <td> <p>新增您要接收郵件副本的收件者：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL名稱]</strong> </p> <p>輸入聯繫人的姓名</p> </li> 
     <li> <p><strong>[!UICONTROL電子郵件地址]</strong> </p> <p>輸入聯繫人的電子郵件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL密件副本收件人]</p> </td> 
   <td> <p>新增您要在訊息上複製的收件者，而不允許其他收件者查看其姓名或電子郵件地址：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL名稱]</strong> </p> <p>輸入聯繫人的姓名</p> </li> 
     <li> <p><strong>[!UICONTROL電子郵件地址]</strong> </p> <p>輸入聯繫人的電子郵件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL附件]</p> </td> 
   <td> <p>將附件新增至電子郵件：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL檔案名]</strong> </p> <p>輸入檔案名。 範例: <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL資料]</strong> </p> <p>將檔案資料輸入欄位或映射檔案的源。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Internet消息標頭]</td> 
   <td> <p>新增電子郵件的訊息標題。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL名稱]</strong> </p> <p>輸入標題的名稱</p> </li> 
     <li> <p><strong>[!UICONTROL電子郵件地址]</strong> </p> <p>輸入標題的值。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 移動訊息]

將電子郵件移至信箱中選取的資料夾。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL消息ID]</td> 
   <td> <p> 選取或對應您要移至其他資料夾之訊息的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL郵件資料夾] </td> 
   <td> <p>選擇或映射要移動郵件的資料夾的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除訊息]

刪除現有的電子郵件訊息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL消息ID]</td> 
   <td> <p> 選取或對應您要刪除之訊息的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 草稿訊息

* [建立草稿訊息](#create-a-draft-message)
* [傳送草稿訊息](#send-a-draft-message)
* [更新訊息](#update-a-message)

#### [!UICONTROL 建立草稿訊息]

建立新的電子郵件訊息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主題]</td> 
   <td> <p>輸入消息的主旨行。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主體內容類型]</td> 
   <td>選取訊息的內文內容為HTML或文字。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL內文]</td> 
   <td> <p>輸入電子郵件的郵件正文文本。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL重要性]</td> 
   <td> <p>選取電子郵件的重要性</p> 
    <ul> 
     <li>[!UICONTROL低]</li> 
     <li>[!UICONTROL標準]</li> 
     <li>[!UICONTROL高]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL對收件者]</p> </td> 
   <td> <p>新增您要傳送訊息的收件者：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL名稱]</strong> </p> <p>輸入聯繫人的姓名</p> </li> 
     <li> <p><strong>[!UICONTROL電子郵件地址]</strong> </p> <p>輸入聯繫人的電子郵件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC收件者]</p> </td> 
   <td> <p>新增收件者您要接收訊息副本：</p> 
    <ul> 
     <li> <p><strong>名稱</strong> </p> <p>輸入聯繫人的姓名</p> </li> 
     <li> <p><strong>電子郵件位址</strong> </p> <p>輸入聯繫人的電子郵件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>密件副本收件者</p> </td> 
   <td> <p>新增您要在訊息上複製的收件者，而不允許其他收件者查看其姓名或電子郵件地址：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL名稱]</strong> </p> <p>輸入聯繫人的姓名</p> </li> 
     <li> <p><strong>[!UICONTROL電子郵件地址]</strong> </p> <p>輸入聯繫人的電子郵件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL附件]</p> </td> 
   <td> <p>將附件新增至電子郵件：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL檔案名]</strong> </p> <p>輸入檔案名。 範例: <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL資料]</strong> </p> <p>將檔案資料輸入欄位或映射檔案的源。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 傳送草稿訊息]

傳送目前處於草稿中的電子郵件訊息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL草稿訊息ID]</td> 
   <td> <p> 選取或對應您要傳送草稿的訊息ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新訊息]

更新現有訊息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸入消息ID]</td> 
   <td> <p>選取要如何識別要更新的訊息：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL手動輸入]</strong> </p> <p>輸入或映射訊息ID。</p> </li> 
     <li> <p><strong>[!UICONTROL從清單中選擇]</strong> </p> <p>選取包含您要更新之訊息的資料夾，然後選取訊息</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主題]</td> 
   <td> <p>輸入消息的主旨行。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL內文]</td> 
   <td> <p>輸入電子郵件的郵件正文文本。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL重要性]</td> 
   <td> <p>選取電子郵件的重要性</p> 
    <ul> 
     <li>[!UICONTROL低]</li> 
     <li>[!UICONTROL標準]</li> 
     <li>[!UICONTROL高]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL對收件者]</p> </td> 
   <td> <p>新增您要傳送訊息的電子郵件地址：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL名稱]</strong> </p> <p>輸入聯繫人的姓名</p> </li> 
     <li> <p><strong>[!UICONTROL電子郵件地址]</strong> </p> <p>輸入聯繫人的電子郵件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC收件者]</p> </td> 
   <td> <p>新增收件者您要接收訊息副本：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL名稱]</strong> </p> <p>輸入聯繫人的姓名</p> </li> 
     <li> <p><strong>[!UICONTROL電子郵件地址]</strong> </p> <p>輸入聯繫人的電子郵件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL密件副本收件人]</p> </td> 
   <td> <p>新增您要在訊息上複製的收件者，而不允許其他收件者查看其姓名或電子郵件地址：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL名稱]</strong> </p> <p>輸入聯繫人的姓名</p> </li> 
     <li> <p><strong>[!UICONTROL電子郵件地址]</strong> </p> <p>輸入聯繫人的電子郵件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL附件]</p> </td> 
   <td> <p>將附件新增至電子郵件：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL檔案名]</strong> </p> <p>輸入檔案名。 範例: <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL資料]</strong> </p> <p>將檔案資料輸入欄位或映射檔案的源。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL將其標籤為已讀]</td> 
   <td>啟用此選項可將更新後的訊息標示為已讀取。</td> 
  </tr> 
 </tbody> 
</table>

### 附件

* [[!UICONTROL 清單附件]](#list-attachments)
* [[!UICONTROL 下載附件]](#download-an-attachment)

#### [!UICONTROL 清單附件]

此模組檢索屬於指定郵件的附件清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL消息ID]</td> 
   <td> <p> 選擇或映射要從中檢索附件的郵件的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>輸入或映射您希望模組在每個方案執行週期中返回的最大附件數。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 下載附件]

此模組會下載指定的附件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL消息ID]</td> 
   <td> <p> 選擇或映射包含要下載附件的郵件的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL附件ID]</td> 
   <td> <p>輸入或映射要下載的附件ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 其他

* [[!UICONTROL 進行API呼叫]](#make-an-api-call)
* [[!UICONTROL 新增附件]](#add-an-attachment)

#### [!UICONTROL 進行API呼叫]

此模組可讓您執行自訂API呼叫。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>輸入相對於的路徑 <code>https://graph.microsoft.com</code>. 範例:<code> /v1.0/me/messages</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL方法]</p> </td> 
   td&gt; <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL標題]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標題。例如， <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] 為您添加授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL查詢字串]</td> 
   <td> <p> 以標準JSON物件的形式新增API呼叫的查詢。</p> </td> 
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

#### [!UICONTROL 新增附件]

此模組會將大型附件新增至訊息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL消息ID]</td> 
   <td> <p> 選擇或映射要添加附件的郵件的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL源檔案]</td> 
   <td> <p>從上一個模組中選擇一個檔案，或映射源檔案的名稱和資料。</p> </td> 
  </tr> 
 </tbody> 
</table>
