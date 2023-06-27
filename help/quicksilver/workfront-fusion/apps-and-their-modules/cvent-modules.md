---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: 事件模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動化使用Cvent的工作流程，並將其連線到多個第三方應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: c95b9764-29a5-4d8c-8e6d-68a3969129e0
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1044'
ht-degree: 1%

---

# [!DNL Cvent] 模組

在 [!DNL Adobe Workfront Fusion] 情境下，您可以自動化使用下列專案的工作流程： [!DNL Cvent]，以及將其連線到多個協力廠商應用程式和服務。

如果您需要建立案例的說明，請參閱 [在中建立情境 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

如需模組的相關資訊，請參閱 [中的模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

有關以下專案的資訊： [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 必要條件

使用 [!DNL Cvent] 模組，您必須擁有 [!DNL Cvent] 帳戶。

## Connect [!DNL Cvent] 至 [!DNL Adobe Workfront Fusion] {#connect-cvent-to-adobe-workfront-fusion}

>[!NOTE]
>
>此 [!DNL Cvent] 模組透過 [!UICONTROL SOAP] API。 若要建立與的連線 [!DNL Cvent]，您必須確保以下各項：
>
>* 您有 [!UICONTROL SOAP] 存取 [!DNL Cvent] API。
>* 此 [!DNL Workfront Fusion] IP位址已新增至貴組織的允許清單。
>
>  如需清單： [!DNL Workfront Fusion] IP位址，請參閱 [用於存取的IP位址 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)


您可以建立與的連線 [!DNL Cvent] 直接從a內的帳戶 [!DNL Cvent] 模組。

1. 在任何 [!DNL Cvent] 模組，按一下 **[!UICONTROL 新增]** 旁邊 [!UICONTROL 連線] 欄位。
1. 選取您要連線的區域。

   * [!UICONTROL 北美]
   * [!UICONTROL 歐洲]
   * [!UICONTROL Sandbox]

1. 按一下 **[!UICONTROL 繼續]** 以建立連線並返回模組。

## [!DNL Cvent] 模組及其欄位

當您設定 [!DNL Cvent] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 除了這些以外， [!DNL Cvent] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應至中的另一個模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [動作](#actions)
* [搜尋](#searches)

### 動作

* [[!UICONTROL 自訂API呼叫]](#create-meeting-request)
* [[!UICONTROL 讀取記錄]](#read-a-record)
* [[!UICONTROL 註冊受邀者]](#register-invitee)
* [[!UICONTROL 新增被邀請者]](#add-invitee)
* [[!UICONTROL 刪除連絡人]](#delete-contact)
* [[!UICONTROL 更新連絡人]](#update-contact)
* [[!UICONTROL 建立會議要求]](#create-meeting-request)

#### [!UICONTROL 自訂API呼叫]

此動作模組可讓您對 [!DNL Cvent] API。 如此一來，您就可以建立其他人無法完成的資料流程自動化 [!DNL Cvent] 模組。

當您設定此模組時，會顯示下列欄位。

模組會傳回狀態代碼，以及API呼叫的標題和正文。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL連線]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Cvent] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] 至 [!DNL Adobe Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">作業</td> 
   td&gt; <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">內文(XML)</td> 
   <td> <p>輸入或對應API呼叫的正文。 這必須只包含XML。 模組將自動包含驗證標頭。 </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 讀取記錄]

此動作模組會讀取特定記錄的相關資訊。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL連線]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Cvent] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] 至 [!DNL Adobe Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL記錄型別]</p> </td> 
   <td>選取您要讀取之記錄的專案型態。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL聯絡人] / [！UICONTROL事件] / [！UICONTROL被邀請者ID]</td> 
   <td> <p>輸入或對應您要讀取的專案的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸出]</td> 
   <td> <p>選取您要納入模組輸出的欄位。 根據您選取的專案型別，可使用欄位。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 註冊受邀者]

此動作模組會註冊事件的被邀請者。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL連線]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Cvent] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] 至 [!DNL Adobe Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>被邀請者ID</p> </td> 
   <td> <p>輸入或對應您要註冊事件的被邀請者ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">事件ID</td> 
   <td> <p>輸入或對應您要註冊受邀者之事件的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 新增被邀請者]

此動作模組會邀請連絡人參加活動。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL連線]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Cvent] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] 至 [!DNL Adobe Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL連絡人ID]</p> </td> 
   <td> <p>輸入或對應您要新增至事件的連絡人ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL事件ID]</td> 
   <td> <p>輸入或對應您要新增連絡人的事件ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除連絡人]

此動作模組會刪除Cvent中的單一連絡人。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL連線]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Cvent] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] 至 [!DNL Adobe Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL連絡人ID]</td> 
   <td> <p>輸入或對應您要刪除之連絡人的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新連絡人]

此動作模組會使用其ID更新現有連絡人。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL連線]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Cvent] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] 至 [!DNL Adobe Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL連絡人ID]</p> </td> 
   <td> <p>輸入或對應您要更新的連絡人ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL欄位]</td> 
   <td> <p>選取您要輸入資訊的欄位，然後填寫這些欄位的所需值。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL自訂欄位]</td> 
   <td> <p>選取您要輸入資訊的欄位，然後填寫這些欄位的所需值。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立會議要求]

此動作模組會將會議要求新增至您的帳戶。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL連線]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Cvent] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] 至 [!DNL Adobe Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL表單ID]</p> </td> 
   <td> <p>輸入或對應您要用來建立新會議要求的表單ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL會議請求欄位]</td> 
   <td> <p>選取您要輸入資訊的會議請求欄位，然後填寫這些欄位的所需值。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL事件請求欄位]</td> 
   <td> <p>選取您要輸入資訊的事件請求欄位，然後填寫這些欄位的所需值。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL RFP要求欄位]</td> 
   <td> <p>選取您要輸入資訊的提案請求欄位，然後填寫這些欄位的所需值。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 搜尋

#### [!UICONTROL 清單記錄]

此搜尋模組會擷取特定型別之所有記錄的相關資訊。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL連線]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示， [!DNL Cvent] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] 至 [!DNL Adobe Workfront Fusion]</a> 本文章內容。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL記錄型別]</p> </td> 
   <td> <p>選取您要列出的記錄型別。</p> 
    <ul> 
     <li> <p>來自您的所有活動 [!DNL Cvent] 帳戶</p> </li> 
     <li> <p>事件的所有工作階段</p> </li> 
     <li> <p>活動的所有受邀者</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL事件ID]</td> 
   <td> <p>如果您要列出被邀請者或工作階段，請輸入或對應這些被邀請者或工作階段相關聯之事件的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>
