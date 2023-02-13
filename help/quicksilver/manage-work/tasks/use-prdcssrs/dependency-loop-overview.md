---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: 任務依賴環概述
description: 將前置關係添加到任務時，您可能會遇到相依性循環。 有關前置任務的資訊，請參閱前置任務概覽。
author: Alina
feature: Work Management
exl-id: 142e9637-841c-43d1-b297-e42c28a9e010
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 0%

---

# 任務依賴環概述

將前置關係添加到任務時，您可能會遇到相依性循環。 有關前置任務的資訊，請參閱 [任務前置任務概述](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## 相依性回圈概觀

當您有兩個或多個彼此相依的任務要完成時，相依性循環便會發生。 Adobe Workfront建立相依性回圈時，不允許您在任務之間建立前置關係。

**範例：** 任務2是任務1的前身，這意味著您必須完成任務2，才能開始處理任務1。

如果嘗試將任務1設定為任務2的前置任務，則會出現依賴環錯誤，因為在任務2完成之前，不能啟動任務1，但在任務1完成之前，無法啟動任務2。

![](assets/dependency-loop-error-message-350x209.png)

![](assets/dependency-loop-in-task-list-nwe-350x97.png)

## 相依性回圈的考量事項

* 相依性回圈可能涉及兩個以上的工作。 有時，您與前置關係連接的任務的父項數，都是建立相依環的父項數。
* 如果您嘗試將父代設為子代的前身，也會發生相依性循環。
* 如果是相依性循環，則無法儲存任務或專案。 為了修復相依性循環，您必須重新評估錯誤消息中列出的任務之間的前置關係並刪除衝突，然後才能保存任務或項目。

 
