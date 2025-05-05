---
content-type: reference
product-previous: workfront-proof
product-area: documents
navigation-topic: organize-your-work-workfront-proof
title: 瞭解 [!DNL Workfront Proof]中的檔案夾許可權
description: 如果人員有權檢視資料夾中的專案，他們也可以檢視資料夾本身。 但是，他們只能看到資料夾中明確與其共用的專案。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 96162fe8-eef9-40f4-bc94-02911b970f02
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 15%

---

# 瞭解[!DNL Workfront Proof]中的檔案夾許可權

>[!IMPORTANT]
>
>本文提及獨立產品[!DNL Workfront Proof]中的功能。 有關[!DNL Adobe Workfront]內部校訂的資訊，請參閱[校訂](../../../review-and-approve-work/proofing/proofing.md)。

如果人員有權檢視資料夾中的專案，他們也可以檢視資料夾本身。 但是，他們只能看到資料夾中明確與其共用的專案。

## 公用資料夾

如果資料夾是公開的，則帳戶中的使用者（不包括觀察者和輕度使用者）可以在左側邊欄中看到資料夾名稱。

您的許可權設定檔也會影響您對公用資料夾的許可權：

| **設定檔/動作** | **檢視資料夾中的所有專案** | **檢視與他們明確共用的專案** | **新增專案** | **刪除專案** | **新增子資料夾** | **刪除子資料夾** | **編輯資料夾詳細資料** |
|---|---|---|---|---|---|---|---|
| **建立者** | 是 | 是 | 是 | 是 | 是 | 是 | 是 |
| **帳單管理員** | 是 | 是 | 是 | 是 | 是 | 是 | 是 |
| **管理員** | 是 | 是 | 是 | 是 | 是 | 是 | 是 |
| **監督員** | 是 | 是 | 是 | 是 | 是 | 是 | 是 |
| **管理員** | 否 | 是 | 是 | 否 | 是 | 否 | 是 |
| **觀察者** | 否 | 是 | 否 | 否 | 否 | 否 | 否 |

{style="table-layout:auto"}

如果公用資料夾為管理員所擁有，他或她可以刪除根資料夾及任何子資料夾。

如需詳細資訊，請參閱 [!DNL Workfront Proof][&#128279;](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)中的校訂許可權設定檔。

## 私人資料夾

如果資料夾是私人的，則同一帳戶中的其他使用者無法在左側邊欄中看到資料夾的名稱，除非資料夾中的資料夾或專案已明確與他們共用，或者他們具有「主管」、「管理員」或「計費管理員」的設定檔：

| **設定檔/動作** | **檢視資料夾中的所有專案** | **檢視與他們明確共用的專案** | **新增專案** | **刪除專案** | **新增子資料夾** | **刪除子資料夾** | **編輯資料夾詳細資料** |
|---|---|---|---|---|---|---|---|
| **建立者** | 是 | 是 | 是 | 是 | 是 | 是 | 是 |
| **帳單管理員** | 是 | 是 | 是 | 是 | 是 | 是 | 是 |
| **管理員** | 是 | 是 | 是 | 是 | 是 | 是 | 是 |
| **監督員** | 是 | 是 | 是 | 是 | 是 | 是 | 是 |
| **管理員** | 否 | 是 | 否 | 否 | 否 | 否 | 否 |
| **觀察者** | 否 | 是 | 否 | 否 | 否 | 否 | 否 |

{style="table-layout:auto"}

例如，如果您希望您的專案經理及其團隊只檢視特定資料夾，專案經理可以設定私人資料夾，然後與特定使用者共用該資料夾。

共用私人資料夾時，您可以決定是否希望管理員能夠建立、編輯和刪除資料夾專案。

您可以在[新增資料夾]頁面中個別設定每個人的此專案，並在[資料夾詳細資料]頁面的[共用對象] 區段中加以變更。 如需詳細資訊，請參閱[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md)中建立資料夾，以及[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders-and-contents.md)中管理資料夾及其內容。

如果與或觀察者共用私人資料夾，他們將對該資料夾中的所有專案具有唯讀存取權。 如需詳細資訊，請參閱 [!DNL Workfront Proof][&#128279;](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)中的[校訂許可權設定檔和 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/share-folders.md)中的共用資料夾。

>[!NOTE]
>
>* 如果父資料夾是私人的，則所有子資料夾也是私人的。 私人父資料夾下不能有公用子資料夾。 不過，您可以在公用父資料夾下擁有私人子資料夾。
>* 資料夾的建立者和擁有者將永遠擁有其存取權，且無法移除。
>* 只有私人資料夾的建立者和擁有者可以刪除資料夾。

