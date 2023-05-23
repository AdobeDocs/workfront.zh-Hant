---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: 跨時區工作
description: 瞭解一下 [!DNL Adobe Workfront] 使用時區來計算對象的時間欄位，以及電子郵件等其他區域的時間。
feature: Get Started with Workfront
exl-id: b6574165-a6dc-4694-a367-d98927abf1e3
source-git-commit: 114d306d99ae9ba0a18abd63a6137ad0568ab202
workflow-type: tm+mt
source-wordcount: '1072'
ht-degree: 0%

---

# 跨時區工作

瞭解一下 [!DNL Adobe Workfront] 使用時區計算以下內容：

* 對象的時間欄位
* 其他時間 [!DNL Workfront] 區域，如自動化的Workfront電子郵件

## 中的時區 [!DNL Workfront]

您在 [!DNL Workfront] 基於組織的時區配置 [!DNL Workfront] 實例和用戶配置檔案。 如果這兩個時區不同，您可能會在不同的區域和功能中看到時間差異。 [!DNL Workfront]。

>[!NOTE]
>
>在附加到對象的自定義表單中，計算的自定義欄位中的日期和時間語句由協調通用時間(UTC)計算和保存，而不是由為組織實例和用戶配置檔案設定的時區配置。 根據每個用戶的單個時區生成和顯示自定義形式的計算。

* [您的組織 [!DNL Workfront] 實例](#your-organization-s-workfront-instance)
* [您的用戶配置檔案](#your-user-profile)

### 您的組織 [!DNL Workfront] 實例 {#your-organization-s-workfront-instance}

組織的時區 [!DNL Workfront] 通常為主辦公室的位置設定實例。 這決定了以下因素：

* 由生成的電子郵件中顯示的時間 [!DNL Workfront]
* 新添加用戶的時區(在 [!DNL Workfront] 管理員根據工作地點為他們配置不同的時區)

   有關這兩個示例的詳細資訊，請參見 [配置系統的基本資訊](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md)。

* 已覆蓋項目開單費率的開始或結束。 有關詳細資訊，請參見 [改寫項目層的職務職責開單費率](../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md)。

### 您的用戶配置檔案 {#your-user-profile}

您的用戶配置檔案中的時區應該配置到您工作的位置。 這決定了以下因素：

<!--
* The time shown in your outgoing [!DNL Workfront] email messages
[NOTE FROM LISA: Saeid that dates/times shown in emails are more complicated than how it is described in the article so we decided to comment out this line.]
-->
* 所處理對象的時間，如開始和結束時間

   如果將多個時區中的用戶分配給對象， [!DNL Workfront] 使用每個用戶配置檔案中配置的時區，轉換所有參與者的對象時間。

   **示例：** 在您工作的「東部標準時間(EST)」區域中，您將任務設定為從下午4:00開始，並將其分配給在太平洋標準時間(PST)區域中工作的用戶。 對於這些用戶，開始時間顯示為下午1:00。 如果把它顯示為下午4點，他們會晚3小時開始工作。

   如果對象建立者沒有注意到受分配者的時區之間的差異，並在設定對象時間時進行必要的調整，或者受分配者沒有注意到這一差異，則當每個人在對象上協作時，很難正確獲取時間。

   **示例：** 您將一天任務配置為在東部時間上午9:00開始，忘記了某些任務用戶在PST區域工作。 對他們來說，是早上6點開始。 因為他們要到9點（你的時間正午）才開始處理它，所以任務開始並延遲了3個小時。

有關在用戶配置檔案中配置時區的資訊，請參閱 [配置我的設定](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md)。

有關如何 [!DNL Workfront] 管理員(或 [!UICONTROL 編輯] 訪問用戶)可以在用戶配置檔案中配置時區，請參閱 [編輯用戶的配置檔案](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

## 如何讓用戶更輕鬆地跨時區工作

您可以通過多種方式幫助用戶更輕鬆地跨多個時區工作：

* [使用計畫](#use-schedules)
* [在自定義窗體中使用計算時間欄位](#use-calculated-time-fields-in-a-custom-form)
* [在自定義窗體中使用文本欄位而不是日期欄位](#use-text-fields-instead-of-date-fields-in-a-custom-form)

### 使用計畫 {#use-schedules}

[!DNL Workfront] 管理員為您組織內的每個時區建立單獨的時間表，以確保無論工作在何處，都為每個人適當地安排工作時間。 一旦管理員建立了計畫，它們就可以與某些項目和用戶關聯：

* **[!UICONTROL 項目]**:項目建立者可以為單個項目選擇計畫。 這根據為受分配人的時區設定的工作小時數確定項目中任務的計畫。
* **[!UICONTROL 用戶]**:A [!DNL Workfront] 管理員(或 [!UICONTROL 編輯] 訪問用戶)可以在用戶配置檔案中為單個用戶選擇計畫。

   此計畫可能與項目計畫不同。 例如，當某人在項目中建立任務但尚未為其分配任何人時，該任務將使用項目計畫。 當用戶被分配到任務時，該任務將使用該用戶的調度。

   如果將多個用戶分配給任務，則系統使用以下任務之一，如在系統範圍的項目首選項中配置的：

   * 任務主要所有者的計畫時區
   * 項目計畫的時區。

   這可能導致任務日期發生更改。

   **示例：** EST用戶被分配到一天任務，該任務計畫在PST時間上午9:00開始，即東部標準時間中午。 由於EST用戶當天僅剩2個工作小時，因此任務完成日期將延長約6小時，直到下一工作日。

   有關 [!UICONTROL 項目首選項] 區域 [!UICONTROL 設定]，請參閱 [配置系統範圍的項目首選項](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

   有關為項目或用戶分配計畫的說明，請參閱 [建立計畫](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)。

   有關在計畫中配置的時區如何影響 [!UICONTROL 計畫小時數] 的 [!DNL Workload Balancer]，請參閱 [管理 [!DNL Workload Balancer]](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)。


### 在自定義窗體中使用計算時間欄位 {#use-calculated-time-fields-in-a-custom-form}

您可以在自定義表單上使用一系列計算的自定義欄位來顯示組織中用戶的當前時間，如顯示多個城市中時間的機場時鐘行。 您可以為用戶工作的每個時區建立一個欄位，每個時區都計算其時區的時間。

有關詳細資訊，請參見 [將計算資料添加到自定義窗體](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)，以及 [日期和時間計算的自定義欄位](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md#date) 在文章中 [計算的資料表達式](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md)。

### 在自定義窗體中使用文本欄位而不是日期欄位 {#use-text-fields-instead-of-date-fields-in-a-custom-form}

如果你不想 [!DNL Workfront] 要轉換在對象中為不同時區的用戶配置的時間，可以使用附加到對象的自定義表單中的文本欄位，而不是日期欄位。 這樣，該時間顯示您為項目中的每個人鍵入的時間。

如果您這樣做，我們建議您提醒表單的用戶計算其時區與您的時區之間的差異，以便他們能夠確定何時開始和結束工作。 您可以將此內容包含在您為自定義表單鍵入的說明中，或包含在該欄位的工具提示中。 有關詳細資訊，請參見 [將自定義欄位添加到自定義表單](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)。
