---
title: 使用克勞德程式碼技能建置App Builder應用程式
description: 使用一組Claude程式碼技能，透過描述您想要的方式建置自訂Adobe Workfront App Builder應用程式，而非自行執行設定和部署步驟。
author: Becky
feature: Digital Content and Documents
hide: true
source-git-commit: e5a288dcac20be9176d1541d531edaf0d8c99a8c
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 5%

---


# 使用克勞德程式碼技能建置App Builder應用程式

一組[!DNL Claude Code]技能可讓[!DNL Claude]為[!DNL Workfront]建置自訂[!DNL Adobe App Builder]應用程式。 這表示您可以用純英文描述您想要的內容，而不需要成為開發人員或自己撰寫設定步驟，藉此建立帳戶。

客戶和合作夥伴可以利用由 Adobe App Builder 提供技術支援的 Workfront UI 擴充功能，建立自訂使用者體驗。 UI擴充功能可讓您修改組織的Workfront體驗，以更符合組織的需求，進而提高效率、提供順暢、連結的體驗，並大幅提升使用者滿意度，並幫助您的組織實現其獨特願景。

如需Workfront UI擴充功能的詳細資訊，請參閱[使用Adobe App Builder建立Workfront的自訂應用程式](/help/quicksilver/app-builder/app-builder.md)。

## Claude的UI擴充性技能

在[!DNL Adobe App Builder]上建置可能相當技術性，如果使用者不熟悉程式或技術，這可能會造成障礙。 UI擴充性技能可使用[!DNL Claude]簡化此程式。 您說明了您想要的功能，而[!DNL Claude]會親自執行工作，例如設定工具、在[!DNL Adobe App Builder]中建立專案、建置應用程式、將其部署到Adobe雲端，以及在Workfront中執行。 只有在需要您執行決定的決策或登入動作時，您才會參與此程式。

## 先決條件

開始之前，請確定您擁有：

* 已安裝&#x200B;**[!DNL Claude Code]**。
* **存取技能**。

  * 您可以在[https://github.com/adobe/skills/blob/main/plugins/app-builder/skills/appbuilder-workfront/SKILL.md](https://github.com/adobe/skills/blob/main/plugins/app-builder/skills/appbuilder-workfront/SKILL.md)找到技能。

    如果此連結未為您開啟，請要求您的管理員授予您存取權。
  * 下載技能後，請執行以下命令進行設定。

    ```
    /plugin marketplace add adobe/skills
    ```

    ```
    /plugin install app-builder@adobe-skills
    ```

* **[!DNL Adobe App Builder]存取權，使用開發人員角色**。 您的Adobe組織需要App Builder授權，且您必須在中新增為開發人員。 這可讓[!DNL Claude]開啟Adobe Developer Console並建立您的專案。

  若要檢查是否符合此先決條件：

  1. 開啟 [Adobe Developer Console](https://developer.adobe.com/console)。
  1. 確認右上角顯示的組織正確無誤。
  1. 按一下&#x200B;**建立新專案** > **從範本建立專案**。
  1. 檢查&#x200B;**App Builder**&#x200B;是否出現在清單中。

     * 如果您在清單中看到&#x200B;**App Builder**，則表示您擁有存取權。
     * 如果沒有&#x200B;**從範本建立專案**&#x200B;選項，或沒有&#x200B;**App Builder**&#x200B;選項，則您還沒有存取權。 請要求您的Workfront或Adobe管理員將您新增為開發人員（在「Adobe Admin Console >使用者>開發人員」中），並確認您的組織擁有App Builder授權。
* **已連線Workfront MCP伺服器**，因此[!DNL Claude]會使用真正的Workfront API，而不是在資料型別、欄位和命令上猜測。

  若要檢查Workfront MCP伺服器是否已連線，請詢問[!DNL Claude]： *「您能看到Workfront MCP資源嗎？」*

  如需詳細資訊與指示，請參閱設定Workfront MCP伺服器一文中的[將Adobe Workfront連線到Claude](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#connect-workfront-to-claude)。
