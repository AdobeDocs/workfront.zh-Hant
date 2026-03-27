---
product-area: documents
navigation-topic: approvals
title: 統一檢閱和核准總覽
description: 深入瞭解由Workfront和Frame.io支援的統一檢閱和核准。
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 32cb95c2-8d12-492b-ad89-b38e2a337fc5
source-git-commit: d35e6c33479ed051aaa87b07ddf38811fffc0cc0
workflow-type: tm+mt
source-wordcount: '835'
ht-degree: 0%

---


# 統一檢閱和核准總覽

由Workfront和Frame.io提供支援的統一檢閱和核准，可讓專案專員在Workfront中管理專案和計畫工作，而創意人員、行銷人員和利害關係人可以在Frame.io中檢閱和核准資產。

## 整合需求

* Workfront和Frame.io必須部署至相同的Identity Management系統(IMS)組織。

* 使用者只能屬於IMS組織內的一個Workfront執行個體。

* 必須在Adobe Unified Experience和Adobe企業儲存空間上啟用Workfront執行個體。

* 整合必須由Adobe Professional Services設定。


## 內建於Adobe企業儲存空間

統一的檢閱和核准是以Adobe企業儲存空間為基礎所打造，這是一種雲端式儲存空間解決方案，可作為Adobe企業產品（包括Workfront和Frame.io）資產的中央存放庫。<!--, and Creative Cloud.-->

Adobe企業儲存的主要優點包括：

* 適用於創意與工作管理資產的統一儲存層
* 使用Adobe Identity Management系統(IMS)集中管理許可權，以進行安全存取控制
* Workfront和Frame.io <!--, and Creative Cloud apps -->的端對端資產可見性
* 可擴充的儲存與配額管理，因應企業需求

如需詳細資訊，請參閱[Adobe企業儲存空間概觀](/help/quicksilver/review-and-approve-work/esm-overview.md)。

## 統一的稽核和核准

透過統一的稽核和核准，您可以：

* 直接從Workfront建立和管理稽核與核准
* 即時追蹤稽核和核准的狀態
* 將意見反應與核准集中於一處
* 確保所有利害關係人都能存取最新版本的資產
* 利用AI稽核者來自動進行品牌法規審查
* 及更多內容

如需詳細資訊，請參閱[整合檔案核准：文章索引](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-reviews-and-approvals.md)。


### 使用Frame.io檢視器

使用Frame.io檢視器檢閱及核准資產。 Frame.io檢視器提供

* 標籤和註解工具
* 版本記錄與比較
* 視訊評論的時間戳記評論
* 行動存取以進行行動稽核和核准

如需詳細資訊，請參閱[開始進行統一檢閱和核准](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)。

#### 影片檢閱限制

視訊校訂要求的年度上限設定為組織總付費Workfront使用者授權的10% — 標準和輕度。 此上限適用於組織層級。

當使用量達到上限的80%和100%時，Workfront管理員會收到通知。

此限制不適用於Frame.io Enterprise客戶。

#### Frame.io檢視器中支援的檔案型別

Frame.io檢視器支援所有常見的視訊、影像、音訊、PDF和MS® Office型別。 如需支援檔案的詳細清單，請參閱Frame.io[上的](https://help.frame.io/en/articles/9436564-supported-file-types-on-frame-io)支援的檔案型別。

#### Frame.io檢視器的存取與授權

Frame.io檢視器是所有Workfront檢閱和核准工作流程的預設檢視器。 所有擁有付費授權的Workfront使用者都會自動包含此功能。 使用Frame.io檢視器進行檢閱和核准不需要額外的Frame.io授權。

如果您的組織想要利用此整合提供的其他Frame.io功能（例如直接將資產上傳到Frame.io中的專案），您可以購買Frame.io Enterprise授權。 請聯絡您的Adobe客戶代表以排程示範，並探索完整Frame.io解決方案的優點。

此整合無法使用Workfront校訂功能。

## Workfront強大的專案管理

專案專員可善用Workfront強大的專案管理功能來規劃、追蹤及管理工作。

如需有關在Workfront中管理專案的詳細資訊，請參閱[專案：文章索引](/help/quicksilver/manage-work/projects/create-projects/create-project.md)。

### 強制的結構與命名慣例

由於統一檢閱和核准是使用Adobe企業儲存空間建立的，因此在管理專案和檔案時，應注意一些強制執行的結構和命名慣例。

* 物件名稱必須是唯一的，而且不能重複
* 對於階層樹狀結構中具有相同父級的對等物件，Adobe企業儲存體必須有唯一的名稱
* 如果檔案屬於相同專案，則不能使用相同名稱
* 檔名稱不能包含下列任何特殊字元： \ / ： * ？ 「 | &lt; >
* 檔名稱上限為255個字元

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

上傳至Workfront的檔案會儲存在Adobe企業儲存空間中，並可在Workfront和Frame.io中存取。 當您將檔案上傳到Workfront中的任務或問題時，系統會在Adobe企業儲存空間中建立一個系統產生的檔案夾，該檔案夾會繼承任務或問題的許可權。 上傳至該任務或問題的所有檔案都會儲存在該資料夾中，並繼承其許可權。 如需Workfront中檔案的詳細資訊，請參閱[新檔案區域概觀](/help/quicksilver/documents/managing-documents/documents-area.md)和[Adobe企業儲存模型的物件許可權和存取層級概觀](/help/quicksilver/review-and-approve-work/esm-access-permissions.md)。

### 檔案體驗限制

不包含下列檔案功能：

<!--* External document providers-->
* 在Workfront中存取校訂
* Workfront中的檔案檢視器
* 我的最愛檔案
* 要求檔案










<!--
# Unified Approvals overview

>[!IMPORTANT]
>
>The content of this article refers to updated document approval functionality that is only available for specific accounts. For information on standard approval processes, see the articles listed in [Work approvals](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

Unified Approvals, previously referred to as New Document Approvals, is a holistic redesign of the existing approvals process that is currently in development for Adobe Workfront. Currently available in limited release, it is designed to be a practical and effective solution for businesses requiring comprehensive stakeholder engagement and version-specific document approvals. Its thoughtful design and purposeful new features facilitate collaboration, role clarity, and version control in the approval process, enhancing efficiency and accountability.

## Key differences from Proofing and legacy document approvals

**Differences from Proofing**

* Document approval participants display in the document Summary, not the proofing workflow tab.
* Unified Approvals are not supported in the current reporting tool. 

    You can join the new Canvas Dashboards beta to [Create a report dashboard for review and approvals](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md), or you can use the Document approval metrics widget available in new Home and Canvas Dashboards provides the following details about Unified Approvals:

    * Approvals by decision
    * Average approval time
    * Pending approvals
    * Overdue approvals

**Differences from Legacy document approvals**

With Unified Approvals, you can

* Add reviewers in addition to approvers
* Designate an entire Workfront team as either reviewers or approvers
* Set a deadline for the review or approval
* Create and resuse approval templates
* Utilize new versions 
* View multiple key performance indicators for your approvals in Workfront Home widgets
* Use Canvas Dashboards to view reporting details about Unified Approvals

## Using Unified Approvals

For users looking to create or manage document approvals, see the articles listed in [Set up and manage unified approvals: article index](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/set-up-and-manage-doc-asset-approvals-toc.md)

For users looking to review or approve documents for which they have received a request, see the articles listed in [Approve and review documents: article index](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-and-approve-documents/review-documents-toc.md).



-->