---
product-area: documents
navigation-topic: approvals
title: Adobe雲端儲存空間概覽
description: Adobe雲端儲存空間概覽
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 16c564a9-abd7-4b07-be3e-9c823f40177d
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/YOO4BspMzbMr8iPoXRBKK65IbU5yfpiJndNuYvYF5SM
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 9d28f52ace4d443bdffc475baf79d482152d4157
workflow-type: tm+mt
source-wordcount: 1004
ht-degree: 0%

---

# Adobe雲端儲存空間概覽

Adobe雲端儲存是以雲端為主的儲存解決方案，可作為Adobe企業產品中資產的中央存放庫。 Workfront與Frame.io整合建立在Adobe雲端儲存空間上，可在這兩種平台之間實現順暢的協同作業和資產管理。

此儲存選項也為日後資產管理與其他Adobe產品（例如Adobe Creative Cloud）的整合鋪平了道路。

## 主要功能

* **統一儲存層**： Adobe雲端儲存空間可作為Workfront、Frame.io、Document Cloud和Creative Cloud的共用儲存後端。 如此一來，便能跨越這些平台進行順暢的協同作業和資產管理。

* **啟用內容supply chain**： Adobe雲端儲存空間是Adobe內容Supply chain願景的基本元件，可讓團隊管理進行中資產，而不需要在各種Adobe應用程式中手動下載或重新上傳。

* **集中式許可權和存取**： Adobe雲端儲存支援企業級存取控制，並與Adobe IMS (Identity Management System)整合，以獲得安全且可擴充的使用者許可權。

* **端對端資產可見性**：儲存在Adobe雲端儲存空間中的Assets可直接在Workfront、Frame.io和Creative Cloud應用程式中顯示和管理，提供一致的中繼資料、版本設定和稽核追蹤。

* **與檢閱和核准工作流程整合**： Adobe雲端儲存空間可作為所有資產的真實來源，以確保集中追蹤意見回饋和核准，進而啟用創意檢閱和核准工作流程。

* **可擴充的儲存空間與配額管理**： Adobe雲端儲存空間提供可擴充的儲存空間選項，以及跨Adobe產品的統一配額追蹤。

## 與檢閱和核准工作流程整合

Workfront和Frame.io整合運用Adobe雲端儲存空間，提供統一的稽核和核准體驗。 此整合可讓專案專員在Workfront中管理專案和計畫工作，而創意人員、行銷人員和利害關係人可以檢閱和核准Frame.io中的資產。 這可確保所有利害關係人都能存取最新版本的資產，並將意見回饋集中在一處。

如需Workfront與Frame.io整合的詳細資訊，請參閱[整合式檢閱和核准總覽](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)。

## Adobe雲端儲存空間與舊版Workfront儲存空間之間的差異

現有Workfront環境同時具備Adobe雲端儲存空間及舊版Workfront儲存空間。 任何在Adobe雲端儲存空間發行前建立的物件，都會使用舊版Workfront儲存空間。

在環境中啟用Adobe雲端儲存空間後，您就可以建立Adobe雲端儲存空間和舊的Workfront儲存空間專案。

>[!NOTE]
>
>全新環境預設啟用Adobe雲端儲存空間，且無法選擇使用舊版Workfront儲存空間。


### 文件

#### 新檔案區域

新的檔案區域是為Adobe雲端儲存空間重新設計的統一檔案區域。

此更新的介面簡化了導覽，提高了清晰度，並使團隊更輕鬆地在一個統一環境中管理審查和核准。 如需詳細資訊，請參閱[檔案區域概觀](/help/quicksilver/documents/managing-documents/documents-area.md)。

#### 新檔案許可權模型

>[!IMPORTANT]
>
>在Adobe雲端儲存空間中，檔案許可權的運作方式與舊版Workfront儲存空間不同。 檔案會繼承其所連結專案、任務或問題的許可權。

檔案無法個別共用。 相反地，系統為每個任務或問題自動產生一個檔案夾，並繼承任務或問題的許可權。 上傳到任務或問題的任何檔案都會儲存在該產生的資料夾中。

如需有關新檔案許可權模型的詳細資訊，請參閱[Adobe雲端儲存模型的](/help/quicksilver/review-and-approve-work/esm-access-permissions.md)物件許可權和存取層級總覽。

##### 資料夾上的連結物件

在專案層級，系統產生的資料夾會顯示連結物件。 資料夾會自動命名為與其所屬的任務或問題相同的名稱。 連結的資料夾是系統知道該資料夾應該顯示在哪個任務或問題的方式。

如需詳細資訊，請參閱[檔案許可權如何運作](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work)。

## Workfront物件

下表比較了Workfront物件的Adobe雲端儲存空間與舊版Workfront儲存空間的功能。

Workfront物件包括投資組合、方案、專案、範本、任務和問題。

| Adobe 雲端儲存空間 | 舊版 Workfront 儲存空間 |
|---|---|
| <ul><li>使用Adobe雲端儲存空間</li><li>與Frame.io整合</li><li>使用新的檔案體驗</li><li>強制嚴格的命名慣例</li><li>無法使用直接檔案共用</li><li>檔案可用於其他Adobe產品，例如Frame.io和Creative Cloud</li></ul> | <ul><li>使用Workfront儲存空間</li><li>使用校訂檢視器</li><li>支援個別檔案共用</li></ul> |

### 移動、複製和轉換物件

在大多數案例中，您可以在類似儲存模式之間移動、複製和轉換Workfront物件。 例如，您可以將任務從一個Adobe雲端儲存空間專案移動至另一個Adobe雲端儲存空間專案。

在三種特定情況下，您可以將舊版Workfront儲存體物件轉換為Adobe雲端儲存體：

* 將舊版Workfront儲存空間任務轉換為Adobe雲端儲存空間專案。
* 將舊版Workfront儲存產品組合轉換為Adobe雲端儲存產品組合。
* 從舊版Adobe儲存空間範本建立Workfront雲端儲存空間專案。

在轉換期間，檔案和檔案資料夾不會從舊版Workfront儲存空間移至Adobe雲端儲存空間。

如需詳細資訊，請參閱[在Adobe雲端儲存空間](/help/quicksilver/review-and-approve-work/workfront-storage.md)上移至Workfront中的[物件可攜性](/help/quicksilver/review-and-approve-work/workfront-storage.md#object-portability)。

## 啟用Adobe雲端儲存空間

您必須使用支援Adobe雲端儲存空間的Workfront版本。 如果貴組織尚未使用支援的版本，請聯絡您的Adobe客戶代表。

如需在您的環境中啟用Adobe雲端儲存空間的相關資訊，請參閱[為您的組織啟用Adobe雲端儲存空間](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md)。

>[!NOTE]
>
>新客戶預設已啟用Adobe雲端儲存空間，且無法選擇使用舊版Workfront儲存空間。



## 沙箱環境中的Adobe雲端儲存空間

Adobe雲端儲存空間可在[!DNL Workfront]沙箱環境中使用，因此您可以在生產環境中啟用它之前先測試它。 不過，沙箱中不提供Frame.io檢視器，因此完整統一檢閱和核准體驗必須在生產環境中驗證。

如果您有自訂重新整理沙箱，您必須在升級至支援Adobe雲端儲存空間的Workfront版本後，重新整理沙箱，才能存取沙箱中的Adobe雲端儲存空間功能。 如需詳細資訊，請參閱[自訂重新整理沙箱環境](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md)。 [!DNL Adobe Workfront] 

## 考量事項

* Workfront可能會與Frame.io或Creative Cloud不同步，例如資產在Workfront中刪除但仍出現在Frame.io中，請聯絡Workfront支援以重新同步您的環境。


