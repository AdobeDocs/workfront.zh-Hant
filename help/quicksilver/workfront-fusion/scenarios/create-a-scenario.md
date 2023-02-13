---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 在Adobe Workfront Fusion中建立案例
description: 下列工作說明如何建立 [!DNL Adobe Workfront Fusion] 藍本。
author: Becky
feature: Workfront Fusion
exl-id: adf66cfc-ccaf-4b29-9199-c13260695569
source-git-commit: fcaa2136310cad8ef478020a9bae34bbe5520c6d
workflow-type: tm+mt
source-wordcount: '1428'
ht-degree: 0%

---

# 在中建立案例 [!DNL Adobe Workfront Fusion]

下列工作說明如何建立 [!DNL Adobe Workfront Fusion] 藍本。

如需逐步引導您建立自動化案例的練習，請參閱 [在中建立實踐自動化案例 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-automation-scenario.md).

如需使用我們提供的資料逐步引導您建立整合案例的練習，請參閱 [在Adobe Workfront Fusion中建立實務整合案例](../../workfront-fusion/get-started/create-a-practice-scenario.md).

>[!NOTE]
>
>若要從範本建立案例，請參閱 [建立方案，使用 [!DNL Adobe Workfront Fusion] 範本](../../workfront-fusion/scenarios/templates/create-scenarios-with-fusion-templates.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p><p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化）</p><p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化）</p>    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 開始建立藍本

1. 按一下 **[!UICONTROL 藍本]** ![](assets/scenarios-icon.png) 中。

1. 按一下 **[!UICONTROL 建立新藍本]** 在頁面的右上角。
1. （選用）下方 **[!UICONTROL 您要整合哪些服務]**，如果您要建立新藍本，請選取您要在藍本中使用的應用程式，然後按一下 **[!UICONTROL 繼續]**.

   或

   按一下 **[!UICONTROL 略過]** 如果您想從案例編輯器中選擇應用程式。

1. 在顯示的畫面（情境編輯器）中，如果您要建立新情境，請按一下 **[!UICONTROL 新藍本]** 在左上角，輸入藍本的名稱。
1. 繼續 [在案例中新增模組](#add-a-module-in-a-scenario).

## 在案例中新增模組

1. 若要將第一個模組新增至案例，請按一下問號圖示。 ![](assets/question-mark-icon.gif)

   或

   若要新增其他模組至案例，請按一下您要其遵循之模組右側的控制代碼。

1. 在隨即顯示的方塊中，尋找並按一下您要開始的應用程式或服務。

   先前選取的任何應用程式都會顯示在方塊中，以方便存取，並會顯示在 **[!UICONTROL 我的最愛]** 區段。

   如果您按一下 **[!UICONTROL 新增其他模組]**，所顯示的模組取決於您新增模組的案例中的位置。 某些模組只能放在其他模組之間，而其他模組只能放在方案的開頭。

   >[!TIP]
   >
   >最常見的兩種模組類型是動作和觸發器。 如需詳細資訊，請參閱 [模組類型](../../workfront-fusion/modules/module-types.md).

1. 在顯示的模組清單中，按一下您要新增至案例的第一個模組。

   顯示的模組取決於您要在案例中新增模組的位置。 某些模組只能放在其他模組之間，而其他模組只能放在方案的開頭。

   最常見的兩種模組類型是動作和觸發器。 如需詳細資訊，請參閱 [模組類型](../../workfront-fusion/modules/module-types.md).

1. 繼續 [將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion]](#connect-the-modules-app-or-web-service-to-workfront-fusion).

## 將模組的應用程式或Web服務連接到 [!DNL Workfront Fusion] {#connect-the-modules-app-or-web-service-to-workfront-fusion}

Workfront Fusion模組，連線至應用程式(例如 [!DNL Workfront], [!DNL Salesforce]，或 [!DNL Jira)] 功能 [!UICONTROL 連線] 欄位。 您可以在此處指定要此模組用來連線至應用程式的連線。 您可以從下拉式清單中選取現有連線，或建立新連線。

當您在案例中選取或建立應用程式的連線時，該應用程式的其他模組會自動使用相同的連線，除非您在設定後續模組時選取不同的連線。

如需詳細資訊，請參閱 [關於連接 [!DNL Adobe Workfront Fusion] 至應用程式或服務](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

![](assets/connection-field-350x169.png)

在內建立連線的方式 [!DNL Workfront Fusion] 模組：

1. 按一下 **[!UICONTROL 新增]** 開啟 **[!UICONTROL 建立連線]** 框。
1. （選用）變更預設值 **[!UICONTROL 連線名稱]**.
1. （條件性）如果應用程式需要進階連線設定，例如ID、金鑰或 [!UICONTROL 秘密]，請輸入該資訊。

   您可能需要按一下 **[!UICONTROL 顯示高級設定]** 顯示可在其中輸入此類資訊的欄位。

1. 按一下 **[!UICONTROL 繼續]**.
1. 在顯示的登入視窗中，輸入您的憑證以登入應用程式（如果尚未登入）。
1. （條件性）若 **[!UICONTROL 允許]** 按鈕顯示，檢查連接器將能執行的動作，然後按一下按鈕將應用程式連線至 [!DNL Workfront Fusion].
1. 繼續 [設定模組](#configure-the-module).


## 設定模組

1. 在「連線」欄位下方的欄位中，設定模組的設定，然後按一下 **[!UICONTROL 確定]**.

   ![](assets/conf-settigs-mod-350x547.png)

   每個模組的這些設定都不同。 粗體標題表示必要的設定。

   >[!TIP]
   >
   >當您處理案例時，您隨時可以按一下模組以顯示此設定方塊。
   >
   >
   >如果您在模組上看到黑色圓圈，表示您尚未完成其設定。 按一下模組以開啟它並繼續設定。
   >
   >
   >![](assets/black-error-circle-on-module.png)

1. 如果您要在案例中新增第一個模組，請選取選項，以指出您希望每次執行案例時啟動的位置。

   ![](assets/choose-where-start-350x194.png)

1. 重複各節中的步驟 [在案例中新增模組](#add-a-module-in-a-scenario) 和 [設定模組](#configure-the-module) 將其他模組添加到方案。

1. （可選）複製並貼上模組或模組群組。

   如需詳細資訊，請參閱 [複製Adobe Workfront Fusion中的模組或案例](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md).

1. 繼續 [設定並搭配您的藍本使用](#configure-and-work-with-your-scenario).

## 設定並搭配您的藍本使用

1. 執行下列任一操作來設定您的案例：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">指定執行情境的時間和頻率</td> 
      <td> <p>按一下時鐘錶徵圖。 </p> <p> <img src="assets/clock-icon.gif"> </p> <p>如需詳細資訊，請參閱 <a href="../../workfront-fusion/scenarios/schedule-a-scenario.md" class="MCXref xref">在中排程藍本 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">設定路由</td> 
      <td> <p>按一下扳手圖示 <img src="assets/wrench-icon.gif"> 並使用下列任一選項。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">將篩選器新增至案例，於 [!DNL Adobe Workfront Fusion]</a>.</p> 
       <ul> 
        <li><strong>[!UICONTROL設定篩選器]</strong>:控制在場景中的特定點使用的套件組合。</li> 
        <li><strong>[!UICONTROL取消連結]</strong>:刪除路由。</li> 
        <li><strong>[!UICONTROL添加路由器]</strong>:在模組之間添加路由器。 </li> 
        <li><strong>[!UICONTROL添加模組]</strong>:在模組之間新增模組。</li> 
        <li><strong>[!UICONTROL添加註釋]</strong>:將注釋添加到路由。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">配置方案設定</td> 
      <td>按一下[!UICONTROL方案設定]表徵圖。 <img src="assets/gear-icon-settings.png"> 這些設定主要針對進階使用者。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">中的藍本設定面板 [!DNL Adobe Workfront Fusion]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">配置流量控制設定</td> 
      <td> <p>按一下[!UICONTROL流量控制]表徵圖。 <img src="assets/flow-control-icon.gif"> 您可以設定任務來重複指定次數、將陣列轉換為一系列捆綁包，然後將多個捆綁包合併為一個捆綁包。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/apps-and-their-modules/flow-control.md" class="MCXref xref">中的流量控制 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">使用進階工具增強案例</td> 
      <td>按一下 [!DNL Tools] 表徵圖。 <img src="assets/tools-icon.gif"> 您可以建立觸發器、動作、匯總器和變壓器。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">工具</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">用戶文本解析工具</td> 
      <td>按一下 [!DNL Text parser] 圖示 <img src="assets/text-parser-icon.gif">. 您可以從HTML程式碼中擷取元素、尋找及擷取符合搜尋模式的字串元素、搜尋及取代文字，以及從網站中「消除」資料。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">工具</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. 執行下列任一操作以搭配您的案例：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">檢視案例執行時發生的事件記錄</td> 
      <td> <p>按一下[!UICONTROL退出編輯]箭頭 <img src="assets/exit-editing-arrow.png"> 在方案編輯器中，以檢視「方案詳細資料」頁面。 日誌顯示在窗口底部或右下角。 它包含每個階段的相關資訊，以及在執行案例期間遇到的任何錯誤。</p> <p>若要在 [!DNL scenario editor]，按一下「藍本詳細資訊」頁面上的任意位置。</p> <p>如需藍本詳細資訊頁面的詳細資訊，請參閱 <a href="../../workfront-fusion/scenarios/scenario-detail.md" class="MCXref xref">中的方案詳細資料 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">存取您最常使用的應用程式和服務</td> 
      <td> 按一下 <strong>[!UICONTROL收藏夾]</strong> 區段。 當您將應用程式和服務新增至案例時，圖示會自動顯示在此區段中。 您也可以按一下[!UICONTROL新增]圖示 <img src="assets/add-icon.gif"> 手動將應用程式和服務新增至此區域的方式。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">檢視動畫，顯示資料如何在情境中流動</td> 
      <td>按一下[!UICONTROL說明流]表徵圖 <img src="assets/explain-flow-airplane-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">自動對齊模組的佈局 </td> 
      <td>按一下[!UICONTROL自動對齊]圖示 <img src="assets/auto-align-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">輸入或檢視藍本的相關附註</td> 
      <td>按一下[!UICONTROL Notes]表徵圖 <img src="assets/notes-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">移除模組</td> 
      <td>以滑鼠右鍵按一下模組，然後按一下 <strong>[!UICONTROL刪除模組]</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. 若要測試執行案例，請按一下 **[!UICONTROL 執行一次]**.

   在啟動情境之前，請務必確認情境是否如預期般執行。 啟動後，情境將根據其排程執行。 如果一切都未如預期般執行，請參閱 [錯誤處理 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md).

1. 當您完成對藍本的編輯時（或在您編輯時的任何時間），按一下 [!UICONTROL 儲存] 表徵圖 ![](assets/save-icon.gif).

如需啟動案例的相關資訊，請參閱 [在中啟用或停用案例 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

## Workfront Fusion方案鍵盤快速鍵

建立或編輯藍本時，可以使用以下鍵盤快速鍵：

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <thead> 
  <tr> 
   <th> <p>動作</p> </th> 
   <th>[!DNL Windows]</th> 
   <th> <p>[!DNL MacOS]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL保存] </td> 
   <td>Ctrl+Shift+S</td> 
   <td><span style="font-weight: normal;">Cmd+Shift+S</span> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL運行一次]</td> 
   <td>Ctrl+Shift+Enter</td> 
   <td><span style="font-weight: normal;">Cmd+Shift+Enter</span> </td> 
  </tr> 
 </tbody> 
</table>
