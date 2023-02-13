---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 連接器
navigation-topic: apps-and-their-modules
title: Gmail模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動化使用Gmail的工作流程，並將其連接至多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: 1987156c-e003-4f99-8913-cb47f77efbfc
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1785'
ht-degree: 0%

---

# [!DNL Gmail] 模組

在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!DNL Gmail]，並將其連接至多個協力廠商應用程式和服務。

如果您需要建立案例的相關指示，請參閱 [在中建立案例 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). 如需模組的相關資訊，請參閱 [中的模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

使用 [!DNL Gmail] 模組，您必須 [!DNL Gmail] 帳戶。

## Connect [!DNL Gmail] to [!DNL Workfront Fusion] {#connect-gmail-to-workfront-fusion}

* [Connect [!DNL Gmail] to [!DNL Workfront Fusion] 使用[!DNL G Suite]](#connect-gmail-to-workfront-fusion-usingg-suite)
* [Connect [!DNL Gmail] to [!DNL Workfront Fusion] 使用 [!DNL gmail.com] 或 [!DNL googlemail].com](#connect-gmail-to-workfront-fusion-using-gmailcom-or-googlemailcom)

### Connect [!DNL Gmail] to [!DNL Workfront Fusion] 使用[!DNL  G Suite] {#connect-gmail-to-workfront-fusion-using-g-suite}

有關連接 [!DNL G Suite] 帳戶 [!UICONTROL Workfront融合]，請參閱 [將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) 在文章中 [在中建立案例 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### Connect [!DNL Gmail] to [!DNL Workfront Fusion] 使用 [!DNL gmail.com] 或 [!DNL googlemail].com {#connect-gmail-to-workfront-fusion-using-gmail-com-or-googlemail-com}

如果您 [!DNL @gmail.com] 或 [!DNL @googlemail.com] 使用者，您必須在 [the [!DNL Google Cloud Platform]](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) 為了獲得 [!UICONTROL 用戶端ID] 和 [!UICONTROL 用戶端密碼].

如需如何建立OAuth用戶端和取得 [!UICONTROL 用戶端ID] 和 [!UICONTROL 用戶端密碼]，請參閱 [使用自訂OAuth用戶端將Adobe Workfront Fusion連線至Google Services](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## [!DNL Gmail] 模組及其欄位

設定時 [!DNL Gmail] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!DNL Gmail] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [觸發器](#triggers)
* [動作](#actions)
* [迭代器](#iterators)

### 觸發器

#### [!UICONTROL 觀看電子郵件]

此觸發模組會在收到要處理的新電子郵件時執行案例。

模組會傳回與記錄或記錄相關聯的所有標準欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Gmail] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] 到[!UICONTROL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資料夾] </td> 
   <td> <p>選取您要監看的電子郵件資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL篩選器類型] </td> 
   <td> <p>選取您要用來監視電子郵件的篩選類型</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL簡單篩選器]</strong> </p> <p>填寫[!UICONTROL條件]、[!UICONTROL發件人電子郵件地址]、[!UICONTROL主題]和[!UICONTROL搜索短語]欄位</p> </li> 
     <li> <p> <strong>[!UICONTROL Gmail篩選器]</strong> </p> <p>在[!UICONTROL查詢]欄位中，輸入要用於篩選電子郵件的查詢。</p> <p>如需 [!DNL Gmail] 篩選器，請參閱 <a href="https://support.google.com/mail/answer/7190">搜尋運算子</a> 在 [!DNL Gmail] 檔案。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL條件]</td> 
   <td>選取您要觀看[!UICONTROL全部電子郵件]、[!UICONTROL僅讀取電子郵件]或[!UICONTROL僅未讀取]電子郵件。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL發件人電子郵件地址]</td> 
   <td> <p> 輸入僅監視從該地址發送的電子郵件的電子郵件地址。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL主題]</td> 
   <td>輸入文字字串，以僅監視主旨中包含該文字字串的電子郵件。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL搜索短語]</td> 
   <td>輸入文字字串，只監視電子郵件中任何位置都有該文字字串的電子郵件。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL將電子郵件標籤為讀取時讀取]</td> 
   <td> <p> 啟用此選項可將擷取的電子郵件標示為已讀取。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL結果的最大數]</td> 
   <td> <p> 設定 [!DNL Workfront Fusion] 可在一個週期中運作。</p> </td> 
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
* [[!UICONTROL 修改電子郵件標籤]](#modify-email-labels)

#### [!UICONTROL 傳送電子郵件]

此動作模組會傳送新電子郵件。

您可以指定電子郵件的收件者。

模組會傳回電子郵件的ID和任何相關欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Gmail] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] to [!DNL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL從]</td> 
   <td> <p>輸入或映射發件人電子郵件地址。</p> <p>注意：如果您輸入的電子郵件地址不正確，則傳送訊息時可能會發生錯誤，因為您的帳戶可能沒有從您自己的地址以外的地址傳送電子郵件的權限。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL To] </td> 
   <td> <p>按一下 <strong>[!UICONTROL添加]</strong>，然後輸入或對應每個收件者的電子郵件地址。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL主題] </td> 
   <td> <p>輸入或對應電子郵件主旨。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL內容] </td> 
   <td> <p>輸入或對應電子郵件內容（訊息內文）。 允許HTML標籤。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL附件] </td> 
   <td> <p>按一下 <strong>[!UICONTROL添加]</strong> 以新增附件。 您可以從先前的模組對應檔案。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL複製收件人]</td> 
   <td> <p> 按一下 <strong>[!UICONTROL添加]</strong>，然後輸入或對應每個副本收件者的電子郵件地址。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL盲副本收件人]</td> 
   <td> <p> 按一下 <strong>[!UICONTROL添加]</strong>，然後輸入或映射每個盲副本收件人的電子郵件地址。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立草稿]

此動作模組會建立新的電子郵件草稿，並將其新增至您指定的資料夾。

指定要建立草稿的資料夾。

模組會傳回電子郵件草稿和任何相關欄位的ID，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Gmail] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] 到[!UICONTROL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資料夾] </td> 
   <td> <p>選取 [!DNL Gmail] 要在中建立草稿的資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL To] </td> 
   <td> <p>按一下 <strong>[!UICONTROL添加]</strong>，然後輸入或對應每個收件者的電子郵件地址。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL主題] </td> 
   <td> <p>輸入或對應電子郵件主旨。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL內容] </td> 
   <td> <p>輸入或對應電子郵件內容（訊息內文）。 允許HTML標籤。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL附件] </td> 
   <td> <p>按一下 <strong>[!UICONTROL添加]</strong> 以新增附件。 您可以從先前的模組對應檔案。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL複製收件人]</td> 
   <td> <p> 按一下 <strong>[!UICONTROL添加]</strong>，然後輸入或對應每個副本收件者的電子郵件地址。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL盲副本收件人]</td> 
   <td> <p> 按一下 <strong>[!UICONTROL添加]</strong>，然後輸入或映射每個盲副本收件人的電子郵件地址。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 將電子郵件標示為已讀取]

此動作模組會將電子郵件標示為已讀取。

您指定電子郵件及其資料夾的ID。

模組會傳回電子郵件的ID和任何相關欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Gmail] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] 到[!UICONTROL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資料夾] </td> 
   <td> <p>選取 [!DNL Gmail] 包含電子郵件的資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL電子郵件ID(UID)]</td> 
   <td> <p> 輸入或對應電子郵件ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 將電子郵件標示為未讀]

此動作模組會將電子郵件或電子郵件草稿標示為未讀。

您指定電子郵件及其資料夾的ID。

模組會傳回電子郵件的ID和任何相關欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Gmail] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] 到[!UICONTROL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資料夾] </td> 
   <td> <p>選取 [!DNL Gmail] 包含電子郵件的資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL電子郵件ID(UID)] </td> 
   <td> <p>輸入或對應您要標示為未讀取之電子郵件的電子郵件ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 移動電子郵件]

此動作模組會將電子郵件或電子郵件草稿移至您指定的資料夾。

您可以指定資料夾、目標資料夾和電子郵件的ID。

模組會傳回電子郵件的ID和任何相關欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Gmail] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] 到[!UICONTROL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資料夾] </td> 
   <td> <p>選取 [!DNL Gmail] 包含要移動的電子郵件的源資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL目標資料夾]</td> 
   <td> <p> 選取 [!DNL Gmail] 您要將電子郵件移至的目標資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL電子郵件ID(UID)]</td> 
   <td> <p> 輸入或對應您要移動之電子郵件的電子郵件ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 複製電子郵件]

此動作模組會將電子郵件或電子郵件草稿複製至您指定的資料夾。

您可以指定資料夾、目標資料夾和電子郵件的ID。

模組會傳回電子郵件的ID和任何相關欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Gmail] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] 到[!UICONTROL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL資料夾] </td> 
   <td> <p>選取 [!DNL Gmail] 包含您要複製之電子郵件的來源資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL目標資料夾]</td> 
   <td> <p>選取 [!DNL Gmail] 您要將電子郵件複製到的目標資料夾。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL電子郵件ID(UID)]</td> 
   <td> <p>輸入或對應您要複製之電子郵件的電子郵件ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除電子郵件]

此動作模組會從您指定的資料夾中移除電子郵件或電子郵件草稿。

模組會傳回電子郵件的ID和任何相關欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Gmail] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] 到[!UICONTROL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL [!DNL Gmail] 消息ID]</p> </td> 
   <td> <p>輸入或對應您要刪除之電子郵件的電子郵件ID。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL永久] </td> 
   <td> <p>啟用此選項可允許模組永久刪除電子郵件，而非將其移至垃圾桶資料夾。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 修改電子郵件標籤]

此動作模組會修改您所指定之電子郵件上的標籤。

模組會傳回電子郵件的ID和任何相關欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Gmail] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Connect [!DNL Gmail] 到[!UICONTROL Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL [!DNL Gmail] 消息ID]</td> 
   <td> <p> 輸入或對應您要刪除之電子郵件的電子郵件ID。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！要添加的標籤]</p> </td> 
   <td> <p>選取或對應您要新增至所選電子郵件的標籤。</p> </td> 
  </tr> 
  <tr> 
   <td>[！要刪除的標籤]</td> 
   <td> <p> 選擇或映射要從所選電子郵件中刪除的標籤。</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>[!UICONTROL 要添加的標籤] 和 [!UICONTROL 要刪除的標籤] 欄位僅載入使用者建立的標籤。

### 迭代器

#### [!UICONTROL 迭代附件]

您可以反覆查詢電子郵件附件。 每個附件是模組輸出中的單獨捆綁。 如需詳細資訊，請參閱 [Adobe Workfront Fusion中的迭代器模組](../../workfront-fusion/modules/iterator-module.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL源模組] </td> 
   <td> <p>選擇要反複查找附件的模組。 </p> </td> 
  </tr> 
 </tbody> 
</table>
