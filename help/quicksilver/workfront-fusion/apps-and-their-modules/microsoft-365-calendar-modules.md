---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;calendars
keywords: 連接器
navigation-topic: apps-and-their-modules
title: Microsoft Office 365日曆
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用Microsoft Office 365日曆的工作流程，並將其連接到多個第三方應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: 814c285e-c106-458a-a0b1-760677634f4f
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1835'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Calendar]

在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動執行使用 [!DNL Microsoft Office 365 Calendar]，並將其連接至多個協力廠商應用程式和服務。

為了使用 [!DNL Office 365 Calendar] with [!DNL Adobe Workfront Fusion]，則必須有 [!DNL Office 365 Excel] 帳戶。 您可以在建立 [www.office.com](http://www.office.com/).

有關將Office 365帳戶連接到 [!DNL Workfront Fusion]，請參閱 [建立連線以Adobe [!DNL Workfront Fusion]  — 基本指示](../../workfront-fusion/connections/connect-to-fusion-general.md)

授與同意後，系統會將您重新導向回 [!UICONTROL Workfront融合] 「管理」頁面，您可以在此處繼續建立案例。

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

使用 [!DNL Microsoft Office 365 Calendar] 模組，您必須 [!DNL Microsoft Office 365 Calendar] 帳戶。

## [!DNL Microsoft Office 365 Calendar] 模組及其欄位

設定時 [!DNL Microsoft Office 365 Calendar] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 此外， [!DNL Microsoft Office 365 Calendar] 視您在應用程式或服務中的存取層級等因素而定，可能會顯示欄位。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [將資訊從一個模組對應到 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Event](#event)
* [行事曆](#calendar)
* [其他](#other)

### Event

* [[!UICONTROL 觀看事件]](#watch-events)
* [[!UICONTROL 搜尋事件]](#search-events)
* [[!UICONTROL 取得事件]](#get-an-event)
* [[!UICONTROL 建立事件]](#create-an-event)
* [[!UICONTROL 更新事件]](#update-an-event)
* [[!UICONTROL 刪除事件]](#delete-an-event)

#### [!UICONTROL 觀看事件]

此觸發器模組會在選取的日曆中建立、更新、刪除、啟動或結束事件時，擷取事件的詳細資訊。

>[!NOTE]
>
>要監視事件系列的已刪除發生次數，請選擇 [!UICONTROL 按更新時間] 在 [!UICONTROL 觀看事件] 欄位。 此模組不會監看已刪除的單一事件或已刪除的事件系列。


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL監看事件]</td> 
   <td> <p>選取您要如何監看事件。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL按建立時間]</strong> </p> <p>留意新事件。</p> </li> 
     <li> <p><strong>[!UICONTROL按更新時間]</strong> </p> <p>觀看更新的事件。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL日曆組ID]</td> 
   <td>選擇包含要監視事件的日曆的[!UICONTROL日曆組]。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL日曆]</td> 
   <td> <p>選取您要觀看的特定日曆。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL篩選器]</td> 
   <td>設定篩選條件，以依主旨、事件ID或內文篩選結果。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>輸入最大消息數 [!DNL Workfront Fusion] 應會在一個案例執行週期期間傳回。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 搜尋事件]

此搜尋模組會在選取的日曆中建立、更新、刪除、啟動或結束事件時，保留事件的詳細資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL日曆組ID]</td> 
   <td>選擇包含要監視事件的日曆的[!UICONTROL日曆組]。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL日曆]</td> 
   <td> <p>選取您要觀看的特定日曆。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL篩選器]</td> 
   <td> <p>設定篩選條件以篩選結果。 您可以依下列屬性進行篩選：</p> 
    <ul> 
     <li>[!UICONTROL主題]</li> 
     <li>[!UICONTROL事件ID]</li> 
     <li>[!UICONTROL建立日期時間]</li> 
     <li>[!UICONTROL上次修改日期時間]</li> 
     <li>[!UICONTROL主體預覽]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL順序依]</td> 
   <td> <p>選擇要如何排序結果。</p> 
    <ul> 
     <li><strong>[!UICONTROL主題]</strong>，遞增或遞減</li> 
     <li><strong>[!UICONTROL建立日期時間]</strong>，遞增或遞減</li> 
     <li><strong>[!UICONTROL上次修改日期時間]</strong>，遞增或遞減</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td>輸入事件數上限 [!DNL Workfront Fusion] 應會在一個案例執行週期期間傳回。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得事件]

此動作模組會擷取指定事件的詳細資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL事件ID]</td> 
   <td> <p>輸入或映射要檢索詳細資訊的事件ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立事件]

此動作模組會建立新事件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主題]</td> 
   <td> <p>輸入或對應已建立事件的標題。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL開始日期]</td> 
   <td> 輸入事件以合併的日期和時間表示形式開始的單一時間點。 使用格式 <code>({date}T{time}</code>;例如， <code>2017-08-29T04:00:00.0000000</code>. 如需支援的日期和時間格式清單，請參閱 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">中的強制類型 [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL結束日期]</td> 
   <td> 輸入事件以合併的日期和時間表示形式結束的單一時間點。 使用格式 <code>{date}T{time}</code>;例如， <code>2017-08-29T04:00:00.0000000</code>. 如需支援的日期和時間格式清單，請參閱 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">中的強制類型 [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL上的提醒]</td> 
   <td>選擇是否為此事件激活提醒。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL提醒]</td> 
   <td>輸入或映射事件開始前應觸發提醒的分鐘數。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL重要性]</td> 
   <td> <p>選取此事件的重要性。</p> 
    <ul> 
     <li>[!UICONTROL低]</li> 
     <li>[!UICONTROL Medium]</li> 
     <li>[!UICONTROL高]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL敏感度] </td> 
   <td> <p>選擇此事件的敏感性。</p> 
    <ul> 
     <li><strong>[!UICONTROL標準]</strong> </li> 
     <li> <p><strong>[!UICONTROL Personal]</strong> </p> <p>收件者會看到「[!UICONTROL請將此郵件視為Personal]」訊息。</p> </li> 
     <li> <p><strong>[!UICONTROL專用]</strong> </p> <p>收件者會看到「[!UICONTROL請將此資訊視為專用]」訊息。 收件者的收件匣規則不會轉送或重新導向此事件。</p> </li> 
     <li> <p><strong>[!UICONTROL機密]</strong> </p> <p>收件者看到「[!UICONTROL請將此資訊視為機密]」訊息。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主體內容類型]</td> 
   <td>選取內文內容為純文字或HTML。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL內文]</td> 
   <td>輸入或映射與事件關聯的消息正文。 它可以是HTML或文字格式（如上方[!UICONTROL Body Content Type]欄位中所指定）。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL位置]</td> 
   <td> <p>輸入事件位置詳細資訊。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！已請求UICONTROL響應]</td> 
   <td>選擇 <strong>[!UICONTROL是]</strong> 請求被邀請者發送對事件邀請的響應。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL顯示為]</td> 
   <td> <p>選取要讓活動對檢視日曆的使用者顯示的方式。</p> 
    <ul> 
     <li>[!UICONTROL免費]</li> 
     <li>[!UICONTROL暫定]</li> 
     <li>[!UICONTROL忙]</li> 
     <li>[!UICONTROL已停用]</li> 
     <li>[!UICONTROL在其他位置工作]</li> 
     <li>[!UICONTROL未知]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL與會者]</p> </td> 
   <td> <p>添加活動出席者。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL名稱]</strong> </p> <p>輸入與會者的姓名。</p> </li> 
     <li> <p><strong>[!UICONTROL電子郵件]</strong> </p> <p>輸入與會者的電子郵件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL類別]</td> 
   <td>輸入或對應您要事件在日曆上顯示為的類別。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新事件]

此動作模組會更新現有事件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL事件ID]</td> 
   <td>輸入、對應或選取您要更新之事件的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主題]</td> 
   <td> <p>輸入或對應已建立事件的標題。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL開始日期]</td> 
   <td> 輸入事件以合併的日期和時間表示形式開始的單一時間點。 使用格式 <code>{date}T{time}</code>;例如， <code>2017-08-29T04:00:00.0000000</code>. 如需支援的日期和時間格式清單，請參閱 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">中的強制類型 [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL結束日期]</td> 
   <td> 輸入事件以合併的日期和時間表示形式結束的單一時間點。 使用格式 <code>({date}T{time}</code>;例如， <code>2017-08-29T04:00:00.0000000</code>. 如需支援的日期和時間格式清單，請參閱 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">中的強制類型 [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL上的提醒]</td> 
   <td>選擇是否為此事件激活提醒。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL提醒]</td> 
   <td>輸入或映射事件開始前應觸發提醒的分鐘數。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL重要性]</td> 
   <td> <p>選取此事件的重要性。</p> 
    <ul> 
     <li>[!UICONTROL低]</li> 
     <li>[!UICONTROL Medium]</li> 
     <li>[!UICONTROL高]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL敏感度] </td> 
   <td> <p>選擇此事件的敏感性。</p> 
    <ul> 
     <li><strong>[!UICONTROL標準]</strong> </li> 
     <li> <p><strong>[!UICONTROL Personal]</strong> </p> <p>收件者會看到「[!UICONTROL請將此郵件視為Personal]」訊息。</p> </li> 
     <li> <p><strong>[!UICONTROL專用]</strong> </p> <p>收件者會看到「[!UICONTROL請將此資訊視為專用]」訊息。 收件者的收件匣規則不會轉送或重新導向此事件。</p> </li> 
     <li> <p><strong>[!UICONTROL機密]</strong> </p> <p>收件者看到「[!UICONTROL請將此資訊視為機密]」訊息。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主體內容類型]</td> 
   <td>選取與事件相關聯的訊息內文內容為純文字或HTML。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL內文]</td> 
   <td>輸入或映射與事件關聯的消息正文。 它可以是HTML或文字格式（如上方[!UICONTROL Body Content Type]欄位中所指定）。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL位置]</td> 
   <td> <p>輸入事件位置詳細資訊。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！已請求UICONTROL響應]</td> 
   <td>選擇 <strong>[!UICONTROL是]</strong> 請求被邀請者發送對事件邀請的響應。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL顯示為]</td> 
   <td> <p>選取要讓活動對檢視日曆的使用者顯示的方式。</p> 
    <ul> 
     <li>[!UICONTROL免費]</li> 
     <li>[!UICONTROL暫定]</li> 
     <li>[!UICONTROL忙]</li> 
     <li>[!UICONTROL已停用]</li> 
     <li>[!UICONTROL在其他位置工作]</li> 
     <li>[!DNL Unknown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL與會者]</p> </td> 
   <td> <p>添加活動出席者。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL名稱]</strong> </p> <p>輸入與會者的姓名。</p> </li> 
     <li> <p><strong>[!UICONTROL電子郵件]</strong> </p> <p>輸入與會者的電子郵件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL類別]</td> 
   <td>輸入或對應您要事件在日曆上顯示為的類別。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除事件]

此動作模組會刪除現有事件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL事件ID]</td> 
   <td> <p>輸入或對應您要刪除之事件的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 行事曆

* [[!UICONTROL 清單日曆]](#list-calendars)
* [[!UICONTROL 取得日曆]](#get-a-calendar)
* [[!UICONTROL 建立日曆]](#create-a-calendar)
* [[!UICONTROL 更新日曆]](#update-a-calendar)
* [[!UICONTROL 刪除日曆]](#delete-a-calendar)

#### [!UICONTROL 清單日曆]

此搜尋模組會擷取所有已驗證使用者日曆的清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL日曆組ID]</td> 
   <td>選擇包含要列出的日曆的[!UICONTROL日曆組]。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td>輸入日曆的最大數量 [!DNL Workfront Fusion] 應會在一個案例執行週期期間傳回。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得日曆]

此動作模組會擷取單一日曆的詳細資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL日曆ID]</td> 
   <td> <p>輸入或映射要檢索有關詳細資訊的日曆的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立日曆]

此動作模組會在您的Google帳戶中建立新日曆。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL日曆名稱]</td> 
   <td> <p>輸入新日曆的名稱。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新日曆]

此動作模組會編輯現有的日曆。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL日曆ID]</td> 
   <td>輸入要更新日曆的[!UICONTROL日曆ID]。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL新日曆名稱]</td> 
   <td> <p>輸入新日曆的名稱。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除日曆]

此動作模組會刪除現有的日曆。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL日曆ID]</td> 
   <td>輸入要刪除的日曆的[!UICONTROL日曆] ID。</td> 
  </tr> 
 </tbody> 
</table>

### 其他

#### [!UICONTROL 進行API呼叫]

此模組可讓您執行自訂API呼叫。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL連接]</td> 
   <td role="rowheader">[!UICONTROL連接] </td> 
   <td> <p>有關連接 [!DNL Office 365] 帳戶 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立連線至 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>輸入相對於的路徑 <code>https://graph.microsoft.com</code>. 範例:<code> /v1.0/me/events</code></p> </td> 
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
