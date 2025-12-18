---
content-type: release-notes
title: Adobe Workfront Planning 2026年第一季度發行活動
description: 這是Adobe Workfront Planning產品2026年第一季的發行活動。
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: a58e7da96c43dd308a213c6d7ef74d5085a2e1ba
workflow-type: tm+mt
source-wordcount: '1268'
ht-degree: 0%

---

# Adobe Workfront Planning 2026年第一季度發行活動

本文介紹2026年第一季度發行的Workfront Planning功能。

<!--keep the sentence below for all future quarterly release pages-->

如需針對Adobe Workfront Planning發行之所有功能的清單，請參閱[Adobe Workfront Planning發行活動：文章索引](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md)。

## 在「連線的專案」記錄頁面中共用檢視

>[!NOTE]
>
>預覽： 2025年12月18日
>生產環境快速發行： 2026年1月14日\
>適用於所有人的生產： 2026年1月15日

為了更方便確保可檢視您所需的資訊，我們新增了在「連線的專案記錄」頁面共用檢視的功能。 現在，您可以與其他使用者、團隊或群組共用檢視。

如需請求檢視的詳細資訊，包括共用，請參閱[在請求區域](/help/quicksilver/manage-work/requests/create-requests/create-views-for-requests-list.md)建立和管理檢視。

## 專案連線檢視篩選器現在提供目前的使用者萬用字元

>[!NOTE]
>
>預覽： 2025年12月18日
>生產環境快速發行： 2026年1月14日\
>適用於所有人的生產： 2026年1月15日

為了更方便篩選套用至您的專案連線，我們已建立目前的使用者萬用字元。 現在，篩選時，您可以選取「我（已登入使用者）」。 該篩選器將套用至正在檢視請求清單的使用者。

將篩選器新增至多個使用者將使用的檢視時，這會很方便。 每位使用者都會看到套用至他們的篩選結果。

值為使用者的欄位可使用萬用字元。

如需設定專案連線檢視的詳細資訊，包括篩選器，請參閱[新增連線記錄至記錄](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md)。

<!--

## Create record type hierarchies in workspaces

>[!NOTE]
>
>Preview: December 18, 2025 
>Production fast: January 14, 2026 
>Production all: January 15, 2026 

You can now define flexible but structured hierarchies between record or object types.  

Hierarchies are connections between record types. You can have up to 4 record and object types connected in one hierarchy, and you can have multiple hierarchies in one workspace. The first record type in the hierarchy is a parent, and all the other record or object types are its children objects.  

You can use hierarchies to organize work in a way that reflects how your teams actually plan, operate, and deliver and to visualize how strategy flows into execution. 

Consider the following when building hierarchies: 

* You can have multiple hierarchies in a workspace 
* You can connect only Planning record types from one workspace and Workfront projects in a hierarchy.  
* A record type or a project can only have one parent in the same workspace. 
* A record type can be the parent in multiple hierarchies 
* Connectable record types cannot be used in hierarchies in other workspaces than their own. 
* Global record types can be used in hierarchies only in the workspaces that they were created in or have been added to.  

When you create hierarchies between record types, they generate breadcrumbs for records that belong to those record types. 

For more information, see [Hierarchy and breadcrumb overview](help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

-->

<!--

## New unified breadcrumbs added to records' pages

>[!NOTE]
>
>Preview: December 18, 2025 
>Production fast: January 14, 2026 
>Production for all: January 15, 2026 

We have added breadcrumbs to a record's page to reflect its spot in a hierarchy. After you create hierarchies, you can see a record's breadcrumb at the top of its page, indicating what other parent or children objects are connected to it. Hierarchies are consistent across Workfront and Planning.  

For example, you can view a project's Planning hierarchy when it's connected to Planning record types in its Planning breadcrumb, and its Workfront hierarchy when it's connected to Workfront object types, like Portfolios or Programs, in Workfront.  

For information, see [Hierarchy and breadcrumb overview](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

-->

## Workspace主要頁面改善

>[!NOTE]
>
>預覽： 2025年12月18日
>生產快速： 2026年1月14日
>所有人的生產： 2026年1月15日

我們已對Workfront Planning中的「工作區」首頁面進行下列改良：

* 更快、更動態的捲動體驗。 如果您的組織擁有大量工作區且適合系統管理員使用，這會特別明顯。

* 我們新增了搜尋方塊，現在可讓您依名稱搜尋特定工作區。

* **其他工作區**&#x200B;索引標籤已重新命名為&#x200B;**所有工作區**，且包含您至少擁有檢視許可權的所有工作區，包括您建立的工作區。

如需詳細資訊，請參閱[編輯工作區](/help/quicksilver/planning/architecture/edit-workspaces.md)。

<!--

## Improvements to connected records pages

>[!NOTE]
>
>Preview: December 18, 2025 
>Production fast: January 14, 2026 
>Production for all: January 15, 2026 

To give you more flexibility when working with connected records pages, we have enhanced the functionality of views in this area of Workfront Planning. The following are improvements in the connected records pages of a record that are coming with this release:

* You can now add a timeline and a calendar view to a record's connected records page.
* You can now share views from a connected records page. The views shared from these pages are visible system-wide by all users you share them with in any other area of Workfront Planning. All views shared in any other areas of Planning are also visible in the connected records page for the same users they are shared with.
* We have added a restriction to only allow one connected records page per each record or object type. Prior to this enhancement, you could add multiple pages for the same record or object type. Now, you can use multiple views for the same record type in one connected records page.
* We have added a **New row** link at the bottom of a table view and a **Connect records** button in the upper-right area of the connected records page. Prior to this enhancement, the **New row** link and the **Connect records** button existed only on a project connected page. 

For information, see [Add a Connected records page to a record](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).

-->

## 在GenStudio工作區中依預設將Brand Connection欄位新增至「產品」和「角色」

>[!NOTE]
>
>預覽： 2025年12月11日
>生產快速發行： 2025年12月11日
>每個人都要生產： 2025年12月11日

具有GenStudio for Performance Marketing品牌的連線欄位現在預設會新增到Workfront Planning的GenStudio工作區中的「產品」和「角色」記錄型別。

貴組織必須同時具備Workfront Planning和Adobe GenStudio for Performance Marketing。

在此增強功能之前，您只能手動將Brand Connection欄位新增到任何記錄型別，包括Products和Personas。 您仍然可以在Workfront Planning中手動將Brand GenStudio記錄型別連結至其他記錄型別。

如需詳細資訊，請參閱[開始使用Adobe Workfront Planning與Adobe GenStudio for Performance Marketing整合](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md)。

## 限制從Planning移除GenStudio for Performance Marketing使用者的許可權

>[!NOTE]
>
>預覽： 2025年12月11日
>生產快速發行： 2025年12月11日
>每個人都要生產： 2025年12月11日

我們新增了護欄，可防止您從Workfront Planning物件中移除GenStudio for Performance Marketing使用者的許可權。 經過這項改善後，您將無法再從Planning的GenStudio工作區中移除GenStudio使用者，也無法對GenStudio工作區中的記錄型別停用繼承許可權(如果這些許可權包含GenStudio使用者)。 在此改善之前，當您從Planning中的GenStudio工作區移除這些使用者時，他們也會失去在GenStudio中記錄型別的許可權。

貴組織必須同時具備Workfront Planning和Adobe GenStudio for Performance Marketing。

如需詳細資訊，請參閱[開始使用Adobe Workfront Planning與Adobe GenStudio for Performance Marketing整合](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md)。


## 已移除次要工作區中全域記錄型別的公開檢視共用


>[!NOTE]
>
>預覽： 2025年12月3日
>生產快速發行： 2025年12月4日
>適用於所有人的生產： 2026年1月15日


在次要工作區中共用全域記錄的檢視時，我們已移除「公用共用」索引標籤。 您無法從現有全域記錄型別新增到另一個工作區的全域記錄型別公開共用檢視。 您可以從原始工作區公開共用全域記錄型別檢視。

如需詳細資訊，請參閱[共用檢視](/help/quicksilver/planning/access/share-views.md)。


## 連結GenStudio for Performance Marketing Brands與Workfront Planning記錄型別

>[!NOTE]
>
>預覽： 2025年11月13日
>生產快速發行： 2025年11月13日
>適用於所有人的生產： 2025年11月13日

您現在可以將Workfront Planning記錄型別與Adobe GenStudio for Performance Marketing的品牌連結起來。 貴組織必須同時具備Workfront Planning和Adobe GenStudio for Performance Marketing。

如需詳細資訊，請參閱[連線記錄型別](/help/quicksilver/planning/architecture/connect-record-types.md)。


## Planning檢視中，篩選器、欄位和列顏色圖示的新欄位搜尋方塊

>[!NOTE]
>
>預覽： 2025年11月6日
>生產快速發行： 2025年12月11日
>適用於所有人的生產： 2026年1月15日

在記錄型別檢視中建立檢視元素時，您現在可以搜尋特定欄位。 當您建立篩選、排序、分組，或設定欄位或列顏色時，我們已新增搜尋方塊。 在此增強功能之前，您只需捲動瀏覽可用欄位清單。

這項改善適用於所有記錄型別檢視。

如需詳細資訊，請參閱[管理資料表檢視](/help/quicksilver/planning/views/manage-the-table-view.md)。


## 全域記錄型別，以及將全域記錄型別新增為其他工作區現有記錄型別的能力

>[!NOTE]
>
>預覽： 2025年10月16日
>生產快速發行： 2025年11月13日
>適用於所有人的生產： 2026年1月15日

針對具有通用工作流程的多團隊組織實作Workfront Planning時，您可能需要為關鍵記錄型別（例如行銷活動或交付專案）定義一致結構和中繼資料，這些記錄型別可以新增到每個團隊的工作區，以擷取和管理其工作。

此外，您可能需要每個團隊的工作彙總到中央層級。

在此類工作流程中，您可以確保團隊在解鎖跨團隊可見度的同時一致地擷取其工作，而無需將組織中的每個人新增到每個工作區。 您可以使用全域記錄型別來達成此目的。

您現在可以將記錄型別指定為全域，並跨多個工作區使用它。 使用者可以使用已在中央工作區中設定的相同欄位結構和連線。

如需詳細資訊，請參閱下列文章：

* [跨工作區記錄型別概觀](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md)

* [設定記錄型別跨工作區功能](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)

* [從另一個工作區新增現有記錄型別](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md)

## 單一記錄型別的連線欄位新限制

>[!NOTE]
>
>預覽： 2025年10月16日
>生產快速發行： 2025年11月13日
>適用於所有人的生產： 2026年1月15日

我們引進了每個記錄型別30個連線欄位的限制。

注意：如果貴組織目前有一個記錄型別的連線欄位超過30個，您可以保留超過30個限制的其他欄位。 但是，您無法向超過限制的記錄型別新增更多連線欄位。 日後，將強制執行30個連線欄位的新限制。

如需詳細資訊，請參閱[連線記錄型別總覽](/help/quicksilver/planning/architecture/connect-record-types-overview.md)。

## 為選取型別的欄位選擇設定好記的值

>[!NOTE]
>
>預覽： 2025年10月16日
>生產快速發行： 2025年11月13日
>適用於所有人的生產： 2026年1月15日

將欄位選擇新增至單選或多選欄位時，Workfront現在會為每個選擇指派不重複的使用者友善值。 在此改善之前，Workfront產生的英數字元ID難以瞭解及用於API呼叫和其他整合。

改良時應考量下列事項：

* 新值將新增到新的欄位選擇中。 現有欄位選擇將保留其英數字元ID。

* 一個欄位的選擇值是唯一的，但可在不同欄位之間重複。

* 重新命名選擇不會更新其原始值。

* 選擇值會以小寫顯示，若為多字選擇，則會以底線分隔。 如果您使用已用作相同欄位另一個選擇名稱的標籤，Workfront會將連續數字新增至值。

如需詳細資訊，請參閱[建立欄位](/help/quicksilver/planning/fields/create-fields.md)。






