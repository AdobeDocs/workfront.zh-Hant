---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: 建立多頁校樣
description: 您可以將多個檔案合併為單一多頁校樣。 審核者可以使用校對檢視器中的導覽工具，以瀏覽多頁校樣中的頁面。
author: Courtney
feature: Digital Content and Documents
exl-id: a8ad80d8-0758-4fea-824e-8c206424e295
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '689'
ht-degree: 0%

---

# 建立多頁校樣

您可以將多個檔案合併為單一多頁校樣。 審核者可以使用校對檢視器中的導覽工具，以瀏覽多頁校樣中的頁面。

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

&#42;若要了解您擁有的計畫、授權或校樣權限設定檔，請聯絡您的Workfront或Workfront Proof管理員。

## 建立多頁校樣

啟用此選項時，靜態檔案和網站可透過單一校樣取得。 禁用此選項時，所有文檔和網站都將作為單個校樣生成，並且您可以在指定時間上載最多100個檔案。

若要建立多頁校樣：

1. 前往您要校樣的專案、任務或問題，然後按一下 **檔案** 區段。
1. 按一下 **新增** > **校樣** .
1. 拖放檔案或瀏覽，然後從檔案總管中選取檔案。 一次最多可上傳50個檔案。 如需檔案限制的資訊，請參閱 [考量事項](#considerations) 一節。

   >[!NOTE]
   >
   >互動式檔案（包括影片和互動式網站）無法結合為單一校樣。

1. 在 **單一校樣**，啟用選項， **將所有相容的檔案合併為單一校樣**.
1. 在 **校樣名稱** 欄位中，指定組合校樣的新名稱。
1. （選用）在您已上傳的檔案清單中，拖曳檔案以重新排序檔案。 檔案的順序是組合校樣的頁面順序。
1. （可選）若要從「新增校樣」頁面移除單一檔案，請將滑鼠指標暫留在檔案上，然後按一下 **垃圾** 表徵圖。

   或

   若要一次刪除所有上傳的檔案，請按一下 **全部刪除** 在清單的右上角。

1. 上傳所有檔案後，您必須決定要設定基本校樣或自動校樣：

   * 透過基本校樣，您可以新增想要校樣的審核者數量，但不會分階段組織。 您新增的所有審核者都可以在建立校樣後立即存取校樣。 若要設定基本校樣，請參閱 [使用基本工作流程建立進階校樣](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md).
   * 透過自動校樣，校樣會從舞台移至舞台，Adobe Workfront會在每位使用者需要檢閱時通知他們。 若要設定自動校樣，請參閱 [使用自動化工作流程建立進階校樣](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## 考量事項 {#considerations}

將檔案合併為單一校樣時，請考量下列事項：

* 您最多可上傳500個不同的檔案。
* 您可以合併不同類型的靜態檔案(例如PDF、JPG、DOC、PPT、EXC)，最多總共2,000頁。
* 您可以結合靜態Web擷取。
* 您可以結合GIF檔案；不過，動畫GIF會以靜態檔案處理。
* 無法組合AV檔案和互動式Web捕獲。
* 校樣的縮圖影像是從校樣的第一頁擷取(請參閱 [在Workfront校樣中管理校樣詳細資料](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md))。
* 您可以檢查已結合以在「校樣」詳細資訊頁面上建立校樣的檔案名稱。 如需詳細資訊，請參閱 [在Workfront校樣中管理校樣詳細資料](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
* 如果校樣上啟用了下載原始檔案的選項，您可以下載已合併的所有檔案，以便將校樣建立為.zip檔案。 如需詳細資訊，請參閱  [下載儲存在Workfront Proof中的檔案](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md).
