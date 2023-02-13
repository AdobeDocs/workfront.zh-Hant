---
user-type: administrator
content-type: overview
product-area: system-administration;timesheets
keywords: 使用者，排程
navigation-topic: configure-timesheets-and-schedules
title: 排程概觀
description: 您可以使用排程來定義工作周。 您可以將排程與使用者或專案建立關聯。 這允許 [!DNL Adobe Workfront] 計算時間表和用戶可用性。 如需指示，請參閱建立排程。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 02350860-f997-4a76-8aec-c6c813d58e2d
source-git-commit: 9f7f8a50bb805b1d6845df79ecffaa329d5abc26
workflow-type: tm+mt
source-wordcount: '749'
ht-degree: 0%

---

# 排程概觀

您可以使用排程定義工作周，並將排程與使用者或專案建立關聯。 這允許 [!DNL Adobe Workfront] 計算時間表和用戶可用性。 如需指示，請參閱 [建立排程](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

在Workfront中使用排程時，請考量下列事項：

* 此 [!DNL Workfront] 管理員在計畫中標識組織的操作小時數。

   同樣，組管理員也可以確定由他們管理的組管理的調度的運行時間。

   如需群組管理員的詳細資訊，請參閱 [群組管理員](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

   例如，排程可定義為：星期一到星期五，上午8:00至下午5:00，午餐休息1小時。

* [!DNL Workfront] 使用計畫來確定工作日的開始和結束時間。

   這不會防止使用者在 [!DNL Workfront] 不在正常工作時間。 通常，不必建立新計畫或計畫例外，即可將精力集中在晚上計畫的工作上。

   同樣地，貴組織的工作日到達時間也可能靈活。 您可能有一組員工在上午8點到達，另一組員工在上午9點到達。 如果群組具有類似或相同的排程，則不需要為每個群組建立唯一排程。 但如果群組的排程大幅不同，則其使用者應與不重複排程相關聯。 員工知道，是否要在下午5點完成分配，這意味著工作必須在工作日結束前完成，而不管他們何時進入工作。

* 建議您為與組織相關聯的每個時區建立個別排程。

   您可以為每個排程指派特定時區，以確保為在不同時區工作的使用者適當排程工作。

* 此 [!DNL Workfront] 當使用者或專案未與排程建立關聯時，時間軸計算會使用預設排程。

   預設排程會隨您 [!DNL Workfront] 系統和無法刪除，除非它已被您建立的新計畫替換。

* 除了計算時間表外， [!DNL Workfront] 使用計畫來計算用戶可用性。

   >[!IMPORTANT]
   >
   >[!DNL Workfront] 使用用戶或項目計畫來確定資源計畫員中的資源可用性。 使用的排程取決於 [!DNL Workfront] 為選擇的管理員 [!UICONTROL 使用計算資源可用性] 設定。 有關資源管理設定的資訊，請參見 [配置資源管理首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## 排程的階層

如果將任務分配給與某個計畫關聯的用戶，並駐留在與第二個計畫關聯的項目上，則您至少有2個計畫可能應用於時間軸計算。

>[!IMPORTANT]
>
>[!DNL Workfront] 僅在 [!UICONTROL 使用計算資源可用性] 設定設為 [!UICONTROL 使用者的排程] 在 [!UICONTROL 資源管理] 區域 [!UICONTROL 設定]. 如需 [!UICONTROL 使用計算資源可用性] 設定會影響用於資源管理的計畫，請參閱 [配置資源管理首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

存在多個調度時系統使用調度的順序是：

* 將用戶分配給任務時， [!DNL Workfront] 使用用戶的計畫來計算任務的時間軸。 這也包括使用者的個人時間。 會忽略專案的排程。

   有關個人時間的詳細資訊，請參閱 [在中配置個人休假時間 [!DNL Adobe Workfront]](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

* 如果為任務分配了多個用戶，並且在任務的時間範圍內用戶具有不同的計畫， [!DNL Workfront] 會使用下列其中一個排程，定義於 [!UICONTROL 專案偏好設定] 區域 [!UICONTROL 設定]:

   * 指定為主要受託人的用戶的計畫
   * 與項目關聯的計畫。

      如需專案偏好設定的詳細資訊，請參閱 [配置系統範圍的項目首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* 如果分配給任務的用戶沒有計畫，或者該任務僅分配給作業角色、團隊或未分配， [!DNL Workfront] 將項目計畫用於時間軸計算。
* 如果分配給任務的用戶沒有計畫，或者該任務僅被分配給作業角色、團隊或未分配，並且項目沒有計畫，則 [!DNL Workfront] 在系統中將調度指定為時間線計算的預設調度。

   ![](assets/default-schedule.png)

## 協作於 [!DNL Workfront] 跨時區

有關使用計畫幫助用戶協作的資訊 [!DNL Workfront] 跨時區，請參閱 [跨時區工作](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).
