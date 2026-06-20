---
product-area: documents
navigation-topic: approvals
title: 更新Workfront Fusion案例以進行統一檢閱和核准
description: 當您的組織採用Workfront雲端儲存空間並統一檢閱和核準時，清查、分類和修正以舊版Workfront校訂為基礎的Adobe Fusion案例。
author: Courtney
feature: Work Management, Digital Content and Documents
role: Admin
source-git-commit: a3ef3b4ea00298e23ebc8b6196c951417e75eebe
workflow-type: tm+mt
source-wordcount: '802'
ht-degree: 0%

---

# 更新Workfront Fusion案例以進行統一檢閱和核准

在舊版Workfront校訂上建置的Workfront Fusion案例不會自動搭配Adobe雲端儲存空間專案使用。 校訂特定的模組、webhook和API端點在某些情況下有直接的同等功能，而在其他情況下會有重大變更。 在將依賴受影響情境的團隊帶入Adobe雲端儲存推出之前，本文會協助您清查受影響的情境、將其分類並決定補救路徑。

範圍設定為舊版Workfront專案的情境照常運作。 本文所述的補救工作適用於您打算針對Adobe雲端儲存空間專案執行的情境。

>[!IMPORTANT]
>
>Adobe Workfront統一檢閱和核准聯結器現在可在Workfront Fusion中使用。 我們建議將此聯結器用於更簡單、更可靠的案例，當搭配使用Fusion和Adobe雲端儲存空間時。
>
>如需相關資訊與指示，請參閱Workfront Fusion檔案中的[Adobe Workfront統一檢閱與核准模組](https://experienceleague.adobe.com/zh-hant/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-review-and-approvals-modules)。

使用本文章清查及分類案例，瞭解升級Fusion案例的最佳方式，以說明Adobe雲端儲存空間。

如需貴組織在Adobe雲端儲存空間上移至Workfront時變更的高層級摘要，請參閱[在Adobe雲端儲存空間上移至Workfront](/help/quicksilver/review-and-approve-work/workfront-storage.md)。


## Fusion在Adobe雲端儲存空間專案上的變更

以Workfront Proof為基礎的現有Fusion案例所依賴的校訂特定模組、webhook觸發器，以及API端點不屬於統一檢閱和核准資料模型。 下表將常見案例型別對應至其預期影響和後續路徑：

| 案例型別 | 影響 | 前進路徑 |
|---|---|---|
| 校訂建立和路由 | 分隔符號 | 在2026年第3季使用統一核准API重新建置 |
| 校訂狀態Webhook | 分隔符號 | 在2026年第3季度使用新的核准事件觸發器重新構建 |
| 檔案上傳觸發程式 | 部分：需要重新測試 | 2026年第3季移轉後稽核並重新測試 |
| 核准提醒通知 | 分隔符號 | 以核准範本截止日期取代 |
| 核准決定路由 | 分隔符號 | 使用新的決定狀態列位重新建置 |
| 自訂核准報告 | 部分：欄位名稱可能會變更 | 將舊版欄位對應到新結構描述 |


## 將每個案例分類為編輯、重建或淘汰

每個情境所需的工作取決於其功用以及統一檢閱和核准中可用的內容。 使用下列分類：

* **編輯**：現有的校訂相關動作在統一檢閱和核准中具有直接對等功能，您可以更新情境以使用新動作。
* **重新建置**：基礎步驟已大幅變更，或案例應使用的新功能已存在，因此需要從頭重新建置案例。
* **淘汰**：原生統一檢閱和核准功能，例如具有截止日期提醒的多階段核准範本，會取代建立情境的目的。

針對您的特定商業邏輯檢閱每個案例，以決定其分類。

## 補救方法

使用下列方法來規劃和執行Fusion修正：

1. **立即清查。** 提取作用中Fusion案例的完整清單，並標籤每個參考校訂建立、校訂狀態、檔案核准或核准路由的案例。 請勿等到Adobe雲端儲存空間啟用後再使用。
1. **根據上一節的條件將每個情境**&#x200B;分類為「編輯」、「重新建置」或「淘汰」。
1. **在將依賴校訂的團隊帶入Adobe雲端儲存試驗之前，請暫停依賴校訂的案例**。 對新模型執行過時的校訂式自動化可能會產生無訊息的失敗或重複的動作。
1. **使用核准範本取代簡單的路由邏輯。** 具有截止日期自動化的原生多階段核准範本可以處理許多先前需要Fusion的使用案例。 如需詳細資訊，請參閱[建立資產和檔案的核准範本](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)。
1. **重建時使用Adobe Workfront整合式檢閱和核准聯結器。** 更新的聯結器會公開專門為統一檢閱和核准而建置的模組，並讓重新建置流程大幅簡化且更可靠。 我們不建議預先針對Workfront API 22版進行重建。
1. **在沙箱執行個體**&#x200B;中端對端測試重建情境，然後在生產環境中啟用它們。 請特別留意事件訂閱裝載 — 欄位名稱和結構描述與舊版校訂事件不同。

>[!TIP]
>
>許多組織都累積了Fusion情境，這些情境是解決舊版校訂中差距的解決方法。 原生統一檢閱和核准功能（包括核准範本、截止日期提醒和多階段路由）可完全消除其中部分情境的需求。 當您分類每個案例時，請評估原生功能是否可以取代它。 淘汰情境通常比重建更乾淨的長期結果。

## 相關文章

* [在Adobe雲端儲存空間上移至Workfront](/help/quicksilver/review-and-approve-work/workfront-storage.md)
* [統一檢閱和核准總覽](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [開始使用統一檢閱和核准](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [建立資產和檔案的核准範本](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)
