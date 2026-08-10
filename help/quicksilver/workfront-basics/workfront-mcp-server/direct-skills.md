---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: 可直接安裝的技能
description: Workfront提供一些可直接安裝在LLM的技能。
author: Becky
feature: Get Started with Workfront
source-git-commit: 20f5a513d8d33ecf8770f35bc73ee799a7de939e
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---


# 可直接安裝的技能

Workfront提供一些可直接安裝在LLM的技能。 技能指南會指導您如何將這些工具用於特定工作，並且已內建正確的步驟。

您可以在Adobe Skills GitHub存放庫中找到這些技能。

>[!NOTE]
>
>目前，這些技能僅適用於Claude。
>如需使用Adobe設定Claude的指示，請參閱Adobe Developer檔案中的[快速入門](https://developer.adobe.com/adobe-for-creativity/getting-started/)。

## 將技能從Workfront GitHub存放庫安裝到Claude。

1. 前往GitHub上的[Adobe Workfront技能存放庫](https://github.com/adobe/skills/tree/main/plugins/workfront)。
1. 下載您要使用的技能資料夾。
1. 將資料夾複製到您的Claude技能庫。

   * 克勞德案頭： `~/Library/Application Support/Claude/skills/` (macOS)或同等專案。
   * 克勞德程式碼： `~/.claude/skills/`。

<!--

1. Go to the [Adobe Workfront skills repository](https://github.com/adobe/skills/tree/main/plugins/workfront) on GitHub.
1. Download the skill file you want to use.
1. In Claude, click **Customize**.
1. Select **Skills**.
1. Click **Create skill** -> **Upload a skill**.
1. Upload the zipped skill file to Claude, then click **Confirm** to install.

-->

## 目前可用的技能

| 技能/資料夾連結 | 技能說明 | 可用於 |
|---|---|---|
| [Planning解決方案架構者](https://github.com/adobe/skills/tree/main/plugins/workfront/skills/wf-planning-solution-architect) | 設定Workfront規劃工作區以滿足您的需求，並回答有關Workfront規劃的問題。 | 克勞德 |
