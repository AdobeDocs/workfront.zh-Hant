---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 從舊版或增強型聯結器移轉至Workfront以進行Adobe Experience Manager as a Cloud Service整合
description: 本頁資訊說明從Workfront移轉至Experience Cloud增強型或舊版聯結器的最佳實務，以便最新原生整合連線Workfront和Adobe Experience Manager Assetsas a Cloud Service。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: af14f408-df39-473c-9e18-bb88022c96ed
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 0%

---

# 從舊版或增強型聯結器移轉至Workfront以進行Adobe Experience Manager as a Cloud Service整合

本頁資訊說明從Workfront移轉至Experience Cloud增強型或舊版聯結器的最佳實務，以便最新原生整合連線Workfront和Adobe Experience Manager Assetsas a Cloud Service。

>[!IMPORTANT]
>
>此資訊不適用於使用Adobe Experience Manager Assets內部部署或Managed Services環境的客戶。

## 將您的Workfront執行個體移至Admin Console

如果客戶想要使用Workfront與Adobe Experience Manager Assetsas a Cloud Service之間的全新原生整合，必須確認其Workfront環境已繫結至Adobe Admin Console。 針對現有Workfront環境，這可能需要將環境移轉至連線的Adobe Admin Console。 如需此移轉的相關詳細資訊以及相關的檢查清單，請參閱 [準備將您的組織加入Adobe Admin Console](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md).

Adobe必須協助進行此移轉。 若要請求協助，請執行下列任一項作業：

* 如果您有Workfront中心存取權，請將您的請求提交至 [Workfront移轉至Adobe Admin Console](https://hub.workfront.com/requests/new?activeTab=tab-new-helpRequest&amp;projectID=629674d500054a38133cf26e01d06a97&amp;path=).
* 如果您沒有Workfront中心存取權，可以將請求提交至 [Workfront移轉至Adobe Admin Console早期移轉請求佇列](https://workfront.az1.qualtrics.com/jfe/form/SV_9T5LuHf05JUOPAi).

## 設定新的Workfront以進行Adobe Experience Manager資產的as a Cloud Service整合

將您的Workfront環境移轉至Adobe Admin Console後，Workfront管理員可以設定新的原生整合。 如需設定說明，請參閱 [設定Experience Manager Assetsas a Cloud Service整合](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).

## 將現有資產移至Workfront，以進行Adobe Experience Manager資產的as a Cloud Service整合

設定環境後，您可以將現有的連結資產和資料夾移至Adobe Experience Manager。 此為選用步驟，但將確保解除安裝先前透過舊版或增強型聯結器連結的資料夾和資產後，仍可存取。

如需有關移動資產的詳細資訊，請參閱 [移轉連結的資料夾和檔案](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md).

## 驗證所有擬使用的關鍵使用案例

在解除安裝舊版或增強型聯結器之前，請務必驗證擬透過原生整合使用的所有關鍵使用案例。

## 解除安裝舊版或增強型聯結器

最後，您必須解除安裝舊版或增強型聯結器。 原生整合併非打算與任一聯結器同時執行。

若要解除安裝，請參閱

* 舊版聯結器解除安裝指示： [解除安裝具有Adobe Experience Manager舊版聯結器的Workfront](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md).
* 增強型聯結器解除安裝指示： [解除安裝具有Adobe Experience Manager增強型聯結器的Workfront](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-enhanced-connector.md).
