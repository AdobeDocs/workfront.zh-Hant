---
product-area: documents
navigation-topic: approvals
title: Frame.io整合概述
description: Frame.io整合概述
author: Courtney
feature: Work Management, Digital Content and Documents
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
source-git-commit: 701f3fc2c885363b5f61fb9d77049c7d4c41963d
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 0%

---


# Frame.io整合概述

Workfront和Frame.io整合可讓專案專員在Workfront中管理專案和計畫工作，而創意人員、行銷人員和利害關係人則可以在Frame.io中檢閱和核准資產。

## 內建於Adobe企業儲存空間管理

這項整合的核心是Adobe企業儲存管理(ESM)，這是雲端式的儲存解決方案，可作為Adobe企業產品(包括Workfront和Frame.io)資產的中央存放庫。

Adobe企業儲存管理的主要優點包括：

* 適用於創意與工作管理資產的統一儲存層
* 透過Adobe IMS集中管理許可權，以進行安全存取控制
* Workfront、Frame.io和Creative Cloud應用程式的端對端資產可見性<!--coming soon?-->
* 可擴充的儲存與配額管理，因應企業需求

如需詳細資訊，請參閱[Adobe企業儲存體管理總覽](help/quicksilver/review-and-approve-work/esm-overview.md)。

## 統一的稽核和核准

Workfront和Frame.io整合使用Workfront的統一核准功能來管理檢閱和核准。 透過統一核准，您可以：

* 直接從Workfront建立和管理稽核與核准
* 即時追蹤稽核和核准的狀態
* 將意見反應與核准集中於一處
* 確保所有利害關係人都能存取最新版本的資產
* 利用AI稽核者來自動進行品牌法規審查
* 及更多內容

如需詳細資訊，請參閱[整合檔案核准：文章索引](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-reviews-and-approvals.md)。


### 使用Frame.io檢視器

整合也會連線至Frame.io檢視器。 Frame.io檢視器提供

* 標籤和註解工具
* 版本記錄與比較
* 視訊評論的時間戳記評論
* 行動存取以進行行動稽核和核准

如需詳細資訊，請參閱[開始使用Frame.io整合](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/get-started-with-frame-integration.md)。

#### 影片檢閱限制

<!--need to confirm these-->

#### Frame.io檢視器中支援的檔案型別

Frame.io檢視器支援所有常見的視訊、影像、音訊、PDF和MS® Office型別。 如需支援檔案的詳細清單，請參閱Frame.io[上的](https://help.frame.io/en/articles/9436564-supported-file-types-on-frame-io)型別。

#### Frame.io檢視器的存取與授權

擁有付費授權的所有Workfront使用者都可使用Frame.io檢視器。 不需額外的Frame.io授權，即可使用此整合的Frame.io檢視器來審查和核准。

如果您的組織想要利用額外的Frame.io功能，例如直接將資產上傳到Frame.io中的專案，您可以購買Frame.io企業授權。<!--link to Frame.io enterprise license info or who to contacT?-->

此整合不提供Workfront校訂功能。

## Workfront強大的專案管理

透過Workfront和Frame.io整合，專案專員可以利用Workfront強大的專案管理功能，來規劃、追蹤和管理工作。

如需有關在Workfront中管理專案的詳細資訊，請參閱[專案：文章索引](/help/quicksilver/manage-work/projects/projects-toc.md)。

### 強制的結構與命名慣例

由於此整合是使用ESM建立的，因此在管理專案和檔案時，應注意一些強制的結構與命名慣例。

* 物件名稱必須是唯一的，而且不能重複
* ESM要求階層樹狀結構中具有相同父項的對等物件有唯一的名稱
* 如果檔案屬於相同專案，則不能使用相同名稱

考慮到這些限制，Workfront會視需要自動重新命名物件或檔案，以避免衝突。

### Workfront的檔案管理

檔案透過此整合在專案層級進行管理，目前無法上傳到任務或問題。

檔案存取也可在專案層級進行管理。 如果使用者擁有專案的存取權，他們可以存取與該專案相關聯的所有檔案。

<!--Documents can't be dragged as full folders.-->

### 檔案體驗限制

由於此整合是使用ESM建立的，因此Workfront中的原始檔案體驗有一些限制：

#### 限制

下列功能不會納入這項整合：

* 外部檔案提供者
* 存取校訂
* Workfront中的檔案檢視器


#### 暫時限制

下列功能暫時無法使用：

* 我的最愛檔案
* 要求檔案
* 傳送檔案至Adobe Experience Manager Assets
* 多階段核准
* 在Workfront中上傳檔案以加入評論或更新
* 將檔案上傳至Workfront中的任務或問題



