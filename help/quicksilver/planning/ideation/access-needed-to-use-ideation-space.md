---
title: 使用構思空間所需的存取許可權
description: Adobe Workfront規劃現在提供另一項功能，可在您啟動行銷活動之前加以構想。 運用AI的強大功能，將資料和直接輸入轉換為實際的計畫，並為團隊提供明智的起點，而不是具有Adobe Ideation空間的空白頁面。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 02ea2cad43b1064e30a7356feaa194f98d448092
workflow-type: tm+mt
source-wordcount: '589'
ht-degree: 1%

---


# 使用構思空間所需的存取許可權

<span class="preview">此頁面上的資訊是指尚未普遍提供的功能。 它只能做為&#x200B;**創意空間Beta**&#x200B;程式的一部分。</span>

<span class="preview">如需詳細資訊，請參閱[開始使用Adobe Workfront Planning的構思空間](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md)。</span>


{{planning-important-intro}}

Adobe Workfront規劃現在提供另一項功能，可在您啟動行銷活動之前加以構想。 運用AI的強大功能，將資料和直接輸入轉換為實際的計畫，並為團隊提供明智的起點，而不是具有Adobe Ideation空間的空白頁面。

本文說明從Workfront Planning存取Ideation Space所需的存取權和許可權。

如需創意力空間的一般資訊，請參閱[開始使用Adobe Workfront計畫的創意力空間](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md)。

## 產品需求

創意力空間不是獨立產品。 它需要Workfront Planning套件，而且只能從Workfront Planning存取。 此外還需要其他產品。

貴組織必須購買下列產品的套件，才能存取創意空間：

* 除了Planning套件之外的Adobe Workfront Workflow套件

  或

  Adobe Workfront Planning已購買作為獨立產品。
* Adobe GenStudio for Performance Marketing授權

  >[!TIP]
  >
  >需要GenStudio for Performance Marketing才能存取正確的字型權益。


<!--only required for closed beta:* An Adobe Customer Journey Analytics license that includes campaign tracking-->

## Workfront Planning存取層級需求

創意力空間存取是在Workfront中設定。

您的Workfront存取層級必須包含下列專案，才能存取創意空間：

* 標準工作流程授權，指貴公司購買計畫套件以外的工作流程套件。
* 標準Planning授權，當您的公司與Workflow和Planning套件一起購買時，或Workfront Planning作為獨立產品時。
* 您必須取消選取存取層級的「設定其他限制」區段中的「停用構思空間」設定。<!--***********check the UI for this***********-->

## Workfront規劃許可權需求

每個Planning記錄都連線到Ideation space中的一個摘要。

創意空間摘要許可權繼承自Workfront Planning記錄許可權。<!--not sure if this is right, because now you can share the ideation with others??-->

您必須在Planning中擁有記錄型別的「管理」許可權才能建立記錄，才能在創意空間建立或編輯記錄。

對記錄具有「檢視」許可權的Planning使用者可檢視記錄的創意空間。

下表顯示Workfront Planning記錄許可權與Ideation Space簡介許可權之間的連線：

| Planning記錄層級許可權 | 創意力空間簡短層級許可權 |
|---|---|
| 管理記錄的許可權 | 可以在記錄的構思空間中建立簡報 |
| 檢視記錄的許可權 | 可以在構思空間中讀取該記錄的摘要，但無法修改它 |

## 創意力空間許可權

<!--this is also duplicated in the intro of the Share an ideation space article-->

計畫許可權會傳輸到記錄的創意空間。

此外，您可以授予其他使用者使用構思空間的許可權，並為其新增構思。

考慮以下事項：

* 創意力建立者一律擁有其創意力的「編輯者」許可權。

* 您必須擁有創意力空間的編輯器許可權，才能建立摘要並將其匯出至其他應用程式。

以下是創意空間許可權及其所提供的功能：

| 創意力空間許可權 | 功能 |
|---|---|
| 編輯者 | 可以編輯、下載及共用創意力空間 |
| 評論者 | 可以在創意力空間上檢視和註解 |
| 檢視者 | 可檢視創意力空間 |

如需共用創意力空間的詳細資訊，請參閱[共用創意力空間](/help/quicksilver/planning/ideation/share-the-ideation-space.md)。

<!--there is no additional setup for Workfront layout template assignment because Contributors an below cannot access Ideation space; only Standard users-->


<!-- 
Not sure if this is needed. Maybe all orgs have IMS for all Adobe?? - asking Becky: 

## Org/IMS-level entitlements

Beyond Planning access itself, a customer's IMS Org needs specific entitlements for the full Ideation space experience to work:

| Requirement | Type | Why it matters |
|---|---|---|
| IMS Org with Workfront Planning | Org requirement | Baseline product access |
| IMS Org with GenStudio PEM | Org requirement | Provides the font entitlements and storage needed to use the Ideation space |
| Fonts entitlement | Entitlement | Missing entitlement can block the full Ideation space experience |
| Adobe Cloud Platform / document storage entitlement | Entitlement | Existing documentation indicates users may be able to reach ideation entry points but fail during actual usage if storage-related entitlements are missing |

Historically, some customer teams relied on GenStudio (GenS) provisioning without realizing they could use the Ideation space directly — provisioning conversations should confirm both Planning and GenStudio PEM entitlements are explicitly set up for the Ideation space, not just assumed via GenS.
-->



<!--
From Claude: Internal information, not customer-facing: 

The permissions and entitlement model below reflects what was documented and confirmed as of the Closed Beta (through Aug 2026). Internal teams were still finalizing a formal access-model document and access-level definitions at this time, so treat this as the current best understanding rather than a final spec — confirm against the latest internal documentation before publishing externally.

## Practical checklist for provisioning a customer

1. Confirm the customer has Workfront Planning (via Workflow+Planning or Planning standalone).
2. Confirm the customer's IMS Org has GenStudio PEM entitlements provisioned (not just assumed).
3. Confirm font and document-storage entitlements are active — test actual usage, not just entry-point visibility.
4. Confirm the "strategic ideation" product is enabled at the org level.
5. During Closed Beta, confirm the user-level feature flag is set for named ideation users.
6. Confirm the target users have **create** (not just view) access to the records they need to ideate on.
7. If the Coworker integration inside the Ideation space is in scope, verify its availability separately.

## Packaging

| Detail | Description |
|---|---|
| Included with Workfront Planning | Yes |
| Standalone option | Can also be launched as its own surface |
| Agent platform | Runs within the Adobe Agent Orchestrator |
| Billing | Monetized through Adobe's AI-credits framework |
-->

<!--

Original Claude write-up, in addition to the info above:

## Baseline product requirement

The Ideation space isn't a standalone purchase — you need **Workfront Planning** to access it, through either:

- Adobe Workfront Workflow with a Workfront Planning package, or
- Adobe Workfront Planning as a standalone product

If your org has Workfront Planning, it has the Ideation space too. The Ideation space can't exist without Planning.

For the Closed Beta and Open Beta, the Ideation space is available only to Planning and GenStudio (GenS) customers.

## Customer-level entry requirements (Closed Beta)

To participate in the Closed Beta, customers needed to meet these criteria:

- An active Adobe Customer Journey Analytics (CJA) deployment with campaign tracking in place
- Multi-channel campaigns with a repeatable planning process
- Active use of Workfront Planning for marketing operations
- At least one identified strategist or ideation user who will be the primary Ideation space user

## Org- and user-level enablement

- Workfront surfaces the Ideation space integration to users only after a Workfront administrator enables the **strategic ideation** product at the org level.
- During the Closed Beta, a user-level feature flag also controls access, so org-level enablement alone isn't enough.
- For Open Beta, access is expected to move to an opt-in model, where customers actively configure themselves in, rather than opt-out.

## Record-level permissions

Your Ideation space permissions come from your Workfront Planning record permissions — there's no separate permission system layered on top:

- If you can create a record in Planning, you can also create a canvas in the Ideation space. Any Planning license is sufficient for this.
- If you have read-only access to a record, you have read-only access to the canvas connected to that record.
- If you only have view access to an existing record, you can't open the Ideation space from it. Workfront shows an "Insufficient permissions" message instead.
- Each canvas is related to exactly one record.

>[!NOTE]
>As of August 2026, the team was still defining discrete access levels for the Ideation space. These are expected to include, at minimum, Can read, Can view, and Can create.

## Org and IMS-level entitlements

Beyond Planning access, your organization's IMS Org needs specific entitlements for the Ideation space to work fully.

| Requirement | Type | Why it matters |
|---|---|---|
| IMS Org with Workfront Planning | Org requirement | Baseline product access |
| IMS Org with GenStudio PEM | Org requirement | Provides the font entitlements and storage needed to use the Ideation space |
| Fonts entitlement | Entitlement | A missing entitlement can block the full Ideation space experience |
| Adobe Cloud Platform or document storage entitlement | Entitlement | Users may be able to reach Ideation space entry points but fail during actual use if storage-related entitlements are missing |

>[!IMPORTANT]
>When you provision a customer, confirm that both the Planning and GenStudio PEM entitlements are set up specifically for the Ideation space. Don't assume that GenStudio (GenS) provisioning alone includes Ideation space access.

## Content-sharing and abuse controls

Because the Ideation space lets you create content and share it with other users through Adobe systems, a **Report Abuse** capability is planned as a requirement before General Availability (GA). Workfront needs this roughly one month ahead of GA to support Adobe's platform license agreement process. This capability may reuse the existing Report Abuse functionality from Adobe Horizon rather than being built from scratch.

## Coworker (conversational AI) access

Access to the **Coworker** integration inside the Ideation space, the conversational right-rail assistant, is being rolled out separately from core Ideation space and Planning access:

- As of mid-August 2026, Coworker access wasn't yet generally available for customer testing.
- By August 17, 2026, Coworker was available inside the Ideation space for internal use, but still being refined.
- If you're documenting or testing the Coworker integration inside the Ideation space specifically, verify current availability separately. Don't assume it's included automatically with standard Planning or Ideation space provisioning.

For more information, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

-->
