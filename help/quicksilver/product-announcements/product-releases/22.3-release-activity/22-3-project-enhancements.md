---
title: 在22.3版本時間範圍內更新專案
description: 在22.3版本時間範圍內更新專案
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1235ad4a-72dd-45c5-8513-d073b3e9a2da
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1562'
ht-degree: 0%

---

# 22.3專案增強功能

本頁說明22.3版對預覽環境所做的所有專案增強功能。 這些增強功能已在2022年7月11日當週的生產環境中推出。 如需22.3版所有可用變更的清單，請參閱 [22.3版本總覽](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## 休假工作委派

現在，當您計畫外出一段時間時，您可以暫時將指派給您的任務和問題委派給其他使用者。 這可確保您的缺席不會成為完成工作的障礙。

在此增強功能之前，您只能委派核准。

以下是此更新中新增的部分功能：

* 在「設定」的「任務與問題偏好設定」區域中為系統或群組管理員設定可在您的環境中啟用委派的設定。

* 「首頁」區域中「委派任務和問題」的新選項，供擁有檢閱或更高授權的使用者委派其工作專案。

* 在「首頁」和「工作總攬」區域中指示將專案委派給其他人的任務和問題標題。

* 「設定」區域中的事件通知和「使用者設定檔」中的電子郵件通知，以控制有關委派工作的電子郵件通知


>[!NOTE]
>
>只有擁有檢閱或更高授權的使用者才能將其工作委派給其他人。 工作可委派給任何使用者，無論其存取層級為何。 受委派的使用者會獲得與受委派專案之受指派人相同的許可權。 如果這些許可權低於使用者的存取層級設定，則委派的使用者可能會無法在委派給他們的任務和問題上執行某些活動。


如需詳細資訊，請參閱 [委派任務和問題總覽](/help/quicksilver/manage-work/delegate-work/delegate-work-overview.md).

## 將問題轉換為任務時的新體驗

為了讓您使用Workfront與新的Workfront體驗一致，我們重新設計了介面，以將問題轉換為任務。

此更新包括：

* 符合新Workfront其餘體驗的更新使用者介面。

* 存取將問題從清單或報告轉換為任務。

* 新增至新任務的預設自訂表單定義於目標專案的任務設定區域。


如需詳細資訊，請參閱 [在Adobe Workfront中將問題轉換為任務](/help/quicksilver/manage-work/issues/convert-issues/convert-issue-to-task.md).

## 將問題轉換為沒有範本的專案時的新體驗

為了讓您使用Workfront與新的Workfront體驗一致，我們重新設計了介面，以便在不使用範本的情況下將問題轉換為專案。

除了符合新Workfront體驗其餘部分的更新使用者介面外，我們還新增了從清單或報告將問題轉換為空白專案的功能。

如需詳細資訊，請參閱 [在Adobe Workfront中將問題轉換為專案](/help/quicksilver/manage-work/issues/convert-issues/convert-issue-to-project.md).

## 更新流中的智慧標籤

我們已改善您在建立新的更新或回覆現有更新時，在更新流中標籤使用者的功能。 現在，當您標籤使用者以將其納入更新時，除了其名稱和頭像外，我們也會顯示其主要角色和電子郵件。 這有助於區分具有類似或相同名稱的多位使用者。

如需詳細資訊，請參閱 [標籤其他人的更新](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

## 自訂欄位計算的新語法

為了準備好日後的增強功能，協助您將計算新增至自訂表單，我們已將您新增至計算的參考欄位語法標準化。 此新語法使用起來很容易，因為當您開始輸入欄位名稱並選取它時，系統會為您輸入它。

如需詳細資訊，請參閱 [文章將計算資料新增至自訂表單](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## 當有兩位具有相同角色的使用者參與核准程式時，請保留精確資訊

為確保您核准工作的資料正確無誤，當多角色核准流程與專案相關聯時，我們已變更專案上記錄核准資訊的方式。

有些核准流程需要兩個不同角色的核准，而兩個不同的核准者可能有相同的其中一個角色。 現在，發生此情況時，在做出核准決策後，Workfront會記錄每個核准者及其與核准流程相關聯的個別角色。

在此變更之前，兩個核准都記錄為第二個使用者，因為它們與第一個核准者共用一個核准角色。 在這種情況下，第二個核准者會覆寫第一個核准者的資訊。

如需Workfront中核准程式的詳細資訊，請參閱 [核准流程總覽](/help/quicksilver/review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

## 變更指派時，分配時數將不再移除

>[!NOTE]
>
>此功能原計畫隨22.2版發行。 它在2022年4月21日發佈到生產環境。


為確保資料的準確性，我們在變更任務指派時，進行了變更以保留分配時數並保留任務計畫時數不變。

已對「簡單期間型別」的工作進行下列變更：

* 移除所有受指派人時，會保留計畫時數。

* 取代使用者和角色時，會保留個別指派分配。

* 移除使用者時，會保留角色上的個別指派分配。 (已從發行版本中移除。 現在，計畫時數將在移除所有受指派人後設為0。)


如需計畫時數的詳細資訊，請參閱 [計畫時數概觀](/help/quicksilver/manage-work/tasks/task-information/planned-hours.md).

## 展示板增強功能

Adobe Workfront展示板已新增下列增強功能：

* 篩選選項 — 您現在可以依展示板上的到期日或狀態篩選。 篩選器也已更新為使用可摺疊區段來分隔選項。

* 封存展示板 — 您現在可以在展示板中封存展示板，而不必前往展示板控制面板。

* 新增團隊到討論區 — 當您搜尋成員時，可以新增整個團隊。 選擇團隊會將團隊中的所有人新增到討論區。

* 將區域拖放到欄中 — 將卡片從一個展示板欄拖放到另一個展示板欄時，現在會顯示將放置卡片的位置，當中會顯示灰色的「拖放區域」。 以前沒有卡片位置的視覺指示器。

* 連線的卡片 — 您現在可以新增連線到Workfront任務和問題的卡片。 更新卡片中的名稱、說明或受指派人，或任務將更新其他位置中的相同欄位。

* 所有卡片上的狀態列位 — 狀態列位和標籤完成按鈕已新增到臨機操作卡片和已連線卡片上。 當您按一下「標示完成」時，狀態會自動變更為「完成」。

* 將臨機操作卡片轉換為已連線的卡片 — 您現在可以選擇從卡片詳細資料將臨機操作卡片轉換為已連線的卡片。

* 中斷連線的卡片 — 中斷連線的卡片會中斷與Workfront物件的連線。 此卡片在展示板上會維持為臨機操作卡片，Workfront物件不受影響。

* 欄中的狀態對應 — 新的欄設定和原則可讓您定義狀態、受指派人或標籤，其將套用至移至該欄的卡片。 此外，新展示板上的預設欄名稱已變更為「欄1」、「欄2」和「欄3」。

* 欄位更新指標 — 儲存卡片時現在會顯示指標，以確認您的更新已儲存。


如需詳細資訊，請參閱 [開始使用Adobe Workfront中的面板](/help/quicksilver/agile/get-started-with-boards/get-started-with-boards.md).

## 僅共用資料夾階層前五個層級的資料夾

為確保使用者共用資料夾的最佳效能，我們目前將共用限制在物件資料夾階層的最前五個層級。

第六層級或更低層級的每個資料夾都會從其正上方的資料夾繼承其共用設定。

如需共用資料夾的詳細資訊，請參閱 [共用頂層檔案資料夾](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

## Workfront Campaigns （測試版） — 管理您工作的新方法

>[!NOTE]
>
>此功能預計於2023年1月9日從預覽版中移除。 如需詳細資訊，請參閱 [23.1版本總覽頁面](/help/quicksilver/product-announcements/product-releases/23.1-release-activity/23-1-release-overview.md).

>[!NOTE]
>
>22.3生產版本將不會包含此功能。 它將在未來版本中發佈到生產環境。


>[!NOTE]
>
>此功能僅以Beta版提供，目前正在建構中。 我們會在未來版本中繼續新增Campaign工作流程的功能。 參與Workfront Campaigns的Beta版計畫屬自願性質。

我們為Adobe Workfront引入全新物件，此物件有可能改變您管理工作方式。

Workfront行銷活動可讓您在新的工作容器中組織來自不同投資組合和方案的專案。 此新容器將在未來版本中改進，最終包含目前在不同獨立單位中管理的所有工作物件。

此版本包含下列功能：

* 名為Campaign的新Workfront物件

* 主要功能表中的新行銷活動（測試版）區域

* 行銷活動區域中的行銷活動清單

* 顯示行銷活動其他資訊的行銷活動詳細資訊頁面

* 將專案新增至行銷活動的功能

* 編輯行銷活動相關資訊的功能

* 從版面配置範本重新命名Campaign物件的功能

  Workfront系統和群組管理員可以在版面配置範本的主要功能表中新增Campaigns (Beta)區域。 這可讓所有指派給範本的使用者使用。 在推出後，Workfront中的任何人都可以建立行銷活動。




