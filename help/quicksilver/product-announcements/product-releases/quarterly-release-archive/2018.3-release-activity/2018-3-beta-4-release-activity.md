---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.3 Beta 4發行活動
description: 本頁說明2018.3 Beta 4版本預覽環境中最近可用的所有變更。 此功能將於2018年8月30日在預覽環境中提供。 它將於2018年11月在生產環境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: b40eda2c-8ad4-4945-a7e3-cb28ed8a14db
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1126'
ht-degree: 0%

---

# 2018.3 Beta 4發行活動

本頁說明2018.3 Beta 4版本預覽環境中最近可用的所有變更。 此功能將於2018年8月30日在預覽環境中提供。 它將於2018年11月在生產環境中提供。

如需2018.3年所有變更的清單，請參閱  [2018.3發行活動總覽](../../../../product-announcements/product-releases/quarterly-release-archive/2018.3-release-activity/2018-3-release-activity-overview.md)。

2018.3 Beta 4版本包含適用於Workfront管理員和其他使用者的增強功能：

管理員的&#x200B;**&#x200B;**

* [以群組管理員身分更新使用者設定檔中的報告結構](#update-reporting-structure-in-the-user-profile-as-a-group-administrator) 

**所有使用者**

* [從資源規劃工具匯出更多資訊](#export-more-information-from-the-resource-planner)
* [工作清單改善](#task-list-improvements)已從發行版本中移除
* [專案清單改善](#project-list-improvements)
* [在甘特圖編輯模式下編輯工作清單](#editing-the-task-list-in-gantt-chart-edit-mode)已從發行版本移除
* [測量工具色彩](#measurement-tool-colors)
* 在新索引標籤[&#128279;](#proofs-open-in-a-new-tab)中開啟的校訂已從發行版本中移除

* [列印摘要增強功能](#print-summary-enhancements)
* [在Workfront行動應用程式中記錄時間（以天為單位）](#log-time-in-days-in-the-workfront-mobile-app)

## 以群組管理員的身分更新使用者設定檔中的報告結構 {#update-reporting-structure-in-the-user-profile-as-a-group-administrator}

群組管理員現在可以編輯他們所管理群組之使用者的「直接下屬」和「下屬對象」欄位。

之前，只有Workfront管理員和對使用者具有管理存取許可權的使用者才能擁有此功能。

如需群組管理員的相關資訊，請參閱[群組管理員](../../../../administration-and-setup/manage-groups/group-roles/group-administrators.md)。

## 從資源規劃工具匯出更多資訊 {#export-more-information-from-the-resource-planner}

您現在可以在資源規劃工具中匯出最多52週、36個月或12季的資訊。 如果您要匯出的資訊量太大，您會收到附有已匯出檔案的電子郵件。 從開始下載開始，您最多可以下載一週的檔案。

過去，您一次最多只能匯出4週、月或季度。

如需詳細資訊，請參閱[從資源規劃工具](../../../../resource-mgmt/resource-planning/export-resource-planner.md)匯出資訊。

## 任務清單改善 {#task-list-improvements}

>[!NOTE]
>
>* 此功能已從預覽環境中移除，將不會包含在2018.3版本中。 它將在稍後發行。

檢視工作清單時，現在有新體驗可用。 此體驗包括提升效能，以及更順暢且更快速的清單導覽。

也可使用下列可見的變更：

* 依預設，群組會摺疊。\
  在此變更之前，依預設會展開群組。
* 快速篩選器已新增至工作清單。
* 向下捲動工作清單時，專案標題仍會顯示。
* 新狀態圖示可供使用。

工作清單中的下列功能已變更：

* 按右鍵功能及其提供的內容功能表。\
  與其在任務上按一下右鍵進行編輯，您可以進行下列操作：

   * 當您選取單一任務時，您現在可以使用「更多」選單，其選項與上一個右鍵選單相同。
   * 選取多個工作時，您可以使用清單頂端的圖示，來執行上一個滑鼠右鍵功能表中包含的任何動作。

     所有變更都會顯示在專案內的任務清單中，以及任務底下的子任務標籤中。

如需使用清單的詳細資訊，請參閱[開始使用Adobe Workfront中的清單](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)。

如需有關在甘特圖中鏈結任務的詳細資訊，請參閱[透過鏈結任務建立前置任務關係](../../../../manage-work/tasks/use-prdcssrs/create-predecessors-by-chaining-tasks.md)。

## 專案清單改善 {#project-list-improvements}

重新排序欄的功能已新增回下列子索引標籤中的專案清單：

* 我擁有的專案
* 我參與的專案
* 所有專案

此功能已在2018.2版本中移除。

如需使用清單的詳細資訊，請參閱[開始使用Adobe Workfront中的清單](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)。

## 在甘特圖編輯模式下編輯工作清單 {#editing-the-task-list-in-gantt-chart-edit-mode}

>[!NOTE]
>
>* 此功能已從預覽環境中移除，將不會包含在2018.3版本中。 它將在稍後發行。

當專案中的任務以甘特圖的編輯模式顯示時，您現在可以對它們執行下列動作：

* 新增任務
* 移除任務
* 內聯編輯任務

雖然您可以看到變更如何影響專案的時間表，但變更不會立即生效。 您可以儲存它們以更新專案時間表，也可以取消它們。

以前，當任務以甘特圖的編輯模式顯示時，您無法對這些任務執行這些動作。 您可以在未顯示在甘特圖中的工作清單中進行這些變更，但變更會立即生效。

如需有關編輯甘特圖中的工作的資訊，請參閱工作清單甘特圖中的[更新資訊](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md)。

## 測量工具顏色 {#measurement-tool-colors}

當您使用測量工具來測量校樣上的區域時，您現在可以變更工具顏色和不透明度。 Workfront會在您開啟的所有校樣中記住這些設定，直到您清空瀏覽器快取為止。

預設顏色現在為紅色。

以前，測量工具僅以藍色顯示，這使得在包含類似藍色調的校樣內容上難以看到。

## 在新標籤中開啟的校訂 {#proofs-open-in-a-new-tab}

>[!NOTE]
>
>* 此功能已從預覽環境中移除，將不會包含在2018.3版本中。

現在當您在Workfront或Workfront Proof中的任何地方開啟校訂時，校訂檢視器會在新的瀏覽器標籤中啟動，且焦點會切換到該標籤。 您可以在多個瀏覽器標籤中工作，檢閱校樣並繼續在Workfront或Workfront Proof中處理專案、任務和問題。

之前，校訂檢視器會在您目前Workfront或Workfront Proof瀏覽器標籤上方的框架中啟動，導致該標籤無法存取，直到您關閉校訂檢視器為止。

如需詳細資訊，請參閱。

## 列印摘要增強功能 {#print-summary-enhancements}

當您列印校樣或將其儲存為PDF或XLS檔案時，列印摘要頁面上現在提供下列增強功能：

* 您可以依建立者來排序校訂的註解。

  之前，您可以依照建立評論的順序或評論在每個頁面上的出現順序來排序評論。

* 您可以依作者、動作和未解決狀態來篩選校訂的註解。

  以前，列印摘要頁面上無法使用評論篩選功能。

* 現在包含階段以及每個階段的詳細資訊。

  以前不包含階段。

如需詳細資訊，請參閱[在Adobe Workfront中列印校訂摘要](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/print-proof-summary-in-wf.md)。

## 在Workfront行動應用程式中記錄時間（以天為單位） {#log-time-in-days-in-the-workfront-mobile-app}

您現在可以在Workfront行動應用程式中記錄時間（以天為單位）。 

以前，即使您的設定檔偏好設定設為以天為單位記錄時間，您也只能在行動應用程式中使用小時來記錄時間。

如需在行動應用程式中記錄時間的詳細資訊，請參閱。 

此功能可立即透過Android Beta應用程式進行測試。 
