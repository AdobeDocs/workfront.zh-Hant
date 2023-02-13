---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 從舊版或增強的連接器移轉至Workfront for Adobe Experience Manager as a Cloud Service整合
description: 本頁的資訊說明從Workfront移轉至Experience Cloud增強或舊版連接器的最佳作法，以及將Workfront與Adobe Experience Manager資產as a Cloud Service連結的最新原生整合。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: af14f408-df39-473c-9e18-bb88022c96ed
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---

# 從舊版或增強的連接器移轉至Workfront for Adobe Experience Manager as a Cloud Service整合

本頁的資訊說明從Workfront移轉至Experience Cloud增強或舊版連接器的最佳作法，以及將Workfront與Adobe Experience Manager資產as a Cloud Service連結的最新原生整合。

>[!IMPORTANT]
>
>使用Adobe Experience Manager Assets On-Premise或Managed Services環境的客戶不適用此資訊。

## 將您的Workfront執行個體移至Admin Console

客戶若想在Workfront和Adobe Experience Manager Assets之間使用新的原生整合，必須as a Cloud Service確保其Workfront環境已系結至Adobe Admin Console。 若為現有的Workfront環境，這可能需要將環境移轉至已連線的Adobe Admin Console。 如需有關此移轉的詳細資訊以及相關檢查清單，請參閱 [準備將貴組織上線至Adobe Admin Console](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md).

Adobe必須協助執行此移轉。 要請求幫助，請執行以下操作之一：

* 如果您有Workfront中樞存取權，請將請求提交至 [Workfront移轉至Adobe Admin Console](https://hub.workfront.com/requests/new?activeTab=tab-new-helpRequest&amp;projectID=629674d500054a38133cf26e01d06a97&amp;path=).
* 如果您沒有Workfront中樞存取權，可以將請求提交至 [Workfront至Adobe Admin Console提早移轉請求佇列](https://workfront.az1.qualtrics.com/jfe/form/SV_9T5LuHf05JUOPAi).

## 設定新的Workfront for Adobe Experience Manager assetsas a Cloud Service整合

將Workfront環境移轉至Adobe Admin Console後，Workfront管理員就可以設定新的原生整合。 如需設定說明，請參閱 [設定Experience Manager Assetsas a Cloud Service整合](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).

## 將現有資產移至Workfront以進行Adobe Experience Manager資產as a Cloud Service整合

設定環境後，您可以將現有的連結資產和資料夾移至Adobe Experience Manager。 這是選用的步驟，但可確保在解除安裝這些連接器後，仍可透過舊版或增強連接器存取先前連結的資料夾和資產。

如需移動資產的詳細資訊，請參閱 [遷移連結的資料夾和文檔](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md).

## 驗證所有要使用的重要使用案例

在解除安裝舊式或增強連接器之前，請務必驗證所有透過原生整合使用的重要使用案例。

## 卸載舊連接器或增強連接器

最後，您需要解除安裝舊連接器或增強連接器。 本機整合不打算與任一連接器並行執行。

若要解除安裝，請參閱

* 舊版連接器解除安裝指示： [解除安裝Workfront與Adobe Experience Manager舊連接器](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md).
* 增強的連接器卸載說明： [解除安裝Workfront與Adobe Experience Manager增強連接器](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-enhanced-connector.md).
