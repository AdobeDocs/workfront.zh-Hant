---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: 在ZIP檔案中建立互動式內容的校訂
description: 您可以為儲存在ZIP檔案中的非網站互動式內容產生校訂。 這類網頁內容的範例包括含有串流視訊或音訊的廣告、HTML動畫、互動橫幅。
author: Courtney
feature: Digital Content and Documents
exl-id: 2ab00d17-a3a3-4417-a958-ac3d95cb8fc8
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 1%

---

# 在ZIP檔案中建立互動式內容的校訂

您可以為儲存在ZIP檔案中的非網站互動式內容產生校訂。 這類網頁內容的範例包括含有串流視訊或音訊的廣告、HTML動畫、互動橫幅。

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

## 在ZIP檔案中建立互動式內容的校訂

一旦您將互動式內容加入ZIP檔案到校訂中，Adobe Workfront就會建立壓縮檔案的校訂。 上傳載入時間會依檔案大小而有所不同。 建立大型檔案需要更長的時間。 您可以離開頁面，Workfront會繼續建立您的檔案。 檔案上傳大小上限為4GB。 

1. 建立ZIP隨附檔案，準備您的內容。

   ZIP檔案必須符合下列要求：

   * 所有資產(例如CSS、JavaScript、影片、聲音和影像)都應包含在套件檔案中。
   * 請確定主檔案（例如index.html、index.htm）位於根資料夾中，而且是唯一儲存在根資料夾中的.html/.htm檔案。

     如果主檔案未放在根資料夾中，Workfront會搜尋資料夾以尋找主檔案。

   * 最大套件大小為500 MB。
   * 若是在iOS中建立ZIP檔案，此工具會自動識別內容所在的正確資料夾。

1. 前往您要上傳ZIP檔案的專案、任務或問題。
1. 按一下左側面板中的&#x200B;**檔案**。
1. 按一下[新增]&#x200B;**&#x200B;**，然後在出現的功能表中按一下[校訂]&#x200B;**&#x200B;**。
1. 在&#x200B;**新增檔案**&#x200B;區段中，拖放或瀏覽您所需的ZIP檔案。
1. 按一下&#x200B;**建立校訂**&#x200B;以建立不含稽核程式的簡單校訂。\
   或\
   繼續設定進階校訂：

   * [使用基本工作流程建立進階校訂](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [使用自動化工作流程建立進階校訂](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
