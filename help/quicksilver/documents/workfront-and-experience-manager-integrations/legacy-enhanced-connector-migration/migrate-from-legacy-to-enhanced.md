---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 從舊式連接器移轉至增強連接器
description: 下列程式概述將Adobe Experience Manager舊連接器移至增強連接器以整合Adobe Workfront與AEM Assets的最佳實務。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4a8d1e2b-9744-4f72-a337-5057448db4fb
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# 從舊式連接器移轉至增強連接器

下列程式概述將Adobe Experience Manager舊連接器移至增強連接器以整合Adobe Workfront與AEM Assets的最佳實務。

>[!IMPORTANT]
>
>本檔案僅適用於使用Adobe Experience Manager Assets On-Premise或Managed Services環境的客戶。


若客戶使用Adobe Experience Manager Assets as a Cloud Service，從舊版連接器移轉至Workfront內的新原生整合路徑。 若要深入了解此移轉程式，請參閱 [從舊版或增強的連接器移轉至Workfront for Adobe Experience Manager as a Cloud Service整合](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/migrate-from-legacy-enhanced-connectors.md).

## 實作增強的連接器

>[!IMPORTANT]
>
>實作增強連接器需要經認證的合作夥伴或Adobe諮詢服務。
>
> 對於希望認證增強型連接器的合作夥伴，請查看以下文章： [Workfront for Experience Manager增強連接器專家系列](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/workfront/enhanced-connector/aem-experts-series/overview.html?lang=en).

若要實作增強連接器，請參閱 [配置Workfront以Experience Manager增強連接器](https://experienceleague.adobe.com/docs/experience-manager-65/assets/integrations/workfront-connector-configure.html?lang=en).


## 移動現有資產

設定環境後，您可以將現有的連結資產和資料夾移至Adobe Experience Manager。 這是選用的步驟，但可確保在解除安裝舊版連接器後，仍可透過舊版連接器存取先前連結的資料夾和資產。

如需移動資產的詳細資訊，請參閱 [遷移連結的資料夾和文檔](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md).

## 驗證所有要使用的重要使用案例

在卸載舊連接器之前，請務必驗證所有打算透過增強連接器使用的重要使用案例。

## 卸載舊連接器

最後，您需要解除安裝舊連接器。 舊連接器不打算與增強連接器並行運行。

若要解除安裝，請參閱 [解除安裝Workfront與Adobe Experience Manager舊連接器](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md).
