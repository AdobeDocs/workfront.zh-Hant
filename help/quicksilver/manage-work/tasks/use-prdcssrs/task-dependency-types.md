---
content-type: overview;reference
product-area: projects
navigation-topic: use-predecessors
title: 任務相關性類型概述
description: 相依性類型是指任務之間的前置關係。 它們定義從屬任務何時可以根據其前身的開始或結束開始或結束。
author: Alina
feature: Work Management
exl-id: 30d1c60d-0632-4a32-b7e7-a9f8e81bf727
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# 任務相關性類型概述

相依性類型是指任務之間的前置關係。 它們定義從屬任務何時可以根據其前身的開始或結束開始或結束。

>[!IMPORTANT]
>
>Adobe Workfront不會根據相依性類型限制相依任務的開始或結束，除非強制執行前置關係。 有關強制前置任務的資訊，請參閱 [強制前置作業](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

在任務之間建立此關係時，必須指定前置關係的「相依性類型」(Dependency Type)。

有關前置任務的詳細資訊，請參閱 [任務前置任務概述](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

以下是Workfront相依性類型：

* **完成開始(fs)**:必須先完成前置任務，然後才能啟動從屬任務。 這是預設的相依類型，在未指定其他相依類型時使用。
* **完成完成(ff)**:前置任務必須在從屬任務完成之前完成。
* **開始(ss)**:必須先啟動前置任務，然後才能啟動從屬任務。 除非前置任務至少已啟動，否則不能啟動從屬任務。
* **開始完成(sf)**:前置任務必須在從屬任務完成之前啟動。 您可以在前置任務開始之前啟動從屬任務，但除非前置任務啟動，否則無法完成它。
* **計畫啟動(sd)**:這將任務安排為「完成 — 開始」，但實際執行類型是「完成 — 完成」。 使用此功能時，將安排從屬任務在前置任務完成後啟動。 但是，強制執行使得相依任務可以隨時啟動，但在前置任務完成之前無法完成。
