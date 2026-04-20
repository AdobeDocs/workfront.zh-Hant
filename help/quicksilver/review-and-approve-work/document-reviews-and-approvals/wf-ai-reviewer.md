---
product-area: documents
navigation-topic: approvals
title: 開始使用Workfront內容檢閱者
description: 使用Workfront Content Reviewer AI Collaborator，在稽核和核准工作流程期間根據品牌指引評估內容。
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 0f4fd3a7-9578-4fda-b10f-9b4be147f1de
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 72fa86e6dc653905181603e0111f65eb0ca5965b
workflow-type: tm+mt
source-wordcount: '785'
ht-degree: 1%

---

# 開始使用Workfront內容檢閱者

內容檢閱者是AI共同作業人員，一種AI代理程式，可新增至您的專案、任務和檔案。 AI共同作業人員可在設定區域中設定，並像使用者一樣指派。

在Workfront中，「內容檢閱者」有助於在整個檢閱和核准程式中提高內容速度並改善品牌法規遵循。 您可以將內容稽核者新增至核准範本，或將他們納入個別稽核和核准請求中。

## 存取權要求

若要在Workfront中設定「內容檢閱者」，您必須是系統管理員。

任何使用者都可以將「內容檢閱者」新增至檢閱和核准請求。

## 需求

* 您的Workfront執行個體必須已啟用統一核准。
* 您的組織必須有GenStudio Foundation。
   * Workfront中的內容檢閱者提供GenStudio Foundation中可用的功能，以進行資產檢閱和核准工作流程。 您不需要直接存取GenStudio Foundation即可完成工作。 您透過「內容檢閱者」存取GenStudio Foundation功能時，需遵守Workfront合約的條款。
* Adobe必須有已簽署的Adobe Gen AI合約檔案。
如需簽署合約的詳細資訊，請參閱[簽署Adobe Gen AI合約](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)。
* 沙箱環境中沒有內容檢閱者可用。


## 支援的檔案類型 {#supported-file-types-ai-reviewer}

>[!CONTEXTUALHELP]
>id="wf_document_approvals_ai_supported_files"
>title="不受支援的檔案類型"
>abstract="此內容檢閱者不支援選取的檔案型別。 上傳支援的檔案型別，或移除內容檢閱者以提交請求。"

內容檢閱者可檢閱下列檔案型別：

* PNG (.png)
* JPEG (.jpeg， .jpg)
* WEBP (.webp)
* 非動畫GIF (.gif)
* PDF (.pdf)
* PPT (.ppt， .pptx)
* DOC (.doc， .docx)

如果您上傳不支援的檔案型別，則在建立核准工作流程時，將無法使用「內容檢閱者」選項。

## 設定品牌指南

Workfront內容檢閱者在檢閱您的內容時，會使用品牌指引。 Workfront管理員可以在Workfront設定區域中設定品牌指南。 在GenStudio Foundation中建立的品牌也可在Workfront中使用。

若要設定品牌指南，系統管理員必須：

1. [授予品牌許可權的存取權](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-brands.md)
1. [建立並管理內容檢閱者的品牌](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md)。


## 建立內容檢閱者

設定至少一個品牌後，Workfront管理員即可在設定區域中開始建立內容稽核者。 您可以建立多個內容檢閱者，並聚焦於不同的方針：

* **影像**：此內容檢閱者會根據您在Workfront中設定的影像品牌指導方針檢閱資產。 [!BADGE Beta]{type=Positive tooltip="此功能目前處於Beta測試階段。"}
   * 系統管理員必須簽署Beta版合約才能啟用此功能。
* **品牌語調**：內容檢閱者會根據您在Workfront中設定的品牌語調准則，檢閱資產。

接著，內容檢閱者就可以被指派給核准範本和個別的檢閱與核准請求。

如需詳細資訊，請參閱[設定AI共同作業人員](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md)。

## 新增內容稽核者以稽核和核准請求

使用者可以將「內容稽核者」新增至現有核准範本或個別稽核與核准請求。

### 核准範本

如果您的組織經常新增相同人員來稽核和核准請求，Standard授權使用者可以在Workfront設定區域中建立核准範本。

使用者可以將內容稽核者新增至核准範本，以在使用範本建立請求時自動檢查品牌相容性。

核准範本建立後，可套用至專案、任務或問題的檔案區域中的資產。

如需詳細資訊，請參閱[建立檔案的核准工作流程範本](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)。

顯示AI檢閱者的![範本清單](assets/ai-review-templates.png)

### 個別檢閱和核准請求

當使用者建立個別稽核和核准請求時，他們可以在中新增內容檢閱者與其他參與者，或者他們可以建立僅包含內容檢閱者的單一請求以檢查品牌相容性。

如需詳細資訊，請參閱[建立檔案核准工作流程](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)。


![內容檢閱者已新增至個別核准請求](assets/new-stage.png)

## 檢視內容檢閱者評分和意見反應

提交具有內容檢閱者的稽核和核准請求後，內容檢閱者的分數和意見反應會在「檔案摘要」面板中提供，即使其他參與者仍在稽核和做出決定。

核准擁有者也會收到電子郵件，通知他們資產上已完成稽核。 在電子郵件中，按一下&#x200B;**前往檢閱**&#x200B;並檢視Workfront中的分數和意見反應。

內容檢閱者並非設計成檢閱及核准工作流程中的決策者。 它只會提供分數和建議，以讓資產符合指定的品牌需求。

如果資產不符合品牌指引，創意內容可以上傳新版本，而核准擁有者可以向內容檢閱者建立第二個稽核和核准請求。

如需有關檢視分數和意見回饋的詳細資訊，請參閱[檢視內容檢閱者分數和意見回饋](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/view-ai-reviewer-feedback.md)。

