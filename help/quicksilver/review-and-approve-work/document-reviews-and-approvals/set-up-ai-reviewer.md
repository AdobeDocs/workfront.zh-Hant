---
product-area: documents
navigation-topic: approvals
title: 建立AI檢閱者
description: 在Workfront中設定至少一個品牌後，您可以建立多個AI稽核者，然後將其指派給核准範本和個別稽核及核准請求。
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
hide: true
exl-id: 4673049e-119e-4315-95f0-f10d8b286856
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/sfM3OtA-DVqywr3Up8VGjcycLRs5WtF22dcpXzRlnvQ
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
  - id: c10f2e93-7a58-4212-aa24-684c265ebe76
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 290
ht-degree: 8%

---

# 建立AI檢閱者

>[!NOTE]
>
>此功能目前處於Beta測試階段。

在Workfront中設定至少一個品牌後，您可以建立多個AI稽核者，然後將其指派給核准範本和個別稽核及核准請求。


## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 封裝</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>標準</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是系統管理員。</p></td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

開始之前，您必須在Workfront中設定影像品牌指導方針。 如需詳細資訊，請參閱[建立和管理內容檢閱者的品牌](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md)。

## 新增AI檢閱者

>[!NOTE]
>
>AI檢閱者並非設計成檢閱和核准工作流程中的決策者。 它只會提供分數和建議，以讓資產符合指定的品牌需求。

若要新增內容檢閱者：

{{step-1-to-setup}}

1. 在左側面板中，移至&#x200B;**檢閱和核准** > **AI檢閱者**。
1. 按一下&#x200B;**新增**。
1. 為檢閱者命名。
1. 選取&#x200B;**品牌**。
1. 在&#x200B;**指引型別**&#x200B;下拉式功能表中選取下列其中一項：
   * **影像**： AI檢閱者會根據您在Workfront中設定的影像品牌指導方針檢閱資產。
   * **品牌聲音**： AI檢閱者會根據您在Workfront中設定的品牌聲音准則檢閱資產。
1. 按一下「**建立**」。

   建立AI稽核者後，使用者可以將AI稽核者新增至核准範本或個別核准。

   如需詳細資訊，請參閱

   * [建立檔案的核准工作流程範本](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)
   * [建立檔案核准工作流程](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)
