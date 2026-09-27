---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: 已移動或複製的任務或問題的自訂狀態
description: 將任務或問題移動或複製到其他專案時，任務或問題的某些狀態可能會更新，以符合目標專案群組使用的狀態。
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 4bd9b89d-9c66-4af7-97bf-f9518ad55d7c
TQID: 'https://experienceleague.adobe.com/GzG3KBfUw05edjA0DVRtODyGprG2mKVjOuUV2L5eWto'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
  - id: 254442ca-6997-5cfa-963e-f420870aea53
    internal-label: People Teams and Groups
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 0%
---
# 已移動或複製之任務或問題的自訂狀態

將任務或問題移動或複製到其他專案時，任務或問題的某些狀態可能會更新，以符合目標專案群組使用的狀態。 這取決於該群組中是否存在具有相同索引鍵的狀態：

* 如果任務或問題上的狀態與目的地專案群組使用的狀態具有相同的索引鍵，則任務或問題上的狀態會維持不變。

  如果這兩種狀態的標籤不符，任務或問題上的狀態會繼承目標專案群組使用的狀態標籤。

* 如果任務或問題中的狀態與目的地專案群組中的對等狀態沒有相同的索引鍵，則任務或問題中的狀態會變更為目的地專案群組中的對等預設狀態。

如需有關狀態金鑰的資訊，請參閱[建立或編輯群組狀態](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md)。
