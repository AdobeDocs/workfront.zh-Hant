---
product-area: projects
navigation-topic: manage-issues
title: 自動將問題狀態從等待意見更新為進行中
description: 當問題的主要聯絡人透過更新欄位（包括自訂欄位）或新增評論來更新問題時，問題狀態會自動更新為進行中。
author: Alina
feature: Work Management
exl-id: f94bb644-910f-4b46-80fd-fecbdf9cb18a
source-git-commit: dc4b6dc284c59281206a457395765e634067ba91
workflow-type: tm+mt
source-wordcount: '281'
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
