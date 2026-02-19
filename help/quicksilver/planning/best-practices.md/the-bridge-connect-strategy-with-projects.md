---
title: 建立Bridge：將策略意圖連結至專案
description: 瞭解如何在Adobe Workfront規劃中的高階計畫與Adobe Workfront中工作流程的日常執行之間建立「策略對話串」。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 567ab223-b282-4b98-9655-7b9766fba869
source-git-commit: 7f3ca12d89a2a5fbebc12b3df8a40edbb17d0ead
workflow-type: tm+mt
source-wordcount: '1156'
ht-degree: 0%

---


# 建置橋樑：將策略意圖連結至專案

>[!IMPORTANT]
>
>本文資訊說明Adobe Workfront的額外功能Adobe Workfront Planning。
>
>貴組織必須有Workfront Planning Prime或更新版本的套件，才能支援本文建議的功能。
>
>如需存取Workfront Planning的需求清單，請參閱[Adobe Workfront Planning存取總覽](/help/quicksilver/planning/access/access-overview.md)。
> 
>如需Workfront Planning的一般資訊，請參閱[開始使用Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md)。

瞭解如何在Adobe Workfront Planning中的高層級計畫與Workfront中的日常執行之間建立策略對話串。 您可以使用連線，在策略和執行之間架設橋樑。

本指南適用於實作Workfront Planning的Workfront管理員和工作區管理員。

## 策略與執行協調的概觀

將您的策略與日常工作連線起來，將願景變為現實。 當高階計畫與執行同步時，您會建立策略執行緒，確保每個專案和任務都會推動業務向前發展。

要達到這種一致性，需要一組技術連結和流程護欄，將Workfront中的工作與Workfront Planning中的策略記錄連線起來。

透過縮短計畫與行動之間的差距，您可以確保團隊的精力永遠聚焦於您最高優先順序的目標。

## 透過建立連線來建立基礎

您必須先定義哪些記錄型別符合連線的條件，才能在規劃與執行之間建立橋樑。

### 連線欄位概觀

橋接器從建立連線欄位開始。

連線欄位可作為記錄型別之間的技術交握。

此欄位型別是Workfront Planning中所有關係背後的引擎。 這是意圖的表示法，其可建立特定記錄型別（例如通道策略）可連結至其他物件型別(無論這些物件型別位於Planning或Workfront)。

如需詳細資訊，請參閱[連線記錄型別概觀](/help/quicksilver/planning/architecture/connect-record-types-overview.md)。

### 定義建立連線的時間

理想情況下，您必須先決定是否需要建立連線，才能建立任何工作。

透過新增連線欄位，您正在架構您的環境以支援策略對話串，無論最終如何建立個別記錄。

## 同步設定策略與執行

為了讓您專注於策略層，我們建議將您的規劃記錄聚焦於高階意圖，同時使用Workfront進行戰術執行。

此方法以下列方式運用這兩個模組的獨特優勢：

* **Workfront規劃（策略層）：**&#x200B;保持高階。 它會追蹤促銷活動、頻道策略和預算。 無雜訊，適合主管使用。

* **Workfront （執行層）：**&#x200B;管理戰術細節。 您可以將個別體驗或活動當成專案、任務和問題來管理。 您可以指派他們以取得所有權，並建立核准以執行。

## 透過啟用橋接器，從意圖移至行動

設定連線後，您必須決定如何啟用特定策略記錄與執行專案之間的連結。

### 使用表格導向路徑

策略師和進階使用者通常使用表格檢視作為其工作台，以隨著時間推移調整計畫。

依預設，在表格中建立記錄不會建立指向Workfront的連結。

當使用者決定啟動連結時，會建立與執行專案的連線。

您可以透過下列方式完成這項操作：

* 直接從Workfront Planning中的連線欄位或記錄詳細資料檢視中的選用連線頁面，手動建立下游連線專案。

  手動建立會導致空白專案沒有特定自訂表單。

  如需詳細資訊，請參閱[連線記錄](/help/quicksilver/planning/records/connect-records.md)。

* 使用Workfront Planning自動化，自動滿足更複雜的需求。

  當您選取表格中的列時，這些自動設定會以動作列中的按鈕形式提供。

  這允許人為監督或建立預留位置，確保專案僅在真正需要時才在您的工作流程環境中產生。

  如需詳細資訊，請參閱[使用Adobe Workfront Planning記錄自動化建立物件](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md)


### 建立自動化啟用

對於具有大量請求或進階自動化需求的組織，可以根據特定事件或根據請求表單中設定的欄位值自動啟用橋接器。

此方法需要Adobe Workfront Fusion的授權。

如需詳細資訊，請參閱[設定和管理Workfront Fusion：文章索引](https://experienceleague.adobe.com/zh-hant/docs/workfront-fusion/using/set-up-and-manage-fusion/set-up-and-manage-workfront-fusion-toc)。

* **使用提交觸發程式：**&#x200B;由於表單提供單一、乾淨的提交事件，因此可將其用作Fusion自動化的觸發程式。 Fusion案例可以偵測表單提交，並立即在Workfront中產生連結專案。

* **使用欄位值觸發程式：**&#x200B;若要進行更深入的自動化，您可以設定Fusion來監視特定欄位。 例如，標示為「已準備好執行」的簡單核取方塊可作為催化劑，在檢查橋接器時自動建立橋接器。

## 新增查閱欄位以取得曲面可見度

連結專案後，您可以直接從專案新增查詢欄位，在Planning記錄中呈現來自Workfront的即時資料。

身為工作區管理員，您可以設定查詢欄位，將任何系統或自訂欄位從連結的專案(例如實際完成日期或Creative銷售機會)提取到Planning記錄型別中。 擷取資料後，您可在策略階層的多個層級中向上彙整這些資料，一直到促銷活動層級。 這可為整個行銷生命週期的利害關係人提供強大的彙總報告，無需離開規劃環境即可隨時瞭解情況。

## 將策略與行動連結起來，達到可見度

Bridge的終極價值是即時可見度。

藉由將意圖與行動連結，您一眼就能回答重要的業務問題。 以下是這些問題的範例：

* 我們的「FY26品牌認知度」行銷活動目前是否主動提供成果？

* 我們的策略策略策略在哪些方面需要更多創意支援才能與時俱進？

* 我們如何根據最高優先順序的戰略支柱來調整資源？

## 最佳作法和秘訣

### 待辦事項：

* **使用「策略對話串」的比喻：**&#x200B;提醒團隊，每個專案都應該是策略字串上的「珠子」。

* **自動切換：**&#x200B;使用自動觸發專案建立，以節省時間和精力，同時改善資料連線能力與控管。

* **連結，不要複製：**&#x200B;使用查詢欄位在您的策略記錄中顯示即時執行資料（如狀態或完成日期）。 這可確保您的策略檢視始終正確，而不需要團隊手動更新。

### 不要：

* **請勿將計畫記錄視為工作清單：**&#x200B;橋接器是用來連線策略意圖與執行專案。 讓您的規劃記錄聚焦於「什麼」和「為什麼」，並讓工作流程模組處理精細的「如何」完成任務和問題。

* **不要過度同步：**&#x200B;您不需要將每個專案層級的詳細資料同步回Planning。 保持策略層的高階與無雜訊。

* **請勿略過橋接器：**&#x200B;如果工作開始於「工作流程」模組，但沒有Planning的連結，則表示您已建立領導無法看到的「陰影計畫」。

<!--original content:

# The Bridge: Connecting Strategic Intent to Projects 

 

## Goal 

Learn how to create a "strategic thread" between your high-level plans in Workfront Planning and your daily execution in the Workflow module. 

 

## Overview 

Connecting your strategy to your daily work turns vision into reality. When high-level plans are in sync with execution, you create a **strategic thread** that ensures every project and task moves the business forward. 

 

Achieving this alignment requires a set of technical links and process guardrails that connect efforts in the **Workflow module** with strategic records in **Workfront Planning (WFP)**. By bridging the gap between planning and action, you ensure that your team's energy is always focused on your highest-priority goals. 

 

## The foundation: Establishing the connection 

Before you can bridge planning and execution, a workspace manager must define which record types are eligible for a connection. 

 

### The connection field: The technical handshake 

The bridge begins with a **connection field**. This field type is the engine behind all relationships in WFP. It is an expression of intent, in that it establishes that a specific record type (like a *channel tactic*) is allowed to be linked to other objects, whether they live in the workflow module or within planning itself. 

 

### Deciding to connect 

Establishing this allowance is a configuration-level decision that typically happens before any work is created. By adding a connection field, you are architecting your environment to support a "strategic thread," regardless of how the individual records are eventually created. 

 

## Strategy and execution in sync 

To keep your strategic layer focused, we recommend focusing your planning records on high-level intent while using the Workflow module for tactical execution. This approach uses the unique strengths of both modules: 

 

*   **Workfront Planning (The strategic layer):** Stays high-level. It tracks the *Campaign*, the *Channel Tactic*, and the *Budget*. It is noise-free and executive-ready. 

*   **Workflow module (The execution layer):** Manages the tactical details. Individual "Experiences" or "Activities" are managed here as **projects, tasks, and issues**. 

 

## Activating the bridge: From intent to action 

Once the connection is configured, you must decide how to activate the link between a specific strategic record and an execution project. 

 

### Professional triage: The table-led path 

Strategists and power users often use the **table view** as their "workbench" to refine plans over time.  

*   **Deliberate handoff:** By default, creating a record in a table does not establish a link to the Workflow module. The connection to an execution project is established when a user decides to activate the link. This can be done by manually creating a downstream connected project directly from the connection field in WFP or an optional **connection view page** in the record's detail view. Note that manual creation results in a blank project without specific custom forms; for more complex needs, you can use a **native WFP automation**. These automations are available when you select a row in a table, appearing as buttons in the blue action bar at the bottom of your screen. This allows for human oversight or placeholder creation, ensuring that projects are only generated in your workflow environment when they are truly needed. 

 

### Automated activation 

For organizations with high-volume requests or advanced automation needs, the bridge can be activated automatically based on specific events or field values. 

*   **Submission triggers:** Because forms provide a single, clean "submission event," they can be used as triggers for **Fusion automations**. A scenario can detect a form submission and immediately generate a linked project in the workflow module. 

*   **Field-value triggers:** For deeper automation, you can configure **Fusion** to monitor specific fields. For example, a simple checkbox labeled "ready for execution" can serve as the catalyst, establishing the bridge automatically the moment it is checked. 

 

## Surfacing visibility: Lookup fields 

Once a project is linked, you can surface real-time data from the Workflow module directly within the WFP record. 

 

A workspace manager can set up **lookup fields** to pull any native or custom field from the linked project (such as *actual completion date* or *creative lead*) into the WFP record type. Once captured, this data can be rolled up through multiple levels of your strategic hierarchy—even all the way to the campaign level. This provides powerful aggregate reporting for stakeholders across the entire marketing lifecycle, keeping them informed without needing to leave the planning environment. 

 

## Strategy-to-action visibility 

The ultimate value of the bridge is **real-time visibility**. By connecting intent to action, you can answer critical business questions at a glance: 

 

*   "Is our 'FY26 Brand Awareness' campaign actively delivering results right now?" 

*   "Where do our strategic tactics need more creative support to stay on schedule?" 

*   "How are we aligning our resources with our highest-priority strategic pillars?" 

 

## Best practices & tips 

 

### Do: 

*   **Use the "strategic thread" metaphor.** Remind teams that every project should be a "bead" on a strategic string. 

*   **Automate the handoff.** Use automations to trigger project creation to save time and effort while also improving data connectivity and governance. 

*   **Link, don't duplicate.** Use lookup fields to surface real-time execution data (like status or completion dates) in your strategic records. This ensures your strategic views are always accurate without requiring manual updates from your team. 

 

### Don't: 

*   **Don't treat planning records as task lists.** The bridge is designed to connect strategic intent to execution projects. Keep your planning records focused on the "what" and "why," and let the workflow module handle the granular "how" through tasks and issues. 

*   **Don't over-sync.** You don't need to sync every project-level detail back to Planning. Keep the strategic layer high-level and noise-free. 

*   **Don't bypass the bridge.** If work starts in the Workflow module without a link to Planning, you've created a "Shadow Plan" that is invisible to leadership. 

-->



