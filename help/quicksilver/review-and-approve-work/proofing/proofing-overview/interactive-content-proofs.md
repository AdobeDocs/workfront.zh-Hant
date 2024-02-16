---
product-area: documents
navigation-topic: proofing-overview
title: 互動式內容校訂概觀
description: 互動式內容提供多種吸引觀眾的方法。 機構可使用從對此內容的回應中收集的分析來衡量其促銷活動的成功。
author: Courtney
feature: Digital Content and Documents
exl-id: fdcad9c6-5508-476a-bfb8-2fe3bfbb007b
source-git-commit: f783e3033a67b4702e4e2d80214cbb0c4591b922
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 0%

---

# 互動式內容校訂概觀

<!-- Audited: 01/2024 -->

互動式內容提供多種吸引觀眾的方法。 機構可使用從對此內容的回應中收集的分析來衡量其促銷活動的成功。

互動式內容的範例包括：

* 網站
* 內嵌或串流視訊
* 互動式橫幅
* HTML5動畫
* 微網站
* 互動式電子郵件

## 關於建立互動式內容的校樣

您可以透過下列其中一種方式來建立互動式內容的校樣：

* 從包含互動式內容的ZIP檔案建立校訂。

  Adobe Workfront會從ZIP檔案解壓縮內容，並將其儲存在Workfront伺服器上。 由於是以這種方式儲存的，因此在整個校訂檢閱週期中，內容可能會保持不變。

* 指定內容的URL。

  這是建立互動式內容校樣的最簡單方法。 這也是以互動方式檢閱內容的唯一方法，因為使用者會在網際網路上體驗內容。

  透過此方法，Workfront未知的外部伺服器會儲存並託管內容。

  我們建議對大型網站使用此方法，因為很難收集構成大型網站的所有檔案。 不過，由於校樣的內容儲存在外部，Workfront無法保護它不受開發人員所做的變更影響，因此您可能無法在整個校樣檢閱週期中依賴保持相同的內容。

## 關於在ZIP檔案中準備互動式內容以進行校樣

將互動式內容繫結在ZIP檔案以進行校訂時，請確定該檔案包含下列規格：

* 所有資產（例如CSS、JavaScript、影片、聲音和影像）都應包含在套件檔案中。
* 互動式內容應包含主檔案(index.html、index.htm)。 如果此檔案未放置在根位置，則工具會自動搜尋資料夾以尋找它。 主檔案名稱不需是index.html/index.htm，不過主位置只能放置一個.html/.htm檔案。
* 檔案必須至少包含一個靜態檔案網頁。
* 最大套件大小為500 MB。
* 若是在iOS中建立的.zip檔案，此工具會自動識別內容所在的資料夾。
* 互動式專案僅支援作為.zip封存。 標準.zip檔案提交將失敗。
* 網站必須是安全的(HTTPS)。

  使用「案頭校訂檢視器」時不需要如此。

  如需詳細資訊，請參閱 [瞭解案頭校訂檢視器](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md).

* 必須允許在iframe中檢視網站。

  使用「案頭校訂檢視器」時不需要如此。

  如需詳細資訊，請參閱 [瞭解案頭校訂檢視器](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md).

## 關於建立互動式校樣

準備ZIP套件組合檔案後，請建立互動式校訂。

如需詳細資訊，請參閱 [在ZIP檔案中建立互動式內容的校訂](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-interactive-content.md).

或者，如果您正在使用Workfront校訂，請參閱區段 [產生互動式內容的校訂](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md#generate-a-proof-for-interactive-content) 在文章中 [在Workfront Proof中產生校訂](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## 關於檢閱互動式校樣

我們建議您使用獨立的案頭校訂檢視器作為互動式校訂的預設檢視器。 但是，如果貴組織的原則不允許使用Desktop Proofing Viewer應用程式，您的Workfront管理員可以設定您的系統，以便您可以在Web Proofing Viewer中檢閱整合在ZIP封存檔案中的互動式內容。 如需有關「案頭校訂檢視器」和「網頁校訂檢視器」的比較資訊，請參閱 [網頁校訂檢視器與案頭校訂檢視器之間的差異概述](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).
