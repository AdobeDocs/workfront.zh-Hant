---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: 鎖定和未鎖定的系統層級狀態
description: 鎖定自訂狀態是確保整個組織的人在其工作流程中使用相同流程的一種方法。 當狀態鎖定時，系統中的所有使用者都可以使用該狀態。 雖然您可以編輯或刪除它，但群組管理員無法為其群組執行此操作。 相反地，解鎖自訂狀態可讓群組管理員更靈活地管理其群組中所使用的獨特工作流程。 他們可以變更解除鎖定狀態的屬性，或刪除其群組的屬性。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0e58a1d6-5e0c-4445-a5ac-400dfd4c4948
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---

# 鎖定和未鎖定的系統層級狀態

鎖定自訂狀態是確保整個組織的人在其工作流程中使用相同流程的一種方法。 當狀態鎖定時，系統中的所有使用者都可以使用該狀態。 雖然您可以編輯或刪除您鎖定的狀態，但群組管理員無法為其群組執行此操作；他們只能變更其在「狀態」清單中的顯示順序。

相反地，解鎖自訂狀態可讓群組管理員更靈活地管理其群組中所使用的獨特工作流程。 解除鎖定狀態時，群組管理員可以變更其屬性，或為其群組刪除屬性。

>[!IMPORTANT]
>
>如果您在自訂狀態解除鎖定任何時間後將其鎖定，則您系統的狀態設定會取代群組管理員所做的設定。 當狀態為鎖定時，群組管理員無法修改或刪除其群組的狀態。

如需鎖定或解除鎖定系統層級狀態的指示，請參閱[建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)。

## 核准流程中的解鎖狀態

您可以在系統核准程式中使用鎖定和未鎖定狀態。 如果您建立的系統核准流程具有未鎖定的系統狀態，則整個系統的使用者可以將核准流程附加到系統中的任何專案、任務或問題。

警告訊息會顯示在下列案例中，以協助您和您的使用者確保您瞭解下列案例的結果：

* 管理員會解除鎖定核准流程中所使用的系統層級狀態。 訊息會警告，可能會刪除其群組的解除鎖定狀態，這會導致群組成員無法正確使用該核准流程來核准指派給其群組的物件。

* 使用者開始編輯使用已解鎖狀態的核准流程。 訊息會提醒使用者解除鎖定的狀態，讓使用者評估重新鎖定或取代會是很好的做法。

* 具有解鎖狀態的系統層級核准程式會附加至物件，且已針對指派給物件的群組刪除其狀態。 當群組成員前往物件的「核准」區段時，會出現一則訊息，說明無法為物件啟動核准流程。

您可以在群組核准程式中使用鎖定和未鎖定狀態。 如果您建立的群組核准流程具有未鎖定的群組狀態，則使用者可以將核准流程附加至與群組相關聯的任何專案、任務或問題。
