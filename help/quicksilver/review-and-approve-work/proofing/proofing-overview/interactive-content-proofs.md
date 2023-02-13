---
product-area: documents
navigation-topic: proofing-overview
title: 互動式內容校樣概觀
description: 互動式內容提供多種吸引檢視者的方法。 代理商可使用從此內容回應中收集的分析，來評估其促銷活動是否成功。
author: Courtney
feature: Digital Content and Documents
exl-id: fdcad9c6-5508-476a-bfb8-2fe3bfbb007b
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 0%

---

# 互動式內容校樣概觀

互動式內容提供多種吸引檢視者的方法。 代理商可使用從此內容回應中收集的分析，來評估其促銷活動是否成功。

互動式內容的範例包括：

* 網站
* 內嵌或串流視訊
* 互動式橫幅
* HTML5動畫
* Microsites
* 互動式電子郵件

本文提供下列關於校對互動式內容的內容：

## 關於建立互動式內容的校樣

您可以透過下列其中一種方式，建立互動式內容的校樣：

* 從包含互動式內容的ZIP檔案建立校樣。

   Adobe Workfront會從ZIP檔案中解壓縮內容，並將其儲存在Workfront伺服器上。 因為是以這種方式儲存的，因此在整個校樣審核週期中，您可以仰賴內容保持相同。

* 指定內容的URL。

   這是建立互動式內容校樣的最簡單方式。 這也是當使用者在網際網路上體驗內容時，以互動方式檢閱內容的唯一方式。

   透過此方法，Workfront未知的外部伺服器會儲存並托管內容。

   建議大型網站使用此方法，因為很難收集組成大型網站的所有檔案。 不過，由於校樣的內容是外部儲存的，Workfront無法保護其免受使用該內容的開發人員所做的變更影響，因此您可能無法依賴內容在整個校樣審核週期中保持相同。

## 關於準備ZIP檔案中的互動式內容以進行校對

將ZIP檔案中的互動式內容打包以進行校對時，請確定內容包含下列規格：

* 套件檔案中應包含所有資產，例如CSS、JavaScript、影片、音效和影像。
* 互動式內容應包含主檔案(index.html、index.htm)。 如果此檔案未置於根位置，則工具會自動搜索資料夾以查找它。 主檔案不需要命名為index.html/index.htm ，但主位置只能放置一個.html/.htm檔案。
* 檔案必須至少包含一個靜態檔案網頁。
* 最大捆綁大小為500 MB。
* 若是在iOS中建立的.zip檔案，此工具會自動識別內容所在的資料夾
* 互動式專案僅支援.zip封存檔。 標準.zip檔案提交會失敗。
* 網站必須安全(HTTPS)。

   使用案頭校對檢視器時，不需要此功能。

   如需詳細資訊，請參閱 [了解案頭打樣檢視器](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md).

* 必須允許在iframe中檢視網站。

   使用案頭校對檢視器時，不需要此功能。

   如需詳細資訊，請參閱 [了解案頭打樣檢視器](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md).

## 關於建立互動式校樣

準備好ZIP套件檔案後，請建立互動式校樣。

如需詳細資訊，請參閱 [建立ZIP檔案中互動式內容的校樣](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-interactive-content-.md).

或者，如果您使用Workfront Proof，請參閱區段 [產生互動式內容的校樣](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md#generati) 在文章中 [在Workfront校樣中產生校樣](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## 關於檢閱互動式校樣

建議您使用獨立案頭校對檢視器作為互動式校樣的預設檢視器。 不過，如果貴組織的原則不允許使用案頭測試檢視器應用程式，則Workfront管理員可以設定您的系統，讓您可以在網頁測試檢視器中，檢閱ZIP封存檔案中隨附的互動式內容。 有關案頭校對查看器和Web校對查看器的比較資訊，請參閱 [Web校對查看器與Desktop Pooting Viewer之間的差異概述](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).
