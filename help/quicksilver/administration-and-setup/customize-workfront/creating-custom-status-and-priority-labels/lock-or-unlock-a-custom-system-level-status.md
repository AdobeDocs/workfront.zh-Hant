---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: 鎖定和解除鎖定系統級狀態
description: 鎖定自訂狀態是確保整個組織的人員在工作流程中使用相同程式的方法。 狀態鎖定後，系統中的所有用戶都可以使用它。 雖然您可以編輯或刪除，但群組管理員無法對群組進行編輯或刪除。 相反地，解鎖自訂狀態可讓群組管理員有更大的彈性，可管理其群組中使用的獨特工作流程。 他們可以更改解鎖狀態的屬性或刪除其組的屬性。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 0e58a1d6-5e0c-4445-a5ac-400dfd4c4948
source-git-commit: c70a10a920d32ad00a2e833b331c92a598902d21
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---

# 鎖定和解除鎖定系統級狀態

鎖定自訂狀態是確保整個組織的人員在工作流程中使用相同程式的方法。 狀態鎖定後，系統中的所有用戶都可以使用它。 雖然您可以編輯或刪除您鎖定的狀態，但群組管理員無法對其群組進行編輯或刪除；它們只能更改「狀態」清單中的顯示順序。

相反地，解鎖自訂狀態可讓群組管理員有更大的彈性，可管理其群組中使用的獨特工作流程。 狀態解除鎖定時，群組管理員可以變更其屬性或刪除其群組的屬性。

>[!IMPORTANT]
>
>如果在自定義狀態解除鎖定後鎖定任意時間段，則狀態的全系統設定將替換由組管理員進行的設定。 在鎖定狀態時，群組管理員無法修改或刪除其群組的狀態。

有關鎖定或解鎖系統級狀態的說明，請參見 [建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

## 核准程式中的解除鎖定狀態

您可以在系統批准過程中使用鎖定狀態和解鎖狀態。 如果您建立具有未鎖定系統狀態的系統批准進程，則系統中的用戶可以將批准進程附加到系統中的任何項目、任務或問題。

警告訊息會顯示在下列案例中，以協助您和您的使用者確定您了解下列案例的結果：

* 管理員解除鎖定在批准過程中使用的系統級狀態。 系統會發出警告，指出可能會刪除其群組的解除鎖定狀態，這會使群組成員無法針對指派給其群組的物件正確使用該核准程式。

* 用戶開始編輯使用解鎖狀態的批准進程。 訊息會提醒使用者解除鎖定狀態，讓他們評估重新鎖定或更換是否是個好主意。

* 對象上附加了具有未鎖定狀態的系統級批准進程，並且為分配給該對象的組刪除了該狀態。 當組成員進入對象的「批准」部分時，消息將說明無法為對象啟動批准進程。

您可以在群組核准程式中使用鎖定和解除鎖定的狀態。 如果您建立了組批准進程，且組狀態處於未鎖定狀態，則用戶可以將批准進程附加到與該組關聯的任何項目、任務或問題。