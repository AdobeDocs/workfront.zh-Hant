---
product-previous: workfront-proof
product-area: documents
navigation-topic: share-proofs-and-files
title: 在中管理校樣角色 [!DNL Workfront Proof]
description: 校樣角色可讓您授予受其使用者設定檔上設定之權限設定檔所限制的使用者權限。 (如需權限設定檔的詳細資訊，請參閱 [!DNL Workfront Proof].)
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: b371cc20-4226-49ce-96c6-9815b2e84713
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1343'
ht-degree: 1%

---

# 在中管理校樣角色 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>本文說明獨立產品中的功能 [!DNL Workfront Proof]. 有關內部校對的資訊 [!DNL Adobe Workfront]，請參閱 [校對](../../../review-and-approve-work/proofing/proofing.md).

校樣角色可讓您授予受其使用者設定檔上設定之權限設定檔所限制的使用者權限。 (如需權限設定檔的詳細資訊，請參閱 [校樣權限設定檔(位於 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).)

校樣角色與帳戶設定檔不同。 您的帳戶設定檔會與您帳戶中的整體權限層級相關，並且會影響您對帳戶中所有證明（甚至未明確與您共用的證明）所擁有的權限。

如需詳細資訊，請參閱 [校樣權限設定檔(位於 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

## 關於校樣角色

在邀請使用者檢閱校樣時，系統會為個別校樣授予使用者下列校樣角色：

* [唯讀](#read-only)
* [檢閱者](#reviewer)
* [核准者](#approver)
* [檢閱者和核准者](#reviewer-approver)
* [作者](#author)
* [仲裁者](#moderator)

校樣角色定義審核者可針對該特定校樣採取的動作。

例如，如果您是審核者，系統會要求您新增標籤和註解以檢閱校樣。 如果您是審核者和核准者，系統會要求您檢閱並決定校樣。

某些校樣角色賦予審核者校樣的編輯權限（即使其帳戶設定檔沒有），並可讓他們使用一些額外功能，例如新增註解的動作、建立新版本以及新增更多審核者至校樣。

如需詳細資訊，請參閱下列文章：

* [對校樣注釋使用動作](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md)
* [在中共用校樣 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md)

### 唯讀

{#read-only}

![cleaner.png](assets/cleaner.png) 可以檢視校樣

![no.png](assets/no.png) 無法添加標籤

![no.png](assets/no.png) 無法添加註釋

![no.png](assets/no.png) 無法做出決定

![no.png](assets/no.png) 無法刪除其他人的注釋

![no.png](assets/no.png) 對校樣沒有編輯權限

>[!NOTE]
>
>如果資料夾已與 [!DNL Workfront Proof]，則會自動為資料夾中所有現有及隨後新增的項目授予唯讀權限。

如需詳細資訊，請參閱 [在中共用資料夾 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/share-folders.md).

### 檢閱者 {#reviewer}

![cleaner.png](assets/cleaner.png) 可以檢視校樣

![cleaner.png](assets/cleaner.png) 可以新增標籤

![cleaner.png](assets/cleaner.png) 可以添加註釋

![[!DNL cleaner].png](assets/cleaner.png) 如果沒有回覆，可以編輯自己的留言

![no.png](assets/no.png) 無法做出決定

![no.png](assets/no.png) 無法編輯或刪除其他人的注釋

![no.png](assets/no.png) 對校樣沒有編輯權限

### 核准者 {#approver}

![cleaner.png](assets/cleaner.png) 可以檢視校樣

![cleaner.png](assets/cleaner.png) 可以做決定

![no.png](assets/no.png) 無法添加標籤

![no.png](assets/no.png) 無法添加註釋

![no.png](assets/no.png) 無法編輯或刪除其他人的注釋

![no.png](assets/no.png) 對校樣沒有編輯權限

### 檢閱者和核准者 {#reviewer-approver}

![cleaner.png](assets/cleaner.png) 可以檢視校樣

![cleaner.png](assets/cleaner.png) 可以新增標籤

![cleaner.png](assets/cleaner.png) 可以添加註釋

![[!DNL cleaner].png](assets/cleaner.png) 如果沒有回覆，可以編輯自己的留言

![cleaner.png](assets/cleaner.png) 可以做決定

![no.png](assets/no.png) 無法編輯或刪除其他人的注釋

![no.png](assets/no.png) 對校樣沒有編輯權限

### 作者 {#author}

![cleaner.png](assets/cleaner.png) 可以新增標籤

![cleaner.png](assets/cleaner.png) 可以添加註釋

![[!DNL cleaner].png](assets/cleaner.png) 如果沒有回覆，可以編輯自己的留言

![cleaner.png](assets/cleaner.png) 可以做決定

![cleaner.png](assets/cleaner.png) 可以提交新版本

![cleaner.png](assets/cleaner.png) 可以建立校樣的副本

![cleaner.png](assets/cleaner.png) 可以和其他人分享證明

![cleaner.png](assets/cleaner.png) 可以對注釋應用操作

![cleaner.png](assets/cleaner.png) 可以解析注釋

![no.png](assets/no.png) 無法編輯或刪除其他人的注釋

>[!NOTE]
>
>此角色只能指派給 [!DNL Workfront Proof]

### 仲裁者 {#moderator}

![cleaner.png](assets/cleaner.png) 可以新增標籤

![cleaner.png](assets/cleaner.png) 可以添加註釋

![[!DNL cleaner].png](assets/cleaner.png) 如果沒有回覆，可以編輯自己的留言

![cleaner.png](assets/cleaner.png) 可以做決定

![cleaner.png](assets/cleaner.png) 可以提交新版本

![cleaner.png](assets/cleaner.png) 可以添加新審閱者

![cleaner.png](assets/cleaner.png) 可以對注釋應用操作

![cleaner.png](assets/cleaner.png) 可以解析注釋

![cleaner.png](assets/cleaner.png) 可以刪除對證明的評論和回覆（由自己或他人提出）

* 刪除注釋線程中的第一個注釋將刪除整個線程
* 刪除評論線程中的回復將僅刪除該回復

![no.png](assets/no.png) 無法編輯其他人的注釋

此角色可讓人員管理並協調校樣意見，讓他們只保留校樣的相關意見，並移除非相關的意見。

>[!NOTE]
>
>此角色只能指派給 [!DNL Workfront Proof].

## 分配校樣角色

您可以在建立新校樣、建立新版本的現有校樣或現有校樣時指派校樣角色。

* [新校樣](#new-proofs)
* [新版本](#new-versions)
* [現有校樣](#existing-proofs)

### 新校樣 {#new-proofs}

校樣角色可指派給 [!UICONTROL 新校樣] 頁面(1)。

![Proof_roles_-_New_Proof_page.png](assets/proof-roles---new-proof-page-350x184.png)

### 新版本 {#new-versions}

建立校樣的新版本時，將自動顯示來自舊版的審閱者（與舊版的角色相同）。

建立新版本(1)時，您可以編輯套用至審核者的校樣角色。

![Proof_roles_-_New_Version_page.png](assets/proof-roles---new-version-page-350x164.png)

### 現有校樣 {#existing-proofs}

如果您想在現有校樣上變更人員的角色，可以在 [!UICONTROL 校樣詳細資料] 內嵌編輯其在工作流程區段中的角色，以建立頁面(1):

![Proof_Roles_-_Proof_Details_page_2.png](assets/proof-roles---proof-details-page-2-350x131.png)

## 在校樣檢視器中檢查角色

您可以直接從校樣檢視器(1)檢查審核者的角色，並視需要編輯(2)。

![Proof_roles_-_Proof_Viewer.png](assets/proof-roles---proof-viewer-350x300.png)

## 預設校樣角色

您可以在 [!DNL Proofing Defaults] 頁面。 這表示將您新增至校樣時，系統會自動填入您的預設校樣角色。 請注意，具有校樣編輯權限的使用者可在校樣層級變更此角色。

>[!NOTE]
>
>只有具有管理員或帳單管理員設定檔的使用者才能變更其帳戶中其他使用者的校對預設值。

如需詳細資訊，請參閱 [中的個人設定 [!DNL Workfront Proof]](../../../workfront-proof/wp-getstarted/personal-settings/personal-settings.md).

## 建立者和擁有者

建立者和擁有者對校樣具有完整的編輯權限。

* [製作者](#creators)
* [擁有者](#owners)

### 製作者 {#creators}

校樣建立者是在第一個執行個體上傳校樣的人。 校樣建立者會自動顯示在校樣的人員清單中（在其預設角色中）。

在 [!UICONTROL 新校樣] 頁面，您可以將不同的校樣角色指派給校樣建立者（其預設角色除外）。

無法更改校樣建立器或從校樣中刪除校樣建立器。

### 擁有者 {#owners}

預設情況下，建立者也是校樣的所有者；但是，建立者可以在最初建立校樣時，將其他人設為校樣擁有者(位於 [!UICONTROL 新校樣] 頁面)。

要更改「新校樣」頁上的「所有者」：

1. 按一下建立者名稱旁顯示的變更連結。
1. 從下拉式功能表中選取新的擁有者。 (2)

![Proof_roles_-_new_proof_page_change_owner_2.png](assets/proof-roles---new-proof-page-change-owner-2-350x185.png)

校樣建立後，仍可變更擁有者。 任何對校樣具有編輯權限的人，都可以透過 [!UICONTROL 校樣詳細資料] 頁面（請參閱下方）。

從工作流管理的角度來看，變更校樣擁有者的功能特別實用。 它可讓專案負責者接管校樣的所有權，讓校樣擁有編輯權限，並能在 [!UICONTROL 我的校樣] 檢視。

若要透過 [!UICONTROL 校樣詳細資料] 頁面：

* 按一下您要成為擁有者之人員名稱旁的「動作」功能表
* 選擇 [!UICONTROL 成為所有者] 從下拉式功能表。
* 或者，您也可以按一下 [!UICONTROL 擁有者] 欄位，然後從顯示的下拉式清單中選擇新的「擁有者」。

完成此操作後，該人員的名稱旁會顯示「擁有者」一字。

>[!NOTE]
>
>只有來自相同帳戶或合作夥伴帳戶的使用者才能成為校樣的擁有者。 只有符合以下條件時，合作夥伴帳戶中的使用者才能成為校樣的擁有者：
>
>* 帳戶之間設定了現有的合作夥伴關係。 如需詳細資訊，請參閱 [合作夥伴帳戶 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/partner-accounts/partner-accounts.md).
>* 上沒有自訂欄位 [!UICONTROL 新校樣] 頁面。
>* 校樣尚未指派給資料夾。
>* 未對校樣套用標籤。
>




在中臨時委派校樣所有權 [!DNL Workfront Proof]，請參閱 [在中指定臨時校樣所有者 [!DNL Workfront Proof]](../../../workfront-proof/wp-getstarted/personal-settings/designate-temp-proof-owners.md).
