---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: ' [!DNL Adobe] Workfront Fusion中的情境編輯器'
description: 情境編輯器可讓您在視覺介面中建立和編輯情境。
author: Becky
feature: Workfront Fusion
exl-id: 4377303d-7615-41eb-b0cc-4bf884899361
source-git-commit: cb4edb02aad8a0738ea80f058fcc2bc016832ce1
workflow-type: tm+mt
source-wordcount: '1108'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]中的案例編輯器

情境編輯器可讓您在視覺介面中建立和編輯情境。

![](assets/scenario-editor.jpg)

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
   <p>舊版授權需求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
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

## 開啟案例編輯器：

1. 按一下左側面板中的&#x200B;**[!UICONTROL 情境]** ![](assets/scenarios-icon.png)。

1. 如果要建立情境，請按一下頁面右上角的&#x200B;**[!UICONTROL 建立新情境]**。

   或

   如果要編輯現有情境，請按一下情境。

   在顯示的案例編輯器中，您可以執行下表所列的所有操作。 如需詳細資訊，請參閱[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md)中建立情境。

1. 當您完成編輯情境時（或在編輯的任何時候），請按一下[!UICONTROL 儲存]圖示。![](assets/save-icon.gif)

   >[!NOTE]
   >
   >儲存您的情境後，三點選單底下將顯示新版本，以備您日後需要存取時使用。 先前儲存的案例版本僅可使用60天。

## 可用的案例編輯器動作

「情境編輯器」中有以下動作：

<table style="table-layout:auto"> 
<tbody>
  <tr>
     <td role="rowheader">新增第一個模組</td>
     <td> <p>按一下問號圖示。 <img src="assets/question-mark-full-size.png"></p> <p> 然後尋找並按一下您要開始使用的應用程式或服務。 如果您在步驟2中選取任何應用程式，它們會出現在此處以方便存取（以及畫面底部的<strong>[！UICONTROL我的最愛]</strong>區段）。</p> </td>
  </tr>
  <tr>
     <td role="rowheader">新增模組</td>
     <td>將游標暫留在模組上，按一下右側的加號圖示，然後在出現的功能表中按一下您想要的模組。</td>
  </tr>  
  <tr>   
     <td role="rowheader">指定案例執行的時間和頻率</td>  
      <td> <p>按一下時鐘圖示。 </p> <p> <img src="assets/clock-icon.gif"> </p> <p>如需詳細資訊，請參閱<a href="../../workfront-fusion/scenarios/schedule-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中排程情境。</p> </td>
  </tr>  
  <tr>
     <td role="rowheader">設定路由</td>   
     <td> <p>按一下兩個模組之間的[！UICONTROL扳手]圖示<img src="assets/wrench-icon.gif">，並使用下列任一選項：</p>    
       <ul>
         <li><strong>[！UICONTROL設定篩選器]</strong>：控制案例中某些點使用哪些組合。 如需詳細資訊，請參閱<a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中將篩選器新增到情境。</li>     
         <li><strong>[！UICONTROL Unlink]</strong>：移除路由。</li>     
         <li><strong>[！UICONTROL新增路由器]</strong>：在模組之間新增路由器。 </li>     
         <li><strong>[！UICONTROL新增模組]</strong>：在模組之間新增模組。</li>     
         <li><strong>[！UICONTROL新增備註]</strong>：新增備註至路由。</li>   
       </ul> 
     </td>  
  </tr>  
  <tr>  
     <td role="rowheader">移除模組</td>   
     <td>以滑鼠右鍵按一下模組，然後按一下<strong>[！UICONTROL刪除模組]</strong>。</td>  
   </tr>  
   <tr> 
     <td role="rowheader">檢視發生事件的紀錄是情境</td>     
     <td> 
       <p>執行案例。 當案例完成執行時，記錄會顯示在[！UICONTROL案例編輯器]的右下角。 </p> <p> <img src="assets/log-350x189.png" style="width: 350;height: 189;"> </p> <p>根據情境的不同，記錄可以包含有關每個階段的難度的資訊，以及在執行情境期間遇到的任何錯誤。</p> 
     </td>  
   </tr>  
   <tr>   
     <td role="rowheader">設定情境設定</td>   
     <td>按一下[！UICONTROL案例設定]圖示。 <img src="assets/gear-icon-settings.png">這些設定主要是供進階使用者使用。</td>  
   </tr>  
   <tr>   
     <td role="rowheader">輸入或檢視情境的相關附註</td>   
     <td>按一下[！UICONTROL附註]圖示。 <img src="assets/notes-icon.gif"></td>  
   </tr>  
   <tr> 
     <td role="rowheader">自動對齊模組版面 </td>   
     <td>按一下[！UICONTROL自動對齊]圖示。 <img src="assets/auto-align-icon.gif"></td>  </tr>  <tr>   <td role="rowheader">檢視顯示資料如何流經情境的動畫</td>   <td>按一下[！UICONTROL說明流程]圖示。 <img src="assets/explain-flow-airplane-icon.gif"></td>  
   </tr>  
   <tr> 
     <td role="rowheader">將情境匯出至您的電腦做為Blueprint</td>   
     <td>按一下[！UICONTROL更多]功能表<img src="assets/more-icon.png">，然後按一下[！UICONTROL匯出Blueprint]。</td>  
   </tr>  
   <tr>   
     <td role="rowheader">從您的電腦匯入情境藍圖</td>   
     <td>按一下[！UICONTROL更多]功能表<img src="assets/more-icon.png">，然後按一下[！UICONTROL匯入Blueprint]。</td>  
   </tr>  
   <tr>   
     <td role="rowheader">還原情境的先前版本</td>   
     <td>請參閱文章<a href="../../workfront-fusion/scenarios/restore-a-scenario-version.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中還原案例版本。</td>  
   </tr>  
   <tr> 
     <td role="rowheader">設定[！UICONTROL流量控制]設定</td>   
     <td> <p>按一下[！UICONTROL流量控制]圖示。 <img src="assets/flow-control-icon.gif">您可以設定任務重複指定次數、將陣列轉換為一系列組合，以及將多個組合合併為單一組合。 如需詳細資訊，請參閱[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/apps-and-their-modules/flow-control.md" class="MCXref xref">流量控制。</p> </td>  
   </tr>  
   <tr> 
     <td role="rowheader">使用進階工具增強情境</td>   
     <td>按一下[！UICONTROL工具]圖示。 <img src="assets/tools-icon.gif">您可以建立觸發程式、動作、彙總器和轉換器。 如需詳細資訊，請參閱<a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">工具</a>。</td>  
   </tr>  
   <tr> 
     <td role="rowheader">使用文字剖析工具</td>   
     <td>按一下[！UICONTROL文字剖析器]圖示。 <img src="assets/text-parser-icon.gif">您可以從HTML程式碼擷取元素、尋找和擷取符合搜尋模式的字串元素、搜尋和取代文字，以及從網站「刮除」資料。 如需詳細資訊，請參閱<a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">工具</a>。</td>  
   </tr>  
   <tr> 
     <td role="rowheader">存取您最常用的應用程式和服務</td>   
     <td> 按一下畫面底部<strong>[！UICONTROL我的最愛]</strong>區段中的圖示。 當您將應用程式和服務新增到您的情境時，圖示會自動顯示在此區段中。 您也可以按一下[新增]圖示<img src="assets/add-icon.gif">，手動將應用程式和服務新增到此區域。</td>  
   </tr>  
   <tr> 
     <td role="rowheader">測試執行情境</td>   
     <td>按一下<strong>[！UICONTROL執行一次]</strong>，在啟用之前先驗證案例是否如預期般執行。 一旦啟用，情境將會根據其排程執行。 如果所有專案都未如預期執行，您可以造訪我們的錯誤處理區段，瞭解如何處理錯誤。</td> 
   </tr> 
   <tr> 
     <td role="rowheader">使用Devtool對案例進行偵錯</td>   
     <td>如需詳細資訊，請參閱<a href="../../workfront-fusion/scenarios/debug-scenarios-with-dev-tool.md" class="MCXref xref">使用[!DNL Adobe Workfront Fusion] Devtool偵錯案例</a>。
</td> 
   </tr> 
<tr>
<td>檢查情境的狀態</td>
<td>案例可以是作用中或非作用中。 您可以按一下案例詳細資訊中的開啟/關閉按鈕來變更案例狀態。

如需詳細資訊，請參閱下列文章：
<ul>
<li><a href="../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md">在Adobe Workfront Fusion中啟用或停用案例</a></li>
<li><a href="../../workfront-fusion/scenarios/scenario-detail.md">Adobe Workfront Fusion中的案例詳細資訊</a></li>
</ul>
</td>
</tr>
<tr>
<td>變更情境的排程</td>
<td>使用中的情境會根據排程執行。 依預設，一個案例每15分鐘執行一次。 您可以定義已啟動案例執行的時間和頻率，以變更此專案。 融合情境可以排程為每5分鐘執行一次。

如需詳細資訊，請參閱<a href="../../workfront-fusion/scenarios/schedule-a-scenario.md">在Adobe Workfront Fusion中排程情境</a>。
</td>
</tr>
<tr>
<td>重新命名案例</td>
<td>若要重新命名案例，請開啟案例，按一下左上角的案例名稱並加以編輯。 按下Enter或按一下已編輯欄位外部以儲存案例名稱。</td>
</tr>
<tr>
<td>選取第一個束</td>
<td>有些觸發程式模組可讓您選取要開始擷取套件的第一個套裝。

如需詳細資訊，請參閱<a href="../../workfront-fusion/modules/choose-where-trigger-module-starts.md">選擇Adobe Workfront Fusion中的觸發程式模組開始位置</a>。</td>
</tr>
<tr>
<td>設定傳回的套件組合數量</td>
<td>依預設，模組一律只傳回兩個組合。 您可以在欄位[！UICONTROL傳回的套件組合數目上限]中的模組設定中變更此設定。</td>
</tr>
<tr>
<td>設定進階案例設定</td>
<td>[!DNL Adobe Workfront Fusion] 可讓您設定許多其他進階設定。

如需詳細資訊，請參閱<a href="../../workfront-fusion/scenarios/scenario-settings-panel.md"> Adobe Workfront Fusion中的案例設定面板</a>。</td>
</tr>
</tbody>
</table>
