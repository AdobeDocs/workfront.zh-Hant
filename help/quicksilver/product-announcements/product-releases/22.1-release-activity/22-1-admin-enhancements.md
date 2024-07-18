---
title: 22.1管理員增強功能
description: 22.1管理員增強功能
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: 63ff1334-aebe-4df4-a855-10011707808b
source-git-commit: ccba3a3d7c0cac50dbd29cae677b076811904a91
workflow-type: tm+mt
source-wordcount: '1505'
ht-degree: 0%

---

# 22.1管理員增強功能

本頁說明22.1版對預覽環境所做的所有管理員增強功能。 這些增強功能將在生產環境中提供

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

2022年1月17日當週。

如需22.1版本可用的所有變更清單，請參閱[22.1版本總覽](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md)。

## 檔案下載記錄到更新區域

為協助您的使用者追蹤他們儲存在Workfront中的檔案下載情形，系統現在會在有人下載檔案時，在更新區域記錄檔案的專案。

>[!NOTE]
>
>我們建議在新上傳檔案的「預覽」中測試此功能。

如需Workfront如何記錄物件的自動更新資訊，請參閱[系統追蹤的更新](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md)。

## 使用存取層級授予團隊存取權

存取層級區域的新區段可讓您更精細地控制來管理使用者對團隊的存取權。 現在您可以決定誰可以建立、編輯和檢視團隊。

這不會變更您使用者對團隊的現有存取權。

<!--
For more information, see [Grant access to teams](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md).
-->

## Blueprint現在提供群組對應

部分Blueprint現在包含群組，您可以在安裝Blueprint之前進行自訂。 您可以將Blueprint中的群組對應至Workfront例項中的現有群組，或視需要建立新群組。

如需詳細資訊，請參閱[設定藍圖](../../../administration-and-setup/blueprints/configure-template-package.md)。

## 自訂Forms區域中的樣式更新

自訂Forms區域具有新外觀，可讓您與新Workfront體驗中的許多其他區域同步更新。

如需建立自訂表單的相關資訊，請參閱[建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)。

## 建立計算自訂欄位的多項增強功能

現在，透過新計算編輯器中的這些新增內容，建立計算自訂欄位變得更加容易：

* 您可以將滑鼠停留在計算中的任何運算式上，以顯示其相關資訊，包括說明、使用方式的範例，以及說明文章中更多資訊的連結。
* 您新增的每個運算式都會根據其型別以不同色彩標示。 這可讓您更輕鬆地找出運算式並立即辨識其型別。
* 行號可協助您識別並參考長計算中的函式。
* 當您開始輸入運算式或欄位名稱時，可用的專案清單會顯示出來，以便您選擇想要的專案。 而且，當您鍵入左括弧時，右括弧會自動新增。
* 您可以使用現有的物件來預覽計算結果，而不需離開計算編輯器。

此外，在可自訂的「指示」中，將計算自訂欄位的文字暫留，您可以顯示或隱藏欄位的公式。 如果您認為填寫自訂表單的使用者不需要該資訊，這將很有用。

如需建立計算自訂欄位的詳細資訊，請參閱[將計算資料新增至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)。

## 檢視有關狀態和公司的稽核記錄資訊

現在，您可以在「設定」的「稽核記錄」區域中檢視有關狀態和公司的資訊，更輕鬆地疑難排解有關它們的事件。

例如：

* 您可以瞭解重新命名、鎖定或隱藏狀態的人員及其時間。
* 您可以瞭解誰從公司中移除了一些成員或工作角色，以及何時移除。

如需有關檢視稽核記錄資訊的資訊，請參閱[檢視和匯出稽核記錄](../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md)。

## 藍圖公司對應和其他增強功能

現已推出下列Blueprint增強功能：

* 部分Blueprint現在包含公司，您可以在安裝Blueprint前進行自訂。 您可以將Blueprint中的公司對應至Workfront執行個體中的現有公司，或視需要建立新公司。
* 現已提供新的Blueprint型別「組織結構」。 某些Blueprint包含來自多種型別的元素（例如，專案範本和組織結構）。 您可以在目錄頁面上按Blueprint型別進行篩選。
* 為簡單起見，設定頁面上的「安裝偏好設定」和「範本所有權」區段已合併到「範本偏好設定」。

如需詳細資訊，請參閱[設定藍圖](../../../administration-and-setup/blueprints/configure-template-package.md)。

## 更輕鬆地管理公司成員資格

在公司區域，更新的工具列可讓您輕鬆將現有Workfront使用者新增到公司以及移除公司成員。

以前，這些動作只能在編輯公司方塊中使用。

更新的工具列也包含先前工具列中可用的所有動作，例如編輯成員的使用者設定檔資訊，以及在系統中停用它們。

如需詳細資訊，請參閱[管理公司成員資格](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md)。

## 在新的計算欄位視窗中選取運算式和欄位

我們繼續讓您更輕鬆地在自訂表單中建立計算欄位。 現在，當您按一下「最大化」開啟新的「計算編輯器」時，您可以找到並選取所需的運算式和欄位。

如需詳細資訊，請參閱[將計算資料新增至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)。

## 群組可以設定自己的時程表和小時偏好設定

>[!NOTE]
>
>此功能最初僅作為21.4版的一部分提供給叢集4上的客戶作為分階段推出的一部分提供。 此功能將在2021年11月8日提供給生產環境中的所有其餘叢集。

在大型組織中，某些群組可能需要單獨設定時程表和小時偏好設定以符合其獨特的工作流程，而不是繼承系統管理員在系統層級設定的偏好設定。 現在，Workfront管理員可以解鎖系統中所有群組的時程表和小時偏好設定，以便他們能夠自行設定。

此功能最近也針對專案偏好設定以及任務和問題偏好設定新增。

如需Workfront管理員如何解除鎖定時程表和小時偏好設定的相關資訊，請參閱[設定時程表和小時偏好設定](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)一文中的[解除鎖定群組的時程表和小時偏好設定](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock)小節。

如需有關群組管理員如何設定群組的解除鎖定任務和問題偏好設定的資訊，請參閱[設定群組的時程表和小時偏好設定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md)。

## 選取您要解除鎖定或重新鎖定群組的多個通知

現在，解鎖或重新鎖定群組的電子郵件通知變得更加快速和輕鬆。 現在您可以選取多個通知，檢查您的選取以確定它們是否正確，然後按一下工具列中顯示的新「解除鎖定」或「鎖定」按鈕。

之前，您必須一次解鎖並重新鎖定一個通知。 Workfront目前有95項通知，因此如果您必須針對全部或多項通知，則需要一段時間才能完成。

如需詳細資訊，請參閱[解除鎖定或鎖定所有群組的事件通知設定](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md)。

## 對於群組管理員：刪除群組時，可更輕鬆選取替代群組

當您刪除群組時，「刪除群組」方塊中的兩項改善可讓您更輕鬆地選取要保留已刪除群組使用者、工作專案和子群組的取代群組：

* 您可以開始輸入群組的名稱，以快速找到它。 先前只有下拉式清單無法輸入。 對於擁有許多群組的組織來說，這會造成問題，因為您必須捲動清單來尋找您想要的群組。 此外，下拉式清單具有專案限制，因此您想要的群組可能不會顯示。
* 您可以使用新資訊圖示來確保選取您想要的取代群組。 將滑鼠指標暫留在圖示上會顯示工具提示，其中列出群組的相關資訊，例如群組上方的階層以及其管理員的姓名。

如需詳細資訊，請參閱[刪除群組](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md)。

## 用於建立計算欄位的較大區域

現在，在自訂表單中建立複雜的計算欄位變得更加容易。 按一下新的「最大化」按鈕，開啟一個大型編輯視窗以建立您的計算。 完成後，按一下「最小化」以繼續處理自訂表單。

如需詳細資訊，請參閱[將計算資料新增至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)。

## 新增自訂表單至群組

群組物件現在支援自訂表單。 這可讓您組織中的群組更輕鬆地擷取及共用符合其特定需求和工作流程的資訊。 使用者可以對群組執行下列動作，就像對其他Workfront物件一樣：

* 建立自訂表格
* 附加自訂表單
* 儲存自訂表單資料
* 移除自訂表格
* 編輯清單中的自訂資料，並在新的Workfront體驗中，從群組頁面編輯自訂資料

如需自訂表單的相關資訊，請參閱[自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md)。

## 建立OAuth2應用程式以將應用程式與Workfront整合

現在，您可以將Workfront與Workfront未提供內建整合的其他應用程式整合。 透過為您要整合的應用程式建立OAuth2應用程式，您可以允許該應用程式存取Workfront，同時瞭解您的資料受到安全且符合產業標準的OAuth2驗證通訊協定保護。

之前，您只能透過內建整合、Workfront Fusion或Workfront API來與其他應用程式整合。

如需詳細資訊，請參閱[為Workfront整合建立OAuth2應用程式](../../../administration-and-setup/configure-integrations/create-oauth-application.md)。

## 公司區域的介面文字改善

在「設定」的「公司」區域中，新的確認訊息和細微的措辭變更可讓您更輕鬆地管理公司成員資格。 例如，左側面板中的區段名稱「People」現在是「公司成員」。

如需有關管理公司成員資格的資訊，請參閱[管理公司成員資格](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md)。
