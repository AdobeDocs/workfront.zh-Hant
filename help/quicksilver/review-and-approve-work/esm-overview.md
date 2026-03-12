---
product-area: documents
navigation-topic: approvals
title: Adobe企業儲存空間概覽
description: Adobe企業儲存空間概覽
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 16c564a9-abd7-4b07-be3e-9c823f40177d
source-git-commit: 97c351ca38a8b6075634b2f755f2330562bc8b52
workflow-type: tm+mt
source-wordcount: '809'
ht-degree: 0%

---

# Adobe企業儲存空間概覽

Adobe企業儲存是以雲端為主的儲存解決方案，可作為Adobe企業產品中資產的中央存放庫。 Workfront與Frame.io整合以Adobe企業儲存空間為基礎，可實現這些平台之間的無縫合作和資產管理。

此儲存選項也為日後資產管理與其他Adobe產品（例如Adobe Creative Cloud）的整合鋪平了道路。

## 主要功能

* **統一儲存層**： Adobe企業儲存空間可作為Workfront、Frame.io、Document Cloud和Creative Cloud的共用儲存後端。 如此一來，便能跨越這些平台進行順暢的協同作業和資產管理。

* **啟用內容supply chain**： Adobe企業儲存空間是Adobe內容Supply chain願景的基本元件，可讓團隊管理進行中的資產，而不需要在多種Adobe應用程式中手動下載或重新上傳。

* **集中式許可權和存取**： Adobe企業儲存支援企業級存取控制，並與Adobe IMS (Identity Management System)整合，以獲得安全且可擴充的使用者許可權。

* **端對端資產可見性**：儲存在Adobe企業儲存空間中的Assets可直接在Workfront、Frame.io和Creative Cloud應用程式中顯示和管理，提供一致的中繼資料、版本設定和稽核追蹤。

* **與檢閱和核准工作流程整合**： Adobe企業儲存空間可作為所有資產的真實來源，以確保集中追蹤意見回饋和核准，進而啟用創意檢閱和核准工作流程。

* **可擴充的儲存和配額管理**： Adobe企業儲存提供可擴充的儲存選項，以及跨Adobe產品的統一配額追蹤。

## 與檢閱和核准工作流程整合

Workfront和Frame.io整合採用Adobe企業儲存空間，可提供統一的稽核和核准體驗。 此整合可讓專案專員在Workfront中管理專案和計畫工作，而創意人員、行銷人員和利害關係人可以檢閱和核准Frame.io中的資產。 這可確保所有利害關係人都能存取最新版本的資產，並將意見回饋集中在一處。

如需Workfront與Frame.io整合的詳細資訊，請參閱[Frame.io整合總覽](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/frame-int-overview.md)。

## Adobe企業儲存裝置與舊版Workfront儲存裝置之間的差異

現有Workfront環境同時具備Adobe企業儲存功能和舊版Workfront儲存功能。 在Adobe企業儲存體發行之前建立的任何物件，都會使用舊版Workfront儲存體。

在環境中啟用Adobe企業儲存空間後，您就可以建立Adobe企業儲存空間和舊版Workfront儲存空間專案。

>[!NOTE]
>
>全新環境預設會啟用Adobe企業儲存空間，且無法選擇使用舊版Workfront儲存空間。


### 文件

#### 新檔案區域

新檔案區域是為Adobe企業儲存空間重新設計的統一檔案區域。

此更新的介面簡化了導覽，提高了清晰度，並使團隊更輕鬆地在一個統一環境中管理審查和核准。 如需詳細資訊，請參閱[檔案區域概觀](/help/quicksilver/documents/managing-documents/documents-area.md)。

#### 新檔案許可權模型

>[!IMPORTANT]
>
>在Adobe企業儲存體中，檔案許可權的運作方式與舊版Workfront儲存體不同。 檔案會繼承其連結的專案、任務或問題的許可權。

檔案無法個別共用。 相反地，系統為每個任務或問題自動產生一個檔案夾，並繼承任務或問題的許可權。 上傳到任務或問題的任何檔案都會儲存在該產生的資料夾中。

如需有關新檔案許可權模型的詳細資訊，請參閱[Adobe企業儲存模型的](/help/quicksilver/review-and-approve-work/esm-access-permissions.md)物件許可權和存取層級總覽。

##### 資料夾上的連結物件

在專案層級，系統產生的資料夾會顯示連結物件。 資料夾會自動命名為與其所屬的任務或問題相同的名稱。 連結的資料夾是系統知道該資料夾應該顯示在哪個任務或問題的方式。

如需詳細資訊，請參閱[檔案許可權如何運作](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work)。

## Workfront物件

下表比較了Workfront物件的Adobe企業儲存功能和舊版Workfront儲存功能。

Workfront物件包括投資組合、方案、專案、範本、任務和問題。

| Adobe企業儲存空間 | 舊版Workfront儲存空間 |
|---|---|
| <ul><li>使用Adobe企業儲存空間</li><li>與Frame.io整合</li><li>使用新的檔案體驗</li><li>強制嚴格的命名慣例</li><li>無法使用直接檔案共用</li><li>檔案可用於其他Adobe產品，例如Frame.io和Creative Cloud</li></ul> | <ul><li>使用Workfront儲存空間</li><li>使用校訂檢視器</li><li>支援個別檔案共用</li></ul> |

### 移動、複製和轉換物件

您可以在類似的儲存模型之間移動、複製和轉換Workfront物件。 例如，您可以將任務從Adobe企業儲存體專案移動至另一個Adobe企業儲存體專案。 您無法將任務從Adobe企業儲存體專案移動至舊版Workfront儲存體專案。

這些動作可從任務或問題的「更多」選單取得。 每個動作都遵循檔案完整性、許可權繼承和Adobe企業儲存規則。

## 啟用Adobe企業儲存空間

現有客戶可在續約時在其環境中啟用Adobe企業儲存空間。 如需有關啟用Adobe企業儲存空間的詳細資訊，請參閱[為您的組織啟用Adobe企業儲存空間](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md)。

>[!NOTE]
>
>新客戶預設已啟用Adobe企業儲存空間，且無法選擇使用舊版Workfront儲存空間。






