---
content-type: release-notes
keywords: 附註，每季，更新
navigation-topic: product-releases
title: 21.1項目管理增強功能
description: 本頁面說明在「預覽」環境的21.1版中所做的所有「專案管理」增強功能。 這些增強功能將於2021年2月15日當周在生產環境中提供。
author: Luke
feature: Product Announcements
exl-id: 95e75a28-5ac2-4d1d-acc3-dbc0b295b28f
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '972'
ht-degree: 1%

---

# 21.1項目管理增強功能

本頁面說明在「預覽」環境的21.1版中所做的所有「專案管理」增強功能。 這些增強功能將於2021年2月15日當周在生產環境中提供。

如需21.1版所有可用變更的清單，請參閱 [21.1版本概觀](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## 現在可在專案的「量度」區段中使用匯出

若要更輕鬆共用專案的狀態和進度，您現在可以將專案「量度」區段中的整個控制面板匯出為.png檔案。

如需詳細資訊，請參閱 [專案量度概觀](../../../manage-work/projects/manage-projects/project-metrics.md).

此功能現已納入 [新Workfront體驗的規劃器基礎知識，第3部分：管理專案](https://one.workfront.com/s/learningpath3/planner-fundamentals-for-the-new-workfront-experience-part-3-manage-a-project-MCG6OJL724XRBLHBXEAKGAUZOJ6U) Workfront一號的學習路徑。

## 更新從問題更新轉換的項目或任務完成的問題百分比

我們已更新問題完成百分比對於已轉換為專案或工作的問題的運作方式。 使用新功能時，當問題轉換為任務或項目時，問題完成百分比將與解決任務或項目完成百分比同步，當「在解決對象的狀態更改時自動更新可解決的問題狀態」設定從設定中啟用時。

如需轉換問題的相關資訊，請參閱 [解析和可解析對象概述](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

## 新提交的請求清單

為了讓您以更簡單、更一致的方式管理您的「已提交請求」，我們已移除「請求」區域中的「我已提交的請求」和「所有請求」區段，並以新的「已提交」清單取代這些區段。 清單的外觀和風格與系統中的所有其他清單相符，可讓您篩選不同類別的已提交請求，並快速搜尋可能很難找到的請求。

如需如何找到已提交請求的相關資訊，請參閱 [找出提交的請求](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

此功能現已納入 [新Workfront體驗的Collaborator基礎知識](https://one.workfront.com/s/learningpath1/collaborator-fundamentals-for-the-new-workfront-experience-MCY5AMOQQTGFDVZB4ODS6TXCYE2A) Workfront一號的學習路徑。

此功能現已納入 [新Workfront體驗中的請求](https://one.workfront.com/s/learningpath3/core-team-requests-in-the-new-workfront-experience-MCHWSSDWRFC5EKXFBXTQ6MJNKE7E) Workfront一號的學習路徑。

## 從「新請求」頁面移除的欄位

>[!NOTE]
>
>從發行中移除。

在重新設計「新請求」頁面時，我們已更新專案「佇列設定」區段中設定的「新問題欄位」。

只有在從專案的「問題」區段建立問題時，才會顯示下列新問題欄位。 在「請求」區域中使用請求佇列提交問題時，系統不會顯示問題：

* 嚴重程度
* 計畫小時
* 計畫開始日期
* URL
* 指派對象
* 職務角色
* 團隊

我們已將「分配給」(Assigned To)、「作業角色」(Job Role)和「團隊」(Team)欄位替換為「新請求」(New Request)頁面上的新「分配」(Assignments)欄位，以便在提交新請求時在公共欄位中高效地指定用戶、作業角色或團隊。

如需定義專案新問題欄位的相關資訊，請參閱 [建立請求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## 在「請求」區域提交請求時的新體驗

>[!NOTE]
>
>從發行中移除；將保持「預覽」狀態，並透過21.2發行至生產環境。

為了與新的Workfront體驗保持一致，並在提交請求時提高效率，我們已重新設計「請求」區域的「新請求」方塊。 以下是部分改善：

* 包含與其餘新Workfront體驗的使用者介面
* 消除「新請求」區域，提供更輕鬆且直覺的體驗
* 將檔案附加至請求的全新、更有效率的方式

可在您輸入請求時共用請求佇列、主題群組或佇列主題的連結。

如需提交請求的相關資訊，請參閱 [建立及提交Workfront請求](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

## 在提交請求時共用請求佇列的連結

>[!NOTE]
>
>從發行中移除；將保持「預覽」狀態，並透過21.2發行至生產環境。

現在，當您建立請求時，可以共用請求佇列、主題群組或佇列主題的連結。

在提交新請求之前，您可以複製請求的請求佇列、主題群組或佇列主題的連結，並與其他使用者共用，或將其內嵌在控制面板中。

如需在提交請求時共用請求佇列連結的相關資訊，請參閱 [共用請求佇列的連結](../../../manage-work/requests/create-requests/share-link-to-request-queue.md).

## 搜尋您要指派給專案的群組並檢視其詳細資料

現在，在將群組指派至專案時，可更輕鬆確定您識別正確的群組。 將滑鼠指標暫留在「群組」方塊中找到的群組名稱上，然後按一下名稱旁顯示的資訊圖示，即可檢視「群組詳細資料」工具提示。

此工具提示包括群組上方的群組階層（如果有）以及群組的管理員。

根據為組配置的詳細資訊，您可能還會看到組的業務主管和說明。

透過此資訊，您可以確信正在選取要指派給專案的正確群組。

如需詳細資訊，請參閱 [在項目概覽區域中管理資訊](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

## 新使用者委派報表

以前，任務、問題和項目核准委託的資訊只能由其所在區域的代表查看。 為了讓其他使用者看到此資訊，計畫使用者現在可以建立「使用者委派」報表，該報表會告訴您：

* 已將這些批准委託給其他用戶
* 已委派這些核准的使用者
* 這些代表團的開始和結束日期

若要進一步了解，請參閱 [建立使用者委派報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md).
