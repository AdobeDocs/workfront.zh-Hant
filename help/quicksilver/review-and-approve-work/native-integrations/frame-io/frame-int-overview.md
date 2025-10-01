---
product-area: documents
navigation-topic: approvals
title: Frame.io整合概述
description: Frame.io整合概述
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: b5f0150b-40b5-4386-98bc-374e7ca65b74
source-git-commit: 9825f095a7be7debb5150ca4bd50f7cf6fd12295
workflow-type: tm+mt
source-wordcount: '736'
ht-degree: 0%

---

# Frame.io整合概述

Workfront和Frame.io整合可讓專案專員在Workfront中管理專案和計畫工作，而創意人員、行銷人員和利害關係人則可以在Frame.io中檢閱和核准資產。

## 內建於Adobe企業儲存空間

這項整合的核心是Adobe企業儲存體：雲端型儲存體解決方案，可作為Adobe企業產品(包括Workfront和Frame.io)資產的中央存放庫。<!--, and Creative Cloud.-->

Adobe企業儲存的主要優點包括：

* 適用於創意與工作管理資產的統一儲存層
* 透過Adobe IMS集中管理許可權，以進行安全存取控制
* Workfront和Frame.io <!--, and Creative Cloud apps -->的端對端資產可見性
* 可擴充的儲存與配額管理，因應企業需求

如需詳細資訊，請參閱[Adobe企業儲存空間概觀](/help/quicksilver/review-and-approve-work/esm-overview.md)。

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

視訊校訂要求的年度上限設定為組織總付費Workfront使用者授權的10% — 標準和輕度。 此上限適用於組織層級。

當使用量達到上限的80%和100%時，Workfront管理員會收到通知。

此限制不適用於Frame.io Enterprise客戶。

#### Frame.io檢視器中支援的檔案型別

Frame.io檢視器支援所有常見的視訊、影像、音訊、PDF和MS® Office型別。 如需支援檔案的詳細清單，請參閱Frame.io[上的](https://help.frame.io/en/articles/9436564-supported-file-types-on-frame-io)型別。

#### Frame.io檢視器的存取與授權

Frame.io檢視器是所有Workfront檢閱和核准工作流程的預設檢視器。 所有擁有付費授權的Workfront使用者都會自動包含此功能。 使用Frame.io檢視器進行檢閱和核准不需要額外的Frame.io授權。

如果您的組織想要利用此整合提供的其他Frame.io功能（例如直接將資產上傳到Frame.io中的專案），您可以購買Frame.io Enterprise授權。 請聯絡您的Adobe客戶代表以排程示範，並探索完整Frame.io解決方案的優點。

此整合無法使用Workfront校訂功能。

## Workfront強大的專案管理

透過Workfront和Frame.io整合，專案專員可以利用Workfront強大的專案管理功能，來規劃、追蹤和管理工作。

如需有關在Workfront中管理專案的詳細資訊，請參閱[專案：文章索引](/help/quicksilver/manage-work/projects/create-projects/create-project.md)。

### 強制的結構與命名慣例

由於此整合是使用ESM建立的，因此在管理專案和檔案時，應注意一些強制的結構與命名慣例。

* 物件名稱必須是唯一的，而且不能重複
* ESM要求階層樹狀結構中具有相同父項的對等物件有唯一的名稱
* 如果檔案屬於相同專案，則不能使用相同名稱

考慮到這些限制，Workfront會視需要自動重新命名物件或檔案，以避免衝突。

### 共用與許可權

在整合過程中，使用者許可權需在Workfront中加以控制並向下流至Frame.io。 這表示您無法邀請使用者加入Frame.io中的專案，也無法修改Frame.io中的使用者許可權。 這些動作需要透過Workfront中的專案共用模式完成。

下表顯示Workfront許可權對應至Frame.io許可權的方式：

<table>
<tr>
<th>Workfront使用者許可權</th>
<th>Frame.io使用者許可權</th>
</tr>
<tr>
<td>管理</td>
<td>編輯與共用</td>
</tr>
<tr>
<td>參與</td>
<td>編輯與共用</td>
</tr>
<tr>
<td>檢視</td>
<td>僅註解</td>
</tr>
</table>



### Workfront的檔案管理

檔案透過此整合在專案層級進行管理，目前無法上傳到任務或問題。

檔案存取也可在專案層級進行管理。 如果使用者擁有專案的存取權，他們可以存取與該專案相關聯的所有檔案。

### 檔案體驗限制

由於此整合是使用Adobe企業儲存空間建立的，因此Workfront中的原始檔案體驗有一些限制：

#### 限制

下列功能不會納入這項整合：

<!--* External document providers-->
* 在Workfront中存取校訂
* Workfront中的檔案檢視器
* 我的最愛檔案
* 要求檔案


<!--#### Temporary limitations

For now, the following capabilities are not available:

* Send documents to Adobe Experience Manager Assets
* Multi-stage approvals
* Upload documents to comments or updates in Workfront
* Upload documents to tasks or issues in Workfront-->
