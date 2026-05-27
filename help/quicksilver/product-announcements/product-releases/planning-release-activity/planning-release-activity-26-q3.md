---
content-type: release-notes
title: Adobe Workfront Planning 2026年第三季度發行活動
description: 這是2026年第三季的Adobe Workfront Planning產品發行活動。
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: f11daa69f72c32418298ac75f81b0fb64835d99b
workflow-type: tm+mt
source-wordcount: '406'
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

## List view updates 

>[!NOTE]
>
>Preview: May 28, 2026
>Production fast release: June 11, 2026
>Production for everyone: July 16, 2026

Multiple field types on the list view have been updated to include keyboard navigation and other enhancements. 

Multi-, Single-select, and Assignee fields now offer keyboard navigation in the list view: 

* Use the up and down arrows on your keyboard to move through the list of people. 

* Press the space bar to select a person or to remove a selected person. 

On single and multi-select fields in the list view:  

* You can add new options directly from the editor when no results are found. Note that this feature may not be available on all lists. 

* The field interaction is now keyboard accessible. This includes navigation between the tags, search options, and list using the up and down arrows. Press the space bar to select an item or remove a selected item. 

Reference fields such as typeahead and external lookup fields, have received some interface enhancements. 

Also, where available, the experience of dragging and dropping columns has been improved visually. 

For more information, see [Manage the list view in Adobe Workfront Planning](/help/quicksilver/planning/views/manage-the-list-view.md). 

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

## Workfront reference fields are enabled as lookup fields for Planning connections

>[!NOTE]
>
>Preview: May 27, 2026 
>Production fast release: June 11, 2026  
>Production for everyone: July 16, 2026 

You can now add Workfront reference fields as lookup fields when connecting a Planning record type with a Workfront object type. 

For example, you can add the Portfolio, Program, Group or Company information from the Project object to a project connection field of a campaign in Planning.  

For information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md). 

## Edit submitted Planning requests

>[!NOTE]
>
>Preview: May 27, 2026 
>Production fast release: June 11, 2026 
>Production for everyone: July 16, 2026 

Users can now edit Planning requests after they submitted them. The following users can edit a submitted request: 

* The request creator 
* Workspace managers for the workspace where the request was submitted 
* System administrators 

For more information, see [Submit Adobe Workfront Planning requests to create records](/help/quicksilver/planning/requests/submit-requests.md). 

## Synchronize Metadata from Planning to AEM Content Fragments  

>[!NOTE]
>
>Preview: May 28 , 2026
>Production fast release: May 28, 2026
>Production for everyone: May 28, 2026
>[!BADGE Off schedule]{type=Neutral}

***************TO ADD MORE INFO AFTER TALKING WITH SYUZANNA**********

To improve data integrity, we've released seamless metadata synchronization between Planning record types in the GenStudio workspace and AEM Content Fragments when Content Fragments are linked to GenStudio campaigns.  

GenStudio campaign information now displays in the Metadata tab of a Content Fragment in AEM.  

With this release key metadata is consistent across both platforms and reflects updates in near real-time, reducing manual reconciliation. 

For information, see [Get Started with Adobe Workfront Planning and GenStudio for Performance Marketing integration](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md).  

## Synchronize Metadata from Planning to AEM Assets (title)
 
>[!NOTE]
>
>Preview: May 28 , 2026
>Production fast release: May 28, 2026
>Production for everyone: May 28, 2026
>[!BADGE Off schedule]{type=Neutral} 

To improve data integrity, we've released seamless metadata synchronization between  GenStudio record types and AEM Assets when AEM Assets are linked to GenStudio record types in Workfront Planning. The following GenStudio for Performance Marketing record types can be connected to AEM Assets: Campaign, Product, Persona, Region, and Channel. 

Information added to a GenStudio record type in Workfront Planning displays in a separate Campaign tab of an AEM Asset in AEM. 

For information, see [Get Started with Adobe Workfront Planning and GenStudio for Performance Marketing integration](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md).

## New filters for the timeline view breakdown feature 

>[!NOTE]
>
>Preview: May 27, 2026 
>Production fast release: June 11, 2026 
>Production for everyone: July 16, 2026 

You can now filter information in the timeline view based on criteria that match items included in the breakdown of the records.  

Prior to this enhancement, you could only apply filters for the main records in the timeline view. 

For information, see [Manage the timeline view](/help/quicksilver/planning/views/manage-the-timeline-view.md). 

## Grant permissions to records

***********CHECKING WITH LILIT ABOUT PREVIEW************ 

>[!NOTE]
>
>Preview: Not available
>Production fast release: May 28, 2026
>Production for everyone: May 28, 2026
>[!BADGE Off schedule]{type=Neutral}

You can now share individual records with users.  

By default, users inherit permissions from the workspace and the record type.  

You can give users the following permissions levels: 

* View 
* Manage 

>[!NOTE]
>
>* You cannot remove a user's permissions from a record at this time. If they have at least View permissions to the record type, they can view all the records of that type.  
>* Sharing records is not available in the Preview environment. It is only available in the Production environment.  

For information, see [Share records](/help/quicksilver/planning/access/share-records.md).

## New indication that edited and deleted fields impact request forms 

>[!NOTE]
>
>Preview: May 27, 2026 
>Production fast release: June 11, 2026 
>Production for everyone: July 16, 2026 

We have added a reminder that record fields that you edit or delete might impact request forms that contain those fields. Now, you will have a chance to review the affected forms and ensure the changes you want to make to the fields will not impact existing information.  

For information, see [Edit field settings](/help/quicksilver/planning/fields/edit-fields.md). 

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

<!--

API new version delayed till May 21, 2026

## Workfront Planning API version 2 

>[!NOTE]
>
>Available for all customers: May 28, 2026

Version 2 of Workfront Planning API is now available and it significantly expands the capabilities of Version 1.  

The following enhancements are included in Version 2: 

* Create, update, and delete workspaces, record types, and fields programmatically. 

* Fully manage records. 
* Improvements to URL structure, error handling, pagination, filtering, and permissions. 
* Includes partial updates via PATCH 
* Includes bulk record operations. 

Version 1 remains available, although we recommend that you switch to using Version 2.  

>[!NOTE]
>
>The Workfront Planning connector for Fusion has not been updated to API Version 2 and it will continue to use Version 1 until further notice.   

For information, see [Adobe Workfront Planning API basics](/help/quicksilver/planning/general/planning-api-basics.md).  

For Workfront Planning API specifications, see the [Workfront Planning API](https://developer.adobe.com/wf-planning/) developer documentation. 

-->



## 新的AEM內容片段預覽視窗

>[!NOTE]
>
>預覽： 2026年5月14日>生產快速發行： 2026年5月14日>適用於所有人的生產： 2026年5月14日>[!BADGE 不在排程]{type=Neutral}內

為了在使用連線到Workfront Planning記錄的AEM內容片段時提高可見度，我們新增了一個預覽視窗，顯示Workfront Planning中片段的相關資訊。

此功能先前可用於AEM資產，而我們現在已將其新增至內容片段。

如需詳細資訊，請參閱[連線記錄](/help/quicksilver/planning/records/connect-records.md)。

## Workfront Planning中現在提供AEM內容片段的查詢欄位

>[!NOTE]
>
>預覽： 2026年5月14日>生產快速發行： 2026年5月14日>適用於所有人的生產： 2026年5月14日>[!BADGE 不在排程]{type=Neutral}內

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
>預覽： 2026年5月14日>生產環境快速發行： 2026年6月11日>適用於所有人的生產： 2026年7月16日

為了在記錄的詳細資訊頁面中顯示您的資訊提供更好的彈性，我們引進了建立此頁面自訂檢視的功能。

除了新增兩個已建置的詳細資料頁面檢視（包含所有記錄欄位或僅表格檢視中顯示的欄位）之外，您現在可以為記錄的詳細資料頁面建立自訂檢視。 您建立的檢視對可以存取該記錄的所有人都可見。

此更新會移除&#x200B;**顯示所有欄位**&#x200B;設定，並以自訂詳細資料檢視取代它。

如需詳細資訊，請參閱[管理記錄頁面](/help/quicksilver/planning/records/manage-the-record-page.md)。

## 將群組新增至「連線的專案」記錄頁面

>[!NOTE]
>
>預覽： 2026年5月14日\
>生產快速： 2026年6月11日>適用於所有人的生產： 2026年7月16日

您現在可以在Workfront Planning中，將資訊分組到記錄的專案連線記錄頁面中。 在此增強功能之前，此功能不存在於此區域。

如需詳細資訊，請參閱[管理清單檢視](/help/quicksilver/planning/views/manage-the-list-view.md)。
