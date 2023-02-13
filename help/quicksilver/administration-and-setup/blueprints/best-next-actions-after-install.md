---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: 安裝Blueprint後要採取的動作
description: 本文概述在中安裝Blueprint後，您應該做什麼 [!DNL Adobe Workfront] 將blueprint完全部署給系統用戶。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6e5da58f-105a-4edf-8fc1-65e8762d43c6
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '1139'
ht-degree: 0%

---

# 安裝Blueprint後要採取的動作

本文概述在中安裝Blueprint後，您應該做什麼 [!DNL Adobe Workfront] 將blueprint完全部署給系統用戶。

* [專案範本建議](#project-template-recommendations)
* [組織結構建議](#organizational-structure-recommendations)
* [控制面板建議](#dashboard-recommendations)

## 專案範本建議 {#project-template-recommendations}

本節包含與藍圖一起安裝的項目模板的建議。

### 將使用者指派給新建立的角色和團隊 {#assign-users-to-newly-created-roles-and-teams}

在Blueprint安裝程式期間建立的角色和/或團隊沒有自動關聯的使用者。 若不將使用者指派給新新增的角色或團隊，您將會為無人挑選的函式建立工作。 在某些情況下，您可能需要建立新使用者來填寫這些角色和團隊。 如需建立新使用者的詳細資訊，請參閱 [新增使用者](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

### 將自訂表單套用至範本和範本工作 {#apply-a-custom-form-to-the-template-and-the-template-tasks}

安裝程式不會將專案範本與任何自訂表單建立關聯。 如果您的專案或工作需要填入特定表單或欄位，以建立報表一致性，或如果您的數位請求表單包含需要在專案層級保留的欄位，建議您將範本或範本工作與這些表單建立關聯。 如需詳細資訊，請參閱 [將自訂表單新增至物件](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

### 更新模板任務持續時間和工作估計 {#update-template-task-duration-and-effort-estimates}

模板中的每個任務都包含計畫的持續時間和計畫的工作估計。 這些估計值可作為這些活動持續時間和逗留時間的起點。 不過，您組織的功能、技能和步調是獨一無二的。 您應查看每個任務的預計持續時間和工作量，以調整它以反映組織的需求。 如需詳細資訊，請參閱 [管理 [!UICONTROL 任務詳細資訊概述] 區域](../../manage-work/tasks/manage-tasks/task-information-in-overview.md).

### 關聯里程碑路徑和里程碑 {#associate-a-milestone-path-and-milestones}

安裝過程不會將項目模板與里程碑路徑關聯。 將里程碑路徑套用至範本，並將里程碑套用至範本中的關鍵任務，以支援您的里程碑報表需求。 如需詳細資訊，請參閱 [將里程碑與任務關聯](../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

### 將範本轉出給您的團隊 {#roll-out-the-template-to-your-team}

為將使用此模板的工作經理和將在項目模板中執行工作的個人貢獻者準備培訓材料。

### 建立或更新報表和控制面板 {#create-or-update-reports-and-dashboards}

如果解決方案代表您的組織先前未執行的新工作類型 [!DNL Workfront]，您可能需要建立新的報表和控制面板來支援工作。 如需詳細資訊，請參閱 [建立自訂報表](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) 和 [建立控制面板](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

如果解決方案類似於您已在中執行的工作 [!DNL Workfront]，則應如預期般確認工作摘要至現有報表和控制面板。 如果它未饋送至您現有的報表，請採取動作來更新篩選器或建立新報表。

## 組織結構建議 {#organizational-structure-recommendations}

本節包含與藍圖一起安裝的組織結構元素的建議。

### 公司

安裝包含公司的藍圖後：

* 新增自訂表單以使用有用的詳細資訊（表單及其詳細資訊對您而言是唯一的）來增強公司記錄。 如需詳細資訊，請參閱 [將自訂表單新增至物件](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
* 如果公司代表客戶，請複查與公司關聯的改寫率。 如需詳細資訊，請參閱 [在公司層改寫職務開單費率](../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).
* 如果公司代表客戶，並且有其他特定於組織的專案範本，請先將專案範本與新新增的公司預先建立關聯。 如需詳細資訊，請參閱 [編輯專案範本](../../manage-work/projects/create-and-manage-templates/edit-templates.md).
* 如果公司代表客戶或供應商，請將可能位於您環境中的外部組織的現有使用者建立關聯。 如需詳細資訊，請參閱 [建立和編輯公司](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).
* 如果公司代表客戶或供應商，請為您的環境中可能需要的外部組織建立額外的協作用戶，以簡化通信、工作執行和審批。 如需建立新使用者的詳細資訊，請參閱 [新增使用者](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).
* 更新與新新增公司關聯之任何使用者的組織圖表關係。 如需詳細資訊，請參閱 [建立直接報表](../../administration-and-setup/add-users/create-and-manage-users/create-direct-reports.md) 和 [檢視組織圖表](../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md).

如需公司的詳細資訊，請參閱 [建立和編輯公司](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## 控制面板建議 {#dashboard-recommendations}

本節包含與Blueprint一起安裝之控制面板和報表的建議。

### 更新新建立的控制面板以新增/移除報表

從Blueprint新增的控制面板有一或多個報表、外部頁面或日曆。 您可能不需要所有報表和其他控制面板元素，或需先以現有報表、外部頁面和日曆來擴大控制面板，才能與其他人共用。 如需詳細資訊，請參閱 [新增報表至控制面板](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md).

### 更新新建立的報表以新增/移除欄或篩選條件

透過控制面板藍圖分發的報表並沒有所有支援您設定的欄或篩選條件 [!DNL Workfront]. 預計您會對報表進行一些調整，以符合您的標準。 為了與環境中的其他報表保持一致，您可能想要為所列出的物件在所有報表上新增您所包含的欄，或新增一些篩選條件，限制結果至特定專案類型或使用者群組。 如需詳細資訊，請參閱 [建立或編輯視圖](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md) 和 [建立或編輯篩選器](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

### 與使用者共用控制面板或報表

如果您不打算將控制面板放置在配置範本上，您應將控制面板與會發現其實用的人員共用。 如需詳細資訊，請參閱 [共用控制面板](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md) 和 [共用報表](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

### 將控制面板新增至配置範本

將控制面板新增至配置範本，是讓其他人也能使用的最佳方式。 識別最能受益於定期檢閱控制面板的人員的配置範本，並將新建立的控制面板新增至這些配置範本。 如需詳細資訊，請參閱 [建立和管理版面範本](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

### 更新其他控制面板和報表

新控制面板及其報表的引入，可讓您淘汰並調整其他現有的控制面板及報表。 請花時間檢閱您現有的報表，以找出任何重複且相互矛盾的報表。

### 將自訂資料發佈至相關表單

控制面板藍圖中包含的某些報表在報表的檢視、篩選或分組中都有自訂資料欄位。 在某些情況下，Blueprint也會有與這些欄位相關聯的表單。 不過，自訂欄位通常不會套用至自訂表單。 為了欄、篩選器或群組才能正常運作，這些欄位必須與連結至使用者、專案、任務或其他物件記錄的表單相關聯。 如需詳細資訊，請參閱 [新增自訂欄位至自訂表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md).
