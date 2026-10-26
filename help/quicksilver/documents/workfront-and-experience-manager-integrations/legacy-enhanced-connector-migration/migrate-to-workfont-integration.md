---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 從舊版或增強型聯結器移轉至Workfront以進行Adobe Experience Manager as a Cloud Service整合
description: 本頁資訊說明從適用於Experience Cloud增強型或舊版聯結器的Workfront移至連線Workfront和Adobe Experience Manager Assets as a Cloud Service的最新原生整合的最佳做法。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: af14f408-df39-473c-9e18-bb88022c96ed
TQID: 'https://experienceleague.adobe.com/0pAHfS7cDqv1tV4TBdx9WqvJA1-zySGsPHVXI8EG7Hc'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
  - id: a1f87682-0525-5459-aa06-3560bb4c3b2a
    internal-label: Workfront Integrations and Apps
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: e7123179a59cd7ed9c76f4718b3b8019854cbfe1
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%
---
# 從舊版或增強型聯結器移轉至Workfront以進行Adobe Experience Manager as a Cloud Service整合

本頁資訊說明從適用於Experience Cloud增強型或舊版聯結器的Workfront移至連線Workfront和Adobe Experience Manager Assets as a Cloud Service的最新原生整合的最佳做法。

>[!IMPORTANT]
>
>此資訊不適用於使用Adobe Experience Manager Assets內部部署或Managed Services環境的客戶。

<!--

## Move your Workfront instance to the Admin Console

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
