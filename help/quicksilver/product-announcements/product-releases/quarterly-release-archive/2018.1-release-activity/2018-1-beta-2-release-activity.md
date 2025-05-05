---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.1 Beta 2發行活動
description: 本頁說明2018.1 Beta 2版本預覽環境中最近可用的所有變更。 此頁面的功能於2017年12月14日在預覽環境中提供。 它將在2018年3月的生產環境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 22e3836c-c41e-48a6-9926-e832af91e616
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1327'
ht-degree: 2%

---

# 2018.1 Beta 2發行活動

本頁說明2018.1 Beta 2版本預覽環境中最近可用的所有變更。 此頁面的功能於2017年12月14日在預覽環境中提供。 它將在2018年3月的生產環境中提供。

>[!IMPORTANT]
>
> 本頁所述的功能在生產環境使用之前可能會有所變更。

如需2018.1年度所有變更的清單，請參閱  [2018.1發行活動總覽](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md)。

2018.1 Beta 2版本包含適用於Workfront管理員和其他使用者的增強功能：

管理員的&#x200B;**&#x200B;**

* [使用者和版面配置範本的群組管理](#group-administration-for-users-and-layout-templates)

**所有使用者**

* [系統範圍寬熒幕顯示器](#system-wide-widescreen-display)
* [在甘特圖上調整時間表快照的大小](#resize-timeline-snapshot-on-the-gantt-chart)
* 業務案例中的[互動式資源規劃工具](#interactive-resource-planner-in-the-business-case)
* 資源規劃工具中的[視覺效果 — 使用者配置圖](#visualization-in-the-resource-planner-user-allocation-chart)
* 首頁區域中的[改善專案](#improvements-in-the-home-area)
* [新校訂檢視器改善](#new-proofing-viewer-improvements) 

## 使用者和版面配置範本的群組管理 {#group-administration-for-users-and-layout-templates}

您現在可以在Workfront中指定群組管理員。 「群組擁有者」欄位已重新命名為群組管理員，被指定為「群組管理員」的使用者擁有額外的許可權，可管理其管理之群組的使用者和配置範本。

* [群組管理員的使用者管理](#user-management-by-group-administrator)
* [群組管理員的版面配置範本管理](#layout-template-management-by-group-administrators)

### 群組管理員的使用者管理 {#user-management-by-group-administrator}

我們將介紹&#x200B;**群組管理員**&#x200B;的新概念。 為了支援此功能，**群組擁有者**&#x200B;欄位已重新命名為&#x200B;**群組管理員**，而且被指定為群組管理員的使用者擁有管理使用者和群組的額外許可權。

除了群組擁有者先前必須擁有的使用者管理許可權之外，群組管理員現在還可在群組內管理設定為群組管理員的使用者時，擁有下列額外存取許可權：

* 以屬於其所管理之群組的其他使用者身分登入。
* 重設屬於其所管理之群組的其他使用者的密碼。
* 建立由其群組管理的版面範本。 

在此變更之前，只有Workfront管理員可以執行這些功能。

如需群組管理員的詳細資訊，請參閱[建立群組](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)中的「瞭解群組管理員」一節。

### 群組管理員的版面配置範本管理 {#layout-template-management-by-group-administrators}

我們即將推出具有管理存取權的&#x200B;**群組**&#x200B;的新概念，您可以將其與配置範本建立關聯。

指定為此群組之群組管理員的使用者有權管理該版面配置範本並建立新的版面配置範本，其中他們管理的群組是範本的管理群組。 

在此變更之前，只有Workfront管理員可以建立版面配置範本。

如需有關建立版面配置範本的詳細資訊，請參閱建立和管理版面配置範本。

## 全系統寬熒幕顯示器 {#system-wide-widescreen-display}

當您在Workfront中顯示任何頁面時，系統會自動填滿整個瀏覽器視窗，並依照您的熒幕大小進行調整。

在此變更之前，只有與下列物件關聯的頁面會以寬熒幕顯示：

* 專案
* 任務
* 問題
* 報告
* 儀表板
* 行事曆

## 在甘特圖上調整時間表快照的大小 {#resize-timeline-snapshot-on-the-gantt-chart}

您現在可以展開時間表快照，以在甘特圖中顯示整個專案。

在此增強功能之前，您可以在時間軸快照上選取特定點，以便在甘特圖中導覽至該點。

如需有關設定資訊在甘特圖上的顯示方式的詳細資訊，請參閱[設定資訊在甘特圖上的顯示方式](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md)。

## 業務案例中的互動式資源規劃工具 {#interactive-resource-planner-in-the-business-case}

身為資源管理員，您現在可以在業務案例的資源預算區段中新增資源集區。 您也可以使用專案層次資源規劃工具來編列專案資源的預算。 將專案的資源編列預算會產生專案的預算勞力成本。

在此變更之前，如果專案已針對全域資源規劃工具中的資源編列預算，則您可以在業務案例中檢視資源預算資訊。

如需在業務案例中完成預算專案資源的詳細資訊，請參閱業務案例中的[預算資源](../../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)。

## 資源規劃工具 — 使用者配置圖中的視覺效果 {#visualization-in-the-resource-planner-user-allocation-chart}

您現在可以在「資源規劃工具」的圖表中顯示所有使用者對其可用性的整體計劃分配。 當您在資源規劃工具中選取&#x200B;**依使用者檢視**&#x200B;時，圖表可供使用。

圖表會顯示下列資訊：

* 所有使用者皆未過度配置的可用性 %
* 所有使用者的過度配置 %
* 所有使用者的使用量過低 %
* 此時間期間內有至少一位使用者過度配置

在此變更之前，您只能以表格格式檢視個別使用者的配置和可用性。

如需資源規劃工具中使用者配置圖表的詳細資訊，請參閱[資源規劃工具概觀](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)。

## 首頁區域的改善 {#improvements-in-the-home-area}

「首頁」區域現在提供各種改善功能，包括：

* 外觀與感覺改善

   * 右側面板現在已變大，可讓您有更多空間存放任務和問題資訊。
   * 在左側面板中選取時，逾期專案現在會以較淺的紅色顯示。
   * 您現在可以更輕鬆地檢視左面板與右面板之間的關係。 左側面板中選取的檔案指向右側面板。

* 顯示所選專案的預設欄位。 

  如需預設欄位的詳細資訊，請參閱建立及管理版面配置範本。

* 在請求上按一下「處理它」後，與問題相關的欄位將顯示在右側面板中。

  如需有關處理首頁區域的請求的詳細資訊，請參閱[管理首頁區域的工作和團隊請求](../../../../workfront-basics/using-home/using-the-home-area/manage-work-and-team-requests-home.md)中的[管理首頁區域的工作和團隊請求](../../../../workfront-basics/using-home/using-the-home-area/manage-work-and-team-requests-home.md)。

* 指向左側面板中工作專案上的使用者頭像，以檢視使用者名稱。
* 展開左側面板中的「延遲」區域以檢視所有延遲的專案（摺疊此區域時，只會顯示前5個專案）。
* 將專案標示為「完成」後，該專案會保留在左側面板中，直到您選取其他專案為止。\
  如需有關顯示已完成專案的資訊，請參閱[顯示首頁區域工作清單中的專案](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md)首頁區域工作清單中的專案[顯示首頁區域的工作清單](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md)。

如需有關使用新首頁區域的詳細資訊，以及說明「我的工作」和「首頁」之間功能差異的資訊，請參閱[使用首頁區域](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md)。

## 新校訂檢視器改進  {#new-proofing-viewer-improvements}

* [改善版面配置與設計](#improved-layout-and-design)
* [依據評論編號搜尋評論](#search-comments-by-comment-number)
* [標籤指標旁編輯註解的選項](#option-to-edit-comment-next-to-the-markup-indicator)
* [將所有評論標示為已讀取](#mark-all-comments-as-read)
* [左側功能表改良](#left-menu-improvements)

### 改善版面配置和設計 {#improved-layout-and-design}

校訂檢視器的外觀與風格均已更新。 此  下列校訂檢視器區域已更新：

* 縮圖區域

  如需有關使用縮圖區域的詳細資訊，請參閱中的。

* 評論區域\
  如需有關註解區域的詳細資訊，請參閱。
* 左側功能表區域

### 按評論編號搜尋評論 {#search-comments-by-comment-number}

現在，當您在校訂檢視器中搜尋註解清單時，可以在搜尋欄位中輸入註解號碼。 接著會篩選註解清單，以顯示您搜尋的註解。 

如需詳細資訊，請參閱中的。

### 標示指標旁的編輯註解選項 {#option-to-edit-comment-next-to-the-markup-indicator}

您現在可以更輕鬆地編輯現有註解。 按一下校樣上的註解指示器後，球標旁會顯示編輯圖示。 

在此變更之前，您必須按一下「註解」區域中的編輯圖示。  

如需詳細資訊，請參閱。

### 將所有註解標示為已讀取 {#mark-all-comments-as-read}

在校訂檢視器中檢視檔案時，您現在可以將所有註解標示為「已讀」。

### 左側功能表改良 {#left-menu-improvements}

校訂檢視器左側的功能表包含下列改良功能：

* 更新外觀
* 選單頂端的圖示可顯示或隱藏選單

  ![proof_viewer_menu_hide.png](assets/proof-viewer-menu-hide.png)

* 將滑鼠移到選單上以自動展開選單以檢檢視示以外的標籤。 （或啟用選項，讓功能表永遠在收合的檢視中。）
