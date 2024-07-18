---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: 任務相依性回圈概觀
description: 將前置任務關係新增至任務時，您可能會遇到相依性回圈。 有關前置任務的資訊，請參閱前置任務概觀。
author: Alina
feature: Work Management
exl-id: 142e9637-841c-43d1-b297-e42c28a9e010
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# 任務相依性回圈概觀

將前置任務關係新增至任務時，您可能會遇到相依性回圈。 有關前置任務的資訊，請參閱[前置任務概觀](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)。

## 相依性回圈概述

當有兩個或多個任務彼此相依而需要完成時，就會發生相依性回圈。 如果Adobe Workfront建立相依性回圈，則不允許您在任務之間建立前置任務關係。

**範例：**&#x200B;任務2是任務1的前置任務，這表示您必須先完成任務2，才能開始處理任務1。

如果您嘗試將任務1變為任務2的前置任務，您會收到相依性回圈錯誤，因為您無法在任務2完成之前啟動任務1，但在任務1完成之前無法啟動任務2。

![](assets/dependency-loop-error-message-350x209.png)

![](assets/dependency-loop-in-task-list-nwe-350x97.png)

## 關於相依性回圈的考量事項

* 相依性回圈可能涉及兩個以上的工作。 有時候，您與前置任務關係連線之任務的父項中任何數量的父項都是建立相依性回圈的父項。
* 如果您嘗試讓父項成為子項的前置項，也會發生相依性回圈。
* 在相依性回圈的情況下，您無法儲存任務或專案。 為了修正相依性回圈，您必須重新評估錯誤訊息中所列任務之間的前置任務關係，並移除衝突，然後才能儲存任務或專案。

 
