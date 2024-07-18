---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 從舊版聯結器移轉至增強型聯結器
description: 下列程式概述將Adobe Experience Manager舊版聯結器移出為增強型聯結器以將Adobe Workfront與AEM Assets整合的最佳做法。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4a8d1e2b-9744-4f72-a337-5057448db4fb
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---

# 從舊版聯結器移轉至增強型聯結器

下列程式概述將Adobe Experience Manager舊版聯結器移出為增強型聯結器以將Adobe Workfront與AEM Assets整合的最佳做法。

>[!IMPORTANT]
>
>本檔案僅適用於使用Adobe Experience Manager Assets內部部署或Managed Services環境的客戶。


若客戶使用Adobe Experience Manager Assetsas a Cloud Service，舊版聯結器的移轉路徑將為Workfront內的全新原生整合。 若要深入瞭解此移轉程式，請參閱[從舊版或增強型聯結器移轉至Workfront以進行Adobe Experience Manager as a Cloud Service整合](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/migrate-from-legacy-enhanced-connectors.md)。

## 實作增強型聯結器

>[!IMPORTANT]
>
>實作增強型聯結器需要認證合作夥伴或Adobe Consulting服務。
>
> 對於希望認證增強型聯結器的合作夥伴，請檢閱下列文章： [Workfront for Experience Manager增強型聯結器專家系列](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/workfront/enhanced-connector/aem-experts-series/overview.html?lang=en)。

若要實作增強型聯結器，請參閱[為Experience Manager增強型聯結器設定Workfront](https://experienceleague.adobe.com/docs/experience-manager-65/assets/integrations/workfront-connector-configure.html?lang=en)。


## 移動現有資產

設定環境後，您可以將現有的連結資產和資料夾移至Adobe Experience Manager。 此為選用步驟，但將確保在解除安裝舊版聯結器後，先前透過舊版聯結器連結的資料夾和資產仍可存取。

如需有關移動資產的詳細資訊，請參閱[移轉連結的資料夾和檔案](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md)。

## 驗證所有擬使用的關鍵使用案例

在解除安裝舊版聯結器之前，請務必驗證所有擬透過增強型聯結器使用的關鍵使用案例。

## 解除安裝舊版聯結器

最後，您必須解除安裝舊版聯結器。 舊版聯結器並非旨在與增強型聯結器同時執行。

若要解除安裝，請參閱[使用Adobe Experience Manager舊版聯結器解除安裝Workfront](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md)。
