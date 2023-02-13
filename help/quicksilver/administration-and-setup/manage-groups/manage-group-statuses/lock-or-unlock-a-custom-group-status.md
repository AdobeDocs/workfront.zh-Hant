---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: 鎖定和解除鎖定的群組狀態
description: 鎖定群組的自訂狀態是確保群組及其子群組中的人員在工作流程中使用相同程式的一種方式。 群組狀態鎖定後，群組和下層群組中的所有使用者都能使用該狀態。 雖然您(或Workfront管理員)可以編輯或刪除您鎖定的狀態，但下面子組的管理員無法編輯或刪除這些組。 反之，解鎖群組的自訂狀態，讓較低子群組的管理員有更大的彈性來管理其工作流程。 他們可以更改解鎖狀態的屬性或刪除其組的屬性。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 3463e4cb-7336-49b7-b81a-c2acef72f61d
source-git-commit: d67de32fcbe4706cf8a1fc6f5bb8ec9d08b07119
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---

# 鎖定和解除鎖定的群組狀態

鎖定群組的自訂狀態是確保群組及其子群組中的人員在工作流程中使用相同程式的一種方式。 群組狀態鎖定後，群組和下層群組中的所有使用者都能使用該狀態。 雖然您(或Workfront管理員)可以編輯或刪除您鎖定的狀態，但下面子組的管理員無法編輯或刪除這些組；它們只能更改「狀態」清單中的顯示順序。

相反，解鎖組的自定義狀態使較低子組的管理員能夠更靈活地管理其組中使用的唯一工作流。 組狀態解除鎖定後，下子組的管理員可以更改其屬性或刪除這些子組的屬性。

>[!IMPORTANT]
>
>如果在自定義狀態解除鎖定後鎖定任意時間段，則狀態設定將替換下層子組中的組管理員所做的設定。 在鎖定狀態時，這些管理員無法修改或刪除其群組的狀態。

有關鎖定或解鎖組狀態的說明，請參閱 [建立或編輯群組狀態](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

您可以在群組核准程式中使用鎖定和解除鎖定的狀態。 如果您建立了組批准進程，且組狀態處於未鎖定狀態，則用戶可以將批准進程附加到與該組關聯的任何項目、任務或問題。

