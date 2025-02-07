---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: Workfront Proof中的校訂許可權設定檔
description: 身為Workfront管理員或Workfront Proof管理員，您可以將校訂許可權設定檔指派給使用者，以指定使用者將擁有系統中所有校訂的校訂權能。 如需設定使用者校訂許可權設定檔的詳細資訊，請參閱在Workfront Proof中設定使用者的校訂許可權設定檔。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 249aa332-c051-49ac-be85-264d8babfcad
source-git-commit: ddaee5b339982c826c14b67775d81f3a2bd7bc37
workflow-type: tm+mt
source-wordcount: '1924'
ht-degree: 0%

---

# [!DNL Workfront Proof]中的校訂許可權設定檔

>[!IMPORTANT]
>
>本文提及獨立產品[!DNL Workfront Proof]中的功能。 有關[!DNL Adobe Workfront]內部校訂的資訊，請參閱[校訂](../../../review-and-approve-work/proofing/proofing.md)。

作為[!DNL Workfront]管理員或[!DNL Workfront Proof]管理員，您可以將校訂許可權設定檔指派給使用者，以指定使用者將擁有的系統中所有校訂的校訂權能。 如需有關設定使用者校訂許可權設定檔的資訊，請參閱[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/config-user-pref-in-wp.md)中設定使用者的校訂許可權設定檔。

>[!NOTE]
>
>您也可以執行下列動作：
>
>* 授予使用者個別校訂的特定角色。 如需校訂角色的詳細資訊，請參閱[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)中管理校訂角色。
>* 為您組織中的使用者建立自訂設定檔。 如需詳細資訊，請參閱[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-custom-profiles.md)中設定自訂設定檔。
>

下表顯示每個校訂許可權設定檔的可用許可權。

| **擁有的專案** |  |  |  |  | **其他使用者的專案** |  |  | **管理員** | **帳單** |
|---|---|---|---|---|---|---|---|---|---|
|   | **新增** | **檢視** | **編輯** | **刪除** | **檢視** | **編輯** | **刪除** | **編輯和刪除** | **編輯** |
| 帳單管理員 | ![核取記號](assets/cleaner2.png) | ![核取記號](assets/cleaner2.png) | ![核取記號](assets/cleaner2.png) | ![核取記號](assets/cleaner2.png) | ![核取記號](assets/cleaner2.png) | ![核取記號](assets/cleaner2.png) | ![核取記號](assets/cleaner2.png) | ![核取記號](assets/cleaner2.png) | ![核取記號](assets/cleaner2.png) |
| 管理員 | ![核取記號](assets/cleaner2.png) | ![核取記號](assets/cleaner2.png) | ![核取記號](assets/cleaner2.png) | ![核取記號](assets/cleaner2.png) | ![核取記號](assets/cleaner2.png) | ![核取記號](assets/cleaner2.png) | ![核取記號](assets/cleaner2.png) | ![核取記號](assets/cleaner2.png) |   |
| 主管 | ![核取記號](assets/cleaner2.png) | ![核取記號](assets/cleaner2.png) | ![核取記號](assets/cleaner2.png) | ![核取記號](assets/cleaner2.png) | ![核取記號](assets/cleaner2.png) | ![核取記號](assets/cleaner2.png) | ![核取記號](assets/cleaner2.png) |   |   |
| 經理 | ![核取記號](assets/cleaner2.png) | ![核取記號](assets/cleaner2.png) | ![核取記號](assets/cleaner2.png) | ![核取記號](assets/cleaner2.png) |   |   |   |   |   |
| 觀察者 |   | ![核取記號](assets/cleaner2.png) |   |   |   |   |   |   |   |
| 訪客 |   | ![核取記號](assets/cleaner2.png) |   |   |   |   |   |   |   |

{style="table-layout:auto"}

關於角色與許可權，請考量下列事項：

* 指派的設定檔許可權僅與您自己的帳戶中的使用者和專案有關。 衛星帳戶的例外情況，其中主要（中樞）帳戶的管理員和帳單管理員可以從中樞帳戶層級存取和管理這些帳戶的帳戶設定和帳單。
* 帳單管理員和管理員可以刪除使用者。 這只能在帳戶設定中完成。
* 當帳單管理員和管理員檢視其帳戶中其他使用者擁有的校訂時，他們會以檢閱者的角色檢視校訂。
* 使用唯讀角色，帳單管理員和管理員可以存取共用給他們的資料夾中或他們建立的資料夾中的校樣。

以下各節說明標準[!DNL Workfront Proof]設定中每個設定檔以及與設定檔相關聯的許可權：

* [帳單管理員](#billing-administrator)
* [管理員](#administrator)
* [監督員](#supervisor)
* [管理員](#manager)
* [觀察者](#observer)
* [訪客](#visitor)
* [來賓](#guest)

## 帳單管理員 {#billing-administrator}

帳單管理員可以存取 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md) and [The [!DNL Workfront Proof] 帳單頁面](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md)中的[帳戶設定，並具有下列許可權：

![核取記號](assets/cleaner2.png)可以產生校樣、上傳檔案和建立資料夾。 如需詳細資訊，請參閱[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)中產生校樣、[將檔案和網頁內容上傳到 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md)以及[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md)中建立資料夾。

![核取記號](assets/cleaner2.png)可以檢視、編輯和刪除自己建立的校樣和檔案。

![核取記號](assets/cleaner2.png)可以檢視、編輯和刪除組織中的所有使用者建立的校訂和檔案。

![核取記號](assets/cleaner2.png)可以刪除其他使用者的公用資料夾。 如需詳細資訊，請參閱[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md)中管理資料夾。

![核取記號](assets/cleaner2.png)擁有對帳號中建立的所有校訂的編輯許可權。

![核取記號](assets/cleaner2.png)可以設定為拖放區域擁有者。 如需詳細資訊，請參閱[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md)中設定dropzone。

![核取記號](assets/cleaner2.png)可以存取帳單頁面並編輯帳單詳細資料。 如需詳細資訊，請參閱[帳單頁面 [!DNL Workfront Proof] ](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md)。

![核取記號](assets/cleaner2.png)可以存取[帳戶設定]頁面並編輯帳戶詳細資料。 如需詳細資訊，請參閱 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md)中的[帳戶設定。

![核取記號](assets/cleaner2.png)可以清空垃圾桶。 如需詳細資訊，請參閱[還原並清空垃圾桶 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md)。

![核取記號](assets/cleaner2.png)可以新增、編輯和刪除使用者。

![核取記號](assets/cleaner2.png)可以建立群組並新增連絡人。

![核取記號](assets/cleaner2.png)可以刪除連絡人。

![核取記號](assets/cleaner2.png)如果校樣上沒有回覆，可以編輯校樣。

![紅色X](assets/no2.png)無法編輯校訂回覆。

![紅色X](assets/no2.png)無法刪除其他使用者的私人資料夾。 如需詳細資訊，請參閱[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md)中管理資料夾。

如需帳戶設定的詳細資訊，請參閱 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md)中的[帳戶設定。

如需計費資訊，請參閱[計費頁面 [!DNL Workfront Proof] ](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md)。

### 管理員 {#administrator}

系統管理員可以存取[帳戶設定](https://support.workfront.com/hc/en-us/sections/115000912147-Account-Settings)並擁有下列許可權：

![核取記號](assets/cleaner2.png)可以建立校樣、上傳檔案和建立資料夾。 如需詳細資訊，請參閱[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)中產生校樣、[將檔案和網頁內容上傳到 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md)以及[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md)中建立資料夾。

![核取記號](assets/cleaner2.png)可以檢視、編輯和刪除校樣及他們建立的檔案。

![核取記號](assets/cleaner2.png)可以檢視、編輯和刪除組織中的所有使用者建立的校訂和檔案。

![核取記號](assets/cleaner2.png)可以刪除其他使用者的公用資料夾。 如需詳細資訊，請參閱[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md)中管理資料夾。

![核取記號](assets/cleaner2.png)擁有對帳號中建立的所有校訂的編輯許可權。

![核取記號](assets/cleaner2.png)可以設定為拖放區域擁有者。 如需詳細資訊，請參閱[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md)中設定dropzone。

![核取記號](assets/cleaner2.png)可以存取[帳戶設定]頁面並編輯帳戶詳細資料。 如需詳細資訊，請參閱 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md)中的[帳戶設定。

![核取記號](assets/cleaner2.png)可以清空垃圾桶。 如需詳細資訊，請參閱[還原並清空垃圾桶 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md)。

![核取記號](assets/cleaner2.png)可以新增、編輯和刪除使用者。

![核取記號](assets/cleaner2.png)可以建立群組並新增連絡人。

![核取記號](assets/cleaner2.png)可以刪除連絡人。

![核取記號](assets/cleaner2.png)如果校樣上沒有回覆，可以編輯校樣。

![紅色X](assets/no2.png)無法編輯校訂回覆。

![紅色X](assets/no2.png)無法刪除其他使用者的私人資料夾。 如需詳細資訊，請參閱[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md)中管理資料夾。

![紅色X](assets/no2.png)無法存取帳單頁面或編輯帳單詳細資料。 如需詳細資訊，請參閱[帳單頁面 [!DNL Workfront Proof] ](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md)。

### 主管 {#supervisor}

主管擁有下列許可權：

![核取記號](assets/cleaner2.png)可以建立校樣、上傳檔案和建立資料夾。 如需詳細資訊，請參閱[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)中產生校樣、[將檔案和網頁內容上傳到 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md)以及[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md)中建立資料夾。

![核取記號](assets/cleaner2.png)可以檢視、編輯和刪除他們建立的校樣和檔案。

![核取記號](assets/cleaner2.png)可以檢視、編輯和刪除組織中的所有使用者建立的校訂和檔案。

![核取記號](assets/cleaner2.png)可以刪除其他使用者的公用資料夾。 如需詳細資訊，請參閱[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md)中管理資料夾。

![核取記號](assets/cleaner2.png)擁有對帳號中建立的所有校訂的編輯許可權。

![核取記號](assets/cleaner2.png)可以設定為拖放區域擁有者。 如需詳細資訊，請參閱[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md)中設定dropzone。

![核取記號](assets/cleaner2.png)可以建立群組並新增連絡人。

![核取記號](assets/cleaner2.png)可以刪除連絡人。

![核取記號](assets/cleaner2.png)如果校樣上沒有回覆，可以編輯校樣。

![紅色X](assets/no2.png)無法編輯校訂回覆。

![紅色X](assets/no2.png)無法刪除其他使用者的私人資料夾。 如需詳細資訊，請參閱 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/folders.md)中的[資料夾。

![紅色X](assets/no2.png)無法存取帳單頁面或帳戶設定。 如需詳細資訊，請參閱[帳單頁面](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md)和 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md)中的[帳戶設定。 [!DNL Workfront Proof] 

![紅色X](assets/no2.png)無法新增、編輯或刪除使用者。

![紅色X](assets/no2.png)無法清空垃圾桶。 如需詳細資訊，請參閱[還原並清空垃圾桶 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md)。

### 經理 {#manager}

管理員擁有下列許可權：

![核取記號](assets/cleaner2.png)可以建立校樣、上傳檔案和建立資料夾。 如需詳細資訊，請參閱[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)中產生校樣、[將檔案和網頁內容上傳到 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md)以及[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md)中建立資料夾。

![核取記號](assets/cleaner2.png)可以檢視、編輯和刪除自己建立或擁有的校樣和檔案。

![核取記號](assets/cleaner2.png)可以檢視、檢閱及核准其他使用者的校樣，這些校樣是明確與他們共用（共用資料夾中所有專案的唯讀許可權）。 如需詳細資訊，請參閱[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)中管理校訂角色。

![核取記號](assets/cleaner2.png)可以建立群組並新增連絡人。

![紅色X](assets/no2.png)無法檢視、編輯或刪除組織中其他使用者建立的校訂和檔案。

![紅色X](assets/no2.png)無法編輯校樣或回覆。

![紅色X](assets/no2.png)無法刪除其他使用者的私人資料夾。 如需詳細資訊，請參閱[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md)中管理資料夾。

![紅色X](assets/no2.png)無法刪除其他使用者的公用資料夾。 如需詳細資訊，請參閱[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md)中管理資料夾。

![紅色X](assets/no2.png)無法存取帳單頁面或帳戶設定。 如需詳細資訊，請參閱[帳單頁面](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md)和 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md)中的[帳戶設定。 [!DNL Workfront Proof] 

![紅色X](assets/no2.png)無法設定為拖放區域擁有者。 如需詳細資訊，請參閱[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md)中設定dropzone。

![紅色X](assets/no2.png)無法清空垃圾桶。 如需詳細資訊，請參閱[還原並清空垃圾桶 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md)。

![紅色X](assets/no2.png)無法新增、編輯或刪除使用者。

![紅色X](assets/no2.png)無法刪除連絡人。

### 觀察者 {#observer}

觀察者具有下列許可權：

![核取記號](assets/cleaner2.png)可以檢視、檢閱及核准其他使用者的校樣，這些校樣是明確與他們共用（共用資料夾中所有內容的唯讀許可權）。 如需詳細資訊，請參閱[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)中管理校訂角色。

![核取記號](assets/cleaner2.png)可以檢視明確與其共用的檔案。

![核取記號](assets/cleaner2.png)可以檢視連絡人和群組

![紅色X](assets/no2.png)無法建立校樣、上傳檔案和建立資料夾。 如需詳細資訊，請參閱[將檔案與網頁內容上傳至 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md)。

![紅色X](assets/no2.png)無法檢視、編輯或刪除組織中其他使用者建立的校訂和檔案。

![紅色X](assets/no2.png)無法編輯校樣或回覆。

![紅色X](assets/no2.png)無法刪除組織中建立的任何專案。

![紅色X](assets/no2.png)無法存取帳單頁面或帳戶設定。 如需詳細資訊，請參閱[帳單頁面](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md)和 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md)中的[帳戶設定。 [!DNL Workfront Proof] 

![紅色X](assets/no2.png)無法設定為拖放區域擁有者。 如需詳細資訊，請參閱[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md)中設定dropzone。

![紅色X](assets/no2.png)無法清空垃圾桶。 如需詳細資訊，請參閱[還原並清空垃圾桶 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md)。

![紅色X](assets/no2.png)無法新增、編輯或刪除使用者。

![紅色X](assets/no2.png)無法建立群組或新增連絡人。

![紅色X](assets/no2.png)無法刪除連絡人。

>[!NOTE]
>
>觀察者可用的選單和功能有限。
>
>* 觀察者在其控制面板中看不到標題功能表或綠色的新功能表
>* 觀察者的「設定」中看不到下列連結：帳戶設定、帳單
>

### 訪客 {#visitor}

訪客擁有下列許可權：

![核取記號](assets/cleaner2.png)可以檢視、檢閱及核准其他使用者的校樣，這些校樣是明確與他們共用（共用資料夾中所有專案的唯讀許可權）。 如需詳細資訊，請參閱[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)中管理校訂角色。

![核取記號](assets/cleaner2.png)可以檢視明確與其共用的檔案。

![紅色X](assets/no2.png)無法檢視連絡人和群組

![紅色X](assets/no2.png)無法建立校樣、上傳檔案和建立資料夾。 如需詳細資訊，請參閱[將檔案與網頁內容上傳至 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md)。

![紅色X](assets/no2.png)無法檢視、編輯或刪除組織中其他使用者建立的校訂和檔案。

![紅色X](assets/no2.png)無法編輯校樣或回覆。

![紅色X](assets/no2.png)無法刪除組織中建立的任何專案。

![紅色X](assets/no2.png)無法存取帳單頁面或帳戶設定。 如需詳細資訊，請參閱[帳單頁面](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md)和 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md)中的[帳戶設定。 [!DNL Workfront Proof] 

![紅色X](assets/no2.png)無法設定為拖放區域擁有者。 如需詳細資訊，請參閱[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md)中設定dropzone。

![紅色X](assets/no2.png)無法清空垃圾桶。 如需詳細資訊，請參閱[還原並清空垃圾桶 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md)。

![紅色X](assets/no2.png)無法新增、編輯或刪除使用者。

![紅色X](assets/no2.png)無法建立群組或新增連絡人。

![紅色X](assets/no2.png)無法刪除連絡人。

>[!NOTE]
>
>訪客可用的功能表和功能有限。
>
>* 訪客在其控制面板中看不到標題功能表或綠色的新功能表
>* 訪客在其「設定」中看不到下列連結：帳戶設定、帳單
>

### 來賓 {#guest}

訪客設定檔可讓沒有自己Workfront Proof帳戶的檢閱者存取校樣。 訪客可透過其個人電子郵件通知直接存取與其共用的校樣。

![核取記號](assets/cleaner2.png)可以檢視、檢閱及核准明確與其共用的校訂。

![核取記號](assets/cleaner2.png)可以檢視明確與其共用的檔案。

![紅色X](assets/no2.png)無法存取儀表板。

![紅色X](assets/no2.png)無法共用資料夾。 如需詳細資訊，請參閱[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md)中管理資料夾。

![紅色X](assets/no2.png)無法新增為校訂的作者或版主。 如需詳細資訊，請參閱[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)中管理校訂角色。

>[!NOTE]
>
>訪客不是Workfront Proof使用者，因此他們無法在自己的控制面板中看到與其共用的所有校樣。

## 編輯使用者的校訂許可權設定檔

管理員和帳單管理員可以編輯帳戶中所有使用者的許可權設定檔。

1. 若要尋找要編輯的使用者，請執行下列任一項作業：

   * 瀏覽至&#x200B;**[!UICONTROL 帳戶設定]**，然後按一下&#x200B;**[!UICONTROL 使用者]**&#x200B;索引標籤。

   * 移至&#x200B;**[!UICONTROL 連絡人]**&#x200B;頁面。

1. 按一下您要編輯其許可權的使用者名稱。 ![選取使用者](assets/screenshot-2018-03-30-14-16-05a-350x69.png)

1. 按一下&#x200B;**[!UICONTROL 許可權設定檔]**&#x200B;下拉式功能表，然後選取新的許可權設定檔。：

   ![許可權設定檔](assets/screenshot-2018-03-30-14-18-03a.png)

   許可權設定檔包括「管理員」、「監督員」、「管理員」和「觀察者」。

1. 按一下功能表之外的任意位置以儲存。

>[!NOTE]
>
>管理員無法指派計費管理員設定檔。 您可以在下列記錄檔中找到設定檔變更清單：
>
>* 帳戶活動記錄
>* 使用者的設定檔記錄（僅供該使用者存取）
>

如需活動記錄的詳細資訊，請參閱[瞭解 [!DNL Workfront Proof] 活動稽核軌跡](../../../workfront-proof/wp-work-proofsfiles/basic-features/activity-audit-trail.md)。
