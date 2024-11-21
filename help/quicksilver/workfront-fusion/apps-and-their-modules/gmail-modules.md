---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Gmail模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用Gmail的工作流程，並將其連線至多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: 1987156c-e003-4f99-8913-cb47f77efbfc
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '1821'
ht-degree: 0%

---

# [!DNL Gmail]模組

在[!DNL Adobe Workfront Fusion]案例中，您可以自動化使用[!DNL Gmail]的工作流程，並將其連線至多個協力廠商應用程式和服務。

如果您需要有關建立案例的指示，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md)中建立案例。 如需模組的相關資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md)中的[模組。

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
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]計畫，貴組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]計畫中。</p>
   <p>或</p>
   <p>舊版產品需求：您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 先決條件

若要使用[!DNL Gmail]模組，您必須有[!DNL Gmail]帳戶。

## 將[!DNL Gmail]連線至[!DNL Workfront Fusion] {#connect-gmail-to-workfront-fusion}

* [使用 [!DNL Google Workspace]連線 [!DNL Gmail] 至 [!DNL Workfront Fusion] ](#connect-gmail-to-workfront-fusion-usingg-suite)
* [使用 [!DNL gmail.com] 或 [!DNL googlemail].com連線 [!DNL Gmail] 至 [!DNL Workfront Fusion] ](#connect-gmail-to-workfront-fusion-using-gmailcom-or-googlemailcom)

### 使用[!DNL  Google Workspace]連線[!DNL Gmail]至[!DNL Workfront Fusion] {#connect-gmail-to-workfront-fusion-using-g-suite}

如需有關將您的[!DNL Google Workspace]帳戶連線到[!UICONTROL Workfront Fusion]的說明，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md)中建立情境[將模組的應用程式或Web服務連線到 [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect)。

### 使用[!DNL gmail.com]或[!DNL googlemail].com連線[!DNL Gmail]至[!DNL Workfront Fusion] {#connect-gmail-to-workfront-fusion-using-gmail-com-or-googlemail-com}

如果您是[!DNL @gmail.com]或[!DNL @googlemail.com]使用者，您必須在[the [!DNL Google Cloud Platform]](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project)上建立OAuth使用者端，才能取得[!UICONTROL 使用者端識別碼]和[!UICONTROL 使用者端密碼]。

如需如何建立OAuth使用者端及取得[!UICONTROL 使用者端ID]和[!UICONTROL 使用者端密碼]的逐步指示，請參閱[使用自訂OAuth使用者端將Adobe Workfront Fusion連線至Google服務](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md)。

## [!DNL Gmail]模組及其欄位

當您設定[!DNL Gmail]模組時，[!DNL Workfront Fusion]會顯示下列欄位。 除了這些欄位以外，可能還會顯示其他[!DNL Gmail]欄位，視您在應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中將資訊從一個模組對應到另一個模組。

![](assets/map-toggle-350x74.png)

* [觸發器](#triggers)
* [動作](#actions)
* [迭代器](#iterators)

### 觸發器

#### [!UICONTROL 觀看電子郵件]

此觸發模組會在收到要處理的新電子郵件時執行情境。

模組會傳回與一個或多個記錄相關聯的所有標準欄位，以及連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需將[!DNL Gmail]帳戶連線至[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">將[!DNL Gmail]連線至[！UICONTROL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL資料夾] </td> 
   <td> <p>選取要監視的電子郵件資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL篩選器型別] </td> 
   <td> <p>選取您要用來觀看電子郵件的篩選型別</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL簡單篩選器]</strong> </p> <p>填寫[！UICONTROL Criteria]、[！UICONTROL Sender Email Address]、[！UICONTROL Subject]和[！UICONTROL Search Phrase]欄位</p> </li> 
     <li> <p> <strong>[！UICONTROL Gmail篩選器]</strong> </p> <p>在[！UICONTROL查詢]欄位中，輸入您要用來篩選電子郵件的查詢。</p> <p>如需[!DNL Gmail]篩選器的詳細資訊，請參閱[!DNL Gmail]檔案中的<a href="https://support.google.com/mail/answer/7190">搜尋運運算元</a>。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL條件]</td> 
   <td>選取您要觀看[！UICONTROL所有電子郵件]、[！UICONTROL僅讀取電子郵件]或[！UICONTROL僅讀取未讀取]電子郵件。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL寄件者電子郵件地址]</td> 
   <td> <p> 輸入電子郵件地址，以僅觀看從該地址傳送的電子郵件。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL主旨]</td> 
   <td>輸入文字字串，只觀看主旨中含有該文字字串的電子郵件。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL搜尋字詞]</td> 
   <td>輸入文字字串，以僅觀看在電子郵件中任何位置具有該文字字串的電子郵件。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL擷取時將電子郵件訊息標示為已讀取]</td> 
   <td> <p> 啟用此選項可將擷取的電子郵件標示為已讀取。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL結果數量上限]</td> 
   <td> <p> 設定[!DNL Workfront Fusion]在一個週期內可處理的最大結果數量。</p> </td> 
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
* [[!UICONTROL 修改電子郵件標籤]](#modify-email-labels)

#### [!UICONTROL 傳送電子郵件]

此動作模組會傳送新電子郵件。

您指定電子郵件的收件者。

模組會傳回電子郵件的ID及任何關聯欄位，以及連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Gmail]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">將[!DNL Gmail]連線到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL From]</td> 
   <td> <p>輸入或對應寄件者電子郵件地址。</p> <p>注意：如果您輸入的電子郵件地址不正確，則在傳送訊息時可能會發生錯誤，因為您的帳戶可能沒有許可權，無法透過不同於您自己的地址傳送電子郵件。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL至] </td> 
   <td> <p>按一下<strong>[！UICONTROL新增]</strong>，然後輸入或對應每個收件者的電子郵件地址。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL主旨] </td> 
   <td> <p>輸入或對映電子郵件主旨。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL內容] </td> 
   <td> <p>輸入或對映電子郵件內容（訊息內文）。 允許使用HTML標籤。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL附件] </td> 
   <td> <p>按一下<strong>[！UICONTROL新增]</strong>以新增附件。 您可以對應先前模組的檔案。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL複製收件者]</td> 
   <td> <p> 按一下<strong>[！UICONTROL新增]</strong>，然後輸入或對應每個副本收件者的電子郵件地址。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Blind副本收件者]</td> 
   <td> <p> 按一下<strong>[！UICONTROL新增]</strong>，然後輸入或對應每個密件副本收件者的電子郵件地址。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立草稿]

此動作模組會建立新的電子郵件草稿，並將其新增至您指定的資料夾。

您可以指定要建立草稿的資料夾。

模組會傳回電子郵件草稿的ID及任何關聯欄位，以及連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需將[!DNL Gmail]帳戶連線至[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">將[!DNL Gmail]連線至[！UICONTROL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL資料夾] </td> 
   <td> <p>選取您要在其中建立草稿的[!DNL Gmail]資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL至] </td> 
   <td> <p>按一下<strong>[！UICONTROL新增]</strong>，然後輸入或對應每個收件者的電子郵件地址。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL主旨] </td> 
   <td> <p>輸入或對映電子郵件主旨。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL內容] </td> 
   <td> <p>輸入或對映電子郵件內容（訊息內文）。 允許使用HTML標籤。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL附件] </td> 
   <td> <p>按一下<strong>[！UICONTROL新增]</strong>以新增附件。 您可以對應先前模組的檔案。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL複製收件者]</td> 
   <td> <p> 按一下<strong>[！UICONTROL新增]</strong>，然後輸入或對應每個副本收件者的電子郵件地址。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Blind副本收件者]</td> 
   <td> <p> 按一下<strong>[！UICONTROL新增]</strong>，然後輸入或對應每個密件副本收件者的電子郵件地址。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 將電子郵件標示為已讀取]

此動作模組將電子郵件標示為已讀取。

您可以指定電子郵件及其資料夾的ID。

模組會傳回電子郵件的ID及任何關聯欄位，以及連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需將[!DNL Gmail]帳戶連線至[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">將[!DNL Gmail]連線至[！UICONTROL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL資料夾] </td> 
   <td> <p>選取包含電子郵件的[!DNL Gmail]資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL電子郵件ID (UID)]</td> 
   <td> <p> 輸入或對應Email ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 將電子郵件標示為未讀取]

此動作模組將電子郵件或電子郵件草稿標示為未讀取。

您可以指定電子郵件及其資料夾的ID。

模組會傳回電子郵件的ID及任何關聯欄位，以及連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需將[!DNL Gmail]帳戶連線至[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">將[!DNL Gmail]連線至[！UICONTROL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL資料夾] </td> 
   <td> <p>選取包含電子郵件的[!DNL Gmail]資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL電子郵件ID (UID)] </td> 
   <td> <p>輸入或對應您要標示為未讀取之電子郵件的電子郵件ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 移動電子郵件]

此動作模組會將電子郵件或電子郵件草稿移至您指定的資料夾。

您可以指定資料夾、目的地資料夾和電子郵件的ID。

模組會傳回電子郵件的ID及任何關聯欄位，以及連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需將[!DNL Gmail]帳戶連線至[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">將[!DNL Gmail]連線至[！UICONTROL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL資料夾] </td> 
   <td> <p>選取包含您要移動之電子郵件的[!DNL Gmail]來源資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL目的地資料夾]</td> 
   <td> <p> 選取您要移動電子郵件的[!DNL Gmail]目標資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL電子郵件ID (UID)]</td> 
   <td> <p> 輸入或對應您要移動之電子郵件的電子郵件ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 複製電子郵件]

此動作模組會將電子郵件或電子郵件草稿複製到您指定的資料夾中。

您可以指定資料夾、目的地資料夾和電子郵件的ID。

模組會傳回電子郵件的ID及任何關聯欄位，以及連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需將[!DNL Gmail]帳戶連線至[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">將[!DNL Gmail]連線至[！UICONTROL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL資料夾] </td> 
   <td> <p>選取包含您要複製之電子郵件的[!DNL Gmail]來源資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL目的地資料夾]</td> 
   <td> <p>選取您要複製電子郵件的[!DNL Gmail]目標資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL電子郵件ID (UID)]</td> 
   <td> <p>輸入或對應您要複製之電子郵件的電子郵件ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除電子郵件]

此動作模組會從您指定的資料夾中移除電子郵件或電子郵件草稿。

模組會傳回電子郵件的ID及任何關聯欄位，以及連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需將[!DNL Gmail]帳戶連線至[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">將[!DNL Gmail]連線至[！UICONTROL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL [!DNL Gmail]訊息識別碼]</p> </td> 
   <td> <p>輸入或對應您要刪除之電子郵件的電子郵件ID。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL永久] </td> 
   <td> <p>啟用此選項可允許模組永久刪除電子郵件，而非將其移至垃圾桶資料夾。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 修改電子郵件標籤]

此動作模組會修改您指定之電子郵件訊息上的標籤。

模組會傳回電子郵件的ID及任何關聯欄位，以及連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需將[!DNL Gmail]帳戶連線至[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">將[!DNL Gmail]連線至[！UICONTROL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL [!DNL Gmail]訊息識別碼]</td> 
   <td> <p> 輸入或對應您要刪除之電子郵件的電子郵件ID。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>要新增的[！UICONTROL標籤]</p> </td> 
   <td> <p>選取或對應您要新增至所選電子郵件訊息的標籤。</p> </td> 
  </tr> 
  <tr> 
   <td>要移除的[！UICONTROL標籤]</td> 
   <td> <p> 選取或對應您要從選取的電子郵件移除的標籤。</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>[!UICONTROL 要新增的標籤]和要移除的[!UICONTROL 標籤]欄位僅載入使用者建立的標籤。

### 迭代器

#### [!UICONTROL 重複附件]

您可以重複電子郵件附件。 每個附件都是模組輸出中的獨立套件。 如需詳細資訊，請參閱Adobe Workfront Fusion中的[疊代器模組](../../workfront-fusion/modules/iterator-module.md)。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Source模組] </td> 
   <td> <p>選取您想從其中反複輸入附件的模組。 </p> </td> 
  </tr> 
 </tbody> 
</table>
