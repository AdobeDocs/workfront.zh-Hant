---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: 了解Workfront校樣中的校樣狀態
description: 在 [!DNL Workfront Proof]，校樣會存在於不同狀態。 這些狀態決定您可以對證明採取哪些動作，例如加上註解或做出決策。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: cd120e53-d6c2-4929-904f-a9f72903f074
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---

# 了解Workfront校樣中的校樣狀態

>[!IMPORTANT]
>
>本文說明獨立產品中的功能 [!DNL Workfront Proof]. 有關內部校對的資訊 [!DNL Adobe Workfront]，請參閱 [校對](../../../review-and-approve-work/proofing/proofing.md).

在 [!DNL Workfront Proof]，校樣會存在於不同狀態。 這些狀態決定您可以對證明採取哪些動作，例如加上註解或做出決策。

## 了解證明狀態

這四種狀態如下：

* [使用中](#active)
* [已鎖定](#locked)
* [草稿（僅限Dropzone）](#draft-dropzone-only)
* [已提交（僅限Dropzone）](#submitted-dropzone-only)

### 使用中 {#active}

上傳至的校樣 [!DNL Workfront Proof] 透過「新校樣」頁面或Dropzone處理後，會顯示為「作用中」。 當校樣為作用中使用者時，可以檢閱、發表意見，並對校樣做出決策。

>[!NOTE]
>
>只有在啟用「提交時啟用校樣」選項時，透過Dropzone上傳的校樣才會顯示為「作用中」。 如果未啟用選項，您必須手動啟用校樣。

如需Dropzone設定的詳細資訊，請參閱 [在 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

### 已鎖定 {#locked}

審核完校樣後，可以鎖定校樣。 鎖定證明表示不能對證明做出更多評論或決定，但證明仍可開啟。

校樣上具有「編輯」權限的任何使用者都可以解除鎖定。

如需權限的詳細資訊，請參閱 [校樣權限設定檔(位於 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

>[!NOTE]
>
>校樣鎖定時，不再傳送電子郵件通知。 例如，如果校樣在截止日期之前被鎖定，則在達到截止日期時不會傳送通知電子郵件。

### 草稿（僅限Dropzone） {#draft-dropzone-only}

當您透過Dropzone提交校樣時，校樣會進入「草稿」狀態，然後管理員才會啟動它。 當它位於繪製區域時，不能對校樣執行任何操作。

### 已提交（僅限Dropzone） {#submitted-dropzone-only}

管理員啟動草稿後，您的校樣會在Dropzone中顯示為「已提交」。 提交後，您可以對校樣採取動作。

## 查看和更改校樣狀態

如需檢視特定狀態中所有校樣的清單（例如檢視所有「使用中」或「鎖定」校樣）的相關資訊，請參閱 [管理中檢視頁面上的項目 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md) 在文章中 [管理中檢視頁面上的項目 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. 存取 [!DNL Workfront Proof] 控制面板。

   如需詳細資訊，請參閱 [存取 [!DNL Workfront Proof] 從Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

1. 在 **[!UICONTROL 控制面板]**，按一下 **[!UICONTROL 展開]** 要查看或更改狀態的校樣旁邊的箭頭。

   ![](assets/screen-shot-2018-05-02-at-11.31.29-am-350x85.png)

   此 **[!UICONTROL 工作流程程式]** 的上界。

   ![](assets/screen-shot-2018-05-02-at-11.33.20-am-350x226.png)

1. 檢視 **[!UICONTROL 狀態]** 在 **[!UICONTROL 工作流程程式]**.

1. （可選）要更改狀態，請將滑鼠移到當前 **[!UICONTROL 狀態]** 按一下下拉式功能表，然後選取新狀態。

   ![](assets/screen-shot-2018-05-02-at-11.35.30-am.png)
