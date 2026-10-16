---
product-area: documents
navigation-topic: approvals
title: Adobe雲端儲存空間有何不同
description: 瞭解Adobe雲端儲存體物件的主要差異，包括新的檔案區域、Frame.io檢視器、檔案許可權、物件命名規則、儲存配額和Workfront Fusion。
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
source-git-commit: c6f385adb378adaa8aa8110373573315f89f2ed8
workflow-type: tm+mt
source-wordcount: '1702'
ht-degree: 0%
---
# Adobe雲端儲存空間有何不同

使用Adobe雲端儲存空間時，您的環境可包含兩種物件型別：舊版Workfront儲存空間上的物件（您目前擁有的物件）和使用Adobe雲端儲存空間建立的物件。 新的「檔案」區域、Frame.io檢視器以及此處說明的其他行為僅適用於使用Adobe雲端儲存空間的物件。

如需移動的方向，請參閱[在Adobe雲端儲存空間上移至Workfront](/help/quicksilver/review-and-approve-work/workfront-storage.md)。

## 瞭解舊版Workfront儲存空間和Adobe雲端儲存空間

總體而言，這兩種儲存模式在資料所在位置、哪些Adobe產品可以看到資料，以及有哪些功能可供使用等方面皆不盡相同：

|  | 舊版Workfront儲存空間上的物件 | Adobe雲端儲存空間上的物件 |
|---|---|---|
| 儲存後端 | 僅限Workfront | Adobe 雲端儲存空間 |
| 跨產品可見性 | 僅限Workfront | Workfront、Frame.io和Creative Cloud |
| 功能 | 舊版功能 | 新功能 |

在Adobe雲端儲存空間成為預設值之前建立的物件，會保留在舊版Workfront儲存空間中。 本文所述行為僅適用於您和您的使用者在Adobe雲端儲存空間設定為預設值後建立的Adobe雲端儲存空間物件。

## 差異摘要

Adobe雲端儲存空間最大的日常變更是新的「檔案」區域和Frame.io檢視器，其內部可支援稽核和核准。 還有其他差異會影響您管理物件、檔案和稽核的方式。 下表中的每一個區域都連結到下面的詳細區段。

| 區域 | 不同之處 | 須知事項 |
|---|---|---|
| [新檔案區域](#the-new-documents-area) | 重新設計、統一的「檔案」區域取代了舊的「檔案」區域。 | 沒有全域檔案區域。 您可以從方案、投資組合、專案、任務或問題存取檔案。 |
| [檔案許可權](#document-permissions) | 檔案會繼承其所連結專案、任務或問題的許可權。 | 您無法共用或設定個別檔案的許可權。 您可以透過Workfront中的物件「共用」模式管理所有存取權，該模式會級聯至系統產生的檔案資料夾。 |
| [物件許可權對應](#object-permissions-mapping) | 管理和貢獻許可權都對應到Frame.io中的編輯和共用。 僅檢視註解的對應。 | 您可以在Workfront中管理許可權。 「管理」和「貢獻」使用者都能在Frame.io中獲得外部共用功能。 |
| [檢閱和核准檢視者](#review-and-approval-viewer) | Frame.io檢視器會取代Workfront校訂檢視器。 | 所有Workfront使用者皆可使用此功能，包括指派給稽核或核准的外部使用者。 支援標示、時間戳記評論、版本記錄、行動裝置、40多種格式，以及最大500 GB的檔案。 |
| [物件命名規則](#object-naming-rules) | 套用嚴格的命名規則：產品組合或專案中的唯一名稱、無特殊字元、無結尾句點或空格，以及255個字元的限制。 | 發生衝突時，Workfront會自動重新命名物件。 稽核產生新專案名稱和結構的範本。 |
| [物件可攜性](#object-portability) | 在大多數情況下，您只能在類似儲存模型之間移動、複製和轉換物件。 | 您可以在三種特定情況下，將舊版物件轉換為Adobe雲端儲存空間。 在轉換期間，檔案和檔案資料夾不會從舊版儲存空間移動。 |
| [功能無法使用](#capabilities-not-available-on-adobe-cloud-storage-objects) | Workfront Proof、Workfront檔案檢視器、我的最愛檔案和請求檔案不屬於體驗。 | 舊版物件仍保留這些功能。 Workfront Proof將不會獲得新投資，並將在未來版本中淘汰。 |
| [儲存配額](#storage-quota) | 儲存空間會針對舊版Workfront專案和Adobe雲端儲存空間專案進行集區，每個獲授權的使用者儲存空間為60 GB，並無硬性上限。 | 系統管理員可以在「設定」的「客戶資訊」頁面上檢視儲存空間使用量。 |
| [年度影片檢閱次數上限](#annual-video-review-cap) | 視訊校訂請求設有組織層級的上限，為付費Workfront使用者授權的10% （標準和輕度）。 | 一旦達到上限，就無法在下一年度期間之前建立新的視訊評論。 您會分別以80%和100%收到應用程式內通知。 上限不適用於Frame.io Enterprise客戶。 |
| [Workfront Fusion](#workfront-fusion-on-adobe-cloud-storage-projects) | 現有的校訂型Fusion案例無法自動用於Adobe雲端儲存空間專案。 | 範圍設定為舊版專案的案例仍可繼續運作。 每個受影響的案例都採取以下三個路徑之一：編輯、重建或淘汰。 |

## 新檔案區域

新的檔案區域是專為Adobe雲端儲存空間設計的統一檔案體驗。 它可簡化導覽、整合稽核及核准活動，並是Frame.io檢視器的入口點。

全域檔案區域不是新體驗的一部分。 在Adobe雲端儲存空間專案中，您可以從方案、投資組合、專案、任務或問題存取檔案。

如需詳細資訊，請參閱[檔案區域](/help/quicksilver/documents/managing-documents/documents-area.md)。

## 檔案許可權

檔案許可權在Adobe雲端儲存空間專案上截然不同：

* 您無法共用或設定個別檔案的許可權。 而是將許可權套用至包含檔案的系統產生檔案資料夾。
* 系統產生的檔案資料夾繼承其父專案、任務或問題的許可權。
* 子檔案夾從父系系統產生的檔案檔案夾繼承許可權。
* 子任務不會從父任務繼承許可權。 您必須直接新增至子任務，才能存取其系統產生的檔案資料夾。

如需檔案許可權如何運作的詳細資訊，請參閱[Adobe雲端儲存模型的](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work)物件許可權和存取層級總覽。

## 物件許可權對應

許可權是在Workfront中設定，且會以一個方向流向Frame.io。 您無法邀請使用者加入Frame.io中的Adobe雲端儲存空間專案，或修改Frame.io中的使用者許可權。

>[!TIP]
>
>訓練專案協調員，讓他們知道Frame.io存取是Workfront許可權的下游反映。 如果利害關係人報告他們無法存取Adobe雲端儲存空間專案的評論，則修正位於Workfront中，而非Frame.io。

下表將Workfront物件許可權對應至Frame.io許可權：

| Workfront許可權 | Frame.io許可權 |
|---|---|
| 管理 | 編輯與共用 |
| 參與 | 編輯與共用 |
| 檢視 | 僅註解 |

在Frame.io中管理及貢獻地圖以編輯和共用。 檢閱Adobe雲端儲存專案的共用模式時，請考慮讓貢獻者具有與管理員相同的檢閱端功能（包括外部共用）是否符合您的治理模式。

如需詳細資訊，請參閱[Adobe雲端儲存模型的](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#permission-mapping-to-frameio)物件許可權和存取層級總覽。

## 檢閱和核准檢視者

在Adobe雲端儲存物件上，Frame.io檢視器是稽核和核准介面，取代Workfront Proof。 所有Workfront使用者皆可免費使用Frame.io檢視器，包括指派給檢閱或核准的外部使用者。

Frame.io檢視器提供：

* 標籤和註解工具，包括手繪繪圖和標準形狀，例如圓形、箭頭和正方形
* 視訊評論的時間戳記加上精確影格
* 版本記錄和版本比較
* 行動存取以進行行動稽核和核准
* 支援40多種檔案格式，包括所有常見的視訊、影像、音訊、PDF和Microsoft Office型別，並支援ProRes、H.265和DNxHD等專業視訊格式的原生播放，以及高達500 GB的檔案支援

## 物件命名規則

Adobe雲端儲存空間會強制實施嚴格的命名和結構規則，以保持跨Adobe產品的儲存層一致性。 這些規則適用於您在Adobe雲端儲存空間專案上建立的物件。 現有的舊版專案會保留其目前名稱。

下列規則適用於Adobe雲端儲存空間專案：

| 規則 | 詳細資訊 |
|---|---|
| 唯一的計畫和專案名稱 | 如果程式和專案屬於相同的投資組合，則不能有相同的名稱。 |
| 唯一檔名稱 | 如果檔案屬於相同專案，則不能使用相同名稱。 檔名稱在資料夾階層的相同父項中必須是唯一的。 |
| 禁止的字元 | 程式、投資組合、專案、範本、任務、問題、檔案資料夾和檔案不能包含下列任何特殊字元： `\ / : * ? " \| < >` |
| 結尾字元 | 計畫、投資組合、專案、範本、任務、問題和檔案資料夾不能有以句點或空格結尾的名稱。 |
| 名稱長度限制 | 物件名稱長度上限為255個字元。 |

如果名稱與這些規則衝突，Workfront會自動重新命名物件以解決衝突。

>[!TIP]
>
>如果您從範本建立Adobe雲端儲存空間專案，請檢閱現有的範本，以便它們產生的專案名稱和結構符合上述規則。

## 物件可攜性

在大多數案例中，您只能在類似儲存模式之間移動、複製和轉換Workfront物件。 例如，您可以將任務從一個Adobe雲端儲存空間專案移動至另一個Adobe雲端儲存空間專案。 您可以在三種特定情況下，將舊版Workfront儲存體物件轉換成Adobe雲端儲存體。

如需詳細資訊，請參閱[將舊物件轉換成Adobe雲端儲存空間](/help/quicksilver/review-and-approve-work/convert-objects-to-adobe-cloud-storage.md)。

## Adobe雲端儲存體物件上未提供的功能

下列功能不是Adobe雲端儲存體物件的一部分：

* Workfront Proof
* Workfront檔案檢視器
* 我的最愛檔案
* 要求檔案

舊版專案仍可存取Workfront Proof及上方列出的舊版檔案功能。 Workfront Proof未來將不會獲得新投資，並將在未來版本中淘汰。

## 儲存配額

系統會針對舊版Workfront物件和Adobe雲端儲存物件來共用儲存空間。 每個獲授權的使用者會收到60 GB的儲存空間。 儲存使用量沒有硬性上限，但是當使用量達到配額的75%、90%和100%時，Workfront管理員會收到電子郵件通知。

若要檢視目前的儲存使用量和配額，請移至&#x200B;**設定** > **系統** > **客戶資訊**。

如需詳細資訊，請參閱[檢查檔案儲存限制](/help/quicksilver/documents/managing-documents/check-document-storage.md)。

## 年度影片檢閱次數上限

視訊校訂要求的年度上限設定為貴組織總付費Workfront使用者授權（標準和輕度）的10%。 此上限適用於組織層級。

* 當使用量達到上限的80%和100%時，Workfront管理員會收到應用程式內通知。
* 一旦達到上限，就無法在下一年度期間之前建立新的視訊評論請求。
* 此限制不適用於Frame.io Enterprise客戶。 如果貴組織定期檢視大量視訊內容，請聯絡您的Adobe客戶代表，瞭解有關Frame.io Enterprise授權的相關資訊。

如需詳細資訊，請參閱[整合式檢閱和核准總覽](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)中的檢閱和核准資產和影片常見問題集。

## Adobe雲端儲存空間專案上的Workfront Fusion

建置在舊版校訂上的現有Workfront Fusion案例不會自動針對Adobe雲端儲存空間專案運作。 校訂特定的模組、webhook和API端點在某些情況下有直接的同等功能，而在其他情況下會有重大變更。 範圍設定為舊版專案的情境照常運作。

如需常見情境型別所受影響的詳細資訊，以及如何根據情境的功能將每個情境分類為「編輯」、「重新建置」或「淘汰」，請參閱[更新Workfront Fusion情境以進行統一稽核和核准](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md)。
