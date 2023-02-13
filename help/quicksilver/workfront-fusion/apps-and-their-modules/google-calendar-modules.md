---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;calendars
keywords: 連接器
navigation-topic: apps-and-their-modules
title: Google日曆模組
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用Google日曆的工作流程，並將其連接至多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: 168e8fce-645d-4108-84b7-46a113c83f41
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '3773'
ht-degree: 0%

---

# [!DNL Google Calendar] 模組

在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!UICONTROL Google日曆]，並將其連接至多個協力廠商應用程式和服務。

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

使用 [!DNL Google Calendar] 模組，您必須 [!DNL Google] 帳戶。

## [!DNL Google Calendar] 模組及其欄位

設定時 [!DNL Google Calendar] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!DNL Google Calendar] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [事件](#events)
* [行事曆](#calendars)
* [存取控制規則](#access-control-rules)
* [迭代器（已廢止）](#iterators-deprecated)
* [其他](#other)

### 事件

* [[!UICONTROL 觀看事件]](#watch-events)
* [[!UICONTROL 搜尋事件]](#search-events)
* [[!UICONTROL 取得事件]](#get-an-event)
* [[!UICONTROL 建立事件]](#create-an-event)
* [[!UICONTROL 更新事件]](#update-an-event)
* [[!UICONTROL 刪除事件]](#delete-an-event)


#### [!UICONTROL 觀看事件]

在您指定的日曆中新增、更新、刪除、啟動或結束新事件時，此觸發器模組會執行案例。 模組會傳回與記錄或記錄相關聯的所有標準欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Calendar] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線以Adobe [!DNL Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL日曆] </td> 
   <td> <p>選取要讓模組使用的日曆。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL監看事件]</td> 
   <td> <p>選擇您要依「建立日期」、「更新日期」、「開始日期」或「結束日期」來監看事件。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL顯示已刪除的事件]</td> 
   <td> <p>啟用此選項可包含已刪除的事件。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL查詢] </td> 
   <td> <p>輸入要搜索的文本。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL限制]</td> 
   <td> <p> 設定 [!DNL Workfront Fusion] 在一個週期中使用（每個方案運行的重複次數）。 如果值設定得太高，則指定的第三方服務（逾時）可能會中斷連線。 [!DNL Workfront Fusion] 對此沒有影響。 建議您設定較低的值，並為最大週期數定義較高的值，或更頻繁地執行藍本。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 搜尋事件]

此動作模組會搜尋所選日曆中的事件。

您可以指定日曆和搜尋參數。

模組會傳回事件ID和任何相關欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td>有關連接 [!DNL Google Calendar] 帳戶至Workfront Fusion，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe Workfront Fusion的連線 — 基本指示</a></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL日曆ID]</td> 
   <td> <p>選擇要搜索的日曆。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL開始日期]</td> 
   <td> <p> 輸入或映射事件開始的日期。 此模組也會擷取在此日期之前開始、仍在輸入開始日期發生的事件。 </p> <p>如需支援的日期和時間格式清單，請參閱 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">中的強制類型 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL結束日期]</td> 
   <td> <p> 輸入或映射事件結束的日期。 </p> <p> 如需支援的日期和時間格式清單，請參閱 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">中的強制類型 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL單一事件]</td> 
   <td> <p> 啟用此選項可將循環事件視為單一例項。 例如，如果您有每週會議且已啟用此選項，則模組會將每週的會議以個別事件的形式傳回。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL查詢]</td> 
   <td> <p>輸入或映射要搜索的搜索詞。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL順序依]</td> 
   <td> <p>選取結果中傳回事件的順序。</p> 
    <ul> 
     <li><strong>[!UICONTROL開始時間]</strong>:依開始日期和時間排序（遞增）。 這僅在查詢單一事件時可用。</li> 
     <li><strong>[!UICONTROL更新時間]</strong>:按上次修改時間排序（升序）。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL限制]</td> 
   <td> <p>設定事件數上限 [!DNL Workfront Fusion] 在一個執行週期中傳回。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得事件]

此動作模組會傳回指定日曆中單一事件的中繼資料。

您可指定日曆和事件。

模組會傳回事件ID和所有相關欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Calendar] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線以Adobe [!DNL Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL日曆ID]</td> 
   <td> <p>輸入或對應包含您要取得之事件的日曆ID。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL事件ID] </td> 
   <td> <p>輸入現有事件ID [!DNL Google Calendar] 事件。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立事件]

此動作模組會建立事件。

您可以指定事件的日曆和參數。

模組會傳回事件ID和任何相關欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td>有關連接 [!DNL Google Calendar] 帳戶至Workfront Fusion，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe Workfront Fusion的連線 — 基本指示</a></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL建立事件]</td> 
   <td> <p>選取您要如何建立事件。</p> 
    <ul> 
     <li><b>[!UICONTROL詳細資訊]</b><p>此選項可讓您更詳細地說明事件。<br></p></li> 
     <li><b>[!UICONTROL快速]</b><p>您只需選取日曆並輸入事件名稱即可。 您可以在名稱中加入時間和位置詳細資訊，以及 [!DNL Google Calendar] 會排程該位置和時間的活動。</p></li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL日曆ID]</td> 
   <td> <p>選取您要顯示事件的日曆。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL顏色]</td> 
   <td>選取事件在日曆上顯示的顏色。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL事件名稱]</td> 
   <td> <p> 輸入或對應事件的名稱。 </p> <p>注意：如果您已在[!UICONTROL建立事件]欄位中選取[!UICONTROL快速添加]，則可以包含事件的日期和時間，以及 [!DNL Workfront Fusion] 會建立該日期和時間的事件。 範例: <code>Appointment at Capitol Hill on June 3rd 10am-10:25am</code>. 如果您選取[!UICONTROL快速添加]，但事件名稱中未包含日期和時間，則會從當前時間建立事件，並持續一小時。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL全天事件]</td> 
   <td>如果事件是全天事件（不需要開始和結束時間），請啟用此選項。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL開始日期]</td> 
   <td> <p>如果這是全天事件，請輸入事件的開始日期。 </p> <p>如需支援的日期格式清單，請參閱 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">中的強制類型 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL結束日期]</td> 
   <td> <p> 如果這是全天事件，請輸入事件的結束日期。 </p> <p>如需支援的日期格式清單，請參閱 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">中的強制類型 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL描述]</td> 
   <td>輸入或對應事件的說明。 此欄位支援HTML。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL位置]</td> 
   <td>以文本形式輸入事件的位置。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL使用此事件的預設提醒設定]</td> 
   <td>啟用此選項以使用預設提醒設定。 如果您在[!UICONTROL提醒]欄位中設定了自定義提醒，則此值將設定為No。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL提醒] </td> 
   <td> <p>為事件新增提醒。 對於每個提醒，請選取您要使用的提醒方法，並定義您要提醒的事件之前的時間（以分鐘為單位）。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL與會者]</td> 
   <td>將出席者添加到活動中。 對於每個與會者，輸入或映射其姓名和電子郵件地址。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL將我顯示為]</td> 
   <td>選擇是否希望查看日曆的人員在此事件期間看到您忙或可用。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL可見性] </td> 
   <td> <p>選取此事件的可見性。 </p> 
    <ul> 
     <li> <p><b>[!UICONTROL預設值]</b></p> <p>事件具有您已在日曆設定中設定的可見性。</p> </li> 
     <li> <p><b>[!UICONTROL公用]</b></p> <p>與共用日曆的任何人都能看到此事件。</p> </li> 
     <li> <p><b>[!UICONTROL專用]</b></p> <p>只有與會者才能看到此活動。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL傳送關於事件建立的通知]</td> 
   <td> <p>選擇是否將建立新事件的通知發送給所有來賓，非[!DNL Google Calendar] 客人，或者沒人。</p> <p>提示：建議僅將[!UICONTROL無]選項用於移轉使用案例。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL來賓可以修改事件]</td> 
   <td> <p>如果希望來賓能夠修改此事件，請啟用此選項。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL週期]</td> 
   <td>新增您要套用至此事件的任何週期規則。 每個規則都需要[!UICONTROL RRULE]、[!UICONTROL EXRULE]、[!UICONTROL RDATE]和[!UICONTROL EXDATE]行的清單，以表示循環事件。 請注意，此欄位中不允許[!UICONTROL DTSTART]和[!UICONTROL DTEND]行；「開始」和「結束」欄位中會指定事件開始和結束時間。 對於單一事件或循環事件的例項，會忽略此欄位。 如需詳細資訊，請參閱 <a href="https://tools.ietf.org/html/rfc5545#section-3.8.5">RFC5545</a>.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新事件]

此動作模組會變更現有事件。

您可指定日曆和事件ID。

模組會傳回事件ID和任何相關欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Calendar] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線以Adobe [!DNL Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL日曆] </td> 
   <td> <p>選擇要使用的日曆。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL事件ID] </td> 
   <td> <p>輸入先前建立之 [!DNL Google Calendar] 要更新的事件。</p> </td> 
  </tr> 
 </tbody> 
</table>

您可以在所需欄位中輸入新值，以更新事件資訊。 如需個別欄位的詳細資訊，請參閱 [[!UICONTROL 建立事件]](#create-an-event).

#### [!UICONTROL 刪除事件]

此動作模組會刪除事件。

您可指定日曆和事件ID。

模組會傳回事件ID和任何相關欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Calendar] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線以Adobe [!DNL Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL日曆ID]</td> 
   <td> <p>選取包含您要刪除之事件的日曆。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL事件ID]</td> 
   <td> <p> 輸入先前建立之事件ID [!DNL Google Calendar] 要刪除的事件。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL傳送關於事件刪除的通知]</td> 
   <td>選擇是否要向所有未使用的來賓發送有關事件刪除的通知 [!DNL Google Calendar]，或者沒有人。</td> 
  </tr> 
 </tbody> 
</table>

### 行事曆

* [[!UICONTROL 清單日曆]](#list-calendars)
* [[!UICONTROL 取得日曆]](#get-a-calendar)
* [[!UICONTROL 建立日曆]](#create-a-calendar)
* [[!UICONTROL 更新日曆]](#update-a-calendar)
* [[!UICONTROL 刪除日曆]](#delete-a-calendar)
* [[!UICONTROL 清除日曆]](#clear-a-calendar)

#### [!UICONTROL 清單日曆]

此動作模組會傳回使用者日曆清單上的日曆。

模組會傳回日曆和任何相關欄位的ID，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Calendar] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線以Adobe [!DNL Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL最低訪問角色]</td> 
   <td> <p>為用戶選擇最小訪問角色。 模組會根據此最小存取角色傳回日曆。</p> 
    <ul> 
     <li><strong>[!UICONTROL忙Reader]</strong>:用戶可以讀取空閒/忙碌資訊。 </li> 
     <li><strong>[!UICONTROL所有者]</strong>:使用者可讀取和修改事件，並可存取控制清單。 </li> 
     <li><strong>[!UICONTROLReader]</strong>:使用者可讀取非私人事件。 </li> 
     <li><strong>[!UICONTROL寫入器]</strong>:使用者可以讀取和修改事件。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL顯示隱藏日曆]</td> 
   <td>啟用此選項，可在模組返回的清單中包含隱藏的日曆。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td>設定日曆的最大數量 [!DNL Workfront Fusion] 在一個執行週期中傳回。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得日曆]

此動作模組會擷取日曆。

指定要檢索的日曆的ID。

模組會傳回記錄和任何相關欄位的ID，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Calendar] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線以Adobe [!DNL Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL日曆ID]</td> 
   <td> <p>選擇要檢索的日曆。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立日曆]

此動作模組會建立新日曆。

可指定日曆的名稱。

模組會傳回日曆和任何相關欄位的ID，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Calendar] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線以Adobe [!DNL Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL日曆名稱]</td> 
   <td> <p> 輸入新日曆的名稱。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新日曆]

此動作模組會更新日曆。

您需指定要更新之日曆的ID。

模組會傳回日曆和任何相關欄位的ID，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Calendar] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線以Adobe [!DNL Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL日曆ID]</td> 
   <td> <p>選擇要更新的日曆。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL日曆名稱]</td> 
   <td> <p> 輸入日曆的新名稱。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除日曆]

此動作模組會刪除日曆。

您可指定要刪除之日曆的ID。

模組會傳回日曆和任何相關欄位的ID，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Calendar] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線以Adobe [!DNL Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL日曆ID]</td> 
   <td> <p>輸入或映射要刪除的日曆的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 清除日曆]

此動作模組會從帳戶的主要日曆中移除所有事件。

您可以指定連線至帳戶的連線，帳戶包含您要清除的日曆。

模組會傳回日曆和任何相關欄位的ID，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Calendar] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線以Adobe [!DNL Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
 </tbody> 
</table>

### 存取控制規則

* [[!UICONTROL 列出訪問控制規則]](#list-access-control-rules)
* [[!UICONTROL 取得存取控制規則]](#get-an-access-control-rule)
* [[!UICONTROL 建立存取控制規則]](#create-an-access-control-rule)
* [[!UICONTROL 更新訪問控制規則]](#update-an-access-control-rule)
* [[!UICONTROL 刪除訪問控制規則]](#delete-an-access-control-rule)

#### [!UICONTROL 列出訪問控制規則]

此動作模組會傳回日曆上存取控制清單中的規則。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Calendar] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線以Adobe [!DNL Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL日曆ID]</td> 
   <td> <p>選擇包含要檢索的訪問控制規則的日曆。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td>設定結果的最大數量 [!DNL Workfront Fusion] 在一個執行週期中傳回。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得存取控制規則]

此動作模組會傳回存取控制規則的中繼資料。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Calendar] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線以Adobe [!DNL Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL日曆ID]</td> 
   <td> <p>選擇包含要檢索的訪問控制規則的日曆。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL訪問控制規則ID]</td> 
   <td>選擇要檢索的訪問控制規則。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立存取控制規則]

此動作模組會建立新的存取控制規則。

可指定日曆的名稱。

模組會傳回存取控制規則的ID和任何相關欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Calendar] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線以Adobe [!DNL Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL日曆ID]</td> 
   <td> <p>選擇要建立訪問控制規則的日曆。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL角色]</td> 
   <td> <p>選擇要分配給訪問規則的角色。 </p> 
    <ul> 
     <li><strong>[!UICONTROL忙Reader]</strong>:用戶可以讀取空閒/忙碌資訊。 </li> 
     <li><strong>[!UICONTROL所有者]</strong>:使用者可讀取和修改事件，並可存取控制清單。 </li> 
     <li><strong>[!UICONTROLReader]</strong>:使用者可讀取非私人事件。 </li> 
     <li><strong>[!UICONTROL寫入器]</strong>:使用者可以讀取和修改事件。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL類型]</td> 
   <td> <p>選擇範圍類型。 </p> 
    <ul> 
     <li><strong>[!UICONTROL預設值]</strong>:公共範圍。 這是預設值。 </li> 
     <li><strong>[!UICONTROL用戶]</strong>:將範圍限制為單一使用者。 </li> 
     <li><strong>[!UICONTROL組]</strong>:將範圍限制為組。 </li> 
     <li><strong>[!UICONTROL域]</strong>:將範圍限制為網域。 </li> 
    </ul> <p>注意：授予[!UICONTROL預設]或公用範圍的權限適用於已驗證或未驗證的任何用戶。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL值]</td> 
   <td>根據範圍類型，輸入用戶或組的電子郵件地址或域的名稱。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL發送通知]</td> 
   <td> <p>啟用此選項可傳送存取變更的相關通知。 </p> <p>注意：訪問刪除時沒有通知。 </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新訪問控制規則]

此動作模組會更新存取控制規則。

可指定日曆的名稱。

模組會傳回存取控制規則的ID和任何相關欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Calendar] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線以Adobe [!DNL Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL日曆ID]</td> 
   <td> <p>選擇包含要更新的訪問控制規則的日曆。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL訪問控制規則ID]</td> 
   <td>選擇要更新的訪問控制規則。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL角色]</td> 
   <td> <p>選擇要分配給訪問規則的角色。 </p> 
    <ul> 
     <li><strong>[!UICONTROL無]</strong>:此角色不提供訪問權。</li> 
     <li><strong>[!UICONTROL忙Reader]</strong>:用戶可以讀取空閒/忙碌資訊。 </li> 
     <li><strong>[!UICONTROL所有者]</strong>:使用者可讀取和修改事件，並可存取控制清單。 </li> 
     <li><strong>[!UICONTROLReader]</strong>:使用者可讀取非私人事件。 </li> 
     <li><strong>[!UICONTROL寫入器]</strong>:使用者可以讀取和修改事件。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL發送通知]</td> 
   <td> <p>啟用此選項可傳送存取變更的相關通知。 </p> <p>注意：訪問刪除時沒有通知。 </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除訪問控制規則]

此動作模組會刪除存取控制規則。

可指定日曆的名稱。

模組會傳回存取控制規則的ID和任何相關欄位，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Google Calendar] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線以Adobe [!DNL Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL日曆ID]</td> 
   <td> <p>選擇或映射包含要刪除的訪問控制規則的日曆的ID。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL訪問控制規則ID]</td> 
   <td>選擇或映射要刪除的訪問控制規則的ID。</td> 
  </tr> 
 </tbody> 
</table>

### 迭代器（已廢止）

此 [!UICONTROL 迭代附件] 和 [!UICONTROL 互訪參與者] 已棄用模組。 要查詢附件或與會者，請使用 [!UICONTROL 流量控制] > [!UICONTROL 迭代器] 模組。 如需詳細資訊，請參閱 [中的迭代器模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md)

### 其他

* [[!UICONTROL 進行API呼叫]](#make-an-api-call)
* [[!UICONTROL 獲取忙/閒資訊]](#get-freebusy-information)

#### [!UICONTROL 進行API呼叫]

此模組可讓您執行自訂API呼叫。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td> <p>有關連接 [!DNL Google Calendar] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線以Adobe [!DNL Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td>輸入相對於的路徑 <code>https://www.googleapis.com/calendar</code>. 範例: <code>/v3/users/me/calendarList</code></td> 
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
   <td> <p>以標準JSON物件的形式新增API呼叫的內文內容。</p> <p>備註:   <p>使用條件陳述式時，例如 <code>if</code> 在JSON中，將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 獲取忙/閒資訊]

此操作模組返回一組日曆的忙閒資訊。

模組會傳回日曆和任何相關欄位的ID，以及連線存取的任何自訂欄位和值。 您可以在案例的後續模組中對應此資訊。

設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL連接] </td> 
   <td>有關連接 [!DNL Google Calendar] 帳戶至Workfront Fusion，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe Workfront Fusion的連線 — 基本指示</a></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL最短時間]</td> 
   <td> <p> 輸入要檢索資訊的間隔的開始。</p> <p> 如需支援的日期和時間格式清單，請參閱 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">中的強制類型 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL最大時間]</td> 
   <td> <p> 輸入要檢索資訊的間隔的結尾。 </p> <p>如需支援的日期和時間格式清單，請參閱 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">中的強制類型 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL日曆]</td> 
   <td> <p>對於要從中檢索資訊的每個日曆，按一下 <strong>新增</strong> 並輸入或映射日曆ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 在事件之前觸發案例

在標準的協助下，您可以在事件之前的指定時間觸發案例 [!DNL Google Calendar] 電子郵件提醒和 [!UICONTROL Webhook] >[!UICONTROL 自訂郵件連結] 模組。

1. 使用 [!UICONTROL Google日曆] >[!UICONTROL 更新事件] 模組，將電子郵件提醒新增至您的事件：

   ![](assets/trigger-scen-before-event-350x209.png)

1. 建立新藍本，以 [!UICONTROL Webhook] >[!UICONTROL 自訂郵件連結] 模組。

   1. 複製郵件連結的電子郵件地址。
   1. 儲存案例並加以執行。

1. 在 [!DNL Gmail]，重新導向 [!DNL Google Calendar] 電子郵件提醒至mailhook的電子郵件地址：

   1. 開啟 **[!UICONTROL [!DNL Gmail]設定]**.
   1. 開啟 **[!UICONTROL 轉發和POP/IMAP]** 標籤。
   1. 按一下 **[!UICONTROL 添加轉發地址].**
   1. 貼上複製的Mailhook的電子郵件地址，按一&#x200B;下&#x200B;**[!UICONTROL 下一個]**，按下確認 **[!UICONTROL 繼續]** 在彈出式視窗中，按一下 **[!UICONTROL 確定]**.

   1. 在 [!DNL Workfront Fusion]，請切換至新案例，此情境應會透過收到確認電子郵件來完成執行。
   1. 按一下模組上方的氣泡以檢查模組的輸出。
   1. 展開 `Text` 項目並複製確認代碼：

      ![](assets/confirmation-code-350x252.png)

   1. 在Gmail中，將確認程式碼貼到編輯方塊中，然後按一&#x200B;下&#x200B;**[!UICONTROL 驗證]**:

      ![](assets/paste-code-350x46.png)

   1. 開啟 **[!UICONTROL 篩選器和已阻止的地址]** 標籤。
   1. 按一下 **[!UICONTROL 建立新篩選器]**.
   1. 設定來自所有電子郵件的篩選器 `     calendar-notification@google.com` 按一&#x200B;下&#x200B;**[!UICONTROL 建立篩選器]**:
   1. 選擇 **[!UICONTROL 轉送至]** 並從清單中選擇mailhook的電子郵件地址。
   1. 按一下 **[!UICONTROL 建立篩選]** 來建立篩選器。

1. （可選） [!DNL Workfront Fusion]，新增 [!UICONTROL 文字剖析器] > [!UICONTROL 匹配模式] 模組之後 [!UICONTROL Webhook] >[!UICONTROL 自訂郵件連結] 模組，剖析電子郵件的HTML程式碼以取得您需要的任何資訊。

   例如，您可以依下列方式設定模組，以取得事件的ID:

   *圖樣*: `<meta itemprop="eventId/googleCalendar" content="(?<evenitID>.*?)"/>`

   *文字*:此 `HTML content` 從 [!UICONTROL Webhook] >[!UICONTROL 自訂郵件連結] 模組。
