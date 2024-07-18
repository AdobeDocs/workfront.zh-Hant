---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 使用Adobe Workfront Fusion Devtool除錯案例
description: Adobe Workfront Fusion Devtool可讓您瞭解情境並疑難排解。 Devtool將額外的面板新增至Chrome開發人員工具。 使用此偵錯工具面板，您可以檢查案例的所有手動執行、檢閱所有已執行的操作，並檢視每個已執行API呼叫的詳細資訊。 您可以檢視導致錯誤的模組、操作或單一回應，並運用該知識來調整您的案例。
author: Becky
feature: Workfront Fusion
exl-id: f7557214-3615-4797-b4cb-4af70e4797ac
source-git-commit: 6edcb5b826bdcf37b62396a926c923875a3a1436
workflow-type: tm+mt
source-wordcount: '1858'
ht-degree: 1%

---

# 使用[!DNL Adobe Workfront Fusion] Devtool偵錯案例

[!DNL Adobe Workfront Fusion] Devtool可讓您瞭解並疑難排解案例。 Devtool將額外的面板新增至[!DNL Chrome Developer Tools]。 使用此偵錯工具面板，您可以檢查案例的所有手動執行、檢閱所有已執行的操作，並檢視每個已執行API呼叫的詳細資訊。 您可以檢視導致錯誤的模組、操作或單一回應，並運用該知識來調整您的案例。

>[!NOTE]
>
>在機密案例、自動執行和成功操作中，偵錯工具面板中的登入將會受到限制或無法使用。

如需Fusion Devtool的影片簡介和逐步解說，請參閱

* [Fusion開發工具](https://video.tv.adobe.com/v/3427031/){target=_blank}。
* [Devtool逐步說明](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/troubleshooting-and-error-handling/dev-tool-walkthrough.html?lang=en)

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront Fusion]授權**</td> 
  <td>
   <p>目前授權需求：無[!DNL Workfront Fusion]授權需求。</p>
   <p>或</p>
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]，[！UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]計畫，您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]計畫中。</p>
   <p>或</p>
   <p>舊版產品需求：您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 存取Workfront Fusion Devtool

存取Devtool會因您在[!DNL Adobe Unified Experience]中是否使用Fusion而有所不同。

* [存取 [!DNL Adobe Unified Experience]中的Devtool](#access-the-devtool-in-the-adobe-unified-experience)
* [存取傳統 [!DNL Fusion] 體驗中的Devtool](#access-the-devtool-in-the-classic-fusion-experience)

### 存取[!DNL Adobe Unified Experience]或新Fusion體驗中的Devtool

如果您在AdobeUnified Shell中使用Fusion，或已更新至新的Fusion體驗，則可以從案例編輯器存取開發工具。

1. 按一下靠近熒幕底部的&#x200B;**協助程式工具** ![協助程式工具](assets/debugger-icon.png)圖示。

或：

1. 前往您要偵錯之情境的「情境編輯器」。

   若要尋找Scenario編輯器，請參閱[Scenario編輯器](/help/quicksilver/workfront-fusion/scenarios/scenario-editor.md)。

1. 以滑鼠右鍵按一下頁面的空白區域（而不是模組）。
1. 選取&#x200B;**開啟Devtool**。

### 存取傳統[!DNL Fusion]體驗中的Devtool

若要在傳統[!DNL Fusion]體驗中使用Devtool，您必須安裝[!DNL Chrome]擴充功能。 然後您可以從[!DNL Chrome]開發人員工具使用此擴充功能。

* [安裝Install the [!DNL Chrome] Devtool擴充功能](#install-the-chrome-devtool-extension)
* [找到 [!DNL Workfront Fusion] Devtool](#locate-the-workfront-fusion-devtool)

#### 安裝[!DNL Chrome] Devtool擴充功能

您可以透過[!UICONTROL [!DNL Chrome]網站商店]，將[!DNL Workfront Fusion] Devtool新增至[!DNL Chrome]。

1. 按一下[此連結](https://chromewebstore.google.com/u/1/detail/workfront-fusion-devtool/hkimbmkkmmejdnhbhoaefggkpkndfjnn)以移至[!UICONTROL [!DNL Chrome]網站商店]上的[!DNL Workfront Fusion] Devtool。
1. 按一下「**[!UICONTROL 新增至[!DNL Chrome]]**」。
1. 在開啟的視窗中，檢查許可權。 如果您同意許可權，請按一下[新增擴充功能]。****

[!DNL Workfront Fusion] Devtool擴充功能已新增至您的[!DNL Chrome]擴充功能。


#### 找到[!DNL Workfront Fusion] Devtool

若要使用[!DNL Workfront Fusion] Devtool，您必須將[!DNL Workfront Fusion] Devtool擴充功能新增至[!DNL Chrome]瀏覽器，如[安裝Chrome Devtool擴充功能](#install-the-chrome-Devtool-extension)中所述。

1. 開啟您的[!DNL Workfront Fusion]案例。
1. 開啟[!DNL Chrome Developer Tools]：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!DNL Mac]</td> 
      <td>Command + Option + I</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Windows]</td> 
      <td> <p>Control + Shift + I</p> <p> 或 </p> <p>F12</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >我們建議將[!DNL Chrome Developer Console]固定於底部，以維持您模組的較佳檢視。

1. 按一下[!DNL Chrome Dev Tools]中的&#x200B;**[!DNL Workfront Fusion]**&#x200B;索引標籤。

## 使用[!DNL Workfront Fusion] Devtool

Workfront Fusion Devtool分為3個主要區段。 您可以在Devtool視窗的左側面板中找到這些專案。

* [即時資料流](#live-stream)
* [案例偵錯工具](#scenario-debugger)
* [工具](#tools)

### Live Stream

即時資料流會在您的情境中按一下「執行一次」時，顯示背景中發生的情形。

1. 按一下&#x200B;**[!UICONTROL 即時資料流]**&#x200B;圖示![](assets/live-stream-icon.png)以開啟即時資料流區段。
1. 執行下列任一項作業：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>動作</th> 
      <th>指示</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">檢視請求資訊</td> 
      <td> <p>您可以檢視情境中每個模組的下列資訊</p> 
       <ul> 
        <li> <p>請求標頭（API端點URL、http方法、呼叫請求的時間和日期、請求標頭以及查詢字串）</p> </li> 
        <li> <p>要求內文</p> </li> 
        <li> <p>回應標頭</p> </li> 
        <li> <p>回應內文</p> </li> 
       </ul> <p>若要檢視此資訊，請按一下[!DNL Workfront Fusion] Devtool右側面板中適當的索引標籤。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>搜尋請求和回應</p> </td> 
      <td> <p>在[!DNL Workfront Fusion] Devtool左側面板的搜尋欄位中輸入搜尋字詞，以僅顯示包含搜尋字詞的請求。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>移除請求清單 </p> </td> 
      <td> <p>按一下Devtool左面板右上角的垃圾桶圖示，以清除[!DNL Workfront Fusion] Devtool所記錄的請求清單。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>啟用主控台記錄</p> </td> 
      <td> <p>按一下Devtool左面板右上角的電腦圖示<img src="assets/console-computer-icon.png">。</p> <p>當電腦圖示為綠色時，會啟用登入主控台。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>以原始JSON格式或cURL擷取請求</p> </td> 
      <td> 
       <ul> 
        <li> <p><strong>原始JSON</strong> </p> <p>按一下Devtool右窗格右上角的<strong>[！UICONTROL Copy RAW]</strong>。</p> </li> 
        <li> <p><strong>cURL</strong> </p> <p>按一下Devtool右窗格右上角的<strong>[！UICONTROL Copy cURL]</strong>。</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

### 案例偵錯工具

情境偵錯工具適用於較複雜的情境。 它會顯示案例執行的歷史記錄，並可讓您依據模組名稱或ID來搜尋模組。

1. 按一下&#x200B;**[!UICONTROL 情境偵錯工具]**&#x200B;圖示![](assets/scenario-debugger-icon.png)以開啟情境偵錯工具。
1. （選擇性）在[!UICONTROL 情境偵錯工具]區段中[!DNL Workfront Fusion] Devtool的左窗格中的搜尋欄位中輸入搜尋字詞（名稱或模組ID）。
1. 連按兩下模組名稱，以在案例編輯器中開啟其設定。
1. 按一下所需的作業以檢視請求詳細資料。

### 工具

[!DNL Workfront Fusion] Devtool提供可讓您更輕鬆設定情境的工具。

1. 按一下&#x200B;**[!UICONTROL 工具]**&#x200B;圖示![](assets/console-tools-icon.png)以開啟工具。
1. 選取您要使用的工具
1. 設定欄位，如下所述。
1. 按一下&#x200B;**[!UICONTROL 執行]**。

工具及其欄位：

* [焦點模組](#focus-a-module)
* [依對應尋找模組](#find-modules-by-mapping)
* [取得應用程式中繼資料](#get-app-metadata)
* [複製對應](#copy-mapping)
* [複製篩選器](#copy-filter)
* [交換連線](#swap-connection)
* [交換變數](#swap-variable)
* [交換應用程式](#swap-app)
* [基底64](#base-64)
* [複製模組名稱](#copy-module-name)
* [重新對應Source](#remap-source)
* [反白顯示應用程式](#highlight-app)
* [移轉GS](#migrate-gs)

#### [!UICONTROL 焦點模組]

依照ID開啟指定模組的設定。

<table style="table-layout:auto">
    <tr>
        <td>[！UICONTROL模組ID]</td>
        <td>輸入您要開啟其設定的模組識別碼。</td>
    </tr>
</table>

#### [!UICONTROL 依對應尋找模組]

可讓您搜尋指定字詞的模組值。 輸出包含模組ID，其中包含您搜尋的字詞。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Keyword]</td> 
   <td> <p> 輸入您要搜尋的字詞。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL僅使用值]</p> </td> 
   <td> <p>啟用此選項以僅搜尋模組欄位的值。</p> <p>停用此選項亦可搜尋模組欄位的名稱。</p> <p>搜尋會透過名稱和標籤引數來執行。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得應用程式中繼資料]

依應用程式的模組名稱或ID擷取應用程式的中繼資料。 例如，在您需要知道情境中使用的應用程式版本時，這很有用。

<table style="table-layout:auto">
    <tr>
        <td>[！UICONTROL Source模組]</td>
        <td>選取您要擷取中繼資料的模組。</td>
    </tr>
</table>

#### [!UICONTROL 複製對應]

將值從來源模組複製到目標模組。

>[!CAUTION]
>
>請務必設定正確的來源和目標模組。 如果您選取不同型別的模組，則會刪除目標模組中的值。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Source模組]</td> 
   <td> <p> 選取模組或輸入您要從中複製欄位值的模組ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL目標模組]</p> </td> 
   <td> <p>選取模組或輸入您要插入來源模組值的模組ID。</p> <p>重要：目標模組中的值將被覆寫。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 複製篩選器]

將篩選設定從來源模組複製到目標模組。

>[!NOTE]
>
>複製動作會在所選模組左側的篩選器上執行。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Source模組]</td> 
   <td> <p> 選取模組或輸入您要從中複製篩選值的模組ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL目標模組]</p> </td> 
   <td> <p>選取模組或輸入要從來源模組插入篩選值之模組的ID。</p> <p>重要：目標模組中的值將被覆寫。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Preserve Fallback Route setting]</p> </td> 
   <td> <p>來源篩選器已設定為遞補路由。 啟用此選項也可以將目標篩選器設定為遞補路由。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 交換連線]

在同一個應用程式的案例中，將來源模組的連線複製到每個模組。

<table style="table-layout:auto">
    <tr>
        <td>[！UICONTROL Source模組]</td>
        <td>選取模組或輸入您要複製連線的模組ID。</td>
    </tr>
</table>

#### [!UICONTROL 交換變數]

搜尋情境中的指定變數，並以新變數取代。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL要尋找的變數]</td> 
   <td> <p> 從情境的模組中找出您要取代的變數藥丸，並將其複製到此（[！UICONTROL要尋找的變數]）欄位。 在欄位中，它會顯示為雙大括弧。 範例： <code>&#123;&#123;5.value&#125;&#125;</code>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL取代為]</p> </td> 
   <td> <p>從情境的模組中，找出您要取代變數的變數藥丸，並將其複製到此（[！UICONTROL要尋找的變數]）欄位。 在欄位中，它會顯示為雙大括弧。 範例： <code>&#123;&#123;5.value&#125;&#125;</code>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL模組]</p> </td> 
   <td> <p>選取您要取代變數的模組。 如果未選取任何模組，則變數會在整個案例中被取代。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 交換應用程式]

以其他應用程式版本取代您情境中選取的應用程式版本。

例如，這可用來將Gmail和電子郵件應用程式的模組升級至最新版本。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">要取代的[！UICONTROL應用程式]</td> 
   <td> <p> 選取您要取代的應用程式。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL取代為]</p> </td> 
   <td> <p>選取您要取代的應用程式。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 基底64]

可讓您將輸入的資料編碼為Base64或解碼Base64。 部分請求會編碼為Base64。 當您想要搜尋編碼請求中的特定資料時，此工具會很有用。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL操作] </td> 
   <td> <p>選取您要將資料從[！UICONTROL Raw Data]欄位編碼為Base64，還是要將Base64解碼為Raw Data。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL原始資料]</p> </td> 
   <td> <p> 根據上面[！UICONTROL Operation]欄位中選取的選項，輸入您要編碼為Base64的資料，或如果您要解碼為原始資料，則輸入Base64。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 複製模組名稱]

將所選模組的名稱複製到剪貼簿。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL模組] </td> 
   <td> <p>選取您要複製名稱的模組。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 重新對應Source]

可讓您將對應來源從一個模組變更為另一個模組。

您必須先將要作為來源模組的模組新增至情境中的路由。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Source模組] </td> 
   <td> <p> 選取您要取代的模組，作為情境中其他模組的對應來源。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL目標模組]</p> </td> 
   <td> <p>選取要作為新對應來源的模組。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL要編輯的模組]</p> </td> 
   <td> <p>如果您不想要變更整個案例中的對應，請選取您要變更其對應的模組。 </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 反白顯示應用程式]

反白顯示情境中指定應用程式的模組。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL要醒目提示的應用程式] </td> 
   <td> <p> 選取您要在情境中反白顯示的應用程式。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL版本] </p> </td> 
   <td> <p>選取要醒目提示的應用程式版本。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL反白顯示色彩]</p> </td> 
   <td> <p> 輸入要用於反白模組的顏色十六進位。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 移轉GS]

此工具的用途是將[!DNL Google Sheets] （舊版）模組升級至最新的[!DNL Google Sheets]版本。 在情境執行路徑中，新版本的模組會新增在舊版模組之後。

此模組不需要您設定任何引數。
