---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Adobe Workfront Fusion中的彙總模組
description: 彙總器模組是一種模組，旨在將數個資料套件合併為單一套件組合。
author: Becky
feature: Workfront Fusion
exl-id: cdc32842-8717-4e05-ab19-2661ee14c12c
source-git-commit: 948fe5fc249e0dcb04655f015c8e46493159c3ed
workflow-type: tm+mt
source-wordcount: '827'
ht-degree: 0%

---

# 在[!DNL Adobe Workfront Fusion]中的[!UICONTROL 彙總]模組

彙總器模組是一種模組，旨在將數個資料套件合併為單一套件組合。

如需模組型別的詳細資訊，請參閱[模組型別](../../workfront-fusion/modules/module-types.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

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

+++

## [!UICONTROL 彙總]模組總覽

執行[!UICONTROL 彙總]模組時，它會執行下列動作：

* 累計單一來源模組作業期間收到的所有組合。
* 輸出單一組合，其陣列包含每個累積組合一個專案。 陣列專案的內容取決於特定的[!UICONTROL 彙總]模組及其設定。

下圖顯示[!UICONTROL 彙總]模組的典型設定：

![](assets/array-aggregator-350x190.png)

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[！UICONTROL Source模組]</p> </td> 
   <td> <p>套件組合彙總開始的模組。 來源模組通常是輸出一系列組合的疊代器或搜尋模組。</p><p>當您設定彙總器的來源模組（並關閉彙總器的設定）時，來源模組與彙總器模組之間的路由會以灰色區域包圍，以便您可以清楚看到彙總的開始與結束。 
   </p> <p>如需迭代器的詳細資訊，請參閱[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/modules/iterator-module.md" class="MCXref xref">[！UICONTROL Iterator]模組</p> <p>如需搜尋模組的詳細資訊，請參閱<a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref">模組型別</a>中的搜尋模組。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL目標結構型別]</p> </td> 
   <td> <p>（僅適用於[！UICONTROL陣列彙總]模組。） 彙總資料的目標結構。 預設選項[！UICONTROL自訂]可讓您選擇應彙總至[！UICONTROL陣列彙總]之輸出套件組合的<code>Array </code>專案的專案：</p> <p> <img src="assets/output-bundle's-array-item-350x213.png" style="width: 350;height: 213;"> </p> <p>在[！UICONTROL陣列彙總]模組之後連線更多模組並返回模組的設定後，[！UICONTROL Target]結構型別下拉式功能表將包含下列所有模組及其欄位的「集合陣列」型別，如[!DNL Slack] &gt;[！UICONTROL建立訊息]模組的[！UICONTROL附件]欄位中所示：</p> <p> <img src="assets/array-aggregator-slack-350x253.png" style="width: 350;height: 253;"> </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL彙總欄位]</td> 
   <td>您要包含在彙總模組輸出中的欄位。</td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL Group by]</p> </td> 
   <td> <p>藉助[！UICONTROL Group by]欄位，可將彙總器的輸出分割成數個群組。 [！UICONTROL Group by]欄位可包含針對每個彙總器的輸入組合進行評估的公式。 然後，彙總器會針對每個不同公式的值輸出一個組合。 每個組合都包含兩個專案：</p> 
    <ul> 
     <li><code>Key </code>包含不同的值。</li> 
     <li><code>Array </code>包含來自套裝的彙總資料，公式針對這些資料評估為<code>Key </code>值。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>在空白彙總後停止處理</p> </td> 
   <td> <p>根據預設，即使沒有套件組合到達[！UICONTROL彙總]模組（例如，因為已在途中篩選掉），[！UICONTROL彙總]模組也會輸出彙總的結果。 如果選項[！UICONTROL Stop processing after an empty aggregation]已啟用，[！UICONTROL Aggregator]模組在此情況下將不會產生任何輸出組合，且流程將停止。</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>來源模組與[!UICONTROL 彙總]模組之間模組產生的組合未由[!UICONTROL 彙總]模組輸出，因此在[!UICONTROL 彙總]之後，流程中的模組無法存取這些組合。 如果您需要來源模組與[!UICONTROL 彙總程式]模組之間模組輸出的任何套件組合資料，請務必在[!UICONTROL 彙總程式]模組的設定（如同[!UICONTROL 陣列彙總程式]模組設定中的[!UICONTROL 彙總欄位]欄位）中包含指定專案。


## 彙總如何運作的範例案例

此範例案例顯示如何壓縮所有電子郵件附件，以及將ZIP上傳至[!DNL Dropbox]。

![](assets/dropbox-archive-350x87.png)

下列案例顯示如何：

* 第一個模組會監視信箱是否有傳入電子郵件： [!UICONTROL 電子郵件] >[!UICONTROL 監視電子郵件]觸發器將會輸出含有專案`Attachments[]`的組合，該專案是包含所有電子郵件附件的陣列。

* 第二個模型會逐一迭代電子郵件的附件： [!UICONTROL 電子郵件] >[!UICONTROL 迭代附件]迭代器會逐一從`Attachments[]`陣列中取得專案，然後以個別的套件組合進一步傳送它們。

* 第三個模組會彙總[!UICONTROL 電子郵件] >[!UICONTROL 重複附件]模組輸出的組合： [!UICONTROL 封存] >[!UICONTROL 建立封存彙總]，會彙總其收到的所有組合，並輸出包含ZIP檔案的單一組合。

* 最後一個模組會將產生的ZIP檔案上傳至[!DNL Dropbox]： [!DNL Dropbox] > [!UICONTROL 上傳檔案]從[!UICONTROL 封存] > [!UICONTROL 建立封存]模組並上傳至[!DNL Dropbox]取得ZIP檔案。



以下是[!UICONTROL 封存] > [!UICONTROL 建立封存]彙總的範例設定：

![](assets/archive-create-an-archive-350x484.png)
