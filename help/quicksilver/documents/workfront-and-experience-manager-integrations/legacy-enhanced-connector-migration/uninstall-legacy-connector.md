---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 解除安裝舊版聯結器
description: 文字
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4b3834bf-2e6d-4588-8d77-671e14390115
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 0%

---

# 解除安裝具有Adobe Experience Manager舊版聯結器的Workfront

您必須解除安裝具有Adobe Experience Manager舊版聯結器的Workfront，才能使用連線Workfront和Adobe Experience Manager Assetsas a Cloud Service的最新原生整合。

## 取消訂閱Workfront

1. 開啟AdobeExperience Manger。
1. 在Experience Manager中，移至&#x200B;**工具** > **Cloud Service** > **Workfront整合組態**。
1. 選取您的設定（預設為global-workfront），然後按一下&#x200B;**屬性**。
   ![取消訂閱workfront](assets/unsubscribe-from-workfront.png)
1. 停用檔案、註解和中繼資料同步。 標籤應為停用日。
這將移除Workfront中的訂閱，並允許使用者使用Day CQ Link Externalizer中定義的相同URL來建立新訂閱。

## 刪除Workfront整合設定

移除訂閱後，現在可以安全刪除Workfront整合設定。

1. 開啟設定，然後選取&#x200B;**刪除**。
   ![刪除組態](assets/delete-wf-configuration.png)

## 移除對應

接下來，您需要刪除Workfront屬性對應。

1. 在Experience Manager中，移至&#x200B;**工具** > **Assets** > **Workfront屬性對應**。

1. 選取所有對應，然後按一下&#x200B;**刪除**。

## 使用者許可權

所有從Workfront存取AEM Dam的使用者皆獲得`/content/dam`的讀取許可權。 如果使用者不再需要該許可權，您可以移除授予該使用者的許可權。

聯結器使用系統使用者workfront-service操作。 解除安裝聯結器時會解除安裝。

>[!NOTE]
>
>如果您使用連線器版本2.0.3並新增群組`workfront-aem-connector-group`，也需要移至&#x200B;**工具** > **安全性** > **群組**&#x200B;來移除此專案。

## Day CQ連結外部化器

如果您不需要Day CQ Link Externalizer，您可以前往`/system/console/configMgr`尋找「Day CQ Link Externalizer」，將此專案還原為`localhost:4502`。

>[!NOTE]
>
>如果您使用Adobe Experience Manager as a Cloud Service，您可以檢視專案並在&#x200B;_ui.apps/src/main/content/jcr_root/apps/mysite/config_&#x200B;中找出檔案&#x200B;_com.day.cq.commons.impl.ExternalizerImpl.xml_&#x200B;來變更此專案。

![天CQ連結外部器](assets/Day-CQ-Link-Externalizer.png)

## 解除安裝聯結器封裝

解除安裝聯結器套件所需的步驟因您擁有的Adobe Experience Manager版本而異。

### Adobe Experience Manager On-Premise

如果您使用Adobe Experience Manager內部部署，請移至&#x200B;_crx/packmgr/index.jsp_，並尋找`workfront-aem-connector.all-<version>.zip`，按一下&#x200B;**更多**，然後&#x200B;**解除安裝**。

請檢查`/conf`下方，確認已移除所有Workfront建立的檔案。

### Adobe Experience Manager as a Cloud Service

對於Adobe Experience Manager as a Cloud Service，您可以從專案的pom.files中移除聯結器的相依性。

## Firewall和Dispatcher

如果不再需要通訊，別忘了移除已列入白名單的Workfront URL。 此外，聯結器會使用設定給Dispatcher的標題apiKey和使用者名稱。 這些檔案也可以移除。
