---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3其他增強功能
description: 本頁說明生產環境第20.3發行版本所做的所有其他增強功能。 這些增強功能已在2020年8月10日當週的生產環境中推出。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6fef7261-114f-4c26-861e-61a4acb22d40
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1503'
ht-degree: 0%

---

# 20.3其他增強功能

本頁說明生產環境第20.3發行版本所做的所有其他增強功能。 這些增強功能已在2020年8月10日當週的生產環境中推出。

如需20.3版所有可用變更的清單，請參閱 [20.3版本總覽](../../../product-announcements/product-releases/20.3-release-activity/20.3-release-overview.md).

## 與私人連結共用行事曆

若要減輕在Workfront中共用行事曆的負擔，您可以共用可將使用者直接導向行事曆的私人連結。 行事曆必須與使用者共用，而且他們必須登入才能檢視。

之前，您可以共用不需要登入即可檢視的公用URL。

如需詳細資訊，請參閱 [共用行事曆報告](../../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md).

## 建立請求時新增草稿區域

為了讓您在處理請求時擁有更多彈性，Workfront現在會自動將您建立的每個請求儲存為新「草稿」區域中的草稿。 如果您沒有完成新請求所需的所有資訊，可以將其保留為草稿、返回並稍後完成。 Workfront會在新草稿區域的每個佇列主題儲存一個請求。 草稿請求可以儲存到您準備好完成並提交為止，只要您需要。 您也可以使用「版面配置範本」來移除或重新定位左側面板中的「草稿」區域。

如需建立請求的詳細資訊，請參閱 [建立及提交Workfront請求](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

>[!NOTE]
>
>在預覽版本中，如果您有指派給您的自訂版面配置範本，您將需要透過修改版面配置範本新增請求的草稿區域。

## 展開或摺疊時程表上的專案

>[!NOTE]
>
>此功能僅在新的Adobe Workfront體驗中可用

為協助您輕鬆管理包含多個專案的時程表，您現在可以按一下按鈕以展開或收合所有專案。

之前，您必須個別按一下每個專案。

如需詳細資訊，請參閱 [記錄時間](../../../timesheets/create-and-manage-timesheets/log-time.md).

## 忽略Workfront行事曆中的實際日期

>[!NOTE]
>
>此功能於2020年6月5日發佈到預覽環境。 它將於2020年6月19日在生產環境中可用。

若要讓您更能掌控物件在行事曆報表中的顯示方式，您可以選擇忽略實際日期，即使這些日期可供使用。

以前，行事曆在可以使用實際日期後會自動使用實際日期。

如需詳細資訊，請參閱 [行事曆報表總覽](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

## 在行事曆報告中使用自訂日期欄位

>[!NOTE]
>
>此功能於2020年5月29日發佈到預覽環境。 它將於2020年6月12日在生產環境中可用。

為協助您更清楚的視覺化及管理日常工作行事曆，自訂日期欄位現在可作為日期選項使用。

以前，您只能在實際日期不可用時，以預計或計畫的方式管理行事曆。

如需詳細資訊，請參閱 [在行事曆報告中使用自訂日期欄位](../../../reports-and-dashboards/reports/calendars/use-custom-dates.md) (或如果您使用Workfront Classic，請參閱 [在行事曆報告中使用自訂日期欄位](https://one.workfront.com/s/article/Use-custom-date-fields-in-a-calendar-report-432597950?language=en_US))。

## 電子郵件變更

**傳出電子郵件變更：** Workfront的所有電子郵件將來自notifications@my.workfront.com。 這包括自動警示和使用者對使用者的通訊。

以前，系統管理員可以在電子郵件設定區域中新增自訂電子郵件地址。

**傳入電子郵件POP回覆變更：** 系統管理員無法再設定自訂POP電子郵件伺服器來接收通知的電子郵件回覆。

如需詳細資訊，請參閱 [電子郵件詐騙和POP回覆電子郵件變更](https://one.workfront.com/s/article/Email-spoofing-and-POP-reply-email-changes?language=en_US).

## 傳出的Workfront電子郵件現在包含DomainKeys識別的郵件(DKIM)

所有外寄電子郵件都將包含電子郵件驗證技術(DKIM)。 一般使用者看不到此DKIM簽章，但允許在伺服器層級驗證，並強化我們現有的驗證架構。

## 更新新Workfront體驗的註冊

為了讓使用者在新Workfront中的註冊體驗更易於管理，群組管理員現在可以註冊和取消註冊屬於其管理群組之使用者。

現在也有顯示下列使用者資訊的使用者詳細資訊連結：

* 姓名
* 工作角色
* 電子郵件地址
* 個人資料圖片

## 管理員的新功能：適用於特定群組、團隊、工作角色和使用者的Brand Workfront

>[!NOTE]
>
>此功能僅在新的Adobe Workfront體驗中可用

現在，您可以使用版面範本來變更頂端導覽區域和[主要]功能表上的標誌，以利特定群組、團隊、工作角色和擁有自己品牌的使用者使用。

如需詳細資訊，請參閱 [品牌化您的Adobe Workfront執行個體](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).

## 群組管理員可以建立和管理核准流程

若要允許對其群組工作流程擁有更多自主權和控制權，群組管理員現在可以存取「設定」中的「核准流程」區域，並針對其管理的群組建立和編輯核准流程。 這些核准程式會以該群組的狀態為基礎。

為了確保群組管理員不會無意中編輯整個系統中使用的核准流程或由其他群組建立的核准流程，他們只能存取與其管理的群組相關聯的核准流程。

如需詳細資訊，請參閱 [建立工作專案的核准流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## 管理員專用：新的「群組」頁面可讓您更輕鬆地建立和管理群組

現在，群組管理員可以更輕鬆地管理群組，因為他們所需的一切都在新的「群組」頁面上。 您不再需要導覽至不同的覆蓋方塊和設定頁面，即可建立和修改群組。

以下是主要重點：

* 群組詳細資料：檢視並編輯群組的基本資訊，例如群組名稱、說明、群組管理員名稱，以及群組是公用或私用。
* 群組成員清單：檢視所有群組成員，並使用新的工具列來快速新增、移除、匯出、啟用和停用成員資格。 您也可以編輯成員的設定檔，並傳送更新註解給他們。
* 標題中的「群組管理員」欄位：檢視您管理的群組時，請快速指派或取消指派群組成員為群組的管理員。 您也可以使用新的「群組角色」欄，在群組成員清單中執行此作業。
* 子群組清單：檢視、編輯、複製、匯出及刪除您管理的群組中的子群組。
* 狀態清單：檢視及管理群組的狀態。

如需詳細資訊，請參閱 [建立群組](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

## 管理員的新增功能：建立最多14層子群組

為了更方便組織您的Workfront群組以符合您的組織階層，我們已將您可以在群組中建立的子群組層級從3個增加到14個。

如需詳細資訊，請參閱 [群組概述](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

## 管理員的新增功能：新增設定側欄

>[!NOTE]
>
>此功能僅在新的Adobe Workfront體驗中可用

「設定」中的左側邊欄現在更快、更易於使用，並運用您已瞭解的基本版面和功能。 除了更現代的外觀與風格，以下還有新增功能：

* 側邊欄中新的非白色背景可讓您更輕鬆地區分「設定」區域的其餘部分。
* 側邊欄中的圖示會稍微大一點，有些經過重新設計，以更清楚地建議選項的用途。
* 側邊欄專案之間的垂直間距增加可讓讀者更容易閱讀。
* 如果您需要在主區域有空間檢視，則可摺疊側邊欄，以執行更多動作，例如檢視其他欄。 當您需要檢視特徵名稱時，可以再次展開側欄。
* 側邊欄收合時，您只會看到每個功能的圖示。 若要檢視主要側邊欄專案底下的子專案，請將滑鼠指標停留在子專案的圖示上，即可在彈出式選單中顯示子專案。 例如，將滑鼠懸停在流程圖示上，即可顯示包含核准和里程碑路徑的功能表。
* 您可以按一下更快存取兩個Kick-Start選項（匯入資料和匯出資料）。 它們已從系統下方移出，並顯示在側邊欄的主要層級。

如需有關如何使用「設定」區域的資訊，請參閱 [管理和設定](../../../administration-and-setup/administration-and-setup.md).

## 在客戶資訊區域包含叢集編號

身為Workfront管理員，您現在可以在Workfront中輕鬆找到叢集編號，不必花費額外時間和精力從我們的支援團隊取得。 我們在設定的「客戶資訊」區域中新增了「叢集設定」欄位。

如需「客戶資訊」區域的詳細資訊，請參閱 [設定系統的基本資訊](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

## 事件訂閱的Base64編碼

base64Encoding欄位是選用欄位，用來啟用事件訂閱裝載的Base64編碼。 如果使用設為true的base64Encoding欄位提出要求，則承載中的newState和oldState物件會以Base64編碼字串傳送。 如果您的網路設定方式不允許在「事件訂閱」中使用特殊字元，此功能會很有用。

如需詳細資訊，請參閱 [事件訂閱API](../../../wf-api/general/event-subs-api.md).

## 移除建立重複事件訂閱的功能

為了防止傳送重複的訊息，您無法再建立重複的訂閱。 此外，先前建立的任何重複訂閱均已移除。

如需詳細資訊，請參閱 [常見問題集 — 事件訂閱](../../../wf-api/general/event-subs-faq.md).
