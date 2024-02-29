---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: 跨時區工作
description: 有助於瞭解如何 [!DNL Adobe Workfront] 會使用時區來計算物件的時間欄位，以及其他區域（例如電子郵件）的時間。
feature: Get Started with Workfront
exl-id: b6574165-a6dc-4694-a367-d98927abf1e3
source-git-commit: 246750d2a7a053d74df2ceb150f14fdb50f32ade
workflow-type: tm+mt
source-wordcount: '1081'
ht-degree: 0%

---

# 跨時區工作

<!-- Audited: 2/2024 -->

有助於瞭解如何 [!DNL Adobe Workfront] 會使用時區來計算下列專案：

* 物件的時間欄位
* 其他時間 [!DNL Workfront] 區域，例如自動化Workfront電子郵件

## 時區單位 [!DNL Workfront]

您在中看到的時間 [!DNL Workfront] 是根據您組織的時區設定 [!DNL Workfront] 例項和以取得您的使用者設定檔。 如果這兩個時區不同，您可能會看到您在中使用的不同區域和功能出現時間差異 [!DNL Workfront].

>[!NOTE]
>
>在附加到物件的自訂表單中，計算自訂欄位中的日期和時間陳述式會由世界協調時間(UTC)計算和儲存，而不是由針對您的組織執行個體和您的使用者設定檔設定的時區設定計算和儲存。 自訂表單中的計算會根據每位使用者的個別時區產生和顯示。

* [您組織的 [!DNL Workfront] 例項](#your-organization-s-workfront-instance)
* [您的使用者設定檔](#your-user-profile)

### 您組織的 [!DNL Workfront] 例項 {#your-organization-s-workfront-instance}

貴組織的時區 [!DNL Workfront] 執行個體通常設定在主辦公室的位置。 這會決定下列專案：

* 電子郵件中所顯示的時間產生者 [!DNL Workfront]
* 新新增使用者的時區(在 [!DNL Workfront] 管理員會根據使用者的工作位置為其設定不同的時區)

  如需這兩個範例的詳細資訊，請參閱 [設定系統的基本資訊](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

* 專案之覆寫收費率的開始或結束。 如需詳細資訊，請參閱 [覆寫專案層級的工作角色收費率](../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

### 您的使用者設定檔 {#your-user-profile}

您使用者設定檔中的時區應該為您工作的位置設定。 這會決定下列專案：

<!--
* The time shown in your outgoing [!DNL Workfront] email messages
[NOTE FROM LISA: Saeid that dates/times shown in emails are more complicated than how it is described in the article so we decided to comment out this line.]
-->
* 處理物件的時間，例如開始和結束時間

  如果將位於多個時區的使用者指派給物件， [!DNL Workfront] 會使用每個使用者設定檔中設定的時區，轉換相關每個人的物件時間。

  **範例：** 在您工作的東部標準時間(EST)區域中，您將工作設定為下午4:00，並將其指派給在太平洋標準時間(PST)區域工作的使用者。 對於這些使用者，開始時間顯示為下午1:00。 如果顯示為下午4:00，他們會延遲三個小時開始處理。

  如果物件建立者沒有注意到受指派人時區之間的差異，並在設定物件時間時進行必要的調整，或受指派人沒有注意到該差異，則當每個人都在物件上合作時，可能很難獲得正確的時機。

  **範例：** 您設定從東部時間上午9:00開始的一天任務，忘記任務上的一些使用者在PST區域工作。 對於他們，開始時間是上午6:00。 由於他們要到時間9:00 （您時間的中午）才會開始處理，因此任務會延遲三個小時開始和完成。

如需在使用者設定檔中設定時區的資訊，請參閱 [設定我的設定](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

關於如何 [!DNL Workfront] 管理員(或具有 [!UICONTROL 編輯] 存取使用者)可以在使用者設定檔中設定時區，請參閱 [編輯使用者設定檔](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## 如何讓使用者更輕鬆地跨時區工作

您可以透過多種方式協助使用者更輕鬆地在數個時區中工作：

* [使用時程表](#use-schedules)
* [在自訂表單中使用計算的時間欄位](#use-calculated-time-fields-in-a-custom-form)
* [在自訂表單中使用文字欄位而非日期欄位](#use-text-fields-instead-of-date-fields-in-a-custom-form)

### 使用時程表 {#use-schedules}

[!DNL Workfront] 管理員會為組織內的每個時區建立個別的時程表，以確保所有人都能適當地排程工作，無論他們身在何處。 管理員建立排程後，便可與特定專案和使用者建立關聯：

* **[!UICONTROL 專案]**：專案建立者可以選取個別專案的排程。 這會根據受指派人時區設定的工作時數，決定專案中任務的排程。
* **[!UICONTROL 使用者]**：A [!DNL Workfront] 管理員(或具有 [!UICONTROL 編輯] 存取使用者)可以在使用者設定檔中選取個別使用者的排程。

  此排程可能與專案排程不同。 例如，當有人在專案中建立任務，但尚未指派任何人給它時，該任務就會使用專案排程。 將使用者指派給任務時，任務會使用該使用者的排程。

  如果將多個使用者指派到一個任務，則系統會使用下列其中一項，如系統範圍專案偏好設定中所設定：

   * 任務主要擁有者的排程時區
   * 專案排程的時區。

  這可能會造成任務日期變更。

  **範例：** EST使用者會被指派給排程在早上9:00 PST （亦即EST中午）開始的一日工作。 由於EST使用者一天只剩下2個工作小時，因此任務完成日期會延長約6小時，直到下一個工作日。

  如需關於的資訊， [!UICONTROL 專案偏好設定] 區域 [!UICONTROL 設定]，請參閱 [設定全系統專案偏好設定](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

  如需將排程指派給專案或使用者的指示，請參閱 [建立排程](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

  如需排程中所設定時區如何影響下列專案分佈的資訊： [!UICONTROL 計畫時數] 在 [!UICONTROL 工作負載平衡器]，請參閱 [在中管理使用者配置 [!UICONTROL 工作負載平衡器]](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).


### 在自訂表單中使用計算的時間欄位 {#use-calculated-time-fields-in-a-custom-form}

您可以在自訂表單中使用一系列計算出的自訂欄位來顯示組織中使用者的目前時間，例如顯示多個城市中的時間的一列機場時鐘。 您可以為使用者工作的每個時區建立一個欄位，每個時區都會計算其時區的時間。

如需詳細資訊，請參閱 [新增計算資料至自訂表單](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)以及區段 [日期與時間計算自訂欄位](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md#date) 在文章中 [計算資料運算式的概觀](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

### 在自訂表單中使用文字欄位而非日期欄位 {#use-text-fields-instead-of-date-fields-in-a-custom-form}

如果您不想 [!DNL Workfront] 若要轉換您在物件中為不同時區的使用者設定的時間，您可以使用附加到物件的自訂表單中的文字欄位，而不是日期欄位。 如此一來，時間就會顯示您為專案中的每個人輸入的時間。

若您這麼做，建議您提醒表單的使用者計算其時區與您的時區之間的差異，以便他們決定工作應該開始與結束的時間。 您可以在自訂表單的指示或該欄位的工具提示中鍵入此資訊。 如需詳細資訊，請參閱 [新增自訂欄位至自訂表單](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md).
