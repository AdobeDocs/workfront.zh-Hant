---
product-previous: workfront-proof
product-area: documents
navigation-topic: share-proofs-and-files
title: 管理校訂角色於 [!DNL Workfront Proof]
description: 校訂角色可讓您向受使用者設定檔上設定的許可權設定檔限制的使用者授予許可權。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: b371cc20-4226-49ce-96c6-9815b2e84713
source-git-commit: 6e24b9c717ecedd6efbdf62ec01e53ac98079cfe
workflow-type: tm+mt
source-wordcount: '1306'
ht-degree: 0%

---

# 管理校訂角色於 [!DNL Workfront Proof]

<!-- Audited: 01/2024 -->

>[!IMPORTANT]
>
>本文提及獨立版產品中的功能 [!DNL Workfront Proof]. 有關內部校訂的資訊 [!DNL Adobe Workfront]，請參閱 [校訂](../../../review-and-approve-work/proofing/proofing.md).

校訂角色可讓您向受使用者設定檔上設定的許可權設定檔限制的使用者授予許可權。 (如需許可權設定檔的詳細資訊，請參閱 [中的校訂許可權設定檔 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).)

校樣角色與帳戶設定檔不同。 您的帳戶設定檔與您帳戶中的整體許可權層級有關，並將影響您對帳戶中所有校訂所擁有的許可權，即使那些尚未明確與您共用的校訂亦然。

如需詳細資訊，請參閱 [中的校訂許可權設定檔 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

## 關於校訂角色

邀請使用者檢閱校訂時，以下校訂角色將授予使用者個人校訂：

* [唯讀](#read-only)
* [檢閱者](#reviewer)
* [核准者](#approver)
* [檢閱者和核准者](#reviewer-approver)
* [作者](#author)
* [仲裁者](#moderator)

校樣角色定義檢閱者可對該特定校樣執行的動作。

例如，如果您是檢閱者，系統會要求您新增標籤和註解以檢閱校訂。 如果您是檢閱者和核准者，系統將會要求您檢閱並決定校訂。

某些校訂角色會為檢閱者提供對校訂的編輯許可權（即使他們的帳戶設定檔沒有），並允許他們使用一些其他功能，例如新增評論動作、建立新版本以及向校訂新增更多檢閱者。

如需詳細資訊，請參閱下列文章：

* [對校訂評論使用動作](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md)
* [在中共用校訂 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md)

### 唯讀

{#read-only}

![cleaner.png](assets/cleaner.png) 可以檢視校訂

![no.png](assets/no.png) 無法新增標籤

![no.png](assets/no.png) 無法新增註解

![no.png](assets/no.png) 無法做出決定

![no.png](assets/no.png) 無法刪除其他人的評論

![no.png](assets/no.png) 沒有校訂的編輯許可權

>[!NOTE]
>
>如果資料夾已與使用者共用 [!DNL Workfront Proof]，這些使用者會自動獲得資料夾中所有現有及後續新增專案的唯讀許可權。

如需詳細資訊，請參閱 [共用資料夾於 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/share-folders.md).

### 檢閱者 {#reviewer}

![cleaner.png](assets/cleaner.png) 可以檢視校訂

![cleaner.png](assets/cleaner.png) 可以新增標籤

![cleaner.png](assets/cleaner.png) 可以新增註解

![[!DNL cleaner].png](assets/cleaner.png) 如果沒有回覆，可以編輯自己的評論

![no.png](assets/no.png) 無法做出決定

![no.png](assets/no.png) 無法編輯或刪除其他人的評論

![no.png](assets/no.png) 沒有校訂的編輯許可權

### 核准者 {#approver}

![cleaner.png](assets/cleaner.png) 可以檢視校訂

![cleaner.png](assets/cleaner.png) 可以做出決定

![no.png](assets/no.png) 無法新增標籤

![no.png](assets/no.png) 無法新增註解

![no.png](assets/no.png) 無法編輯或刪除其他人的評論

![no.png](assets/no.png) 沒有校訂的編輯許可權

### 檢閱者和核准者 {#reviewer-approver}

![cleaner.png](assets/cleaner.png) 可以檢視校訂

![cleaner.png](assets/cleaner.png) 可以新增標籤

![cleaner.png](assets/cleaner.png) 可以新增註解

![[!DNL cleaner].png](assets/cleaner.png) 如果沒有回覆，可以編輯自己的評論

![cleaner.png](assets/cleaner.png) 可以做出決定

![no.png](assets/no.png) 無法編輯或刪除其他人的評論

![no.png](assets/no.png) 沒有校訂的編輯許可權

### 作者 {#author}

![cleaner.png](assets/cleaner.png) 可以新增標籤

![cleaner.png](assets/cleaner.png) 可以新增註解

![[!DNL cleaner].png](assets/cleaner.png) 如果沒有回覆，可以編輯自己的評論

![cleaner.png](assets/cleaner.png) 可以做出決定

![cleaner.png](assets/cleaner.png) 可以提交新版本

![cleaner.png](assets/cleaner.png) 可以建立校訂副本

![cleaner.png](assets/cleaner.png) 可以與其他人共用校訂

![cleaner.png](assets/cleaner.png) 可以對評論套用動作

![cleaner.png](assets/cleaner.png) 可以解析評論

![no.png](assets/no.png) 無法編輯或刪除其他人的評論

>[!NOTE]
>
>此角色只能指派給以下使用者： [!DNL Workfront Proof].

### 仲裁者 {#moderator}

![cleaner.png](assets/cleaner.png) 可以新增標籤

![cleaner.png](assets/cleaner.png) 可以新增註解

![[!DNL cleaner].png](assets/cleaner.png) 如果沒有回覆，可以編輯自己的評論

![cleaner.png](assets/cleaner.png) 可以做出決定

![cleaner.png](assets/cleaner.png) 可以提交新版本

![cleaner.png](assets/cleaner.png) 可以新增檢閱者

![cleaner.png](assets/cleaner.png) 可以對評論套用動作

![cleaner.png](assets/cleaner.png) 可以解析評論

![cleaner.png](assets/cleaner.png) 可以刪除校訂上的評論和回覆（由自己或其他人進行）

* 刪除註解對話串中的第一個註解將刪除整個對話串
* 刪除評論對話串中的回覆只會刪除該回覆

![no.png](assets/no.png) 無法編輯其他人的評論

此角色可讓人員管理和稽核校訂評論，讓他們有機會在校訂上僅保留相關評論並移除不相關評論。

>[!NOTE]
>
>此角色只能指派給以下使用者： [!DNL Workfront Proof].

## 指派校訂角色

建立新校訂、建立現有校訂的新版本或現有校訂時，您可以指派校訂角色。

### 新校訂 {#new-proofs}

校訂角色可指派給上的檢閱者 [!UICONTROL 新校訂] 在校訂建立過程中的頁面(1)。

![Proof_roles_-_New_Proof_page.png](assets/proof-roles---new-proof-page-350x184.png)

### 新版本 {#new-versions}

建立新版本的校訂時，將會自動顯示先前版本的稽核者（具有與先前版本相同的角色）。

建立新版本(1)時，您可以編輯套用到稽核者的校訂角色。

![Proof_roles_-_New_Version_page.png](assets/proof-roles---new-version-page-350x164.png)

### 現有校訂 {#existing-proofs}

如果您想變更某人在現有校訂上的角色，您可以對以下專案進行： [!UICONTROL 校訂詳細資訊] 頁面，方式為在工作流程區段(1)內聯編輯其角色。

![Proof_Roles_-_Proof_Details_page_2.png](assets/proof-roles---proof-details-page-2-350x131.png)

## 在校訂檢視器中檢查角色

您可以直接從「校訂檢視器」(1)檢查檢閱者的角色，並視需要編輯它(2)。

![Proof_roles_-_Proof_Viewer.png](assets/proof-roles---proof-viewer-350x300.png)

## 預設校訂角色

您可以在以下位置設定您的預設校訂角色： [!DNL Proofing Defaults] 頁面（在您的「個人」設定中）。 這表示當您新增至校訂時，將會自動填入您的預設校訂角色。 請注意，此角色可由在校訂上擁有編輯許可權的使用者在校訂層級變更。

>[!NOTE]
>
>只有具有管理員或計費管理員設定檔的使用者才能變更其帳戶中其他使用者的校訂預設值。

如需詳細資訊，請參閱 [中的個人設定 [!DNL Workfront Proof]](../../../workfront-proof/wp-getstarted/personal-settings/personal-settings.md).

## 建立者和擁有者

建立者和擁有者擁有對校訂的完整編輯許可權。

### 建立者 {#creators}

校訂建立者是在第一個例項中上傳校訂的人。 校訂建立者會自動顯示在校訂的人員清單中（在其預設角色中）。

在 [!UICONTROL 新校訂] 頁面您可以將不同的校訂角色指派給校訂建立者（除了其預設角色）。

校訂建立者無法變更或從校訂中移除。

### 擁有者 {#owners}

依預設，建立者也是校訂的擁有者；但是，建立者可以在最初建立校訂時讓他人成為校訂擁有者(位於 [!UICONTROL 新校訂] 頁面)。

若要變更新校訂頁面上的擁有者：

1. 按一下「建立者」名稱旁顯示的變更連結。
1. 從下拉式選單中選取新的擁有者。 (2)

![Proof_roles_-_new_proof_page_change_owner_2.png](assets/proof-roles---new-proof-page-change-owner-2-350x185.png)

建立校訂後，仍可以變更所有者。 擁有校訂編輯許可權的任何人將能夠透過 [!UICONTROL 校訂詳細資訊] 頁面（請參閱下文）。

從工作流程管理的角度來看，變更校訂擁有者的功能特別有用。 它可讓專案負責人取得校訂的所有權，賦予他們編輯校訂的許可權，並可在 [!UICONTROL 我的校訂] 檢視。

若要透過變更校訂的所有者 [!UICONTROL 校訂詳細資訊] 頁面：

* 按一下您要成為「擁有者」之人員名稱旁的「動作」功能表。
* 選取 [!UICONTROL **建立擁有者**] （從下拉式功能表）。
* 或者，您也可以按一下 [!UICONTROL **所有者**] 欄位，並從顯示的下拉式清單中選擇新的擁有者。

完成此操作後，「所有者」字樣將顯示在該人員名稱的旁邊。

>[!NOTE]
>
>只有來自相同帳戶或合作夥伴帳戶的使用者才能成為校訂的擁有者。 只有符合以下條件時，合作夥伴帳戶中的使用者才能成為校訂的擁有者：
>
>* 帳戶之間已設定現有的合作夥伴關係。 如需詳細資訊，請參閱 [中的合作夥伴帳戶 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/partner-accounts/partner-accounts.md).
>* 「 」上沒有自訂欄位 [!UICONTROL 新校訂] 頁面。
>* 校訂尚未指派到資料夾。
>* 尚未將任何標籤套用到校訂。

暫時委派校訂擁有權於 [!DNL Workfront Proof]，請參閱 [指定臨時校訂擁有者 [!DNL Workfront Proof]](../../../workfront-proof/wp-getstarted/personal-settings/designate-temp-proof-owners.md).
