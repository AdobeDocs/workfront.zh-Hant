---
content-type: release-notes
keywords: 備註，每季，更新
navigation-topic: product-releases
title: 21.1管理員增強功能
description: 本頁說明21.1版對「預覽」環境所做的所有管理員增強功能。 這些增強功能將在2021年2月15日當週的生產環境中提供。
author: Luke
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: 4048f8b5-70e2-4d63-ae64-a4fbf91a57df
source-git-commit: 6fe1a2c71f53d6b314c2b1402a547f9c934bfbea
workflow-type: tm+mt
source-wordcount: '1347'
ht-degree: 0%

---

# 21.1管理員增強功能

本頁說明21.1版對「預覽」環境所做的所有管理員增強功能。 這些增強功能將在2021年2月15日當週的生產環境中提供。

如需21.1版本可用的所有變更清單，請參閱[21.1版本概觀](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md)。

## 引入新的存取層級設定以複製專案

為了讓您作為系統管理員對計畫者可以對專案執行的操作擁有更多控制權，我們引入新設定，讓您啟用或停用其複製專案的能力，讓存取層級中的專案編輯存取權更精細。 在此變更之前，當您啟用使用者編輯專案的存取權時，他們會自動獲得複製專案的存取權。 透過新功能，您可以停用新的複製設定，授予某人編輯專案的存取權，而不需要擁有複製專案的存取權。

如果使用者在此變更前有存取層級編輯專案的許可權，當此功能發行時，他們會自動啟用此設定。

如需計畫存取層級的詳細資訊，請參閱[授予專案的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)。

如需有關複製專案的資訊，請參閱[複製專案](../../../manage-work/projects/manage-projects/copy-project.md)。

此功能現在包含在新Workfront體驗第1部分：使用者組織[&#128279;](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home)的Workfront One學習路徑的管理員基礎課程中。

## 在物件的自訂表單中，選取多選下拉式欄位中的所有專案

>[!NOTE]
>
>目前當您提交新請求時，無法使用此功能。

在物件的「詳細資訊」頁面上，當您在自訂表單中填寫多選下拉欄位時，如果您需要選取所有可用的選項，可以按一下「全選」。

如需有關編輯自訂表單上資料的資訊，請參閱[編輯自訂表單欄位中的資訊](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md)。

## 重新計算物件的所有自訂表單欄位

現在，可以更輕鬆確保計算自訂欄位中的所有資料都是物件的最新資料。 新的「重新計算運算式」功能表選項可讓您快速重新計算這些欄位中的所有資料。

在有人編輯物件中另一個由計算自訂欄位參考的物件資料後，此功能特別有用。

以前，使用者必須使用因應措施，以確保計算自訂欄位中的所有資料都是最新的。 例如，他們編輯物件與其他物件，以使用可大量編輯的重新計算選項。

如需詳細資訊，請參閱[編輯自訂表單欄位中的資訊](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md)。

## 解鎖群組管理員的任務和問題偏好設定

>[!NOTE]
>
>在2021年6月24日之前，這僅可作為分階段推出的一部分，提供給能夠解鎖群組專案偏好設定的客戶。 現在可供所有客戶使用。

Adobe Workfront管理員現在可以解鎖個別任務和問題偏好設定，賦予群組管理員更多自主權。 解鎖偏好設定後，群組管理員可以為其群組設定它，以滿足每個群組的獨特需求和內部流程。

如需詳細資訊，請參閱[設定群組的任務和問題偏好設定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)。

此功能現在包含在新Workfront Experience第2部分：專案設定[&#128279;](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home)的Workfront One學習路徑的管理員基礎課程中。

## 分別設定投資組合和計畫的存取層級設定

現在，由於您可以單獨設定其存取層級設定，因此可更輕鬆管理使用者對投資組合和計畫的存取權。

先前，投資組合和計畫的存取層級設定是合併的。 這表示您無法為方案設定存取設定，除非以相同的方式為投資組合進行設定，反之亦然。

如需有關設定存取層級的資訊，請參閱[建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

如需您可以為程式與產品組合設定的存取設定相關資訊，請參閱[每個物件型別可設定的功能存取權](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md)。

此功能現在包含在新Workfront體驗第1部分：使用者組織[&#128279;](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home)的Workfront One學習路徑的管理員基礎課程中。

## 在自訂表單中編輯資訊時，選取序列中的所有核取方塊

>[!NOTE]
>
>目前當您提交新請求時，無法使用此功能。

在物件的「詳細資訊」頁面上，當您填寫包含核取方塊的「自訂表單」欄位時，如果您需要選取所有可用的核取方塊，可以按一下「全選」。

只有在欄位包含2個以上的核取方塊時，才會顯示此選項。

如需詳細資訊，請參閱[編輯自訂表單欄位中的資訊](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md)。

## 設定您的Workfront電子郵件允許清單

為了更妥善保護您的資料，您現在可以使用電子郵件網域允許清單來：

* 控制Workfront電子郵件如果包含儲存在Workfront中的報告或檔案，可以傳送的位置
* 控制電子郵件網域可以在使用者設定檔中指定的電子郵件地址中

例如，如果您想保護敏感資料，例如列出有風險客戶的報表，您只能在電子郵件允許清單中加入內部電子郵件網域或網域。 如此一來，使用者無法將該報表(或任何其他Workfront報表)傳送至外部電子郵件地址。

如需詳細資訊，請參閱[設定防火牆允許清單](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)一文中的[設定防火牆允許清單](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md#configur)一節。

## 指派子群組的群組管理員

為了讓您組織的層級更易於獨立運作，我們新增了將群組管理員指派給子群組的功能。 現在，您可以確定您要將子群組管理委派給適當的人員。

以前，只有最上層群組才有群組管理員，而這些管理員負責管理最上層群組下的所有子群組。

如需詳細資訊，請參閱文章[子群組總覽](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md)中的[子群組的群組管理員](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md#for)一節。

此功能現在包含在新Workfront體驗第1部分：使用者組織[&#128279;](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home)的Workfront One學習路徑的管理員基礎課程中。

## 設定群組的事件通知

>[!NOTE]
>
>分階段推出僅供能夠解鎖群組專案偏好設定的客戶使用。 這包括叢集4和6上的所有客戶，以及其他叢集上的少數客戶。 當更多叢集可以使用此功能時，將會更新此附註。

Workfront管理員現在可以允許群組管理員為其最上層群組設定事件通知，賦予群組管理員更多自主權。 子群組會繼承其上層父群組的事件通知設定。

以前，事件通知只能由Workfront管理員在系統層級設定，這意味著所有群組都必須使用相同的事件通知集。

如需詳細資訊，請參閱下列文章：

* [解除鎖定所有群組的事件通知設定](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md)
* [檢視和設定群組的事件通知](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)

<!--This feature is now included in the [Administrator Fundamentals in the new Workfront experience, Part 1: User Organization](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home) learning path on Workfront One.

This feature is now included in the [Email and In-App Notifications in the new Workfront experience](https://experienceleague.adobe.com/en/docs/workfront/using/home://one.workfront.com/s/learningpath2/email-and-in-app-notifications-in-the-new-workfront-experience-MCDSDH3SRJ4ZGTJF5NJI64F4TW2U) learning path on Workfront One.-->

## 在群組區域中使用群組專案和核准流程

如果您是群組管理員，現在您的群組專案和核准程式已列於群組區域中，可輕鬆檢視和處理這些專案和核准程式。 從群組的主要頁面，您可以：

* 按一下左側功能表中的「專案」 ，檢視群組的專案並為群組建立新專案。 如果選取的專案已與您共用，您可以使用工具列中的按鈕來編輯、匯出、複製或刪除專案。

  如需詳細資訊，請參閱[建立和修改群組的專案](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md)。

* 按一下左側功能表中的「核准」 ，即可檢視和管理與群組相關聯的所有核准流程。

  如需詳細資訊，請參閱[群組層級核准流程](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md)。

Workfront管理員也可使用此功能。

## 檢視在群組中使用和配置的授權數目

若要判斷授權的分發狀況，您現在可以檢視群組及其下方任何子群組中使用的授權數目。

如果您管理最上層群組，則可以檢視群組（及其子群組）中使用的授權數目，以及配置給該群組的授權數目上限。

如需詳細資訊，請參閱[檢視新Adobe Workfront體驗中群組所配置及使用的授權數目](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-number-licenses-allocated-used-group.md)。

