---
title: 架構您的成功：模型化您的行銷活動階層
description: 瞭解如何使用「重心」和多工作區架構，將複雜的業務流程轉換為可擴充、受管理的行銷活動階層。
feature: Workfront Planning
role: Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 02e3b55f-9188-42bf-8d0b-c9fed86c63c4
source-git-commit: 7f3ca12d89a2a5fbebc12b3df8a40edbb17d0ead
workflow-type: tm+mt
source-wordcount: '1537'
ht-degree: 0%

---

# 架構您的成功：模型化您的行銷活動階層

<!--see the file again for additional comments from Seth and others-->

>[!IMPORTANT]
>
>本文資訊說明Adobe Workfront的額外功能Adobe Workfront Planning。
>
>貴組織必須有Workfront Planning Prime或更新版本的套件，才能支援本文建議的功能。
>
>如需存取Workfront Planning的需求清單，請參閱[Adobe Workfront Planning存取總覽](/help/quicksilver/planning/access/access-overview.md)。
> 
>如需Workfront Planning的一般資訊，請參閱[開始使用Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md)。

瞭解如何在Adobe Workfront Planning中使用重心和多工作區架構，將複雜的業務流程轉換為可擴充、受管理的行銷活動階層。

本指南適用於Workfront管理員和進階使用者，協助他們在Workfront Planning中實作及設計您的環境架構。

## 成功架構概觀

隨著您的行銷作業日漸成熟，您資料的複雜度也會隨之提升。 如果沒有清晰的藍圖，您的行銷記錄系統可能會很快變成垃圾桶，裡面會棧滿中斷連線的記錄、衝突的術語和報告孤島。

當您建置成功的架構時，您會在Workfront Planning中建立架構，用於模型化您的行銷活動階層。 它將您從試算表混亂轉移到受控制的物件導向模型，確保每個團隊都說著相同的語言，同時保持他們執行所需的靈活性。

## 建立階層以定義意圖層級

為了保持清晰度和擴充性，我們建議您在使用Workfront Planning設計工作流程時，從經驗證的核心路徑開始。

從那裡，您可以透過新增更多層級到您的架構來擴展您的策略。

### 核心路徑：如何從策略邁向行動

雖然組織可以隨著其營運需求的發展而擴大此階層，但從以下各節所述的三個層級開始，可確保策略與執行之間架起穩固的橋樑。

從我們的發現中，我們注意到Workfront Planning最成功的實作是在橫跨Planning和Workfront的乾淨、三層架構模型上取得成果。

以下是成功的Planning實作層級，以及您可能會考慮建立以在此過程中支援您的成品：

* **第1級：行銷活動(Workfront規劃)**

   * **焦點：**&#x200B;定義長期策略支柱與年度計畫。 例如，為您的組織定義名為「FY26全球品牌認知度」的計畫。 這是指定時間範圍的焦點。 建立行銷活動以支援此計畫。

   * **角色：**&#x200B;此層級的利害關係人可以是行銷人員、行銷副總或其他策略性潛在客戶。

  如需詳細資訊，請參閱[建立記錄型別](/help/quicksilver/planning/architecture/create-record-types.md)。

* **第2級：通路策略(Workfront規劃)**

   * **焦點：**&#x200B;定義概述特定管道之「內容」的營運簡介。 這是工作開始前策略性意圖的最後一層。 例如，建立「第1季社群媒體閃爍」策略。 然後，您就可以將其與行銷活動配對。

   * **角色：**&#x200B;主要利害關係人是行銷營運負責人、頻道負責人或行銷活動經理。

* **第3級：專案(規劃與Workfront)**

   * **焦點：**&#x200B;在將會最終完成您方案的確切體驗或活動上執行。 有些交付專案是特定的，例如社交貼文、電子郵件、網頁。

   * **實作：**&#x200B;您可以在Planning中建立策略，並將其直接連結至Workfront中的&#x200B;**專案**，其中個別交付專案會作為任務和問題管理。

   * **角色：**&#x200B;這裡的主要利害關係人是創意人員、個人貢獻者，以及負責為支援此計畫而工作的所有人。

### 策略性擴充：如何新增更多層級

建立核心路徑後，在仔細考慮特定業務複雜度後，您可以選擇新增其他圖層。

您可能會發現建立下列其他專案很有用：

* **頻道計畫：**&#x200B;促銷活動與戰術之間的圖層，可將跨職能策略分組。 例如，名為「數位策略」的計畫。

* **活動：**&#x200B;如果您在低容量環境中工作（您每年可能有5,000個或更少的交付專案），某些團隊在成為Workfront專案之前，可能偏好追蹤個別體驗作為Workfront Planning記錄。

>[!IMPORTANT]
>
>如果您的組織每年產生超過5,000個活動，您應該將個別交付專案追蹤移至Workfront。
>
>在Planning中管理大量體驗記錄，可能會導致資料累積，使您的策略可見性變得模糊。
>我們建議您遵循這項廣泛的指引，以發揮最大效率：
>
>* 使用Planning瞭解「原因」和「內容」
>* 將Workfront用於高容量的「做法」。

## 瞭解重心以建置您的架構

企業級行銷記錄系統並非建置在單一工作區中。 它使用「軸輻式」架構，在自然的重心中管理記錄型別。

如需詳細資訊，請參閱[推出您的策略首頁：30天啟動台](/help/quicksilver/planning/best-practices.md/30-day-launchpad.md)。

若要使用軸輻式方法建置架構，您必須建立下列專案：

* 分類中心
* 策略規劃工作區
* 功能輻條

### 將分類中樞建置為您的分類

您必須先為全域分類建立一個集中式工作區，以定義組織中的每個人必須瞭解的主要概念。 例如，在中央工作區中建立以下記錄型別：品牌、地區、產品、角色。

如需詳細資訊，請參閱[建立記錄型別](/help/quicksilver/planning/architecture/create-record-types.md)。

在建立分類時建立下列專案：

* **主要位置：**&#x200B;請選擇主要工作區。 此工作區應該是您建立之記錄型別的真實來源。

* **優點：**&#x200B;藉由將這些定義整合到其他企業中，您便可釐清像「地區：歐洲、中東及非洲」這樣的概念對每個團隊來說都是相同意義。

### 將策略規劃工作區建立為您的執行中心

執行中心是高階行銷活動（以及任何管道計畫）的舉辦地。

* **主要位置：**&#x200B;這是執行重心，為策略決策提供無雜訊環境。

* **優點：**&#x200B;領導階層無需聆聽日常戰術雜訊，即可管理行銷活動組合。

### 將功能輻條定義為團隊的工作區

功能單位(社交、Creative、電子郵件)有各自的工作區來管理其策略。

* **主要位置：**&#x200B;這些工作區是本機專案團隊執行的個別重心。

* **優點：**&#x200B;團隊使用來自中樞的全域行銷活動和分類，同時維護自己的本機物件。

  例如，團隊可從中央工作區將行銷活動記錄型別新增至團隊的工作區，但建立僅與團隊工作區相關的行銷活動。 行銷活動的範例為「Media outlets」或「Usage rights」。

## 使用名詞式治理方法

若要確保您的架構承受壓力，請遵循名詞式治理的原則。

在Workfront Planning中建立實體時，我們建議採取下列步驟：

* **使用名詞，而非動詞：**&#x200B;在追蹤的事情之後命名記錄型別（將其命名為「Campaign」或「Tague」），而不是要完成的動作（不要將其命名為「Campaigning」或「Planning」）。

* **標準化命名法：**&#x200B;在所有工作區中使用相同的名稱。 這可讓您彙總整個投資組合的資料，以利執行報告。

## 現有的投資組合和計畫呢？

成熟組織的一個常見問題是如何處理已在Workfront中建立的投資組合和計畫。 過去，這些物件經常用來模擬策略規劃。

現在，我們建議您將此方法轉移至Workfront Planning，自然而然地適合策略性的規劃方法。

### 以記錄型別取代投資組合和計畫

在許多組織中，產品組合用於代表高階品牌或業務單位，而計畫則代表策略主題。

在Workfront Planning中，這些最好在您的分類中樞中模組化為「記錄型別」。

通過將品牌或業務單位視為記錄型別，您可以將它們連結到整個企業的促銷活動或策略，提供比靜態Portfolio （計畫結構）更靈活的報告。

### 使用報告橋接策略

雖然Workfront Planning是策略性意圖的未來，但其透過畫布控制面板的原生報表仍日趨成熟。

許多組織仍仰賴Workfront中與其舊版Portfolio和方案結構繫結的強大報表功能。

我們建議嘗試以下解決方法：

* 請勿刪除您的投資組合和計畫。
* 使用Planning自動化在您的記錄型別與投資組合和計畫之間建立橋樑。

  在Workfront Planning中建立策略或行銷活動時，該記錄可在Workfront中產生相對應的Portfolio或方案。

  如需詳細資訊，請參閱[使用Adobe Workfront Planning記錄自動化建立物件](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md)。

這可讓您：

* 使用時間軸和行事曆，享受Workfront Planning卓越的策略視覺效果。

* 針對尚未準備好移至畫布的利害關係人，維護您在Workfront中的舊版報告。

## 最佳作法和秘訣

### 待辦事項

* **堅持核心路徑優先方法：**&#x200B;先建立您的行銷活動對策略對專案流程，再增加更多複雜性。

* **指定主要工作區：**&#x200B;請確定每個記錄型別都有一個主工作區（請考量其重心）做為報告的彙總。

* **為擷取程式排定要求表單的優先順序：**&#x200B;在Workfront Planning中使用較不複雜的群組記錄表單，以確保中繼資料的完整性。

  >[!CAUTION]
  >
  >雖然進階使用者可從表格檢視中的直接資料輸入中獲益，但應謹慎行事。
  >表格中的大量變更可以輕鬆為其他利害關係人建立資料難題。

### 不要

* **請勿使用一般化：**&#x200B;例如，在談論執行時，不要談論「核心」環境，而是要特別提到Workfront和專案物件。

* **不要過於複雜：**&#x200B;每個額外的階層層級都會增加管理稅。 僅新增回答目前無法回答之業務問題的層級。

* **不要建立獨立單位：**&#x200B;請確認您的記錄型別是跨工作區共用的，因此團隊不會重新輸入相同的資料。


<!--original content:


## Goal 

Learn how to translate your complex business processes into a scalable, governed campaign hierarchy using "Centers of Gravity" and a multi-workspace architecture. 

 

## Overview 

As your marketing operations scale, so does the complexity of your data. Without a clear blueprint, your Marketing System of Record (MSOR) can quickly become a "junk drawer" of disconnected records, conflicting terminology, and reporting silos. 

 

The "Blueprint of Success" is a framework for modeling your campaign hierarchy in Workfront Planning. It moves you from "spreadsheet chaos" to a governed, object-oriented model that ensures every team speaks the same language while maintaining the agility they need to execute. 

 

## The Hierarchy: Finding Your Levels of Intent 

To maintain clarity and scalability, we recommend starting with a proven **Core Path**. While organizations can expand this hierarchy as their operational needs evolve, beginning with these three levels ensures a strong bridge between strategy and execution. 

 

### The Core Path: Strategy to Action 

Most successful implementations thrive on a clean, three-tier model that spans both Planning and Workflow: 

 

1. **Level 1: Campaigns (Planning Module)** 

    * **Focus:** Long-term strategic pillars and annual initiatives (e.g., "FY26 Global Brand Awareness").  

    * **Persona:** CMO, VP of Marketing, Strategic Leads. 

2. **Level 2: Channel Tactics (Planning Module)** 

    * **Focus:** The operational briefs defining the "what" for specific channels (e.g., "Q1 Social Media Blitz"). This is the final layer of strategic intent before work begins. 

    * **Persona:** Marketing Ops, Channel Leads, Campaign Managers. 

3. **Level 3: Workflow Projects (Workflow Module)** 

    * **Focus:** The actual execution of "Experiences" or "Activities" (e.g., specific social posts, emails, web pages).  

    * **Implementation:** Tactics in Planning link directly to **Projects** in the Workflow module, where individual deliverables are managed as tasks and issues. 

    * **Persona:** Creatives, Individual Contributors. 

 

### Strategic Expansion: Adding More Levels 

Once the core path is established, organizations may choose to add additional layers after careful consideration of their specific business complexity: 

 

* **Channel Plans:** A layer between *Campaigns* and *Tactics* to group cross-functional strategies (e.g., "Digital Strategy"). 

* **Workfront Planning Activities:** In lower-volume environments (typically <5,000 deliverables/year), some teams prefer to track individual "Experiences" as Workfront Planning records before they become projects. 


>[!TIP]
>
>**Crucial Tip: The 5,000 Deliverable Threshold** 
>
>If your organization produces more than 5,000 activities per year, you should **always** offload individual deliverable tracking to the **Workflow module**. Managing high-volume "Experience" records in Planning can lead to data accumulation that obscures your strategic visibility. Use Planning for the "Why" and "What," and the Workflow module for the high-volume "How." 

 

## Architecture: Centers of Gravity 

An enterprise-grade MSOR isn't built in a single workspace. It uses a "Hub-and-Spoke" architecture where record types are managed in their natural **Centers of Gravity**. 

 

### 1. The Taxonomy Hub (Classifications) 

Establish one centralized workspace for your "Global Classifications" (e.g., Brands, Regions, Products, Personas). 

* **Primary Location:** This workspace is the "Source of Truth" for these objects. 

* **The Benefit:** By syndicating these definitions to the rest of the business, you solve "Semantic Drift"—ensuring that "Region: EMEA" means the same thing to every team. 

 

### 2. The Strategic Planning Workspace (Executive Center) 

This is where high-level **Campaigns** (and any **Channel Plans**) live.  

* **Primary Location:** This is the executive center of gravity, providing a noise-free environment for strategic decision-making. 

* **The Benefit:** Leadership can manage the portfolio without seeing the day-to-day tactical mess. 

 

### 3. Functional Spokes (Team Workspaces) 

Functional units (Social, Creative, Email) have their own workspaces to manage their **Tactics**. 

* **Primary Location:** These workspaces are the center of gravity for local team execution.  

* **The Benefit:** Teams "consume" the global campaigns and classifications from the hubs, while maintaining their own local objects (like *Media Outlets* or *Usage Rights*). 

 

## Noun-Based Governance: Speak One Language 

To ensure your blueprint holds up under pressure, follow the principle of **Noun-Based Governance**.  

 

* **Use Nouns, Not Verbs:** Name your record types after the "things" you are tracking (`Campaign`, `Tactic`), not the "actions" (`Campaigning`, `Planning`). 

* **Standardize Nomenclature:** Use the same names across all workspaces. This allows you to aggregate data across the entire portfolio for executive reporting. 

 

## What About Existing Portfolios and Programs? 

A common question for mature organizations is how to handle the Portfolios and Programs they've already built in the **Workflow module**. In the past, these objects were often used to mimic strategic planning. 

 

### 1. Portfolios & Programs → Record Types 

In many organizations, **Portfolios** are used to represent high-level Brands or Business Units (BUs), while **Programs** represent strategic themes. 

* **The Shift:** These are best modeled as **Record Types** in your **Taxonomy Hub**. By treating "Brand" or "Business Unit" as a record type, you can link them to any campaign or tactic across the entire enterprise, providing much more flexible reporting than a static Portfolio/Program structure. 

 

### 2. The "Reporting Bridge" Strategy 

While Workfront Planning is the future of strategic intent, its native reporting via **Canvas Dashboards** is still maturing. Many organizations still rely on the robust reporting capabilities tied to their legacy Portfolio and Program structures in the Workflow module. 

* **The Recommendation:** Don't delete your Portfolios and Programs yet. Instead, use **Fusion automations** to create a bridge.  

* **How it Works:** When a Tactic or Campaign is created in Workfront Planning, Fusion can automatically mirror that record into a corresponding Portfolio or Program in the Workflow module. This allows you to: 

    1. Enjoy Workfront Planning's superior **strategic visualization** (Timelines/Calendars). 

    2. Maintain your **legacy reporting** in the Workflow module for stakeholders who aren't yet ready to move to Canvas. 

## Best Practices & Tips 

### Do: 

* **Stick to the Core Path first.** Establish your Campaign-to-Tactic-to-Project flow before adding more complexity. 

* **Designate Primary Workspaces.** Ensure each record type has one "home" workspace (its center of gravity) that acts as the aggregator for reporting. 

* **Prioritize Forms for Intake.** Use record forms for groups with less sophistication in Workfront Planning to ensure metadata integrity. While Power Users may benefit from direct data entry in Table views, this should be approached with caution—bulk changes in a table can easily create data headaches for other stakeholders. 
 

### Don't: 

* **Don't say "Core".** Refer specifically to the **Workflow module** and the **Project** objects when talking about execution. 

* **Don't over-complicate.** Every additional level of hierarchy adds a "management tax." Only add levels that answer a business question you can't currently answer. 

* **Don't create silos.** Ensure your record types are shared across workspaces so teams aren't re-typing the same data.
-->