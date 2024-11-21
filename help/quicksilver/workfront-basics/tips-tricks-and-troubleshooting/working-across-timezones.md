---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: 跨時區工作
description: 瞭解 [!DNL Adobe Workfront] 如何使用時區來計算物件的時間欄位，以及在其他區域（例如電子郵件）中的時間會很有幫助。
feature: Get Started with Workfront
exl-id: b6574165-a6dc-4694-a367-d98927abf1e3
source-git-commit: ef7f5d00bd74feee5e06b935c4bb8a18ee8b08a8
workflow-type: tm+mt
source-wordcount: '1252'
ht-degree: 0%

---

# 跨時區工作

<!-- Audited: 2/2024 -->

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在預覽環境中可供所有客戶使用。 每月發行至生產環境後，生產環境中為啟用快速發行的客戶也提供相同的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

瞭解[!DNL Adobe Workfront]如何使用時區來計算下列專案會很有幫助：

* 物件的時間欄位
* 其他[!DNL Workfront]區域(例如自動化Workfront電子郵件)的時間

>[!WARNING]
>
>如果您在我們提供的清單中找不到確切的時區，請尋找最接近您的時區，然後為您的執行個體更新該時區。
>
>此外，請考量類似的時區可能並不完全符合您的時區。
>
>例如，某些國家或地區可能會觀察到日光節約時間，但您的國家/地區可能不會。 如有需要，您可能需要根據這些變更調整您的系統時區。


## [!DNL Workfront]中的時區

您在[!DNL Workfront]中看到的時間是根據您組織[!DNL Workfront]執行個體和使用者設定檔的時區設定。 如果這兩個時區不同，您可能會在[!DNL Workfront]中使用的不同區域和功能中看到時間差異。

>[!NOTE]
>
>在附加到物件的自訂表單中，計算自訂欄位中的日期和時間陳述式會由世界協調時間(UTC)計算和儲存，而不是由針對您的組織執行個體和您的使用者設定檔設定的時區設定計算和儲存。 自訂表單中的計算會根據每位使用者的個別時區產生和顯示。

* [您組織的 [!DNL Workfront] 執行個體](#your-organization-s-workfront-instance)
* [您的使用者設定檔](#your-user-profile)

### 您組織的[!DNL Workfront]執行個體 {#your-organization-s-workfront-instance}

您組織的[!DNL Workfront]執行個體時區通常設定在主辦公室的位置。 這會決定下列專案：

* 由[!DNL Workfront]產生的電子郵件中所顯示的時間
* 新新增使用者的時區（在[!DNL Workfront]管理員根據使用者的工作位置為其設定不同時區之前）

  如需這兩個範例的詳細資訊，請參閱[設定您系統的基本資訊](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md)。

* 專案之覆寫收費率的開始或結束。 如需詳細資訊，請參閱專案層級](../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md)的[覆寫工作角色收費率。

### 您的使用者設定檔 {#your-user-profile}

您使用者設定檔中的時區應該為您工作的位置設定。 這會決定下列專案：

<!--
* The time shown in your outgoing [!DNL Workfront] email messages
[NOTE FROM LISA: Saeid that dates/times shown in emails are more complicated than how it is described in the article so we decided to comment out this line.]
-->
* 處理物件的時間，例如開始和結束時間

  如果將位於多個時區的使用者指派給物件，[!DNL Workfront]會使用每個使用者設定檔中設定的時區，轉換每個相關人員的物件時間。

  **範例：**&#x200B;在您工作的東部標準時間(EST)區域中，您將工作設定為下午4:00，並將其指派給在太平洋標準時間(PST)區域工作的使用者。 對於這些使用者，開始時間顯示為下午1:00。 如果顯示為下午4:00，他們會延遲三個小時開始處理。

  如果物件建立者沒有注意到受指派人時區之間的差異，並在設定物件時間時進行必要的調整，或受指派人沒有注意到該差異，則當每個人都在物件上合作時，可能很難獲得正確的時機。

  **範例：**&#x200B;您設定從東部時間上午9:00開始的一天工作，忘記工作上的某些使用者在PST區域工作。 對於他們，開始時間是上午6:00。 由於他們要到時間9:00 （您時間的中午）才會開始處理，因此任務會延遲三個小時開始和完成。

如需在使用者設定檔中設定時區的資訊，請參閱[設定我的設定](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md)。

如需[!DNL Workfront]管理員（或具有[!UICONTROL 編輯]使用者存取許可權的人）如何在使用者設定檔中設定時區的相關資訊，請參閱[編輯使用者設定檔](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

## 如何讓使用者更輕鬆地跨時區工作

您可以透過多種方式協助使用者更輕鬆地在數個時區中工作：

* [使用時程表](#use-schedules)
* [在自訂表單中使用計算的時間欄位](#use-calculated-time-fields-in-a-custom-form)
* [在自訂表單中使用文字欄位而非日期欄位](#use-text-fields-instead-of-date-fields-in-a-custom-form)

### 使用時程表 {#use-schedules}

[!DNL Workfront]管理員會為貴組織內的每個時區建立個別排程，以確保所有人都能適當地排程工作，無論他們身在何處。 管理員建立排程後，便可與特定專案和使用者建立關聯：

* **[!UICONTROL 專案]**：專案建立者可以選取個別專案的排程。 這會根據受指派人時區設定的工作時數，決定專案中任務的排程。
* **[!UICONTROL 使用者]**： [!DNL Workfront]管理員（或具有[!UICONTROL 編輯]使用者存取許可權的人）可以在使用者設定檔中為個別使用者選取排程。

  此排程可能與專案排程不同。 例如，當有人在專案中建立任務，但尚未指派任何人給它時，該任務就會使用專案排程。 將使用者指派給任務時，任務會使用該使用者的排程。

  如果將多個使用者指派到一個任務，則系統會使用下列其中一項，如系統或群組範圍專案偏好設定中所設定：

   * 任務主要擁有者的排程時區
   * 專案排程的時區。

  <div class="preview">

  如果將一位使用者指派給任務，則系統會使用下列其中一項，如系統或群組範圍專案偏好設定中所設定：

   * 任務受指派人排程的時區
   * 專案排程的時區。

  </div>

  這可能會造成任務日期變更。

>[!BEGINSHADEBOX]

**範例：**
EST使用者會被指派給排程在早上9:00 PST （亦即EST中午）開始的一日工作。 由於EST使用者一天只剩下2個工作小時，因此任務完成日期會延長約6小時，直到下一個工作日。


>[!ENDSHADEBOX]

如需[!UICONTROL 安裝程式]之[!UICONTROL 專案偏好設定]區域的相關資訊，請參閱[設定全系統的專案偏好設定](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

如需將排程指派給專案或使用者的指示，請參閱[建立排程](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)。

如需排程中設定的時區如何影響[!UICONTROL 工作負載平衡器]中[!UICONTROL 規劃時數]的分佈的相關資訊，請參閱[在[!UICONTROL 工作負載平衡器]](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)中管理使用者配置。


### 在自訂表單中使用計算的時間欄位 {#use-calculated-time-fields-in-a-custom-form}

您可以在自訂表單中使用一系列計算出的自訂欄位來顯示組織中使用者的目前時間，例如顯示多個城市中的時間的一列機場時鐘。 您可以為使用者工作的每個時區建立一個欄位，每個時區都會計算其時區的時間。

如需詳細資訊，請參閱[將計算欄位新增至表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)，以及文章[計算資料運算式概觀](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md)中的[日期與時間計算自訂欄位](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md#date)一節。

### 在自訂表單中使用文字欄位而非日期欄位 {#use-text-fields-instead-of-date-fields-in-a-custom-form}

若您不希望[!DNL Workfront]轉換您在物件中為不同時區的使用者設定的時間，您可以使用附加到物件的自訂表單中的文字欄位，而不是日期欄位。 如此一來，時間就會顯示您為專案中的每個人輸入的時間。

若您這麼做，建議您提醒表單的使用者計算其時區與您的時區之間的差異，以便他們決定工作應該開始與結束的時間。 您可以在自訂表單的指示或該欄位的工具提示中鍵入此資訊。 如需詳細資訊，請參閱[建立自訂表格](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。
