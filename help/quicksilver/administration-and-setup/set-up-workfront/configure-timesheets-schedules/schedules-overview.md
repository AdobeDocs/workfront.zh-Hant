---
user-type: administrator
content-type: overview
product-area: system-administration;timesheets
keywords: user，schedule
navigation-topic: configure-timesheets-and-schedules
title: 排程總覽
description: 您可以使用排程來定義您的工作週。 您可以將排程與使用者或專案建立關聯。 這可讓 [!DNL Adobe Workfront] 計算時間表和使用者可用性。 如需指示，請參閱建立排程。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 02350860-f997-4a76-8aec-c6c813d58e2d
source-git-commit: ef7f5d00bd74feee5e06b935c4bb8a18ee8b08a8
workflow-type: tm+mt
source-wordcount: '864'
ht-degree: 0%

---

# 排程總覽

<!-- Audited: 1/2024 -->

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

您可以使用排程來定義您的工作週，並將排程與使用者或專案相關聯。 這可讓[!DNL Adobe Workfront]計算時間表和使用者可用性。 如需指示，請參閱[建立排程](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)。

在Workfront中使用排程時，請考慮下列事項：

* [!DNL Workfront]管理員會識別排程中組織的作業時數。

  同樣地，群組管理員可以識別由他們管理的群組所管理之排程的作業時數。 如需群組管理員的詳細資訊，請參閱[群組管理員](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md)。

  例如，排程可定義為：星期一至星期五、上午8點至下午5點，以及午飯休息一小時。

* [!DNL Workfront]會使用排程來判斷工作日的開始和結束時間。

  這不會妨礙使用者在正常營業時間以外於[!DNL Workfront]內工作或完成工作。 一般而言，您不需要建立新的排程或排程例外來聚焦於晚上計畫的工作。

  同樣地，貴組織可能有彈性工作日抵達時間。 您可能有一組員工於上午8點到達，而另一組員工於上午9點到達。 如果群組具有類似或相同的排程，則不需要為每個群組建立唯一的排程。 但是，如果群組擁有截然不同的排程，則其使用者應該與唯一排程相關聯。 員工瞭解指派是否要在下午5點完成，這表示工作必須在營業日結束前完成，無論他們何時上班。

* 建議您為與組織相關聯的每個時區建立個別的時程表。

  您可以為每個排程指派特定時區，以確保為在不同時區工作的使用者適當地排程工作。

* 當使用者或專案未與排程關聯時，[!DNL Workfront]預設排程用於時間表計算。

  預設排程隨附於您的[!DNL Workfront]系統，除非以您建立的新排程取代，否則無法刪除。

* 除了計算時間表之外，[!DNL Workfront]還會使用排程來計算使用者可用性。

  >[!IMPORTANT]
  >
  >[!DNL Workfront]使用使用者或專案排程來決定資源規劃工具中的資源可用性。 使用哪個排程取決於管理員為[!UICONTROL 使用]計算資源可用性設定選取的[!DNL Workfront]專案。 如需有關資源管理設定的資訊，請參閱[設定資源管理喜好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)。

## 排程階層

如果任務指派給與排程相關聯的使用者，並駐留在與第二排程相關聯的專案上，則您至少有2個排程可能套用至您的時間表計算。

>[!IMPORTANT]
>
>只有在[!UICONTROL 安裝程式]的[!UICONTROL 資源管理]區域中的[!UICONTROL 使用來計算資源可用性]設定設為[!UICONTROL 使用者的排程]時，[!DNL Workfront]才會使用使用者的排程。 如需[!UICONTROL 使用]計算資源可用性的設定如何影響用於資源管理的排程，請參閱[設定資源管理喜好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)。

存在多個排程時，系統使用排程的順序為：


* 將一位使用者指派給任務時，根據您使用的環境，將出現以下情境：

   * 在生產環境中，[!DNL Workfront]會使用使用者的排程來計算任務的時間表。 這也包括使用者的個人時間。 專案的排程會被忽略。

     如需個人時間的詳細資訊，請參閱[設定個人休假](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md)。

   * <span class="preview">在預覽環境中，[!DNL Workfront]會使用下列其中一個排程，如[!UICONTROL 設定]的[!UICONTROL 專案偏好設定]區域中所定義：</span>

      * <span class="preview">指派給工作</span>的使用者排程
      * <span class="preview">與專案關聯的排程。</span>

* 當多個使用者被指派到一個任務，並且該使用者在該任務的時間範圍內具有不同的排程時，[!DNL Workfront]會使用以下其中一個排程，如[!UICONTROL 設定]的[!UICONTROL 專案偏好設定]區域中所定義：

   * 被指定為主要受指派者的使用者的排程
   * 與專案關聯的排程。

     如需有關專案偏好設定的詳細資訊，請參閱[設定全系統的專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

* 如果指派給任務的使用者沒有排程，或任務僅指派給工作角色、團隊或未指派，[!DNL Workfront]會使用專案排程進行時間表計算。
* 如果指派給任務的使用者沒有排程，或任務僅指派給工作角色、團隊或未指派，並且專案沒有排程，則[!DNL Workfront]會使用系統中指定為預設排程的排程來計算時間表。

  ![](assets/default-schedule.png)

## 跨時區[!DNL Workfront]中的Collaboration

如需使用排程協助使用者在[!DNL Workfront]中跨時區共同作業的資訊，請參閱[跨時區工作](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md)。
