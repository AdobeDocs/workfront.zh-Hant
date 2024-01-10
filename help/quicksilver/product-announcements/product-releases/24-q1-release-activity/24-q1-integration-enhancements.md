---
title: 2024年第一季度整合增強功能
description: 2024年第一季度整合增強功能
author: Becky
feature: Product Announcements
exl-id: 0d581f3c-2aaf-4ac1-97a5-df1b01627080
source-git-commit: 44dd48b72e798b8967c4a4e3dc7d523fe9b130d2
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

# 2024年第一季度整合增強功能

本頁面說明2024年第一季度版本與「預覽」環境配合所做的所有整合增強功能。 這些增強功能將在2024年第一季度版本的生產環境中提供。

如需2024年第一季發行週期目前可用的所有變更清單，請參閱 [2024年第一季版本總覽](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).

## Experience Manager Assets Essentials中的對應中繼資料現在使用 `xcm:keywords` 而非 `dc:subject`

我們已更新Experience Manager Assets Essentials整合，以符合Experience Manager Assetsas a Cloud Service整合的體驗。 現在，將多個單行文字欄位對應到Experience Manager Assets中的單一欄位時，兩種服務都會使用 `xcm:keywords` 欄位。

以前，這些欄位會對應 `dc:subject` 欄位(位於Experience Manager Assets Essentials)。 Experience Manager Assetsas a Cloud Service功能未變更。

目前對應的任何Experience Manager Assets Essentials中繼資料 `dc:subject` 必須重新對應至 `xcm:keywords`.

如需將中繼資料對應至Experience Manager Assets Essentials的相關資訊，請參閱 [AEM關鍵字](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md#aem-keyword).

## Adobe Experience Manager整合現在提供預先輸入欄位

為了更方便在Workfront和Adobe Experience Manager之間連結欄位，我們在中繼資料對應中新增了預先輸入欄位的支援。 現在，您可以將預先輸入欄位對應至Adobe Experience Manager中的對應欄位。

如果使用者為Workfront中的欄位選取不同的值，此變更會立即反映在Adobe Experience Manager中。 此外，如果欄位值選項變更（例如團隊將其名稱變更為新名稱），此變更也會反映在Adobe Experience Manager中。

如需Adobe Experience Manager整合中中繼資料對應的相關資訊和指示，請參閱 [設定中繼資料](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-metadata-optional).

## 在Adobe Experience Manager中自動發佈資產

我們已新增另一個工作流程至Adobe Experience Manager整合。 現在，您可以將資產設定為在傳送至Adobe Experience Manager時自動發佈。 整合可設定為發佈至Adobe Experience Manager發佈服務或Adobe Experience Manager Brand Portal。

自動發佈工作流程可在Adobe Experience Manager整合中啟用和設定。 啟用後，即可在專案範本或專案層級編輯工作流程。

如需詳細資訊，請參閱 [發佈資產](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md#publishing-assets) 在 [在Experience Manager Assets整合中使用工作流程](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md).
