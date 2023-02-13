---
product-area: projects
navigation-topic: manage-issues
title: 自動將問題狀態從「等待反饋」更新為「正在進行」
description: 當問題的主要聯繫人通過更新欄位（包括自定義欄位）或添加評論來更新問題時，問題狀態將自動更新為「正在進行」。
author: Alina
feature: Work Management
exl-id: f94bb644-910f-4b46-80fd-fecbdf9cb18a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 0%

---

# 自動將問題狀態從「等待反饋」更新為「正在進行」

當問題的主要聯繫人通過更新欄位（包括自定義欄位）或添加評論來更新問題時，問題狀態將自動更新為「正在進行」。

為了進行此自動狀態變更，需要下列項目：

* 必須透過請求佇列輸入問題。

   有關建立請求隊列的資訊，請參閱 [建立和管理請求隊列](../../../manage-work/requests/create-and-manage-request-queues/create-manage-request-queues.md) 區段。 如需建立請求的詳細資訊，請參閱 [建立及提交Adobe Workfront請求](../../../manage-work/requests/create-requests/create-submit-requests.md).

* 請求佇列中的「佇列詳細資料」必須具備下列設定：
   * **當有人提出要求時，會自動授予** 設為 **貢獻存取**
   * **更改狀態** 在「進階設定」下選取

   ![隊列詳細資訊提供Contribute訪問權，並且選擇更改狀態。](assets/queuedetails-contributeaccess-changestatus.png)

   如需「佇列詳細資料」的詳細資訊，請參閱 [建立請求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

* 問題必須處於「等待反饋」狀態。
* 系統級別的問題必須有等待反饋(AWF)狀態。

   有關係統級狀態的詳細資訊，請參閱 [建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
