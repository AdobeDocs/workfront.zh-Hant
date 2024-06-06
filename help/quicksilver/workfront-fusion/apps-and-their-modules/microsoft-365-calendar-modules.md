---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;calendars
keywords: 聯結器
navigation-topic: apps-and-their-modules
title: Microsoft Office 365行事曆
description: 在 [!DNL Adobe Workfront Fusion] 案例中，您可以自動化使用Microsoft Office 365行事曆的工作流程，並將其連線到多個協力廠商應用程式和服務。
author: Becky
feature: Workfront Fusion
exl-id: 814c285e-c106-458a-a0b1-760677634f4f
source-git-commit: 7d5f7c21fe38d43fb5601c81b8a31cc80587848f
workflow-type: tm+mt
source-wordcount: '1999'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Calendar]

在 [!DNL Adobe Workfront Fusion] 情境中，您可以使用自動化工作流程 [!DNL Microsoft Office 365 Calendar]，並連結至多個協力廠商應用程式和服務。

為了使用 [!DNL Office 365 Calendar] 替換為 [!DNL Adobe Workfront Fusion]，您必須擁有 [!DNL Office 365 Excel] 帳戶。 您可以在下列位置建立一個 [www.office.com](https://www.office.com/).

如需有關將您的Office 365帳戶連線至的說明 [!DNL Workfront Fusion]，請參閱 [建立與Adobe的連線 [!DNL Workfront Fusion]  — 基本指示](../../workfront-fusion/connections/connect-to-fusion-general.md)

在您同意後，系統會將您重新導向回 [!UICONTROL Workfront Fusion] 「管理」頁面，您可以在此頁面繼續建立情境。

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

使用 [!DNL Microsoft Office 365 Calendar] 模組，您必須擁有 [!DNL Microsoft Office 365 Calendar] 帳戶。

## 連線 [!DNL Office 365 Calendar] 服務對象 [!DNL Workfront Fusion]

如需有關連線您的電腦的指示 [!DNL Office 365 Calendar] 帳戶至 [!UICONTROL Workfront Fusion]，請參閱 [建立與的連線 [!UICONTROL Adobe Workfront Fusion]  — 基本指示](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>部分Microsoft應用程式使用相同的連線，而此連線會繫結至個別使用者許可權。 因此，在建立連線時，許可權同意畫面會顯示先前授與此使用者連線的所有許可權，以及目前應用程式所需的任何新許可權。
>
>例如，如果使用者擁有透過Excel聯結器授予的「讀取表格」許可權，然後在Outlook聯結器中建立連線以讀取電子郵件，則許可權同意畫面會顯示已授予的「讀取表格」許可權和新要求的「寫入電子郵件」許可權。

## [!DNL Microsoft Office 365 Calendar] 模組及其欄位

當您設定 [!DNL Microsoft Office 365 Calendar] 模組， [!DNL Workfront Fusion] 顯示下列欄位。 除了這些以外， [!DNL Microsoft Office 365 Calendar] 欄位可能會顯示，端視您應用程式或服務中的存取層級等因素而定。 模組中的粗體標題表示必填欄位。

如果您在欄位或函式上方看到對應按鈕，則可以使用它來設定該欄位的變數和函式。 如需詳細資訊，請參閱 [在中將資訊從一個模組對應到另一個模組 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [事件](#event)
* [行事曆](#calendar)
* [其他](#other)

### 事件

* [[!UICONTROL 觀看活動]](#watch-events)
* [[!UICONTROL 搜尋事件]](#search-events)
* [[!UICONTROL 取得事件]](#get-an-event)
* [[!UICONTROL 建立事件]](#create-an-event)
* [[!UICONTROL 更新事件]](#update-an-event)
* [[!UICONTROL 刪除事件]](#delete-an-event)

#### [!UICONTROL 觀看活動]

在所選行事曆中建立、更新、刪除、開始或結束事件時，此觸發程式模組會擷取事件的詳細資料。

>[!NOTE]
>
>若要觀看事件序列刪除的相符項，請選取「 」 [!UICONTROL 依更新時間] 在 [!UICONTROL 觀看活動] 欄位。 此模組不會監視已刪除的單一事件或刪除的事件系列。


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL Office 365] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL觀看活動]</td> 
   <td> <p>選取您要如何觀看活動。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL By Created Time]</strong> </p> <p>觀看新活動。</p> </li> 
     <li> <p><strong>[！UICONTROL，按更新時間]</strong> </p> <p>觀看更新事件。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL行事曆群組ID]</td> 
   <td>選取包含您要觀看活動之日曆的[！UICONTROL日曆群組]。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL行事曆]</td> 
   <td> <p>選取您要觀看的特定行事曆。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL篩選器]</td> 
   <td>設定篩選條件，依主旨、事件ID或本文篩選結果。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>輸入訊息數目上限 [!DNL Workfront Fusion] 應該會在一個案例執行週期中傳回。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 搜尋事件]

此搜尋模組會在所選行事曆中建立、更新、刪除、開始或結束事件時，擷取事件的詳細資料。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL Office 365] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL行事曆群組ID]</td> 
   <td>選取包含您要觀看活動之日曆的[！UICONTROL日曆群組]。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL行事曆]</td> 
   <td> <p>選取您要觀看的特定行事曆。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL篩選器]</td> 
   <td> <p>設定篩選條件以篩選結果。 您可以依下列屬性篩選：</p> 
    <ul> 
     <li>[！UICONTROL主旨]</li> 
     <li>[！UICONTROL事件ID]</li> 
     <li>[！UICONTROL建立日期時間]</li> 
     <li>[！UICONTROL上次修改日期時間]</li> 
     <li>[！UICONTROL Body Preview]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Order by]</td> 
   <td> <p>選取您要如何排序結果。</p> 
    <ul> 
     <li><strong>[！UICONTROL主旨]</strong>，遞增或遞減</li> 
     <li><strong>[！UICONTROL建立日期時間]</strong>，遞增或遞減</li> 
     <li><strong>[！UICONTROL上次修改日期時間]</strong>，遞增或遞減</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td>輸入事件數目上限 [!DNL Workfront Fusion] 應該會在一個案例執行週期中傳回。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得事件]

此動作模組會擷取指定事件的詳細資料。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL Office 365] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL事件ID]</td> 
   <td> <p>輸入或對應您要擷取其詳細資訊之事件的ID。</p> </td> 
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
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL Office 365] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL主旨]</td> 
   <td> <p>輸入或對應已建立事件的標題。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL開始日期]</td> 
   <td> 輸入事件在合併的日期和時間表示中開始時的單一時間點。 使用格式 <code>({date}T{time}</code>；例如， <code>2017-08-29T04:00:00.0000000</code>. 如需支援的日期和時間格式清單，請參閱 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">輸入強制 [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL結束日期]</td> 
   <td> 當事件以合併的日期和時間表示結束時，請輸入單一時間點。 使用格式 <code>{date}T{time}</code>；例如， <code>2017-08-29T04:00:00.0000000</code>. 如需支援的日期和時間格式清單，請參閱 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">輸入強制 [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL提醒於]</td> 
   <td>選取是否要為此事件啟用提醒。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL提醒]</td> 
   <td>輸入或對應提醒觸發時，事件開始前的分鐘數。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL重要性]</td> 
   <td> <p>選取此事件的重要性。</p> 
    <ul> 
     <li>[！UICONTROL低]</li> 
     <li>[！UICONTROL Medium]</li> 
     <li>[！UICONTROL高]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL敏感度] </td> 
   <td> <p>選取此事件的敏感度。</p> 
    <ul> 
     <li><strong>[！UICONTROL Normal]</strong> </li> 
     <li> <p><strong>[！UICONTROL Personal]</strong> </p> <p>收件者看到「[！UICONTROL請將此視為個人]」訊息。</p> </li> 
     <li> <p><strong>[！UICONTROL Private]</strong> </p> <p>收件者看到「[！UICONTROL請將此視為私人]」訊息。 收件者的收件匣規則不會轉寄或重新導向此事件。</p> </li> 
     <li> <p><strong>[！UICONTROL機密檔案]</strong> </p> <p>收件者看到「[！UICONTROL請將此視為機密]」訊息。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL內文內容型別]</td> 
   <td>選取內文內容是純文字還是HTML。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL內文內容]</td> 
   <td>輸入或對應與事件相關之訊息的正文。 它可以是HTML或文字格式（如上方[！UICONTROL Body Content Type]欄位中所指定）。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL位置]</td> 
   <td> <p>輸入事件地點詳細資料。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">已要求[！UICONTROL回應]</td> 
   <td>選取 <strong>[！UICONTROL是]</strong> 要求受邀者傳送活動邀請的回應。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL顯示為]</td> 
   <td> <p>選取您想要讓檢視您行事曆的人員看到事件的方式。</p> 
    <ul> 
     <li>[！UICONTROL自由]</li> 
     <li>[！UICONTROL Tentative]</li> 
     <li>[！UICONTROL忙碌]</li> 
     <li>[！UICONTROL外出]</li> 
     <li>[！UICONTROL在其他地方工作]</li> 
     <li>[！UICONTROL未知]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL出席者]</p> </td> 
   <td> <p>新增活動的出席者。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL名稱]</strong> </p> <p>輸入出席者的名稱。</p> </li> 
     <li> <p><strong>[！UICONTROL電子郵件]</strong> </p> <p>輸入出席者的電子郵件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL類別]</td> 
   <td>輸入或對應您希望事件在行事曆上顯示的類別。</td> 
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
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL Office 365] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL事件ID]</td> 
   <td>輸入、對應或選取您要更新之事件的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL主旨]</td> 
   <td> <p>輸入或對應已建立事件的標題。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL開始日期]</td> 
   <td> 輸入事件在合併的日期和時間表示中開始時的單一時間點。 使用格式 <code>{date}T{time}</code>；例如， <code>2017-08-29T04:00:00.0000000</code>. 如需支援的日期和時間格式清單，請參閱 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">輸入強制 [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL結束日期]</td> 
   <td> 當事件以合併的日期和時間表示結束時，請輸入單一時間點。 使用格式 <code>({date}T{time}</code>；例如， <code>2017-08-29T04:00:00.0000000</code>. 如需支援的日期和時間格式清單，請參閱 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">輸入強制 [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL提醒於]</td> 
   <td>選取是否要為此事件啟用提醒。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL提醒]</td> 
   <td>輸入或對應提醒觸發時，事件開始前的分鐘數。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL重要性]</td> 
   <td> <p>選取此事件的重要性。</p> 
    <ul> 
     <li>[！UICONTROL低]</li> 
     <li>[！UICONTROL Medium]</li> 
     <li>[！UICONTROL高]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL敏感度] </td> 
   <td> <p>選取此事件的敏感度。</p> 
    <ul> 
     <li><strong>[！UICONTROL Normal]</strong> </li> 
     <li> <p><strong>[！UICONTROL Personal]</strong> </p> <p>收件者看到「[！UICONTROL請將此視為個人]」訊息。</p> </li> 
     <li> <p><strong>[！UICONTROL Private]</strong> </p> <p>收件者看到「[！UICONTROL請將此視為私人]」訊息。 收件者的收件匣規則不會轉寄或重新導向此事件。</p> </li> 
     <li> <p><strong>[！UICONTROL機密檔案]</strong> </p> <p>收件者看到「[！UICONTROL請將此視為機密]」訊息。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL內文內容型別]</td> 
   <td>選取與事件相關之訊息的內文內容為純文字還是HTML。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL內文內容]</td> 
   <td>輸入或對應與事件相關之訊息的正文。 它可以是HTML或文字格式（如上方[！UICONTROL Body Content Type]欄位中所指定）。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL位置]</td> 
   <td> <p>輸入事件地點詳細資料。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">已要求[！UICONTROL回應]</td> 
   <td>選取 <strong>[！UICONTROL是]</strong> 要求受邀者傳送活動邀請的回應。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL顯示為]</td> 
   <td> <p>選取您想要讓檢視您行事曆的人員看到事件的方式。</p> 
    <ul> 
     <li>[！UICONTROL自由]</li> 
     <li>[！UICONTROL Tentative]</li> 
     <li>[！UICONTROL忙碌]</li> 
     <li>[！UICONTROL外出]</li> 
     <li>[！UICONTROL在其他地方工作]</li> 
     <li>[!DNL Unknown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL出席者]</p> </td> 
   <td> <p>新增活動的出席者。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL名稱]</strong> </p> <p>輸入出席者的名稱。</p> </li> 
     <li> <p><strong>[！UICONTROL電子郵件]</strong> </p> <p>輸入出席者的電子郵件地址。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL類別]</td> 
   <td>輸入或對應您希望事件在行事曆上顯示的類別。</td> 
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
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL Office 365] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL事件ID]</td> 
   <td> <p>輸入或對應您要刪除之事件的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 行事曆

* [[!UICONTROL 清單行事曆]](#list-calendars)
* [[!UICONTROL 取得行事曆]](#get-a-calendar)
* [[!UICONTROL 建立行事曆]](#create-a-calendar)
* [[!UICONTROL 更新行事曆]](#update-a-calendar)
* [[!UICONTROL 刪除行事曆]](#delete-a-calendar)

#### [!UICONTROL 清單行事曆]

此搜尋模組會擷取所有已驗證使用者行事曆的清單。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL Office 365] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL行事曆群組ID]</td> 
   <td>選取包含要列出之行事曆的[！UICONTROL行事曆群組]。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td>輸入行事曆數目上限 [!DNL Workfront Fusion] 應該會在一個案例執行週期中傳回。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得行事曆]

此動作模組會擷取單一行事曆的詳細資料。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL Office 365] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL行事曆ID]</td> 
   <td> <p>輸入或對應您要擷取其詳細資訊的行事曆的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 建立行事曆]

此動作模組會在您的Google帳戶中建立新行事曆。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL Office 365] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL行事曆名稱]</td> 
   <td> <p>輸入新行事曆的名稱。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新行事曆]

此動作模組會編輯現有行事曆。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL Office 365] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL行事曆ID]</td> 
   <td>為您要更新的行事曆輸入[！UICONTROL行事曆ID]。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL新行事曆名稱]</td> 
   <td> <p>輸入新行事曆的名稱。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刪除行事曆]

此動作模組會刪除現有的行事曆。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL Office 365] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL行事曆ID]</td> 
   <td>輸入您要刪除之行事曆的[！UICONTROL行事曆] ID。</td> 
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
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>如需有關連線您的電腦的指示 [!DNL Office 365] 帳戶至 [!DNL Workfront Fusion]，請參閱 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">建立與的連線 [!DNL Adobe Workfront Fusion]  — 基本指示</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL URL]</p> </td> 
   <td> <p>輸入相對於 <code>https://graph.microsoft.com</code>. 範例：<code> /v1.0/me/events</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL方法]</p> </td> 
   td&gt; <p>選取設定API呼叫所需的HTTP要求方法。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP要求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers]</td> 
   <td> <p>以標準JSON物件的形式新增請求的標頭。例如， <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] 為您新增授權標頭。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查詢字串]</td> 
   <td> <p> 以標準JSON物件的形式新增API呼叫的查詢。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Body]</td> 
   <td> <p>以標準JSON物件的形式新增API呼叫的內文內容。</p> <p>注意：   <p>使用條件陳述式時，例如 <code>if</code> 在JSON中，將引號放在條件陳述式之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>
