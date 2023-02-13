---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 在Adobe Workfront中列印校樣摘要
description: 您可以列印校樣摘要、儲存為PDF，或匯出為針對Adobe Reader最佳化的XLS檔案或PDF檔案。
author: Courtney
feature: Digital Content and Documents
exl-id: 129c8e6b-5c66-445b-a5d0-7b1460aeabd6
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '749'
ht-degree: 1%

---

# 在Adobe Workfront中列印校樣摘要

您可以列印校樣摘要、儲存為PDF，或匯出為針對Adobe Reader最佳化的XLS檔案或PDF檔案。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>當前計畫：Pro或更高</p> <p>或</p> <p>舊計畫：Select或Premium</p> <p>如需使用不同計畫校對存取權限的詳細資訊，請參閱 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">存取Workfront中的校對功能</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>當前計畫：工作或計畫</p> <p>舊計畫：任何（您必須為使用者啟用校對）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">校訂權限設定檔 </td> 
   <td>管理員或更高</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對文檔的訪問</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、角色或校樣權限設定檔，請聯絡您的Workfront或Workfront Proof管理員。

## 打印校樣摘要或將其另存為PDF檔案

您可以直接從文檔清單打印校樣摘要。

>[!NOTE]
>
>不能同時從文檔清單中打印多個校樣摘要。

1. 從包含校樣的檔案清單中，將滑鼠指標暫留在包含檔案的列上，然後按一下 **打印摘要**.

   ![proof_printsummary.png](assets/proof-printsummary-350x166.png)

   或

   在校對檢視器中檢視校樣時，按一下 **列印**&#x200B;圖示 ![](assets/print-icon-in-pv.png) 的下一頁。 (如果左側工具欄不可見，請按一下「菜單」表徵圖 ![](assets/menu-icon-in-pv.png) （位於校對檢視器的左上角）。

1. 使用下列任一選項：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">顯示</td> 
      <td> <p>指定要打印的內容：</p> 
       <ul> 
        <li>此 <strong>最新版本</strong> 或 <strong>所有版本</strong> 證明</li> 
        <li>僅 <strong>含有留言的頁面</strong> 或 <strong>所有頁面</strong></li> 
        <li>僅 <strong>頁面縮圖</strong> （每個頁面呈現的小幅內容）或 <strong>完整頁面</strong> （完整呈現校樣）<br></li> 
        <p>注意：要在打印輸出中查看標籤上的釘號，您需要選擇「完整頁」，而不是「頁面縮圖」。 </p> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">按注釋排序</td> 
      <td> <p>（只有在您選取上方的「頁面縮圖」時才可用）指定要列印校樣備注的順序：</p> 
       <ul> 
        <li><strong>最舊</strong>:從第一個評論到最後</li> 
        <li><strong>最新</strong>:從上次評論到第一</li> 
        <li><strong>頁面</strong>:依頁面、從第一頁到最後一頁，或從最後一頁到第一頁</li> 
        <li><strong>建立者</strong>:按添加它們的用戶的名稱，從A-Z或Z-A</li> 
       </ul> <p>這些選項不影響導出為XLS或PDF檔案的輸出。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">依篩選注釋</td> 
      <td> <p>您可以使用這些選項的任意組合，在打印或導出為XLS或PDF檔案的輸出中僅包括某些注釋：</p> 
       <ul> 
        <li>您選取的作者（預設）</li> 
        <li>您選取的動作</li> 
        <li><strong>未解析</strong> 狀態</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">工作流程</td> 
      <td> <p>（只有校樣具有自動化工作流程時才可用）您可以按一下 <strong>顯示圖</strong> 在打印輸出中包含一個圖表，顯示在每個階段上進行的校樣和決策。 在顯示的圖中，顏色表示在舞台上做出的決策：</p> <p><strong>綠色</strong>:已核准</p> <p><strong>藍色</strong>:待決</p> <p><strong>紅色</strong>:需要做出的更改</p> <p><strong>灰色</strong>:尚未開始</p> <p><strong>黃色</strong>:已核准並變更</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **列印**.
1. 在顯示視窗的右側面板中，如果要打印摘要，請按一下 **目的地** ，然後按一下 **查看更多**. 在顯示的清單中，按一下您要使用的打印機，然後按一下 **列印**.

   或

   如果要將摘要儲存為PDF檔案，請按一下 **目的地** 按一下 **另存為PDF**，然後按一下 **儲存**.

## 將校樣摘要匯出為XLS或PDF

您可以將靜態內容的校樣摘要匯出為XLS檔案或PDF檔案。 校樣匯出僅包含校樣的內容。

1. 從包含校樣的檔案清單中，將滑鼠指標暫留在包含檔案的列上，然後按一下 **打印摘要**.

   ![proof_printsummary.png](assets/proof-printsummary-350x166.png)

1. 按一下頁面右上角附近的XLS圖示或PDF圖示。

   ![](assets/xls-pdf-icons-350x136.png)

匯出的檔案準備就緒時，您會收到電子郵件，可從中下載檔案。

如果將摘要匯出為PDF檔案，校樣的註解會顯示在PDF讀取器中。 如果注釋有多個與其關聯的標籤，則注釋將多次出現在注釋清單中（每個標籤一次）。
