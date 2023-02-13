---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Adobe Workfront Fusion中的整合模組
description: 聚合器模組是一種模組，旨在將多個資料包合併為單個包。
author: Becky
feature: Workfront Fusion
exl-id: cdc32842-8717-4e05-ab19-2661ee14c12c
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '752'
ht-degree: 0%

---

# [!UICONTROL 匯總器] 模組 [!DNL Adobe Workfront Fusion]

聚合器模組是一種模組，旨在將多個資料包合併為單個包。

如需模組類型的詳細資訊，請參閱 [模組類型](../../workfront-fusion/modules/module-types.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自動化和整合） </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL 匯總器] 模組

當 [!UICONTROL 匯總器] 模組執行，會執行下列動作：

* 累計它在單個源模組操作期間接收的所有套件組合。
* 輸出單個束，每個累積束包含一個項的陣列。 陣列項目的內容取決於特定 [!UICONTROL 匯總器] 模組及其設定。

下圖顯示 [!UICONTROL 匯總器] 模組：

![](assets/array-aggregator-350x190.png)

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL源模組]</p> </td> 
   <td> <p>將從中啟動捆綁聚合的模組。 源模組通常是迭代器或搜索模組，可輸出一系列捆綁。 設定聚合器的源模組（並關閉聚合器設定）時，源模組和聚合器模組之間的路由將包在灰色區域中，以便您清楚地看到聚合的開始和結束。 
   </p> <p>如需迭代程式的詳細資訊，請參閱 <a href="../../workfront-fusion/modules/iterator-module.md" class="MCXref xref">中的[!UICONTROL迭代器]模組 [!DNL Adobe Workfront Fusion]</a></p> <p>如需搜尋模組的詳細資訊，請參閱 <a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref">模組類型</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL目標結構類型]</p> </td> 
   <td> <p>（僅適用於[!UICONTROL陣列聚合器]模組。） 資料應匯總的目標結構。 預設選項[!UICONTROL自定義]允許您選擇應聚合到A[!UICONTROL射線聚合器]輸出包的項 <code>Array </code>項目：</p> <p> <img src="assets/output-bundle's-array-item-350x213.png" style="width: 350;height: 213;"> </p> <p>在[!UICONTROL陣列聚合器]模組之後連接更多模組並返回模組的設定後，[!UICONTROL目標]結構類型下拉清單將包含屬於集合類型的所有以下模組及其欄位，如的[!UICONTROL附件]欄位中所示 [!DNL Slack] &gt;[!UICONTROL建立消息]模組：</p> <p> <img src="assets/array-aggregator-slack-350x253.png" style="width: 350;height: 253;"> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL聚合欄位]</td> 
   <td>選取要納入匯總模組輸出的欄位。</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL組依據]</p> </td> 
   <td> <p>借助於[!UICONTROL Group by]欄位，聚合器的輸出可以拆分為多個組。 [!UICONTROL Group by]欄位可包含針對每個聚合器的輸入包進行評估的公式。 然後，聚合器會為每個相異公式的值輸出一個組合。 每個套件都包含兩個項目：</p> 
    <ul> 
     <li><code>Key </code>包含不重複值。</li> 
     <li><code>Array </code>包含從公式評估為的套件組合中的匯總資料 <code>Key </code>值。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>空匯總後停止處理</p> </td> 
   <td> <p>預設情況下，即使沒有捆綁到達[!UICONTROL聚合器]模組（例如，因為已按其方式過濾掉它們）,[!UICONTROL聚合器]模組也會輸出聚合的結果。 如果啟用空聚合後的[!UICONTROL停止處理]選項，則[!UICONTROL聚合器]模組將不會在此情況下生成任何輸出束，並且流將停止。</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>由源模組和 [!UICONTROL 匯總器] 模組不會由 [!UICONTROL 匯總器] 模組，因此在 [!UICONTROL 匯總器]. 如果需要源模組和源模組之間的模組輸出的捆束中的任何資料 [!UICONTROL 匯總器] 模組，請務必在 [!UICONTROL 匯總器] 模組的設定(如 [!UICONTROL 匯總欄位] 欄位 [!UICONTROL 陣列聚合器] 模組)。


>[!INFO]
>
>**範例：** 使用案例：壓縮所有電子郵件附件，並將ZIP上傳至 [!DNL Dropbox]
>
>以下案例顯示如何：
>
>* 監視傳入電子郵件的郵箱： [!UICONTROL 電子郵件] >[!UICONTROL 觀看電子郵件] 觸發器會輸出包含項目的套件組合 `Attachments[]`，此陣列包含所有電子郵件的附件。
>
>* 查看電子郵件的附件： [!UICONTROL 電子郵件] >[!UICONTROL 迭代附件] 迭代器會從 `Attachments[]` 逐一陣列，並以個別套件形式進一步傳送。
>
>* 匯總 [!UICONTROL 電子郵件] >[!UICONTROL 迭代附件] 模組： [!UICONTROL 封存] >[!UICONTROL 建立封存匯總器] 累計它接收的所有套件組合，並輸出包含ZIP檔案的單一套件組合。
>
>* 將產生的ZIP檔案上傳至 [!DNL Dropbox]: [!DNL Dropbox] > [!UICONTROL 上傳檔案] 從 [!UICONTROL 封存] > [!UICONTROL 建立封存] 模組和上傳至 [!DNL Dropbox].
>
>![](assets/dropbox-archive-350x87.png)
>
>以下是 [!UICONTROL 封存] > [!UICONTROL 建立封存] 匯總：
>
>![](assets/archive-create-an-archive-350x484.png)
