---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: 事件模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用Cvent的工作流程，並將其連線到多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: c95b9764-29a5-4d8c-8e6d-68a3969129e0
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '1059'
ht-degree: 1%

---

# [!DNL Cvent]模組

在[!DNL Adobe Workfront Fusion]案例中，您可以自動化使用[!DNL Cvent]的工作流程，並將其連線至多個協力廠商應用程式和服務。

如果您需要有關建立案例的指示，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md)中建立案例。

如需模組的相關資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md)中的[模組。

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

若要使用[!DNL Cvent]模組，您必須有[!DNL Cvent]帳戶。

## Cvent API資訊

Cvent聯結器使用下列專案：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">API版本</td> 
   <td> V200611.ASMX </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API標籤</td> 
   <td>v1.7.14</td> 
  </tr>
 </tbody> 
 </table>

## 將[!DNL Cvent]連線至[!DNL Adobe Workfront Fusion] {#connect-cvent-to-adobe-workfront-fusion}

>[!NOTE]
>
>[!DNL Cvent]模組透過[!UICONTROL SOAP] API運作。 若要建立與[!DNL Cvent]的連線，您必須確定下列事項：
>
>* 您有[!UICONTROL SOAP]的[!DNL Cvent] API存取權。
>* [!DNL Workfront Fusion] IP位址已新增至您組織的允許清單。
>
>  如需[!DNL Workfront Fusion] IP位址的清單，請參閱[要存取的IP位址 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)


您可以直接從[!DNL Cvent]模組內建立與您的[!DNL Cvent]帳戶的連線。

1. 在任何[!DNL Cvent]模組中，按一下[!UICONTROL 連線]欄位旁的&#x200B;**[!UICONTROL 新增]**。
1. 選取您要連線的區域。

   * [!UICONTROL 北美]
   * [!UICONTROL 歐洲]
   * [!UICONTROL 沙箱]

1. 按一下&#x200B;**[!UICONTROL 繼續]**&#x200B;以建立連線並返回模組。

## [!DNL Cvent]模組及其欄位

當您設定[!DNL Cvent]模組時，[!DNL Workfront Fusion]會顯示下列欄位。 除了這些欄位以外，可能還會顯示其他[!DNL Cvent]欄位，視您在應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中將資訊從一個模組對應到另一個模組。

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

此動作模組可讓您對[!DNL Cvent] API進行自訂的已驗證呼叫。 如此一來，您就可以建立其他[!DNL Cvent]模組無法完成的資料流程自動化。

當您設定此模組時，會顯示下列欄位。

模組會傳回a狀態代碼，以及API呼叫的標題和正文。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL Cvent]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">將[!DNL Cvent]連線到[!DNL Adobe Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">作業</td> 
   td&gt; <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP要求方法。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">內文(XML)</td> 
   <td> <p>輸入或對應API呼叫的正文。 這必須只包含XML。 模組會自動包含驗證標頭。 </p> </td> 
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
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL Cvent]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">將[!DNL Cvent]連線到[!DNL Adobe Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL記錄型別]</p> </td> 
   <td>選取您要讀取之記錄的專案型態。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL聯絡人] / [！UICONTROL事件] / [！UICONTROL邀請者ID]</td> 
   <td> <p>輸入或對應您要讀取的專案識別碼。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸出]</td> 
   <td> <p>選取您要納入模組輸出的欄位。 根據您選取的專案型別，可使用欄位。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 註冊受邀者]

此動作模組會為事件註冊受邀者。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL Cvent]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">將[!DNL Cvent]連線到[!DNL Adobe Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>被邀請者ID</p> </td> 
   <td> <p>輸入或對應您要註冊事件的受邀者ID。</p> </td> 
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
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL Cvent]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">將[!DNL Cvent]連線到[!DNL Adobe Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL聯絡人ID]</p> </td> 
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
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL Cvent]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">將[!DNL Cvent]連線到[!DNL Adobe Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL聯絡人ID]</td> 
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
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL Cvent]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">將[!DNL Cvent]連線到[!DNL Adobe Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL聯絡人ID]</p> </td> 
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
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL Cvent]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">將[!DNL Cvent]連線到[!DNL Adobe Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL表單ID]</p> </td> 
   <td> <p>輸入或對應您要用來建立新會議要求的表單ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL會議要求欄位]</td> 
   <td> <p>選取您要輸入資訊的會議邀請欄位，然後填寫這些欄位的所需值。</p> </td> 
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
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL Cvent]帳戶連線到[!DNL Workfront Fusion]的說明，請參閱本文中的<a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">將[!DNL Cvent]連線到[!DNL Adobe Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL記錄型別]</p> </td> 
   <td> <p>選取您要列出的記錄型別。</p> 
    <ul> 
     <li> <p>來自您[!DNL Cvent]帳戶的所有事件</p> </li> 
     <li> <p>事件的所有工作階段</p> </li> 
     <li> <p>活動的所有受邀者</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL事件ID]</td> 
   <td> <p>如果您要列出被邀請者或工作階段，請輸入或對應與被邀請者或工作階段相關聯之事件的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>
