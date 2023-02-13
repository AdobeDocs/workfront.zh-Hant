---
content-type: release-notes
keywords: 附註，每季，更新
navigation-topic: product-releases
title: 21.1管理員增強功能
description: 本頁面說明在「預覽」環境的21.1版中進行的所有管理員增強功能。 這些增強功能將於2021年2月15日當周在生產環境中提供。
author: Luke
feature: Product Announcements, System Setup and Administration
exl-id: 4048f8b5-70e2-4d63-ae64-a4fbf91a57df
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1440'
ht-degree: 0%

---

# 21.1管理員增強功能

本頁面說明在「預覽」環境的21.1版中進行的所有管理員增強功能。 這些增強功能將於2021年2月15日當周在生產環境中提供。

如需21.1版所有可用變更的清單，請參閱 [21.1版本概觀](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## 引入新的「存取層級」設定來複製專案

為了讓您作為系統管理員能夠更好地控制規劃人員可以對項目執行什麼操作，我們引入了允許您啟用或禁用其複製項目能力的新設定，使訪問級別的項目的編輯訪問更加精細。 在此變更前，當您啟用使用者的「編輯」專案存取權時，他們會自動擁有複製專案的存取權。 使用新功能，您可以讓使用者存取編輯專案的權限，而無需借由停用新的「複製」設定來複製專案。

如果您的使用者在進行此變更前，有權在其存取層級存取「編輯」專案，當此功能發行時，他們會自動啟用此設定。

有關計畫訪問級別的資訊，請參閱 [授予專案的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

如需複製專案的相關資訊，請參閱 [複製專案](../../../manage-work/projects/manage-projects/copy-project.md).

此功能現已納入 [新Workfront體驗的管理員基礎知識，第1部分：使用者組織](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) Workfront一號的學習路徑。

## 在物件的「自訂表單」中，在多選下拉式欄位中選取所有項目

>[!NOTE]
>
>當您提交新請求時，目前無法使用此功能。

在對象的「詳細資訊」(Details)頁面上，在「自定義表單」上填寫多選下拉欄位時，如果需要選擇所有可用選項，可以按一下「全部選擇」。

如需在自訂表單上編輯資料的相關資訊，請參閱 [在自訂表單欄位中編輯資訊](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## 重新計算對象的所有自定義表單欄位

現在可更輕鬆確保計算的自訂欄位中的所有資料都為物件最新。 新的「重新計算表達式」菜單選項可讓您快速重新計算這些欄位中的所有資料。

當某人編輯另一個物件中的資料時（該物件中的已計算自訂欄位已參照），這個用法特別有用。

過去，使用者必須使用因應措施，以確保計算自訂欄位中的所有資料都為最新資料。 例如，他們編輯了對象以及其他對象，以使用可用於批量編輯的重新計算選項。

如需詳細資訊，請參閱 [在自訂表單欄位中編輯資訊](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## 解鎖組管理員的任務和問題首選項

>[!NOTE]
>
>在2021年6月24日之前，只有能夠解除群組專案偏好設定鎖定的客戶，才能分階段推出此功能。 現在，它可供所有客戶使用。

Adobe Workfront管理員現在可以解除鎖定個別任務和問題偏好設定，讓群組管理員擁有更大的自治權。 當首選項解除鎖定時，組管理員可以為其組配置該首選項，以滿足每個組的獨特需要和內部進程。

如需詳細資訊，請參閱 [配置組的任務和問題首選項](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

此功能現已納入 [新Workfront體驗的管理員基礎知識，第2部分：專案設定](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-1-project-workfl-MCTBVZ3Q3J5RHNLIPPZPFSQRLKUY) Workfront一號的學習路徑。

## 分別配置產品組合和程式的訪問級別設定

現在管理使用者對產品組合和方案的存取權限更為輕鬆，因為您可以個別設定其存取層級設定。

之前，產品組合和方案的存取層級設定皆已結合。 這表示，若不以與產品組合相同的方式配置程式，便無法配置程式的存取設定，反之亦然。

有關配置訪問級別的資訊，請參見 [建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

如需可針對方案和產品組合設定之存取設定的相關資訊，請參閱 [可針對每個對象類型配置對功能的訪問](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

此功能現已納入 [新Workfront體驗的管理員基礎知識，第1部分：使用者組織](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) Workfront一號的學習路徑。

## 在「自訂表單」中編輯資訊時，選取系列中的所有核取方塊

>[!NOTE]
>
>當您提交新請求時，目前無法使用此功能。

在對象的「詳細資訊」頁上，當您填寫包含複選框的「自定義表單」欄位時，如果需要選擇所有可用複選框，則可以按一下「全部選擇」。

只有在欄位包含超過2個核取方塊時，才會顯示此選項。

如需詳細資訊，請參閱 [在自訂表單欄位中編輯資訊](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## 設定Workfront電子郵件允許清單

為了更妥善保護您的資料，您現在可以使用電子郵件網域允許清單：

* 如果Workfront電子郵件包含儲存在Workfront中的報表或檔案，請控制其可前往的位置
* 控制電子郵件網域可以位於使用者可在其使用者設定檔中指定的電子郵件地址中

例如，如果您想要保護敏感資料，例如列出您面臨風險之客戶的報表，則只能在電子郵件允許清單中納入您的內部電子郵件網域或網域。 如此一來，使用者就無法將該報表(或任何其他Workfront報表)傳送至外部電子郵件地址。

如需詳細資訊，請參閱 [配置防火牆的允許清單](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md#configur) 在文章中 [配置防火牆的允許清單](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## 為子組分配組管理員

為了讓您的組織級別更容易獨立運行，我們添加了將組管理員分配給子組的能力。 現在，您可以確保將子組管理委派給正確的人員。

以前，只有頂級組才能有組管理員，這些管理員管理了頂級組下的所有子組。

如需詳細資訊，請參閱 [子組的組管理員](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md#for) 在文章中 [子組概述](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

此功能現已納入 [新Workfront體驗的管理員基礎知識，第1部分：使用者組織](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) Workfront一號的學習路徑。

## 設定群組的事件通知

>[!NOTE]
>
>只有能夠解除鎖定群組專案偏好設定的客戶，才能在分階段推出中取得。 這包括群集4和6上的所有客戶以及其他群集上的少量客戶。 當功能可供更多叢集使用時，此備注將會更新。

Workfront管理員現在可讓群組管理員為其頂層群組設定事件通知，以賦予群組管理員更多自治權。 子組會從其父組繼承事件通知配置。

以前，事件通知只能由系統層級的Workfront管理員設定，這表示所有群組都必須使用同一組事件通知。

如需詳細資訊，請參閱下列文章：

* [解鎖或鎖定所有組的事件通知配置](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md)
* [檢視及設定群組的事件通知](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)

此功能現已納入 [新Workfront體驗的管理員基礎知識，第1部分：使用者組織](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) Workfront一號的學習路徑。

此功能現已納入 [新Workfront體驗中的電子郵件和應用程式內通知](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-https://one.workfront.com/s/learningpath2/email-and-in-app-notifications-in-the-new-workfront-experience-MCDSDH3SRJ4ZGTJF5NJI64F4TW2U) Workfront一號的學習路徑。

## 在「組」區域中使用組項目和審批流程

如果您是群組管理員，現在將群組的專案和核准程式列在「群組」區域中，您就能輕鬆檢視及處理這些專案和核准程式。 從群組的首頁，您可以：

* 按一下左側功能表中的「專案」 ，查看群組的專案並為群組建立新專案。 如果已與您共用選取的專案，您可以使用工具列中的按鈕來編輯、匯出、複製或刪除專案。

   如需詳細資訊，請參閱 [建立和修改群組的專案](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

* 按一下左側功能表中的「核准」 ，查看並管理與群組相關聯的所有核准程式。

   如需詳細資訊，請參閱 [組級審批流程](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

Workfront管理員也可使用此功能。

## 查看組中使用和分配的許可證數

要確定許可證的分配程度，您現在可以查看組中使用的許可證數，以及組下的任何子組。

如果管理頂級組，則可以查看組（及其子組）中使用的許可證數以及為組分配的許可證數上限。

如需詳細資訊，請參閱 [在新Adobe Workfront體驗中檢視群組中分配和使用的授權數量](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-number-licenses-allocated-used-group.md).

