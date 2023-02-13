---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion DevTool的除錯案例
description: Adobe Workfront Fusion DevTool可讓您了解並疑難排解案例。 DevTool會在Chrome開發人員工具中新增額外的面板。 使用此除錯工具面板，您可以檢查案例的所有手動執行、檢閱所有執行的操作，並查看每個執行之API呼叫的詳細資訊。 您可以查看哪個模組、操作或單一回應造成錯誤，並使用該知識來調整您的情境。
author: Becky
feature: Workfront Fusion
exl-id: f7557214-3615-4797-b4cb-4af70e4797ac
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1665'
ht-degree: 0%

---

# 使用 [!DNL Adobe Workfront Fusion] DevTool

此 [!DNL Adobe Workfront Fusion] DevTool可讓您了解並疑難排解案例。 DevTool會在 [!DNL Chrome Developer Tools]. 使用此除錯工具面板，您可以檢查案例的所有手動執行、檢閱所有執行的操作，並查看每個執行之API呼叫的詳細資訊。 您可以查看哪個模組、操作或單一回應造成錯誤，並使用該知識來調整您的情境。

## 存取需求

您必須具備下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[!UICONTROL計畫]、[!UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]授權**</td> 
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p><p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化） </p>  </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 安裝 [!DNL Chrome] DevTool擴充功能

若要使用 [!DNL Workfront Fusion] DevTool，您必須先安裝它。

1. 按一下 [此連結](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/workfront-fusion-devtool.zip) 下載擴充功能。
1. 下載檔案後，將它們解壓縮至您所選擇的資料夾。
1. 在 [!DNL Chrome]
1. 在索引標籤的搜尋列中，輸入 `chrome://extensions`.
1. 按一下 **[!UICONTROL 開發人員模式]** 在畫面右上方切換，以啟用開發人員模式。 如果切換至右側，則會啟用開發人員模式。
1. 按一下 **[!UICONTROL 載入未打包]**.
1. 選取包含DevTool的資料夾（在步驟2中擷取檔案）。

   解壓縮後，DevTool就會出現在您其他Chrome擴充功能中。

## 找出 [!DNL Workfront Fusion] DevTool

若要使用 [!DNL Workfront Fusion] DevTool，您必須新增 [!DNL Workfront Fusion] DevTool擴充功能 [!DNL Chrome] 瀏覽器，如 [安裝Chrome DevTool擴充功能](#install-the-chrome-devtool-extension).

1. 開啟 [!DNL Workfront Fusion] 藍本。
1. 開啟 [!DNL Chrome Developer Tools]:

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
      <td> <p>Ctrl + Shift + I</p> <p> 或 </p> <p>F12</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >建議將 [!DNL Chrome Developer Console] 向下顯示，以便更好地查看模組。

1. 按一下 **[!DNL Workfront Fusion]** 標籤 [!DNL Chrome Dev Tools].

## 使用 [!DNL Workfront Fusion] DevTool

Workfront Fusion DevTool分為3個主要部分。 您可以在DevTool窗口的左側面板中找到這些。

* [即時資料流](#live-stream)
* [藍本偵錯器](#scenario-debugger)
* [工具](#tools)

### 即時資料流

當您在案例中按一下「執行一次」時，「即時資料流」會顯示背景發生的情況。

1. 按一下 **[!UICONTROL 即時資料流]** 圖示 ![](assets/live-stream-icon.png) 來開啟「即時資料流」區段。
1. 執行下列任一操作：

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
      <td> <p>您可以檢視案例中每個模組的下列資訊</p> 
       <ul> 
        <li> <p>請求標題（API端點URL、http方法、呼叫請求的時間和日期、請求標題及查詢字串）</p> </li> 
        <li> <p>要求內文</p> </li> 
        <li> <p>回應標題</p> </li> 
        <li> <p>回應內文</p> </li> 
       </ul> <p>若要檢視此資訊，請按一下 [!DNL Workfront Fusion] 開發工具。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>搜尋請求和回應</p> </td> 
      <td> <p>在左側面板的搜尋欄位中輸入搜尋詞 [!DNL Workfront Fusion] DevTool，只顯示包含搜尋詞的請求。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>移除請求清單 </p> </td> 
      <td> <p>按一下DevTool左側面板右上角的垃圾桶圖示，以清除 [!DNL Workfront Fusion] 開發工具。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>啟用主控台記錄</p> </td> 
      <td> <p>按一下電腦表徵圖 <img src="assets/console-computer-icon.png"> 位於DevTool左面板的右上角。</p> <p>電腦圖示為綠色時，主控台中的記錄功能便會啟用。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>以原始JSON格式或cURL擷取要求</p> </td> 
      <td> 
       <ul> 
        <li> <p><strong>原始JSON</strong> </p> <p>按一下 <strong>[!UICONTROL複製原始]</strong> 在DevTool右窗格的右上角。</p> </li> 
        <li> <p><strong>cURL</strong> </p> <p>按一下 <strong>[!UICONTROL複製cURL]</strong> 在DevTool右窗格的右上角。</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

### 藍本偵錯器

情節除錯工具對更複雜的情境很實用。 它會顯示案例執行的歷史記錄，並可讓您依模組名稱或ID來搜尋模組。

1. 按一下 **[!UICONTROL 藍本偵錯器]** 圖示 ![](assets/scenario-debugger-icon.png) 以開啟藍本偵錯器。
1. （可選）在左窗格的搜尋欄位中輸入搜尋詞（名稱或模組ID） [!DNL Workfront Fusion] 中的DevTool [!UICONTROL 藍本偵錯器] 區段。
1. 連按兩下模組的名稱，以在案例編輯器中開啟其設定。
1. 按一下所需的操作即可檢視請求詳細資訊。

### 工具

此 [!DNL Workfront Fusion] DevTool提供工具，讓您更輕鬆設定案例。

1. 按一下 **[!UICONTROL 工具]** 圖示 ![](assets/console-tools-icon.png) 來開啟「工具」。
1. 選取您要使用的工具
1. 設定欄位，如下所述。
1. 按一下 **[!UICONTROL 執行]**.

工具及其欄位：

* [聚焦模組](#focus-a-module)
* [通過映射查找模組](#find-modules-by-mapping)
* [取得應用程式中繼資料](#get-app-metadata)
* [複製對應](#copy-mapping)
* [複製篩選器](#copy-filter)
* [交換連接](#swap-connection)
* [交換變數](#swap-variable)
* [交換應用程式](#swap-app)
* [基64](#base-64)
* [複製模組名稱](#copy-module-name)
* [重新映射源](#remap-source)
* [突出顯示應用](#highlight-app)
* [遷移GS](#migrate-gs)

#### [!UICONTROL 聚焦模組]

按ID開啟指定模組的設定。

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL模組ID]</td>
        <td>輸入要開啟設定的模組ID。</td>
    </tr>
</table>

#### [!UICONTROL 通過映射查找模組]

可讓您搜尋指定詞語的模組值。 輸出包含模組ID，這些模組包含您搜索的詞。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL關鍵字]</td> 
   <td> <p> 輸入要搜索的詞。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL僅使用值]</p> </td> 
   <td> <p>啟用此選項，僅在模組欄位的值中搜索。</p> <p>停用此選項也可在模組欄位的名稱中搜尋。</p> <p>搜尋會透過名稱和標籤參數執行。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 取得應用程式中繼資料]

依應用程式的模組名稱或ID擷取應用程式的中繼資料。 例如，當您需要知道案例中使用的應用程式版本時，這個功能就很實用。

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL源模組]</td>
        <td>選取您要擷取中繼資料的模組。</td>
    </tr>
</table>

#### [!UICONTROL 複製對應]

將值從源模組複製到目標模組。

>[!CAUTION]
>
>請務必設定正確的來源和目標模組。 如果您選取不同的模組類型，則目標模組中的值將會刪除。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL源模組]</td> 
   <td> <p> 選取模組，或輸入要從中複製欄位值的模組ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Target模組]</p> </td> 
   <td> <p>選擇要插入源模組值的模組或輸入模組的ID。</p> <p>重要：目標模組中的值將被覆寫。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 複製篩選器]

將篩選器設定從源模組複製到目標模組。

>[!NOTE]
>
>複製動作會對置於所選模組左側的篩選器執行。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL源模組]</td> 
   <td> <p> 選取模組，或輸入要從中複製篩選值的模組ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Target模組]</p> </td> 
   <td> <p>選擇模組或輸入要從源模組插入篩選值的模組的ID。</p> <p>重要：目標模組中的值將被覆寫。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL保留回退路由設定]</p> </td> 
   <td> <p>源篩選器設定為後援路由。 啟用此選項也可將目標篩選器設定為後援路由。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 交換連接]

在同一應用程式的案例中，將來源模組與每個模組的連線重複。

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL源模組]</td>
        <td>選取模組或輸入要複製連線的模組ID。</td>
    </tr>
</table>

#### [!UICONTROL 交換變數]

在案例中搜尋指定的變數，並以新變數取代。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！要查找的變數]</td> 
   <td> <p> 在案例中，找出您要從模組取代的變數藥丸，並將其複製到此（[!UICONTROL要尋找的變數]）欄位。 在欄位中，會以雙大括弧顯示。 範例: <code>&#123;&#123;5.value&#125;&#125;</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL替換為]</p> </td> 
   <td> <p>在您的案例中，從模組找出您要將變數取代為的變數小丸，並複製到此（[!UICONTROL要尋找的變數]）欄位。 在欄位中，會以雙大括弧顯示。 範例: <code>&#123;&#123;5.value&#125;&#125;</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL模組]</p> </td> 
   <td> <p>選取要取代變數的模組。 如果未選取任何模組，則整個案例中會取代變數。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 交換應用程式]

以其他應用程式版本取代您案例中選取的應用程式版本。

例如，您可以將Gmail和電子郵件應用程式的模組升級至最新版本。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！要替換的UICONTROL應用]</td> 
   <td> <p> 選取您要取代的應用程式。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL替換為]</p> </td> 
   <td> <p>選取您要取代為的應用程式。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 基64]

允許將輸入的資料編碼為Base64或將Base64解碼。 有些要求會編碼為Base64。 當您想在編碼請求中搜尋特定資料時，此工具會很實用。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL操作] </td> 
   <td> <p>選擇要將[!UICONTROL原始資料]欄位中的資料編碼為Base64，還是將Base64解碼為原始資料。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL原始資料]</p> </td> 
   <td> <p> 根據上面[!UICONTROL操作]欄位中選擇的選項，輸入要編碼為Base64或Base64的資料（如果要解碼為原始資料）。</p> </td> 
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
   <td role="rowheader">[!UICONTROL模組] </td> 
   <td> <p>選取您要複製的模組名稱。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 重新映射源]

可讓您將對應來源從一個模組變更為另一個模組。

您必須先將要用作源模組的模組添加到方案中的路由。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL源模組] </td> 
   <td> <p> 選擇要替換的模組作為方案中其他模組的映射源。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Target模組]</p> </td> 
   <td> <p>選擇要用作新映射源的模組。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！要編輯的UICONTROL模組]</p> </td> 
   <td> <p>如果您不想在整個案例中變更對應，請選取您要變更對應的模組。 </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 突出顯示應用]

在您的案例中，反白顯示指定應用程式的模組。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！要突出顯示的UICONTROL應用] </td> 
   <td> <p> 選取您要在案例中醒目提示的應用程式。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL版本] </p> </td> 
   <td> <p>選取您要反白顯示的應用程式版本。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL突出顯示顏色]</p> </td> 
   <td> <p> 輸入要用於突出顯示模組的顏色十六進位。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 遷移GS]

此工具的製作目的是為了升級 [!DNL Google Sheets] （舊版）模組至最新 [!DNL Google Sheets] 版本。 它會在案例路由中模組的舊版本後面添加新版本的模組。

此模組不要求您設定任何參數。
