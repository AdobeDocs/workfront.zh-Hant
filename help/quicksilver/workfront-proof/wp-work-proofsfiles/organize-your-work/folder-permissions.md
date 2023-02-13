---
content-type: reference
product-previous: workfront-proof
product-area: documents
navigation-topic: organize-your-work-workfront-proof
title: 了解 [!DNL Workfront Proof]
description: 如果人員有權查看資料夾中的項目，他們也可以查看資料夾本身。 但是，他們只能看到資料夾中已明確與其共用的項目。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 96162fe8-eef9-40f4-bc94-02911b970f02
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 17%

---

# 了解 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>本文說明獨立產品中的功能 [!DNL Workfront Proof]. 有關內部校對的資訊 [!DNL Adobe Workfront]，請參閱 [校對](../../../review-and-approve-work/proofing/proofing.md).

如果人員有權查看資料夾中的項目，他們也可以查看資料夾本身。 但是，他們只能看到資料夾中已明確與其共用的項目。

## 公用資料夾

如果資料夾為公用資料夾，帳戶中的使用者（不包括觀察者和輕型使用者）可以在左側邊欄中看到資料夾名稱。

您的權限設定檔也會影響您對公用資料夾的權限：

| **設定檔/動作** | **查看資料夾中的所有項** | **查看與其顯式共用的項目** | **新增項目** | **刪除項目** | **添加子資料夾** | **刪除子資料夾** | **編輯資料夾詳細資訊** |
|---|---|---|---|---|---|---|---|
| **建立者** | 是 | 是 | 是 | 是 | 是 | 是 | 是 |
| **帳單管理員** | 是 | 是 | 是 | 是 | 是 | 是 | 是 |
| **管理員** | 是 | 是 | 是 | 是 | 是 | 是 | 是 |
| **主管** | 是 | 是 | 是 | 是 | 是 | 是 | 是 |
| **經理** | 否 | 是 | 是 | 否 | 是 | 否 | 是 |
| **觀察者** | 否 | 是 | 否 | 否 | 否 | 否 | 否 |

{style=&quot;table-layout:auto&quot;}

如果公用資料夾歸經理所有，則可以刪除根資料夾和任何子資料夾。

如需詳細資訊，請參閱 [校樣權限設定檔(位於 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

## 專用資料夾

如果資料夾為專用資料夾，則同一帳戶中的其他用戶將無法在左側邊欄中查看資料夾的名稱，除非資料夾中的資料夾或項目已與他們顯式共用，或者他們具有主管、管理員或計費管理員的配置檔案：

| **設定檔/動作** | **查看資料夾中的所有項** | **查看與其顯式共用的項目** | **新增項目** | **刪除項目** | **添加子資料夾** | **刪除子資料夾** | **編輯資料夾詳細資訊** |
|---|---|---|---|---|---|---|---|
| **建立者** | 是 | 是 | 是 | 是 | 是 | 是 | 是 |
| **帳單管理員** | 是 | 是 | 是 | 是 | 是 | 是 | 是 |
| **管理員** | 是 | 是 | 是 | 是 | 是 | 是 | 是 |
| **主管** | 是 | 是 | 是 | 是 | 是 | 是 | 是 |
| **經理** | 否 | 是 | 否 | 否 | 否 | 否 | 否 |
| **觀察者** | 否 | 是 | 否 | 否 | 否 | 否 | 否 |

{style=&quot;table-layout:auto&quot;}

例如，如果您希望項目經理及其團隊只查看特定資料夾，則項目經理可以設定私人資料夾，然後與特定用戶共用該資料夾。

共用私人資料夾時，您可以決定是否要讓管理員能夠建立、編輯和刪除資料夾項目。

您可以在「新資料夾」頁面上，個別為每個人設定此項目，並在 [!UICONTROL 共用給] 區段。 如需詳細資訊，請參閱 [在中建立資料夾 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md) 和 [在中管理資料夾及其內容 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders-and-contents.md).

如果與或觀察者共用私人資料夾，他們將具有對資料夾中所有項目的唯讀存取權。 如需詳細資訊，請參閱 [校樣權限設定檔(位於 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) 和 [在中共用資料夾 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/share-folders.md).

>[!NOTE]
>
>* 如果父資料夾為專用資料夾，則所有子資料夾也將為專用資料夾。 私人父資料夾下不能有公用子資料夾。 但是，您可以在公用父資料夾下方有私人子資料夾。
>* 資料夾的建立者和擁有者將一律有權存取該資料夾，且不可移除。
>* 只有私人資料夾的「建立者」和「擁有者」才能刪除資料夾。


