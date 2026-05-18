---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: 設定Adobe Workfront MCP伺服器
description: 設定您的Workfront執行個體和AI助理，讓您透過自然語言對話來使用Workfront。
author: Courtney
feature: Get Started with Workfront
hide: true
source-git-commit: 4517d45ecc653d27d435a8192a612241120dd33f
workflow-type: tm+mt
source-wordcount: '693'
ht-degree: 3%

---


# 設定Adobe Workfront MCP伺服器

[!DNL Adobe Workfront] MCP伺服器可讓您在受支援的AI助理（如Claude或ChatGPT）中，透過自然語言對話處理Workfront資料。

在您可以將AI助理連線到Workfront之前，Workfront管理員必須在您的Workfront執行個體中啟用MCP伺服器存取。 每個支援的AI助理連線到AI助理的確切步驟不同。

如需Workfront MCP伺服器的詳細資訊，請參閱[Adobe Workfront MCP伺服器概述](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-overview.md)。

## 支援的AI助理

Workfront MCP伺服器目前支援下列AI助理：

* [!DNL Claude]

<!-- NEEDS DETAIL: Update this list as Adobe adds support for additional AI assistants (for example, [!DNL Gemini], or [!DNL Microsoft Copilot]). -->

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 封裝</td> 
   <td><p><!-- NEEDS DETAIL: Confirm Workfront package requirement (Select, Prime, Ultimate, Any?) --></p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p><!-- NEEDS DETAIL: Confirm Workfront license requirement (Standard, Work, etc.) --></p></td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

在將Workfront連線至AI助理之前，您必須：

* 擁有使用中的[!DNL Adobe Workfront]帳戶，該帳戶具有存取您要使用之資料的許可權。
* 擁有[!DNL Claude]等AI助理的存取權。

  <!-- NEEDS DETAIL: Confirm which Claude tiers are supported. Claude Enterprise is confirmed; Claude Pro and Claude Team support is unconfirmed. -->

### 管理員必要條件

MCP伺服器存取許可權由兩個不同的管理員所控制。 兩者都必須啟用存取，才能連線。

* **您的Workfront管理員**&#x200B;必須在Workfront執行個體中啟用MCP伺服器存取權。

* 如果您使用企業版的AI助理員，您的AI助理管理員必須為您的組織啟用[!DNL Adobe Workfront]聯結器。


## 將Workfront連線至Claude

您針對每個[!DNL Claude]帳戶連線至Workfront一次。 連線會針對特定Workfront執行個體驗證您的身分，而且您會保持連線，直到您選擇中斷連線為止。


>[!IMPORTANT]
>
>如果您使用[!DNL Claude] Enterprise，**您的[!DNL Claude] Enterprise系統管理員**&#x200B;必須為您的組織啟用[!DNL Adobe Workfront]聯結器。 在這之前，當您在[!DNL Claude]中搜尋[!DNL Adobe Workfront]聯結器時，該聯結器將不會顯示。 請先連絡您的[!DNL Claude]系統管理員。


若要將Workfront連線至[!DNL Claude]：

1. 開啟[!DNL Claude]。

1. 瀏覽至聯結器區域。

   <!-- NEEDS DETAIL: Exact menu path (for example, "Click Settings, then click Connectors"). -->

1. 在聯結器清單中尋找&#x200B;**[!DNL Adobe Workfront]**。

   如果沒有看見，請參閱本文中的[管理員必要條件](#admin-prerequisites)。

1. 按一下&#x200B;**連線**。

   <!-- NEEDS DETAIL: Confirm the exact button label. -->

1. 出現提示時，請登入您的Workfront執行個體。

   <!-- NEEDS DETAIL: Describe the auth flow — does it open a new browser tab, an in-app window, prompt for a Workfront domain? -->

1. 驗證完成之後，就會連線。

   <!-- NEEDS DETAIL: Add a screenshot of the connected state in Claude. -->

### 驗證您的連線

若要確認[!DNL Claude]已連線至Workfront，請要求[!DNL Claude]列出Workfront MCP伺服器可供使用的動作。 例如：

* *您可以執行哪些Workfront動作？*
* *列出您有權存取的Workfront工具。*

[!DNL Claude]會傳回可用動作的清單。

<!-- NEEDS DETAIL: Add a screenshot of the tool-list response. -->

### 切換至其他Workfront執行個體

每個連線都會驗證單一Workfront執行個體的[!DNL Claude]。 若要使用不同的執行個體，請中斷連線並重新連線。

若要連線至其他Workfront執行個體：

1. 在[!DNL Claude]中，中斷[!DNL Adobe Workfront]聯結器的連線。
1. 重新連線聯結器。
1. 驗證至新的Workfront執行個體。

>[!NOTE]
>
>單獨登出[!DNL Claude]並不會切換Workfront執行個體。 您必須中斷連線並重新連線聯結器。

## 使用技能自訂Claude行為

<!-- NEEDS DETAIL: Confirm whether Adobe is shipping any pre-built Claude skills alongside the MCP server. If yes, list them and link to download or installation guidance. If no, decide whether to mention skills as a user-driven workaround at all, or remove this section. -->

[!DNL Claude]支援使用者建立的指令集，稱為技能。 您可以使用技能來自訂[!DNL Claude]在Workfront中的行為方式。 例如，您可以建立一項技能，告訴[!DNL Claude]永遠從Workfront擷取最新資料，而不是依賴較早的結果。

## 疑難排解設定和驗證

| 問題 | 可能的原因 | 修正 |
|---|---|---|
| 您在[!DNL Claude]中找不到[!DNL Adobe Workfront]聯結器。 | 您的[!DNL Claude]管理員尚未啟用它。 | 請連絡您的[!DNL Claude]系統管理員（非Workfront系統管理員），要求他們啟用[!DNL Adobe Workfront]聯結器。 |
| 您已連線，但看不到資料。 | 您已驗證錯誤的Workfront執行個體。 | 中斷聯結器的連線，重新連線，並驗證至正確的執行個體。 |
| 驗證失敗，或連線已停止運作。 | 您的驗證工作階段已過期或發生連線錯誤。 | 中斷連線並重新連線聯結器。 |
| 您想要切換至不同的Workfront執行個體。 | 單一連線會將您連結至一個執行個體。 | 中斷新執行個體的連線、重新連線及驗證。 |

<!-- NEEDS DETAIL: Add additional setup/authentication troubleshooting scenarios discovered during hands-on testing. -->

如需連線後的日常疑難排解（例如，過時結果或意外的行為），請參閱[使用Adobe Workfront MCP伺服器](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md)。

## 關於設定的常見問題

### 我可以一次連線到多個Workfront執行個體嗎？

否。 每個連線都會將AI助理繫結至單一Workfront執行個體。 若要切換、中斷連線並重新連線，驗證新執行個體。

### 這適用於Claude Pro或Claude Team，還是僅適用於Claude Enterprise？

<!-- NEEDS DETAIL: Confirm Claude tier support and answer this directly. -->

### 哪位管理員會啟用此功能？

Workfront管理員和AI助理管理員。 您的Workfront管理員會在Workfront端啟用MCP伺服器存取權。 您的AI助理管理員會在AI助理端啟用Workfront存取權。 對於[!DNL Claude]，[!DNL Claude]企業管理員會啟用[!DNL Adobe Workfront]聯結器。
