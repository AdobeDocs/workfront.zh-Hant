---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: 建立多頁校訂
description: 您可以將多個檔案合併為單一多頁校訂。 檢閱者可以使用校訂檢視器中的導覽工具來瀏覽多頁校訂中的頁面。
author: Courtney
feature: Digital Content and Documents
exl-id: a8ad80d8-0758-4fea-824e-8c206424e295
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '693'
ht-degree: 0%

---

# 建立多頁校訂

您可以將多個檔案合併為單一多頁校訂。 檢閱者可以使用校訂檢視器中的導覽工具來瀏覽多頁校訂中的頁面。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>目前計畫：Pro或更高版本</p> <p>或</p> <p>舊版計畫：選擇或Premium</p> <p>如需有關不同方案的校訂存取許可權的詳細資訊，請參閱<a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">存取Workfront中的校訂功能</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>目前計畫：工作或計畫</p> <p>舊版計畫：任何（您必須為使用者啟用校訂）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">校樣權限設定檔 </td> 
   <td>經理或以上</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯檔案的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權或校訂許可權設定檔，請連絡您的Workfront或Workfront Proof管理員。

## 建立多頁校訂

啟用此選項後，靜態檔案和網站可在單一校訂中使用。 停用此選項時，所有檔案和網站都會產生為個別校訂，您一次最多可上傳100個檔案。

若要建立多頁校訂：

1. 前往您要校訂的專案、任務或問題，然後按一下「**檔案**」區段。
1. 按一下「**新增** > **校訂**」。
1. 拖放檔案，或從檔案總管中瀏覽並選取檔案。 您一次最多可上傳50個檔案。 如需檔案限制的資訊，請參閱本文章的[考量事項](#considerations)一節。

   >[!NOTE]
   >
   >互動式檔案（包括視訊和互動式網站）無法合併為單一校訂。

1. 在&#x200B;**單一校訂**&#x200B;底下，啟用選項&#x200B;**將所有相容檔案合併為單一校訂**。
1. 在&#x200B;**校訂名稱**&#x200B;欄位中，指定合併校訂的新名稱。
1. （選用）在您上傳的檔案清單中，拖曳檔案以重新排序。 檔案的順序是合併校訂的頁面順序。
1. （選擇性）若要從新校訂頁面移除單一檔案，請將滑鼠游標停留在檔案上，然後按一下右側出現的&#x200B;**垃圾桶**&#x200B;圖示。

   或

   若要一次刪除所有已上傳的檔案，請按一下清單右上角的&#x200B;**全部刪除**。

1. 上傳所有檔案後，您必須決定要設定基本校樣或自動校樣：

   * 有了基本校訂，您可以新增任意數目的檢閱者來校訂，但他們不會分成多個階段。 您新增的所有檢閱者都可以在您建立校訂後立即存取校訂。 若要設定基本校訂，請參閱[使用基本工作流程建立進階校訂](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)。
   * 有了自動校訂，校訂會從不同階段移動，而Adobe Workfront會在輪到使用者檢閱時通知他們。 若要設定自動化校訂，請參閱[使用自動化工作流程建立進階校訂](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)。

## 考量事項 {#considerations}

將檔案合併為單一校訂時，請考慮下列事項：

* 您最多可以上傳500個個別檔案。
* 您可以合併不同型別的靜態檔案(例如，PDF、JPG、DOC、PPT、EXC)，最多總共2,000頁。
* 您可以合併靜態網頁擷取。
* 您可以合併GIF檔案；不過，動畫GIF會以靜態檔案處理。
* 您無法結合AV檔案和互動式網頁擷取。
* 校訂的縮圖影像是從校訂的第一頁取得(請參閱[在Workfront Proof中管理校訂詳細資訊](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md))。
* 您可以檢查已合併以在校樣詳細資訊頁面上建立校樣的檔案名稱。 如需詳細資訊，請參閱[在Workfront Proof中管理校訂詳細資訊](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)。
* 如果在校樣上啟用了下載原始檔案的選項，則可以下載所有已組合的檔案，以將校樣建立為.zip檔案。 如需詳細資訊，請參閱  [下載儲存在Workfront Proof中的檔案](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md)。
