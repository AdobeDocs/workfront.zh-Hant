---
title: 2026年第三季度發行時間範圍內的其他增強功能
description: 2026年第三季度發行時間範圍內的其他增強功能
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 937b49b44f102fee6c9847ab950eb2b274aee89b
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 0%

---

# 2026年第三季度發行時間範圍內的其他增強功能

本頁說明2026年第三季度版本對預覽環境所做的增強功能。 如上所述，這些增強功能將於生產環境中提供。

如需2026年第三季度發行週期中目前可用的所有變更清單，請參閱[2026年第三季度發行概觀](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md)。

## Workfront MCP聯結器的更新

我們已對Workfront MCP聯結器進行下列更新：

* 我們已擴充MCP伺服器，以使用歐盟<!-- and US instances that are not on AWS. Each MCP server can only connect to one instance, but are no longer limited to US instances on AWS-->的執行個體。
* 為了擴充Workfront MCP聯結器的彈性，我們新增了連線Claude的功能。 現在，您可以在Claude的聯結器清單中找到Workfront，或直接使用URL連線。

如需詳細資訊與指示，請參閱[設定Adobe Workfront MCP伺服器](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md)。


## 更新評論通知電子郵件的外觀

>[!NOTE]
>
>客戶的生產版本：自2026年7月16日起分階段推出

更新區域中評論的電子郵件通知具有新外觀，且符合更廣泛的Adobe電子郵件設計。

更新的電子郵件格式包括：

* 新的Adobe Workfront頁首，取代之前的Workfront品牌。
* 著重於最新註解的簡化版面。
* 主要&#x200B;**在Workfront**&#x200B;按鈕中檢視以直接開啟專案。

先前註釋的執行緒不再包含在電子郵件內文中。 若要檢視專案上先前的註解，請使用&#x200B;**在Workfront中檢視它**&#x200B;在Workfront中開啟交談。

此變更將分階段向客戶推出。 確認轉出排程時，此頁面將會更新。

![已更新評論通知email.png](assets/email-look-and-feel-update.png)

## 使用Workfront MCP伺服器將Workfront連線至您的AI工具

>[!NOTE]
>
>預覽： 2026年5月28日>生產快速版本： 2026年6月11日>每個人的生產： 2026年7月16日

您的團隊的營運環境存在於Workfront中。 現在有了Workfront MCP伺服器，該內容就可以從您團隊已使用的AI工具中操作。

將Workfront連線至任何與MCP相容的AI平台，包括Claude、ChatGPT、Copilot、Gemini等，並使用自然語言尋找、建立、更新和管理Workfront專案，而不需離開您選擇的AI工具。 詢問您逾期的任務、推播專案的完成日期、傳送提醒給核准者、更新行銷活動預算，而您的AI平台會在Workfront中為您工作。

此外，藉由Claude的AI技能和排程工作，您可以更進一步，自動化針對即時Workfront資料主動執行的週期性工作流程。 例如，星期一早上專案簡報、每週容量報告、每月行銷活動健康情況檢查 — 設定一次，AI會根據您操作的完整內容自動處理。

這是代理式工作管理系統的基礎 — 其中AI以您最豐富的營運資料為基礎，而人類和AI共同作業，讓工作以全速運作。

>[!IMPORTANT]
>
>目前，Workfront MCP伺服器僅開放美國地區的客戶使用，供使用AWS的客戶使用。

如需詳細資訊，請參閱[Adobe Workfront MCP伺服器總覽](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-overview.md)。

## 增強型清單更新

>[!NOTE]
>
>預覽： 2026年5月28日>生產快速版本： 2026年6月11日>每個人的生產： 2026年7月16日

增強型清單上的多種欄位型別已更新，包括鍵盤導覽和其他增強功能。

增強型清單中的受指派人欄位現在提供鍵盤導覽：

* 使用鍵盤上的向上和向下箭頭在人員清單中移動。
* 按空格鍵以選取人員，或\&lt;Delete\>以移除選取的人員。

在增強型清單中的單一和多重選取欄位上：

* 欄位互動現在可使用鍵盤存取。 這包括標籤之間的導覽、搜尋選項，以及使用向上和向下箭頭的清單。 按空格鍵以選取專案，或\&lt;Delete\>以移除選取的專案。
* 找不到結果時，可以直接從編輯器建立新選項。 請注意，並非所有清單都提供此功能。

預先輸入和外部查詢欄位等參考欄位已收到一些介面增強功能。

此外，在視覺上改善拖放欄（在提供拖放功能的清單上）的體驗。

如需詳細資訊，請參閱[使用增強型清單](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)。
