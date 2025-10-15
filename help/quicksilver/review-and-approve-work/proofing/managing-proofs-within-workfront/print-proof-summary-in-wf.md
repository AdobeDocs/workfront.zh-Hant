---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 在Adobe Workfront中列印校訂摘要
description: 您可以列印校樣摘要、將其儲存為PDF，或匯出為針對Adobe Reader最佳化的XLS檔案或PDF檔案。
author: Courtney
feature: Digital Content and Documents
exl-id: 129c8e6b-5c66-445b-a5d0-7b1460aeabd6
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 1%

---

# 在Adobe Workfront中列印校訂摘要

您可以列印校樣摘要、將其儲存為PDF，或匯出為針對Adobe Reader最佳化的XLS檔案或PDF檔案。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> 
   <p>標準</p>
   <p>工作或計畫</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">校樣權限設定檔 </td> 
   <td>經理或以上</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯檔案的存取權</p> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 列印校訂摘要或儲存為PDF檔案

您可以直接從檔案清單列印校訂摘要。

>[!NOTE]
>
>* 不支援大於1 GB的摘要。
>* 您無法同時從檔案清單列印多個校訂摘要。

1. 在包含校樣的檔案清單中，將滑鼠移至包含檔案的列，然後按一下&#x200B;**列印摘要**。

   ![proof_printsummary.png](assets/proof-printsummary-350x166.png)

   或

   在校訂檢視器中檢視校訂時，按一下左側工具列中的&#x200B;**列印**&#x200B;圖示![列印圖示](assets/print-icon-in-pv.png)。 （如果看不到左邊的工具列，請按一下校訂檢視器左上角的功能表圖示![功能表圖示](assets/menu-icon-in-pv.png)。）

1. 使用下列任一選項：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">顯示</td> 
      <td> <p>指定您要列印的內容：</p> 
       <ul> 
        <li>校訂的<strong>目前版本</strong>或<strong>所有版本</strong></li> 
        <li>僅限含有註解的<strong>頁面</strong>或<strong>所有頁面</strong></li> 
        <li>僅<strong>頁面縮圖</strong> （每個頁面的小量轉譯）或<strong>完整頁面</strong> （證明的完整轉譯）<br></li> 
        <p>附註：若要在列印輸出中檢視標示上的圖釘號碼，您必須選取「整頁」，而不是「頁面縮圖」。 </p> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">評論排序依據</td> 
      <td> <p>（僅當您選取上面的「頁面縮圖」時可用）指定您要校樣註解的列印順序：</p> 
       <ul> 
        <li><strong>Oldest</strong>：從第一個註解到最後一個註解</li> 
        <li><strong>Latest</strong>：從上一個註解到第一個註解</li> 
        <li><strong>頁面</strong>：依頁面，從第一頁到最後一頁，或從最後一頁到第一頁</li> 
        <li><strong>建立者</strong>：根據新增的使用者名稱，從A-Z或從Z-A</li> 
       </ul> <p>這些選項不會影響您匯出為XLS或PDF檔案的輸出。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">篩選註解依據</td> 
      <td> <p>您可以使用這些選項的任何組合，在列印或匯出為XLS或PDF檔案的輸出中僅包含某些註解：</p> 
       <ul> 
        <li>您選取的作者（預設）</li> 
        <li>您選取的動作</li> 
        <li><strong>未解決</strong>狀態</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">工作流程</td> 
      <td> <p>（只有在校訂具有自動化工作流程時才可用）您可以按一下<strong>顯示圖表</strong>，在列印輸出中加入圖表，顯示校訂的階段以及在每個階段所做的決定。 在出現的圖表中，顏色代表在舞台上所做的決策：</p> <p><strong>綠色</strong>：已核准</p> <p><strong>藍色</strong>：擱置決定</p> <p><strong>紅色</strong>：需要變更決定</p> <p><strong>灰色</strong>：尚未開始</p> <p><strong>黃色</strong>：已核准變更</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**列印**。
1. 在出現的視窗的右側面板中，如果要列印摘要，請按一下&#x200B;**目的地**&#x200B;功能表，然後按一下&#x200B;**檢視更多**。 在顯示的清單中按一下您要使用的印表機，然後按一下[列印]。****

   或

   如果您要將摘要儲存為PDF檔案，請按一下&#x200B;**目的地**&#x200B;功能表，按一下&#x200B;**儲存為PDF**，然後按一下&#x200B;**儲存**。

## 將校訂摘要匯出為XLS或PDF

您可以將靜態內容的校訂摘要匯出為XLS檔案或PDF檔案。 校訂匯出僅包含校訂的內容。

1. 在包含校樣的檔案清單中，將滑鼠移至包含檔案的列，然後按一下&#x200B;**列印摘要**。

   ![proof_printsummary.png](assets/proof-printsummary-350x166.png)

1. 按一下頁面右上角附近的XLS圖示或PDF圖示。

   ![XLS PDF圖示](assets/xls-pdf-icons-350x136.png)

當匯出的檔案準備就緒時，您會收到一封電子郵件，您可從中下載檔案。

如果您將摘要匯出為PDF檔案，則校訂上的評論會顯示在PDF閱讀器中。 如果註解具有多個相關聯的標示，註解將會在註解清單中出現多次（每次標示出現一次）。
