---
title: 開始使用Adobe Workfront Planning
description: Adobe Workfront Planning是Adobe Workfront的額外功能。 您可以建立可完全自訂的工作區，以定義符合企業內每個組織單位需求的工作流程。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: b1d6e0b3-e6d4-46d1-a6a2-4b8b73f7d3f7
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/EXDQUUA9-OKoA8Yj3de1TnanFEgXfKPvP8ksBGChiSI
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aadid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2: id: c3a155b4-a54b-4a82-a3d2-c8f0f971673eid: e147ce9d-7675-49bd-8a32-44f27d865560id: eb361af2-3e4f-4a79-b5f3-7a344ac5794cid: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: f8dfa5a4aec4541d885bcc45933488cd1fdefac4
workflow-type: tm+mt
source-wordcount: 1228
ht-degree: 0%

---

# 開始使用Adobe Workfront Planning

<!--

this article is linked to the WF Planning landing page - do not change URL or move it; send the team a new URL after we add the redirects for this page

-->

<!--do not use the snippet for IMPORTANT as it links to this article-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

>[!IMPORTANT]
>
>本文資訊為Adobe Workfront Planning。 Workfront Planning是獨立產品，或是另外購買的Adobe Workfront功能。
>
>
>本文包含客戶同時購買Workfront或Workflow套件時，有關Workfront Planning的一般資訊。
>
>如需包含Workfront Planning檔案的完整文章清單，請參閱[Adobe Workfront Planning的一般資訊和文章索引](/help/quicksilver/planning/planning-information.md)。
>
>如需Workfront Planning作為獨立產品的詳細資訊，請參閱[開始使用Adobe Workfront Planning作為獨立產品](/help/quicksilver/planning/planning-sta/planning-sta-overview.md)。


## Workfront規劃可用性

<!--
the bullets repeat in the "Access needed for Planning STA" article
-->

當您的組織購買下列其中一個Workfront套件時，即可存取Workfront計畫：

* Workfront Workflow和Workfront Planning一起購買。 組織中的每個使用者都有「工作流程」和「計畫」授權。 這可讓所有使用者完整存取這兩個模組的所有Workfront功能。

* 適用於組織中每個人的Workfront工作流程以及僅適用於組織中某些使用者的Workfront Planning。 這可讓使用者完整存取所有Workflow的功能，並為已指派Planning授權的使用者提供對Planning功能的更有限存取權。

* Workfront Planning可作為獨立產品，供貴組織使用者使用。 這讓使用者無法存取任何Workfront Workflow功能，也無法存取Planning功能。

如需以獨立產品形式包含在Planning中的功能相關資訊，請參閱[開始以獨立產品形式使用Adobe Workfront Planning ](/help/quicksilver/planning/planning-sta/planning-sta-overview.md)。

## Adobe Workfront規劃簡介

與工作流程授權一起購買時，Adobe Workfront Planning是Adobe Workfront的額外功能。 Workfront Planning的目的在於全面掌握組織的營運細節，並回答工作管理生命週期各階段的關鍵業務問題。

Workfront Planning可回答下列問題：

* 第4季我們在EMEA執行多少行銷活動？
* 並行行銷活動之間是否有任何對象重疊？
* 認識計畫目前表現如何？
  <!--* What do the assets look like for a particular campaign? Which of them must still be approved?-->

若要回答這些問題，領導力需要一個解決方案，針對從規劃到執行、從交付到結果衡量的每個工作階段，提供整體檢視。 目前，組織擁有可涵蓋程式某些部分的工具，但許多工具無法與所有工作階段建立良好的連線，也無法可靠地提供結果。

以下是部分主要功能：

* 解決跨所有階段以及參與工作流程的所有利害關係人管理工作的問題。
* 完全自訂您的工作流程，從決定您的組織使用哪些物件型別（或記錄型別），到設定這些物件如何彼此連結。
* 從其他系統連結到物件型別，為所有流程建立一致的架構。

## 為您的Workfront例項中的使用者啟用Workfront Planning

貴組織購買Workfront Planning套件後，身為Workfront管理員，您必須確定已具備下列專案，使用者才能存取Workfront Planning：

* 將包含Planning的版面配置範本指派給具有貢獻者或輕度存取層級的使用者。

  標準使用者和系統管理員預設啟用Planning。

  如需詳細資訊，請參閱[使用配置範本自訂主功能表](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)和[將使用者指派給配置範本](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)。

* 指派使用者Workfront與Planning授權以及Workfront Planning許可權，讓他們能夠在Workfront Planning中檢視或建立物件。

  如需授與存取權給其他人以及允許其他人使用Workfront Planning的詳細資訊，請參閱[Adobe Workfront Planning存取權概觀](/help/quicksilver/planning/access/access-overview.md)。

## Workfront規劃術語

雖然Workfront Planning是Workfront的一部分，但隨附專有概念和術語。 開始為組織設定Workfront規劃前，請務必熟悉這些概念。

Workfront Planning的架構可完全自訂。 您可以建立所有記錄型別、其屬性以及與其相關聯的任何欄位，以符合您組織的確切需求。

如需詳細資訊，請參閱[Workfront Planning術語概觀](/help/quicksilver/planning/general/planning-terminology.md)。

<!--the content from this section was moved to the article linked above-->

## 找到Adobe Workfront Planning

若要找到Adobe Planning，請確保貴組織已獲得Workfront Planning的存取權，且您的系統或群組管理員已將Planning區域新增至您的主功能表。 如需詳細資訊，請參閱[Adobe Planning存取總覽](/help/quicksilver/planning/access/access-overview.md)。

若要找到Workfront Planning：

1. 登入Workfront。

{{step1-click-main-menu-shell-only}}

1. 按一下&#x200B;**計畫** ![計畫圖示](assets/planning-icon.png)。

   Workfront Planning首頁面隨即開啟。

   ![規劃登陸頁面管理員](assets/planning-landing-page-admin.png)

   >[!TIP]
   >
   >    您的Workfront管理員可以將「規劃」區域新增至版面配置範本中的「選取登陸頁面」選項，以便您登入Workfront後立即開啟「規劃」。 如需詳細資訊，請參閱[使用版面配置範本自訂登入頁面](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)。

1. （條件式與選用式）如果您是Workfront管理員，請按一下下列其中一個標籤：
   * **我所在的工作區**：顯示您建立的工作區或與您共用的工作區。
   * **其他工作區**：顯示系統中的所有其他工作區。

   對於所有其他使用者，他們建立或與他們共用的工作區都會顯示在&#x200B;**工作區**&#x200B;區域中。

1. （選用且建議使用）繼續下列部分動作，以建置您的工作結構：

   1. 從頭開始或使用範本建立工作區。 如需詳細資訊，請參閱[建立工作區](/help/quicksilver/planning/architecture/create-workspaces.md)。

   1. 新增區段至新工作區。 如需詳細資訊，請參閱[編輯工作區](/help/quicksilver/planning/architecture/edit-workspaces.md)。
   1. 重新命名新工作區中的現有區段。
   1. 將記錄型別新增至新工作區。 如需詳細資訊，請參閱[建立記錄型別](/help/quicksilver/planning/architecture/create-record-types.md)。

   1. 按一下記錄型別的名稱以開啟記錄型別的頁面。 記錄型別頁面預設會在「表格」檢視中開啟。

      您也可以建立時間表或行事曆檢視。 如需詳細資訊，請參閱[管理記錄檢視](/help/quicksilver/planning/views/manage-record-views.md)。

   1. 在表格檢視中，新增列以開始新增記錄

      或

      透過新增欄開始新增記錄欄位。

      如需詳細資訊，請參閱下列文章：

      * [建立記錄](/help/quicksilver/planning/records/create-records.md)
      * [建立欄位](/help/quicksilver/planning/fields/create-fields.md)。

## Workfront Planning的其他資源

* [Adobe Workfront Planning的一般資訊和文章索引](/help/quicksilver/planning/planning-information.md)：包含有關Workfront Planning檔案的所有文章索引，依興趣區域分組。
* [以獨立產品形式開始使用Adobe Workfront Planning](/help/quicksilver/planning/planning-sta/planning-sta-overview.md)：以獨立產品形式購買時，提供Workfront Planning的一般資訊。
* [Adobe Workfront Planning AI Assistant總覽](/help/quicksilver/planning/general/planning-ai-assistant-overview.md)：使用Workfront AI Assistant for Planning，您可以使用命令來搜尋記錄，或建立、更新和刪除記錄，並讓助理為您工作。

  <!--
    >[!NOTE]
    >
    >The Workfront AI Assistant has been temporarily removed and it will be available at a later date.
    -->

* [適用於Workfront Fusion的Adobe Workfront規劃模組](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-planning-modules)：透過Adobe Workfront規劃模組，您可以在Workfront規劃中發生事件時觸發情境。 您也可以建立、讀取、更新及刪除記錄，或對Adobe Workfront Planning帳戶執行自訂API呼叫。 您必須購買額外的授權才能存取Workfront Fusion。

* [Adobe Workfront Planning API基本知識](/help/quicksilver/planning/general/planning-api-basics.md)： Adobe Workfront Planning API的目標是透過引入透過HTTP運作的REST-ful架構，簡化與Planning的整合建置。

* [開始使用Adobe Workfront Planning與Adobe GenStudio for Performance Marketing整合](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md)：您可以在Workfront Planning的GenStudio for Performance Marketing工作區中管理GenStudio的記錄。 您必須購買GenStudio for Performance Marketing授權。

* [畫布儀表板總覽](/help/quicksilver/reports-and-dashboards/canvas-dashboards/canvas-dashboards-overview.md)：您可以使用Workfront Canvas Dashboard，在Workfront的報表中檢視Workfront Planning資訊。 您必須購買Workfront工作流程授權才能存取畫布控制面板。


<!--
## Currently available Workfront Planning features
(*****for GA just make a list of what features ARE included in Planning and eliminate the last 2 columns; also update the title of this section*****)

(*****at GA: update the link below to the new place for release notes *****)

For information about new features and when they are released, see [Adobe Workfront Planning release activity for 2024](/help/quicksilver/planning/general/release-activity.md). 

The following features are currently available in Workfront Planning:

* Create workspaces             
* Create record types             
* Create record custom fields             
(************ * Import record types and fields using an Excel or CSV file*****)
          
* Display records in a table view            
* Display records in a timeline view            
* Display records in a calendar view            
* Filter, sort, and group records in a table view
* Filter, group, and color code records in the timeline view
* Filter records in the calendar view 
* Search for records in the table and timeline views             
* Connect records that belong to the same workspace  
* Connect records that belong to different workspaces   
* Connect Workfront Planning records to Workfront projects, programs, portfolios, companies, groups             
* Connect Workfront Planning records to Adobe Experience Manager assets          
    You must have an Adobe Experience Manager Assets license and an integration between AEM Assets and Workfront.
    For information, see [Adobe Workfront for Experience Manager Assets and Assets Essentials: article index](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md). 
* View record information in the Details tab
* View record connections in the Connections tab
* Customize the layout of a record's page             
* Share workspaces             
* Share views             
* Share views publicly with any external resource, even people who are not Workfront users         
* Duplicate views             
* Submit requests to create records            
* Export record details to Word and PDF.
* Add comments to records             
* Receive in-app notifications             
* Receive email notifications             
* Add thumbnails and cover pages to records             
* View the history of changes on a record             
* Rich Text formatting for Paragraph fields             
* Access Planning records from Workfront objects             
* Connect and disconnect Planning records from Workfront objects 
* Create Planning records by submitting a request form            
* Workfront Planning public API             
* Adobe Workfront Planning modules for Adobe Workfront Fusion             
* Workfront Planning AI Assistant
* Reporting on Workfront Planning information
    You can report on Planning information using the Canvas Dashboard. For information, see [Canvas Dashboards overview](/help/quicksilver/reports-and-dashboards/canvas-dashboards/canvas-dashboards-overview.md). 

-->

<!--
<table style="table-layout:auto"> 

|       Feature                                      |     Available now  |     Coming soon   |     In research  |
|----------------------------------------------------|:-----------------------------:|:--------------------------------:|:----------------:|
|     Create workspaces                              |   ✓                           |                                  |                  |
|     Create record types                |   ✓                           |                                  |                  |
|     Create record custom fields                    |   ✓                           |                                  |                  |
|     Import record types and fields using an Excel  or CSV file                              |                              |           ✓                       |                  |
|     Link records                                   |   ✓                           |                                  |                  |
|     View records in a table                        |   ✓                           |                                  |                  |
|     View records in a timeline                     |   ✓                           |                                  |                  |
|     View records in a calendar                     |   ✓                           |                                  |                  |
|     Filter records                                 |   ✓                           |                                  |                  |
|     Group records in the timeline view             |   ✓                           |                                  |                  |
|     Group records in the table view                | ✓                              |                                 |                  |
|     Sort records in the table view                                 |  ✓                             |                                 |                  |
|     Sort records in the timeline view                                 |                               |   ✓                              |                  |
|     Sort groupings in the table view                                 |                               |   ✓                              |                  |
|     Sort groupings in the timeline view                                 |                               |   ✓                              |                  |
|   Search for records in the table view    | ✓    |   |
|   Search for records in the timeline view    | ✓    |   |
|     Connect Workfront Planning records to Workfront projects, programs, portfolios, companies, groups  |   ✓                            |                                 |                  |
|     Connect Workfront Planning records to Adobe Experience Manager assets                                  |      ✓                         |                                  |                 |
|     Connect Planning records from different workspaces                                  |      ✓                         |                                  |                 |
|     Record page with detailed information                            |   ✓                           |                                  |                  |
|     Update the layout of the record's page              |    ✓                           |                                 |                  |
|  Share workspaces | ✓| |  |
|  Share views |✓ | |  |
|  Share views publicly with external resources |✓ | |  |
|  Duplicate views |✓ | |  |
|     Submit requests                                |                               |          ✓                        |                 |
|     Export record details to Word                                 |    ✓                           |                                  |                 |
|     Export record details to PDF                                 |                               |                                  |       ✓          |
|     Customize the color and icon of a record                                 |      ✓                         |                                  |                 |
|     Add comments to records                                 | ✓                              |                                  |                 |
|     Receive in-app notifications                                 | ✓                              |                                  |                 |
|     Receive email notifications                                 | ✓                              |                                  |                 |
|     Add thumbnails to records                                 | ✓                              |                                  |                 |
|     View history of changes on a record                                 | ✓                              |                                  |                 |
|     Rich Text formatting for Paragraph fields                                 |      ✓                         |                                  |                 |
|     Adobe Workfront Planning modules for Adobe Workfront Fusion                                 |      ✓                         |                                  |                 |
|     Copy and paste information from one field to another                                  |      ✓                         |                                  |                 |
|     Access Planning records from Workfront objects                                  |      ✓                         |                                  |                 |
|     Connect Planning records from Workfront objects                                  |      ✓                         |                                  |                 |
|     Workfront Planning public API                                 |      ✓                         |                                  |                 |
|     Workfront Planning AI Assistant*                                 |      ✓                         |                                  |                 |
|     Reporting on Workfront Planning information (Canvas Dashboard)                              |                               |       ✓                           |                 |
</table>

-->