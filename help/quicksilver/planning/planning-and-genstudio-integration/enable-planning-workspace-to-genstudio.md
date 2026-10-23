---
title: 在GenStudio for Performance Marketing中啟用Workfront規劃Workspace
description: 如果您已在Adobe Workfront Planning中擁有工作區，則可為GenStudio for Performance Marketing啟用它，而非重新建立資料。
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 0747fb80-496f-41c0-b469-1203e1605f05
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/wHSc0Neshdl-Owh1siw72wdO-H1hnEPy-dAk91tDOrI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 0bcb6ef2abbf3789339af27119422ef413cd6eef
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 2%
---
# 啟用Workfront規劃工作區至GenStudio for Performance Marketing

{{planning-important-intro}}

<!-- THIS IS HIDDEN FROM TOC-->

<!--
Better metadata, at publishing:
---
title: Promote a Workfront Planning workspace to GenStudio
description: The GenStudio for Performance Marketing workspace is available in Adobe Workfront Planning when your company has purchased both products and your instance of Workfront is integrated with your company's instance of GenStudio. You can promote a Workfront Planning workspace to GenStudio and have its information visible and updated from both systems.
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
---
-->
除了Workfront Planning之外，如果貴公司也購買Adobe GenStudio for Performance Marketing，則當您的GenStudio執行個體與貴公司的Adobe Workfront執行個體整合時，GenStudio Planning中會提供Workfront工作區。

如果您已在Workfront Planning中擁有工作區，則可為GenStudio啟用它，而非重新建立資料。

啟用工作區可將其連結至Adobe儲存專案，並將其記錄型別和欄位對應至GenStudio工作區結構描述。 完成設定後，您可以在GenStudio中開啟工作區的記錄。

考慮以下事項：

* 您必須同時擁有Workfront Planning和GenStudio for Performance Marketing的存取權。
* 您必須擁有Adobe雲端儲存空間專案，才能連結至工作區。 組織管理員可以在Adobe Admin Console中建立一個。

  如需詳細資訊，請參閱[管理Adobe儲存空間](https://helpx.adobe.com/business/enterprise/manage-storage-assets/manage-storage/manage-adobe-storage.html)。<!--ensure this site still works-->


## 啟用Workfront規劃工作區至GenStudio

1. 在Workfront Planning中，開啟您要啟用的工作區。
1. 按一下工作區名稱右側的&#x200B;**更多**&#x200B;功能表![更多功能表](assets/more-menu.png)，然後按一下&#x200B;**啟用GenStudio**。

   **讓工作區GenStudio**&#x200B;啟用方塊開啟，包括以下步驟：

   1. **ACPC專案**：選取您要與此工作區同步的&#x200B;**ACPC專案** （Adobe雲端儲存空間專案），然後按一下[下一步]**。**&#x200B;使用者可透過此專案存取GenStudio中的工作區。

      ![啟用工作區GenStudio - ACPC專案步驟](assets/make-workspace-genstudio-enabled-box-acpc-step.png)

   1. **記錄型別**：將工作區的記錄型別對應到GenStudio所需的六種記錄型別：

      * 行銷活動
      * 產品
      * 人物誌
      * 管道
      * 區域
      * 啟用

      請針對每個專案，開啟清單並選取相符的Planning記錄型別，或選取&#x200B;**新增**&#x200B;以建立它，然後按一下&#x200B;**下一步**。

      ![啟用工作區GenStudio — 記錄型別步驟](assets/make-workspace-genstudio-enabled-box-record-types-step.png)

   1. **欄位**：對應每個記錄型別的欄位。 使用對話方塊頂端的索引標籤，在記錄型別之間移動。 對於每個欄位，選取相符的Planning欄位，或選取&#x200B;**新增**&#x200B;以建立它。

      對所有記錄型別重複欄位設定。

      ![啟用工作區GenStudio — 欄位步驟](assets/make-workspace-genstudio-enabled-box-fields-step.png)

   1. 檢閱並解決任何警告。

      例如，新欄位可以成為記錄型別的主要欄位，或者已使用的欄位別名已重新命名（如果您已經有名為「Regions」的欄位，則匯入的欄位可能會變成「Regions 2」）。

      對應&#x200B;**狀態**&#x200B;欄位會新增必要選項。

   1. 點擊&#x200B;**發佈**。

      工作區啟用時會顯示確認訊息。 對應記錄型別會在工作區中標示。

      對應為可從GenStudio存取的記錄型別卡片上有新的&#x200B;**Adobe**&#x200B;圖示。

      ![具有Adobe圖示的行銷活動記錄型別](assets/campaigns-record-type-card-with-adobe-icon.png)

1. 開啟GenStudio，選取&#x200B;**行銷活動**，然後按一下畫面左下角您為此設定所原始設定的&#x200B;**ACPC專案**。 檢閱匯入的記錄型別和欄位。

   >[!TIP]
   >
   >您只會看到ACPC專案成員資格允許的記錄。
