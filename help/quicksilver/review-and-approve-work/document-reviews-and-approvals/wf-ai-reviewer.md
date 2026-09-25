---
product-area: documents
navigation-topic: approvals
title: 開始使用Workfront AI Reviewer
description: 使用Workfront AI檢閱者在檢閱和核准工作流程期間，根據品牌指引評估內容。
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 0f4fd3a7-9578-4fda-b10f-9b4be147f1de
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: 'https://experienceleague.adobe.com/5nwapHAbb8wRWqen7a49QfpsAMLPZNEfJUJ2vm4R7SA'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
    internal-label: Approvals
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
    internal-label: Get started
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: bc354886dc8c2f1dae24513f1d74e800e19fb3ab
workflow-type: tm+mt
source-wordcount: '958'
ht-degree: 2%
---
# 開始使用Workfront AI Reviewer

AI檢閱者是AI共同作業人員 — 一種AI代理程式，可新增至您的專案、任務和檔案。 AI共同作業人員可在設定區域中設定，並像使用者一樣指派。

在Workfront中，AI Reviewer可協助提升內容速度，並改善整個稽核和核准程式中的品牌合規性。 您可以將AI稽核者新增至核准範本，或將其納入個別稽核和核准請求中。

## 存取權要求

若要在Workfront中設定AI檢閱者，您必須是系統管理員。

任何使用者都可以將AI稽核者新增至稽核和核准請求。

## 需求

* 您的Workfront執行個體必須已啟用統一核准。
* 您的組織必須有GenStudio Foundation。
  * Workfront中的AI檢閱者提供GenStudio Foundation中可用於資產檢閱和核准工作流程的功能。 您不需要直接存取GenStudio Foundation即可完成工作。 您透過AI Reviewer存取GenStudio Foundation功能須遵守Workfront合約的條款。
* Adobe必須有已簽署的Adobe Gen AI合約檔案。
如需簽署合約的詳細資訊，請參閱[簽署Adobe Gen AI合約](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)。
* AI檢閱者不適用於沙箱環境。


## 支援的檔案類型 {#supported-file-types-ai-reviewer}

>[!CONTEXTUALHELP]
>id="wf_document_approvals_ai_supported_files"
>title="不受支援的檔案類型"
>abstract="此 AI 檢閱者不支援所選的檔案類型。 上傳支援的檔案型別，或移除AI檢閱者以提交請求。"

AI檢閱者可檢閱下列檔案型別：

* PNG (.png)
* JPEG (.jpeg， .jpg)
* WEBP (.webp)
* 非動畫GIF (.gif)
* PDF (.pdf)
* PPT (.ppt， .pptx)
* DOC (.doc， .docx)

如果您上傳不支援的檔案型別，則在建立核准工作流程時，將無法使用AI檢閱者選項。

## 設定品牌指南

Workfront AI Reviewer在檢閱內容時會使用品牌指引。 Workfront管理員可以在Workfront設定區域中設定品牌指南。 在GenStudio Foundation中建立的品牌也可在Workfront中使用。

若要設定品牌指南，系統管理員必須：

1. [授予品牌許可權的存取權](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-brands.md)
1. [為AI檢閱者建立和管理品牌](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md)。


## 建立AI檢閱者

設定至少一個品牌後，Workfront管理員即可在設定區域中開始建立AI檢閱者。 您可以建立多個AI檢閱者，重點關注不同的准則：

* **影像**：此AI檢閱者會根據您在Workfront中設定的影像品牌指導方針檢閱資產。 [!BADGE Beta]{type=Positive tooltip="此功能目前處於Beta測試階段。"}
  * 系統管理員必須簽署Beta版合約才能啟用此功能。
* **品牌聲音**： AI檢閱者會根據您在Workfront中設定的品牌聲音准則檢閱資產。

然後可以將AI稽核者指派給核准範本和個別稽核與核准請求。

如需詳細資訊，請參閱[設定AI共同作業人員](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md)。

## AI檢閱者會評估哪些專案 {#what-ai-reviewer-evaluates}

AI檢閱者會根據指引型別以不同方式評估內容：影像或品牌聲音。

### 影像

AI檢閱者會評估：

* **構成**：焦點、背景、裁切、創意框架
* **燈光與情緒**：使用光線、活力、樂觀主義
* **多樣性和包容性**：代表人物（種族、性別、年齡、能力）

AI檢閱者不會評估：

* **標誌使用方式**：位置、空間、大小、正確的標誌版本
* **調色盤**：符合品牌色彩規範，避免未核准的色彩
* **印刷樣式**：字型系列、粗細、間距、對齊
* **插圖樣式**：與品牌的插圖方式一致
* **協助工具**：對比相容性、清晰度

### 品牌語調

AI檢閱者會評估：

* **語調**：對話式、清晰、人性化，符合品牌個性
* **行話/形式**：避免使用流行語、精英或過度的形式
* **訊息**：鼓勵、誠實、負責的定位（例如AI主題）

AI檢閱者不會評估：

* **法律/法規遵循**：商標使用方式、免責宣告、本地化規則

如需有關撰寫與AI檢閱者評估內容一致的品牌指導方針的指引，請參閱[為AI檢閱者建立和管理品牌](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md)。

## 新增AI稽核者以稽核和核准請求

使用者可以將AI稽核者新增至現有核准範本或個別稽核與核准請求。

### 核准範本

如果您的組織經常新增相同人員來稽核和核准請求，Standard授權使用者可以在Workfront設定區域中建立核准範本。

使用者可以將AI稽核者新增至核准範本，以在範本用於建立請求時自動檢查品牌相容性。

核准範本建立後，可套用至專案、任務或問題的檔案區域中的資產。

如需詳細資訊，請參閱[建立檔案的核准工作流程範本](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)。

顯示AI檢閱者的![範本清單](assets/ai-review-templates.png)

### 個別檢閱和核准請求

當使用者建立個別稽核和核准請求時，他們可以在中新增一個AI檢閱者與其他參與者，或者他們也可以建立單個請求，只讓AI檢閱者檢查品牌相容性。

如需詳細資訊，請參閱[建立檔案核准工作流程](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)。


![AI檢閱者已新增至個別核准請求](assets/new-stage.png)

## 檢視AI檢閱者評分和意見反應

在提交具有AI檢閱者的檢閱和核准請求後的幾秒鐘，來自AI檢閱者的分數和意見可在「檔案摘要」面板中取得 — 即使其他參與者仍在檢閱和做出決定。

核准擁有者也會收到電子郵件，通知他們資產上已完成稽核。 在電子郵件中，按一下&#x200B;**前往檢閱**&#x200B;並檢視Workfront中的分數和意見反應。

AI檢閱者並非設計成檢閱和核准工作流程中的決策者。 它只會提供分數和建議，以讓資產符合指定的品牌需求。

如果資產不符合品牌指引，創意內容可以上傳新版本，而核准擁有者可以使用AI檢閱者建立第二個稽核和核准請求。

如需有關檢視分數和意見回饋的詳細資訊，請參閱[檢視AI檢閱者分數和意見回饋](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/view-ai-reviewer-feedback.md)。

