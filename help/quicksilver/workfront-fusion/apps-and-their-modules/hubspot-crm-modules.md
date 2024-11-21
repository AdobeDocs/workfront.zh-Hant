---
title: hubspot CRM模組
description: ' [!DNL Adobe Workfront Fusion] HubSpot CRM模組可讓您監視 [!DNL HubSpot CRM] 帳戶中的事件、記錄、連絡人、預約、檔案和表單提交，或建立、擷取、更新和刪除記錄、連絡人、預約、事件或檔案。'
author: Becky
feature: Workfront Fusion
exl-id: d58e0c12-a798-495c-8f88-fbf2a532f8a4
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '6411'
ht-degree: 0%

---

# [!DNL HubSpot CRM]模組

[!DNL Adobe Workfront Fusion] [!DNL HubSpot CRM]模組可讓您監視事件、記錄、連絡人、預約、檔案和表單提交，或建立、擷取、更新和刪除您[!DNL HubSpot CRM]帳戶中的記錄、連絡人、預約、事件或檔案。

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

若要使用[!DNL HubSpot CRM]模組，您必須有[!DNL HubSpot CRM]帳戶。

## HubSpot CRM API資訊

HubSpot CRM聯結器使用下列專案：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">基礎URL</td> 
   <td>https://api.hubapi.com</td> 
  </tr>
  <tr> 
   <td role="rowheader">API標籤</td> 
   <td>v2.0.14</td> 
  </tr>
 </tbody> 
 </table>

## 將[!DNL Adobe Workfront Fusion]連線至[!DNL HubSpot CRM]

如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱[建立連線到 [!DNL Adobe Workfront Fusion]  — 基本指示](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>設定連線時，請選取&#x200B;**HubSpot CRM**&#x200B;連線型別。 HubSpot CRM （已淘汰）型別支援現有連線，但我們不建議使用它來建立新連線。

## [!DNL HubSpot CRM]模組及其欄位

當您設定[!DNL Hubspot CRM]模組時，[!DNL Workfront Fusion]會顯示下列欄位。 除了這些欄位以外，可能還會顯示其他[!DNL Hubspot CRM]欄位，視您在應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中將資訊從一個模組對應到另一個模組。

![](assets/map-toggle-350x74.png)

* [crm物件](#crm-objects)
* [記錄（交易、聯絡人和公司）](#records-deals-contacts-and-companies)
* [連絡人](#contacts)
* [交易](#deals)
* [公司](#companies)
* [參與](#engagements)
* [事件與通知](#events-and-notifications)
* [檔案](#files)
* [任務](#tasks)
* [使用者](#users)
* [票證](#tickets)
* [表格](#forms)
* [社群媒體（廣播）](#social-media-broadcast)
* [部落格](#blog-posts)
  <!--* [Workflows]-->
* [訂閱](#subscriptions)
  <!--* [Associations](#associations)-->
* [其他](#other)

+++**CRM物件**

### crm物件

* [搜尋CRM物](#search-for-crm-objects)
* [觀看CRM物件](#watch-crm-objects)

#### [!UICONTROL 搜尋CRM物件]

此搜尋模組會依自訂屬性或查詢來搜尋CRM物件。 若要搜尋產品或條列專案，請使用具有所需自訂範圍的特殊連線。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td>輸入或對應模組在一個執行週期內傳回的最大專案數。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">要搜尋的[！UICONTROL物件型別]</td> 
   <td>選取您要搜尋的Hubspot CRM物件型別。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸出屬性]</td> 
   <td>選取您要顯示在模組輸出中的屬性。 可用的欄位取決於您選取的物件。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL篩選依據] </td> 
   <td> <p>選取您要如何篩選搜尋</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL查詢]</strong> </p> <p>輸入或對映查詢</p> </li> 
     <li> <p><strong>[！UICONTROL屬性]</strong> </p> <p>輸入搜尋的群組或篩選器。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL排序依據]</td> 
   <td> <p>如果要排序結果，請按一下。 如果您選擇排序結果，則會顯示下列欄位。 </p> 
    <ul> 
     <li> <p><strong>[！UICONTROL屬性名稱]</strong> </p> <p>選取您要用來排序結果的屬性</p> </li> 
     <li> <p><strong>[！UICONTROL方向]</strong> </p> <p>選擇您要以遞增或遞減方向排序結果。</p> </li> 
    </ul> </td> 
  </tr> 
   <tr> 
    <td role="rowheader">開始位移</td> 
    <td>輸入或對應您要擷取其詳細資訊的第一個專案ID。 此模組一次最多只會傳回5000個結果。 設定起始位移可讓您擷取前5000個專案以外的專案。 如果起始位移為5000，模組會傳回專案5000-9999。</td> 
   </tr>
 </tbody> 
</table>

#### 觀看CRM物件

此觸發模組會在建立或更新CRM物件時啟動案例。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td>輸入或對應模組在一個執行週期內傳回的最大專案數。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">要搜尋的[！UICONTROL物件型別]</td> 
   <td> <p>選取您要搜尋的物件型別。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸出屬性]</td> 
   <td>選取您要包含在此模組輸出中的屬性。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL已建立/已更新]</td> 
   <td>選取您要觀看建立的（新）物件或更新的（已修改）物件。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL篩選依據]</td> 
   <td>您可以新增篩選器，以確保案例只會在符合某些條件時開始。<ul><li><b>查詢</b><p>輸入您要依據的查詢。</li><li><b>屬性</b><p>針對您想要用來篩選結果的每個屬性，按一下<b>新增專案</b>並輸入屬性名稱、運運算元及屬性值。</td> 
  </tr> 
 </tbody> 
</table>

+++

+++**筆記錄（交易、連絡人和公司）**

### 記錄（交易、聯絡人和公司）

* [建立記錄](#create-a-record)
* [[!UICONTROL 建立記錄（舊版）]](#create-a-record-legacy)
* [[!UICONTROL 刪除記錄]](#delete-a-record)
* [[!UICONTROL 取得記錄]](#get-a-record)
* [[!UICONTROL 取得記錄屬性]](#get-a-record-property)
* [清單記錄](#list-records)
* [[!UICONTROL 更新記錄]](#update-a-record)
* [[!UICONTROL 觀看記錄]](#watch-records)

#### 建立記錄

此動作模組會建立聯絡人、公司或交易。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別]</td> 
   <td> <p>選取您要建立的記錄型別。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL屬性群組]</td> 
   <td>對於建立記錄時想要新增的每個屬性，選取屬性所在的群組。 屬性群組將會開啟，然後您可以填入屬性的值。 可用的屬性群組和屬性取決於您要建立的記錄型別。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立記錄（舊版）]

此動作模組會建立聯絡人、公司或交易。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別]</td> 
   <td> <p>選取您要建立的記錄型別。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL屬性]</td> 
   <td>填寫您要為記錄設定的任何屬性。 可用欄位取決於您要建立的記錄型別。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除記錄]

此動作模組會刪除連絡人、公司或交易。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別]</td> 
   <td>選取您要刪除的記錄型別。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL ID]</td> 
   <td>輸入您要刪除的連絡人、公司或交易的識別碼。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得記錄]

此動作模組會取得聯絡人、公司或交易的詳細資料。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別]</td> 
   <td> <p>選取記錄型別。</p> 
    <ul> 
     <li>[！UICONTROL連絡人]</li> 
     <li>[！UICONTROL公司] </li> 
     <li>[！UICONTROL交易]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL搜尋型別]</td> 
   <td>如果您有連絡人，請選取您要以ID或電子郵件地址來識別。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL ID]</td> 
   <td>輸入您要擷取之聯絡人、公司或交易的識別碼。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL電子郵件]</td> 
   <td>輸入您要擷取其詳細資訊之連絡人的電子郵件地址。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得記錄屬性]

此動作模組透過其（內部）名稱取得特定記錄屬性的中繼資料。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別]</td> 
   <td>選取具有您要擷取中繼資料之屬性的記錄型別。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL屬性名稱]</td> 
   <td>選取您要擷取中繼資料的屬性。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL選項ID]</td> 
   <td> <p> 有些屬性具有一組可用選項，使用者可選取這些選項作為屬性值。 輸入代表您要擷取之屬性值的選項ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### 清單記錄

此搜尋模組會傳回聯絡人、公司或交易的清單。 輸出限製為5000個連絡人、12,500家公司或12,500筆交易。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL型別]</td> 
   <td> <p>選取您要傳回的記錄型別。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸出屬性]</td> 
   <td>選取您要包含在此模組輸出中的屬性。</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</p> </td> 
  </tr>

</tbody> 
</table>

#### [!UICONTROL 更新記錄]

此動作模組會更新聯絡人、公司或交易。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別]</td> 
   <td>選取您要更新的記錄型別。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL搜尋型別]</td> 
   <td> <p>如果您要取得連絡人，請選取您要如何識別記錄：</p> 
    <ul> 
     <li> <p>[！UICONTROL ID]</p> </li> 
     <li> <p>[！UICONTROL電子郵件]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL ID]</td> 
   <td>輸入您要更新的聯絡人、公司或交易的識別碼。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL電子郵件]</td> 
   <td>輸入您要更新其詳細資訊之連絡人的電子郵件地址。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL屬性]</td> 
   <td>填寫您要為記錄設定的任何屬性。 可用欄位取決於您要建立的記錄型別。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 觀看記錄]

在過去30天內修改或建立連絡人、公司或交易時，此觸發模組就會開始案例。 輸出限製為10,000筆記錄。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別]</td> 
   <td>選取具有您要觀看之屬性的記錄型別。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL搜尋]</td> 
   <td>選取您要觀看最近修改或最近建立的記錄。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸出屬性]</td> 
   <td>選取要包含在模組輸出中的屬性。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**連絡人**

### 連絡人

* [[!UICONTROL 新增連絡人至清單]](#add-contacts-to-a-list)
* [建立/更新連絡人](#createupdate-a-contact)
* [[!UICONTROL 建立/更新連絡人（舊版）]](#createupdate-a-contact-legacy)
* [[!UICONTROL 建立/更新連絡人群組]](#createupdate-a-group-of-contacts)
* [[!UICONTROL 列出連絡人]](#list-contacts)
* [[!UICONTROL 列出公司的連絡人]](#list-contacts-of-a-company)
* [[!UICONTROL 合併連絡人]](#merge-contacts)
* [[!UICONTROL 從清單移除連絡人]](#remove-a-contact-from-a-list)
* [[!UICONTROL 搜尋連絡人]](#search-for-contacts)
* [觀看新增至清單的連絡人](#watch-contacts-added-to-a-list)

#### [!UICONTROL 新增連絡人至清單]

此模組會將系統中已建立的連絡人記錄新增至連絡人清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL清單ID] </td> 
   <td>選取您要新增連絡人的清單識別碼。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL ID/電子郵件] </td> 
   <td> <p>選取要如何識別要新增至清單的連絡人：</p> 
    <ul> 
     <li> <p>[！UICONTROL IDs]</p> <p>新增您要新增至清單的連絡人ID。</p> </li> 
     <li> <p>[！UICONTROL電子郵件]</p> <p>新增您要新增至清單的連絡人電子郵件地址。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### 建立/更新連絡人

如果連絡人不存在入口網站中，此動作模組會建立連絡人。 如果入口網站中確實有連絡人，此模組會以提供的值更新連絡人。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL屬性群組]</td> 
   <td>對於建立連絡人時要新增的每個屬性，請選取屬性所在的群組。 屬性群組將會開啟，然後您可以填入屬性的值。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立/更新連絡人（舊版）]

如果入口網站中不存在連絡人，則建立連絡人；如果入口網站中不存在連絡人，則使用最新屬性值更新連絡人。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL屬性]</td> 
   <td>填寫您要設定或更新連絡人的任何屬性。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立/更新連絡人群組]

建立連絡人群組或更新連絡人（如果已經存在）。 當批次大小限製為100個或更少聯絡人時，效能最佳。 透過此端點進行的變更會以非同步方式處理，因此可能需要幾分鐘的時間才能將變更套用至聯絡人記錄。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL要建立/更新的連絡人批次] </td> 
   <td> <p>新增批次連絡人。</p> <p>按一下<strong>[！UICONTROL新增專案]</strong>以新增連絡人。 在出現的視窗中，輸入或對應下列資訊：</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL搜尋型別]</strong> </p> <p>選取您要如何識別連絡人：</p> 
      <ul> 
       <li> <p>[！UICONTROL ID]</p> <p>輸入要建立或更新之連絡人的識別碼。 </p> </li> 
       <li> <p>[！UICONTROL電子郵件]</p> <p>輸入您要建立或更新之連絡人的電子郵件地址。 </p> </li> 
      </ul> </li> 
     <li> <p><strong>[！UICONTROL屬性]</strong> </p> <p>填寫您要設定或更新連絡人的任何屬性。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出連絡人]

傳回入口網站中建立的所有連絡人。 輸出限製為5000個連絡人。 若要列出上一個或下一個連絡人，您可以使用[!UICONTROL 進階]引數來位移清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td>一個案例執行週期內應傳回的聯絡人數目上限[!DNL Workfront Fusion]。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸出屬性]</td> 
   <td>選取您要顯示在模組輸出中的屬性。 </td> 
  </tr> 
   <tr> 
    <td role="rowheader">聯絡人ID [開始位移] </td> 
    <td>輸入或對應您要啟動清單之使用者的ID。 例如，將連絡人ID設定為第101位連絡人的ID將允許模組列出連絡人101-5100，而非1-5000。 </td> 
   </tr>
 </tbody> 
</table>

#### [!UICONTROL 列出公司的連絡人]

擷取公司中的聯絡人清單。 輸出限製為5000個連絡人。 若要列出上一個或下一個連絡人，您可以使用[!UICONTROL 進階]引數來位移清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL ID]</td> 
   <td>輸入要列出其聯絡人的公司ID。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td>一個案例執行週期內應傳回的聯絡人數目上限[!DNL Workfront Fusion]。 </td> 
  </tr> 
   <tr> 
    <td role="rowheader">聯絡人ID [開始位移] </td> 
    <td>輸入或對應您要啟動清單之使用者的ID。 例如，將連絡人ID設定為第101位連絡人的ID將允許模組列出連絡人101-5100，而非1-5000。 </td> 
   </tr>
 </tbody> 
</table>

#### [!UICONTROL 合併連絡人]

此動作模組會合併連絡人

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL ID 1] </td> 
   <td>輸入您要合併之連絡人的識別碼。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL ID 2] </td> 
   <td>輸入您要合併的其他連絡人的ID。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 從清單移除連絡人]

從連絡人清單移除連絡人。

>[!NOTE]
>
>您無法從動態清單中手動移除連絡人。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL清單ID] </td> 
   <td>選取您要移除連絡人的清單識別碼。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL聯絡人ID] </td> 
   <td>輸入您要從清單中移除之連絡人的ID。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 搜尋連絡人]

使用搜尋查詢來擷取連絡人清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Query]</td> 
   <td>輸入搜尋查詢。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制] </td> 
   <td>輸入或對應在一個案例執行週期內應傳回的聯絡人數目上限[!DNL Workfront Fusion]。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 觀看連絡人已新增至清單]

此觸發模組會在清單中新增連絡人時啟動案例。 此僅供擁有付費行銷帳戶的使用者使用。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL清單ID]</td> 
   <td>輸入或對應包含您要觀看之連絡人的清單ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸出屬性]</td> 
   <td>選取要包含在模組輸出中的屬性。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**個交易**

### 交易

* [[!UICONTROL 取得交易的CRM管道]](#get-a-deals-crm-pipeline)
* [[!UICONTROL 列出交易/票證管道]](#list-dealticket-pipelines)

#### [!UICONTROL 取得交易的CRM管道]

傳回特定交易管道。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL管道ID] </td> 
   <td>輸入或對應您要擷取詳細資訊的管道ID。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL階段ID] </td> 
   <td>輸入或對應您要擷取詳細資訊的階段ID。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出交易/票證管道]

傳回給定入口網站的所有交易和票證管道。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL物件型別] </td> 
   <td>選取您要列出交易或票證。</td> 
  </tr> 
 </tbody> 
</table>

+++

+++**公司**

### 公司

#### [!UICONTROL 依網域搜尋公司]

根據與網域屬性的完全相符專案擷取公司清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL網域] </td> 
   <td>輸入您要搜尋的公司網域，例如<code>[!DNL hubspot].com</code>。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td>在一個案例執行週期內應傳回的公司數目上限[!DNL Workfront Fusion]。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸出屬性]</td> 
   <td>選取您要顯示在模組輸出中的屬性。 </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**參與**

### 參與

* [將參與與CRM物件建立關聯](#associate-an-engagement-with-a-crm-object)
* [建立參與](#create-an-engagement)
* [刪除參與](#delete-an-engagement)
* [Watch參與](#watch-engagements)

#### 將參與與CRM物件建立關聯

此動作模組會將參與和聯絡人、公司或交易建立關聯。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL型別]</td> 
   <td>選取您要與參與建立關聯的CRM記錄型別。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL參與ID]</td> 
  <td>輸入或對應您要與物件關聯的參與ID。</td> 
   </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄ID]</td> 
  <td>輸入或對應您要與參與產生關聯的記錄ID。</td> 
   </tr> 
 </tbody> 
</table>

#### 建立參與

此動作模組會在HubSpot中建立具有CRM物件的參與（例如附註、任務或活動）。 參與是指與應登入CRM之連絡人的任何互動。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL是否啟用？]</td> 
   <td>如果新參與在建立時處於活動狀態，則啟用此選項。 參與必須為作用中狀態，才能顯示在時間軸中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL型別]</td> 
  <td>選取您要建立的參與型別。
  <ul>
  <li><b>電子郵件</b><p></p>繼續<a href="#email-metadata" class="MCXref xref" >電子郵件中繼資料</a>。</p></li>
  <li><b>呼叫</b><p>繼續<a href="#call-metadata" class="MCXref xref" >呼叫中繼資料</a>。</p></li>
  <li><b>會議</b><p>繼續<a href="#meeting-fields" class="MCXref xref" >會議欄位</a>。</p></li>
  <li><b>任務</b><p>繼續到<a href="#task-fields" class="MCXref xref" >工作欄位</a>。</p></li>
  <li><b>備註</b><p>在「內文」欄位中，輸入註記文字。</p></li>
  </ul>
  </td> 
   </tr> 
  <tr> 
   <td role="rowheader">時間戳記</td> 
   <td>輸入或對應參與的時間戳記。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">所有者 ID</td> 
   <td>輸入或對應預訂將指派至的人員之擁有者ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">UID</td> 
   <td>輸入或對應可用於各種物件型別的參與ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">入口網站ID</td> 
   <td>輸入或對應入口網站的ID。 如果您的組織有多個入口網站，這會很有用。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">關聯的連絡人</td> 
   <td>針對您想要與此參與關聯的每個連絡人，按一下<b>新增專案</b>並輸入連絡人識別碼。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">關聯公司</td> 
   <td>針對您想要與這個參與建立關聯的每個公司，按一下[新增專案] <b>並輸入公司ID。</b></td> 
  </tr> 
  <tr> 
   <td role="rowheader">關聯交易</td> 
   <td>針對您想要與此參與關聯的每個交易，按一下<b>新增專案</b>並輸入交易識別碼。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">關聯的票證</td> 
   <td>針對您想要與此參與關聯的每個票證，按一下<b>新增專案</b>並輸入票證ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">附件</td> 
   <td>針對您想要與此參與關聯的每個附件，按一下[新增專案] <b> </b>，然後輸入要附加檔案的檔案識別碼。</td> 
  </tr> 
 </tbody> 
</table>

##### 電子郵件中繼資料

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[！UICONTROL From &gt; Email]</p> </td> 
   <td> <p>輸入或對應寄出電子郵件的電子郵件地址。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL名字]</td> 
   <td>輸入或對應電子郵件寄件者的名字。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL姓氏]</td> 
  <td>輸入或對應電子郵件寄件者的姓氏。
  </td> 
   </tr> 
  <tr> 
   <td role="rowheader">到</td> 
   <td>針對您想要傳送電子郵件的每個電子郵件地址，按一下[新增專案] <b> </b>，然後輸入或對應電子郵件地址。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Cc</td> 
   <td>針對您想要寄送電子郵件的每個電子郵件地址，按一下<b>新增專案</b>，然後輸入或對應電子郵件地址。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">密件副本</td> 
   <td>針對您想要以密件副本寄送電子郵件的每個電子郵件地址，按一下<b>新增專案</b>，然後輸入或對應電子郵件地址。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">主旨</td> 
   <td>輸入或對應電子郵件主旨的文字</td> 
  </tr> 
  <tr> 
   <td role="rowheader">HTML</td> 
   <td>若要傳送HTML格式的電子郵件，請輸入或對映電子郵件內文，包括HTML標籤。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">文字</td> 
   <td>若要傳送純文字電子郵件，請輸入或對應電子郵件內文的文字。</td> 
  </tr> 
 </tbody> 
</table>

##### 呼叫中繼資料

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[！UICONTROL至Number]</p> </td> 
   <td> <p>輸入或對應來電的目標電話號碼。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL From Number]</td> 
   <td>輸入或對應撥打該電話的電話號碼。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL狀態]</td> 
  <td>選取通話狀態。
  </td> 
   </tr> 
  <tr> 
   <td role="rowheader">內文</td> 
   <td>輸入或對應呼叫的詳細資訊或附註。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">外部 ID</td> 
   <td>此欄位代表在HubSpot中所進行呼叫的內部ID。 不需要採取任何動作。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">期間</td> 
   <td>輸入或對應呼叫的長度（以毫秒為單位）</td> 
  </tr> 
  <tr> 
   <td role="rowheader">外部帳戶ID</td> 
   <td>此欄位代表在HubSpot中進行的呼叫的內部帳戶ID。 不需要採取任何動作。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">錄製URL</td> 
   <td>輸入或對應錄製檔案的URL。</td> 
  </tr> 
 </tbody> 
</table>

##### 會議欄位

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[！UICONTROL標題]</p> </td> 
   <td> <p>輸入或對映會議的標題或主旨。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Body]</td> 
   <td>輸入或對應會議說明或詳細資訊的文字。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL開始時間]</td> 
  <td>輸入或對應會議開始時間作為UNIX時間戳記。
  </td> 
   </tr> 
  <tr> 
   <td role="rowheader">結束時間</td> 
   <td>輸入或對應會議結束時間作為UNIX時間戳記。</td> 
  </tr> 
 </tbody> 
</table>

##### 工作列位

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[！UICONTROL主旨]</p> </td> 
   <td> <p>輸入或對映工作的標題或主旨。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Body]</td> 
   <td>輸入或對應工作說明或詳細資訊的文字。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">狀態</td> 
   <td>選取工作的狀態。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL For Object Type]</td> 
  <td>輸入<code>CONTACT</code>或<code>COMPANY</code>。
  </td> 
   </tr> 
 </tbody> 
</table>

#### 刪除參與

此動作模組會依ID刪除參與。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL檔案ID]</td> 
   <td>輸入或對應您要刪除的參與ID。</td> 
  </tr> 
 </tbody> 
</table>

#### Watch參與

此觸發模組會在入口網站中建立新參與時開始案例。 此模組僅傳回過去30天內建立的記錄，或最近建立的10,000筆記錄。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td>在一個案例執行週期內應傳回的公司數目上限[!DNL Workfront Fusion]。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL始自]</td> 
   <td>輸入或對應您要觀看事件的最早日期。 使用格式<code>MM/DD/YYYY h:mm</code>。</td> 
  </tr> 
 </tbody> 
</table>

+++

+++**個事件和通知**

### 事件與通知

* [建立/更新時間表事件](#create--update-a-timeline-event)
* [列出時間表事件型別](#list-timeline-event-types)
* [觀看行事曆事件](#watch-calendar-events)
* [Watch通知](#watch-notifications)

#### 建立/更新時間表事件

此動作模組會建立或更新時間表事件。 此模組只能與包含使用者識別碼、HubSpot API金鑰、使用者端ID和使用者端密碼的開發人員連線一起使用。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL應用程式ID]</td> 
   <td>輸入或對應此事件所屬之應用程式的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL事件ID]</td> 
   <td>輸入或對應此事件的ID。 系統不會產生事件ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL事件型別ID]</td> 
   <td>輸入或對應此事件事件事件型別的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL電子郵件]</td> 
   <td>輸入或對應您要建立事件的連絡人電子郵件地址。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL物件ID]</td> 
   <td>輸入或對應您要建立事件的連絡人ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL時間戳記]</td> 
   <td>輸入或對應此事件的時間戳記。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL自訂資料]</td> 
   <td>針對您想要新增至此事件的每個自訂資料專案，按一下<b>新增專案</b>並輸入專案的名稱和值。</td> 
  </tr> 
 </tbody> 
</table>

#### 列出時間表事件型別

此搜尋模組會傳回特定應用程式的所有時間表事件清單。 此模組只能與包含使用者識別碼、HubSpot API金鑰、使用者端ID和使用者端密碼的開發人員連線一起使用。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL應用程式ID]</td> 
   <td>輸入或對應此事件所屬之應用程式的ID。 </td> 
  </tr> 
 </tbody> 
</table>

#### 觀看行事曆事件

此觸發模組會在新事件新增至行事曆時啟動案例。 它包含最多500個介於開始和結束日期之間的任務。 此模組只能與包含使用者識別碼、HubSpot API金鑰、使用者端ID和使用者端密碼的開發人員連線一起使用。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL事件型別]</td> 
   <td>選取您要觀看社交活動、內容活動或所有活動。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大檔案數。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL開始日期]</td> 
   <td>輸入或對映開始日期。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL結束日期]</td> 
   <td>輸入或對映結束日期。</td> 
  </tr> 
 </tbody> 
</table>

#### Watch通知

此觸發模組會在傳送有關變更的新通知時啟動案例。  它包含最多500個介於開始和結束日期之間的任務。 此模組只能與包含使用者識別碼、HubSpot API金鑰、使用者端ID和使用者端密碼的開發人員連線一起使用。 在HubSpot中，每個開發人員應用程式只能有一個webhook URL。

若要建立此模組的webhook，請按一下webhook欄位旁的&#x200B;**新增**，並填寫下列欄位：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL應用程式ID]</td> 
   <td>輸入您要用於此webhook的應用程式ID。 您可以在您的HubSpot開發人員入口網站中找到該ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL訂閱]</td> 
   <td> <p>針對您要觀看的每種通知型別，按一下<b>新增專案</b>並選取訂閱型別。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL強制移除舊訂閱]</td> 
   <td>啟用此選項以分離或刪除附加到此webhook的舊訂閱。</td> 
  </tr> 
 </tbody> 
</table>

+++

+++**檔案**

### 檔案

* [[!UICONTROL 建立資料夾]](#create-a-folder)
* [刪除檔案](#delete-a-file)
* [[!UICONTROL 刪除資料夾]](#delete-a-folder)
* [清單檔案](#list-files)
* [[!UICONTROL 移動檔案]](#move-a-file)
* [上傳檔案](#upload-a-file)
* [觀看檔案](#watch-files)

#### [!UICONTROL 建立資料夾]

此模組會建立資料夾。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資料夾名稱] </td> 
   <td>輸入或對應新資料夾的名稱。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL父資料夾ID] </td> 
   <td>選取您要建立之資料夾的父資料夾ID。 </td> 
  </tr> 
 </tbody> 
</table>

#### 刪除檔案

此動作模組會從檔案管理員永久刪除檔案及所有相關資料和縮圖。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL檔案ID]</td> 
   <td>輸入或對應您要刪除之檔案的ID。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除資料夾]

將資料夾標籤為已刪除。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL ID]</td> 
   <td>輸入或對應您要刪除的資料夾識別碼。</td> 
  </tr> 
 </tbody> 
</table>

#### 清單檔案

此搜尋模組會傳回儲存在檔案管理員中的檔案清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大檔案數。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資料夾ID]</td> 
   <td>輸入或對應包含您要列出之檔案的資料夾識別碼。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL篩選器]</td> 
   <td>若只要在檔案名稱中包含包含特定字元的檔案，請輸入或對應您要檔案名稱包含的字元。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 移動檔案]

將檔案移至其他資料夾。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL檔案ID] </td> 
   <td>輸入或對應您要移動之檔案的ID。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資料夾ID] </td> 
   <td>選取您要移動檔案的資料夾識別碼。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL名稱]</td> 
   <td>輸入已移動檔案的名稱。</td> 
  </tr> 
 </tbody> 
</table>

#### 上傳檔案

此動作模組會將檔案上傳至檔案管理員。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Source檔案]</td> 
   <td> <p>從先前的模組中選取來源檔案，或對應來源檔案的名稱和資料。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL存取型別] </td> 
   <td>選取您要讓檔案為私人、公用，但不可索引，或是公用，且可索引。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資料夾ID] </td> 
   <td>選取您要上傳檔案的資料夾識別碼。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL覆寫]</td> 
   <td>啟用此選項以覆寫資料夾中已存在的檔案。</td> 
  </tr> 
 </tbody> 
</table>

### 觀看檔案

此觸發模組會在新檔案儲存至檔案管理員時啟動案例。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大檔案數。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL資料夾ID]</td> 
   <td>輸入或對應包含要監視之檔案的資料夾識別碼。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL篩選器]</td> 
   <td>若只要在檔案名稱中包含包含特定字元的檔案，請輸入或對應您要檔案名稱包含的字元。</td> 
  </tr> 
 </tbody> 
</table>

+++

+++**任務**

### 任務

* [建立行事曆任務](#create-a-calendar-task)
* [刪除行事曆任務](#create-a-calendar-task)
* [觀看任務事件](#watch-task-events)

#### 建立行事曆任務

此動作模組會為行事曆建立新任務。 此模組中使用的連線必須使用擁有付費行銷帳戶之使用者的認證。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL名稱]</td> 
   <td>輸入或對應新行事曆工作的名稱。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL說明]</td> 
   <td>輸入或對應新行事曆工作的描述。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL擁有者ID]</td> 
   <td>輸入或對應指派給此任務之使用者的擁有者ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL事件日期]</td> 
   <td>輸入或對應此工作的日期。<p>如需支援的日期和時間格式清單，請參閱<a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中鍵入強制。</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL類別]</td> 
   <td>選取事件型別。<ul><li><b>部落格貼文</b><p>輸入內容群組識別碼。 這是部落格頁面的ID。</p></li><li><b>電子郵件</b><p>輸入或對應您要使用之電子郵件範本的路徑。</li><li><b>登陸頁面</b><p>輸入路徑或對映至您要使用的登入頁面範本。</li><li><b>自訂</b></li><ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL狀態]</td> 
   <td>輸入事件是否處於「待辦事項」或「完成」狀態。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL促銷活動GUID]</td> 
   <td>輸入或對應此事件所屬促銷活動的內部HubSpot ID。</td> 
  </tr> 
 </tbody> 
</table>

#### 刪除行事曆任務

此動作模組會刪除行事曆工作。 此模組中使用的連線必須使用擁有付費行銷帳戶之使用者的認證。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL ID]</td> 
   <td>輸入或對應您要刪除之工作的ID。</td> 
  </tr> 
 </tbody> 
</table>

#### 觀看任務事件

當行事曆中有新任務事件時，此觸發模組會啟動案例。 此模組中使用的連線必須使用擁有付費行銷帳戶之使用者的認證。 模組最多可傳回500個事件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>輸入或對應您希望模組在每個案例執行週期中傳回的最大檔案數。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL開始日期]</td> 
   <td>輸入或對應您要觀看事件的最早日期。 使用格式<code>MM/DD/YYYY h:mm</code>。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL結束日期]</td> 
   <td>輸入或對應您要觀看活動的最新日期。 使用格式<code>MM/DD/YYYY h:mm</code>。</td> 
  </tr> 
 </tbody> 
</table>

+++

+++**使用者**

### 使用者

* [取得擁有者](#get-an-owner)
* [清單擁有者](#list-owners)

#### 取得擁有者

此動作模組會傳回擁有者的詳細資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL擁有者ID]</td> 
   <td> <p>輸入或對應您要傳回詳細資訊之擁有者的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### 清單擁有者

此搜尋模組會傳回HubSpot帳戶中所有擁有者的清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**票**

### 票證

<!--* [Create a Ticket]-->
* [刪除票證](#delete-a-ticket)
  <!--* [Create a Ticket]-->
  <!--* [Create a Ticket]-->
  <!--* [Create a Ticket]-->
  <!--* [Create a Ticket]-->

<!-- Create a Ticket Need to find a working connection-->

#### [!UICONTROL 刪除票證]

依其ID刪除現有票證。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL ID]</td> 
   <td>輸入您要刪除的票證ID。 </td> 
  </tr> 
 </tbody> 
</table>

<!-- Get a Ticket  Need to find a working connection-->

<!-- List Tickets  Need to find a working connection-->

&lt;！ — 更新票證需要找到有效的連線 — >

<!-- Watch Tickets Need to find a working connection-->

+++

+++**Forms**

### 表格

* [透過表單上傳檔案](#get-a-file-uploaded-via-form)
* [列出Forms](#list-forms)
  <!--* [Submit Data to a Form]-->
  <!--* [Watch Submissions for a Form]-->

#### 透過表單上傳檔案

此動作模組會傳回透過表單上傳的檔案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL檔案URL]</td> 
   <td>輸入或對應您要擷取的檔案URL。 這可在表單中繼資料中找到。</td> 
  </tr> 
 </tbody> 
</table>

#### 列出Forms

此動作模組會傳回在與用於此模組的連線相關聯的帳戶中建立的所有表單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td>輸入或對應模組在一個執行週期內傳回的最大表單數量。</td> 
  </tr> 
 </tbody> 
</table>

<!--#### Submit Data to a Form Need to find a working connection-->



&lt;！—####觀看表單提交 — 需要尋找有效連線>—>

+++

+++**社群媒體（廣播）**

### 社群媒體（廣播）

* [取消廣播訊息](#cancel-a-broadcast-message)
* [建立廣播訊息](#create-a-broadcast-message)
* [觀看廣播訊息](#watch-broadcast-messages)

#### 取消廣播訊息

此動作模組會取消已排程的廣播，例如推文或Facebook貼文。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL廣播ID]</td> 
   <td>輸入或對應您要取消的廣播ID。</td> 
  </tr> 
 </tbody> 
</table>

#### 建立廣播訊息

此動作模組會在指定的社群媒體頻道上建立並立即發佈訊息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL管道ID]</td> 
   <td>輸入或對應您要用於此廣播的頻道ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL標題]</td> 
   <td>輸入或對應此廣播的標題。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Body]</td> 
   <td>輸入或對映廣播的文字。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL像片URL]</td> 
   <td>輸入或對應您要納入廣播之像片的URL。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL縮圖URL]</td> 
   <td>輸入或對應您要用於此廣播的縮圖URL。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL觸發於]</td> 
   <td>輸入或對應您要傳送廣播的日期和時間。 如果將此項保留為空白，則會立即傳送廣播。<p>如需支援的日期和時間格式清單，請參閱<a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中鍵入強制。</p></td> 
  </tr> 
 </tbody> 
</table>

#### 觀看廣播訊息

從HubSpot張貼訊息至指定的社群媒體頻道時，此觸發模組就會開始案例。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td>輸入或對應模組在一個執行週期內傳回的最大專案數。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL按狀態篩選]</td> 
   <td>若要只在訊息處於特定狀態時啟動案例，請選取狀態。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL依據管道的篩選器]</td> 
   <td>若要只在訊息位於特定頻道時啟動案例，請選取頻道。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL廣播ID]</td> 
   <td>若要只在訊息位於特定日期當天或之後才開始此案例，請以<code>MM/DD/YYYY</code>格式輸入或對應日期。</td> 
  </tr> 
 </tbody> 
</table>

+++

+++**部落格**

### 部落格貼文

<!--* [Create a Blog Post]-->
* [刪除部落格](#delete-a-blog-post)
  <!--* [List Blog Posts]-->
* [Publish/取消發佈部落格](#publish--unpublish-a-blog-post)
  <!--* [Watch Blog Posts]-->

<!--
#### Create a Blog Post May need connection
-->


#### 刪除部落格

此動作模組會刪除單一部落格。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL ID]</td> 
   <td>輸入或對應您要刪除之部落格的識別碼。</td> 
  </tr> 
 </tbody> 
</table>

<!--#### List Blog Posts May need connection

This search module retrieves posts from a HubSpot blog.-->

#### Publish /取消發佈部落格

此動作模組會排程或取消發佈部落格。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL ID]</td> 
   <td>輸入或對應您要排程或取消之部落格的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL動作]</td> 
   <td>選取是否要排程部落格，或取消先前排程的部落格。</td> 
  </tr> 
 </tbody> 
</table>

<!--#### Watch Blog PostsMay need connection-->

+++

<!--+++**Workflows**>

<!--### Workflows May need connection

#### Add a Contact to a Workflow


#### Remove a Contact from a Workflow

-->

<!--+++-->

+++**訂閱**

### 訂閱

* [更新電子郵件訂閱](#update-email-subscription)
* [觀看入口網站的訂閱時間表](#watch-subscriptions-timeline-for-a-portal)

#### 更新電子郵件訂閱

此動作模組會更新HubSpot中的電子郵件訂閱。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL電子郵件]</td> 
   <td>輸入或對應您要更新之訂閱的電子郵件地址。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL狀態]</td> 
   <td>針對您想要更新訂閱的每個狀態，按一下<b>新增專案</b>，然後輸入狀態識別碼，以及電子郵件地址是否會訂閱該狀態。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL入口網站訂閱法律狀態]</td> 
   <td>若要記錄此訂閱的GDPR法律依據，請選取此訂閱的法律狀態。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL入口網站訂閱法律基礎說明]</td> 
   <td>若要新增此訂閱之GDPR法律基礎的相關備註，請輸入或對應備註文字。</td> 
  </tr> 
 </tbody> 
</table>

#### 觀看入口網站的訂閱時間表

此觸發模組會在新的電子郵件時間表訂閱新增至入口網站時啟動案例。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td>輸入或對應模組在一個執行週期內傳回的最大專案數。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL開始時間戳記]</td> 
   <td>若要傳回特定日期當天或之後的結果，請以格式輸入日期 <code>MM/DD/YYYY.</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL結束時間戳記]</td> 
   <td>若要傳回特定日期當天或之前的結果，請以格式輸入日期 <code>MM/DD/YYYY.</code></td> 
  </tr> 
 </tbody> 
</table>

+++

<!--+++**Associations**-->

<!--### Associations-->

<!--#### Associate CRM Objects  May need connection

This action module associates two CRM objects.-->

<!--#### Associate Multiple CRM Objects  May need connection-->



<!--#### Delete an Association May need connection-->



<!--#### Delete Multiple Associations between CRM Objects May need connection-->



<!--#### List Associations for a CRM Object May need connection-->

<!--+++-->

+++**其他**

### 其他

#### [!UICONTROL 進行API呼叫]

可讓您執行自訂API呼叫。

>[!NOTE]
>
>下列端點已於2023年8月31日在HubSpot API中遭到取代，因此無法再用於Fusion模組。
>
>* 列出內容事件
>* 列出社交活動
>* 列出行事曆任務事件
>* 列出所有行事曆事件
>* 建立行事曆任務
>* 依ID取得行事曆工作
>* 更新行事曆任務
>* 刪除行事曆任務

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL HubSpot CRM]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與[!DNL Adobe Workfront Fusion]的連線 — 基本指示</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL URL]</p> </td> 
   <td> <p>輸入相對於https://api.hubapi.com/的路徑。 例如， /contacts/v1/lists/all/contacts/all</p> <p>如需可用端點的清單，請參閱<a href="https://legacydocs.hubspot.com/docs/overview">[!DNL HubSpot] API檔案</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL方法]</p> </td> 
   <td> <p>選取您要使用的HTTP方法：</p> <p>[！UICONTROLGET]</p> <p>以擷取專案的資訊。</p> <p>[！UICONTROLPOST]</p> <p>以建立新專案。</p> <p>[！UICONTROLPUT]</p> <p>更新/取代現有專案。</p> <p>[！UICONTROLPATCH]</p> <p>進行部份專案更新。</p> <p>[！UICONTROLDELETE]</p> <p>刪除專案。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers]</td> 
   <td> <p> 輸入所需的請求標頭。 您不需要新增授權標頭；我們已為您完成此操作。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查詢字串]</td> 
   <td> <p> 輸入請求查詢字串。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Body]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的內文內容。在JSON中使用條件陳述式（例如<code>if</code>）時，請將引號放在條件陳述式之外。<img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"></p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**範例：**&#x200B;下列API呼叫傳回您[!DNL HubSpot]帳戶中的所有連絡人：
>
>**URL**： `/contacts/v1/lists/all/contacts/all`
>
>**方法**： `GET`
>
>![](assets/hubspot-api-config.png)
>
>在[!UICONTROL 組合] > [!UICONTROL 內文] > [!UICONTROL 連絡人]下的模組輸出中，可找到搜尋的相符專案。
>
>在我們的範例中，傳回3個連絡人：
>
>![](assets/hubspot-api-output.png)

+++

## 建立新的應用程式

1. 登入您的[!DNL HubSpot]開發人員帳戶。
1. 選取&#x200B;**[!UICONTROL 建立應用程式]**&#x200B;選項。
1. 輸入應用程式名稱並[!UICONTROL 儲存]對話方塊。
1. 選取您的webhook所需的範圍。

   例如，新增連絡人範圍，以便在建立或刪除新連絡人時觸發模組。

   [!UICONTROL 連絡人範圍]是您接收連絡人、交易和公司活動Webhook所需的全部。

   >[!IMPORTANT]
   >
   >請勿填寫[!UICONTROL 重新導向URL]欄位。
