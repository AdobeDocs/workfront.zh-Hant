---
title: HubSpot CRM模組
description: 此 [!DNL Adobe Workfront Fusion] HubSpot CRM模組使您能夠監視事件、記錄、聯繫人、參與、檔案和表單提交，或者建立、檢索、更新和刪除記錄、聯繫人、參與、事件或檔案 [!DNL HubSpot CRM] 帳戶。
author: Becky
feature: Workfront Fusion
exl-id: d58e0c12-a798-495c-8f88-fbf2a532f8a4
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2485'
ht-degree: 0%

---

# [!DNL HubSpot CRM] 模組

此 [!DNL Adobe Workfront Fusion] [!DNL HubSpot CRM] 模組可讓您監控事件、記錄、聯絡人、參與、檔案和表單提交，或建立、擷取、更新和刪除您中的記錄、連絡人、參與、事件或檔案 [!DNL HubSpot CRM] 帳戶。

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

使用 [!DNL HubSpot CRM] 模組，您必須 [!DNL HubSpot CRM] 帳戶。

## Connect [!DNL Adobe Workfront Fusion] to [!DNL HubSpot CRM]

有關連接 [!DNL HubSpot CRM] 帳戶 [!DNL Workfront Fusion]，請參閱 [建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL HubSpot CRM] 模組及其欄位

設定時 [!DNL Hubspot CRM] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!DNL Hubspot CRM] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [CRM對象](#crm-objects)
* [記錄（交易、聯繫人和公司）](#records-deals-contacts-and-companies)
* [連絡人](#contacts)
* [交易](#deals)
* [公司](#companies)
* [檔案](#files)
* [票證](#tickets)
* [進行API呼叫](#make-an-api-call)

### CRM對象

#### [!UICONTROL 搜索CRM對象]

此搜索模組按自定義屬性或按查詢搜索CRM對象。 要搜索產品或行項目，請使用具有所需自定義範圍的特殊連接。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL HubSpot CRM] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td>輸入或映射模組將在一個執行週期中返回的最大項目數。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！要搜索的對象類型]</td> 
   <td>選擇要搜索的Hubspot CRM對象類型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸出屬性]</td> 
   <td>選取您要在模組輸出中顯示的屬性。 可用欄位取決於您選取的物件。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL篩選器依據] </td> 
   <td> <p>選取要如何篩選搜尋</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL查詢]</strong> </p> <p>輸入或映射查詢</p> </li> 
     <li> <p><strong>[!UICONTROL屬性]</strong> </p> <p>輸入搜索的組或篩選器。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL排序依據]</td> 
   <td> <p>如果要排序結果，請按一下。 如果您選擇排序結果，則會顯示下列欄位。 </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL屬性名稱]</strong> </p> <p>選擇要按哪個屬性對結果排序</p> </li> 
     <li> <p><strong>[!UICONTROL方向]</strong> </p> <p>選擇您要依遞增或遞減方向排序結果。</p> </li> 
    </ul> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Start Offset</td> 
    <td>Enter or map the ID of the first item you want to retrieve details for. This module only returns up to 5000 results at a time. Setting a start offset allows you to retrieve items other than the first 5000. If the start offset is 5000, the module would return items 5000-9999.</td> 
   </tr>
  --> 
 </tbody> 
</table>

### 記錄（交易、聯繫人和公司）

* [[!UICONTROL 建立記錄（舊版）]](#create-a-record-legacy)
* [[!UICONTROL 取得記錄]](#get-a-record)
* [[!UICONTROL 更新記錄]](#update-a-record)
* [[!UICONTROL 刪除記錄]](#delete-a-record)
* [[!UICONTROL 取得記錄屬性]](#get-a-record-property)
* [[!UICONTROL 監看記錄]](#watch-records)

#### [!UICONTROL 建立記錄（舊版）]

此動作模組會建立連絡人、公司或交易。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL HubSpot CRM] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL記錄類型]</td> 
   <td> <p>選擇要建立的記錄類型</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL屬性]</td> 
   <td>填入要為記錄設定的任何屬性。 可用欄位取決於您要建立的記錄類型。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得記錄]

此動作模組會取得聯絡人、公司或交易的詳細資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL HubSpot CRM] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL記錄類型]</td> 
   <td> <p>選擇記錄類型。</p> 
    <ul> 
     <li>[!UICONTROL聯繫人]</li> 
     <li>[!UICONTROL公司] </li> 
     <li>[!UICONTROL交易]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL搜索類型]</td> 
   <td>如果您要取得連絡人，請選取您要依ID或電子郵件地址識別。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>輸入要檢索的聯繫人、公司或交易的ID。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL電子郵件]</td> 
   <td>輸入要檢索其詳細資訊的聯繫人的電子郵件地址。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新記錄]

此動作模組會更新連絡人、公司或交易。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL HubSpot CRM] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL記錄類型]</td> 
   <td>選擇要更新的記錄類型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL搜索類型]</td> 
   <td> <p>如果您要聯繫，請選擇要如何識別記錄：</p> 
    <ul> 
     <li> <p>[!UICONTROL ID]</p> </li> 
     <li> <p>[!UICONTROL電子郵件]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>輸入要更新的聯繫人、公司或交易的ID。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL電子郵件]</td> 
   <td>輸入要更新其詳細資訊的聯繫人的電子郵件地址。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL屬性]</td> 
   <td>填入要為記錄設定的任何屬性。 可用欄位取決於您要建立的記錄類型。</td> 
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
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL HubSpot CRM] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL記錄類型]</td> 
   <td>選擇要刪除的記錄類型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>輸入要刪除的聯繫人、公司或交易的ID。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得記錄屬性]

此動作模組依其（內部）名稱取得特定記錄屬性的中繼資料。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL HubSpot CRM] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL記錄類型]</td> 
   <td>選擇具有要檢索元資料的屬性的記錄類型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL屬性名稱]</td> 
   <td>選取您要擷取中繼資料的屬性。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL選項ID]</td> 
   <td> <p> 有些屬性有一組可用選項，使用者可以選取這些選項作為屬性值。 輸入代表您要擷取之屬性值之選項的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 監看記錄]

此觸發模組會在最近30天內修改或建立連絡人、公司或交易時啟動案例。 輸出限制為10,000筆記錄。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL HubSpot CRM] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL記錄類型]</td> 
   <td>選擇具有要監視的屬性的記錄類型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL搜索]</td> 
   <td>選擇要監視最近修改的記錄還是最近建立的記錄。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸出屬性]</td> 
   <td>選取要包含在模組輸出中的屬性。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 連絡人

* [[!UICONTROL 建立/更新連絡人（舊版）]](#createupdate-a-contact-legacy)
* [[!UICONTROL 建立/更新一組聯繫人]](#createupdate-a-group-of-contacts)
* [[!UICONTROL 將聯繫人添加到清單]](#add-contacts-to-a-list)
* [[!UICONTROL 從清單中刪除聯繫人]](#remove-a-contact-from-a-list)
* [[!UICONTROL 合併聯繫人]](#merge-contacts)
* [[!UICONTROL 搜索聯繫人]](#search-for-contacts)
* [[!UICONTROL 列出聯繫人]](#list-contacts)
* [[!UICONTROL 列出公司的聯繫人]](#list-contacts-of-a-company)

#### [!UICONTROL 建立/更新連絡人（舊版）]

如果門戶中尚未存在聯繫人，則建立該聯繫人；如果門戶中已存在該聯繫人，則用最新的屬性值更新該聯繫人。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL HubSpot CRM] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL屬性]</td> 
   <td>填寫您要為聯繫人設定或更新的任何屬性。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立/更新一組聯繫人]

建立一組聯繫人或更新它們（如果它們已存在）。 當批大小限制為100個或更少聯繫人時，效能最好。 透過此端點所做的變更會以非同步方式處理，因此可能需要幾分鐘的時間才會將變更套用至聯絡記錄。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL HubSpot CRM] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL要建立/更新的聯繫人批次] </td> 
   <td> <p>添加聯繫人批。</p> <p>按一下 <strong>[!UICONTROL添加項]</strong> 添加新聯繫人。 在顯示的視窗中，輸入或映射下列資訊：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL搜索類型]</strong> </p> <p>選擇要如何識別聯繫人：</p> 
      <ul> 
       <li> <p>[!UICONTROL ID]</p> <p>輸入要建立或更新的聯繫人的ID。 </p> </li> 
       <li> <p>[!UICONTROL電子郵件]</p> <p>輸入要建立或更新的聯繫人的電子郵件地址。 </p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL屬性]</strong> </p> <p>填寫您要設定或更新聯繫人的任何屬性。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 將聯繫人添加到清單]

此模組將系統中已建立的聯繫人記錄添加到聯繫人清單中。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL HubSpot CRM] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL清單ID] </td> 
   <td>選擇要添加聯繫人的清單的ID。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID/電子郵件] </td> 
   <td> <p>選擇要如何標識要添加到清單中的聯繫人：</p> 
    <ul> 
     <li> <p>[!UICONTROL ID]</p> <p>添加要添加到清單的聯繫人的ID。</p> </li> 
     <li> <p>[!UICONTROL電子郵件]</p> <p>添加要添加到清單的聯繫人的電子郵件地址。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 從清單中刪除聯繫人]

從聯繫人清單中刪除聯繫人。

>[!NOTE]
>
>不能手動從動態清單中刪除聯繫人。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL HubSpot CRM] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL清單ID] </td> 
   <td>選擇要從中刪除聯繫人的清單的ID。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL聯繫人ID] </td> 
   <td>輸入要從清單中刪除的聯繫人的ID。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 合併聯繫人]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL HubSpot CRM] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID 1] </td> 
   <td>輸入要合併的其中一個聯繫人的ID。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID 2] </td> 
   <td>輸入要合併的其他聯繫人的ID。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 搜索聯繫人]

使用搜索查詢檢索聯繫人清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL HubSpot CRM] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL查詢]</td> 
   <td>輸入搜索查詢。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制] </td> 
   <td>輸入或映射最大聯繫人數 [!DNL Workfront Fusion] 應會在一個案例執行週期期間傳回。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出聯繫人]

返回已在門戶中建立的所有聯繫人。 輸出限制為5000個聯繫人。 要列出以前或下一個聯繫人，可以使用 [!UICONTROL 進階] 參數來偏移清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL HubSpot CRM] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td>聯繫人的最大數 [!DNL Workfront Fusion] 應會在一個案例執行週期期間傳回。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸出屬性]</td> 
   <td>選取您要在模組輸出中顯示的屬性。 </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Contact ID [start offset] </td> 
    <td>Enter or map the ID of the user that you want to start the list. For example, setting the Contact ID as the ID of the 101st contact will allow the module to list contacts 101-5100 rather than 1-5000. </td> 
   </tr>
  --> 
 </tbody> 
</table>

#### [!UICONTROL 列出公司的聯繫人]

檢索公司中的聯繫人清單。 輸出限制為5000個聯繫人。 要列出以前或下一個聯繫人，可以使用 [!UICONTROL 進階] 參數來偏移清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL HubSpot CRM] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>輸入要列出其聯繫人的公司ID。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td>聯繫人的最大數 [!DNL Workfront Fusion] 應會在一個案例執行週期期間傳回。 </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Contact ID [start offset] </td> 
    <td>Enter or map the ID of the user that you want to start the list. For example, setting the Contact ID as the ID of the 101st contact will allow the module to list contacts 101-5100 rather than 1-5000. </td> 
   </tr>
  --> 
 </tbody> 
</table>

#### [!UICONTROL 將監視聯繫人添加到清單]

此觸發模組會在新連絡人新增至清單時啟動案例。 這僅適用於具有付費行銷帳戶的使用者。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL HubSpot CRM] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL清單ID]</td> 
   <td>輸入或映射包含您要監視的聯繫人的清單的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸出屬性]</td> 
   <td>選取要包含在模組輸出中的屬性。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>輸入或映射您希望模組在每個方案執行週期中返回的最大記錄數。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 交易

* [[!UICONTROL 列出交易/票證管道]](#list-dealticket-pipelines)
* [[!UICONTROL 取得交易的CRM管道]](#get-a-deals-crm-pipeline)

#### [!UICONTROL 列出交易/票證管道]

返回給定門戶的所有交易和票證管道。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL HubSpot CRM] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL對象類型] </td> 
   <td>選擇要列出交易還是票證。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得交易的CRM管道]

返回特定交易管道……

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL HubSpot CRM] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL管道ID] </td> 
   <td>輸入或映射要檢索詳細資訊的管道的ID。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL階段ID] </td> 
   <td>輸入或映射要檢索詳細資訊的階段的ID。 </td> 
  </tr> 
 </tbody> 
</table>

### 公司

#### [!UICONTROL 依網域搜尋公司]

根據與網域屬性完全相符的項目，擷取公司清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL HubSpot CRM] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL域] </td> 
   <td>輸入要搜索的公司的域，例如 <code>[!DNL hubspot].com</code>. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td>公司數上限 [!DNL Workfront Fusion] 應會在一個案例執行週期期間傳回。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL輸出屬性]</td> 
   <td>選取您要在模組輸出中顯示的屬性。 </td> 
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
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL HubSpot CRM] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資料夾名稱] </td> 
   <td>輸入或映射新資料夾的名稱。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL父資料夾ID] </td> 
   <td>為要建立的資料夾選擇父資料夾的ID。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除資料夾]

將資料夾標示為已刪除。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL HubSpot CRM] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>輸入要刪除的資料夾ID。</td> 
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
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL HubSpot CRM] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL檔案ID] </td> 
   <td>輸入或映射要移動的檔案的ID。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL資料夾ID] </td> 
   <td>選取要移動檔案的資料夾ID。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL名稱]</td> 
   <td>輸入已移動檔案的名稱。</td> 
  </tr> 
 </tbody> 
</table>

### 票證

#### [!UICONTROL 刪除票證]

按票證ID刪除現有票證。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>有關連接 [!DNL HubSpot CRM] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>輸入要刪除的票證ID。 </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 進行API呼叫]

可讓您執行自訂API呼叫。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL HubSpot CRM] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>輸入相對於https://api.hubapi.com/的路徑。 例如， /contacts/v1/lists/all/contacts/all</p> <p>如需可用端點的清單，請參閱 <a href="https://legacydocs.hubspot.com/docs/overview">[!DNL HubSpot] API檔案</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL方法]</p> </td> 
   <td> <p>選取您要使用的HTTP方法：</p> <p>[!UICONTROLGET]</p> <p>來檢索條目的資訊。</p> <p>[!UICONTROLPOST]</p> <p>以建立新條目。</p> <p>[!UICONTROLPUT]</p> <p>更新/替換現有條目。</p> <p>[!UICONTROLPATCH]</p> <p>進行部分條目更新。</p> <p>[!UICONTROLDELETE]</p> <p>刪除條目。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL標題]</td> 
   <td> <p> 輸入所需的請求標題。 您不必添加授權標頭；我們已經為你做了。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL查詢字串]</td> 
   <td> <p> 輸入請求查詢字串。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL正文]</td> 
   <td> <p>以標準JSON物件的形式，新增API呼叫的內文內容。使用條件陳述式時，例如 <code>if</code> 在JSON中，將引號放在條件陳述式之外。<img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"></p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**範例：** 下列API呼叫會傳回您 [!DNL HubSpot] 帳戶：
>
>**URL**: `/contacts/v1/lists/all/contacts/all`
>
>**方法**: `GET`
>
>![](assets/hubspot-api-config.png)
>
>如需搜尋的相符項目，請在模組的「輸出」下方找到 [!UICONTROL 捆綁] > [!UICONTROL 主體] > [!UICONTROL 聯繫人].
>
>在我們的示例中，返回了3個聯繫人：
>
>![](assets/hubspot-api-output.png)

## 建立新應用程式

1. 登入 [!DNL HubSpot] 開發人員帳戶。
1. 選取 **[!UICONTROL 建立應用程式]** 選項。
1. 輸入應用程式名稱，然後 [!UICONTROL 儲存] 對話框。
1. 選擇網頁鈎點所需的範圍。

   例如，在建立或刪除新聯繫人時添加觸發模組的聯繫人範圍。

   此 [!UICONTROL 聯繫人範圍] 是您接收聯絡人、交易和公司事件網頁鈎點所需的全部。

   >[!IMPORTANT]
   >
   >請勿填入 [!UICONTROL 重新導向URL] 欄位。
