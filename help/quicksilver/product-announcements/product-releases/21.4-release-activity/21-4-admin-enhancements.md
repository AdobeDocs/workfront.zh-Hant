---
title: 21.4管理員增強功能
description: 21.4管理員增強功能
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
exl-id: fc85b4c2-4a76-4226-9120-11635b03aa4e
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1882'
ht-degree: 0%

---

# 21.4管理員增強功能

本頁面說明在「預覽」環境的21.4版中進行的所有管理員增強功能。 這些增強功能將於2021年10月4日當周在生產環境中提供。

如需21.4版所有可用變更的清單，請參閱 [21.4版本概觀](../../../product-announcements/product-releases/21.4-release-activity/21.4-release-overview.md).

## 對於管理員：查看哪些組與批准流程關聯

為了幫助您了解哪些組與系統中的審批流程相關聯，我們在「設定」的「審批」頁面上的「標準」視圖中添加了「組名」列。 現在，您不必建立自訂檢視即可檢視此資訊。

如需核准程式的相關資訊，請參閱 [核准流程概述](../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

如需管理群組核准程式的相關資訊，請參閱 [組級審批流程](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

## 管理員新增功能：組可以配置自己的時間表和小時首選項

>[!NOTE]
>
>起初，在生產環境中，此功能將僅針對叢集4的客戶，在分階段推出中提供。 當功能可供其他叢集使用時，就會更新此備注。

在大型組織中，某些組可能需要單獨配置時間表和小時首選項以符合其唯一的工作流，而不是繼承由系統級別管理員配置的首選項。 現在，Workfront管理員可解除鎖定系統中所有群組的時間表和小時偏好設定，以便自行設定。

最近還針對專案偏好設定和任務和問題偏好設定新增了此功能。

有關Workfront管理員如何解除工時表和小時首選項鎖定的資訊，請參閱 [解鎖組的工時單和小時首選項](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) 在文章中 [配置工時單和小時首選項](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

有關組管理員如何配置解除鎖定任務以及發佈組首選項的資訊，請參見 [配置組的時間表和小時首選項](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

## Workfront管理員新增功能：為新Workfront體驗中自動布建的使用者設定配置範本

現在，您可以在新的Workfront體驗中為自動布建的使用者設定版面範本。 在您對應使用者屬性（「設定」>「系統」>「單一登入」）的「Workfront使用者屬性」下拉式功能表中，現在有新的「新配置範本」功能表項目可供進行此設定。 以前，您只能在Workfront Classic中為自動布建的使用者設定版面範本。

有關映射用戶屬性的說明，請參閱 [映射用戶屬性並自動布建新用戶](../../../administration-and-setup/add-users/create-and-manage-users/map-user-attributes.md).

## 新欄位會顯示您的使用者所屬的群組

現在，您很容易就能找到使用者所屬的群組。 在列出使用者的報表或檢視中，您可以使用新的「其他群組」欄位來建立欄。 此欄位列出每個用戶是其成員的組。

如需使用報表和檢視的相關資訊，請參閱 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) 和 [Adobe Workfront中的檢視概觀](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## 「藍圖詳細資訊」頁現在顯示一個映像

每個Blueprint的詳細資訊頁面現在會顯示隨Blueprint安裝的專案範本影像。 影像提供Blueprint內容的預覽，讓您知道要安裝什麼。 您可以選擇在瀏覽器中預覽完整影像或下載影像。

如需詳細資訊，請參閱 [藍圖概述](../../../administration-and-setup/blueprints/blueprints-overview.md).

![](assets/blueprint-detailspage.png)

## 新問題的Blueprint首選項

現在，某些藍圖提供了新的問題首選項。 預設會安裝這些偏好設定，但當您設定安裝詳細資訊時，可以選擇退出安裝偏好設定。

首選項包括隊列主題組、隊列主題和路由規則，以在提交問題或請求時收集正確資訊，並將問題或請求發送到正確的作業角色或團隊。 使用偏好設定有助於建立專案中擷取新問題或要求的一致性。

請注意，使用這些偏好設定時，不會將從範本建立的專案放入請求佇列中。

如需詳細資訊，請參閱 [設定Blueprint](../../../administration-and-setup/blueprints/configure-template-package.md).

## 群組管理員新增功能：查看和管理組最近刪除和還原的項目

>[!NOTE]
>
>此功能僅適用於新的Adobe Workfront體驗。

我們繼續讓您更輕鬆地在一個位置管理您的群組及其相關物件。 現在，您可以從「群組」區域檢視並處理群組最近刪除和還原的項目。 這樣您就不必轉到「設定」中的「最近刪除」或「最近恢復」區域來管理這些項。 它會保留您正在使用的群組項目清單，與系統中其他已刪除和已還原的項目分開。

如需詳細資訊，請參閱 [檢視及管理群組最近刪除的項目](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-deleted-objects.md) 和 [查看和管理組最近還原的項目](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-restored-objects.md).

## 群組管理員新增功能：群組偏好設定現在會影響群組範本

現在可更輕鬆確認群組的專案範本符合群組的需求。 在建立組時為組分配新項目模板時，該模板會從組的項目和任務首選項中繼承以下設定：

* 績效指數方法
* 狀態類型
* 排程自
* 用戶超時
* 更新類型
* 存取區段設定

在與組關聯的項目模板中建立新模板任務時，模板任務會從組的任務首選項中繼承以下設定：

* 期間類型
* 收入類型
* 成本類型

以前，項目模板和項目模板任務從系統級別設定的項目和任務首選項中繼承了這些設定。

如果您建立的模板或模板任務沒有組（例如，從主「模板」頁），則上述設定是從系統級項目和任務首選項中繼承的。 但是，如果您以後將組分配給模板或模板任務，則組的首選項不會影響它。

如需詳細資訊，請參閱文章中的偏好設定如何套用至範本和範本工作一節 [建立和修改群組的專案範本](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).

## 管理員新增功能：了解哪些自訂表單使用自訂欄位

現在，以自訂表單變更自訂欄位更輕鬆。 只要按一下自訂表單，您就可以找到其他也使用欄位的自訂表單。 您必須評估這些表單是否需要調整，以便在您進行變更後繼續正常運作。

如需詳細資訊，請參閱 [檢視使用特定自訂欄位或介面工具集的所有自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-custom-forms-that-use-a-particular-custom-field.md).

## 群組管理員新增功能：鎖定和解鎖組的項目、任務和問題首選項

現在，您可以確保組下子組中的每個人都使用相同的首選項設定，或者允許他們為其唯一的工作流配置首選項設定。

* 在Workfront管理員解除系統級首選項的鎖定後，您可以配置並鎖定組下的所有子組。 雖然您仍可以重新配置鎖定的首選項，但下子子組的管理員不能為其組重新配置。

   反之，您可以解鎖組的首選項。 這可讓子組管理員根據其用戶的獨特項目、任務或問題工作流需求進行配置。

   如需詳細資訊，請參閱 [鎖定或解除鎖定子組的項目、任務或問題首選項](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

* 如果您是Workfront管理員，則無需前往「群組」區域來設定子群組的偏好設定。 在主「項目首選項」、「任務和問題首選項」或「時間表和小時首選項」區域中，可以使用頁面頂部的搜索框查找子組並配置其首選項。

   如需詳細資訊，請參閱 [配置組的項目首選項](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) 和 [配置組的任務和問題首選項](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## 群組管理員新增功能：從「組」區域建立和編輯模板

>[!NOTE]
>
>此功能僅適用於新的Workfront體驗。

我們繼續讓您更輕鬆地在一個位置管理您的群組及其相關物件。 現在，您可以從「設定」的「群組」區域檢視及使用群組的範本。 這樣您就不必前往「範本」區域來管理群組的範本。 它保留了您正在處理的組模板的清單，而整個系統中的模板與其他模板分開。

如需詳細資訊，請參閱 [建立和修改群組的專案範本](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).

## 一次以一個附加的自訂表單輸入並儲存資訊

>[!NOTE]
>
>此功能僅適用於新的Adobe Workfront體驗。

現在，在物件的「詳細資訊」區段中提供資訊會更輕鬆：在單個自定義欄位或可擴展區域（如概述和財務）中鍵入和保存資訊，即使對象上其他自定義表單中的必需欄位尚未填寫。

以前，當您在一個自定義表單或可擴展區域中為對象輸入資訊時，附加到對象的所有自定義表單都進入編輯模式，必須先完成其所有必需欄位，然後才能保存更改。 如果您無法填寫必要欄位，因為該欄位是供其他使用者使用，就會發生問題。

如果您確實想要編輯對象的「詳細資訊」部分中的所有自定義表單和可展開區域，可以按一下新「編輯」(Edit)菜單上的「全部編輯」(Edit all)，我們將其添加到「編輯」(Edit)表徵圖中。 或者，在相同的功能表中，您可以按一下名稱以捲動至您要變更的自訂表單或區段

>[!NOTE]
>
>此功能原本發行於21.3版的「預覽」。

為了讓組織的所有層級都能更輕鬆地獨立管理和控制其工作流程，我們推出了為子組建立和管理狀態的功能。 現在，從「設定」的「群組」區段，您可以對您在任何層級管理的群組執行下列動作：

* 建立、編輯、刪除和隱藏組的狀態
* 鎖定任何組的狀態，以便其下所有較低的子組都能以相同的方式使用它
* 解鎖任何組的狀態，以便較低子組的管理員可以自定義它以滿足他們的獨特需求
* 將組狀態設定為預設狀態
* 對對象上的組狀態重新排序和隱藏顯示

Workfront管理員也可以執行這些動作（適用於所有群組）。

過去，此功能僅適用於頂層群組。

如需詳細資訊，請參閱 [管理組狀態](../../../administration-and-setup/manage-groups/manage-group-statuses/manage-group-statuses.md).

## Workfront管理員新增功能：將版面範本從Workfront Classic自行移轉至新的Workfront體驗

>[!NOTE]
>
>此功能已於2021年7月1日發佈至「預覽」環境。 它將於2021年7月15日發行至生產環境。

為協助您在使用者改用新Workfront體驗時管理版面範本，我們已建立一個按鈕，讓您將版面範本從Workfront Classic移轉至新體驗，而不需依賴Workfront客戶支援。

以前，只有Workfront客戶支援可將版面範本從Workfront Classic移轉至新的Workfront體驗。

## 將模板與組關聯時，請在「隊列詳細資訊」和「隊列主題」中選擇組批准流程

已將新選項新增至將範本與群組關聯的程式中。 現在，您可以在範本的「佇列詳細資料」或其其中一個「佇列主題」中，針對問題選取群組專屬的核准程式。

在21.3中，新增將群組範本與群組建立關聯的功能時，您可以在範本中選取群組專屬的核准程式，但無法在範本的「佇列詳細資料」或「佇列主題」中選取。

如需詳細資訊，請參閱 [將新審批流程或現有審批流程與工作關聯](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
