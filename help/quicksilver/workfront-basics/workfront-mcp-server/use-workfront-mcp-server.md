---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: 使用Adobe Workfront MCP伺服器
description: 使用Adobe Workfront MCP伺服器，透過AI代理平台中的自然語言對話來搜尋、建立、更新和管理Workfront專案。
author: Courtney
feature: Get Started with Workfront
source-git-commit: e009d9d52ddb478759c11a20967d48049f797d97
workflow-type: tm+mt
source-wordcount: '1875'
ht-degree: 0%

---


# 使用Adobe Workfront MCP伺服器

[!DNL Adobe Workfront] MCP伺服器可讓您透過詢問自然語言的AI代理平台，來尋找、建立、更新和管理Workfront專案。 平台會決定要呼叫哪些Workfront動作，並替您處理與Workfront的對話。

>[!IMPORTANT]
>
>目前，Workfront MCP伺服器僅供使用AWS的客戶使用。

## 先決條件

* 您必須設定AI代理平台與Workfront MCP伺服器之間的連線。 如需安裝指示，請參閱[設定Adobe Workfront MCP伺服器](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md)。
* 您的Workfront執行個體必須在Adobe Identity Management系統(IMS)上啟用。
* 您必須擁有對您要使用的專案具有必要存取層級和物件許可權的Workfront帳戶。
* 若要搭配Workfront Planning使用MCP，您的組織必須位於包含Adobe Workfront Planning的Workfront套件上。

本文假設您已設定連線。 如需安裝程式的詳細資訊，請參閱[設定Adobe Workfront MCP伺服器](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md)。

## 可用的工具

Workfront MCP伺服器會公開AI代理平台代表您呼叫的一組工具。 例如，搜尋Workfront、建立專案、更新欄位和管理核准的工具。 如需完整參考清單，請參閱[Adobe Workfront MCP伺服器工具](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-tools.md)。

>[!IMPORTANT]
>
>當您將AI代理平台連線到Workfront時，它會使用您的Workfront帳戶和許可權在Workfront中運作。 平台的動作與您直接在Workfront介面中執行的動作具有相同的效果。<br>
>
>您和您的AI代理平台提供者需負責平台在Workfront中採取的動作。 Adobe不負責變更AI代理平台對您的Workfront資料。<br>
>
>在讓AI代理平台繼續處理請求之前，請確認您瞭解它要做什麼，尤其是針對變更或刪除資料的動作。


## 要問的問題的範例

連線之後，請在AI代理平台中輸入自然語言請求。 AI代理平台會決定要呼叫哪些Workfront動作並傳回結果。

>[!NOTE]
>
>由於Workfront設定區域中的管理員控制項，部分動作可能無法使用。 例如，如果您的Workfront管理員已停用MCP伺服器的寫入動作，您可能無法建立專案。


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

<!--
* *Remove Anna Jones from all approvals in this project, and replace with Sione Carter.*
-->


### 使用Planning記錄

>[!IMPORTANT]
>
>* 若要搭配Workfront Planning使用MCP，您的組織必須位於包含Adobe Workfront Planning的Workfront套件上。

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


## 考量事項

使用Workfront MCP伺服器時，請謹記下列考量事項：

### AI代理平台可能會使用交談中先前提供的資訊

AI代理平台有時會重複使用交談中先前提供的資料，而非要求Workfront提供最新資訊。 如果自從上次檢視AI代理平台後，Workfront中發生某些變更，您可能會看到過時的資訊。

若要強制AI代理平台擷取最新資料，請明確要求擷取最新資料。 例如：

* *從Workfront取得最新資料。 不要使用快取的結果。*

### 檢查Workfront MCP伺服器的更新

您可能想要定期重新整理與Workfront MCP伺服器的連線，以確保您擁有最新的工具和功能。

大部分的更新應該都會自動進行。 不過，我們建議您定期檢視Workfront發行說明。


## 資料與安全性

Workfront MCP伺服器工具與API呼叫的運作方式一致。 Workfront不會儲存提示、回應或任何其他資料。 您可以透過Workfront平台存取您所要求的任何Workfront資料。

您的存取層級和物件許可權會決定您可以查詢或寫入Workfront的內容。 您的Workfront管理員可以控制Workfront設定區域中的MCP讀取和寫入動作。

### 哪些資料離開Workfront

AI代理平台提供者可存取您透過Workfront MCP伺服器互動的Workfront資料。 如需詳細資訊，請洽詢您的AI代理平台提供者。


### AI代理平台提供者如何處理您的Workfront資料

Workfront無法控制AI代理平台提供者處理您Workfront資料的方式。 如需詳細資訊，請洽詢您的AI代理平台提供者。

## 疑難排解日常使用

+++ 展開以檢視Workfront MCP伺服器的日常使用疑難排解提示。

| 問題 | 可能的原因 | 修正 |
| --- | --- | --- |
| AI代理平台提供您過時的資訊。 | AI代理平台正在重複使用交談中先前提供的資料。 | 向Workfront索取最新資料。 |
| AI代理平台從錯誤的Workfront專案傳回資料。 | AI代理平台根據模稜兩可的措辭挑選了錯誤的專案。 | 再次詢問您更具體的名稱、ID或篩選器。 |
| 更新或刪除在Workfront中未生效。 | 您的Workfront管理員已停用Workfront MCP伺服器的寫入動作，或您無權對特定專案執行動作。 | 透過AI代理平台確認該動作已執行。 然後檢查是否已為Workfront MCP伺服器啟用寫入動作，以及您是否有變更專案的許可權。 |

如需有關設定和驗證問題的詳細資訊，請參閱[設定Adobe Workfront MCP伺服器](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md)中的[疑難排解設定和驗證](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#troubleshoot-setup-and-authentication)。

+++

## 常見問題

+++ 展開以檢視關於使用Workfront MCP伺服器的常見問題。

### 什麼是AI代理平台？

AI代理平台是一種AI工具，可以在以下位置代表您執行動作：
其他系統，而不只是回答問題。 當您將一個連結至Workfront時
透過MCP伺服器，它可以找到、建立、更新和刪除Workfront
根據您以自然語言詢問的專案而定。 範例包括Claude
案頭、ChatGPT和其他與MCP相容的AI使用者端。


### 我是否需要成為Workfront管理員才能使用Workfront MCP伺服器？

否。 任何Workfront使用者都可透過連線使用Workfront MCP伺服器
AI代理平台。 AI代理平台會使用您的Workfront運作
帳戶、存取層級和物件許可權，因此您只能執行您自己的操作
可能已經直接在Workfront中執行。

### 為什麼AI代理平台無法為我建立、更新或刪除專案？

您的Workfront管理員可控制中允許的MCP動作
Workfront設定區域。 如果寫入動作停用，AI代理平台
仍可尋找和閱讀Workfront專案，但無法進行變更。 您也
需要特定專案的正確存取層級和物件許可權
您正在使用的專案。

### AI代理平台會在變更或刪除Workfront資料之前詢問我嗎？

這取決於AI代理平台，而不是Workfront。 大部分平台
在執行動作前提示您確認，尤其是刪除動作。
核准請求前，請先詳閱平台說明即將進行的作業 — 
變更會在Workfront中發生，就像您進行變更時一樣
介面中為您自己。

<!--

### Can I undo something the AI agentic platform did in Workfront?

Changes the AI agentic platform makes in Workfront work the same way as 
changes you make in the interface. If Workfront supports undoing or 
restoring a particular action (for example, restoring a deleted item from 
the Recycle Bin), the same options apply. If Workfront doesn't normally let 
you undo an action, you can't undo it through the AI agentic platform either.

-->

### 為什麼AI代理平台傳回錯誤的Workfront專案？

AI代理平台會根據您使用的字詞挑選專案。 若您的
請求模稜兩可 — 例如，兩個專案具有相似的名稱 — 它
可能會選錯對象。 再次詢問您更具體的名稱、ID、日期、
或篩選以縮小結果。


### 我可以透過AI代理平台處理哪些Workfront專案？

透過存取層級和，您在Workfront中有權存取的任何專案
物件許可權。 這包括專案、任務、問題、檔案、
核准、規劃記錄等。

### 其他人能看見我與AI代理平台的對話嗎？

Workfront不會儲存您的提示或AI代理平台的回應。
提供您的AI代理平台的人可控制您的對話方式
會儲存或共用。 請洽詢您的AI代理平台提供者，以瞭解
詳細資料。

### 我是否需要知道Workfront API或要使用哪種MCP工具？

否。 AI代理平台會將您的自然語言請求轉譯為
Workfront的正確動作，並為您挑選正確的工具。 如果您是
已經熟悉Workfront API，這些動作會很熟悉，
但這不是必要條件。

### 我的Workfront資料會傳送給AI代理平台提供者還是由他們儲存？

如需詳細資訊，請參閱此專案中的[資料與安全性](#data-and-security)
文章。

### 新版本的Workfront MCP伺服器發行時會發生什麼事？

MCP伺服器通常會自動更新，但有時您可能需要重新整理與MCP伺服器的連線，才能檢視最新的工具和功能。

### 如果Workfront Identity Management System (IMS)上未啟用我的Workfront執行個體，我可以使用Adobe MCP伺服器嗎？

否。 您的Workfront執行個體必須在Adobe Identity Management系統(IMS)上啟用，才能使用Workfront MCP伺服器。 如果您不確定您的執行個體是否已在IMS上啟用，請聯絡您的Workfront管理員。


+++
