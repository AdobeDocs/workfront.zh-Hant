---
title: 21.4管理員增強功能
description: 21.4管理員增強功能
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: fc85b4c2-4a76-4226-9120-11635b03aa4e
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1891'
ht-degree: 0%

---

# 21.4管理員增強功能

本頁說明21.4版對預覽環境所做的所有管理員增強功能。 這些增強功能將在2021年10月4日當週的生產環境中提供。

如需21.4版本可用的所有變更清單，請參閱[21.4版本總覽](../../../product-announcements/product-releases/21.4-release-activity/21-4-release-overview.md)。

## 對於管理員：檢視與核准流程相關聯的群組

為協助您找出哪些群組與系統中的核准流程相關聯，我們在「設定」的「核准」頁面上，將「群組名稱」欄新增至「標準」檢視。 現在，您無需建立自訂檢視即可檢視此資訊。

如需核准程式的資訊，請參閱[核准程式概觀](../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md)。

如需有關管理群組核准流程的資訊，請參閱[群組層級核准流程](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md)。

## 管理員的新增功能：群組可以設定自己的時程表和小時偏好設定

>[!NOTE]
>
>最初，在生產環境中，此功能將僅作為分階段推出的一部分，提供給叢集4上的客戶。 當功能可供其他叢集使用時，將會更新此附註。

在大型組織中，某些群組可能需要單獨設定時程表和小時偏好設定以符合其獨特的工作流程，而不是繼承系統管理員在系統層級設定的偏好設定。 現在，Workfront管理員可以解鎖系統中所有群組的時程表和小時偏好設定，以便他們能夠自行設定。

此功能最近也針對專案偏好設定以及任務和問題偏好設定新增。

如需Workfront管理員如何解除鎖定時程表和小時偏好設定的相關資訊，請參閱[設定時程表和小時偏好設定](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)一文中的[解除鎖定群組的時程表和小時偏好設定](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock)小節。

如需有關群組管理員如何設定群組的解除鎖定任務和問題偏好設定的資訊，請參閱[設定群組的時程表和小時偏好設定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md)。

## Workfront管理員的新增功能：在新的Workfront體驗中為自動布建的使用者設定版面範本

現在您可以在新的Workfront體驗中設定版面配置範本，供自動布建的使用者使用。 在對應使用者屬性的Workfront「使用者屬性」下拉式功能表中（「設定」>「系統」>「單一登入」），新的「全新配置範本」功能表專案現在可用於進行此設定。 之前，您只能在Workfront Classic中為自動布建的使用者設定版面範本。

如需對應使用者屬性的指示，請參閱[對應使用者屬性和自動布建新使用者](../../../administration-and-setup/add-users/create-and-manage-users/map-user-attributes.md)。

## 新欄位顯示您的使用者所屬的群組

現在，您可輕鬆瞭解使用者屬於哪些群組。 在列出使用者的報表或檢視中，您可以使用新的「其他群組」欄位來建立欄。 此欄位會列出每個使用者所屬的群組。

如需有關使用報告和檢視的資訊，請參閱[在Adobe Workfront中建立自訂報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)和[檢視總覽](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)。

## 藍圖詳細資訊頁面現在會顯示影像

現在，每個Blueprint的詳細資訊頁面都會顯示與Blueprint一起安裝的專案範本影像。 此影像提供Blueprint內容的預覽，讓您知道要安裝的內容。 您可以選擇在瀏覽器中預覽完整影像或下載影像。

如需詳細資訊，請參閱[藍圖概觀](../../../administration-and-setup/blueprints/blueprints-overview.md)。

![](assets/blueprint-detailspage.png)

## 新問題的藍圖偏好設定

某些Blueprint現在提供新的問題偏好設定。 預設會安裝偏好設定，但當您設定安裝詳細資訊時，可以選擇退出安裝偏好設定。

偏好設定包括佇列主題群組、佇列主題和路由規則，可在提交問題或請求時收集正確資訊，並將問題或請求傳送給正確的工作角色或團隊。 使用偏好設定有助於在專案上擷取新問題或請求的方式建立一致性。

請注意，使用這些偏好設定不會將從範本建立的專案放入請求佇列。

如需詳細資訊，請參閱[設定藍圖](../../../administration-and-setup/blueprints/configure-template-package.md)。

## 群組管理員的新增功能：檢視及管理群組最近刪除及還原的專案

>[!NOTE]
>
>此功能僅在新的Adobe Workfront體驗中可用。

我們持續讓您更輕鬆地集中管理群組及其相關物件。 現在，您可以從「群組」區域檢視和使用群組最近刪除和還原的專案。 這可讓您無須前往「設定」中的「最近刪除」或「最近還原」區域來管理這些專案。 而且它會將您正在使用的群組專案清單與系統中其他已刪除和還原的專案分開。

如需詳細資訊，請參閱[檢視和管理群組最近刪除的專案](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-deleted-objects.md)和[檢視和管理群組最近還原的專案](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-restored-objects.md)。

## 群組管理員的新增功能：群組偏好設定現在會影響群組範本

現在，可以更輕鬆確定您群組的專案範本符合您群組的需求。 當您在建立群組時將新專案範本指派給群組時，範本會繼承群組專案和任務偏好設定的下列設定：

* 績效指數方法
* 狀況類型
* 排程開始日期
* 使用者休假
* 更新型別
* 存取區段設定

在與群組相關聯的專案範本中建立新範本任務時，範本任務會繼承群組任務偏好設定的下列設定：

* 期間類型
* 收入類型
* 成本類型

以前，專案範本和專案範本任務從系統層級設定的專案和任務偏好設定繼承這些設定。

如果您建立沒有群組的範本或範本任務（例如，從主「範本」頁面），則上述設定會繼承自系統層級的專案和任務偏好設定。 但是，如果您稍後將群組指派給範本或範本任務，群組的偏好設定不會影響它。

如需詳細資訊，請參閱文章[建立及修改群組的專案範本](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md)中的「偏好設定如何套用至範本和範本任務」一節。

## 管理員的新增功能：瞭解哪些自訂表單正在使用自訂欄位

現在變更自訂表單中的自訂欄位更容易。 只要在自訂表單中按一下，您就可以找到有關也使用該欄位的任何其他自訂表單。 請務必評估這些表單是否需要調整，以便在您進行變更後能夠繼續正常運作。

如需詳細資訊，請參閱[檢視使用特定自訂欄位或Widget](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-custom-forms-that-use-a-particular-custom-field.md)的所有自訂表單。

## 群組管理員的新增功能：鎖定和解鎖群組的專案、任務和問題偏好設定

現在，您可以確保群組下方子群組中的每個人都使用相同的偏好設定，或者您可以允許他們為其唯一的工作流程設定偏好設定。

* Workfront管理員在系統層級解除鎖定偏好設定後，您就可以為群組下的所有子群組設定並鎖定它。 雖然您仍然可以重新設定鎖定的偏好設定，但較低子群組的管理員無法為其群組這麼做。

  反之，您可以解鎖群組的偏好設定。 這允許子群組管理員根據其使用者獨特的專案、任務或問題工作流程需求來設定它。

  如需詳細資訊，請參閱[鎖定或解除鎖定子群組的專案、任務或問題偏好設定](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md)。

* 如果您是Workfront管理員，就不需要前往「群組」區域設定子群組的偏好設定。 從主要專案偏好設定、任務和問題偏好設定或時程表和時數偏好設定區域，您可以使用頁面頂端的搜尋方塊來尋找子群組並設定其偏好設定。

  如需詳細資訊，請參閱[設定群組的專案偏好設定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)和[設定群組的任務和問題偏好設定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)。

## 群組管理員的新增功能：從群組區域建立和編輯範本

>[!NOTE]
>
>此功能僅在新的Workfront體驗中可用。

我們持續讓您更輕鬆地在一個位置管理群組及其關聯的物件。 現在您可以從「設定」的「群組」區域檢視和使用群組的範本。 這可讓您無須前往「範本」區域來管理群組的範本。 而且它會將您正在處理的群組範本清單與整個系統中的其他群組範本清單分開。

如需詳細資訊，請參閱[建立和修改群組的專案範本](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md)。

## 一次在一個附加的自訂表單中輸入並儲存資訊

>[!NOTE]
>
>此功能僅在新的Adobe Workfront體驗中可用。

現在，在物件的詳細資訊區段中提供資訊變得更加容易：在單一自訂欄位或可展開區域（例如Overview和Finance）中輸入並儲存資訊，即使物件上其他自訂表單中的必填欄位尚未填寫。

先前，當您在一個自訂表單或物件的可展開區域中輸入資訊時，附加到物件的所有自訂表單都會進入編輯模式，而且您必須先完成其所有必填欄位，然後才能儲存變更。 如果您因為某個必填欄位是提供給其他使用者而無法完成，則會發生問題。

如果您確實想要編輯物件「詳細資訊」區段中的所有自訂表單和可展開區域，您可以按一下新增至「編輯」圖示的新「編輯」選單上的「全部編輯」。 或者，在相同功能表上，您可以按一下名稱，捲動至您要變更的自訂表單或區段

>[!NOTE]
>
>此功能最初是在21.3版發行的「預覽」功能。

為了更方便組織的所有層級獨立管理和控制其工作流程，我們引進了建立和管理子群組狀態的功能。 現在，您可以從「設定」的「群組」區段，為您在任何層級上管理的群組執行下列動作：

* 建立、編輯、刪除和隱藏群組的狀態
* 鎖定任何群組的狀態，以便其下方的所有較低子群組可以相同方式使用它
* 解鎖任何群組的狀態，以便較低子群組的管理員可以自訂該狀態以滿足其獨特需求
* 將群組狀態設定為預設狀態
* 重新排序和隱藏物件上群組狀態的顯示

Workfront管理員也可以（針對所有群組）執行這些操作。

以前，此功能僅適用於頂層群組。

如需詳細資訊，請參閱[管理群組狀態](../../../administration-and-setup/manage-groups/manage-group-statuses/manage-group-statuses.md)。

## Workfront管理員的新功能：自行將版面範本從Workfront Classic移轉至新的Workfront體驗

>[!NOTE]
>
>此功能已於2021年7月1日發佈到預覽環境。 它將於2021年7月15日發佈到生產環境。

為協助您在使用者切換使用新Workfront體驗時管理版面範本，我們已建立按鈕，您可以使用它將版面範本從Workfront Classic移轉到新體驗，而不依賴Workfront客戶支援。

之前，只有Workfront客戶支援可將您的版面配置範本從Workfront Classic移轉到新的Workfront體驗。

## 將範本與群組產生關聯時，在佇列詳細資料和佇列主題中選取群組核准程式

我們在建立範本與群組的關聯程式中，新增了一個選項。 現在，您可以在範本的「佇列詳細資訊」或其中一個佇列主題中，為問題選取群組特定的核准流程。

在21.3中，當我們新增將群組範本與群組建立關聯的功能時，您可以在範本中選取群組特定的核准程式，但您無法在範本的「佇列詳細資訊」或「佇列主題」中執行此操作。

如需詳細資訊，請參閱[將新的或現有的核准程式與工作建立關聯](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)。
