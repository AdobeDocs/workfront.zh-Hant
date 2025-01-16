---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 在Adobe Workfront Fusion中建立情境
description: Adobe Workfront Fusion檔案已移至新位置。 本文已棄用，但包含新文章的連結，內容涵蓋此功能。
author: Becky
feature: Workfront Fusion
exl-id: adf66cfc-ccaf-4b29-9199-c13260695569
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1473'
ht-degree: 0%

---

# 在[!DNL Adobe Workfront Fusion]中建立情境

>[!IMPORTANT]
>
>Adobe Workfront Fusion檔案已移至新位置。
>
>本文資訊可在以下文章中找到：
>
>* [建立情境的工作流程](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/plan-a-scenario/create-a-scenario-workflow.html)
>
>請更新任何書籤。
>
>本文已不再更新，將於不久將來移除。

下列工作說明如何建立[!DNL Adobe Workfront Fusion]情境。

如需逐步說明如何建立自動化案例的練習練習，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-automation-scenario.md)中建立練習自動化案例。

若要進行練習練習，以逐步引導您使用我們提供的資料建立整合案例，請參閱[在Adobe Workfront Fusion中建立練習整合案例](../../workfront-fusion/get-started/create-a-practice-scenario.md)。

>[!NOTE]
>
>若要從範本建立案例，請參閱[使用 [!DNL Adobe Workfront Fusion] 範本建立案例](../../workfront-fusion/scenarios/templates/create-scenarios-with-fusion-templates.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto"> 
  <tbody>  
    <tr>  
      <td>Adobe Workfront計畫</td>  
      <td>任何</td>  
    </tr>  
    <tr>  
      <td>Adobe Workfront授權</td>  
      <td>
        新增： Standard<br>
        或<br>
        目前：工作或以上
      </td>  
    </tr>  
    <tr>  
      <td>Adobe Workfront Fusion授權</td>  
      <td> 
        目前：無Workfront Fusion授權需求。<br>
        或<br>
        舊版：任何
      </td>  
    </tr>  
    <tr>  
      <td>產品</td>  
      <td> 
        新增：選取或Prime Workfront計畫：您的組織必須購買Adobe Workfront Fusion。<br>
        Ultimate Workfront計畫：包含Workfront Fusion。<br>
        或<br>
        目前：您的組織必須購買Adobe Workfront Fusion。
      </td>  
    </tr> 
  </tbody>  
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

+++

## 開始建立情境

1. 按一下左側面板中的&#x200B;**[!UICONTROL 情境]** ![](assets/scenarios-icon.png)。

1. 按一下頁面右上角的&#x200B;**[!UICONTROL 建立新案例]**。
1. 在出現的畫面（情境編輯器）中，如果您要建立新情境，請按一下左上角的&#x200B;**[!UICONTROL 新情境]**，然後輸入情境的名稱。
1. 繼續以[在情境](#add-a-module-in-a-scenario)中新增模組。

## 在情境中新增模組

1. 若要將第一個模組新增至情境，請按一下問號圖示。![](assets/question-mark-icon.gif)

   或

   若要將其他模組新增至情境，請按一下您希望其追蹤模組右側的控點。

1. 在顯示的方塊中，尋找並按一下您要開始使用的應用程式或服務。

   任何先前選取的應用程式都會顯示在方塊中，以方便存取，並顯示在畫面底部的&#x200B;**[!UICONTROL 我的最愛]**&#x200B;區段中。

   如果您按一下&#x200B;**[!UICONTROL 新增另一個模組]**，顯示的模組會根據您新增模組的情境中的位置而定。 有些模組只能放在其他模組之間，有些模組則只能放在情境的開頭處。

   >[!TIP]
   >
   >最常見的兩種模組型別為動作和觸發器。 如需詳細資訊，請參閱[模組型別](../../workfront-fusion/modules/module-types.md)。

1. 在顯示的模組清單中，按一下您要新增至情境的第一個模組。

   顯示的模組取決於您要在情境中新增模組的位置。 有些模組只能放在其他模組之間，有些模組則只能放在情境的開頭處。

   最常見的兩種模組型別為動作和觸發器。 如需詳細資訊，請參閱[模組型別](../../workfront-fusion/modules/module-types.md)。

1. 繼續到[將模組的App或Web服務連線到 [!DNL Workfront Fusion]](#connect-the-modules-app-or-web-service-to-workfront-fusion)。

## 將模組的App或Web服務連線至[!DNL Workfront Fusion] {#connect-the-modules-app-or-web-service-to-workfront-fusion}

連線到應用程式的Workfront Fusion模組（例如[!DNL Workfront]、[!DNL Salesforce]或[!DNL Jira)]）具有[!UICONTROL 連線]欄位。 您可以在此處指定此模組要用來連線至應用程式的連線。 您可以從下拉式選單中選取現有連線，或建立新連線。

當您為某個案例中的應用程式選取或建立連線時，除非您在設定較新的模組時選取不同的連線，否則該應用程式的其他模組會自動使用相同的連線。

如需詳細資訊，請參閱[連線總覽](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md)。

![](assets/connection-field-350x169.png)

若要在[!DNL Workfront Fusion]模組內建立連線：

1. 按一下&#x200B;**[!UICONTROL [新增]]**&#x200B;以開啟&#x200B;**[!UICONTROL [建立連線]]**&#x200B;方塊。
1. （選擇性）變更預設的&#x200B;**[!UICONTROL 連線名稱]**。
1. （條件式）如果應用程式需要進階連線設定（例如ID、金鑰或[!UICONTROL 密碼]），請輸入該資訊。

   您可能需要按一下「顯示進階設定」****&#x200B;來顯示可輸入這類資訊的欄位。

1. 按一下&#x200B;**[!UICONTROL 繼續]**。
1. 在顯示的登入視窗中，輸入您的認證以登入應用程式（如果尚未這麼做）。
1. （條件式）如果顯示&#x200B;**[!UICONTROL 允許]**&#x200B;按鈕，請檢查聯結器能夠採取的動作，然後按一下按鈕以將應用程式連線到[!DNL Workfront Fusion]。
1. 繼續進行[設定模組](#configure-the-module)。


## 設定模組

1. 在[連線]欄位下方的欄位中，設定模組的設定，然後按一下[確定]。****

   ![](assets/conf-settigs-mod-350x547.png)

   這些設定對每個模組都不同。 粗體標題表示必要的設定。

   >[!TIP]
   >
   >當您處理情境時，可以隨時按一下模組以顯示此設定方塊。
   >
   >
   >如果您在模組中看到黑色圓圈，表示您尚未完成其設定。 按一下模組以開啟並繼續設定。
   >
   >
   >![](assets/black-error-circle-on-module.png)

1. 如果您在情境中新增第一個模組，請選取一個選項，以指出每次執行情境時，希望情境從何處開始。

   ![](assets/choose-where-start-350x194.png)

1. 重複區段[在情境中新增模組](#add-a-module-in-a-scenario)和[設定模組](#configure-the-module)以新增其他模組至情境中的步驟。

1. （選用）複製並貼上模組或模組群組。

   如需詳細資訊，請參閱[在Adobe Workfront Fusion中複製模組或案例](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md)。

1. 繼續進行[設定並處理您的情境](#configure-and-work-with-your-scenario)。

## 設定並搭配您的情境

1. 執行下列任一項作業來設定您的情境：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">指定案例執行的時間和頻率</td> 
      <td> <p>按一下時鐘圖示。 </p> <p> <img src="assets/clock-icon.gif"> </p> <p>如需詳細資訊，請參閱<a href="../../workfront-fusion/scenarios/schedule-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中排程情境。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">設定路由</td> 
      <td> <p>按一下兩個模組之間的扳手圖示<img src="assets/wrench-icon.gif">，並使用下列任一選項。 如需詳細資訊，請參閱<a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中將篩選器新增到情境。</p> 
       <ul> 
        <li><strong>[！UICONTROL設定篩選器]</strong>：控制案例中某些點使用哪些組合。</li> 
        <li><strong>[！UICONTROL Unlink]</strong>：移除路由。</li> 
        <li><strong>[！UICONTROL新增路由器]</strong>：在模組之間新增路由器。 </li> 
        <li><strong>[！UICONTROL新增模組]</strong>：在模組之間新增模組。</li> 
        <li><strong>[！UICONTROL新增備註]</strong>：新增備註至路由。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">設定情境設定</td> 
      <td>按一下[！UICONTROL案例設定]圖示。 <img src="assets/gear-icon-settings.png">這些設定主要是供進階使用者使用。 如需詳細資訊，請參閱[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">情境設定面板。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">設定流量控制設定</td> 
      <td> <p>按一下[！UICONTROL流量控制]圖示。 <img src="assets/flow-control-icon.gif">您可以設定任務重複指定次數、將陣列轉換為一系列組合，以及將多個組合合併為單一組合。 如需詳細資訊，請參閱[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/apps-and-their-modules/flow-control.md" class="MCXref xref">流量控制。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">使用進階工具增強情境</td> 
      <td>按一下[!DNL Tools]圖示。 <img src="assets/tools-icon.gif">您可以建立觸發程式、動作、彙總器和轉換器。 如需詳細資訊，請參閱<a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">工具</a>。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">使用者文字剖析工具</td> 
      <td>按一下[!DNL Text parser]圖示<img src="assets/text-parser-icon.gif">。 您可以從HTML程式碼擷取元素、尋找及擷取符合搜尋模式的字串元素、搜尋及取代文字，以及從網站「刮取」資料。 如需詳細資訊，請參閱<a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">工具</a>。</td> 
     </tr> 
    </tbody> 
   </table>

1. 執行下列任一項作業以搭配您的情境使用：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">檢視案例執行時發生的事件記錄</td> 
      <td> <p>按一下案例編輯器中的[！UICONTROL Exit editing]箭頭<img src="assets/exit-editing-arrow.png">以檢視「案例」詳細資料頁面。 記錄會顯示在視窗底部或右下角。 它包含有關每個階段的資訊，以及在執行案例期間遇到的任何錯誤。</p> <p>若要在[!DNL scenario editor]中返回使用您的案例，請按一下[案例]詳細資訊頁面上的任何位置。</p> <p>如需「案例詳細資料」頁面的詳細資訊，請參閱[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/scenarios/scenario-detail.md" class="MCXref xref">案例詳細資料。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">存取您最常用的應用程式和服務</td> 
      <td> 按一下畫面底部<strong>[！UICONTROL我的最愛]</strong>區段中的圖示。 當您將應用程式和服務新增到您的情境時，圖示會自動顯示在此區段中。 您也可以按一下[！UICONTROL新增]圖示<img src="assets/add-icon.gif">，手動將應用程式和服務新增至此區域。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">檢視顯示資料如何流經情境的動畫</td> 
      <td>按一下[！UICONTROL說明流程]圖示<img src="assets/explain-flow-airplane-icon.gif">。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">自動對齊模組版面 </td> 
      <td>按一下[！UICONTROL自動對齊]圖示<img src="assets/auto-align-icon.gif">。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">輸入或檢視情境的相關附註</td> 
      <td>按一下[！UICONTROL附註]圖示<img src="assets/notes-icon.gif">。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">移除模組</td> 
      <td>以滑鼠右鍵按一下模組，然後按一下<strong>[！UICONTROL刪除模組]</strong>。</td> 
     </tr> 
    </tbody> 
   </table>

1. 若要測試執行情境，請按一下[執行一次]。****

   啟用前，請務必確認情境能如預期般執行。 一旦啟用，情境將會根據其排程執行。 如果一切未如預期般執行，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md)中的[錯誤處理。

1. 當您完成案例的編輯後（或在編輯期間），請按一下視窗![](assets/save-icon.gif)底部的[!UICONTROL 儲存]圖示。

如需啟動情境的相關資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md)中啟動或停用情境。

## Workfront Fusion案例鍵盤快速鍵

建立或編輯案例時，您可以使用下列鍵盤快速鍵：

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
   <td role="rowheader">[！UICONTROL儲存] </td> 
   <td>Ctrl+Shift+S</td> 
   <td><span style="font-weight: normal;">Cmd+Shift+S</span> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL執行一次]</td> 
   <td>Ctrl+Shift+Enter</td> 
   <td><span style="font-weight: normal;">Cmd+Shift+Enter</span> </td> 
  </tr> 
 </tbody> 
</table>
