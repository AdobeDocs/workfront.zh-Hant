---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: 安裝Blueprint後要採取的動作
description: 本文概述您在 [!DNL Adobe Workfront] 中安裝Blueprint後，應該做什麼，才能將該Blueprint完全部署給您的系統使用者。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 6e5da58f-105a-4edf-8fc1-65e8762d43c6
source-git-commit: 55c8a3e5d0041a0e975bfd979a2d2e38930fea8d
workflow-type: tm+mt
source-wordcount: '1138'
ht-degree: 0%

---

# 安裝Blueprint後要採取的動作

本文概述您在[!DNL Adobe Workfront]中安裝Blueprint以將Blueprint完全部署給系統使用者後應該做什麼。

* [專案範本建議](#project-template-recommendations)
* [組織結構建議](#organizational-structure-recommendations)
* [控制面板建議](#dashboard-recommendations)

## 專案範本建議 {#project-template-recommendations}

本節包含與您的Blueprint一起安裝的專案範本的建議。

### 將使用者指派給新建立的角色和團隊 {#assign-users-to-newly-created-roles-and-teams}

在Blueprint安裝過程中建立的角色和/或團隊不會自動擁有與其相關聯的使用者。 您不需要將使用者指派給新加入的角色或團隊，就能為無人接手的功能建立工作。 在某些情況下，您可能需要建立新使用者來填入這些角色和團隊。 如需建立新使用者的詳細資訊，請參閱[新增使用者](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)。

### 套用自訂表單至範本和範本任務 {#apply-a-custom-form-to-the-template-and-the-template-tasks}

安裝程式不會將專案範本與任何自訂表單建立關聯。 如果您的專案或任務需要填入特定表單或欄位來建立報告一致性，或者如果您的數位請求表單包含需要保留在專案級別的欄位，我們建議您將範本或範本任務與這些表單相關聯。 如需詳細資訊，請參閱[新增自訂表單至物件](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)。

### 更新範本任務持續時間和工作量估計 {#update-template-task-duration-and-effort-estimates}

範本中的每個任務都包含計畫持續時間和計畫投入估計值。 這些估計值會作為這些活動的持續時間和逗留時間的起點。 不過，貴組織的能力、技能和步調是獨特的。 您應該檢閱每個任務的估計持續時間和工作量，以調整它以反映您組織的需求。 如需相關資訊，請參閱[!UICONTROL 任務詳細資訊總覽]區域](../../manage-work/tasks/manage-tasks/task-information-in-overview.md)中的[管理任務資訊。

### 關聯里程碑路徑和里程碑 {#associate-a-milestone-path-and-milestones}

安裝程式不會將專案範本與里程碑路徑建立關聯。 將里程碑路徑套用至範本，並將里程碑套用至範本中的關鍵工作，以支援您的里程碑報告需求。 如需詳細資訊，請參閱[將里程碑與任務關聯](../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md)。

### 將範本轉出給您的團隊 {#roll-out-the-template-to-your-team}

為將使用此範本的工作經理以及將在專案範本內執行工作的個別貢獻者準備訓練教材。

### 建立或更新報告和儀表板 {#create-or-update-reports-and-dashboards}

如果解決方案代表貴組織先前未在[!DNL Workfront]中執行的新工作型別，您可能需要建立新的報告和儀表板以支援該工作。 如需詳細資訊，請參閱[建立自訂報告](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)和[建立儀表板](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md)。

如果解決方案與您已在[!DNL Workfront]中執行的工作類似，則您應驗證工作饋送是否如預期般進入現有報表和控制面板。 如果它未匯入您的現有報告中，請採取行動來更新篩選器或建立新報告。

## 組織結構建議 {#organizational-structure-recommendations}

本節包含與您的Blueprint一起安裝之組織結構元素的建議。

### 公司

安裝包含公司的Blueprint後：

* 新增自訂表單，以使用有用的詳細資料來增加公司記錄（表單及其詳細資料是唯一的）。 如需詳細資訊，請參閱[新增自訂表單至物件](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)。
* 如果公司代表客戶，請檢閱與公司關聯的覆寫率。 如需相關資訊，請參閱[覆寫公司層級](../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md)的工作角色收費率。
* 如果公司代表客戶，並且有其他專案範本屬於該組織，請先將專案範本與新增的公司預先建立關聯。 如需詳細資訊，請參閱[編輯專案範本](../../manage-work/projects/create-and-manage-templates/edit-templates.md)。
* 如果公司代表客戶或廠商，請關聯來自外部組織的現有使用者（可能已在您的環境中）。 如需詳細資訊，請參閱[建立和編輯公司](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md)。
* 如果公司代表客戶或廠商，請為您環境中可能需要的外部組織建立其他共同作業人員使用者，以簡化溝通、工作執行和核准。 如需建立新使用者的詳細資訊，請參閱[新增使用者](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)。
* 更新任何現在與新增公司相關聯之使用者的組織圖關係。 如需詳細資訊，請參閱[建立直接下屬](../../administration-and-setup/add-users/create-and-manage-users/create-direct-reports.md)和[檢視組織圖](../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md)。

如需有關公司的其他資訊，請參閱[建立和編輯公司](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md)。

## 控制面板建議 {#dashboard-recommendations}

本節包含與藍圖一起安裝之控制面板和報表的建議。

### 更新新建立的儀表板以新增/移除報表

從Blueprint新增的控制面板有一或多個報告、外部頁面或行事曆。 您可能不需要所有報告和其他儀表板元素，或者您可能需要先使用現有的報告、外部頁面和行事曆來增加儀表板，然後才能與其他人共用。 如需詳細資訊，請參閱[新增報告至儀表板](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md)。

### 更新新建立的報告以新增/移除欄或篩選條件

透過儀表板Blueprint分發的報告沒有所有欄或篩選條件可支援您的[!DNL Workfront]設定。 預計您將會對報表進行一些調整，以符合您的標準。 為了與環境中的其他報告保持一致，您可能想要為列出的物件新增一個欄，或新增一些將結果限制在特定專案型別或使用者群組的篩選條件。 如需詳細資訊，請參閱[建立或編輯檢視](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md)和[建立或編輯篩選器](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md)。

### 與使用者共用儀表板或報表

如果您不打算將儀表板放在版面配置範本上，您應該將儀表板與認為它有用的人員共用。 如需詳細資訊，請參閱[共用儀表板](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md)和[共用報告](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)。

### 將儀表板新增到版面配置範本

讓其他人可以取得資訊的最佳方式是將儀表板新增到版面配置範本。 找出最受益於定期檢閱儀表板並將新建立的儀表板新增到這些版面範本的人員版面範本。 如需詳細資訊，請參閱[建立及管理配置範本](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)。

### 更新其他儀表板和報表

新控制面板及其報表的推出可能會讓您可以淘汰並調整其他現有的控制面板和報表。 請花點時間檢閱現有報告，找出任何多餘和矛盾的報告。

### 將自訂資料分發到相關表單

儀表板Blueprint中包含的某些報表在報表的檢視、篩選或分組中有自訂資料欄位。 在某些情況下，Blueprint還將具有與這些欄位關聯的表單。 不過，自訂欄位通常不會套用至自訂表單。 為了使欄、篩選器或群組正常運作，這些欄位必須與連線到使用者、專案、任務或其他物件記錄的表單相關聯。 如需詳細資訊，請參閱[使用表單設計工具](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)設計表單。
