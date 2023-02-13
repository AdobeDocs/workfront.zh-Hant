---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 連接器
navigation-topic: apps-and-their-modules
title: 事件模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用Cvent的工作流程，並將其連接至多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: c95b9764-29a5-4d8c-8e6d-68a3969129e0
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '996'
ht-degree: 1%

---

# [!DNL Cvent] 模組

在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!DNL Cvent]，並將其連接至多個協力廠商應用程式和服務。

如果您需要建立案例的相關指示，請參閱 [在中建立案例 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

如需模組的相關資訊，請參閱 [中的模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

使用 [!DNL Cvent] 模組，您必須 [!DNL Cvent] 帳戶。

## Connect [!DNL Cvent] to [!DNL Adobe Workfront Fusion] {#connect-cvent-to-adobe-workfront-fusion}

>[!NOTE]
>
>此 [!DNL Cvent] 模組通過 [!UICONTROL SOAP] API。 建立連線至 [!DNL Cvent]，您必須確保：
>
>* 您擁有 [!UICONTROL SOAP] 存取 [!DNL Cvent] API。
>* 此 [!DNL Workfront Fusion] IP位址已新增至貴組織的允許清單。
>
>  若需 [!DNL Workfront Fusion] IP位址，請參閱 [用於存取的IP位址 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)


您可以建立與 [!DNL Cvent] 直接從內部 [!DNL Cvent] 模組。

1. 在任何 [!DNL Cvent] 模組，按一下 **[!UICONTROL 新增]** 旁邊 [!UICONTROL 連線] 欄位。
1. 選擇要連接的區域。

   * [!UICONTROL 北美]
   * [!UICONTROL 歐洲]
   * [!UICONTROL Sandbox]

1. 按一下 **[!UICONTROL 繼續]** 若要建立連線，請返回模組。

## [!DNL Cvent] 模組及其欄位

設定時 [!DNL Cvent] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!DNL Cvent] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [動作](#actions)
* [搜尋](#searches)

### 動作

* [[!UICONTROL 自訂API呼叫]](#create-meeting-request)
* [[!UICONTROL 讀取記錄]](#read-a-record)
* [[!UICONTROL 註冊被邀請者]](#register-invitee)
* [[!UICONTROL 添加被邀請者]](#add-invitee)
* [[!UICONTROL 刪除連絡人]](#delete-contact)
* [[!UICONTROL 更新聯繫人]](#update-contact)
* [[!UICONTROL 建立會議請求]](#create-meeting-request)

#### [!UICONTROL 自訂API呼叫]

此動作模組可讓您對 [!DNL Cvent] API。 這樣，您就可以建立資料流自動化，而另一個無法完成 [!DNL Cvent] 模組。

設定此模組時，會顯示下列欄位。

模組會傳回狀態代碼，以及API呼叫的標題和內文。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Cvent] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] to [!DNL Adobe Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">作業</td> 
   td&gt; <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">內文(XML)</td> 
   <td> <p>輸入或對應API呼叫的內文。 這必須僅包含XML。 模組將自動包含驗證標題。 </p> </td> 
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
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Cvent] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] to [!DNL Adobe Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL記錄類型]</p> </td> 
   <td>選擇要讀取的記錄的項目類型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL聯繫人] / [!UICONTROL事件] / [!UICONTROL邀請者ID]</td> 
   <td> <p>輸入或映射要讀取的項的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸出]</td> 
   <td> <p>選取您要納入模組輸出的欄位。 欄位是根據您選取的項目類型而可用。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 註冊被邀請者]

此動作模組會為事件註冊受邀者。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Cvent] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] to [!DNL Adobe Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>被邀請者ID</p> </td> 
   <td> <p>輸入或映射要註冊事件的被邀請者的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">事件ID</td> 
   <td> <p>輸入或映射要註冊被邀請者的事件ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 添加被邀請者]

此動作模組會邀請聯絡人參與事件。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Cvent] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] to [!DNL Adobe Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL聯繫人ID]</p> </td> 
   <td> <p>輸入或映射要添加到事件的聯繫人的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL事件ID]</td> 
   <td> <p>輸入或映射要添加聯繫人的事件的ID。</p> </td> 
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
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Cvent] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] to [!DNL Adobe Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL聯繫人ID]</td> 
   <td> <p>輸入或映射要刪除的聯繫人的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新聯繫人]

此動作模組會使用現有連絡人的ID來更新。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Cvent] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] to [!DNL Adobe Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL聯繫人ID]</p> </td> 
   <td> <p>輸入或映射要更新的聯繫人的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL欄位]</td> 
   <td> <p>選取您要輸入資訊的欄位，然後填寫這些欄位的所需值。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL自定義欄位]</td> 
   <td> <p>選取您要輸入資訊的欄位，然後填寫這些欄位的所需值。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立會議請求]

此動作模組會將會議請求新增至您的帳戶。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Cvent] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] to [!DNL Adobe Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL表單ID]</p> </td> 
   <td> <p>輸入或映射要用於建立新會議請求的表單的ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL會議請求欄位]</td> 
   <td> <p>選擇要輸入資訊的會議請求欄位，然後填寫這些欄位的所需值。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL事件請求欄位]</td> 
   <td> <p>選取您要輸入資訊的事件要求欄位，然後填寫這些欄位的所需值。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL RFP請求欄位]</td> 
   <td> <p>選擇要輸入建議欄位資訊的請求，然後為這些欄位填寫所需值。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 搜尋

#### [!UICONTROL 清單記錄]

此搜索模組檢索有關特定類型的所有記錄的資訊。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL Cvent] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Connect [!DNL Cvent] to [!DNL Adobe Workfront Fusion]</a> 這篇文章。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL記錄類型]</p> </td> 
   <td> <p>選擇要列出的記錄類型。</p> 
    <ul> 
     <li> <p>來自 [!DNL Cvent] 帳戶</p> </li> 
     <li> <p>事件的所有工作階段</p> </li> 
     <li> <p>活動的所有被邀請者</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL事件ID]</td> 
   <td> <p>如果要列出邀請者或會話，請輸入或映射這些邀請者或會話關聯的事件ID。</p> </td> 
  </tr> 
 </tbody> 
</table>
