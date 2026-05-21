---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: 使用Adobe Workfront MCP伺服器
description: 使用Adobe Workfront MCP伺服器，透過AI代理平台中的自然語言對話來搜尋、建立、更新和管理Workfront專案。
author: Courtney
feature: Get Started with Workfront
hide: true
source-git-commit: 152486b7850e01f3de23f22bbe3729c5cd3d3aa2
workflow-type: tm+mt
source-wordcount: '1164'
ht-degree: 0%

---


# 使用Adobe Workfront MCP伺服器

[!DNL Adobe Workfront] MCP伺服器可讓您透過詢問純英文的AI代理平台，來尋找、建立、更新和管理Workfront專案。 平台會決定要呼叫哪些Workfront動作，並替您處理與Workfront的對話。

[!DNL Claude]是目前唯一受支援的AI代理平台，但本文中的範例和模式適用於任何支援Workfront MCP伺服器的AI代理平台。

本文假設您已設定連線。 如需安裝程式的詳細資訊，請參閱[設定Adobe Workfront MCP伺服器](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md)。 如需Workfront MCP伺服器的詳細資訊，請參閱[Adobe Workfront MCP伺服器概述](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-overview.md)。

## 可用的工具

Workfront MCP伺服器會公開AI代理平台代表您呼叫的一組工具，例如搜尋Workfront、建立專案、更新欄位和管理核准的工具。 如需依Workfront區域分組的完整參考清單，請參閱[Adobe Workfront MCP伺服器工具](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-tools.md)。

>[!IMPORTANT]
>
>當您將AI代理平台連線到Workfront時，它會使用您的Workfront帳戶和許可權在Workfront中運作。 平台的動作與您直接在Workfront介面中執行的動作具有相同效果。
>
>您和您的AI代理平台提供者需負責平台在Workfront中採取的動作。 Adobe對使用AI代理平台變更Workfront資料概不負責。
>
>在讓AI代理平台繼續處理請求之前，請確認您瞭解它要做什麼，尤其是針對變更或刪除資料的動作。


## 要問的問題的範例

連線之後，請在AI代理平台中輸入自然語言請求。 AI代理平台會決定要呼叫哪些Workfront動作並傳回結果。

### 尋找並檢視您的工作

若要搜尋Workfront中符合您要尋找的專案，請詢問：

* *顯示品牌行銷團隊的所有使用中專案。*
* *取得指派給Joan Harris的所有工作。*
* *顯示[技術]類別下[網站重新設計]專案中的所有問題。*

### 建立新專案

若要建立專案、任務或其他Workfront專案，請詢問：

* *從3月10日起至4月30日止，建立名為「Q2 Innovation Sandbox」的空白專案。 將我設為擁有者。*
* *將名為「登陸頁面QA」的新任務新增至專案，並排程從4月22日至4月26日。*
* *建立名為「2026年夏季優惠」的新行銷活動記錄。*

### 更新現有專案

若要變更Workfront中已有的專案，請詢問：

* *更新「設計評論」任務，使其在4月18日完成，並將其指派給創意團隊。*
* *若為「Lucent AI Launch - NA」專案，請將完成時間推進至4月中旬，並將預算增加至$150,000。*
* *將「夏季行銷活動」記錄中的預算欄位更新為$75,000。*

### 刪除專案

若要移除Workfront專案，請詢問：

* *刪除名為「Q1測試促銷活動」的專案。*
* *從專案移除[列印資產生產]工作。*
* *刪除名為「舊促銷活動」的行銷活動記錄。*

>[!WARNING]
>
>透過AI代理平台刪除Workfront中的專案，與在Workfront介面中刪除它們相同。 在讓AI代理平台繼續之前，請先確認要刪除的內容。

### 使用核准

若要管理檔案和資產核准，請詢問：

* *將Sarah Chen和Miguel Alvarez新增為目前檔案的核准者。*
* *傳送提醒給資產「Spring Campaign影片」上尚未回應的核准者。*
* *將「行銷啟動」核准範本套用至資產「春季行銷活動影片」。*


### 使用Planning記錄

若要管理計畫記錄，請詢問：

* *為品牌行銷團隊建立名為「Q2行銷計畫」的新計畫記錄。*
* *新增名為「社群媒體稽核」的工作至計畫記錄。*
* *更新「社群媒體稽核」任務，使其於4月18日完成，並將其指派給創意團隊。*

### 使用工作流程

若要管理工作流程，請詢問：

* *將「Q2 Innovation Sandbox」專案路由至Innovation Review Board。*
* *將「夏季行銷活動」記錄更新為「準備啟動」狀態。*
* *核准「夏季行銷活動」記錄。*


### 在交談中鏈結請求

您可以在單一交談中鏈結要求。 AI代理平台會保留上下文，以便每個請求都可以建置在先前的請求上。 例如：

1. 要求一組專案： *尋找我的逾期工作。*
1. 取得清單之後，請要求針對結果執行動作： *將所有結果更新至下個星期五。*

<!-- NEEDS DETAIL: Test multi-step prompt chaining in a working setup and document the patterns that produce reliable results. -->

## 考量事項

使用Workfront MCP伺服器時，請謹記下列考量事項。

### AI代理平台可能會使用交談中先前提供的資訊

AI代理平台有時會重複使用交談中先前提供的資料，而非要求Workfront提供最新資訊。 如果自從上次檢視AI代理平台後，Workfront中發生某些變更，您可能會看到過時的資訊。

若要強制AI代理平台擷取最新資料，請明確要求擷取最新資料。 例如：

* *從Workfront取得最新資料。 不要使用快取的結果。*

### Workfront MCP伺服器會自動更新

Adobe發行新版Workfront MCP伺服器時，您的AI代理平台會自動使用新版本。 您不需要重新連線或變更任何專案。

## 資料與安全性

<!-- NEEDS DETAIL: Document Adobe's official position on data handling and security when Workfront data is passed through an AI agentic platform. Cover: what data leaves Workfront, where it goes, whether it is retained or used for training by the AI agentic platform provider, what happens to it after the conversation ends, and any differences between AI agentic platforms (for example, Anthropic's enterprise data handling policies for Claude). This section needs sign-off from security and legal before publication. -->

### 哪些資料離開Workfront

<!-- NEEDS DETAIL: List the categories of Workfront data that can be sent to the AI agentic platform (item names, field values, attachments, user identifiers, etc.) and any data that the MCP server explicitly does not expose. -->

### AI代理平台提供者如何處理您的Workfront資料

<!-- NEEDS DETAIL: For each supported AI agentic platform, summarize the provider's data handling stance: retention, training opt-out, and enterprise vs. consumer differences. Link to the provider's official documentation. Start with Claude (Anthropic). -->

### AI代理平台之間的差異

<!-- NEEDS DETAIL: Note any meaningful differences in how each supported AI agentic platform handles Workfront data once additional AI agentic platforms are supported. -->

## 疑難排解日常使用

+++ 展開以檢視Workfront MCP伺服器的日常使用疑難排解提示。

| 問題 | 可能的原因 | 修正 |
|---|---|---|
| AI代理平台提供您過時的資訊。 | AI代理平台正在重複使用交談中先前提供的資料。 | 向Workfront索取最新資料。 |
| AI代理平台從錯誤的Workfront專案傳回資料。 | AI代理平台根據模稜兩可的措辭挑選了錯誤的專案。 | 再次詢問您更具體的名稱、ID或篩選器。 |
| 更新或刪除在Workfront中未生效。 | AI代理平台尚未呼叫動作，或您的許可權不允許此操作。 | 透過AI代理平台確認動作已執行，然後檢查您的Workfront許可權。 |

如需有關設定和驗證問題的詳細資訊，請參閱[設定Adobe Workfront MCP伺服器](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md)中的[疑難排解設定和驗證](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#troubleshoot-setup-and-authentication)。

+++

## 常見問題

+++ 展開以檢視關於使用Workfront MCP伺服器的常見問題。

### 我可以透過AI代理平台處理哪些Workfront專案？

您在Workfront中透過存取層級和物件許可權存取的任何專案。

<!-- NEEDS DETAIL: List the supported Workfront object types. -->

### 我的Workfront資料會傳送給AI代理平台提供者還是由他們儲存？

如需詳細資訊，請參閱本文中的[資料與安全性](#data-and-security)。

### 新版本的Workfront MCP伺服器發行時會發生什麼事？

MCP伺服器會自動更新。 您不需要重新連線或變更任何專案。

### 要使用Workfront MCP伺服器，我是否需要知道Workfront API？

否。 AI代理平台會將您的自然語言請求轉譯為正確的Workfront動作。 如果您已熟悉Workfront API，會覺得這些動作很熟悉，但這不是必要條件。

+++
