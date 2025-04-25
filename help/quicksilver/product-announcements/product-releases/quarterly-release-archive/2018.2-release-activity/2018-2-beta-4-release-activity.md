---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.2 Beta 4發行活動
description: 本頁說明2018.2 Beta 4版本預覽環境中最近可用的所有變更。 此功能將於2018年5月17日在預覽環境中提供。 它將在2018年7月的生產環境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4b54b9e6-d1bf-4802-9d6c-9c3d3b6a6583
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1705'
ht-degree: 0%

---

# 2018.2 Beta 4發行活動

本頁說明2018.2 Beta 4版本預覽環境中最近可用的所有變更。 此功能將於2018年5月17日在預覽環境中提供。 它將在2018年7月的生產環境中提供。

>[!IMPORTANT]
>
> 本頁所述的功能在生產環境使用之前可能會有所變更。

如需2018.2年度所有變更的清單，請參閱  [2018.2發行活動總覽](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md)。

2018.2 Beta 4版本包含Workfront管理員和其他使用者的增強功能：

管理員的&#x200B;****

* [系統設定：外部頁面中的工作階段資訊](#system-setting-session-information-in-external-pages)

**所有使用者**

* Kanban展示板上的[進行中的工作(WIP)限制增強功能](#work-in-progress-wip-limit-enhancements-on-the-kanban-board)
* [改善設定敏捷團隊狀態的介面](#improved-interface-for-configuring-statuses-for-an-agile-team)
* 首頁區域中的[已更新工作清單（左側面板）](#updated-work-list-left-panel-in-the-home-area)
* [新的案頭校訂檢視器以校訂互動式（多媒體）內容](#new-desktop-proofing-viewer-for-proofing-interactive-rich-media-content) 
* [匯出資源規劃工具中的使用者檢視](#export-the-user-view-in-the-resource-planner)
* [支援Google Team磁碟機](#support-for-google-team-drives)
* [甘特圖新的匯出限制](#new-export-limit-for-the-gantt-chart)
* 使用Internet Explorer或Safari時，[從剪貼簿貼上現在會顯示為暗灰色](#paste-from-clipboard-option-now-displays-as-dimmed-when-using-internet-explorer-or-safari)
* [適用於Android的新Beta環境以及新功能](#new-beta-environment-for-android-along-with-new-features)
* [事件訂閱訊息的篩選器範例](#examples-of-filters-for-event-subscriptions-messages)

## Kanban面板上的進行中工作(WIP)限制增強功能 {#work-in-progress-wip-limit-enhancements-on-the-kanban-board}

### 設定Kanban面板上每個欄位的在製品(WIP)限制

現在您可以為Kanban面板上的每個欄設定進行中工作(WIP)限制。 

在此變更之前，您只能設定一個套用至Kanban面板上所有欄的WIP限制。 

如需詳細資訊，請參閱區段  [在文章中設定進行中的工作(WIP)限制](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur4)  [設定Kanban](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md)。

### 直接從Kanban面板更新在製品(WIP)限制

現在，擁有團隊編輯許可權的團隊成員可以直接從Kanban面板更新WIP限制。

在此變更之前，您只能從「專案團隊設定」區域更新WIP限制。

如需詳細資訊，請參閱  （在文章中）。

## 改善設定敏捷團隊狀態的介面 {#improved-interface-for-configuring-statuses-for-an-agile-team}

設定敏捷團隊狀態的介面已更新，其中包含下列改善專案：

* 全新外觀
* 透過拖放重新排序狀態列 

如需詳細資訊，請參閱下列文章：

* [設定Kanban](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
* [設定Scrum](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md)

## 更新工作清單（左側面板）首頁區域 {#updated-work-list-left-panel-in-the-home-area}

首頁區域的工作清單包含以下改進：

* 未讀取的專案現在會以粗體和藍點突出。

  在「首頁」區域之外檢視的專案，在「首頁」區域仍會顯示為「未讀取」。

  如需詳細資訊，請參閱[首頁區域的工作清單顯示專案](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md)。

* 問題現在以問題旁邊顯示的問題圖示加以區分。
* 核准現在會依核准型別區分，並顯示核准型別。 可能的核准型別包括任務、專案、問題、存取、檔案、時程表和校訂。

  在此變更之前，核准僅以「核准」一詞區分。

* 專案現在可透過其是否準備好開始來區分。 可能的選項包括「準備開始」、「未就緒」或「正在處理」。

  此資訊不會顯示給核准，因為核准隨時可以開始。

* 每當檔案附加到專案時，專案名稱下方都會顯示檔案圖示。
* 您現在可以在工作清單中摺疊和展開群組，以便更好地控制哪些資訊可見。 分組包括延遲、專案、日期和完成。

  依預設，「本週」區段會展開，而所有其他群組則會摺疊。

* 選擇是依「計畫完成日期」或「確認日期」來排序料號。
* 每個群組中的專案數現在會顯示在群組標題旁的括弧中。

  此數字不適用於「已完成」群組。

  如需詳細資訊，請參閱[首頁區域的工作清單顯示專案](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md)。

* 透過拖放調整工作清單的大小。 您可以調整工作清單的大小，以使用最多一半的畫面。 下次存取「首頁」時，您設定的大小會保留。

  在此變更之前，無法變更工作清單的大小。

* 對於請求，現在會顯示提出請求的使用者的使用者頭像，其文字為&quot;[Approver_name]希望您核准開啟。&quot;
* 建立新的個人任務時，「待辦事項」按鈕現在標籤為「個人」。

  如需詳細資訊，請參閱文章[從首頁區域建立工作專案](../../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md)中的[從首頁區域建立工作專案](../../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md)。

* 延遲料號只有在超過計畫完成日期一小時後才會顯示為「延遲」。

如需主區域的詳細資訊，請參閱[使用主區域](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md)。

## 新的案頭校訂檢視器用於校訂互動式（多媒體）內容 {#new-desktop-proofing-viewer-for-proofing-interactive-rich-media-content}

全新的案頭校訂檢視器可讓您校訂互動式內容。 不同於在瀏覽器中執行的現有舊版校訂檢視器和新版校訂檢視器，「案頭校訂檢視器」是在您的工作站上執行的應用程式。

在新的案頭校訂檢視器之前，您只能在舊版校訂檢視器中校訂互動式內容。 

「案頭校訂檢視器」在用於校訂互動內容的舊版校訂檢視器上包括以下增強功能：

* 檢閱不安全(HTTP)網站

  舊版校訂檢視器允許您僅檢閱安全(HTTPS)網站

* 檢閱受iframe保護的網站（受保護，無法在iframe內檢視的網站）。

  舊版校訂檢視器不支援針對在iframe內受到保護而無法檢視的網站進行檢視。

* 以預先設定的解析度檢視各種裝置的內容。 例如，您可以看到內容在各種標準案頭解析度上或iPhone 8等個別裝置上的顯示方式。 

如需有關下載，安裝和使用Desktop Proofing Viewer的詳細資訊，請參閱。

如需有關案頭校訂檢視器與瀏覽器校訂檢視器之間功能差異的資訊，請參閱[網頁校訂檢視器與案頭校訂檢視器之間的差異](../../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md)。

## 匯出資源規劃工具中的使用者檢視 {#export-the-user-view-in-the-resource-planner}

當資料顯示在使用者檢視中時，為了解決一些效能問題，我們暫時禁止從資源規劃工具匯出資料。 在此版本中，我們在使用者檢視中顯示資源規劃工具時，重新啟用資料匯出。

如需將資源規劃工具資料匯出至Excel的詳細資訊，請參閱[資源規劃工具導覽概觀](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md)中的「匯出選項」一節。

若要參與我們目前資源規劃工具的Beta版計畫，請參閱[資源規劃工具績效Beta。](https://experienceleaguecommunities.adobe.com/t5/workfront/ct-p/workfront)

## 系統設定：外部頁面中的工作階段資訊 {#system-setting-session-information-in-external-pages}

Workfront管理員現在可以在建立外部頁面時，限制使用工作階段資訊（例如工作階段ID）。

在此變更前，可建立外部頁面的使用者可在將其他網站內嵌至Workfront儀表板時，使用任何工作階段資訊。 

如需有關在Workfront中設定系統偏好設定的詳細資訊，請參閱[設定系統安全性偏好設定](../../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)。

## 支援Google團隊磁碟機 {#support-for-google-team-drives}

您現在可以從Workfront連結位於Google團隊磁碟機的檔案或資料夾。

在此增強功能之前，您可以連結僅位於Google我的磁碟上的檔案或資料夾。

如需從各種應用程式連結檔案和資料夾到Workfront的詳細資訊，請參閱[從外部應用程式連結檔案](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)。

## 甘特圖新的匯出限制 {#new-export-limit-for-the-gantt-chart}

您現在可以匯出甘特圖中多達500個任務。

之前，您最多只能匯出250個任務。

如需詳細資訊，請參閱[將甘特圖匯出至PDF](../../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md)。

## 使用Internet Explorer或Safari時，「從剪貼簿貼上」選項現在會以灰色顯示 {#paste-from-clipboard-option-now-displays-as-dimmed-when-using-internet-explorer-or-safari}

使用Internet Explorer或Safari瀏覽器時，「從剪貼簿貼上」選項現在會以灰色顯示，工具提示會說明此功能僅支援Chrome和Firefox瀏覽器。

在此變更之前，使用Internet Explorer或Safari時未顯示此選項。 

如需從剪貼簿貼上影像的詳細資訊，請參閱[從剪貼簿貼上影像](../../../../documents/managing-documents/paste-image-clipboard.md)。

## 適用於Android的全新Beta環境與新功能 {#new-beta-environment-for-android-along-with-new-features}

您現在可以註冊成為Beta測試者，在正式發行之前，體驗我們團隊為行動應用程式設計的最新功能。 Workfront行動應用程式目前僅支援Android手機使用這個環境。

如需如何註冊成為Workfront行動應用程式Beta測試者的詳細資訊，請參閱。

以下為行動應用程式Beta版提供的改良功能：

* 新增帳戶頁面

  您現在可以檢視帳戶資訊，以及管理行動設定、提交意見或從新的「帳戶」頁面登出。

  在此改善之前，您無法在行動應用程式上檢視您的帳戶資訊，而且您可以存取設定、提交意見反應，以及從Workfront主功能表登出。

* 新的導覽底部面板

  熒幕底部現在提供更顯眼的導覽列，可啟動行動應用程式的所有區域。

  在此改善之前，功能區域列於Workfront主功能表中。 Workfront主要功能表已移除，並由新的底部導覽列取代。

  如需關於設定新導覽列的詳細資訊，請參閱中的「設定行動應用程式」一節。

* 新通知清單檢視

  改良後的通知清單外觀，可讓您根據通知的型別和是否閱讀過來輕鬆區分清單中的通知。

* 「搜尋方塊」已移至更顯眼的位置。

* 全新登入體驗更精簡的全新登入體驗。

* 新的教學課程體驗

  現在提供新的教學課程，可在使用者首次登入時，透過應用程式進行簡短指導。 在此體驗之前，教學課程僅在使用者存取特定功能區域時啟動。

## 事件訂閱訊息的篩選器範例 {#examples-of-filters-for-event-subscriptions-messages}

為了示範如何篩選事件訂閱以僅接收與您組織相關的訊息，現在提供範常式式碼片段來篩選進入您端點的事件流程。 若要進一步瞭解檢視篩選範例，請參閱[篩選事件訂閱訊息](../../../../wf-api/api/filter-event-sub-messages.md)。
