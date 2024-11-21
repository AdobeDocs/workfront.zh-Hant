---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Microsoft Office 365電子郵件
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用Microsoft Office 365電子郵件的工作流程，並將其連線至多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: 29b69e8c-a889-441e-a052-287f1db2052d
source-git-commit: 2e91e9a4c691430f3c98e3cbddb30706ea57f84a
workflow-type: tm+mt
source-wordcount: '2723'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Email]模組

在[!DNL Adobe Workfront Fusion]案例中，您可以自動處理使用[!UICONTROL Microsoft Office 365電子郵件]的工作流程，並將其連線至多個協力廠商應用程式和服務。

若要搭配[!DNL Adobe Workfront Fusion]使用[!UICONTROL Office 365電子郵件]，必須有[!UICONTROL Office 365帳戶]。 您可以在www.office.com建立一個。

如需有關將您的[!UICONTROL Office 365]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱[建立與 [!DNL Adobe Workfront Fusion] 的連線 — 基本指示](../../workfront-fusion/connections/connect-to-fusion-general.md)

在您授與同意後，系統會將您重新導向回[!UICONTROL Workfront Fusion]管理頁面，您可在此繼續建立情境。

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

若要使用[!DNL Microsoft Office 365 Email]模組，您必須有[!DNL Microsoft Office 365 Email]帳戶。

## Microsoft Office 365電子郵件API資訊

Microsoft Office 365電子郵件聯結器使用下列專案：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">基礎URL</td> 
   <td> https://graph.microsoft.com/v1.0</td> 
  </tr> 
  <tr> 
   <td role="rowheader">API版本</td> 
   <td> v1.0 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API標籤</td> 
   <td>v2.6.5</td> 
  </tr>
 </tbody> 
 </table>



## 正在將[!DNL Office 365 Email]服務連線到[!DNL Workfront Fusion]

如需有關將您的[!DNL Office 365 Email]帳戶連線到[!UICONTROL Workfront Fusion]的指示，請參閱[建立與[!UICONTROL Adobe Workfront Fusion]的連線](../../workfront-fusion/connections/connect-to-fusion-general.md) — 基本指示

>[!NOTE]
>
>部分Microsoft應用程式使用相同的連線，而此連線會繫結至個別使用者許可權。 因此，在建立連線時，許可權同意畫面會顯示先前授與此使用者連線的所有許可權，以及目前應用程式所需的任何新許可權。
>
>例如，如果使用者擁有透過Excel聯結器授予的「讀取表格」許可權，然後在Outlook聯結器中建立連線以讀取電子郵件，則許可權同意畫面會顯示已授予的「讀取表格」許可權和新要求的「寫入電子郵件」許可權。

## [!DNL Microsoft Office 365 Email]模組及其欄位

當您設定[!DNL Microsoft Office 365 Email]模組時，[!DNL Workfront Fusion]會顯示下列欄位。 除了這些欄位以外，可能還會顯示其他[!DNL Microsoft Office 365 Email]欄位，視您在應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中將資訊從一個模組對應到另一個模組。

![](assets/map-toggle-350x74.png)

* [訊息](#message)
* [草稿訊息](#draft-message)
* [附件](#attachment)
* [其他](#other)

### 訊息

* [[!UICONTROL 建立並傳送訊息（舊版）]](#create-and-send-a-message)
* [[!UICONTROL 刪除訊息]](#delete-a-message)
* [[!UICONTROL 取得訊息]](#get-a-message)
* [[!UICONTROL 移動訊息]](#move-a-message)
* [[!UICONTROL 搜尋訊息]](#search-messages)
* [[!UICONTROL 觀看訊息]](#watch-messages)



#### [!UICONTROL 建立並傳送訊息（舊版）]

建立並傳送電子郵件訊息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Office 365]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL主旨]</td> 
   <td> <p>輸入或對映訊息的主旨行。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[！UICONTROL內文內容型別]</td> 
   <td>選取訊息的正文內容是HTML還是文字。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL內文內容]</td> 
   <td> <p>輸入或對應電子郵件的郵件內文。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL重要性]</td> 
   <td> <p>選取電子郵件的重要性</p> 
    <ul> 
     <li>[！UICONTROL低]</li> 
     <li>[！UICONTROL Normal]</li> 
     <li>[！UICONTROL高]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL至收件者]</p> </td> 
   <td> <p>新增您要傳送訊息的電子郵件地址：</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL名稱]</strong> </p> <p>輸入連絡人姓名</p> </li> 
     <li> <p><strong>[！UICONTROL電子郵件地址]</strong> </p> <p>輸入連絡人的電子郵件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL CC收件者]</p> </td> 
   <td> <p>新增您要接收郵件復本的收件者：</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL名稱]</strong> </p> <p>輸入連絡人姓名</p> </li> 
     <li> <p><strong>[！UICONTROL電子郵件地址]</strong> </p> <p>輸入連絡人的電子郵件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL密件副本收件者]</p> </td> 
   <td> <p>新增您要在郵件中複製的收件者，不允許其他收件者檢視其名稱或電子郵件地址：</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL名稱]</strong> </p> <p>輸入連絡人姓名</p> </li> 
     <li> <p><strong>[！UICONTROL電子郵件地址]</strong> </p> <p>輸入連絡人的電子郵件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL附件]</p> </td> 
   <td> <p>將附件新增至電子郵件：</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL檔案名稱]</strong> </p> <p>輸入檔案名稱。 範例： <code>sample.doc</code></p> </li> 
     <li> <p><strong>[！UICONTROL資料]</strong> </p> <p>在欄位中輸入檔案資料，或對映檔案的來源。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Internet郵件標頭]</td> 
   <td> <p>新增電子郵件的郵件標題。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL名稱]</strong> </p> <p>輸入頁首的名稱</p> </li> 
     <li> <p><strong>[！UICONTROL電子郵件地址]</strong> </p> <p>輸入頁首的值。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立並傳送訊息]

建立並傳送電子郵件訊息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Office 365]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL主旨]</td> 
   <td> <p>輸入或對映訊息的主旨行。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[！UICONTROL內文內容型別]</td> 
   <td>選取訊息的正文內容是HTML還是文字。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL內文內容]</td> 
   <td> <p>輸入或對應電子郵件的郵件內文。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL重要性]</td> 
   <td> <p>選取電子郵件的重要性</p> 
    <ul> 
     <li>[！UICONTROL低]</li> 
     <li>[！UICONTROL Normal]</li> 
     <li>[！UICONTROL高]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL至收件者]</p> </td> 
   <td> <p>新增您要傳送訊息的電子郵件地址：</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL名稱]</strong> </p> <p>輸入連絡人姓名</p> </li> 
     <li> <p><strong>[！UICONTROL電子郵件地址]</strong> </p> <p>輸入連絡人的電子郵件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL CC收件者]</p> </td> 
   <td> <p>新增您要接收郵件復本的收件者：</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL名稱]</strong> </p> <p>輸入連絡人姓名</p> </li> 
     <li> <p><strong>[！UICONTROL電子郵件地址]</strong> </p> <p>輸入連絡人的電子郵件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL密件副本收件者]</p> </td> 
   <td> <p>新增您要在郵件中複製的收件者，不允許其他收件者檢視其名稱或電子郵件地址：</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL名稱]</strong> </p> <p>輸入連絡人姓名</p> </li> 
     <li> <p><strong>[！UICONTROL電子郵件地址]</strong> </p> <p>輸入連絡人的電子郵件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL附件]</p> </td> 
   <td> <p>將附件新增至電子郵件：</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL檔案名稱]</strong> </p> <p>輸入檔案名稱。 範例： <code>sample.doc</code></p> </li> 
     <li> <p><strong>[！UICONTROL資料]</strong> </p> <p>在欄位中輸入檔案資料，或對映檔案的來源。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Internet郵件標頭]</td> 
   <td> <p>新增電子郵件的郵件標題。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL名稱]</strong> </p> <p>輸入頁首的名稱</p> </li> 
     <li> <p><strong>[！UICONTROL電子郵件地址]</strong> </p> <p>輸入頁首的值。</p> </li> 
    </ul> </td> 
  </tr> 
   <td role="rowheader">[！UICONTROL From e-mail address]</td> 
   <td> <p> 若要使用共用電子郵件地址，請在此輸入地址。 用於此模組之連線中使用其認證的使用者必須擁有共用資料夾的存取權。<p>將此欄位留空將使用連線擁有者自己的電子郵件地址。</p></p> </td> 
  </tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</td> 
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
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Office 365]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL From e-mail address]</td> 
   <td> <p> 若要使用共用電子郵件地址，請在此輸入地址。 用於此模組之連線中使用其認證的使用者必須擁有共用資料夾的存取權。<p>將此欄位留空將使用連線擁有者自己的電子郵件地址。</p></p> </td> 
  </tr> 
   <td role="rowheader">[！UICONTROL訊息ID]</td> 
   <td> <p> 選取或對應您要刪除之訊息的ID。</p> </td> 
  </tr> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得訊息]

取得特定訊息的中繼資料

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Office 365]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL From e-mail address]</td> 
   <td> <p> 若要使用共用電子郵件地址，請在此輸入地址。 用於此模組之連線中使用其認證的使用者必須擁有共用資料夾的存取權。<p>將此欄位留空將使用連線擁有者自己的電子郵件地址。</p></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL訊息ID]</td> 
   <td> <p> 選取或對應您要擷取中繼資料的訊息ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL取得MIME內容]</td> 
   <td>啟用此選項以擷取有關訊息MIME內容的資料。 [！UICONTROL MIME]內容可能包含影像、音訊、視訊或其他型別的檔案。</td> 
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
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Office 365]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL訊息ID]</td> 
   <td> <p> 選取或對應您要移至其他資料夾的郵件ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL郵件資料夾] </td> 
   <td> <p>選取或對應您要移動郵件的資料夾識別碼。</p> </td> 
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
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Office 365]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
    <tr> 
   <td role="rowheader">[！UICONTROL From e-mail address]</td> 
   <td> <p> 若要使用共用電子郵件地址，請在此輸入地址。 用於此模組之連線中使用其認證的使用者必須擁有共用資料夾的存取權。<p>將此欄位留空將使用連線擁有者自己的電子郵件地址。</p></p> </td> 
  </tr> 
<tr> 
   <td role="rowheader">[！UICONTROL郵件資料夾]</td> 
   <td> <p>選取包含您要搜尋之郵件的資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL搜尋]</td> 
   <td>輸入您的搜尋查詢。 如需如何撰寫搜尋查詢的詳細資訊，請參閱[!DNL Microsoft]支援文章<a href="https://support.microsoft.com/en-us/office/search-mail-and-people-in-outlook-com-88108edf-028e-4306-b87e-7400bbb40aa7?ui=en-us&amp;rs=en-us&amp;ad=us">在[!DNL Outlook.com]</a>中搜尋郵件和人員。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Order by]</td> 
   <td> <p>選取您要如何排序結果：</p> 
    <ul> 
     <li>[！UICONTROL主旨（遞增或遞減）]</li> 
     <li>[！UICONTROL建立的日期時間（升序或降序）]</li> 
     <li>[！UICONTROL上次修改的日期時間（升序或降序）]</li> 
     <li>[！UICONTROL收到日期時間（升序或降序）]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>輸入在一個案例執行週期中[!DNL Workfront Fusion]應傳回的最大訊息數。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 觀看訊息]

在傳送或接收新電子郵件時觸發。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Office 365]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL監視訊息]</p> </td> 
   <td> <p>選取您要觀看的訊息：</p> 
    <ul> 
     <li>[！UICONTROL Only Unread]</li> 
     <li>[！UICONTROL唯讀]</li> 
     <li>[！UICONTROL All]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL郵件資料夾]</td> 
   <td> <p>選取包含您要觀看之郵件的資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL搜尋]</td> 
   <td>輸入您的搜尋查詢。 如需如何撰寫搜尋查詢的詳細資訊，請參閱[!DNL Microsoft]支援文章<a href="https://support.microsoft.com/en-us/office/search-mail-and-people-in-outlook-com-88108edf-028e-4306-b87e-7400bbb40aa7?ui=en-us&amp;rs=en-us&amp;ad=us">在[!DNL Outlook.com]</a>中搜尋郵件和人員。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制] </td> 
   <td> <p>輸入在一個案例執行週期中[!DNL Workfront Fusion]應傳回的最大訊息數。</p> </td> 
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
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Office 365]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL主旨]</td> 
   <td> <p>輸入訊息的主旨行。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL內文內容型別]</td> 
   <td>選取訊息的正文內容是HTML還是文字。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL內文內容]</td> 
   <td> <p>輸入電子郵件的郵件內文。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL重要性]</td> 
   <td> <p>選取電子郵件的重要性</p> 
    <ul> 
     <li>[！UICONTROL低]</li> 
     <li>[！UICONTROL Normal]</li> 
     <li>[！UICONTROL高]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL至收件者]</p> </td> 
   <td> <p>新增您要傳送訊息的收件者：</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL名稱]</strong> </p> <p>輸入連絡人姓名</p> </li> 
     <li> <p><strong>[！UICONTROL電子郵件地址]</strong> </p> <p>輸入連絡人的電子郵件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL CC收件者]</p> </td> 
   <td> <p>新增收件者您想要收到訊息復本的：</p> 
    <ul> 
     <li> <p><strong>名稱</strong> </p> <p>輸入連絡人姓名</p> </li> 
     <li> <p><strong>電子郵件地址</strong> </p> <p>輸入連絡人的電子郵件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>密件副本收件者</p> </td> 
   <td> <p>新增您要在郵件中複製的收件者，不允許其他收件者檢視其名稱或電子郵件地址：</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL名稱]</strong> </p> <p>輸入連絡人姓名</p> </li> 
     <li> <p><strong>[！UICONTROL電子郵件地址]</strong> </p> <p>輸入連絡人的電子郵件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL附件]</p> </td> 
   <td> <p>將附件新增至電子郵件：</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL檔案名稱]</strong> </p> <p>輸入檔案名稱。 範例： <code>sample.doc</code></p> </li> 
     <li> <p><strong>[！UICONTROL資料]</strong> </p> <p>在欄位中輸入檔案資料，或對映檔案的來源。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL From e-mail address]</td> 
   <td> <p> 若要使用共用電子郵件地址，請在此輸入地址。 用於此模組之連線中使用其認證的使用者必須擁有共用資料夾的存取權。<p>將此欄位留空將使用連線擁有者自己的電子郵件地址。</p></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 傳送郵件草稿]

傳送目前為草稿的電子郵件訊息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Office 365]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL From e-mail address]</td> 
   <td> <p> 若要使用共用電子郵件地址，請在此輸入地址。 用於此模組之連線中使用其認證的使用者必須擁有共用資料夾的存取權。<p>將此欄位留空將使用連線擁有者自己的電子郵件地址。</p></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL草稿訊息ID]</td> 
   <td> <p> 選取或對應您要傳送之草稿的訊息ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新訊息]

更新現有的訊息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Office 365]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL From e-mail address]</td> 
   <td> <p> 若要使用共用電子郵件地址，請在此輸入地址。 用於此模組之連線中使用其認證的使用者必須擁有共用資料夾的存取權。<p>將此欄位留空將使用連線擁有者自己的電子郵件地址。</p></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸入訊息ID]</td> 
   <td> <p>選取您要如何識別要更新的訊息：</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL手動輸入]</strong> </p> <p>輸入或對映訊息ID。</p> </li> 
     <li> <p><strong>[！UICONTROL從清單中選取]</strong> </p> <p>選取包含要更新之郵件的資料夾，然後選取郵件</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL主旨]</td> 
   <td> <p>輸入訊息的主旨行。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL內文內容]</td> 
   <td> <p>輸入電子郵件的郵件內文。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL重要性]</td> 
   <td> <p>選取電子郵件的重要性</p> 
    <ul> 
     <li>[！UICONTROL低]</li> 
     <li>[！UICONTROL Normal]</li> 
     <li>[！UICONTROL高]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL至收件者]</p> </td> 
   <td> <p>新增您要傳送訊息的電子郵件地址：</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL名稱]</strong> </p> <p>輸入連絡人姓名</p> </li> 
     <li> <p><strong>[！UICONTROL電子郵件地址]</strong> </p> <p>輸入連絡人的電子郵件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL CC收件者]</p> </td> 
   <td> <p>新增收件者您想要收到訊息復本的：</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL名稱]</strong> </p> <p>輸入連絡人姓名</p> </li> 
     <li> <p><strong>[！UICONTROL電子郵件地址]</strong> </p> <p>輸入連絡人的電子郵件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL密件副本收件者]</p> </td> 
   <td> <p>新增您要在郵件中複製的收件者，不允許其他收件者檢視其名稱或電子郵件地址：</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL名稱]</strong> </p> <p>輸入連絡人姓名</p> </li> 
     <li> <p><strong>[！UICONTROL電子郵件地址]</strong> </p> <p>輸入連絡人的電子郵件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL附件]</p> </td> 
   <td> <p>將附件新增至電子郵件：</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL檔案名稱]</strong> </p> <p>輸入檔案名稱。 範例： <code>sample.doc</code></p> </li> 
     <li> <p><strong>[！UICONTROL資料]</strong> </p> <p>在欄位中輸入檔案資料，或對映檔案的來源。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL將其標籤為已讀]</td> 
   <td>啟用此選項可將更新的訊息標示為已讀取。</td> 
  </tr> 
 </tbody> 
</table>

### 附件

* [[!UICONTROL 下載附件]](#download-an-attachment)
* [[!UICONTROL 列出附件]](#list-attachments)

#### [!UICONTROL 下載附件]

此模組會下載指定的附件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Office 365]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL From e-mail address]</td> 
   <td> <p> 若要使用共用電子郵件地址，請在此輸入地址。 用於此模組之連線中使用其認證的使用者必須擁有共用資料夾的存取權。<p>將此欄位留空將使用連線擁有者自己的電子郵件地址。</p></p> </td> 
  </tr> 
   <td role="rowheader">[！UICONTROL訊息ID]</td> 
   <td> <p> 選取或對應包含要下載之附件的郵件ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL附件ID]</td> 
   <td> <p>輸入或對應您要下載之附件的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出附件]

此模組會擷取屬於指定郵件的附件清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Office 365]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL From e-mail address]</td> 
   <td> <p> 若要使用共用電子郵件地址，請在此輸入地址。 用於此模組之連線中使用其認證的使用者必須擁有共用資料夾的存取權。<p>將此欄位留空將使用連線擁有者自己的電子郵件地址。</p></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL訊息ID]</td> 
   <td> <p> 選取或對應您要擷取附件的郵件ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大附件數量。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 其他

* [[!UICONTROL 新增附件]](#add-an-attachment)
  <!--Create and send a message-->
* [[!UICONTROL 進行API呼叫]](#make-an-api-call)

#### [!UICONTROL 新增附件]

此模組會將大型附件新增至郵件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Office 365]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL From e-mail address]</td> 
   <td> <p> 若要使用共用電子郵件地址，請在此輸入地址。 用於此模組之連線中使用其認證的使用者必須擁有共用資料夾的存取權。<p>將此欄位留空將使用連線擁有者自己的電子郵件地址。</p></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL訊息ID]</td> 
   <td> <p> 選取或對應您要新增附件的郵件識別碼。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Source檔案]</td> 
   <td> <p>從先前的模組中選取檔案，或對應來源檔案的名稱和資料。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 進行API呼叫]

此模組可讓您執行自訂API呼叫。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Office 365]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL URL]</p> </td> 
   <td> <p>輸入相對於<code>https://graph.microsoft.com</code>的路徑。 範例：<code> /v1.0/me/messages</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL方法]</p> </td> 
   td&gt; <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP要求方法。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers]</td> 
   <td> <p>以標準JSON物件的形式新增要求的標頭。例如，<code>{"Content-type":"application/json"}</code>。 [!DNL Workfront Fusion]為您新增授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查詢字串]</td> 
   <td> <p> 以標準JSON物件的形式新增API呼叫的查詢。</p> </td> 
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
