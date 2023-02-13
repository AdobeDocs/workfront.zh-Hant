---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adobe Workfront Fusion的基本術語
description: Adobe Workfront Fusion除了需要Adobe Workfront授權外，還需要Adobe Workfront Fusion授權。
author: Becky
feature: Workfront Fusion
exl-id: 2169dc2e-2135-47e0-a615-3de12cd120a9
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '824'
ht-degree: 0%

---

# 基本術語， [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] 要求 [!DNL Adobe Workfront Fusion] 除 [!UICONTROL Adobe Workfront] 授權。


<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>動作</p> </td> 
   <td>可讓您從選取的應用程式或服務讀取或寫入套件組合的模組。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL聚合器]</p> </td> 
   <td> <p>一種模組，將多個套件組合（多個資料陣列）合併為一個套件組合。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/aggregator-module.md" class="MCXref xref">[!UICONTROL Adobe Workfront Fusion]中的[!UICONTROL Aggregator]模組</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API 密鑰</td> 
   <td>識別呼叫軟體API（用於驗證）的使用者、開發人員或程式的唯一程式碼。 自 [!DNL Adobe Workfront Fusion] 模組可透過連接API來運作，有時需要API金鑰。 API金鑰由需要的應用程式發佈。 例如，若您需要 [!DNL ActiveCampaign]，您可透過 [!DNL ActiveCampaign] 帳戶。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">應用程式或服務</td> 
   <td> <p>最常見的軟體應用程式。</p> <p>應用程式也可以是處理資料的特殊函式，例如迭代器或匯總器。 </p> <p>服務是套件組合的來源，可能包含Web API、網頁、不同類型的伺服器(FTP、SMTP、IMAP)等。 </p> <p> <img src="assets/apps-350x420.jpg" style="width: 350;height: 420;"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">應用程式連接器</td> 
   <td>連線至其他系統的應用程式。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>捆綁</p> </td> 
   <td> <p>套件是模組傳回或接收的基本單元。 套件組合包含項目。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL連接]</p> </td> 
   <td> <p>將應用程式或服務新增至案例時，您很可能必須先建立 [!DNL Workfront Fusion] 和應用程式或服務，以擷取或傳送選取的資料。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md" class="MCXref xref">關於連接 [!DNL Adobe Workfront Fusion] 至應用程式或服務</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>循環</p> </td> 
   <td> <p>週期表示方案運行的兩個階段：操作和提交。 情境可包含一或多個週期。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md" class="MCXref xref">中的方案執行、週期和階段 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>資料儲存</p> </td> 
   <td> <p>一種工具，可儲存來自藍本的資料，或讓您在個別藍本或藍本執行之間傳輸資料。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/data-stores.md" class="MCXref xref">[!UICONTROL Adobe Workfront Fusion]中的資料儲存</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>資料傳輸</p> </td> 
   <td> <p>透過您的案例傳輸的資料量。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/scenarios/scenario-detail.md" class="MCXref xref">[!UICONTROL Adobe Workfront Fusion]中的方案詳細資訊</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>篩選器</p> </td> 
   <td> <p>可在兩個模組之間套用的其他功能。 篩選條件可讓您只使用符合特定條件的套件組合。 您可以套用許多不同的篩選。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">為[!UICONTROL Adobe Workfront Fusion]中的案例新增篩選器</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>ID</p> </td> 
   <td> <p>用來唯一識別套件組合的名稱。 ID通常用於區分要從指定服務更新或刪除的套件組合。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>項目</p> </td> 
   <td> <p>一束的一部分。 套件組合可由多個項目組成。 項目有數種不同類型：文字、數字、布林值（是/否）、日期、時間、緩衝（二進位資料）、集合、選取功能表、陣列和驗證。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL迭代器]</p> </td> 
   <td> <p>一種模組，可讓您取用一組資料（一組資料），並分割為個別的套件。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/iterator-module.md" class="MCXref xref">中的[!UICONTROL迭代器]模組 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>模組</p> </td> 
   <td> <p>藍本中執行功能的單一步驟，例如在相關聯的應用程式或服務中建立記錄。</p> <p>每個應用程式或服務都有各種模組，可定義其回應請求的方式。</p> <p>模組類型有4種：動作、觸發器、迭代器和匯總器。</p> <p> <img src="assets/module.jpg"> </p> <p>如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref">模組類型</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>作業</p> </td> 
   <td> <p>由模組執行的任務。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">公開/私密金鑰</td> 
   <td>公開和私密金鑰用於加密和解密資料。 公鑰可以分發，任何擁有公鑰的人都可以加密資料，但只有私鑰才能解密。 同樣，使用私鑰的用戶可以加密任何使用公鑰的人都可以解密的資料。 私密金鑰加密可確保資料來自私密金鑰的擁有者，並作為資料來源的驗證。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL路由器]</p> </td> 
   <td>允許您複製資料或向方案添加新路由，以便重新路由資料並單獨處理不同的資料組。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/modules/router-module.md" class="MCXref xref">中的[!UICONTROL Router]模組 [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>情境</p> </td> 
   <td> <p>由用戶建立的一系列自動化步驟，每個步驟由模組表示和執行。 案例的目的是移動和操控資料。</p> <p> <img src="assets/scenario-350x178.jpg" style="width: 350;height: 178;"> </p> <p> 如需詳細資訊，請參閱 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!UICONTROL Adobe Workfront Fusion]中建立案例</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>交易</p> </td> 
   <td> <p>[!DNL Workfront Fusion] 使用交易式處理來擷取情境生命週期。 事務由多個階段組成，在這些階段中，資料從一個一致狀態轉換為另一個一致狀態。 共分4個階段：初始化、操作（讀或寫）、提交/回滾和最終處理。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>觸發</p> </td> 
   <td> <p>可讓您抓取自上次執行案例後新增或更新的套件組合的模組。 觸發器有2種類型：輪詢和即時(webhook)。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">中的即時觸發器(Webhook) [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Webhook</p> </td> 
   <td> <p>一種特殊類型的觸發器，可讓您在新套件組合可用後立即執行案例。 如需詳細資訊，請參閱 <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">[!UICONTROL Adobe Workfront Fusion]中的即時觸發器(Webhook)</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
