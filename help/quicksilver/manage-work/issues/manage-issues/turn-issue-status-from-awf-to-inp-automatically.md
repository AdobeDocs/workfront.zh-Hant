---
product-area: projects
navigation-topic: manage-issues
title: 自動將問題狀態從等待意見更新為進行中
description: 當問題的主要聯絡人透過更新欄位（包括自訂欄位）或新增評論來更新問題時，問題狀態會自動更新為進行中。
author: Alina
feature: Work Management
exl-id: f94bb644-910f-4b46-80fd-fecbdf9cb18a
TQID: https://experienceleague.adobe.com/axgDUT8M6p79omHTSO8OrvM7qAM81AjG0Fug2JUl4ck
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 282
ht-degree: 0%

---

# 自動將問題狀態從等待回饋更新為進行中

<!--Audited: 109/2025-->

當問題的主要聯絡人透過更新欄位（包括自訂欄位）或新增評論來更新問題時，問題狀態會自動更新為進行中。

為了進行此自動狀態變更，需要下列專案：

* 必須使用請求佇列新增問題。

  如需有關建立請求佇列的資訊，請參閱[建立及管理請求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-manage-request-queues.md)區段。

  如需有關將請求提交至請求佇列的資訊，請參閱[建立和提交Adobe Workfront請求](../../../manage-work/requests/create-requests/create-submit-requests.md)。

* 請求佇列中的「佇列詳細資料」必須有下列設定：
   * **某人提出要求時，自動授予**&#x200B;設定為&#x200B;**貢獻存取權**
   * 已選取&#x200B;**變更狀態**

  已選取![佇列詳細資料授予Contribute存取權和變更狀態。](assets/queuedetails-contributeaccess-changestatus.png)

  >[!IMPORTANT]
  >
  >  設定請求佇列時，您可以定義主要聯絡人對他們提交的問題具有的存取權。
  >
  >當您在設定請求佇列時取消選取「變更狀態」設定時，請記住，系統管理員始終有權變更問題的狀態，即使請求佇列設定中已取消選取「變更狀態」選項。

  如需佇列詳細資料的詳細資訊，請參閱[建立要求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)。

* 問題必須處於等待回饋狀態。
* 系統層級的問題必須具有「等待回饋」(AWF)狀態。

  如需系統層級狀態的詳細資訊，請參閱[建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)。
