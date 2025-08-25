---
product-area: documents
navigation-topic: approvals
title: 開始使用Workfront AI Reviewer
description: Workfront AI檢閱者
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 0f4fd3a7-9578-4fda-b10f-9b4be147f1de
source-git-commit: 945fa710e98b094a37258d5c94f7b1a2eb056abb
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 4%

---

# 開始使用Workfront AI Reviewer

>[!NOTE]
>
>此功能目前處於Beta測試階段。

有了Workfront AI Reviewer，您可以加快內容速度，並在稽核和核准工作流程中最佳化品牌合規性。 您可以在Workfront中將AI稽核者新增至核准範本或個別稽核和核准請求。

## 存取需求

若要在Workfront中設定AI檢閱者，您必須是系統管理員。

任何使用者都可以將AI稽核者新增至稽核和核准請求。


## 先決條件

* 貴組織必須已移轉至Adobe IMS (Identity Management系統)。
* 您的Workfront執行個體必須已啟用統一核准。
* Adobe必須有已簽署的Adobe Gen AI合約檔案。
如需簽署合約的詳細資訊，請參閱[簽署Adobe Gen AI合約](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)。


## 支援的檔案類型 {#supported-file-types-ai-reviewer}

>[!CONTEXTUALHELP]
>id="wf_document_approvals_ai_supported_files"
>title="不受支援的檔案類型"
>abstract="此 AI 檢閱者不支援所選的檔案類型。上傳支援的檔案類型，或移除 AI 檢閱者以提交請求。"

AI檢閱者可檢閱下列檔案型別：

* PNG (.png)
* JPEG (.jpeg， .jpg)
* WEBP (.webp)
* 非動畫GIF (.gif)

## 設定品牌指南

Workfront AI檢閱者在檢閱內容時，會使用Genstudio Foundation中設定的品牌准則。 目前，您只能設定影像的品牌指南。 如需詳細資訊，請參閱[開始使用Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/zh-hant/docs/genstudio-for-performance-marketing/user-guide/get-started)。


## 建立AI檢閱者

一旦GenStudio基礎中至少設定了一個品牌，Workfront管理員即可在設定區域中開始建立AI檢閱者。 然後可以將這些AI稽核者指派給核准範本和個別稽核與核准請求。 目前，AI檢閱者只能根據影像品牌准則進行檢閱。

如需詳細資訊，請參閱[建立AI檢閱者](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/set-up-ai-reviewer.md)。

## 新增AI稽核者以稽核和核准請求

使用者可以將AI稽核者新增至現有的核准範本或個別稽核與核准請求。

### 核准範本

如果您的組織經常新增相同人員來稽核和核准請求，Standard授權使用者可以在Workfront設定區域中建立核准範本。

使用者可以將AI稽核者新增至核准範本，以在範本用於建立請求時自動檢查品牌相容性。

核准範本建立後，可套用至專案、任務或問題的檔案區域中的資產。

如需詳細資訊，請參閱[建立資產和檔案的核准範本](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)。

顯示AI檢閱者的![範本清單](assets/ai-review-templates.png)

### 個別檢閱和核准請求

當使用者建立個別稽核和核准請求時，他們可以在中新增一個AI檢閱者與其他參與者，或者他們也可以建立單個請求，只讓AI檢閱者檢查品牌相容性。

如需詳細資訊，請參閱[建立檔案檢閱或核准要求](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)。


![AI稽核者已新增至個別核准請求](assets/ad-ai-reviewer-to-request.png)

## 檢視AI檢閱者評分和意見反應

在提交具有AI檢閱者的檢閱和核准請求後的幾秒鐘，來自AI檢閱者的分數和意見可在「檔案摘要」面板中取得 — 即使其他參與者仍在檢閱和做出決定。

核准擁有者也會收到電子郵件，通知他們資產上已完成稽核。 在電子郵件中，按一下&#x200B;**前往檢閱**&#x200B;並檢視Workfront中的分數和意見反應。

AI檢閱者並非設計成檢閱和核准工作流程中的決策者。 它只會提供分數和建議，以讓資產符合指定的品牌需求。

如果影像長度不符合品牌准則，創意人員可以上傳新版本，而核准擁有者可以透過AI檢閱者建立第二個稽核和核准請求，讓您在版本之間切換並比較意見回應。

如需有關檢視分數和意見回饋的詳細資訊，請參閱[檢視AI檢閱者分數和意見回饋](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/view-ai-reviewer-feedback.md)。


![AI檢閱者意見](assets/ai-reviewer-feedback.png)


## 影片逐步解說

>[!VIDEO](https://video.tv.adobe.com/v/3470847/)