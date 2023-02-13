---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3其他增強功能
description: 本頁說明在生產環境的20.3版中所做的所有其他增強功能。 這些增強功能已於2020年8月10日當周在生產環境中推出。
author: Luke
feature: Product Announcements
exl-id: 6fef7261-114f-4c26-861e-61a4acb22d40
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1510'
ht-degree: 0%

---

# 20.3其他增強功能

本頁說明在生產環境的20.3版中所做的所有其他增強功能。 這些增強功能已於2020年8月10日當周在生產環境中推出。

如需20.3版所有可用變更的清單，請參閱 [20.3版本概觀](../../../product-announcements/product-releases/20.3-release-activity/20.3-release-overview.md).

## 與私人連結共用日曆

若要減輕在Workfront中共用日曆的負擔，您可以共用將使用者直接帶至日曆的私人連結。 日曆必須與用戶共用，用戶必須登錄才能查看。

過去，您可以共用不需要登入即可檢視的公用URL。

如需詳細資訊，請參閱 [共用日曆報表](../../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md).

## 建立請求時的「新草稿」區域

為了在處理請求時提供更大的彈性，Workfront現在會自動儲存您在新「草稿」區域中以草稿形式建立的所有請求。 如果您沒有完成新請求所需的所有資訊，可以將其保留為草稿，返回並稍後完成。 Workfront會在新的「草稿」區域中，為每個佇列主題儲存一個請求。 在您準備好完成並提交草稿請求之前，您可以視需要儲存草稿請求。 您也可以使用「佈局模板」(Layout Template)移除或重新定位左側面板中的「草稿」區域。

如需建立請求的詳細資訊，請參閱 [建立及提交Workfront請求](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

>[!NOTE]
>
>在預覽版本中，如果您有指派給您的自訂配置範本，則需要修改配置範本，以新增請求的「草稿」區域。

## 展開或折疊工時單上的項

>[!NOTE]
>
>此功能僅適用於新的Adobe Workfront體驗

為幫助您輕鬆管理包含多個項目的工時單，您現在可以按一下按鈕展開或折疊所有項目。

之前，您必須個別按一下每個項目。

如需詳細資訊，請參閱 [記錄時間](../../../timesheets/create-and-manage-timesheets/log-time.md).

## 忽略Workfront日曆中的實際日期

>[!NOTE]
>
>2020年6月5日發佈至「預覽」環境的功能。 此功能將於2020年6月19日在生產環境中推出。

若要讓您更能控制物件在日曆報表中的顯示方式，您可以選擇忽略實際日期，即使這些日期可用亦然。

以前，日曆會在日期可用後自動使用實際日期。

如需詳細資訊，請參閱 [日曆報表概觀](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

## 在日曆報表中使用自訂日期欄位

>[!NOTE]
>
>2020年5月29日發佈至「預覽」環境的功能。 2020年6月12日起將可在生產環境中使用。

為協助您透過日曆更形象化地管理日常工作，自訂日期欄位現在提供日期選項。

以前，您只能在實際日期不可用時，使用預計的計畫日曆來管理日曆。

如需詳細資訊，請參閱 [在日曆報表中使用自訂日期欄位](../../../reports-and-dashboards/reports/calendars/use-custom-dates.md) (或者，如果您使用Workfront Classic，請參閱 [在日曆報表中使用自訂日期欄位](https://one.workfront.com/s/article/Use-custom-date-fields-in-a-calendar-report-432597950?language=en_US))。

## 電子郵件變更

**傳出電子郵件變更：** 來自Workfront的所有電子郵件將來自notifications@my.workfront.com。 這包括自動警報和用戶與用戶的通信。

以前，系統管理員可以在「電子郵件設定」區域新增自訂電子郵件地址。

**傳入電子郵件POP回覆變更：** 系統管理員將無法再為傳入的電子郵件對通知的回覆設定自訂POP電子郵件伺服器。

如需詳細資訊，請參閱 [電子郵件欺騙和POP回覆電子郵件變更](https://one.workfront.com/s/article/Email-spoofing-and-POP-reply-email-changes?language=en_US).

## 傳出的Workfront電子郵件現已包含DomainKeys Indified Mail(DKIM)

所有傳出電子郵件都會包含電子郵件驗證技術(DKIM)。 此DKIM簽名不會顯示給最終用戶，但允許在伺服器級別進行驗證，並增強我們現有的驗證框架。

## 更新新Workfront體驗的註冊

為了讓新Workfront體驗中的使用者註冊更容易管理，群組管理員現在可以存取註冊和取消註冊屬於他們所管理群組的使用者。

現在也提供使用者詳細資訊連結，可顯示下列使用者資訊：

* 名稱
* 工作角色
* 電子郵件地址
* 個人資料圖片

## 管理員新增功能：品牌Workfront，適用於特定群組、團隊、工作角色和使用者

>[!NOTE]
>
>此功能僅適用於新的Adobe Workfront體驗

現在，您可以使用「版面範本」，針對具有自己品牌的特定群組、團隊、工作角色和使用者，變更頂端導覽區域和主功能表中的標誌。

如需詳細資訊，請參閱 [品牌化您的Adobe Workfront執行個體](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).

## 群組管理員可以建立和管理核准程式

為了獲得更多自治權並控制其組的工作流，組管理員現在可以訪問「設定」中的「批准流程」區域，並建立和編輯他/她管理的組的批准流程。 這些核准程式是根據該群組的狀態。

為了確保群組管理員不會不慎編輯整個系統使用或由其他群組建立的核准程式，他們只能存取與其所管理群組相關聯的核准程式。

如需詳細資訊，請參閱 [建立工作項的審批流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## 對於管理員：「新增群組」頁面可讓您更輕鬆建立和管理群組

由於新的「群組」頁面上顯示了群組管理員所需的所有內容，因此群組管理員現在可更輕鬆地管理群組。 您不再需要在各種覆蓋方塊和「設定」頁面之間導覽，即可建立和修改群組。

主要重點如下：

* 組詳細資訊：查看和編輯有關組的基本資訊，如組名、說明、組管理員的名稱，以及組是公用還是專用的。
* 組成員清單：查看所有組成員，並使用新工具欄快速添加、刪除、導出、激活和停用成員資格。 您也可以編輯成員的配置檔案併發送更新注釋。
* 標題中的「組管理員」欄位：查看您管理的組時，快速分配或取消分配組成員作為組的管理員。 您也可以使用新的「群組角色」欄，在群組成員清單中執行此操作。
* 子組清單：查看、編輯、複製、導出和刪除您管理的組中的子組。
* 狀態清單：檢視及管理群組的狀態。

如需詳細資訊，請參閱 [建立群組](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

## 管理員新增功能：建立多達14個級別的子組

為了更方便地組織您的Workfront群組，以符合您的組織階層，我們將您可在群組中建立的子群組層級從3個提升至14個。

如需詳細資訊，請參閱 [群組概觀](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

## 管理員新增功能：新設定側欄

>[!NOTE]
>
>此功能僅適用於新的Adobe Workfront體驗

「設定」中的左側邊欄現在更快速、更容易使用，並運用您已知的基本版面和功能。 除了更現代的外觀和感覺，還有以下新鮮之處：

* 側欄中新的非白色背景，可讓您更輕鬆區分「設定」區域的其餘部分。
* 側欄中的表徵圖比較大，有些經過重新設計，以更清楚地說明選項的作用。
* 側邊欄項目之間的垂直空間越多，閱讀就越容易。
* 當您需要主區域中的空間來查看和執行更多操作（如查看其他列）時，可以折疊側欄。 當需要查看功能名稱時，您可以再次展開側欄。
* 邊欄收合時，您只會看到每個功能的圖示。 若要在主要側欄項目下查看子項目，請將滑鼠指標暫留在其圖示上，以在彈出式功能表中顯示。 例如，將滑鼠指標暫留在「處理」圖示上，以顯示包含「核准」和「里程碑路徑」的功能表。
* 您可以更快地按一下，存取兩個「開始」選項（「匯入資料」和「匯出資料」）。 它們已從「系統」下移出，以顯示在側欄的主要層級。

有關如何使用「設定」區域的資訊，請參閱 [管理與設定](../../../administration-and-setup/administration-and-setup.md).

## 在「客戶資訊」區域中包含群集號

身為Workfront管理員，您現在可以輕鬆找到Workfront內的叢集號碼，不必再花更多時間和精力從我們的支援團隊取得叢集號碼。 我們在「設定」的「客戶資訊」區域中新增「叢集設定」欄位。

有關「客戶資訊」區域的資訊，請參閱 [配置系統的基本資訊](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

## 事件訂閱的Base64編碼

base64Encoding欄位是可選欄位，用於啟用事件訂閱負載的Base64編碼。 如果使用設為true的base64Encoding欄位來提出要求，則裝載中的newState和oldState物件會以Base64編碼字串的形式傳送。 如果您的網路設定為在「事件訂閱」中不允許特殊字元，則此功能會很實用。

如需詳細資訊，請參閱 [事件訂閱API](../../../wf-api/general/event-subs-api.md).

## 移除建立重複事件訂閱的功能

為防止傳送重複訊息，您無法再建立重複訂閱。 此外，先前建立的任何重複訂閱均已移除。

如需詳細資訊，請參閱 [常見問題集 — 事件訂閱](../../../wf-api/general/event-subs-faq.md).
