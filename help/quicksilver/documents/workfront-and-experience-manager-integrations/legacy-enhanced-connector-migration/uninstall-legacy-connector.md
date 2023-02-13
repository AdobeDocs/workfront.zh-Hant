---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 卸載舊連接器
description: 文字
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4b3834bf-2e6d-4588-8d77-671e14390115
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 0%

---

# 解除安裝Workfront與Adobe Experience Manager舊連接器

您必須將Workfront與Adobe Experience Manager舊連接器解除安裝，以取得連接Workfront與Adobe Experience Manager Assets的最新原生整合as a Cloud Service。

## 取消訂閱Workfront

1. 開啟Adobe Experience Manager。
1. 在Experience Manager中，前往 **工具** > **Cloud Services** > **Workfront整合設定**.
1. 選取您的設定（預設為全域工作線），然後按一下 **屬性**.
   ![取消訂閱workfront](assets/unsubscribe-from-workfront.png)
1. 禁用文檔、注釋和元資料同步。 標籤應為「禁用」日。
這會移除Workfront中的訂閱，並允許使用者使用Day CQ Link Externalizer中定義的相同url建立新訂閱。

## 刪除Workfront整合設定

移除訂閱後，現在刪除Workfront整合設定是安全的。

1. 開啟設定，然後選取 **刪除**.
   ![刪除配置](assets/delete-wf-configuration.png)

## 刪除映射

接下來，您需要刪除Workfront屬性對應。

1. 在Experience Manager中，前往 **工具** > **資產** > **Workfront屬性對應**.

1. 選擇所有映射，然後按一下 **刪除**.

## 使用者權限

所有從Workfront存取AEM Dam的使用者，都獲得 `/content/dam`. 如果使用者不再需要，您可以移除指定給該使用者的權限。

連接器使用系統用戶工作前服務運行。 卸載連接器時，將卸載此操作。

>[!NOTE]
>
>如果您使用連接器2.0.3版並新增群組 `workfront-aem-connector-group`，此項目也需移除，方法是 **工具** > **安全性** > **群組**.

## Day CQ Link Externalizer

如果您不需要Day CQ Link Externalizer，可將此還原回 `localhost:4502` 通過 `/system/console/configMgr` 和尋找「Day CQ Link Externalizer」。

>[!NOTE]
>
>如果您使用Adobe Experience Manager as a Cloud Service，則可查看專案並找到檔案以變更此項目 _com.day.cq.commons.impl.ExternalizerImpl.xml_ in _ui/apps/src/main/content/jcr_root/apps/mysite/config_.

![Day CQ Link Externalizer](assets/Day-CQ-Link-Externalizer.png)

## 卸載連接器封裝

解除安裝連接器封裝所需的步驟因您擁有的Adobe Experience Manager版本而異。

### Adobe Experience Manager內部部署

如果您使用內部部署的Adobe Experience Manager，請前往 _crx/packmgr/index.jsp_，並尋找 `workfront-aem-connector.all-<version>.zip`，按一下 **更多** 然後 **解除安裝**.

請查看下 `/conf` 確認已移除所有Workfront建立的檔案。

### Adobe Experience Manager as a Cloud Service

對於Adobe Experience Manager as a Cloud Service，您可以從專案的pom.files中移除連接器的相依性。

## 防火牆和Dispatcher

如果不再需要通訊，請記得移除已列入白名單的Workfront URL。 此外，連接器也使用已設為Dispatcher的標題apiKey和使用者名稱。 這些也可以移除。
