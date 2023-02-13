---
user-type: administrator
content-type: overview
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: 藍圖概述
description: Blueprint提供了基本的構建塊，幫助您建立一個隨您而增長的工作管理系統。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4c487598-2066-4507-8dfe-1a54d38f5eea
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 0%

---

# 藍圖概述

Blueprint提供了基本的構建塊，幫助您建立一個隨您而增長的工作管理系統。 系統管理員可以瀏覽藍圖目錄並安裝可供使用的項目模板。 其他使用者可以瀏覽目錄，並要求安裝Blueprint。 如需詳細資訊，請參閱 [瀏覽藍圖目錄並請求安裝藍圖](../../administration-and-setup/blueprints/browse-catalog.md).

每個藍圖都針對某個部門和特定的成熟度級別，以幫助您更快地在系統中實施經驗證的最佳做法。 Blueprint目錄卡和詳細資訊中顯示了以下詳細的成熟度級別。

**[!UICONTROL 受管]:** 托管項目模板有助於在活動和交付件被完全接受為標準程式之前，支援採用新的業務流程。 它們包含任務，以確保新進程的每個步驟都得到遵守。

**[!UICONTROL 整合]:** 整合項目模板假定業務功能通過標準操作程式得到支援。 程式的貢獻者了解他們需要完成的步驟和工作，才能遵循程式。 支援此流程的項目模板包含的任務較少，只能跟蹤里程碑和用於報告目的所需的其他關鍵交付項。

## 找到正確的藍圖

您可以按使用案例、成熟度級別、安裝狀態以及在目錄右側的篩選器中鍵入內容來瀏覽藍圖。 找到您感興趣的藍圖後，您就可以在詳細資訊頁面上查看詳細資訊。

### Blueprint 類型

Blueprint類型會顯示Blueprint中包含的項目。 類型會列在目錄的Blueprint卡底部。 請注意，Blueprint可以有多個類型。

有以下類型的藍圖可用：

* 專案範本：包括與項目模板（任務、問題、角色和團隊）相關聯的標準對象，以及與這些對象相關的一些首選項。 如需詳細資訊，請參閱 [設定Blueprint](../../administration-and-setup/blueprints/configure-template-package.md).
* 組織結構：包括與組織結構（公司、組、角色和團隊）相關聯的對象。 如需詳細資訊，請參閱 [設定Blueprint](../../administration-and-setup/blueprints/configure-template-package.md).
* 控制面板：包含特定使用案例（例如實作服務）的一或多個控制面板。

<!--
* Request queues: Includes one or more projects configured as request queues.
* Custom forms: Includes custom forms attached to another object type, such as a project or portfolio.
* Setup features: Includes one or more elements that are configured in the Setup area of Workfront, such as layout templates.
-->

要查看當前藍圖，請參閱 [可用藍圖清單](/help/quicksilver/administration-and-setup/blueprints/list-of-available-blueprints.md).

### 檢視「」詳細資料

每個Blueprint都包含詳細資訊頁面。 在此頁面中，您可以：

* 檢視工作流程內容的摘要
* 閱讀Blueprint的簡要摘要
* 查看安裝歷史記錄(按一下 **[!UICONTROL 請參閱詳細資訊]** 查看隨Blueprint安裝的對象的完整清單)
* 請參閱角色、團隊、公司和群組說明
* 查看特定Blueprint的視覺範例，例如專案範本（您可以在瀏覽器中預覽完整影像或下載影像）

![[!UICONTROL Blueprint詳細資訊] 頁面](assets/blueprint-details-page-2022.png)

## 安裝Blueprint

系統管理員可以直接在生產環境或沙箱環境中安裝。 若要進一步了解，請參閱 [安裝Blueprint](../../administration-and-setup/blueprints/blueprints-install.md) 或 [設定Blueprint](../../administration-and-setup/blueprints/configure-template-package.md).

安裝後，您可能不確定接下來要採取的最佳動作。 如需詳細資訊，請參閱 [安裝Blueprint後要採取的動作](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

## 有關藍圖和模板的其他說明

Blueprint不替換 [!DNL Adobe Workfront]. Blueprint是您更快建立新模板以組織更多工作的一種方法 [!DNL Workfront].

您無法複製或編輯Blueprint。 不過，從Blueprint安裝解決方案後，您就可以修改從Blueprint建立的專案範本、工作角色或團隊，如同您一般在 [!DNL Workfront] 介面。 此外，安裝Blueprint時，範本會儲存在 [!UICONTROL 範本] 區域 [!DNL Workfront] 而原始的藍圖則留在 [!UICONTROL 藍圖] 的上界。 開始根據您的需求量身打造範本之前，您不需要先製作範本復本。

Blueprint不會刪除或更換環境中配置的任何內容。 如果要通過安裝建立新模板的藍圖來替換現有模板，建議您停用舊版本，以避免從模板構建項目的規劃人員產生混淆。
