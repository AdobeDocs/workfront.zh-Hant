---
content-type: release-notes
keywords: 備註，每季，更新
navigation-topic: product-releases
title: 21.1專案管理增強功能
description: 本頁說明21.1版對預覽環境所做的所有專案管理增強功能。 這些增強功能將在2021年2月15日當週的生產環境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 95e75a28-5ac2-4d1d-acc3-dbc0b295b28f
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '956'
ht-degree: 1%

---

# 21.1專案管理增強功能

本頁說明21.1版對預覽環境所做的所有專案管理增強功能。 這些增強功能將在2021年2月15日當週的生產環境中提供。

如需21.1版本可用的所有變更清單，請參閱[21.1版本概觀](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md)。

## 專案的「量度」區段現已提供匯出功能

為了更輕鬆地共用專案的狀態和進度，您現在可以將專案的「量度」區段中的整個儀表板匯出到.png檔案。

如需詳細資訊，請參閱[專案量度概觀](../../../manage-work/projects/manage-projects/project-metrics.md)。

此功能現在包含在新Workfront體驗的[規劃師基礎知識部分，第3部分：管理Workfront One上的專案](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home)學習路徑。

## 從問題更新轉換而來的專案或任務時，更新問題完成百分比

我們已更新問題完成百分比的運作方式，這些問題已轉換為專案或任務。 運用新功能時，當問題轉換為任務或專案時，當從設定啟用「當解決物件的狀態變更時自動更新可解決的問題狀態」設定時，問題的完成百分比會與解決任務或專案的完成百分比同步。

如需轉換問題的相關資訊，請參閱[解析和可解析物件概述](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md)。

## 新提交的請求清單

為了讓您以更簡單、更一致的方式管理您提交的請求，我們已移除「我已提交的請求」和「請求」區域中的「所有請求」區段，並以新的「已提交」清單取代。 清單具有熟悉的外觀和風格，符合系統中的所有其他清單，可讓您篩選不同類別的已提交請求，並快速搜尋可能難以找到的請求。

如需如何尋找已提交要求的詳細資訊，請參閱[尋找已提交的要求](../../../manage-work/requests/create-requests/locate-submitted-requests.md)。

此功能現已包含在Workfront One上的新Workfront Experience](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/manage-work/issues-requests/make-a-request)學習路徑的[Collaborator基礎知識中。

此功能現已包含在Workfront One上新Workfront體驗](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/manage-work/request-queues/understand-request-queues)學習路徑的[要求中。

## 從新請求頁面移除的欄位

>[!NOTE]
>
>已從發行版本中移除。

在重新設計「新請求」頁面時，我們已更新在專案的「佇列設定」區段中設定的「新問題欄位」 。

下列新問題欄位只有在從專案的問題區段建立問題時才會顯示。 使用請求區中的請求佇列提交問題時不會顯示這些問題：

* 嚴重程度
* 規劃時數
* 規劃開始日期
* URL
* 指派至
* 職務角色
* 團隊

我們已將「指派至」、「工作角色」及「專案團隊」欄位取代為「新請求」頁面上的新「指派」欄位，以便在您提交新請求時，於共用欄位中有效地指定使用者、工作角色或專案團隊。

如需為專案定義新問題欄位的相關資訊，請參閱[建立請求佇列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)。

## 在請求區域中提交請求的新體驗

>[!NOTE]
>
>已從發行中移除；將保留在21.2版的預覽和發行至生產環境。

為了與新的Workfront體驗保持一致，並為您建立提交請求時的效率，我們重新設計了請求區域的新請求方塊。 以下是一些改善專案：

* 與其他全新Workfront體驗相同的使用者介面
* 消除了「新請求」區域，體驗更簡單直觀
* 更有效率的新方式可將檔案附加至您的請求

可在您輸入請求時，共用請求佇列、主題群組或佇列主題的連結。

如需有關提交請求的資訊，請參閱[建立並提交Workfront請求](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)。

## 提交請求時分享請求佇列的連結

>[!NOTE]
>
>已從發行中移除；將保留在21.2版的預覽和發行至生產環境。

現在已可讓您在建立請求時，共用請求佇列、主題群組或佇列主題的連結。

在提交新請求之前，您可以複製請求的請求佇列、主題群組或佇列主題的連結，並將其與其他使用者共用，或嵌入到儀表板中。

如需在提交請求時共用請求佇列連結的相關資訊，請參閱[共用請求佇列的連結](../../../manage-work/requests/create-requests/share-link-to-request-queue.md)。

## 搜尋您要指派給專案的群組並檢視其詳細資訊

現在指派群組至專案時，可以更輕鬆確定您識別出正確的群組。 將游標暫留在您在「群組」方塊中找到的群組名稱上，然後按一下名稱旁邊顯示的資訊圖示，以檢視「群組詳細資料」工具提示。

此工具提示包括群組上方的群組階層（如果有的話），以及群組的管理員。

根據為群組設定的詳細資訊，您也可能看到群組的業務主管和說明。

有了這些資訊，您就可以確信您選取了要指派給專案的正確群組。

如需詳細資訊，請參閱[管理專案概觀區域的資訊](../../../manage-work/projects/manage-projects/understand-project-overview-area.md)。

## 新增使用者委派報告

以前，任務、問題和專案核准委託的資訊只能由委託人在其「首頁」區域中檢視。 若要讓其他使用者檢視此資訊，計畫使用者現在可以建立「使用者委派」報告，該報告將告訴您：

* 誰已將這些核准委派給其他使用者
* 哪些使用者已被委派這些核准
* 這些委派的開始和結束日期

若要深入瞭解，請參閱[建立使用者委派報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md)。
