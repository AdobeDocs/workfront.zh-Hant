---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;calendars
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Google行事曆模組
description: Adobe Workfront Fusion檔案已移至新位置。 本文已棄用，但包含新文章的連結，內容涵蓋此功能。
author: Becky
feature: Workfront Fusion
exl-id: 168e8fce-645d-4108-84b7-46a113c83f41
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '3889'
ht-degree: 0%

---

# [!DNL Google Calendar]模組

>[!IMPORTANT]
>
>Adobe Workfront Fusion檔案已移至新位置。
>
>本文資訊可在以下文章中找到：
>
>* [Google行事曆模組](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules.html)
>
>請更新任何書籤。
>
>本文已不再更新，將於不久將來移除。

在[!DNL Adobe Workfront Fusion]案例中，您可以自動執行使用[!UICONTROL Google Calendar]的工作流程，並將其連線至多個協力廠商應用程式和服務。

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

若要使用[!DNL Google Calendar]模組，您必須有[!DNL Google]帳戶。

## Google日曆API資訊

Google Calendar聯結器使用下列專案：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">基礎URL</td> 
   <td> https://www.googleapis.com/calendar/v3</td> 
  </tr> 
  <tr> 
   <td role="rowheader">API版本</td> 
   <td> v3 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API標籤</td> 
   <td>v5.4.5</td> 
  </tr>
 </tbody> 
 </table>

## [!DNL Google Calendar]模組及其欄位

當您設定[!DNL Google Calendar]模組時，[!DNL Workfront Fusion]會顯示下列欄位。 除了這些欄位以外，可能還會顯示其他[!DNL Google Calendar]欄位，視您在應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中將資訊從一個模組對應到另一個模組。

![](assets/map-toggle-350x74.png)

* [活動](#events)
* [行事曆](#calendars)
* [存取控制規則](#access-control-rules)
* [迭代器（已棄用）](#iterators-deprecated)
* [其他](#other)

### 活動

* [[!UICONTROL 觀看活動]](#watch-events)
* [[!UICONTROL 搜尋事件]](#search-events)
* [[!UICONTROL 取得事件]](#get-an-event)
* [[!UICONTROL 建立事件]](#create-an-event)
* [[!UICONTROL 更新事件]](#update-an-event)
* [[!UICONTROL 刪除事件]](#delete-an-event)


#### [!UICONTROL 觀看活動]

此觸發器模組會在您指定的行事曆中新增、更新、刪除、開始或結束新事件時執行情境。 模組會傳回與一個或多個記錄相關聯的所有標準欄位，以及連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Calendar]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe[!DNL Workfront Fusion]的連線 — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL行事曆] </td> 
   <td> <p>選取您希望模組使用的行事曆。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL觀看活動]</td> 
   <td> <p>選擇您要依「建立日期」、「更新日期」、「開始日期」或「結束日期」觀看事件。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL顯示已刪除的事件]</td> 
   <td> <p>啟用此選項以包含已刪除的事件。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Query] </td> 
   <td> <p>輸入要搜尋的文字。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL限制]</td> 
   <td> <p> 設定[!DNL Workfront Fusion]在一個週期內處理的最大事件數（每個案例執行的重複數目）。 如果該值設定得太高，則在指定的第三方服務端可能會中斷連線（逾時）。 [!DNL Workfront Fusion]對此沒有影響。 我們建議您設定較低的值，並為最大週期數定義較高的值，或是更頻繁地執行情境。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 搜尋事件]

此動作模組會在選取的行事曆中搜尋事件。

您可以指定搜尋的行事曆和引數。

模組會傳回事件的ID和任何關聯欄位，以及連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td>如需有關將您的[!DNL Google Calendar]帳戶連線到Workfront Fusion的說明，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe Workfront Fusion的連線 — 基本說明</a></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL行事曆ID]</td> 
   <td> <p>選取您要搜尋的行事曆。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL開始日期]</td> 
   <td> <p> 輸入或對應事件開始的日期。 此模組也會擷取在此日期之前開始的、在輸入開始日期仍然發生的事件。 </p> <p>如需支援的日期和時間格式清單，請參閱<a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中鍵入強制。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL結束日期]</td> 
   <td> <p> 輸入或對應事件結束的日期。 </p> <p> 如需支援的日期和時間格式清單，請參閱<a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中鍵入強制。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL單一事件]</td> 
   <td> <p> 啟用此選項可將週期性事件視為單一例項。 例如，如果您有每週會議且已啟用此選項，模組會以個別事件的形式傳回每週的會議。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Query]</td> 
   <td> <p>輸入或對應您要搜尋的搜尋字詞。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Order by]</td> 
   <td> <p>選取結果中傳回事件的順序。</p> 
    <ul> 
     <li><strong>[！UICONTROL開始時間]</strong>：依開始日期和時間（升序）排序。 這僅在查詢單一事件時可用。</li> 
     <li><strong>[！UICONTROL更新時間]</strong>：依上次修改時間排序（升序）。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL限制]</td> 
   <td> <p>設定在一個執行週期內[!DNL Workfront Fusion]傳回的最大事件數。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得事件]

此動作模組會傳回指定日曆中單一事件的中繼資料。

您可以指定日曆和事件。

模組會傳回事件的ID和所有關聯的欄位，以及連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Calendar]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe[!DNL Workfront Fusion]的連線 — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL行事曆ID]</td> 
   <td> <p>輸入或對應包含您要取得之事件的行事曆ID。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL事件ID] </td> 
   <td> <p>輸入要取得的現有[!DNL Google Calendar]事件的事件識別碼。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立事件]

此動作模組會建立事件。

您可以指定事件的行事曆和引數。

模組會傳回事件的ID和任何關聯欄位，以及連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td>如需有關將您的[!DNL Google Calendar]帳戶連線到Workfront Fusion的說明，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe Workfront Fusion的連線 — 基本說明</a></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL建立事件]</td> 
   <td> <p>選取您要如何建立事件。</p> 
    <ul> 
     <li><b>[！UICONTROL詳細資料]</b><p>此選項可讓您更詳細地輸入有關事件的資訊。<br></p></li> 
     <li><b>[！UICONTROL快速]</b><p>您只需要選取行事曆並輸入事件的名稱。 您可以在名稱中包含時間和地點的詳細資訊，[!DNL Google Calendar]會針對該地點和時間排程事件。</p></li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL行事曆ID]</td> 
   <td> <p>選取您要顯示事件的行事曆。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL色彩]</td> 
   <td>選取事件在行事曆上顯示的顏色。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL事件名稱]</td> 
   <td> <p> 輸入或對應事件的名稱。 </p> <p>注意：如果您在[！UICONTROL建立事件]欄位中選取[！UICONTROL快速新增]，您可以包含事件的日期和時間，然後[!DNL Workfront Fusion]會針對該日期和時間建立事件。 範例： <code>Appointment at Capitol Hill on June 3rd 10am-10:25am</code>。 如果您選取[！UICONTROL快速新增]，但未在事件名稱中加入日期和時間，則事件將從目前時間建立並持續一小時。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL全天事件]</td> 
   <td>如果事件是全天事件（不需要開始和結束時間），則啟用此選項。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL開始日期]</td> 
   <td> <p>如果這是全天事件，請輸入事件的開始日期。 </p> <p>如需支援的日期格式清單，請參閱<a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中輸入強制格式。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL結束日期]</td> 
   <td> <p> 如果這是全天事件，請輸入事件的結束日期。 </p> <p>如需支援的日期格式清單，請參閱<a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中輸入強制格式。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL說明]</td> 
   <td>輸入或對應事件的說明。 此欄位支援HTML。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL位置]</td> 
   <td>以文字形式輸入事件的位置。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL使用此事件的預設提醒設定]</td> 
   <td>啟用此選項以使用預設提醒設定。 如果您在[！UICONTROL Reminder]欄位中設定自訂提醒，此值會設為「否」。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL提醒] </td> 
   <td> <p>新增事件提醒。 對於每個提醒，選取您要用來提醒的方法，並定義您要提醒的事件之前的時間長度（以分鐘為單位）。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL出席者]</td> 
   <td>將出席者新增至活動。 為每位出席者輸入或對應其姓名和電子郵件地址。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL顯示為]</td> 
   <td>選取您希望檢視您行事曆的人員在此活動期間將您視為「忙碌」或「可用」。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL可見性] </td> 
   <td> <p>選取此事件的可見性。 </p> 
    <ul> 
     <li> <p><b>[！UICONTROL預設值]</b></p> <p>事件具有您在行事曆設定中設定的可見度。</p> </li> 
     <li> <p><b>[！UICONTROL Public]</b></p> <p>與該行事曆共用之任何人都可以看見此事件。</p> </li> 
     <li> <p><b>[！UICONTROL Private]</b></p> <p>只有與會者可看見此活動。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL傳送有關事件建立的通知]</td> 
   <td> <p>選取是否將建立新事件的通知傳送給所有來賓、非[!DNL Google Calendar]來賓，或不要傳送給任何人。</p> <p>提示：我們建議僅在移轉使用案例中使用[！UICONTROL無]選項。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL來賓可以修改事件]</td> 
   <td> <p>如果您希望來賓能夠修改此事件，請啟用此選項。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL遞回]</td> 
   <td>新增您要套用至此事件的任何遞回規則。 每個規則都需要有[！UICONTROL RRULE]、[！UICONTROL EXRULE]、[！UICONTROL RDATE]和[！UICONTROL EXDATE]行的清單，才能處理週期性事件。 請注意，此欄位中不允許有[！UICONTROL DTSTART]和[！UICONTROL DTEND]行；事件的開始和結束時間是在開始和結束欄位中指定。 單一事件或週期性事件的例項會省略此欄位。 如需詳細資訊，請參閱<a href="https://tools.ietf.org/html/rfc5545#section-3.8.5">RFC5545</a>。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新事件]

此動作模組會變更現有事件。

您可以指定日曆和事件ID。

模組會傳回事件的ID和任何關聯欄位，以及連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Calendar]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe[!DNL Workfront Fusion]的連線 — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL行事曆] </td> 
   <td> <p>選取您要使用的行事曆。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL事件ID] </td> 
   <td> <p>輸入先前建立的[!DNL Google Calendar]事件中要更新的事件ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

您可以在所需欄位中輸入新值，以更新事件資訊。 如需個別欄位的詳細資訊，請參閱[[!UICONTROL 建立事件]](#create-an-event)。

#### [!UICONTROL 刪除事件]

此動作模組會刪除事件。

您可以指定日曆和事件ID。

模組會傳回事件的ID和任何關聯欄位，以及連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Calendar]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe[!DNL Workfront Fusion]的連線 — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL行事曆ID]</td> 
   <td> <p>選取包含您要刪除之事件的行事曆。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL事件ID]</td> 
   <td> <p> 輸入先前建立的[!DNL Google Calendar]要刪除之事件的事件ID。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL傳送有關事件刪除的通知]</td> 
   <td>選取您要將事件刪除通知傳送給所有來賓、未使用[!DNL Google Calendar]的來賓，或無來賓。</td> 
  </tr> 
 </tbody> 
</table>

### 行事曆

* [[!UICONTROL 列出行事曆]](#list-calendars)
* [[!UICONTROL 取得行事曆]](#get-a-calendar)
* [[!UICONTROL 建立行事曆]](#create-a-calendar)
* [[!UICONTROL 更新行事曆]](#update-a-calendar)
* [[!UICONTROL 刪除行事曆]](#delete-a-calendar)
* [[!UICONTROL 清除行事曆]](#clear-a-calendar)

#### [!UICONTROL 列出行事曆]

此動作模組會傳回使用者行事曆清單上的行事曆。

模組會傳回行事曆的ID及任何關聯欄位，連同連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Calendar]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe[!DNL Workfront Fusion]的連線 — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL最低存取角色]</td> 
   <td> <p>選取使用者的最小存取角色。 模組會根據此最小存取角色傳回行事曆。</p> 
    <ul> 
     <li><strong>[！UICONTROL空閒/忙碌Reader]</strong>：使用者可以讀取空閒/忙碌資訊。 </li> 
     <li><strong>[！UICONTROL擁有者]</strong>：使用者可以讀取和修改事件，也可以存取控制清單。 </li> 
     <li><strong>[！UICONTROLReader]</strong>：使用者可以讀取非私人事件。 </li> 
     <li><strong>[！UICONTROL Writer]</strong>：使用者可以讀取和修改事件。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL顯示隱藏行事曆]</td> 
   <td>啟用此選項可在模組傳回的清單中包含隱藏行事曆。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td>設定在一個執行週期內傳回行事曆[!DNL Workfront Fusion]的最大數目。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得行事曆]

此動作模組會擷取行事曆。

您可以指定要擷取的行事曆ID。

模組會傳回記錄ID及任何關聯欄位，連同連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Calendar]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe[!DNL Workfront Fusion]的連線 — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL行事曆ID]</td> 
   <td> <p>選取您要擷取的行事曆。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立行事曆]

此動作模組會建立新行事曆。

您可以指定行事曆的名稱。

模組會傳回行事曆的ID及任何關聯欄位，連同連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Calendar]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe[!DNL Workfront Fusion]的連線 — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL行事曆名稱]</td> 
   <td> <p> 輸入新行事曆的名稱。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新行事曆]

此動作模組會更新行事曆。

您可以指定要更新的行事曆識別碼。

模組會傳回行事曆的ID及任何關聯欄位，連同連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Calendar]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe[!DNL Workfront Fusion]的連線 — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL行事曆ID]</td> 
   <td> <p>選取您要更新的行事曆。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL行事曆名稱]</td> 
   <td> <p> 輸入行事曆的新名稱。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除行事曆]

此動作模組會刪除行事曆。

您可以指定要刪除的行事曆識別碼。

模組會傳回行事曆的ID及任何關聯欄位，連同連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Calendar]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe[!DNL Workfront Fusion]的連線 — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL行事曆ID]</td> 
   <td> <p>輸入或對應您要刪除的行事曆識別碼。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 清除行事曆]

此動作模組會從帳戶的主要行事曆移除所有事件。

您可以指定連線至包含您要清除之行事曆的帳戶。

模組會傳回行事曆的ID及任何關聯欄位，連同連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Calendar]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe[!DNL Workfront Fusion]的連線 — 基本指示</a></p> </td> 
  </tr> 
 </tbody> 
</table>

### 存取控制規則

* [[!UICONTROL 列出存取控制規則]](#list-access-control-rules)
* [[!UICONTROL 取得存取控制規則]](#get-an-access-control-rule)
* [[!UICONTROL 建立存取控制規則]](#create-an-access-control-rule)
* [[!UICONTROL 更新存取控制規則]](#update-an-access-control-rule)
* [[!UICONTROL 刪除存取控制規則]](#delete-an-access-control-rule)

#### [!UICONTROL 列出存取控制規則]

此動作模組會傳回行事曆上存取控制清單中的規則。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Calendar]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe[!DNL Workfront Fusion]的連線 — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL行事曆ID]</td> 
   <td> <p>選取包含您要擷取之存取控制規則的行事曆。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td>設定在一個執行週期內傳回的結果數目上限[!DNL Workfront Fusion]。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得存取控制規則]

此動作模組會傳回存取控制規則的中繼資料。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Calendar]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe[!DNL Workfront Fusion]的連線 — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL行事曆ID]</td> 
   <td> <p>選取包含您要擷取之存取控制規則的行事曆。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL存取控制規則ID]</td> 
   <td>選取您要擷取的存取控制規則。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立存取控制規則]

此動作模組會建立新的存取控制規則。

您可以指定行事曆的名稱。

模組會傳回存取控制規則ID及任何關聯欄位，連同連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Calendar]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe[!DNL Workfront Fusion]的連線 — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL行事曆ID]</td> 
   <td> <p>選取您要建立存取控制規則的行事曆。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL角色]</td> 
   <td> <p>選取要指派給存取規則的角色。 </p> 
    <ul> 
     <li><strong>[！UICONTROL空閒/忙碌Reader]</strong>：使用者可以讀取空閒/忙碌資訊。 </li> 
     <li><strong>[！UICONTROL擁有者]</strong>：使用者可以讀取和修改事件，也可以存取控制清單。 </li> 
     <li><strong>[！UICONTROLReader]</strong>：使用者可以讀取非私人事件。 </li> 
     <li><strong>[！UICONTROL Writer]</strong>：使用者可以讀取和修改事件。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL型別]</td> 
   <td> <p>選取範圍型別。 </p> 
    <ul> 
     <li><strong>[！UICONTROL預設值]</strong>：公用範圍。 這是預設值。 </li> 
     <li><strong>[！UICONTROL User]</strong>：將範圍限製為單一使用者。 </li> 
     <li><strong>[！UICONTROL群組]</strong>：將範圍限製為群組。 </li> 
     <li><strong>[！UICONTROL網域]</strong>：將範圍限製為網域。 </li> 
    </ul> <p>注意：授與[！UICONTROL Default]或公用範圍的許可權適用於未經驗證的任何使用者。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL值]</td> 
   <td>根據範圍型別，輸入使用者或群組的電子郵件地址，或網域名稱。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL傳送通知]</td> 
   <td> <p>啟用此選項以傳送有關存取變更的通知。 </p> <p>注意：移除存取權時沒有通知。 </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新存取控制規則]

此動作模組會更新存取控制規則。

您可以指定行事曆的名稱。

模組會傳回存取控制規則ID及任何關聯欄位，連同連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Calendar]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe[!DNL Workfront Fusion]的連線 — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL行事曆ID]</td> 
   <td> <p>選取包含您要更新之存取控制規則的行事曆。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL存取控制規則ID]</td> 
   <td>選取要更新的存取控制規則。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL角色]</td> 
   <td> <p>選取要指派給存取規則的角色。 </p> 
    <ul> 
     <li><strong>[！UICONTROL None]</strong>：此角色不提供存取權。</li> 
     <li><strong>[！UICONTROL空閒/忙碌Reader]</strong>：使用者可以讀取空閒/忙碌資訊。 </li> 
     <li><strong>[！UICONTROL擁有者]</strong>：使用者可以讀取和修改事件，也可以存取控制清單。 </li> 
     <li><strong>[！UICONTROLReader]</strong>：使用者可以讀取非私人事件。 </li> 
     <li><strong>[！UICONTROL Writer]</strong>：使用者可以讀取和修改事件。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL傳送通知]</td> 
   <td> <p>啟用此選項以傳送有關存取變更的通知。 </p> <p>注意：移除存取權時沒有通知。 </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除存取控制規則]

此動作模組會刪除存取控制規則。

您可以指定行事曆的名稱。

模組會傳回存取控制規則ID及任何關聯欄位，連同連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>如需有關將您的[!DNL Google Calendar]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe[!DNL Workfront Fusion]的連線 — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL行事曆ID]</td> 
   <td> <p>選取或對應包含您要刪除之存取控制規則的行事曆的ID。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL存取控制規則ID]</td> 
   <td>選取或對應您要刪除之存取控制規則的ID。</td> 
  </tr> 
 </tbody> 
</table>

### 迭代器（已棄用）

已棄用[!UICONTROL 迭代附件]與[!UICONTROL 迭代出席者]模組。 若要疊代附件或出席者，請使用[!UICONTROL 流量控制] > [!UICONTROL 疊代器]模組。 如需詳細資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md)中的[疊代器模組

### 其他

* [[!UICONTROL 進行API呼叫]](#make-an-api-call)
* [[!UICONTROL 取得空閒/忙碌資訊]](#get-freebusy-information)

#### [!UICONTROL 進行API呼叫]

此模組可讓您執行自訂API呼叫。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>如需有關將您的[!DNL Google Calendar]帳戶連線到[!DNL Workfront Fusion]的指示，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe[!DNL Workfront Fusion]的連線 — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL URL]</p> </td> 
   <td>輸入相對於<code>https://www.googleapis.com/calendar</code>的路徑。 範例： <code>/v3/users/me/calendarList</code></td> 
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
   <td> <p>以標準JSON物件的形式新增API呼叫的內文內容。</p> <p>注意：   <p>在JSON中使用條件陳述式（例如<code>if</code>）時，請將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得空閒/忙碌資訊]

此動作模組會傳回一組行事曆的空閒/忙碌資訊。

模組會傳回行事曆的ID及任何關聯欄位，連同連線存取的任何自訂欄位和值。 您可以在情境中的後續模組中對應此資訊。

當您設定此模組時，會顯示下列欄位。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td>如需有關將您的[!DNL Google Calendar]帳戶連線到Workfront Fusion的說明，請參閱<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與Adobe Workfront Fusion的連線 — 基本說明</a></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL最短時間]</td> 
   <td> <p> 輸入您要擷取資訊的間隔的開始。</p> <p> 如需支援的日期和時間格式清單，請參閱<a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中鍵入強制。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL最長時間]</td> 
   <td> <p> 輸入您要擷取資訊的間隔結束。 </p> <p>如需支援的日期和時間格式清單，請參閱<a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中鍵入強制。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL行事曆]</td> 
   <td> <p>針對您想要擷取資訊的每個行事曆，按一下<strong>新增</strong>，然後輸入或對應行事曆ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 在事件之前觸發案例

您可以在事件之前的指定時間觸發案例，並透過標準[!DNL Google Calendar]電子郵件提醒和[!UICONTROL Webhook] >[!UICONTROL 自訂mailhook]模組提供協助。

1. 使用[!UICONTROL Google行事曆] >[!UICONTROL 更新活動]模組將電子郵件提醒新增至您的活動：

   ![](assets/trigger-scen-before-event-350x209.png)

1. 從[!UICONTROL Webhook] >[!UICONTROL 自訂mailhook]模組開始建立新情境。

   1. 複製mailhook的電子郵件地址。
   1. 儲存情境並執行情境。

1. 在[!DNL Gmail]中，將[!DNL Google Calendar]電子郵件提醒重新導向至mailhook的電子郵件地址：

   1. 開啟您的&#x200B;**[!UICONTROL [!DNL Gmail]設定]**。
   1. 開啟&#x200B;**[!UICONTROL 轉送和POP/IMAP]**&#x200B;標籤。
   1. 按一下&#x200B;**[!UICONTROL 新增轉寄地址].**
   1. 貼上複製的郵件鉤子的電子郵件地址，按&#x200B;**[!UICONTROL 下一步]**，在快顯視窗中按&#x200B;**[!UICONTROL 繼續]**&#x200B;進行確認，然後按一下&#x200B;**[!UICONTROL 確定]**。

   1. 在[!DNL Workfront Fusion]中，切換至應透過接收確認電子郵件完成其執行的新案例。
   1. 按一下模組上方的泡泡圖示，檢查模組的輸出。
   1. 展開`Text`專案並複製確認代碼：

      ![](assets/confirmation-code-350x252.png)

   1. 在Gmail中，將確認代碼貼到編輯方塊中，然後按一下&#x200B;**[!UICONTROL 驗證]**：

      ![](assets/paste-code-350x46.png)

   1. 開啟&#x200B;**[!UICONTROL 篩選器和封鎖的地址]**&#x200B;索引標籤。
   1. 按一下&#x200B;**[!UICONTROL 建立新篩選器]**。
   1. 為來自`     calendar-notification@google.com`的所有電子郵件設定篩選器，然後按一下&#x200B;**[!UICONTROL 建立篩選器]**：
   1. 選取&#x200B;**[!UICONTROL 將其轉寄至]**，並從清單中選擇Mailhook的電子郵件地址。
   1. 按一下&#x200B;**[!UICONTROL 建立篩選器]**&#x200B;以建立篩選器。

1. （選擇性）在[!DNL Workfront Fusion]中，在[!UICONTROL Webhooks] >[!UICONTROL 自訂mailhook]模組之後新增[!UICONTROL 文字剖析器] > [!UICONTROL 符合模式]模組，以剖析電子郵件的HTML代碼，以取得您所需的任何資訊。

   例如，您可以依照以下方式設定模組，以取得事件的ID：

   *模式*： `<meta itemprop="eventId/googleCalendar" content="(?<evenitID>.*?)"/>`

   *文字*：從[!UICONTROL Webhook] >[!UICONTROL 自訂mailhook]模組輸出的`HTML content`專案。
