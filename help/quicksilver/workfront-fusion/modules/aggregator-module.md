---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Adobe Workfront Fusion中的彙總模組
description: 彙總器模組是一種模組，旨在將數個資料套件合併成單一套件。
author: Becky
feature: Workfront Fusion
exl-id: cdc32842-8717-4e05-ab19-2661ee14c12c
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

# [!UICONTROL 彙總] 中的模組 [!DNL Adobe Workfront Fusion]

彙總器模組是一種模組，旨在將數個資料套件合併成單一套件。

如需模組型別的詳細資訊，請參閱 [模組型別](../../workfront-fusion/modules/module-types.md).

## 存取需求

您必須具有下列存取權才能使用本文中的功能：

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
   <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront Fusion]授權**</td> 
   <td>
   <p>目前授權需求：否 [!DNL Workfront Fusion] 授權需求。</p>
   <p>或</p>
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] 適用於工作自動化與整合] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 計畫，您的組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 計畫。</p>
   <p>或</p>
   <p>舊版產品需求：貴組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有哪些計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

有關以下專案的資訊： [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL 彙總] 模組

當 [!UICONTROL 彙總] 模組會執行，其會執行下列動作：

* 累計單一來源模組作業期間收到的所有組合。
* 輸出單一組合，其陣列包含每個累積組合一個專案。 陣列專案的內容取決於特定 [!UICONTROL 彙總] 模組及其設定。

下圖顯示下列專案的典型設定： [!UICONTROL 彙總] 模組：

![](assets/array-aggregator-350x190.png)

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[！UICONTROL來源模組]</p> </td> 
   <td> <p>開始套件組合彙總的模組。 來源模組通常是輸出一系列套件的疊代器或搜尋模組。 當您設定彙總的來源模組（並關閉彙總的設定）時，來源模組與彙總模組之間的路由會以灰色區域包圍，以便您可以清楚看到彙總的開始與結束。 
   </p> <p>如需疊代器的詳細資訊，請參閱 <a href="../../workfront-fusion/modules/iterator-module.md" class="MCXref xref">中的[！UICONTROL迭代器]模組 [!DNL Adobe Workfront Fusion]</a></p> <p>如需搜尋模組的詳細資訊，請參閱中的搜尋模組。 <a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref">模組型別</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL目標結構型別]</p> </td> 
   <td> <p>（僅適用於[！UICONTROL陣列彙總]模組。） 資料應彙總到的目標結構。 預設選項[！UICONTROL Custom]可讓您選擇應彙總至A[！UICONTROL陣列彙總器]的輸出套件組合中的專案 <code>Array </code>專案：</p> <p> <img src="assets/output-bundle's-array-item-350x213.png" style="width: 350;height: 213;"> </p> <p>在[！UICONTROL陣列彙總]模組之後連線更多模組並返回模組的設定後，[！UICONTROL目標]結構型別下拉式清單將包含下列所有模組及其屬於集合陣列型別的欄位，如的[！UICONTROL附件]欄位中所示 [!DNL Slack] &gt;[！UICONTROL建立訊息]模組：</p> <p> <img src="assets/array-aggregator-slack-350x253.png" style="width: 350;height: 253;"> </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL彙總欄位]</td> 
   <td>選取要包含在彙總器模組輸出中的欄位。</td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL Group by]</p> </td> 
   <td> <p>在[！UICONTROL Group by]欄位的協助下，可將彙總器的輸出分割成數個群組。 [！UICONTROL Group by]欄位可包含針對每個彙總器的輸入組合所評估的公式。 然後，彙總器會針對每個相異公式的值輸出一個組合。 每個組合都包含兩個專案：</p> 
    <ul> 
     <li><code>Key </code>包含不同的值。</li> 
     <li><code>Array </code>包含來自套裝的彙總資料，公式針對這些資料評估為 <code>Key </code>值。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>在空白彙總後停止處理</p> </td> 
   <td> <p>根據預設，[！UICONTROL Aggregator]模組會輸出彙總的結果，即使沒有套件組合達到[！UICONTROL Aggregator]模組（例如，因為已在途中篩選出所有套件）。 如果啟用空的彙總之後停止處理選項[！UICONTROL Stop processing]，在此情況下[！UICONTROL Aggregator]模組將不會產生任何輸出組合，且流程將停止。</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>來源模組與之間模組產生的套件組合 [!UICONTROL 彙總] 模組不會輸出 [!UICONTROL 彙總] 模組，因此它們無法由流程中的模組在之後存取 [!UICONTROL 彙總]. 如果您需要來源模組與之間模組輸出的套件組合中的任何資料 [!UICONTROL 彙總] 模組，請務必在下列專案中包含指定專案： [!UICONTROL 彙總] 模組的設定(如同 [!UICONTROL 彙總欄位] 欄位中的設定 [!UICONTROL 陣列彙總] 模組)。


>[!INFO]
>
>**範例：** 使用案例：壓縮所有電子郵件附件並將壓縮檔上傳至 [!DNL Dropbox]
>
>以下案例顯示如何：
>
>* 觀看接收電子郵件的信箱： [!UICONTROL 電子郵件] >[!UICONTROL 觀看電子郵件] 觸發器將輸出包含專案的套件組合 `Attachments[]`，此陣列包含所有電子郵件的附件。
>
>* 重複電子郵件的附件： [!UICONTROL 電子郵件] >[!UICONTROL 迭代附件] 迭代器從以下位置取得專案： `Attachments[]` 一個一個陣列，然後以個別的套件組合進一步傳送。
>
>* 彙總以下專案輸出的組合： [!UICONTROL 電子郵件] >[!UICONTROL 迭代附件] 模組： [!UICONTROL 封存] >[!UICONTROL 建立封存彙總] 累積它收到的所有組合，並輸出包含ZIP檔案的單一組合。
>
>* 將產生的ZIP檔案上傳至 [!DNL Dropbox]： [!DNL Dropbox] > [!UICONTROL 上傳檔案] 從取得ZIP檔案 [!UICONTROL 封存] > [!UICONTROL 建立封存] 模組並將其上傳至 [!DNL Dropbox].
>
>![](assets/dropbox-archive-350x87.png)
>
>以下為的範例設定 [!UICONTROL 封存] > [!UICONTROL 建立封存] 彙總：
>
>![](assets/archive-create-an-archive-350x484.png)
