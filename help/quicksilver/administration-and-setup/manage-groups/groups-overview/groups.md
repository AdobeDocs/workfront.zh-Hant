---
title: 群組
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
description: Workfront管理員可以建立符合您部門結構的使用者群組。 群組類似，但與團隊和公司不同。 Workfront管理員授予群組工作和通訊所需Workfront區域的存取權。 然後，每個群組都可將其Workfront資訊（例如使用者、範本和自訂表單，以及專案）與其他部門的資訊分開。 每個組至少需要一個組管理員。 群組管理員可使用「群組」頁面在單一位置管理其群組。 在一個組下最多可以建立14個子組級別。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1353ab04-7de7-4d30-a092-27807c950777
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '999'
ht-degree: 0%

---

# 群組概觀

Workfront管理員可以建立符合您部門結構的使用者群組。 群組類似，但與團隊和公司不同。

Workfront管理員授予群組工作和通訊所需Workfront區域的存取權。 然後，每個群組都可將其Workfront資訊（例如使用者、範本和自訂表單，以及專案）與其他部門的資訊分開。

每個組至少需要一個組管理員。 群組管理員可使用「群組」頁面在單一位置管理其群組。 如需詳細資訊，請參閱 [群組管理員](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

在一個組下最多可以建立14個子組級別。 如需詳細資訊，請參閱 [子組概述](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md) 和 [建立子組](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

## 使用群組來組織使用者

身為Workfront管理員或群組管理員，您可以將使用者與群組和子群組建立關聯。 如果將組設為公用組，則具有計畫員許可證的用戶可以將用戶與其關聯。 如需群組管理員和公用群組的詳細資訊，請參閱 [建立群組](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

當您建立使用者時，建議您將該使用者新增至該使用者應該使用的適當首頁群組和其他群組。 一個用戶只能有一個「首頁組」，但可以在多個其他組中。

作為組的一部分，用戶可以訪問與組和子組共用的對象。 例如，如果您與群組共用專案，群組和群組的子群組中的使用者有權存取該專案。

>[!TIP]
>
>如果組織中的部門經常合作管理這些項目的項目和資源，則可能不需要將部門劃分為許多較小的組。 幾個高層級群組的運作方式可能最佳。

一個群組可以有不限數量的使用者。

如需建立新使用者的詳細資訊，請參閱 [新增使用者](../../../administration-and-setup/add-users/add-users.md).

## 授予對對象的組訪問權

與組共用對象時，該組的所有成員（包括任何子組的成員）都有權訪問該對象。 如需在Workfront中共用的詳細資訊，請參閱 [對象共用權限概述](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## 將組與對象關聯

建立或編輯下列其中一個Workfront物件時，可將其與群組建立關聯：

* **專案**:您可以將單個組與項目關聯，以指明項目的所有權。

   這不會隱含授予群組每個成員對專案的權利。 若要擁有專案的權限，使用者必須透過與他們共用專案來接收權限。

   雖然使用者可以是多個群組的成員，但專案可以有與其相關聯的單一群組。 如果已與其或其群組共用專案，其他群組的使用者仍可處理相同的專案。 與項目關聯的組通常是負責完成項目的組，或項目交付的組。

   有關將項目與組關聯的說明，請參閱 [在項目概覽區域中管理資訊](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

* **Portfolio、方案或公司**:當您建立或編輯產品組合、方案或公司時，可以為其分配單個組，以指明該組擁有或負責該組。 有了這種關聯，管理員和用戶可以輕鬆識別其團隊正在從事的產品組合、計畫和公司。

   例如，群組管理員可使用清單或群組欄中的報表和附註來列出組織中的所有產品組合，而將產品組合指派給其群組。

   >[!NOTE]
   >
   >將群組指派給具有群組的產品組合、方案或公司，並不會自動表示群組可存取其資料的資訊。 您必須先手動與群組共用資料的存取權，資料才能看到。

   如需指示，請參閱 [建立產品組合](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md), [建立方案](../../../manage-work/portfolios/create-and-manage-programs/create-program.md)，和 [建立和編輯公司](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* **核准程式**:您可以讓核准程式適用於屬於特定群組的專案、任務和問題。 如需詳細資訊，請參閱 [建立工作項的審批流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).
* **里程碑路徑**:您可以允許某些群組中的使用者透過其專案使用里程碑路徑。 如需詳細資訊，請參閱 [建立里程碑路徑](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).
* **版面範本**:您可以授予群組的管理員修改配置範本的權限。 如需指示，請參閱 [授予版面範本的管理存取權](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md).

* **時間表配置檔案**:您可以授予組的管理員修改時間表配置檔案的權限。 如需詳細資訊，請參閱 [建立、編輯和分配工時單配置檔案](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

* **排程**:您可以授予群組管理員修改排程的權限。 如需詳細資訊，請參閱 [建立排程](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).
* **團隊**:您可以將組與團隊關聯，以便組及其子組的管理員可以從「組」區域查看和與這些團隊協作。 如需詳細資訊，請參閱 [建立團隊](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md) 或 [編輯團隊設定](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).
* **範本**:您可以指派群組至專案範本。 這可協助您簡化專案建立程式，並協助您更輕鬆地識別和報告擁有哪些專案範本的群組。 如需詳細資訊，請參閱 [概述](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#overview) 在文章中 [編輯專案範本](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

* **最近刪除和還原的項目**:您可以檢視及管理最近刪除的群組項目。 如需詳細資訊，請參閱 [檢視及管理群組最近刪除的項目](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-deleted-objects.md) 和 [查看和管理組最近還原的項目](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-restored-objects.md).
