---
title: 群組概述
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
description: Workfront管理員可建立與您的部門結構一致的使用者群組。 群組與類似，但與團隊和公司不同。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1353ab04-7de7-4d30-a092-27807c950777
source-git-commit: b5e0a590d258df4510a0bb6a44b57099f32ae6b9
workflow-type: tm+mt
source-wordcount: '927'
ht-degree: 0%

---

# 群組概述

<!-- Audited: 01/2024 -->

Workfront管理員可建立與您的部門結構一致的使用者群組。 群組與類似，但與團隊和公司不同。

Workfront管理員會授予群組對其需要工作和溝通的Workfront區域的存取權。 然後，每個群組都可以將其Workfront資訊（例如，使用者、範本和自訂表格）和專案與其他部門的資訊分開。

每個群組至少需要一個群組管理員。 群組管理員可以使用「群組」頁面在一個位置管理其群組。 如需詳細資訊，請參閱[群組管理員](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md)。

您最多可以在一個群組下建立14層子群組。 如需詳細資訊，請參閱[子群組概述](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md)和[建立子群組](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md)。

## 使用群組來組織使用者

身為Workfront管理員或群組管理員，您可以將使用者與群組和子群組建立關聯。 如果您將群組設定為公用，則擁有「標準」 （新）或「計畫」 （目前）授權的使用者可以將使用者與其相關聯。 如需群組管理員與公用群組的詳細資訊，請參閱[建立群組](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)。

當您建立使用者時，我們建議您將該使用者新增至該使用者應在其中工作的適當主群組和其他群組。 一個使用者只能有一個主群組，但可以位於多個其他群組中。

成為群組的一部分可讓使用者存取與群組和子群組共用的物件。 例如，如果您與群組共用專案，則該群組和該群組的子群組中的使用者有權存取該專案。

>[!TIP]
>
>如果貴組織中的部門經常一起合作來管理專案及這些專案的資源，則可能不需要將部門分成許多較小的群組。 一些高階群組可能效果最佳。

群組可以有不限數量的使用者。

如需有關建立新使用者的詳細資訊，請參閱[新增使用者](../../../administration-and-setup/add-users/add-users.md)。

## 授予群組存取物件的許可權

當您與群組共用物件時，該群組的所有成員（包括任何子群組的成員）都可以存取該物件。 如需在Workfront中共用的詳細資訊，請參閱[物件共用許可權總覽](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。

## 建立群組與物件的關聯

當您建立或編輯下列Workfront物件之一時，可以將其與群組相關聯：

* **專案**：您可以將單一群組與專案建立關聯，以表示專案的所有權。

  這不會隱含地授予群組的每個成員專案的許可權。 若要擁有專案的使用者許可權，他們必須擁有與其共用的專案。

  雖然使用者可以是多個群組的成員，但一個專案可以有一個相關聯的單一群組。 如果專案已與他們或其群組共用，則其他群組的使用者仍可處理相同的專案。 與專案相關聯的群組通常是負責完成專案的群組，或是專案交付的群組。

  如需將專案與群組建立關聯的說明，請參閱[專案概述區域](../../../manage-work/projects/manage-projects/understand-project-overview-area.md)中的管理資訊。

* **Portfolio、方案或公司**：當您建立或編輯投資組合、方案或公司時，可以指派單一群組給它，以表示該群組擁有它或對其負責。 建立此關聯後，管理員和使用者就可輕鬆識別其群組正在處理的投資組合、計畫和公司。

  例如，群組管理員可以使用清單或報告列出組織中的所有投資組合，並在「群組」欄中記下指派給其群組的投資組合。

  >[!NOTE]
  >
  >將群組指派給具有群組的投資組合、方案或公司，並不自動錶示群組中的資訊有權存取其資料。 您需要先手動與群組共用資料的存取權，群組才能看見。

  如需指示，請參閱[建立投資組合](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md)、[建立方案](../../../manage-work/portfolios/create-and-manage-programs/create-program.md)和[建立和編輯公司](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md)。

* **核准流程**：您可以讓核准流程適用於屬於特定群組的專案、任務和問題。 如需詳細資訊，請參閱[建立工作專案的核准程式](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)。
* **里程碑路徑**：您可以允許特定群組中的使用者將里程碑路徑用於其專案。 如需詳細資訊，請參閱[建立里程碑路徑](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md)。
* **配置範本**：您可以授予群組的管理員許可權來修改配置範本。 如需指示，請參閱[授與配置範本的管理存取權](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md)。

* **時程表設定檔**：您可以授予群組的管理員許可權，以修改時程表設定檔。 如需詳細資訊，請參閱[建立、編輯和指派週期性時程表](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)。

* **排程**：您可以授予群組的管理員許可權來修改排程。 如需詳細資訊，請參閱[建立排程](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)。
* **團隊**：您可以將群組與團隊建立關聯，以便群組及其子群組的管理員可以從「群組」區域檢視及與這些團隊合作。 如需詳細資訊，請參閱[建立團隊](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md)或[編輯團隊設定](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md)。
* **範本**：您可以將群組指派給專案範本。 這可協助您簡化專案建立流程，並協助您更輕鬆地識別及報告哪些群組擁有哪些專案範本。 如需詳細資訊，請參閱文章[編輯專案範本](../../../manage-work/projects/create-and-manage-templates/edit-templates.md)中的[概觀](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#overview)一節。

* **最近刪除及還原的專案**：您可以檢視及管理群組最近刪除的專案。 如需詳細資訊，請參閱[檢視和管理群組最近刪除的專案](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-deleted-objects.md)和[檢視和管理群組最近還原的專案](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-restored-objects.md)。
