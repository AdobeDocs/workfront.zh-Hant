---
content-type: release-notes
title: Adobe Workfront Planning 2026年第三季度發行活動
description: 這是2026年第三季的Adobe Workfront Planning產品發行活動。
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 63f9627ccda9080a9ce505963f9ee495ccfbd8f3
workflow-type: tm+mt
source-wordcount: '2809'
ht-degree: 0%

---

# Adobe Workfront Planning 2026年第三季度發行活動

<!--
take the next sentence out when we start listing features
-->

<!--
There are no features released during the Third Quarter Release for 2026. When features are released for this quarter, we will document them in this article. 
-->

<!--keep the sentence below for all future quarterly release pages-->

本文介紹2026年第三季度發行中針對Workfront Planning所推出的功能。

如需針對Adobe Workfront Planning發行之所有功能的清單，請參閱[Adobe Workfront Planning發行活動：文章索引](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md)。

## Snowflake中Workfront Planning的自動化存取控制

>[!IMPORTANT]
>
>所有客戶的預覽和生產： 2026年7月16日不在排程&rbrack;{type=Neutral}內


此發行版本引入了Snowflake中Workfront Planning資料的自動化、權益導向式存取管理，作為Workfront Data Connect的一部分。

首先，將安全檢視的產生延伸至Planning表格，建立下游存取控制的必要基礎，並使基於權利的授權成為可能。

以此為基礎，讀取器帳戶布建現在會在建立時檢查TMS權益，並自動套用或保留Planning資料庫的授權，以確保正確無誤。

在此增強功能之前，這僅適用於Workfront。

此更新包含下列功能：

* 自動的每日工作會偵測現有客戶的權益變更
* 新工作會根據許可權授予、撤銷或保留存取權
* 提供完整的生命週期涵蓋範圍，涵蓋布建、建立帳戶及進行中的權益變更。

[Workfront Data Connect資料字典](/help/quicksilver/reports-and-dashboards/data-lake/data-dictionary.md)文章將在發行日期後更新。


## 設定記錄的預設許可權

>[!NOTE]
>
>預覽： 2026年7月7日生產快速發行： 2026年7月15日適用於所有人的生產： 2026年7月16日

Workspace管理員現在可以為每種記錄型別設定預設許可權規則（開啟或限制），因此新建立的記錄會自動受到保護，無需任何手動步驟。

當您選取「受限制的」時，只有記錄建立者以及任何明確選取的使用者、群組、團隊、角色或公司可以編輯記錄，而其他所有人將保留僅供檢視的存取權。

此規則會自動套用至新記錄，無論記錄的建立方式為何（新記錄按鈕、請求表單、API、使用Fusion自動化或AI助理）。 規則的變更只會影響往後建立的記錄，而不會影響現有記錄。

建立記錄後，其許可權仍可以獨立更新，而不會影響未來記錄的預設規則。

如需詳細資訊，請參閱[設定記錄的預設許可權](/help/quicksilver/planning/access/set-default-record-permissions.md)。

## 時間軸檢視的泳道群組配置

>[!NOTE]
>
>預覽： 2026年7月7日生產快速發行： 2026年7月15日適用於所有人的生產： 2026年7月16日

群組的時間軸檢視現在支援泳道配置，群組呈現為凍結的左側標題欄，而不是捲動水準帶。 此群組型別是目前棧疊群組的額外型別。

巢狀群組層級會顯示為縮排的子欄，而每個車道中的記錄都會保持子棧疊和排序狀態。

您可以在群組檢視表中拖放記錄，以順利更新其資訊和日期。

所有檢視的使用者都可以看見套用的群組。

如需詳細資訊，請參閱[管理時間表檢視](/help/quicksilver/planning/views/manage-the-timeline-view.md)。


## 支援畫布儀表板中的貨幣計畫欄位

>[!NOTE]
>
>預覽： 2026年6月25日生產快速發行： 2026年7月15日適用於所有人的生產： 2026年7月16日

您現在可以在「畫布控制面板」的表格、重要績效指標及圖表報表中，加入貨幣計畫欄位。

在此增強功能之前，畫布儀表板中不支援貨幣欄位。

如需詳細資訊，請參閱[在畫布儀表板中使用貨幣欄位](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-canvas-dashboards/switch-currencies.md)。

## 列色彩控制項介面改善

>[!NOTE]
>
>預覽： 2026年6月22日生產快速發行： 2026年7月15日適用於所有人的生產： 2026年7月16日

我們更新了表格檢視中「列」顏色控制項的外觀和風格。

如需詳細資訊，請參閱[管理資料表檢視](/help/quicksilver/planning/views/manage-the-table-view.md)。

## 新增選取欄位與人員型態欄位的預設選擇

>[!NOTE]
>
>預覽： 2026年6月18日生產快速發行： 2026年7月15日適用於所有人的生產： 2026年7月16日

當您建立單一、多重選取的欄位或「人員」型態欄位時，您現在可以指定這些欄位的預設值。 當欄位在記錄上可見時，將一律套用預設值。

儲存欄位後，您可以變更欄位的預設設定。 處理記錄時，您可以取代欄位的預設值。

如需詳細資訊，請參閱[建立欄位](/help/quicksilver/planning/fields/create-fields.md)。

## 表格檢視中的介面改善

>[!NOTE]
>
>預覽： 2026年6月11日生產快速發行： 2026年7月15日適用於所有人的生產： 2026年7月16日

我們已更新Workfront Planning中下列區域的表格檢視外觀：

* 所有記錄型別頁面

* 所有連線的記錄型別頁面，專案除外

除了某些導覽變更和設計改進，此更新中的某些改進包括：

* 在表格底部加入彙總列，使用下列彙總來彙總數字、貨幣、百分比和一些公式欄位：SUM、AVG、MAX、MIN。

* 新增日期欄位時，採用較簡單的日期格式，格式型別較少。

* 新增日期欄位時，能夠選取所有使用者可見的時區，無論其設定檔的時區為何。

* 移除列編號，讓外觀更乾淨

* 「持續列」選取方塊，而非僅在暫留列時顯示

* 持續使用欄分隔符號行以提高可讀性

* 從欄標題排序時更簡單的排序體驗

如需詳細資訊，請參閱[管理資料表檢視](/help/quicksilver/planning/views/manage-the-table-view.md)。


## 現在可將GenStudio for Performance Marketing品牌新增至Planning請求表單

>[!NOTE]
>
>所有客戶的預覽和生產： 2026年6月5日僅適用於也擁有Adobe GenStudio for Performance Marketing的Adobe Workfront Planning客戶。不在排程&rbrack;{type=Neutral}內


若要讓您從提交請求開始，將品牌新增至行銷活動，您現在可以將「品牌已連線」記錄欄位新增至「計畫」請求表單。

當Planning記錄型別與GenStudio Brands記錄型別連結時，您可以將Brands connected欄位新增至與Planning記錄型別關聯的Planning請求表單。

如需詳細資訊，請參閱[開始使用Adobe Workfront Planning與Adobe GenStudio for Performance Marketing整合](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md)。


## 新增「範例工作區」索引標籤至Planning登陸頁面

>[!NOTE]
>
>預覽： 2026年6月1日生產環境快速發行： 2026年6月11日適用於所有人的生產： 2026年7月16日

我們已在Planning登陸區中新增「範例工作區」索引標籤，您可在此檢視最佳實務工作區範例。 工作區不可編輯。 Workspace管理員可以修改範例工作區中的檢視。 標準和系統管理員使用者可看見此索引標籤。

我們建議您檢視範例工作區作為範例，並使用多工作區範本組合來建立、編輯和共用以該範本產生的工作區。  範本束包含與「範例工作區」標籤相同的工作區。

如需詳細資訊，請參閱[工作區概述](/help/quicksilver/planning/architecture/workspaces-overview.md)。

## Workfront Planning API 2

>[!NOTE]
>
>所有客戶皆可使用： 2026年5月28日不在排程&rbrack;{type=Neutral}內

Workfront Planning API第2版現已可用，並大幅擴充第1版的功能。

版本2中包括下列增強功能：

* 以程式設計方式建立、更新和刪除工作區、記錄型別和欄位。

* 完整管理記錄。
* 改善URL結構、錯誤處理、分頁、篩選和許可權。
* 包括透過PATCH的部分更新
* 包含大量記錄作業。

第1版仍可使用，但建議您改用第2版。

>[!NOTE]
>
>適用於Fusion的Workfront Planning聯結器尚未更新為API版本2，在進一步通知之前，它將繼續使用版本1。

如需詳細資訊，請參閱[Adobe Workfront Planning API基本知識](/help/quicksilver/planning/general/planning-api-basics.md)。

如需Workfront Planning API的規格，請參閱[Workfront Planning API](https://developer.adobe.com/wf-planning/)開發人員檔案。

## 授予記錄許可權

>[!NOTE]
>
>預覽： 2026年5月28日生產環境快速發行： 2026年6月11日適用於所有人的生產： 2026年7月16日


您現在可以調整個別記錄許可權，以控制誰可以在記錄型別中管理這些許可權。

依預設，使用者會從工作區和記錄型別繼承記錄許可權。 您現在可以覆寫特定記錄的繼承許可權，以授與使用者子集的「檢視」或「管理」存取權。 許可權覆寫可以套用至個別記錄，或大量更新多個記錄。

<!-- 
Laurel asked for this to be replaced with the above: 

Users inherit record permissions from the workspace and record type by default. To give only select users with record type permissions Manage permissions to only certain records, you can disable inherited permissions on select records and grant only those users Manage access to those records. You can adjust permissions for one record, or for multiple records at the same time, in bulk.

You can give users the following permissions levels: 

* View 
* Manage 
-->

>[!NOTE]
>
>* 使用者的記錄層級許可權不能超過其記錄型別許可權。 例如，對於記錄型別的具有檢視存取許可權的使用者，不能被授予該型別個別記錄的管理存取許可權。
>* 您目前無法從記錄中移除使用者的許可權。 至少具有該記錄型別檢視存取許可權的任何使用者都可以檢視該型別的所有記錄。

如需詳細資訊，請參閱[共用記錄](/help/quicksilver/planning/access/share-records.md)。

## 簡化全域記錄型別新增

>[!NOTE]
>
>預覽： 2026年5月28日生產環境快速發行： 2026年6月11日適用於所有人的生產： 2026年7月16日

為了減少點按次數，並協助您快速找到所需的記錄型別，我們強化了新增記錄的體驗，讓您在將全域記錄型別新增到另一個工作區時，能更快且更直覺地新增記錄。

當您選擇從現有的記錄型別新增記錄時，您現在會立即看到所有可用的全域記錄型別清單。

您可以直接從這個畫面同時選取並新增一或多個全域記錄型別。

如需詳細資訊，請參閱[從其他工作區新增現有記錄型別](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md)。

## Beta現在提供所有Designer Planning客戶的Planning Workfront

>[!NOTE]
>
>預覽： 2026年5月28日生產環境快速發行： 2026年6月11日適用於所有人的生產： 2026年7月16日在Beta&rbrack;{type=Neutral}

您現在可以使用由AI支援的Adobe Planning Designer，輕鬆設定工作區和資料結構。 Planning Designer支援從建立和設定工作區到定義欄位和公式、管理記錄、檢閱變更記錄和建立自訂檢視的所有功能。

不論是直接使用或透過AI Assistant使用，Planning Designer都能提供彈性、強大的環境，用於建立及維護結構化、連線的資訊。

Workfront管理員可從「設定」的「系統偏好設定」區域管理Planning Designer的可用性。

如需詳細資訊，請參閱[開始使用Adobe Workfront Planning Designer](/help/quicksilver/planning/general/planning-ai-designer.md)。


## 將中繼資料從Planning同步至AEM Assets

>[!NOTE]
>
>每個人都能預覽和生產： 2026年5月28日僅適用於同時擁有Adobe GenStudio for Performance Marketing和Adobe Experience Manager的Adobe Workfront Planning客戶。不在排程&rbrack;{type=Neutral}內

為了改善資料整合功能，我們已發佈在GenStudio for Performance Marketing記錄型別與AEM Assets之間的無縫中繼資料同步，當AEM Assets在Workfront Planning中連結至GenStudio記錄型別時。

下列GenStudio for Performance Marketing記錄型別可連線至AEM Assets：行銷活動、產品、角色、地區和頻道。

在Workfront Planning中新增至GenStudio記錄型別的資訊，會顯示在AEM中AEM資產的獨立Campaign索引標籤中。 該促銷活動的產品、角色、地區和頻道相關資訊，也會以唯讀模式顯示在該標籤上。

透過此發行版本，重要中繼資料在兩個平台上都是一致的，並近乎即時地反映更新，可減少手動協調。

如需詳細資訊，請參閱[在Adobe Workfront規劃中管理GenStudio工作區](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md)。

## 將中繼資料從Planning同步至AEM內容片段

>[!NOTE]
>
>每個人都能預覽和生產： 2026年5月28日僅適用於同時擁有Adobe GenStudio for Performance Marketing和Adobe Experience Manager的Adobe Workfront Planning客戶。不在排程&rbrack;{type=Neutral}內

為了改善資料完整性，我們已在內容片段連結至AEM行銷活動時，在GenStudio工作區中的Planning記錄型別與GenStudio for Performance Marketing內容片段之間發佈順暢的中繼資料同步。

GenStudio促銷活動資訊現在顯示在AEM中內容片段的「中繼資料」標籤中。  該促銷活動的產品、角色、地區和頻道相關資訊，也會以唯讀模式顯示在該標籤上。

透過此發行版本，重要中繼資料在兩個平台上都是一致的，並近乎即時地反映更新，可減少手動協調。

如需詳細資訊，請參閱[在Adobe Workfront規劃中管理GenStudio工作區](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md)。


## 清單檢視更新

>[!NOTE]
>
>預覽： 2026年5月27日生產環境快速發行： 2026年6月11日適用於所有人的生產： 2026年7月16日

清單檢視上的多個欄位型別已更新，包括鍵盤導覽和其他增強功能。

多選、單選和受指派人欄位現在提供清單檢視中的鍵盤導覽：

* 使用鍵盤上的向上和向下箭頭在人員清單中移動。

* 按空格鍵以選取人員或移除選取的人員。

在清單檢視中的單一和多重選取欄位上：

* 找不到結果時，可以直接從編輯器新增選項。 請注意，並非所有清單都提供此功能。

* 欄位互動現在可使用鍵盤存取。 這包括標籤之間的導覽、搜尋選項，以及使用向上和向下箭頭的清單。 按空格鍵以選取專案或移除選取的專案。

參考欄位（例如預先輸入和外部查詢欄位）已收到一些介面增強功能。

此外，在可用的情況下，拖放欄的體驗已獲得視覺上的改善。

如需詳細資訊，請參閱[在Adobe Workfront規劃中管理清單檢視](/help/quicksilver/planning/views/manage-the-list-view.md)。

## Workfront參考欄位可作為Planning連線的查閱欄位啟用

>[!NOTE]
>
>預覽： 2026年5月27日生產環境快速發行： 2026年6月11日\
>適用於所有人的生產： 2026年7月16日

現在當您將Planning記錄型別與Workfront物件型別連線時，可以新增Workfront參考欄位做為查閱欄位。

例如，您可以從Project物件將Portfolio、方案、群組或公司資訊新增至Planning中行銷活動的專案連線欄位。

如需詳細資訊，請參閱[連線記錄型別](/help/quicksilver/planning/architecture/connect-record-types.md)。

## 時間表檢視劃分功能的新篩選器

>[!NOTE]
>
>預覽： 2026年5月27日生產環境快速發行： 2026年6月11日適用於所有人的生產： 2026年7月16日

您現在可以根據符合記錄劃分中所包含物件的條件，來篩選時間軸檢視中的資訊。

在此增強功能之前，您只能對時間軸檢視中的主要記錄套用篩選器。

如需詳細資訊，請參閱[管理時間表檢視](/help/quicksilver/planning/views/manage-the-timeline-view.md)。

## 新指示已編輯和刪除的欄位會影響請求表單

>[!NOTE]
>
>預覽： 2026年5月27日生產環境快速發行： 2026年6月11日適用於所有人的生產： 2026年7月16日

我們已新增提醒，提醒您編輯或刪除的記錄欄位可能會影響包含這些欄位的請求表單。 現在，您可以檢閱受影響的表單，並確保您想要對欄位進行的變更不會影響現有資訊。

如需詳細資訊，請參閱[編輯欄位設定](/help/quicksilver/planning/fields/edit-fields.md)。

## 編輯已提交的計畫請求

>[!NOTE]
>
>預覽： 2026年5月27日生產環境快速發行： 2026年6月11日適用於所有人的生產： 2026年7月16日

您現在可以在提交Planning請求之後，從請求建立記錄之前，編輯這些請求。

下列使用者可以編輯提交的請求：

* 請求建立者
* 已提交請求的工作區的Workspace管理員
* 系統管理員

在此增強功能之前，您無法編輯已提交的請求。

如需詳細資訊，請參閱[提交Adobe Workfront Planning要求以建立記錄](/help/quicksilver/planning/requests/submit-requests.md)。

## 新的AEM內容片段預覽視窗

>[!NOTE]
>
>所有客戶的預覽和生產： 2026年5月14日不在排程&rbrack;{type=Neutral}內

為了在使用連線到Workfront Planning記錄的AEM內容片段時提高可見度，我們新增了一個預覽視窗，顯示Workfront Planning中片段的相關資訊。

此功能先前可用於AEM資產，而我們現在已將其新增至內容片段。

如需詳細資訊，請參閱[連線記錄](/help/quicksilver/planning/records/connect-records.md)。

## Workfront Planning中現在提供AEM內容片段的查詢欄位

>[!NOTE]
>
>所有客戶的預覽和生產： 2026年5月14日僅適用於也擁有Adobe Experience Manager的Adobe Workfront Planning客戶。不在排程&rbrack;{type=Neutral}內

當您將Planning記錄型別連線至AEM內容片段時，現在可以新增下列查閱欄位：

* 建立者
* 建立時間
* 修改者
* 修改時間

在此增強功能之前，查詢欄位僅適用於AEM資產和資料夾。

如需詳細資訊，請參閱[連線記錄型別](/help/quicksilver/planning/architecture/connect-record-types.md)。



## 記錄的詳細資訊頁面的自訂檢視

>[!NOTE]
>
>預覽： 2026年5月14日生產環境快速發行： 2026年6月11日適用於所有人的生產： 2026年7月16日

為了在記錄的詳細資訊頁面中顯示您的資訊提供更好的彈性，我們引進了建立此頁面自訂檢視的功能。

除了新增兩個已建置的詳細資料頁面檢視（包含所有記錄欄位或僅表格檢視中顯示的欄位）之外，您現在可以為記錄的詳細資料頁面建立自訂檢視。 您建立的檢視對可以存取該記錄的所有人都可見。

此更新會移除&#x200B;**顯示所有欄位**&#x200B;設定，並以自訂詳細資料檢視取代它。

如需詳細資訊，請參閱[管理記錄頁面](/help/quicksilver/planning/records/manage-the-record-page.md)。

## 將群組新增至「連線的專案」記錄頁面

>[!NOTE]
>
>預覽： 2026年5月14日\
>生產快速： 2026年6月11日適用於所有人的生產： 2026年7月16日

您現在可以在Workfront Planning中，將資訊分組到記錄的專案連線記錄頁面中。 在此增強功能之前，此功能不存在於此區域。

如需詳細資訊，請參閱[管理清單檢視](/help/quicksilver/planning/views/manage-the-list-view.md)。

