---
product-area: documents
navigation-topic: approvals
title: 從舊版檔案核准移至整合式核准
description: 瞭解當您的組織移至支援統一核准的Workfront版本時，現有檔案核准工作流程的情況。
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
source-git-commit: b612a50b7445732f90b7de2a216f4bca499fd96b
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 1%

---

# 從舊版檔案核准移至整合式核准

移到支援Adobe雲端儲存空間的Workfront版本，也會將您的組織從舊版檔案核准移至統一核准。 本文提供整合式核准中可以使用哪些功能的相關資訊，以及建議Workfront管理員將使用者從舊版檔案核准中移除。


>[!IMPORTANT]
>
>當您改用支援Adobe雲端儲存空間的Workfront版本時，這項變更會套用至整個組織。 從舊版檔案核准移至統一核準時，沒有試行群組或逐步推出選項。<br>
>如需Adobe雲端儲存空間變更的詳細資訊，請參閱[在Adobe雲端儲存空間上移至Workfront](/help/quicksilver/review-and-approve-work/workfront-storage.md)。

## 瞭解從舊版檔案核准到統一核准的變更

|  | 舊版檔案核准 | 整合式核准 |
| --- | --- | --- |
| 核准者和稽核者 | 僅由個別使用者核准 | 由個別使用者或團隊核准或檢閱 |
| 截止日期和提醒 | 沒有自動提醒 | 72小時、24小時及到期日的自動提醒 |
| 核准階段和路徑 | 一個核准階段，沒有平行路徑 | [多個核准階段與平行稽核路徑](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md) |
| 核准範本 | 每個核准都是從頭開始設定 | 在Workfront安裝程式中提供[可重複使用的範本](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md) |
| 檢閱和標示 | 校訂檢視器 | 舊版Workfront儲存物件上的[校訂檢視器](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/doc-approvals-and-proofing.md)，或Adobe雲端儲存物件上的[Frame.io檢視器](/help/quicksilver/review-and-approve-work/workfront-storage.md#review-and-approval-viewer) |
| AI輔助檢閱 | 未提供 | 使用[內容檢閱者](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md)自動進行品牌相容性檢查 |
| 報告 | 舊版報告 | 首頁KPI Widget和[畫布儀表板](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md) |



### 進行中的核准有何變化

在舊版檔案核准中建立的執行中核准，將繼續像升級前一樣運作。 但是，在升級後建立的任何新核准都將使用統一核准。


## 準備升級

* 與一般使用者共用[開始進行統一檢閱和核准](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)文章。
* 檢閱您現有的Workfront Fusion案例。 如果您使用含校訂的舊版檔案核准，請在貴組織升級之前，參閱[更新Workfront Fusion案例以進行統一檢閱和核准](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md)。
* 在畫布儀表板中設定檢閱和核准儀表板，以取代任何舊版核准報告。 如需詳細資訊，請參閱[建立稽核與核准儀表板](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md)。


### 使用者說明文章

* [開始使用統一檢閱和核准](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [檔案核准的可用功能](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/asset-review-and-approval.md)
* [統一檢閱和核准總覽](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [使用Frame.io檢視器檢閱並核准](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-with-frame.md)
* [一起使用統一核准和校訂](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/doc-approvals-and-proofing.md)
* [檔案決定狀態概觀](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/document-approval-status.md)
* [開始使用Workfront內容檢閱者](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md)
