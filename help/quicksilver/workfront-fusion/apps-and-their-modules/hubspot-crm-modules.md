---
title: hubspot CRM模組
description: 此 [!DNL Adobe Workfront Fusion] HubSpot CRM模組可讓您監視事件、記錄、連絡人、參與、檔案和表單提交，或是建立、擷取、更新和刪除記錄、連絡人、參與、事件或檔案。 [!DNL HubSpot CRM] 帳戶。
author: Becky
feature: Workfront Fusion
exl-id: d58e0c12-a798-495c-8f88-fbf2a532f8a4
source-git-commit: 1c56cf8aa9da7ec2644955d5533c71f60160d580
workflow-type: tm+mt
source-wordcount: '2615'
ht-degree: 0%

---

# [!DNL HubSpot CRM] 模組

此 [!DNL Adobe Workfront Fusion] [!DNL HubSpot CRM] 模組可讓您監視事件、記錄、連絡人、預約、檔案和表單提交，或建立、擷取、更新和刪除您的中的記錄、連絡人、預約、事件或檔案 [!DNL HubSpot CRM] 帳戶。

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
   <p>目前授權需求：否 [!DNL Workfront Fusion] 授權需求。</p>
   <p>或</p>
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] 適用於工作自動化與整合] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 計畫，您的組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述的功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 計畫。</p>
   <p>或</p>
   <p>舊版產品需求：貴組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

有關的資訊 [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 先決條件

使用 [!DNL HubSpot CRM] 模組，您必須擁有 [!DNL HubSpot CRM] 帳戶。

## 連線 [!DNL Adobe Workfront Fusion] 至 [!DNL HubSpot CRM]

如需有關連線您的電腦的指示 [!DNL HubSpot CRM] 帳戶至 [!DNL Workfront Fusion]，請參閱 [建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>設定連線時，選取 **HubSpot CRM** 連線型別。 HubSpot CRM （已淘汰）型別支援現有連線，但我們不建議使用它來建立新連線。

## [!DNL HubSpot CRM] 模組及其欄位

當您設定 [!DNL Hubspot CRM] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 除了這些以外， [!DNL Hubspot CRM] 欄位可能會顯示，端視您應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [在中將資訊從一個模組對應到另一個模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [crm物件](#crm-objects)
* [記錄（交易、聯絡人和公司）](#records-deals-contacts-and-companies)
* [連絡人](#contacts)
* [交易](#deals)
* [公司](#companies)
* [檔案](#files)
* [票證](#tickets)
* [進行API呼叫](#make-an-api-call)

### crm物件

#### [!UICONTROL 搜尋CRM物]

此搜尋模組會依自訂屬性或查詢來搜尋CRM物件。 若要搜尋產品或條列專案，請使用具有所需自訂範圍的特殊連線。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL HubSpot CRM] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
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
     <li> <p><strong>[！UICONTROL Query]</strong> </p> <p>輸入或對映查詢</p> </li> 
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
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Start Offset</td> 
    <td>Enter or map the ID of the first item you want to retrieve details for. This module only returns up to 5000 results at a time. Setting a start offset allows you to retrieve items other than the first 5000. If the start offset is 5000, the module would return items 5000-9999.</td> 
   </tr>
  --> 
 </tbody> 
</table>

### 記錄（交易、聯絡人和公司）

* [[!UICONTROL 建立記錄（舊版）]](#create-a-record-legacy)
* [[!UICONTROL 取得記錄]](#get-a-record)
* [[!UICONTROL 更新記錄]](#update-a-record)
* [[!UICONTROL 刪除記錄]](#delete-a-record)
* [[!UICONTROL 取得記錄屬性]](#get-a-record-property)
* [[!UICONTROL 觀看記錄]](#watch-records)

#### [!UICONTROL 建立記錄（舊版）]

此動作模組會建立聯絡人、公司或交易。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL HubSpot CRM] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL記錄型別]</td> 
   <td> <p>選取您要建立的記錄型別</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL屬性]</td> 
   <td>填寫您要為記錄設定的任何屬性。 可用欄位取決於您要建立的記錄型別。</td> 
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
   <td> <p>如需有關連線您的電腦的指示 [!DNL HubSpot CRM] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
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

#### [!UICONTROL 更新記錄]

此動作模組會更新聯絡人、公司或交易。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL HubSpot CRM] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
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

#### [!UICONTROL 刪除記錄]

此動作模組會刪除連絡人、公司或交易。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL HubSpot CRM] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
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

#### [!UICONTROL 取得記錄屬性]

此動作模組透過其（內部）名稱取得特定記錄屬性的中繼資料。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL HubSpot CRM] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
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

#### [!UICONTROL 觀看記錄]

在過去30天內修改或建立連絡人、公司或交易時，此觸發模組就會開始案例。 輸出限製為10,000筆記錄。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL HubSpot CRM] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
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

### 連絡人

* [[!UICONTROL 建立/更新連絡人（舊版）]](#createupdate-a-contact-legacy)
* [[!UICONTROL 建立/更新連絡人群組]](#createupdate-a-group-of-contacts)
* [[!UICONTROL 新增連絡人至清單]](#add-contacts-to-a-list)
* [[!UICONTROL 從清單中移除連絡人]](#remove-a-contact-from-a-list)
* [[!UICONTROL 合併連絡人]](#merge-contacts)
* [[!UICONTROL 搜尋連絡人]](#search-for-contacts)
* [[!UICONTROL 列出連絡人]](#list-contacts)
* [[!UICONTROL 列出公司的聯絡人]](#list-contacts-of-a-company)

#### [!UICONTROL 建立/更新連絡人（舊版）]

如果入口網站中不存在連絡人，則建立連絡人；如果入口網站中不存在連絡人，則使用最新屬性值更新連絡人。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL HubSpot CRM] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
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
   <td> <p>如需有關連線您的電腦的指示 [!DNL HubSpot CRM] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL要建立/更新的連絡人批次] </td> 
   <td> <p>新增批次連絡人。</p> <p>按一下 <strong>[！UICONTROL新增專案]</strong> 以新增連絡人。 在出現的視窗中，輸入或對應下列資訊：</p> 
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

#### [!UICONTROL 新增連絡人至清單]

此模組會將系統中已建立的連絡人記錄新增至連絡人清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL HubSpot CRM] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
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

#### [!UICONTROL 從清單中移除連絡人]

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
   <td> <p>如需有關連線您的電腦的指示 [!DNL HubSpot CRM] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
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

#### [!UICONTROL 合併連絡人]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL HubSpot CRM] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
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

#### [!UICONTROL 搜尋連絡人]

使用搜尋查詢來擷取連絡人清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL HubSpot CRM] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Query]</td> 
   <td>輸入搜尋查詢。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制] </td> 
   <td>輸入或對應連絡人數上限 [!DNL Workfront Fusion] 應該會在一個案例執行週期中傳回。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出連絡人]

傳回入口網站中建立的所有連絡人。 輸出限製為5000個連絡人。 若要列出上一個或下一個連絡人，您可以使用 [!UICONTROL 進階] 位移清單的引數。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL HubSpot CRM] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td>連絡人數上限 [!DNL Workfront Fusion] 應該會在一個案例執行週期中傳回。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸出屬性]</td> 
   <td>選取您要顯示在模組輸出中的屬性。 </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Contact ID [start offset] </td> 
    <td>Enter or map the ID of the user that you want to start the list. For example, setting the Contact ID as the ID of the 101st contact will allow the module to list contacts 101-5100 rather than 1-5000. </td> 
   </tr>
  --> 
 </tbody> 
</table>

#### [!UICONTROL 列出公司的聯絡人]

擷取公司中的聯絡人清單。 輸出限製為5000個連絡人。 若要列出上一個或下一個連絡人，您可以使用 [!UICONTROL 進階] 位移清單的引數。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL HubSpot CRM] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL ID]</td> 
   <td>輸入要列出其聯絡人的公司ID。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td>連絡人數上限 [!DNL Workfront Fusion] 應該會在一個案例執行週期中傳回。 </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Contact ID [start offset] </td> 
    <td>Enter or map the ID of the user that you want to start the list. For example, setting the Contact ID as the ID of the 101st contact will allow the module to list contacts 101-5100 rather than 1-5000. </td> 
   </tr>
  --> 
 </tbody> 
</table>

#### [!UICONTROL 觀看新增到清單的連絡人]

此觸發模組會在清單中新增連絡人時啟動案例。 此僅供擁有付費行銷帳戶的使用者使用。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL HubSpot CRM] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
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

### 交易

* [[!UICONTROL 列出交易/票證管道]](#list-dealticket-pipelines)
* [[!UICONTROL 取得交易的CRM管道]](#get-a-deals-crm-pipeline)

#### [!UICONTROL 列出交易/票證管道]

傳回給定入口網站的所有交易和票證管道。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL HubSpot CRM] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL物件型別] </td> 
   <td>選取您要列出交易或票證。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得交易的CRM管道]

傳回特定交易管道。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL HubSpot CRM] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
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

### 公司

#### [!UICONTROL 依網域搜尋公司]

根據與網域屬性的完全相符專案擷取公司清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL HubSpot CRM] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL網域] </td> 
   <td>輸入您要搜尋的公司的網域，例如 <code>[!DNL hubspot].com</code>. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td>公司數目上限 [!DNL Workfront Fusion] 應該會在一個案例執行週期中傳回。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL輸出屬性]</td> 
   <td>選取您要顯示在模組輸出中的屬性。 </td> 
  </tr> 
 </tbody> 
</table>

### 檔案

* [[!UICONTROL 建立資料夾]](#create-a-folder)
* [[!UICONTROL 刪除資料夾]](#delete-a-folder)
* [[!UICONTROL 移動檔案]](#move-a-file)

#### [!UICONTROL 建立資料夾]

此模組會建立資料夾。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL HubSpot CRM] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
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

#### [!UICONTROL 刪除資料夾]

將資料夾標籤為已刪除。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL HubSpot CRM] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL ID]</td> 
   <td>輸入您要刪除的資料夾識別碼。</td> 
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
   <td> <p>如需有關連線您的電腦的指示 [!DNL HubSpot CRM] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
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

### 票證

#### [!UICONTROL 刪除票證]

依其ID刪除現有票證。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Connection]</p> </td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL HubSpot CRM] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL ID]</td> 
   <td>輸入您要刪除的票證ID。 </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 進行API呼叫]

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
   <td> <p>如需有關連線您的電腦的指示 [!DNL HubSpot CRM] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL URL]</p> </td> 
   <td> <p>輸入相對於https://api.hubapi.com/的路徑。 例如， /contacts/v1/lists/all/contacts/all</p> <p>如需可用端點的清單，請參閱 <a href="https://legacydocs.hubspot.com/docs/overview">[!DNL HubSpot] API檔案</a>.</p> </td> 
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
   <td> <p>以標準JSON物件的形式新增API呼叫的正文內容。使用條件陳述式(例如 <code>if</code> 在JSON中，將引號放在條件陳述式之外。<img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"></p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**範例：** 下列API呼叫會傳回您網站中 [!DNL HubSpot] 帳戶：
>
>**URL**： `/contacts/v1/lists/all/contacts/all`
>
>**方法**： `GET`
>
>![](assets/hubspot-api-config.png)
>
>您可以在模組的輸出中找到搜尋的相符專案，位於 [!UICONTROL 組合] > [!UICONTROL 內文] > [!UICONTROL 連絡人].
>
>在我們的範例中，傳回3個連絡人：
>
>![](assets/hubspot-api-output.png)

## 建立新的應用程式

1. 登入您的 [!DNL HubSpot] 開發人員帳戶。
1. 選取 **[!UICONTROL 建立應用程式]** 選項。
1. 輸入應用程式名稱並 [!UICONTROL 儲存] 對話方塊。
1. 選取您的webhook所需的範圍。

   例如，新增連絡人範圍，以便在建立或刪除新連絡人時觸發模組。

   此 [!UICONTROL 連絡人範圍] 是您接收連絡人、交易和公司活動webhook所需的一切。

   >[!IMPORTANT]
   >
   >請勿填寫 [!UICONTROL 重新導向URL] 欄位。
