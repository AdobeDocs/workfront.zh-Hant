---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 遷移連結的資料夾和文檔
description: 您可以使用API將連結的資料夾和檔案移轉至Adobe Experience Manager Assets。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 586ab0a8-52ee-4aba-9298-af5a304acb02
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 0%

---

# 遷移連結的資料夾和文檔

您可以使用API將連結的資料夾和檔案移轉至Adobe Experience Manager Assets。

## 程式

1. 標識與前一個外部文檔儲存提供程式連結的所有文檔和資料夾，並注意其Workfront內部文檔或資料夾標識符以及任何包含資料夾的資料夾ID。

   >[!NOTE]
   >
   > 您應檢查所有發現的資料夾或文檔，以確認它們尚未與新提供程式建立連結。

1. 按路徑在新儲存庫中查找文檔和資料夾，然後在外部系統中查找其標識。

1. 建立內部Workfront ID與新外部商店ID的對應。 您需要這個項目，才能在下列步驟中建立新連結。

1. 在Workfront中建立新檔案或檔案資料夾連結，並透過新外部ID指向新位置中的資源。

   1. **檔案**:使用新的外部文檔提供程式添加現有文檔的新版本。
   1. **資料夾**:在同名的同一位置建立新檔案夾。

>[!CAUTION]
>
>   請勿刪除現有的連結資料夾。 這可能導致資料遺失。 若要從Workfront應用程式移除舊資料夾連結，請停用「設定」區域中的自訂檔案整合。


## 移轉連結的范常式式

![簡化連結流程](assets/links-flow-simplified.png)

## API資訊

如需本節中Workfront API的詳細資訊，請參閱 [開發人員檔案：檔案](https://developer.workfront.com/documents.html).

### 查找所有文檔

全部查找 **文檔(DOCU)** 連結至 **文檔提供程式** of **providerType** with **documentProviderID**.

```
Http Method: GET
 
Http Endpoint: {host}/attask/api/v14.0/document/search?fields=currentVersion:*&currentVersion:externalIntegrationType={providerType}
```

[API檔案參考](https://developer.workfront.com/documents.html#get-/docu/search)

### 查找所有資料夾

全部查找 **文檔資料夾(DOCFDR)** 連結至的檔案提供者 **providerType** with **documentProviderID**.

```
Http Method: GET
 
Http Endpoint: {host}/attask/api/v14.0/documentFolder/search?fields=*,linkedFolder:*&linkedFolder:externalIntegrationType={providerType}
```

API檔案：（developer.workfront.com中當前未涵蓋的文檔資料夾端點）

### 連結文檔

連結 **文檔(DOCU)** 從 **外部文檔提供程式** of **providerType** with **documentProviderID**.

>[!IMPORTANT]
>
>文檔被臨時儲存。 也就是說，您可以存取檔案的所有版本。 建立連結時，可以指定現有的文檔ID，因此您只需將新版本寫入該文檔，資料從外部托管在新提供程式中。 此文檔ID與要替換的文檔連結上找到的文檔ID相同。 是同樣的概念性檔案。 您只是在表示此新版本的位元組與不同提供者一起儲存。

```
Http Method: POST
 
Endpoint: {host}/internal/documents/linkExternalObjects
 
Http Body:
refObjCode=DOCU&refObjID={documentId}&providerType={providerType}&documentProviderID={documentProviderID}
```

API檔案：（developer.workfront.com目前未涵蓋的內部連結端點）

### 連結資料夾

連結 **文檔資料夾(DOCFDR)** 從 **外部文檔提供程式** of **providerType** with **documentProviderID**.

>[!IMPORTANT]
>
>對於資料夾連結，與「檔案」連結不同，您需要Workfront中要將新連結置入之資料夾的「documentFolderId」。 這很可能與我們要複製的連結資料夾相同的父資料夾。

>[!CAUTION]
>
>資料夾不會暫時儲存。 請勿刪除舊資料夾。 在設定區域中禁用自定義文檔整合以刪除舊資料夾。


```
Http Method: POST
 
Endpoint: {host}/internal/document/version/linkExternal
 
Http Body:
providerType={providerType}&documentProviderID={documentProviderID}&breadcrumb=[]&linkAction=LINKEXTERNAL&refObjCode={USER|PROJECT_TASK|TEMPLATE_TASK|securityRootObjectCode}&refObjID={userID|taskID|templateTaskID|securityRootId}&destFolderID={parentFolderId}
```

API檔案：（developer.workfront.com目前未涵蓋的內部連結端點）

## 重要詞語

* **檔案**:Workfront中的數位資產

* **文檔資料夾**:Workfront中的數位資產容器

* **檔案ID**:Workfront數位資產的內部ID

* **文檔資料夾ID**:Workfront數位資產資料夾的內部ID

* **文檔提供程式ID**:與特定檔案提供者相關聯的ID

>[!IMPORTANT]
>
> 對於任何指定的文檔提供程式類型，客戶可能有多個連接的實例。 例如，他們可能有多個AEM存放庫連結。 或連結多個Google Drive實例。 文檔提供程式ID指示要替換或切換到的連接類型的特定實例。

* **文檔儲存提供程式類型（也稱為「外部整合類型」）**:Workfront支援的檔案儲存提供者整合類型。 透過專用整合或「自訂整合」。

* **當前文檔儲存提供程式類型(providerType)**:

   ```
   ATTASK
   BOX
   GOOGLE
   SHAREPOINT
   WEBDAM
   WORKFRONTDAM
   INFERNO
   WIDEN
   DROPBOX
   DROPBOX_BUSINESS
   ONEDRIVE
   QUIP
   WEBHOOKS
   AEM
   MOCK
   ```

* **連結的文檔**:在外部檔案儲存提供者中托管的數位資產。 Workfront會有其專屬資產的內部「檔案ID」，但位元組會從外部儲存。 為方便執行此作業，Workfront也會儲存「外部檔案ID」，以協助在遠端存放庫或存放區中找到外部參考的資源。

* **連結的文檔資料夾**:在外部檔案儲存提供者中托管的數位資產容器。 Workfront會有其專屬資產的內部「檔案資料夾ID」，但位元組會從外部儲存。 為方便執行此作業，Workfront也會儲存「外部檔案ID」，以協助在遠端存放庫或存放區中找到外部參考的資源。

* **外部文檔ID**:當資產儲存在工作區外部時指派的ID。 Workfront會透過此「外部檔案識別碼」欄位，將其內部識別碼對應至用於在外部系統中尋找資產的識別碼。 因此，從新外部儲存庫連結文檔或資料夾時，必須以適當格式組成新的外部文檔標識符，以便外部文檔提供程式識別新儲存庫或儲存庫中的文檔。

   >[!NOTE]
   >
   > Workfront尚未提供外部檔案識別碼的標準。 AEM ID正在使用新規格，但是對於其他ID，外部文檔ID可能會採用不同的表單（取決於提供程式類型）。


* **對象類型**:此為僅適用於本檔案目的的API術語。 這是工作區中您想與之互動的一般物件類型。 在這種情況下，您將與分別具有「DOCU」和「DOCFDR」類型的文檔和資料夾交互。

* **物件ID**:您要與之互動的一般物件的內部Workfront識別碼。 您將與文檔和資料夾交互，因此這將分別是文檔ID或文檔資料夾ID。
