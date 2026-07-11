---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: 設定Adobe Workfront MCP伺服器
description: 設定您的Workfront執行個體和AI代理平台，讓您透過自然語言對話來使用Workfront。
author: Courtney
feature: Get Started with Workfront
source-git-commit: 5592c1b93b5e44c732f92d626ed878d2c4647ceb
workflow-type: tm+mt
source-wordcount: '1769'
ht-degree: 0%

---


# 設定Adobe Workfront MCP伺服器

<span class="preview">此頁面上的資訊是指尚未普遍提供的功能。 它只能在「預覽Sandbox」環境中使用。</span>

[!DNL Adobe Workfront] MCP伺服器可讓您在支援的AI代理程式平台上，透過自然語言對話處理您的Workfront資料。

在您可以將AI代理平台連線到Workfront之前，Workfront管理員必須在您的Workfront執行個體中啟用MCP伺服器存取。 每個支援的AI代理平台連線AI代理平台的確切步驟不同。

>[!IMPORTANT]
>
>目前，Workfront MCP伺服器僅供使用AWS的客戶使用。 使用GCP或Azure的客戶將能在不久的將來使用Workfront MCP功能。

## 支援的AI代理平台

Workfront MCP伺服器可與任何支援模型內容通訊協定(MCP)的AI代理平台搭配使用。

本文將逐步說明下列專案的連線步驟：

* [!DNL Claude]
* [!DNL ChatGPT]

如果您使用其他MCP相容的AI代理平台（例如，[!DNL Gemini]或[!DNL Microsoft Copilot]），請依照該平台檔案中的步驟新增自訂MCP伺服器。 當系統提示您輸入MCP伺服器URL時，請輸入您地區的URL：

| 區域 | URL |
| --- | --- |
| 美國 | `https://mcp.workfront.adobe.com/mcp/v1/workfront` |
| 歐盟 | `https://mcp-eu.workfront.adobe.com/mcp/v1/workfront` |

## 先決條件

在將Workfront連線至AI代理平台之前，您必須：

* 擁有使用中的[!DNL Adobe Workfront]帳戶，該帳戶具有存取您要使用之資料的許可權
* 存取類似[!DNL Claude]的AI代理平台
* 您的Workfront執行個體必須在Adobe Identity Management系統(IMS)上啟用。
* 若要搭配Workfront Planning使用MCP，您的組織必須位於包含Adobe Workfront Planning的Workfront套件上。


### 管理員必要條件

MCP伺服器存取許可權由兩個不同的管理員所控制。

* 您的Workfront管理員可透過系統偏好設定中的兩個切換，控制Workfront執行個體的MCP伺服器存取： **唯讀MCP工具** （預設為啟用）和&#x200B;**寫入MCP工具** （預設為停用）。 如果您可以透過AI代理平台找到Workfront專案，但無法建立、更新或刪除它們，請要求Workfront管理員啟用寫入動作。

  如需詳細資訊，請參閱[設定系統偏好設定](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md)。

* 如果您使用AI代理平台的企業版，該平台的管理員必須為您的組織啟用[!DNL Adobe Workfront]聯結器，或為您提供連線至Workfront MCP伺服器的自訂URL存取權。


## 將Workfront連線至Claude

您針對每個[!DNL Claude]帳戶連線至Workfront一次。 連線會針對特定Workfront執行個體驗證您的身分，而且您會保持連線，直到您選擇中斷連線為止。



### 從聯結器目錄連線到Claude案頭

>[!IMPORTANT]
>
>目前，Claude Connector僅支援連線至美國地區的Workfront MCP伺服器。  若要連線到歐盟地區的Workfront執行個體，請參閱本文中的[使用URL連線到Claude](#connect-to-claude-with-a-url)。

+++ 展開以檢視將Workfront連線到[!DNL Claude]的逐步指示。

若要將Workfront連線至[!DNL Claude]：

1. 開啟[!DNL Claude]。

1. 瀏覽至聯結器區域。



1. 在聯結器清單中尋找&#x200B;**[!DNL Adobe Workfront]**。

   如果沒有看見，請參閱本文中的[管理員必要條件](#admin-prerequisites)。

1. 按一下&#x200B;**連線**。



1. 出現提示時，請登入您的Workfront執行個體。


1. 驗證完成之後，就會連線。



+++

### 使用URL連線到Claude

+++ 展開以檢視使用URL將Workfront連線至[!DNL Claude]的逐步指示。

>[!NOTE]
>
>您必須是企業Claude環境中的擁有者才能執行此程式。
>
>如需Claude關於擁有者需求的陳述，請參閱Claude檔案中的[新增自訂聯結器](https://support.claude.com/en/articles/11175166-get-started-with-custom-connectors-using-remote-mcp#:~:text=Note%3A%20While,has%20access%20to)。

若要使用URL將Workfront連線至[!DNL Claude]：

1. 使用您的認證登入[Claude](https://claude.ai)。
1. 在左側功能表中，選取&#x200B;**自訂**&#x200B;圖示。
1. 選取&#x200B;**聯結器**，然後選取&#x200B;**+**&#x200B;圖示以新增聯結器。
1. 選取&#x200B;**建立應用程式**&#x200B;按鈕。
1. 為聯結器指定所需的名稱（例如「Workfront」），然後輸入所需的MCP伺服器URL：

   | 區域 | URL |
   | --- | --- |
   | 美國 | `https://mcp.workfront.adobe.com/mcp/v1/workfront` |
   | 歐盟 | `https://mcp-eu.workfront.adobe.com/mcp/v1/workfront` |

1. 建立聯結器後，會彈出登入視窗。 使用您的Adobe ID憑證進行驗證。 如果您屬於多個Workfront執行個體，請務必選取所需執行個體。

   >[!NOTE]
   >
   >您的Workfront執行個體必須連線到該執行個體所在地區的MCP伺服器。 例如，EU執行個體必須連線至EU MCP伺服器。
   >
   >選取執行個體時，與MCP伺服器區域不相容的執行個體會顯示為灰色，您無法連線到它們。
   >
   >若要連線到與MCP伺服器區域不相容的執行個體，請為該區域設定一個具有正確URL的新MCP連線。

+++

### 使用技能自訂Claude行為

[!DNL Claude]支援使用者建立的指令集，稱為技能。 您可以使用技能來自訂[!DNL Claude]在Workfront中的行為方式。 例如，您可以建立一項技能，告訴[!DNL Claude]永遠從Workfront擷取最新資料，而不是依賴較早的結果。

若要進一步瞭解[!DNL Claude]技能，請參閱[Claude使用者檔案](https://code.claude.com/docs/en/skills)或向Claude尋求技能方面的協助。

## 連線到ChatGPT

1. 使用您的認證登入[ChatGPT](https://chatgpt.com)。
1. 在左下方，選取&#x200B;**您的名稱** → **設定**。
1. 選取&#x200B;**應用程式**，然後啟用&#x200B;**開發人員模式**。
1. 選取&#x200B;**建立應用程式**&#x200B;按鈕。
1. 為應用程式指定所需的名稱（例如「Workfront」），然後輸入所需的MCP伺服器URL：

   | 區域 | URL |
   | --- | --- |
   | 美國 | `https://mcp.workfront.adobe.com/mcp/v1/workfront` |
   | 歐盟 | `https://mcp-eu.workfront.adobe.com/mcp/v1/workfront` |

1. 確定驗證已設定為&#x200B;**OAuth** （預設為設定），並選取接受核取方塊以繼續。
1. 建立應用程式後，系統會隨即顯示登入視窗。 使用您的Adobe ID憑證進行驗證。 如果您屬於多個Workfront執行個體，請務必選取所需執行個體。

   >[!NOTE]
   >
   >您的Workfront執行個體必須連線到該執行個體所在地區的MCP伺服器。 例如，EU執行個體必須連線至EU MCP伺服器。
   >
   >選取執行個體時，與MCP伺服器區域不相容的執行個體會顯示為灰色，您無法連線到它們。
   >
   >若要連線到與MCP伺服器區域不相容的執行個體，請為該區域設定一個具有正確URL的新MCP連線。


### 使用自訂GPT自訂ChatGPT行為

ChatGPT支援使用者建立的助理，稱為自訂GPT。 您可以使用自訂GPT來自訂ChatGPT與聯結器的行為方式。 例如，您可以建立自訂GPT，告訴ChatGPT一律從連線的服務擷取最新資料，而非依賴先前的結果。

若要深入瞭解自訂GPT，請參閱[ChatGPT使用者檔案](https://help.openai.com/en/articles/8554397-creating-and-editing-gpts)，或向ChatGPT尋求自訂GPT的協助。

## 驗證您的連線

若要確認AI代理平台已連線至Workfront，請要求AI代理平台列出Workfront MCP伺服器可供使用的動作。 例如：

* *您可以執行哪些Workfront動作？*
* *列出您有權存取的Workfront工具。*

您也可以在[Adobe Workfront MCP伺服器工具](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-tools.md)中檢視完整的工具清單。

## 可用的工具

Workfront MCP伺服器會公開連線的AI代理平台代表您呼叫的一組工具，例如搜尋Workfront、建立專案、更新欄位和管理核准的工具。 如需依Workfront區域分組的完整參考清單，請參閱[Adobe Workfront MCP伺服器工具](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-tools.md)。

## 切換至其他Workfront執行個體

每個連線都會驗證單一Workfront執行個體的AI代理平台。 若要使用不同的執行個體，請中斷連線並重新連線。

若要連線至其他Workfront執行個體：

1. 在AI代理平台中，中斷Workfront MCP伺服器的連線。
1. 重新連線聯結器。
1. 驗證至新的Workfront執行個體。

>[!NOTE]
>
>* 單獨登出不會切換Workfront執行個體。 您必須中斷連線並重新連線聯結器。
>
>* 您的Workfront執行個體必須連線到該執行個體所在地區的MCP伺服器。 例如，EU執行個體必須連線至EU MCP伺服器。
>
>   選取執行個體時，與MCP伺服器區域不相容的執行個體會顯示為灰色，您無法連線到它們。
>
>   若要連線到與MCP伺服器區域不相容的執行個體，請為該區域設定一個具有正確URL的新MCP連線。


<!--

## Connect to Gemini

>[!IMPORTANT]
>
>You must be an administrator on the Gemini platform to set up the MCP server. If you aren't an administrator, share these instructions with your administrator so they can set up the connection for you.


To set up the connection between Gemini and the Workfront MCP server, follow the instructions provided by Google for [connecting Gemini to external tools using MCP](https://docs.cloud.google.com/gemini/enterprise/docs/connectors/custom-mcp-server/set-up-custom-mcp-server). 

When prompted for the MCP Server URL, enter the following URL for your Workfront MCP server:  

   | Region | URL |
   | --- | --- |
   | US | `https://mcp.workfront.adobe.com/mcp/v1/workfront` |
   | EU | `https://mcp-eu.workfront.adobe.com/mcp/v1/workfront` |
   
-->

<!--
## Connect to Microsoft Copilot

✅ 1) Copilot Studio (most common for agents / enterprise use)
This is the cleanest "paste a URL" flow.
Steps
1. Open your Copilot Studio agent
2. Go to Tools
3. Click:
    * Add a tool → New tool → Model Context Protocol
4. In the wizard, fill in:
    * Server name (anything)
    * Server description
    * ✅ Server URL (your MCP endpoint)
5. Choose auth (if needed):
    * None / API key / OAuth
6. Click Create
👉 That's it—your MCP server is now attached to the agent.
This flow is explicitly documented:
* You add MCP via Tools → Add tool → Model Context Protocol
* Then provide Server name, description, and URL ￼
￼
What happens next
* Copilot discovers tools automatically from the MCP server
* You can enable/disable tools per agent
* The agent calls them when relevant

-->

## 疑難排解設定和驗證

+++ 展開以檢視Workfront MCP伺服器設定和驗證的疑難排解提示。

| 問題 | 可能的原因 | 修正 |
| --- | --- | --- |
| 您在[!DNL Claude]中找不到[!DNL Adobe Workfront]聯結器。 | 您的[!DNL Claude]管理員尚未啟用它。 | 請連絡您的[!DNL Claude]系統管理員（非Workfront系統管理員），要求他們啟用[!DNL Adobe Workfront]聯結器。 |
| 您已連線，但看不到資料。 | 您已驗證錯誤的Workfront執行個體。 | 中斷聯結器的連線，重新連線，並驗證至正確的執行個體。 |
| 驗證失敗，或連線已停止運作。 | 您的驗證工作階段已過期或發生連線錯誤。 | 中斷連線並重新連線聯結器。 |
| 您想要切換至不同的Workfront執行個體。 | 單一連線會將您連結至一個執行個體。 | 中斷新執行個體的連線、重新連線及驗證。 |
| 您無法連線至Workfront，或看到訊息顯示MCP伺服器存取已停用。 | 您的Workfront管理員已關閉您執行個體的MCP伺服器存取權。 | 請連絡您的Workfront管理員，要求他們在「系統偏好設定」中啟用MCP伺服器存取。 |
| 您要連線的Workfront執行個體會呈現灰色，而您會看到一則訊息，指出該執行個體無法在您的地區連線 | 您的MCP伺服器是針對執行個體以外的不同地區（歐盟或美國）設定的。 | 使用指派您的Workfront執行個體所在地區的URL設定MCP伺服器。 |
| AI代理平台可以找到您的Workfront專案，但無法建立、更新或刪除它們。 | 您的Workfront管理員已停用Workfront MCP伺服器的寫入動作。 | 請連絡您的Workfront管理員，並要求他們啟用「系統偏好設定」中的寫入動作。 |

如需連線後的日常疑難排解（例如，過時結果或意外的行為），請參閱[使用Adobe Workfront MCP伺服器](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md)。


+++

## 關於設定的常見問題

+++ 展開以檢視關於設定Workfront MCP伺服器的常見問題。

### 我可以同時連線到多個Workfront執行個體嗎？

否。 每個連線都會將AI代理平台繫結至單一Workfront執行個體。 若要切換、中斷連線並重新連線，驗證新執行個體。

### 哪位管理員會啟用此功能？

您的Workfront管理員和AI代理平台的管理員。 您的Workfront管理員會在Workfront端啟用MCP伺服器存取權。 您的AI代理平台管理員可在該平台側啟用Workfront存取權。 對於[!DNL Claude]，[!DNL Claude]企業管理員會啟用[!DNL Adobe Workfront]聯結器。

### 如果Workfront Identity Management System (IMS)上未啟用我的Workfront執行個體，我可以使用Adobe MCP伺服器嗎？

否。 您的Workfront執行個體必須在Adobe Identity Management系統(IMS)上啟用，才能使用Workfront MCP伺服器。 如果您不確定您的執行個體是否已在IMS上啟用，請聯絡您的Workfront管理員。

+++ 

