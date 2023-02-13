---
title: 22.1管理員增強功能
description: 22.1管理員增強功能
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
exl-id: 63ff1334-aebe-4df4-a855-10011707808b
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1496'
ht-degree: 0%

---

# 22.1管理員增強功能

本頁面說明在「預覽」環境的22.1版中進行的所有管理員增強功能。 這些增強功能將可在生產環境中使用

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

2022年1月17日當周。

如需22.1版所有可用變更的清單，請參閱 [22.1版本概觀](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## 記錄在「更新」區域中的文檔下載

為協助您的使用者追蹤其在Workfront中儲存的檔案下載，系統現在會在有人下載檔案時，於「更新」區域中記錄檔案項目。

>[!NOTE]
>
>建議您在新上傳檔案的預覽中測試此功能。

如需Workfront如何記錄物件自動更新的詳細資訊，請參閱 [系統追蹤更新](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

## 使用存取層級授予團隊的存取權

「存取層級」區域的新區段可讓您以更精細的控制方式管理使用者對團隊的存取。 現在您可以決定可以建立、編輯和檢視團隊的人員。

這不會變更使用者對團隊的現有存取權。

<!--
For more information, see [Grant access to teams](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md).
-->

## Blueprint中現在提供組映射

現在，有些藍圖包括組，您可以在安裝藍圖之前對其進行自定義。 您可以將Blueprint中的群組對應至Workfront例項中的現有群組，或視需要建立新群組。

如需詳細資訊，請參閱 [設定Blueprint](../../../administration-and-setup/blueprints/configure-template-package.md).

## 自訂Forms區域中的樣式更新

「自訂Forms」區域具有新的外觀，可與新Workfront體驗中的許多其他區域更新。

如需建立自訂表單的相關資訊，請參閱 [建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## 建立計算自訂欄位的許多增強功能

在新的計算編輯器中新增以下內容，現在建立計算自訂欄位更為輕鬆：

* 您可以將滑鼠移至計算中的任何運算式上，以顯示其相關資訊，包括說明、其使用方式範例，以及說明文章中詳細資訊的連結。
* 您新增的每個運算式都會以色彩編碼，視其類型而定。 這可讓您更容易找出運算式，並立即辨識其類型。
* 行號有助於您識別和參考長計算中的函式。
* 開始輸入運算式或欄位名稱時，會顯示可用項目清單，以便您選擇所要的項目。 而且，當您鍵入左括弧時，將自動添加右括弧。
* 您可以使用現有對象來預覽計算結果，而無需離開計算編輯器。

此外，在可自訂的「指示」中，將滑鼠移至計算自訂欄位的文字中，您可以顯示或隱藏欄位的公式。 如果您認為填寫自訂表單的使用者不需要該資訊，這個功能就十分實用。

如需建立計算自訂欄位的詳細資訊，請參閱 [將計算資料新增至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## 查看有關狀態和公司的審核日誌資訊

現在，您可以在「設定」的「稽核記錄」區域中檢視狀態和公司的相關資訊，以更輕鬆地疑難排解這些事件。

例如：

* 您可以找出重新命名、鎖定或隱藏狀態的人，以及他們執行此動作的時間。
* 您可以了解哪些人從公司中移除了某些成員或工作角色，以及他們刪除這些角色的時間。

有關查看審核日誌資訊的資訊，請參閱 [查看和導出審核日誌](../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## Blueprint公司映射和其他增強功能

現在提供了以下Blueprint增強功能：

* 現在，有些藍圖包括公司，您可以在安裝藍圖之前對其進行自定義。 您可以將Blueprint中的公司對應至Workfront例項中的現有公司，或視需要建立新公司。
* 現在提供新的Blueprint類型「組織結構」。 有些藍圖包括來自多種類型的元素（例如，項目模板和組織結構）。 您可以在目錄頁面上依Blueprint類型篩選。
* 為簡單起見，設定頁面上的「安裝偏好設定」和「範本擁有權」區段已結合為「範本偏好設定」。

如需詳細資訊，請參閱 [設定Blueprint](../../../administration-and-setup/blueprints/configure-template-package.md).

## 更輕鬆管理公司會籍

在「公司」區域中，更新的工具列可讓您輕鬆將現有的Workfront使用者新增至公司，以及移除公司成員。

以前，這些動作只能在「編輯公司」方塊中使用。

更新的工具欄還包含以前工具欄中提供的所有操作，例如編輯成員的用戶配置檔案資訊並在系統中將其停用。

如需詳細資訊，請參閱 [管理公司會籍](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).

## 在新計算欄位窗口中選擇表達式和欄位

我們將繼續讓以自訂表單建立計算欄位更輕鬆。 現在，當按一下「最大化」以開啟新的計算編輯器時，您可以找到並選取所需的運算式和欄位。

如需詳細資訊，請參閱 [將計算資料新增至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## 組可以配置自己的時間表和小時首選項

>[!NOTE]
>
>此功能最初是分階段推出的一部分，但第21.4發行版本僅適用於叢集4的客戶。 2021年11月8日，此功能將適用於生產環境中的所有剩餘叢集。

在大型組織中，某些組可能需要單獨配置時間表和小時首選項以符合其唯一的工作流，而不是繼承由系統級別管理員配置的首選項。 現在，Workfront管理員可解除鎖定系統中所有群組的時間表和小時偏好設定，以便自行設定。

最近還針對專案偏好設定和任務和問題偏好設定新增了此功能。

有關Workfront管理員如何解除工時表和小時首選項鎖定的資訊，請參閱 [解鎖組的工時單和小時首選項](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) 在文章中 [配置工時單和小時首選項](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

有關組管理員如何配置解除鎖定任務以及發佈組首選項的資訊，請參見 [配置組的時間表和小時首選項](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

## 選擇要解除鎖定或重新鎖定組的多個通知

現在，解鎖或重新鎖定群組的電子郵件通知更快速更輕鬆。 現在，您可以選取多個通知、檢查您的選取項目以確定它們正確無誤，然後按一下工具列中顯示的新「解除鎖定」或「鎖定」按鈕。

之前，您必須一次解鎖並重新鎖定通知。 Workfront目前有95個通知，因此若您必須全部或許多通知，這需要一段時間。

如需詳細資訊，請參閱 [解鎖或鎖定所有組的事件通知配置](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).

## 對於群組管理員：刪除群組時，可更輕鬆選取取代群組

刪除組時，「刪除組」(Delete Group)框中的兩項改進使您能夠更輕鬆地選擇要保留已刪除組的用戶、工作項和子組的替換組：

* 您可以開始輸入群組名稱以快速找到。 之前，只有下拉式清單無法輸入。 對於具有許多群組的組織而言，這有問題，因為您必須捲動清單才能找到您想要的群組。 此外，下拉式清單中也有項目限制，因此可能沒有顯示您想要的群組。
* 您可以使用新資訊圖示，確定您正在選取想要的取代群組。 將滑鼠指標暫留在圖示上，會顯示列出群組相關資訊的工具提示，例如上方的群組階層及其管理員姓名。

如需詳細資訊，請參閱 [刪除群組](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md).

## 建立計算欄位的較大區域

現在，在自訂表單中建立複雜的計算欄位更輕鬆。 按一下新的「最大化」按鈕，開啟用於建立計算的大型編輯窗口。 完成後，按一下「最小化」以繼續使用自訂表單。

如需詳細資訊，請參閱 [將計算資料新增至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## 將自訂表單新增至群組

「群組」物件現在支援自訂表單。 這可讓您組織中的群組更容易擷取和分享符合其特定需求和工作流程的資訊。 使用者可對群組執行下列操作，就像對其他Workfront物件一樣：

* 建立自訂表單
* 附加自訂表單
* 儲存自訂表單資料
* 移除自訂表單
* 從清單中編輯自訂資料，並在新的Workfront體驗中，從群組頁面編輯自訂資料

如需自訂表單的相關資訊，請參閱 [自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md).

## 建立OAuth2應用程式以整合應用程式與Workfront

現在，您可以將Workfront與Workfront未提供內建整合的其他應用程式整合。 透過為您要整合的應用程式建立OAuth2應用程式，您可讓該應用程式存取Workfront，同時知道您的資料受到安全、業界標準的OAuth2驗證通訊協定保護。

過去，您只能透過內建整合、Workfront Fusion或Workfront API來與其他應用程式整合。

如需詳細資訊，請參閱 [建立OAuth2應用程式以進行Workfront整合](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## 「公司」區域中的介面文字改良

在「設定」的「公司」區域中，新的確認訊息和略微的措辭變更，可讓管理公司會籍更為輕鬆。 例如，左側面板中名為「People」的區段現在是「公司成員」。

有關管理公司成員資格的資訊，請參見 [管理公司會籍](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).
