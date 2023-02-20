---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: 跨時區工作
description: 了解 [!DNL Adobe Workfront] 使用時區來計算以下內容 — EDIT ME。
feature: Get Started with Workfront
exl-id: b6574165-a6dc-4694-a367-d98927abf1e3
source-git-commit: fb538c6511514eedf81f4b9be452d5f87e3f7577
workflow-type: tm+mt
source-wordcount: '1072'
ht-degree: 0%

---

# 跨時區工作

了解 [!DNL Adobe Workfront] 使用時區來計算下列項目：

* 對象的時間欄位
* 其他時間 [!DNL Workfront] 區域，例如自動化Workfront電子郵件

## 中的時區 [!DNL Workfront]

在 [!DNL Workfront] 是根據貴組織的時區設定 [!DNL Workfront] 例項和使用者設定檔。 如果這兩個時區不同，您可能會在中使用的不同區域和功能中看到時間差異 [!DNL Workfront].

>[!NOTE]
>
><div class="preview">在附加至物件的自訂表單中，計算自訂欄位中的日期和時間陳述式是由協調通用時間(UTC)計算並儲存，而非由組織例項和使用者設定檔所設定的時區設定。 根據每個用戶的各個時區生成並顯示自定義格式的計算。</div>




* [貴組織的 [!DNL Workfront] 執行個體](#your-organization-s-workfront-instance)
* [您的使用者設定檔](#your-user-profile)

### 貴組織的 [!DNL Workfront] 執行個體 {#your-organization-s-workfront-instance}

貴組織的 [!DNL Workfront] 通常為主辦公室的位置設定實例。 這會決定下列項目：

* 由產生的電子郵件中顯示的時間 [!DNL Workfront]
* 新新增使用者的時區(在 [!DNL Workfront] 管理員會根據其工作位置為其配置不同的時區)

   如需這兩個範例的詳細資訊，請參閱 [配置系統的基本資訊](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

* 已覆蓋的項目開單費率的開始或結束。 如需詳細資訊，請參閱 [在項目層改寫任務職責開單費率](../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

### 您的使用者設定檔 {#your-user-profile}

應針對您所在的位置設定使用者設定檔中的時區。 這會決定下列項目：

* 傳出的 [!DNL Workfront] 電子郵件訊息
* 您使用的物件的時間，例如開始和結束時間

   如果將多個時區的用戶分配給某個對象， [!DNL Workfront] 使用每個使用者設定檔中設定的時區，來轉換相關每個人的物件時間。

   **範例：** 在您工作的東部標準時間(EST)區域中，您設定了一個任務，從下午4:00開始，並將其分配給在太平洋標準時間(PST)區域中工作的用戶。 對於這些使用者，開始時間會顯示為下午1:00。 如果要在下午4:00顯示，他們會延遲3小時開始工作。

   如果對象建立者沒有注意到受分配者的時區之間的差異並在設定對象時間時進行必要的調整，或者受分配者沒有注意到這種差異，則當每個人都協作對對象時，很難正確地獲取時間。

   **範例：** 您將一天的任務配置為在東部標準時間上午9:00開始，而忘記了任務上的某些用戶在太平洋標準時工作。 對他們來說，早上6:00 因為他們要等到9:00（您的時間中午）才會開始處理，所以任務開始並延遲3小時完成。

如需在使用者設定檔中設定時區的資訊，請參閱 [配置我的設定](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

如需 [!DNL Workfront] 管理員(或 [!UICONTROL 編輯] 存取使用者)可在使用者設定檔中設定時區，請參閱 [編輯使用者的設定檔](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## 如何讓使用者更輕鬆地跨時區工作

您可以透過數種方式，協助使用者更輕鬆地跨多個時區工作：

* [使用排程](#use-schedules)
* [在自訂表單中使用計算時間欄位](#use-calculated-time-fields-in-a-custom-form)
* [在自訂表單中使用文字欄位，而非日期欄位](#use-text-fields-instead-of-date-fields-in-a-custom-form)

### 使用排程 {#use-schedules}

[!DNL Workfront] 管理員會為組織內的每個時區建立不同的排程，確保無論工作在何處，都能為每個人適當排程工作。 管理員建立排程後，即可與特定專案和使用者建立關聯：

* **[!UICONTROL 專案]**:專案建立者可以選取個別專案的排程。 這根據為受分配者的時區設定的工作時數，決定項目中任務的排程。
* **[!UICONTROL 使用者]**:A [!DNL Workfront] 管理員(或 [!UICONTROL 編輯] 存取使用者)可以在使用者的設定檔中選取個別使用者的排程。

   此排程可能與專案排程不同。 例如，當某人在項目中建立了任務，但尚未為其分配任何人時，該任務將使用項目計畫。 將用戶分配給任務時，該任務將使用該用戶的調度。

   如果為任務分配了多個用戶，則系統將使用以下任一項，如系統範圍的項目首選項中所配置：

   * 任務主要所有者的計畫時區
   * 專案排程的時區。

   這可能會導致任務日期變更。

   **範例：** EST用戶被分配給一天的任務，該任務計畫在9:00 AM PST（正午為EST）開始。 因為EST用戶一天只剩下2個工作小時，任務完成日期將延長約6小時，直到下一個工作日。

   如需 [!UICONTROL 專案偏好設定] 區域 [!UICONTROL 設定]，請參閱 [配置系統範圍的項目首選項](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   有關為項目或用戶分配計畫的說明，請參閱 [建立排程](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

   有關在計畫中配置的時區如何影響 [!UICONTROL 計畫小時數] 在 [!DNL Workload Balancer]，請參閱 [在 [!DNL Workload Balancer]](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).


### 在自訂表單中使用計算時間欄位 {#use-calculated-time-fields-in-a-custom-form}

您可以在自訂表單上使用一系列計算的自訂欄位，來顯示組織中使用者的目前時間，例如一列機場時鐘，顯示多個城市的時間。 您可以為使用者工作的每個時區建立欄位，每個時區都會計算時間。

如需詳細資訊，請參閱 [將計算資料新增至自訂表單](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)，以及區段 [日期和時間計算的自訂欄位](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md#date) 在文章中 [計算資料運算式](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

### 在自訂表單中使用文字欄位，而非日期欄位 {#use-text-fields-instead-of-date-fields-in-a-custom-form}

如果你不想 [!DNL Workfront] 要為不同時區的用戶在對象中配置的時間進行轉換，可以使用附加到對象的自定義表單中的文本欄位，而不是日期欄位。 這樣，該時間會顯示您為專案中的每個人輸入的時間。

若您這麼做，建議您提醒表單的使用者計算其時區與您時區之間的差異，以便決定工作的開始和結束時間。 您可以將此內容納入您為自訂表單輸入的指示中，或納入該欄位的工具提示中。 如需詳細資訊，請參閱 [新增自訂欄位至自訂表單](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md).
