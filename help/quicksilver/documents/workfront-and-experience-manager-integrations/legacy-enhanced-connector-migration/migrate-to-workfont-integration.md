---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 從舊版或增強型聯結器移轉至Workfront以進行Adobe Experience Manager as a Cloud Service整合
description: 本頁上的資訊說明從Experience Cloud增強型或舊版聯結器的Workfront移至連線Workfront和Adobe Experience Manager Assets as a Cloud Service的最新原生整合的最佳實務。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: af14f408-df39-473c-9e18-bb88022c96ed
source-git-commit: f381b37e6d4537e6f83e55ed4a2f4ff7f868dd54
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---

# 從舊版或增強型聯結器移轉至Workfront以進行Adobe Experience Manager as a Cloud Service整合

本頁上的資訊說明從Experience Cloud增強型或舊版聯結器的Workfront移至連線Workfront和Adobe Experience Manager Assets as a Cloud Service的最新原生整合的最佳實務。

>[!IMPORTANT]
>
>此資訊不適用於使用Adobe Experience Manager Assets內部部署或Managed Services環境的客戶。

## 將您的Workfront執行個體移至Admin Console

>[!IMPORTANT]
>
>由於所有Workfront組織皆已移轉至Adobe Admin Console，因此本節將於近期移除。

<!--DELETE THIS SECTION MARCH 2026-->

<!--
Customers that intend to use the new native integration between Workfront and Adobe Experience Manager Assets as a Cloud Service must ensure their Workfront environment is tied to an Adobe Admin Console. For existing Workfront environments, this will likely require a migration of the environment to a connected Adobe Admin Console. For more details regarding this migration and the associated checklist, see [Prepare to onboard your organization to the Adobe Admin Console](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md). 

 Adobe must help carry out this migration. To request help, do one of the following:

* If you have Workfront Hub access, submit your request to the [Workfront Migration to Adobe Admin Console](https://hub.workfront.com/requests/new?activeTab=tab-new-helpRequest&projectID=629674d500054a38133cf26e01d06a97&path=).
* If you do not have Workfront Hub access, you can submit your request to the [Workfront to Adobe Admin Console Early Migration Request Queue](https://workfront.az1.qualtrics.com/jfe/form/SV_9T5LuHf05JUOPAi).

-->

## 設定新的Workfront以進行Adobe Experience Manager資產as a Cloud Service整合

將您的Workfront環境移轉至Adobe Admin Console後，Workfront管理員可以設定新的原生整合。 如需設定說明，請參閱[設定Experience Manager Assets as a Cloud Service整合](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md)。

## 將現有資產移至Workfront，以進行Adobe Experience Manager資產as a Cloud Service整合

設定環境後，您可以將現有的連結資產和資料夾移至Adobe Experience Manager。 此為選用步驟，但將確保解除安裝先前透過舊版或增強型聯結器連結的資料夾和資產後，仍可存取。

如需有關移動資產的詳細資訊，請參閱[移轉連結的資料夾和檔案](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md)。

## 驗證所有擬使用的關鍵使用案例

在解除安裝舊版或增強型聯結器之前，請務必驗證擬透過原生整合使用的所有關鍵使用案例。

## 解除安裝舊版或增強型聯結器

最後，您必須解除安裝舊版或增強型聯結器。 原生整合併非打算與任一聯結器同時執行。

若要解除安裝，請參閱

* 舊版聯結器解除安裝指示： [使用Adobe Experience Manager舊版聯結器解除安裝Workfront](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md)。
* 增強聯結器解除安裝指示： [使用Adobe Experience Manager增強聯結器解除安裝Workfront](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-enhanced-connector.md)。
