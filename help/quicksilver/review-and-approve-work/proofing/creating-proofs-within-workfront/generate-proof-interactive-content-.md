---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: 建立ZIP檔案中互動式內容的校樣
description: 您可以為儲存在ZIP檔案中的非網站互動式內容產生校樣。 這類網路內容的範例包括具有串流視訊或音訊的廣告、HTML動畫、互動式橫幅。
author: Courtney
feature: Digital Content and Documents
exl-id: 2ab00d17-a3a3-4417-a958-ac3d95cb8fc8
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 1%

---

# 建立ZIP檔案中互動式內容的校樣

您可以為儲存在ZIP檔案中的非網站互動式內容產生校樣。 這類網路內容的範例包括具有串流視訊或音訊的廣告、HTML動畫、互動式橫幅。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>當前計畫：Pro或更高</p> <p>或</p> <p>舊計畫：Premium</p> <p>如需使用不同計畫校對存取權限的詳細資訊，請參閱 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">存取Workfront中的校對功能</a>.</p> </td> 
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

## 建立ZIP檔案中互動式內容的校樣

將ZIP檔案中的互動式內容新增至校樣後，Adobe Workfront會建立壓縮檔案的校樣。 上傳載入時間可能會因檔案大小而異。 建立較大的檔案需要較長的時間。 您可以離開頁面，Workfront會繼續建立您的檔案。 檔案上傳大小上限為4GB。 

1. 建立ZIP套件檔案，以準備您的內容。

   ZIP檔案必須符合下列要求：

   * 套件檔案中應包含所有資產，例如CSS、JavaScript、影片、音效和影像。
   * 請確定主檔案（如index.html、index.htm）位於根資料夾中，且該檔案是唯一儲存在該處的.html/.htm檔案。

      如果主檔案未置於根資料夾中，Workfront會搜尋資料夾以尋找主檔案。

   * 最大捆綁大小為500 MB。
   * 若是在iOS中建立的ZIP檔案，此工具會自動識別內容所在的正確資料夾。

1. 前往您要上傳ZIP檔案的專案、工作或問題。
1. 按一下 **檔案** 中。
1. 按一下 **新增**，然後按一下&#x200B;**校樣** 中。
1. 在 **新增檔案** 區段中，拖放或瀏覽所需的ZIP檔案。
1. 按一下 **建立校樣** 建立簡單校樣，而不需進行審核程式。\
   或\
   繼續操作，方法是配置高級校樣：

   * [使用基本工作流程建立進階校樣](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [使用自動化工作流程建立進階校樣](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
