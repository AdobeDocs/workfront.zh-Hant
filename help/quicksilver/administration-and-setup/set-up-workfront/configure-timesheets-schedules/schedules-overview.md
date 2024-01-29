---
user-type: administrator
content-type: overview
product-area: system-administration;timesheets
keywords: user，schedule
navigation-topic: configure-timesheets-and-schedules
title: 排程總覽
description: 您可以使用排程來定義您的工作週。 您可以將排程與使用者或專案建立關聯。 這允許 [!DNL Adobe Workfront] 以計算時間表和使用者可用性。 如需指示，請參閱建立排程。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 02350860-f997-4a76-8aec-c6c813d58e2d
source-git-commit: 32da139d7385e05436a669bdc6f36b71ad83c8d2
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 0%

---

# 排程總覽

<!-- Audited: 1/2024 -->

您可以使用排程來定義您的工作週，並將排程與使用者或專案相關聯。 這允許 [!DNL Adobe Workfront] 以計算時間表和使用者可用性。 如需指示，請參閱 [建立排程](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

在Workfront中使用排程時，請考慮下列事項：

* 此 [!DNL Workfront] 管理員會識別排程中組織的作業時數。

  同樣地，群組管理員可以識別由他們管理的群組所管理之排程的作業時數。 如需群組管理員的詳細資訊，請參閱 [群組管理員](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

  例如，排程可定義為：星期一至星期五、上午8點至下午5點，以及午飯休息一小時。

* [!DNL Workfront] 使用排程來判斷工作日開始和結束的時間。

  這不會妨礙使用者在中工作或完成工作 [!DNL Workfront] 超出正常營業時間。 一般而言，您不需要建立新的排程或排程例外來聚焦於晚上計畫的工作。

  同樣地，貴組織可能有彈性工作日抵達時間。 您可能有一組員工於上午8點到達，而另一組員工於上午9點到達。 如果群組具有類似或相同的排程，則不需要為每個群組建立唯一的排程。 但是，如果群組擁有截然不同的排程，則其使用者應該與唯一排程相關聯。 員工瞭解指派是否要在下午5點完成，這表示工作必須在營業日結束前完成，無論他們何時上班。

* 建議您為與組織相關聯的每個時區建立個別的時程表。

  您可以為每個排程指派特定時區，以確保為在不同時區工作的使用者適當地排程工作。

* 此 [!DNL Workfront] 使用者或專案未與排程關聯時，預設排程用於時間表計算。

  預設排程隨附於 [!DNL Workfront] 系統，而且無法刪除，除非以您建立的新排程取代。

* 除了計算時間表， [!DNL Workfront] 使用排程來計算使用者可用性。

  >[!IMPORTANT]
  >
  >[!DNL Workfront] 使用使用者或專案排程來決定資源規劃工具中的資源可用性。 要使用哪個排程取決於 [!DNL Workfront] 管理員已為 [!UICONTROL 計算資源可用性，使用] 設定。 如需有關「資源管理」設定的資訊，請參閱 [設定資源管理喜好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## 排程階層

如果任務指派給與排程相關聯的使用者，並駐留在與第二排程相關聯的專案上，則您至少有2個排程可能套用至您的時間表計算。

>[!IMPORTANT]
>
>[!DNL Workfront] 僅在以下情況下使用使用者的排程： [!UICONTROL 計算資源可用性，使用] 設定已設為 [!UICONTROL 使用者的排程] 在 [!UICONTROL 資源管理] 區域 [!UICONTROL 設定]. 關於如何 [!UICONTROL 計算資源可用性，使用] 設定會影響用於「資源管理」的排程，請參閱 [設定資源管理喜好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

存在多個排程時，系統使用排程的順序為：

* 將使用者指派給任務時， [!DNL Workfront] 使用使用者的排程來計算任務的時間表。 這也包括使用者的個人時間。 專案的排程會被忽略。

  如需個人時間的詳細資訊，請參閱 [設定個人休假](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

* 當多個使用者被指派到一個任務，且使用者在該任務的時間範圍內具有不同的排程時， [!DNL Workfront] 會使用以下其中一個排程，如 [!UICONTROL 專案偏好設定] 區域 [!UICONTROL 設定]：

   * 被指定為主要受指派者的使用者的排程
   * 與專案關聯的排程。

     如需有關專案偏好設定的詳細資訊，請參閱 [設定全系統專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* 如果指派給任務的使用者沒有排程，或任務僅指派給工作角色、專案團隊或未指派， [!DNL Workfront] 使用專案排程進行時間表計算。
* 如果指派給任務的使用者沒有排程，或任務僅指派給工作角色、團隊或未指派，並且專案沒有排程，則 [!DNL Workfront] 使用系統中指定為時間表計算預設排程的排程。

  ![](assets/default-schedule.png)

## 共同作業位置 [!DNL Workfront] 跨時區

有關使用排程協助使用者在中共同作業的資訊 [!DNL Workfront] 跨越時區，請參見 [跨時區工作](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).
