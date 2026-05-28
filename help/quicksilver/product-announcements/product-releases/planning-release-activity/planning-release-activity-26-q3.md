---
content-type: release-notes
title: Adobe Workfront Planning 2026年第三季度發行活動
description: 這是2026年第三季的Adobe Workfront Planning產品發行活動。
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 12552dfefc58a664c278598496097f1b30d3cf0e
workflow-type: tm+mt
source-wordcount: '1448'
ht-degree: 0%

---

# Adobe Workfront Planning 2026年第三季度發行活動

<!--take the next sentence out when we start listing features-->

<!--
There are no features released during the Third Quarter Release for 2026. When features are released for this quarter, we will document them in this article. 
-->

<!--keep the sentence below for all future quarterly release pages-->

本文介紹2026年第三季度發行中針對Workfront Planning所推出的功能。

如需針對Adobe Workfront Planning發行之所有功能的清單，請參閱[Adobe Workfront Planning發行活動：文章索引](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md)。



<!--

## Planning Designer now available in Beta for all Workfront Planning customers

>[!NOTE]
>
>Preview: May 28, 2026 
>Production fast release: June 11, 2026 
>Production for everyone: July 16, 2026 
>[!BADGE In Beta]{type=Neutral}

You can now use the Adobe Planning Designer powered by AI to configure your workspaces and data structures with ease. The Planning Designer supports everything from creating and configuring workspaces to defining fields and formulas, managing records, reviewing change history and building custom views.  

Whether used directly or through the AI Assistant, the Planning Designer provides a flexible, powerful environment for building and maintaining structured, connected information. 

A Workfront administrator can manage the availability of the Planning Designer from the System Preferences area in Setup.   

For information, see [Get started with the Adobe Workfront Planning Designer](/help/quicksilver/planning/general/planning-ai-designer.md).

## New Sample workspaces tab added to the Planning landing page

>[!NOTE]
>
>Preview: May 28, 2026 
>Production fast release: June 11, 2026 
>Production for everyone: July 16, 2026 

We have added the Sample workspaces tab in the Planning landing area where you can view example of best-practice workspaces. The workspaces are not editable and we recommend that you use them as examples to create your own.  

We also recommend that you use the multi-workspace template to create, and edit and share workspaces that result as a use of that template.  The template contains the same workspaces as the Sample workspaces tab.   

Workspace managers can modify views in sample workspaces.     

For information, see Workspaces overview (/help/quicksilver/planning/architecture/workspaces-overview.md). 

-->

## Workfront Planning API 2

>[!NOTE]
>
>所有客戶皆可使用：2026年5月28日>[!BADGE 取消排程]{type=Neutral}

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
>預覽： 2026年5月28日>生產快速版本： 2026年6月11日>每個人的生產： 2026年7月16日

您現在可以調整個別記錄許可權，以控制誰可以在記錄型別中管理這些許可權。

依預設，使用者會從工作區和記錄型別繼承記錄許可權。 若要僅將記錄型別許可權授與特定使用者「管理」許可權給僅特定記錄，您可以停用特定記錄的繼承許可權，並僅授予這些使用者「管理」存取這些記錄的許可權。 您可以大量調整一筆記錄或同時調整多筆記錄的許可權。

您可以授予使用者下列許可權層級：

* 檢視
* 管理

>[!NOTE]
>
>* 使用者的記錄層級許可權不能超過其記錄型別許可權。 例如，對於記錄型別的具有檢視存取許可權的使用者，不能被授予該型別個別記錄的管理存取許可權。
>* 您目前無法從記錄中移除使用者的許可權。 至少具有該記錄型別檢視存取許可權的任何使用者都可以檢視該型別的所有記錄。

如需詳細資訊，請參閱[共用記錄](/help/quicksilver/planning/access/share-records.md)。

## 簡化全域記錄型別新增

>[!NOTE]
>
>預覽： 2026年5月28日>生產快速版本： 2026年6月11日>每個人的生產： 2026年7月16日

為了減少點按次數，並協助您快速找到所需的記錄型別，我們強化了新增記錄的體驗，讓您在將全域記錄型別新增到另一個工作區時，能更快且更直覺地新增記錄。

當您選擇從現有的記錄型別新增記錄時，您現在會立即看到所有可用的全域記錄型別清單。

您可以直接從這個畫面同時選取並新增一或多個全域記錄型別。

如需詳細資訊，請參閱[從其他工作區新增現有記錄型別](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md)。


## 將中繼資料從Planning同步至AEM Assets

>[!NOTE]
>
>預覽： 2026年5月28日>生產快發行： 2026年5月28日>所有人生產： 2026年5月28日>[!BADGE 排程外]{type=Neutral}

為了改善資料整合功能，我們已發佈在GenStudio for Performance Marketing記錄型別與AEM Assets之間的無縫中繼資料同步，當AEM Assets在Workfront Planning中連結至GenStudio記錄型別時。

下列GenStudio for Performance Marketing記錄型別可連線至AEM Assets：行銷活動、產品、角色、地區和頻道。

在Workfront Planning中新增至GenStudio記錄型別的資訊，會顯示在AEM中AEM資產的獨立Campaign索引標籤中。 該促銷活動的產品、角色、地區和頻道相關資訊，也會以唯讀模式顯示在該標籤上。

透過此發行版本，重要中繼資料在兩個平台上都是一致的，並近乎即時地反映更新，可減少手動協調。

如需詳細資訊，請參閱[在Adobe Workfront規劃中管理GenStudio工作區](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md)。

## 將中繼資料從Planning同步至AEM內容片段

>[!NOTE]
>
>預覽： 2026年5月28日>生產快發行： 2026年5月28日>所有人生產： 2026年5月28日>[!BADGE 排程外]{type=Neutral}

為了改善資料完整性，我們已在內容片段連結至AEM行銷活動時，在GenStudio工作區中的Planning記錄型別與GenStudio for Performance Marketing內容片段之間發佈順暢的中繼資料同步。

GenStudio促銷活動資訊現在顯示在AEM中內容片段的「中繼資料」標籤中。  該促銷活動的產品、角色、地區和頻道相關資訊，也會以唯讀模式顯示在該標籤上。

透過此發行版本，重要中繼資料在兩個平台上都是一致的，並近乎即時地反映更新，可減少手動協調。

如需詳細資訊，請參閱[在Adobe Workfront規劃中管理GenStudio工作區](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md)。


## 清單檢視更新

>[!NOTE]
>
>預覽： 2026年5月27日>生產快速版本： 2026年6月11日>每個人的生產： 2026年7月16日

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
>預覽： 2026年5月27日>生產快速發行： 2026年6月11日\
>適用於所有人的生產： 2026年7月16日

現在當您將Planning記錄型別與Workfront物件型別連線時，可以新增Workfront參考欄位做為查閱欄位。

例如，您可以從Project物件將Portfolio、方案、群組或公司資訊新增至Planning中行銷活動的專案連線欄位。

如需詳細資訊，請參閱[連線記錄型別](/help/quicksilver/planning/architecture/connect-record-types.md)。

## 時間表檢視劃分功能的新篩選器

>[!NOTE]
>
>預覽： 2026年5月27日>生產快速版本： 2026年6月11日>每個人的生產： 2026年7月16日

您現在可以根據符合記錄劃分中所包含物件的條件，來篩選時間軸檢視中的資訊。

在此增強功能之前，您只能對時間軸檢視中的主要記錄套用篩選器。

如需詳細資訊，請參閱[管理時間表檢視](/help/quicksilver/planning/views/manage-the-timeline-view.md)。

## 新指示已編輯和刪除的欄位會影響請求表單

>[!NOTE]
>
>預覽： 2026年5月27日>生產快速版本： 2026年6月11日>每個人的生產： 2026年7月16日

我們已新增提醒，提醒您編輯或刪除的記錄欄位可能會影響包含這些欄位的請求表單。 現在，您可以檢閱受影響的表單，並確保您想要對欄位進行的變更不會影響現有資訊。

如需詳細資訊，請參閱[編輯欄位設定](/help/quicksilver/planning/fields/edit-fields.md)。

## 編輯已提交的計畫請求

>[!NOTE]
>
>預覽： 2026年5月27日>生產快速版本： 2026年6月11日>每個人的生產： 2026年7月16日

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
>預覽： 2026年5月14日>生產快發行： 2026年5月14日>所有人生產： 2026年5月14日>[!BADGE 排程外]{type=Neutral}

為了在使用連線到Workfront Planning記錄的AEM內容片段時提高可見度，我們新增了一個預覽視窗，顯示Workfront Planning中片段的相關資訊。

此功能先前可用於AEM資產，而我們現在已將其新增至內容片段。

如需詳細資訊，請參閱[連線記錄](/help/quicksilver/planning/records/connect-records.md)。

## Workfront Planning中現在提供AEM內容片段的查詢欄位

>[!NOTE]
>
>預覽： 2026年5月14日>生產快發行： 2026年5月14日>所有人生產： 2026年5月14日>[!BADGE 排程外]{type=Neutral}

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
>預覽： 2026年5月14日>生產快速版本： 2026年6月11日>每個人的生產： 2026年7月16日

為了在記錄的詳細資訊頁面中顯示您的資訊提供更好的彈性，我們引進了建立此頁面自訂檢視的功能。

除了新增兩個已建置的詳細資料頁面檢視（包含所有記錄欄位或僅表格檢視中顯示的欄位）之外，您現在可以為記錄的詳細資料頁面建立自訂檢視。 您建立的檢視對可以存取該記錄的所有人都可見。

此更新會移除&#x200B;**顯示所有欄位**&#x200B;設定，並以自訂詳細資料檢視取代它。

如需詳細資訊，請參閱[管理記錄頁面](/help/quicksilver/planning/records/manage-the-record-page.md)。

## 將群組新增至「連線的專案」記錄頁面

>[!NOTE]
>
>預覽： 2026年5月14日\
>快速生產： 2026年6月11日>所有人生產： 2026年7月16日

您現在可以在Workfront Planning中，將資訊分組到記錄的專案連線記錄頁面中。 在此增強功能之前，此功能不存在於此區域。

如需詳細資訊，請參閱[管理清單檢視](/help/quicksilver/planning/views/manage-the-list-view.md)。
