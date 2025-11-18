---
title: 開始使用Adobe Workfront Planning
description: Adobe Workfront Planning是Adobe Workfront的額外功能。 您可以建立可完全自訂的工作區，以定義符合企業內每個組織單位需求的工作流程。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: b1d6e0b3-e6d4-46d1-a6a2-4b8b73f7d3f7
source-git-commit: 96028446d76f32daf512adf77d3b1c53021821ec
workflow-type: tm+mt
source-wordcount: '2046'
ht-degree: 1%

---

# 開始使用Adobe Workfront Planning

<!--this article is linked to the WF Planning landing page - do not change URL or move it; send the team a new URL after we add the redirects for this page-->

<!--do not use the snippet for IMPORTANT as it links to this article-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span> -->

>[!IMPORTANT]
>
>本文資訊說明Adobe Workfront的額外功能Adobe Workfront Planning。
>
>您必須具備下列專案，才能完整存取Workfront Planning中的所有功能：
>
>* 新的Workfront套件和授權。 Workfront計畫不適用於舊版Workfront套件或授權。
>* Workfront計畫套件。
>* 貴組織的Workfront執行個體必須上線至Adobe統一體驗。
>
> 如需存取Workfront Planning的完整需求清單，請參閱[Adobe Planning存取總覽](/help/quicksilver/planning/access/access-overview.md)。
> 

本文包含有關Workfront Planning的一般資訊。

如需包含Workfront Planning檔案的完整文章清單，請參閱[Adobe Workfront Planning的一般資訊](/help/quicksilver/planning/planning-information.md)。

## Adobe Workfront規劃簡介

Adobe Workfront Planning是Adobe Workfront的額外功能。 Workfront Planning的目的在於全面掌握組織的營運細節，並回答工作管理生命週期各階段的關鍵業務問題。

Workfront Planning可回答下列問題：

* 第4季我們在EMEA執行多少行銷活動？
* 並行行銷活動之間是否有任何對象重疊？
* 認識計畫目前表現如何？
* 特定行銷活動的資產看起來如何？ 其中哪些仍須核准？

若要回答這些問題，領導力需要一個解決方案，針對從規劃到執行、從交付到結果衡量的每個工作階段，提供整體檢視。 目前，組織擁有可涵蓋程式某些部分的工具，但許多工具無法與所有工作階段建立良好的連線，也無法可靠地提供結果。

以下是部分主要功能：

* 解決跨所有階段以及參與工作流程的所有利害關係人管理工作的問題。
* 完全自訂您的工作流程，從決定您的組織使用哪些物件型別（或記錄型別），到設定這些物件如何彼此連結。
* 從其他系統連結到物件型別，為所有流程建立一致的架構。

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

<!--OLD: 

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
-->

## 為您的Workfront例項中的使用者啟用Workfront Planning

貴組織購買Workfront Planning套件後，身為Workfront管理員，您必須確定已具備下列專案，使用者才能存取Workfront Planning：

* 在主要功能表中指派包含Planning的版面配置範本，給下列使用者：

   * 將版面配置範本指派給Light和Contribute使用者。

     標準使用者和系統管理員預設啟用Planning。

  如需詳細資訊，請參閱[使用配置範本自訂主功能表](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)和[將使用者指派給配置範本](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)。

* 為使用者指派Workfront授權和Workfront Planning許可權，讓他們能夠在Workfront Planning中檢視或建立物件。 如需授與存取權給其他人以及允許其他人使用Workfront Planning的詳細資訊，請參閱[Adobe Workfront Planning存取權概觀](/help/quicksilver/planning/access/access-overview.md)。

## Workfront規劃術語

雖然Workfront Planning是Workfront的一部分，但隨附專有概念和術語。 開始為組織設定Workfront規劃前，請務必熟悉這些概念。

Workfront Planning的架構可完全自訂。 您可以建立所有記錄型別、其屬性以及與其相關聯的任何欄位，以符合您組織的確切需求。

您可以建立的Workfront Planning物件數目存在限制。 如需詳細資訊，請參閱[Adobe Workfront Planning物件限制總覽](/help/quicksilver/planning/general/limitations-overview.md)。

以下是主要的Workfront Planning物件和概念：

* **Workspace**：定義特定組織作業生命週期的記錄型別集合。 工作區是組織單位的工作框架。

  ![具有記錄型別分類的行銷工作區開啟頁面](assets/marketing-workspace-with-record-type-taxonomies-opening-page.png)

  如需詳細資訊，請參閱[建立工作區](/help/quicksilver/planning/architecture/create-workspaces.md)。

* **記錄型別**： Workfront Planning中的物件型別名稱。

  記錄型別會填入工作區。

  與Workfront （預先定義物件型別）不同，您可以在Workfront Planning中建立自己的物件型別。

  例如，在Workfront中，已建立方案、Portfolio、專案、任務或問題的物件型別。

  在Workfront Planning中，您可以建立符合組織工作流程的任何記錄型別。 稍後，您可以定義記錄型別如何相互關聯或表單相依性。

  如需詳細資訊，請參閱[記錄型別概觀](/help/quicksilver/planning/architecture/overview-of-record-types.md)。

* **記錄**：記錄型別的執行個體。

  ![行銷活動記錄型別清單中反白的記錄](assets/records-highlighted-in-campaign-record-type-list.png)

  將記錄型別新增至工作區後，您就可以開始在記錄型別的頁面上新增該型別的記錄。

  例如，「Campaign」可以是記錄型別，「Summer Campaign for EMEA」是Campaign記錄型別的記錄。

  如需詳細資訊，請參閱[建立記錄](/help/quicksilver/planning/records/create-records.md)。

* **Workspace範本**：您可以使用預先定義的範本建立工作區。 您可以使用範本中預先定義的記錄型別和欄位，也可以新增您自己的記錄型別和欄位。

  ![含有範本縮圖的工作區頁面](assets/workspaces-page-with-templates-thumbnails.png)

  Adobe Workfront Planning包含下列範本：

   * 基本：行銷管理
   * 進階：行銷管理
   * 企業：行銷管理
   * 銷售管理
   * 產品管理

  如需詳細資訊，請參閱[工作區範本清單](/help/quicksilver/planning/architecture/workspace-templates.md)。

* **欄位**：欄位是您可以新增到記錄型別的屬性。 欄位包含有關記錄型別的資訊。<!--check the shot below, "Connection" needs to be in lowercase-->

  ![記錄欄位的下拉式清單](assets/drop-down-list-of-record-fields.png)

  有關記錄欄位的考量事項：

   * 您為記錄型別新增的欄位會自動與該型別的所有記錄相關聯，並可用於擷取有關這些記錄的資料。

   * 在套用至記錄型別頁面的「表格」檢視中，欄位會顯示為欄。 它們也會顯示在紀錄的頁面中。

   * 欄位對記錄型別是唯一的，不會從一種記錄型別轉移到另一種記錄型別。

   * 欄位可完全自訂，僅可在Workfront Planning中存取。 您無法從Workfront存取Workfront規劃欄位。

  如需詳細資訊，請參閱[建立欄位](/help/quicksilver/planning/fields/create-fields.md)。

  依預設，新的記錄型別與下列預先定義的欄位相關聯：

   * 名稱
   * 說明
   * 開始日期
   * 結束日期
   * 狀態

  您可以建立下列型別的自訂欄位：

   * 單行文字
   * 段落
   * 多選
   * 單選
   * 日期
   * 數字
   * 百分比
   * 貨幣
   * 核取方塊
   * 公式
   * 人員
   * 建立者
   * 建立日期
   * 上次修改者
   * 上次修改日期

* **連線的記錄型別**、**連線的記錄**&#x200B;和&#x200B;**連線的欄位**：您可以在Workfront Planning中的下列實體之間建立連線：

   * 兩種Workfront Planning記錄型別。
   * 記錄型別和Workfront專案、方案、投資組合、公司或群組物件型別。
   * 記錄型別和Adobe Experience Manager資產或資料夾。

     您必須擁有Adobe Experience Manager授權，才能將記錄型別與Experience Manager物件連線。

     ![使用Workfront AEM選項的新連線標籤](assets/new-connection-tab-with-workfront-aem-options.png)

   * 記錄型別和Adobe GenStudio for Performance Marketing品牌。

     您必須擁有Adobe GenStudio for Performance Marketing授權，才能將記錄型別與GenStudio品牌連線。

     ![使用Adobe GenStudio Brand選項的新連線標籤](assets/new-connection-tab-with-genstudio-option.png)


  在記錄型別之間建立連線之後，可以將這些型別的個別記錄或物件彼此連線。 記錄之間的連線會顯示為已連線的記錄欄位或連線。

  當有數種工作物件型別影響彼此時，連線記錄型別會很有幫助。 例如，您可以使用行銷活動，而每個行銷活動可能會迎合多個品牌。 若要指出此關係，您可以將行銷活動連結至品牌。 此外，每個行銷活動的工作可能會在Workfront的多個專案中進行規劃。 若要指出此問題，您可以將行銷活動連結至相關專案。 連線記錄型別，然後連線個別記錄，可在Workfront Planning中達成此關係。

* **查詢欄位** （或連結欄位）：當您建立兩個記錄型別之間的連線，並將個別記錄連線在一起後，就可以參照您正在連線的記錄中連線記錄的欄位。

  例如，如果您將Campaign記錄型別與Workfront專案物件型別連線，則可以在行銷活動記錄上顯示已連線專案的「預算」欄位。

  ![新增查閱欄位方塊](assets/add-lookup-fields-modal.png)

  >[!TIP]
  >
  > 您無法從連線的記錄或物件型別將下列欄位型別新增為查閱欄位：
  >
  >* 人員
  >* 建立者
  >* 上次修改者
  >* Workfront預先輸入欄位（包括專案所有者或專案贊助者等欄位）

  如需有關連線記錄型別、記錄和建立連結欄位的資訊，請參閱下列文章：

   * [連線記錄型別](/help/quicksilver/planning/architecture/connect-record-types.md)
   * [連接記錄](/help/quicksilver/planning/records/connect-records.md)

<!--not yet:* Fields are reusable across Record Types.  -->

* **檢視**：記錄會顯示在不同檢視型別的個別記錄型別頁面下。

  ![記錄型別清單中的檢視型別下拉式清單](assets/view-types-drop-down-from-record-type-list.png)

  檢視包含特定檢視型別的個人化設定，例如欄位清單（欄）、記錄清單（列）、其順序（排序）、套用或適用的篩選以及分組。

  以下是您可以套用至記錄型別頁面的檢視型別：

   * **資料表檢視**：以資料表格式顯示記錄及其欄位，包括連線和查詢欄位。 表格的列是個別記錄，欄是記錄欄位。 表格檢視是預設的檢視。

     ![資料表檢視範例](assets/table-view-example.png)

   * **時間表檢視**：在時間軸中顯示至少有兩個日期型別欄位的記錄。 您最多可以在時間軸檢視中顯示5個連線的記錄型別及其記錄。

     ![在時間表檢視中套用的群組](assets/grouping-applied-in-timeline-view.png)

   * **行事曆檢視**：以行事曆格式顯示至少有兩個日期型別欄位的記錄。
     ![行事曆檢視範例](assets/calendar-view-example.png)


如需詳細資訊，請參閱[管理記錄檢視](/help/quicksilver/planning/views/manage-record-views.md)。

## 找到Adobe Workfront Planning

若要找到Adobe Planning，請確保貴組織已獲得Workfront Planning的存取權，且您的系統或群組管理員已將Planning區域新增至您的主功能表。 如需詳細資訊，請參閱[Adobe Planning存取總覽](/help/quicksilver/planning/access/access-overview.md)。

若要找到Workfront Planning：

1. 登入Workfront。

{{step1-click-main-menu}}

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

## Workfront Planning發行活動

<!--update this with the new release activity page - the article index for all Planning releases-->

我們會定期為Workfront Planning發佈新功能。

如需已發行功能的最新清單，請參閱[Adobe Workfront Planning發行活動：文章索引](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md)。

## Workfront Planning的其他資源

* [Adobe Workfront Planning的一般資訊](/help/quicksilver/planning/planning-information.md)：包含有關Workfront Planning檔案的所有文章的索引，依興趣區域分組。
* [Adobe Workfront Planning AI Assistant總覽](/help/quicksilver/planning/general/planning-ai-assistant-overview.md)：使用Workfront AI Assistant for Planning，您可以使用命令來搜尋記錄，或建立、更新和刪除記錄，並讓助理為您工作。

  <!--
    >[!NOTE]
    >
    >    The Workfront AI Assistant has been temporarily removed and it will be available at a later date.-->

* [適用於Workfront Fusion的Adobe Workfront規劃模組](https://experienceleague.adobe.com/zh-hant/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-planning-modules)：透過Adobe Workfront規劃模組，您可以在Workfront規劃中發生事件時觸發情境。 您也可以建立、讀取、更新及刪除記錄，或對Adobe Workfront Planning帳戶執行自訂API呼叫。

* [Adobe Workfront Planning API基本知識](/help/quicksilver/planning/general/planning-api-basics.md)： Adobe Workfront Planning API的目標是透過引入透過HTTP運作的REST-ful架構，簡化與Planning的整合建置。

* [開始使用Adobe Workfront Planning與Adobe GenStudio for Performance Marketing整合](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md)：您可以在Workfront Planning的GenStudio for Performance Marketing工作區中管理GenStudio的記錄。

* **Workfront Planning報告功能**：您現在可以使用Workfront Canvas Dashboard，在Workfront的報告中檢視Workfront Planning資訊。 如需詳細資訊，請參閱[畫布儀表板概觀](/help/quicksilver/reports-and-dashboards/canvas-dashboards/canvas-dashboards-overview.md)。

