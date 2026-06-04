---
content-type: overview;reference
product-area: projects
navigation-topic: use-predecessors
title: 作業相依性型態概要
description: 相依性型別是指任務之間的前置任務關係。 它們根據前置任務的開始或完成來定義相依任務何時可以開始或完成。
author: Alina
feature: Work Management
exl-id: 30d1c60d-0632-4a32-b7e7-a9f8e81bf727
TQID: https://experienceleague.adobe.com/AioKERGt0FLv1eBE5-evwa2d35fItwknWI-ZouBECSo
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 322
ht-degree: 0%

---

# 作業相依性型別的概要

<!-- Audited: 12/2023 -->

相依性型別是指任務之間的前置任務關係。 它們根據前置任務的開始或完成來定義相依任務何時可以開始或完成。

>[!IMPORTANT]
>
>Adobe Workfront不會根據相依性型別限制相依性任務的開始或完成，除非已強制執行前置任務關係。 如需強制前置任務的相關資訊，請參閱[強制前置任務](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md)。

當您在任務之間建立此關係時，必須指定前置任務關係的相依性型別。

如需前置任務的詳細資訊，請參閱[前置任務概觀](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)。

以下是Workfront相依性型別：

* **完成 — 開始(fs)**：前置任務必須先完成，相依任務才能開始。 這是預設的相依性型別，在未指定其他相依性型別時使用。
* **完成 — 完成(ff)**：前置任務必須先完成，相依任務才能完成。
* **開始 — 開始(ss)**：前置任務必須先開始，相依任務才能開始。 除非前置任務至少已開始，否則您無法啟動相依任務。
* **開始 — 完成(sf)**：前置任務必須先開始，相依任務才能完成。 您可以在前置任務開始之前開始相關任務，但除非前置任務開始，否則您無法完成它。
* **已排程 — 開始(sd)**：這會將工作排程為「完成 — 開始」，但實際強制型別是「完成 — 完成」。 使用此項時，相依任務會排定在前置任務完成後開始。 但是，強制會讓依存性任務隨時開始，但在前置任務完成之前無法完成。

>[!NOTE]
>
>「相依性型別」的縮寫用於工作清單中，以定義前置任務關係。 如需詳細資訊，請參閱[前置任務概觀](/help/quicksilver/manage-work/tasks/use-prdcssrs/predecessors-overview.md)中[工作清單](/help/quicksilver/manage-work/tasks/use-prdcssrs/predecessors-overview.md#examples-of-predecessor-values-in-a-task-list)的前置任務值範例。

