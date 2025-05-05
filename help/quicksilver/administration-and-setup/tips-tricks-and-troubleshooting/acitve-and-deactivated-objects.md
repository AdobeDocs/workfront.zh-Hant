---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 使用中及已停用的物件
description: 作為 [!DNL Adobe Workfront] 管理員，您可以啟動或停用系統內的物件。 我們建議您永遠不要刪除可以停用的物件。 您應該直接停用物件以防止將來使用，並從其他物件的下拉式選單中移除它。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: a0617270-e233-4ebe-a5ee-8df7a8a85823
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '747'
ht-degree: 2%

---

# 使用中及已停用的物件

作為[!DNL Adobe Workfront]管理員，您可以啟動或停用系統內的物件。 我們建議您永遠不要刪除可以停用的物件。 您應該直接停用物件以防止將來使用，並從其他物件的下拉式選單中移除它。

例如，若要檢視特定的[!UICONTROL 小時型別]，[!UICONTROL 小時型別]必須為作用中。 非使用中或已停用的[!UICONTROL 時數型別]未出現在[!UICONTROL 時數型別]下拉式功能表中，但會保留在系統中，以保留過去可能使用此[!UICONTROL 時數型別]的完整歷史記錄。

「作用中」一詞用於識別系統中是否啟用某些物件。 在此內容中，「作用中」用於下列物件：

## 電子郵件通知

您可以啟用電子郵件通知，以允許某些動作觸發所有使用者的電子郵件通知。

如需關於啟用或停用電子郵件通知的資訊，請參閱[為系統中的每個人設定事件通知](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)。

## 時數類型

您可以啟用小時型別，讓使用者在記錄時間時可選取這些型別。

如需有關啟用或停用時數型別的資訊，請參閱[管理時數型別](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md)。

## 專案組合

投資組合必須處於作用中狀態，才能出現在[!UICONTROL 新專案（業務案例）]表單中。

您可以在編輯投資組合時，讓投資組合處於作用中狀態。

如需有關編輯投資組合的資訊，請參閱[建立投資組合](../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md)。

## 計劃

程式必須為使用中狀態，才能出現在專案的[!UICONTROL 程式]欄位中。

您可以在編輯程式時啟動程式。

如需有關編輯程式的資訊，請參閱[建立程式](../../manage-work/portfolios/create-and-manage-programs/create-program.md)。

## 範本

範本必須為作用中狀態，才能顯示在專案的「範本」欄位中。

您可以在編輯範本時啟動範本。

如需有關編輯範本的資訊，請參閱[編輯專案範本](../../manage-work/projects/create-and-manage-templates/edit-templates.md)。

## 核准流程

核准流程必須處於作用中狀態，才能出現在專案、任務或問題的[!UICONTROL 核准流程]欄位中。

您可以在編輯核准流程時啟用核准流程。

如需有關編輯核准流程的資訊，請參閱[建立工作專案的核准流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)。

## 里程碑路徑

里程碑路徑必須為作用中狀態，才能出現在專案的[!UICONTROL 里程碑路徑]欄位中。

您可以在編輯里程碑路徑時啟動里程碑路徑。

如需有關編輯里程碑路徑的資訊，請參閱[建立里程碑路徑](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md)。

## 自訂表單

自訂表單必須處於作用中狀態，才能出現在其他物件的[!UICONTROL 自訂表單]欄位中。

您可以在編輯自訂表單時啟用自訂表單。

如需有關編輯自訂表單的資訊，以及可與其建立關聯的物件清單，請參閱[建立自訂表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

## 公司

公司必須處於作用中狀態，才能出現在專案、使用者或範本的[!UICONTROL 公司]欄位中。

您可以在編輯公司時讓公司生效。

如需詳細資訊，請參閱[建立和編輯公司](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md)。

## 使用者

使用者必須在進行指派或共用物件時，才會出現在所有其他物件的任何預先輸入欄位中。

您可以從使用者頁面或當您編輯使用者時，停用使用者。

如需停用使用者的詳細資訊，請參閱[停用或重新啟用使用者](../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md)。

>[!IMPORTANT]
>
>如果您的組織已加入[!DNL Adobe Business Platform]，您必須透過[!UICONTROL Adobe Admin Console]停用使用者。
>
>如需在[!UICONTROL Adobe Admin Console]中停用使用者的指示，請參閱文章[個別管理使用者](https://helpx.adobe.com/tw/enterprise/using/manage-users-individually.html)中的「移除使用者」一節，或連絡您的[!UICONTROL Adobe Admin Console]系統管理員。
>
>如需根據貴組織是否已加入[!DNL Adobe Business Platform]而不同的程式清單，請參閱[以平台為基礎的管理差異(Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)。

## 團隊

專案團隊必須處於作用中狀態，才能在進行指派或共用物件時，出現在所有其他物件的任何預先輸入欄位中。

您可以在編輯團隊時停用團隊。

如需停用團隊的詳細資訊，請參閱[停用團隊](../../people-teams-and-groups/create-and-manage-teams/deactivate-a-team.md)。

## 職務角色

工作角色必須為作用中，才能在指派或共用物件時，出現在所有其他物件的任何預先輸入欄位中。

您可以在編輯工作角色時將其停用。

如需有關停用工作角色的資訊，請參閱[停用工作角色](../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md)。

