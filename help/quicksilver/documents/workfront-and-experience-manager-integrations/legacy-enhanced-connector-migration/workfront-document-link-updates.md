---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 移轉連結的資料夾和檔案
description: 您可以使用API將連結的資料夾和檔案移轉至Adobe Experience Manager Assets。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 586ab0a8-52ee-4aba-9298-af5a304acb02
source-git-commit: aad8f4648a57c93047a1a691d5e608c327d78c1b
workflow-type: tm+mt
source-wordcount: '918'
ht-degree: 0%

---

# 移轉連結的資料夾和檔案

您可以使用API將連結的資料夾和檔案移轉至Adobe Experience Manager Assets。

## 程式

1. 識別與先前外部檔案儲存提供者連結的所有檔案和資料夾，並記錄其Workfront內部檔案或資料夾識別碼以及任何容納資料夾的資料夾ID。

   >[!NOTE]
   >
   > 您應該檢查所有探索到的資料夾或檔案，以確認他們尚未與新的提供者建立連結。

1. 依路徑在新存放庫中尋找檔案和資料夾，然後在外部系統中查詢其身分。

1. 建立內部Workfront ID與新外部存放區中ID的對應。 您需要在下列步驟中建立新連結。

1. 在Workfront中建立新檔案或檔案資料夾連結，透過其新外部ID指向新位置的資源。

   1. **檔案**：使用新的外部檔案提供者新增現有檔案的新版本。
   1. **資料夾**：在相同位置建立相同名稱的新資料夾。

>[!CAUTION]
>
>   請勿刪除現有的連結資料夾。 這可能會造成資料遺失。 若要從Workfront應用程式中移除舊資料夾連結，請在「設定」區域中停用自訂檔案整合。


## 移轉連結的範例程式

![簡化連結流程](assets/links-flow-simplified.png)

## API資訊

如需本節中Workfront API的詳細資訊，請參閱[開發人員檔案：檔案](https://developer.workfront.com/documents.html)。

### 尋找所有檔案

尋找連結到&#x200B;**providerType**&#x200B;之&#x200B;**檔案提供者**&#x200B;且具有&#x200B;**documentProviderID**&#x200B;的所有&#x200B;**檔案(DOCU)**。

```
Http Method: GET
 
Http Endpoint: {host}/attask/api/v14.0/document/search?fields=currentVersion:*&currentVersion:externalIntegrationType={providerType}
```

[API檔案參考](https://developer.workfront.com/documents.html#get-/docu/search)

### 尋找所有資料夾

尋找連結到&#x200B;**providerType**&#x200B;之檔案提供者（具有&#x200B;**documentProviderID**）的所有&#x200B;**檔案資料夾(DOCFDR)**。

```
Http Method: GET
 
Http Endpoint: {host}/attask/api/v14.0/documentFolder/search?fields=*,linkedFolder:*&linkedFolder:externalIntegrationType={providerType}
```

API檔案： (developer.workfront.com目前未涵蓋的檔案資料夾端點)

### 連結檔案

從&#x200B;**providerType**&#x200B;的&#x200B;**外部檔案提供者**&#x200B;使用&#x200B;**documentProviderID**&#x200B;連結&#x200B;**檔案(DOCU)**。

>[!IMPORTANT]
>
>檔案會暫時儲存。 也就是說，您可以存取檔案的所有版本。 當您建立連結時，可以指定現有的檔案ID，因此您只需將新版本寫入該檔案，且資料會由新的提供者於外部託管。 此檔案ID與您所取代檔案連結上的檔案ID相同。 這是相同的概唸檔案。 您只需指出這個新版本的位元組是儲存在不同的提供者中。

```
Http Method: POST
 
Endpoint: {host}/internal/documents/linkExternalObjects
 
Http Body:
refObjCode=DOCU&refObjID={documentId}&providerType={providerType}&documentProviderID={documentProviderID}
```

API檔案： (developer.workfront.com目前未涵蓋的內部連結端點)

### 連結資料夾

從&#x200B;**providerType**&#x200B;的&#x200B;**外部檔案提供者**&#x200B;使用&#x200B;**documentProviderID**&#x200B;連結&#x200B;**檔案資料夾(DOCFDR)**。

>[!IMPORTANT]
>
>針對資料夾連結，與檔案連結不同，您需要Workfront中要將新連結放置到的資料夾的「documentFolderId」。 這很可能與我們複製的連結資料夾是相同的父資料夾。

>[!CAUTION]
>
>資料夾不會暫時儲存。 請勿刪除舊資料夾。 在設定區域中停用自訂檔案整合，以移除舊資料夾。


```
Http Method: POST
 
Endpoint: {host}/internal/document/version/linkExternal
 
Http Body:
providerType={providerType}&documentProviderID={documentProviderID}&breadcrumb=[]&linkAction=LINKEXTERNAL&refObjCode={USER|PROJECT_TASK|TEMPLATE_TASK|securityRootObjectCode}&refObjID={userID|taskID|templateTaskID|securityRootId}&destFolderID={parentFolderId}
```

API檔案： (developer.workfront.com目前未涵蓋的內部連結端點)

## 重要詞語

* **檔案**： Workfront中的數位資產

* **檔案資料夾**： Workfront中數位資產的容器

* **檔案ID**：數位資產的Workfront內部識別碼

* **檔案資料夾識別碼**：數位資產資料夾的Workfront內部識別碼

* **檔案提供者識別碼**：與特定檔案提供者關聯的識別碼

>[!IMPORTANT]
>
> 對於任何特定的檔案提供者型別，客戶可以有多個連線的執行個體。 舉例來說，他們可能連結了多個AEM存放庫。 或多個連結的Google Drive執行個體。 檔案提供者ID指示我們要取代或切換到的連線型別的特定執行個體。

* **檔案儲存提供者型別（也稱為「外部整合型別」）**： Workfront支援的檔案儲存提供者整合型別。 透過專用整合或「自訂整合」。

* **目前的檔案儲存提供者型別( providerType)**：

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

* **連結的檔案**：託管於外部檔案儲存提供者的數位資產。 Workfront將有資產專用的內部「檔案ID」，但位元組會儲存在外部。 為方便起見，Workfront也會儲存「外部檔案ID」，以協助找出遠端存放庫或存放區中的外部參考資源。

* **連結的檔案資料夾**：在外部檔案儲存提供者中代管的數位資產容器。 Workfront將有資產專用的內部「檔案資料夾ID」，但位元組會儲存在外部。 為方便起見，Workfront也會儲存「外部檔案ID」，以協助找出遠端存放庫或存放區中的外部參考資源。

* **外部檔案ID**：當資產儲存在Workfront外部時指派的ID。 Workfront透過此「外部檔案識別碼」欄位，將其內部識別碼對應至用於在外部系統中尋找資產的識別碼。 因此，從新的外部存放區連結檔案或資料夾時，必須以適當的格式構成新的外部檔案識別碼，以便外部檔案提供者識別新存放庫或存放區中的檔案。

  >[!NOTE]
  >
  > Workfront還沒有外部檔案識別碼的標準。 AEM ID使用新的規格，但對於其他ID，外部檔案ID可能會根據提供者型別而採用不同的表單。


* **物件型別**：此為API專用字詞，僅供本檔案使用。 這是Workfront中您希望與其互動的通用物件型別。 在這種情況下，您將分別與型別為「DOCU」和「DOCFDR」的檔案和資料夾進行互動。

* **物件識別碼**：您要與互動之一般物件的內部Workfront識別碼。 您將與檔案和資料夾互動，因此這將會是檔案ID或檔案資料夾ID。
