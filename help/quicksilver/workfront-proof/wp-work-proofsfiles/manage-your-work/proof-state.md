---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: 瞭解Workfront Proof中的校訂狀態
description: 在 [!DNL Workfront Proof]中，校樣以不同的狀態存在。 這些狀態會決定您可以對校訂採取哪些動作，例如評論或決策。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: cd120e53-d6c2-4929-904f-a9f72903f074
source-git-commit: ddaee5b339982c826c14b67775d81f3a2bd7bc37
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 0%

---

# 瞭解Workfront Proof中的校訂狀態

>[!IMPORTANT]
>
>本文提及獨立產品[!DNL Workfront Proof]中的功能。 有關[!DNL Adobe Workfront]內部校訂的資訊，請參閱[校訂](../../../review-and-approve-work/proofing/proofing.md)。

在[!DNL Workfront Proof]中，校樣以不同的狀態存在。 這些狀態會決定您可以對校訂採取哪些動作，例如評論或決策。

## 瞭解校訂狀態

四種狀態如下：

* [作用中](#active)
* [已鎖定](#locked)
* [草稿（僅限下拉區域）](#draft-dropzone-only)
* [已提交（僅限Dropzone）](#submitted-dropzone-only)

### 作用中 {#active}

透過新校訂頁面或拖放區域上傳至[!DNL Workfront Proof]的校訂在處理後會顯示為作用中。 當校訂為作用中時，使用者可以對校訂進行檢閱、評論和決策。

>[!NOTE]
>
>只有在啟用「提交時啟動校訂」選項時，透過Dropzone上傳的校訂才會顯示為「作用中」。 如果未啟用選項，您必須手動啟動校訂。

如需Dropzone設定的詳細資訊，請參閱[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md)中設定dropzone。

### 已鎖定 {#locked}

檢閱完校訂後，您可以鎖定校訂。 鎖定校訂表示校訂上無法再做出評論或決定，但校訂仍可開啟。

任何對校樣具有編輯許可權的使用者都可以將其解鎖。

如需許可權的詳細資訊，請參閱 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)中的[校訂許可權設定檔。

>[!NOTE]
>
>鎖定校訂時不再傳送電子郵件通知。 例如，如果在截止日期前鎖定校訂，則到達截止日期時不會傳送通知電子郵件。

### 草稿（僅限下拉區域） {#draft-dropzone-only}

當您透過Dropzone提交校訂時，它會在管理員啟動之前進入草稿狀態。 當它位於草稿區域中時，您無法對校樣採取任何動作。

### 已提交（僅限Dropzone） {#submitted-dropzone-only}

管理員啟動草稿後，您的校訂在拖放區域中顯示為「已提交」。 提交校訂後，您可以對校訂執行操作。

## 檢視和變更校訂狀態

如需有關檢視處於特定狀態之所有校訂清單的資訊，例如檢視所有作用中或鎖定的校訂，請參閱 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md)中檢視頁面上的[管理專案一文中的[管理檢視頁面上的專案 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md)。

1. 存取您的[!DNL Workfront Proof]儀表板。

   如需詳細資訊，請參閱[從Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md)存取 [!DNL Workfront Proof] 。

1. 在&#x200B;**[!UICONTROL 儀表板]**&#x200B;上，按一下您要檢視或變更其狀態的校訂旁的&#x200B;**[!UICONTROL 展開]**&#x200B;箭頭。

   ![展開](assets/screen-shot-2018-05-02-at-11.31.29-am-350x85.png)

   **[!UICONTROL 工作流程處理序]**&#x200B;區段隨即顯示。

   ![工作流程處理序](assets/screen-shot-2018-05-02-at-11.33.20-am-350x226.png)

1. 檢視&#x200B;**[!UICONTROL 工作流程處理序]**&#x200B;中的&#x200B;**[!UICONTROL 狀態]**。

1. （選擇性）若要變更狀態，請將滑鼠移至目前的&#x200B;**[!UICONTROL 狀態]**&#x200B;上，然後按一下下拉式功能表，然後選取新的狀態。

   ![新狀態](assets/screen-shot-2018-05-02-at-11.35.30-am.png)
