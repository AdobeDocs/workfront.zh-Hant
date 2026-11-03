---
user-type: administrator
product-area: system-administration;setup;user-management
navigation-topic: configure-proofing-functionality
title: 設定使用者的校訂存取權
description: 身為Adobe Workfront管理員或Workfront Proof管理員，您可以設定使用者在Workfront和Workfront Proof中建立和檢視校訂的存取權。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 98c90139-f31a-41bc-af0b-577dd8b254e3
TQID: 'https://experienceleague.adobe.com/L-AMDvQYgtXJwxmtwekimbEA9OQQN72QHIcoQ2iKzGU'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4ea8bc003ce17978be5e5a6fd838012dfcfeae78
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 3%
---
# 設定使用者的校訂存取權

身為Adobe Workfront管理員或Workfront Proof管理員，您可以設定使用者在Workfront和Workfront Proof中建立和檢視校訂的存取權。

如需可用於基本與整合校訂之校訂功能的相關資訊，請參閱[存取Workfront中的校訂功能](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md)。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td>規劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>您必須是Workfront管理員或Workfront Proof管理員。 如需Workfront管理員的相關資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整管理存取權</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

+++

<!--

## Configure a user's proof permission profile

The permission profile you select is granted to the users for each proof that exists within your organization.

{{step-1-to-users}}
 
1. Select one or more users, then click **Edit**.  

1. In the **Access** section, click one of the following Workfront Proof permission options in the **Proof Permission Profile** drop-down menu:

   >[!NOTE]
   >
   >If you are on a legacy Workfront plan, make sure the **User can generate proofs** option is enabled, as explained above in the section [Enable and disable proofing for a user (legacy plans only)](#enable-and-disable-proofing-for-a-user-legacy-plans-only). 

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Supervisor</strong> </td> 
      <td>Users can manage and view all proofs created on your organization's account. They can also edit reviewers added to these proofs. Users with this permission profile can't manage users or edit Workfront Proof settings.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Manager</strong> </td> 
      <td> <p> Users can manage and view proofs created or owned on your organization's account. They can view other users' proofs only when added as a reviewer. This is a default setting. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Administrator</strong> </td> 
      <td> Users are given Administrator permissions in Workfront Proof and can edit account settings. Users can manage and view all proofs created on your organization's account. This includes adding and removing reviewers, proofs, and comments.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Custom</strong> </td> 
      <td> <p>Available only if you have configured a custom permission profile within Workfront Proof.</p> <p><b>NOTE</b>:  <p>Ensure that the permission profile you grant here does not provide higher access than the user's Access Level setting in Workfront (see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>). If it does provide higher access, the user can access proofs within Workfront Proof that he or she cannot access within Workfront.</p> <p>This is especially important if you plan to allow all Workfront users to access Workfront Proof directly from the Workfront as described in <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md" class="MCXref xref">Access Workfront Proof from Adobe Workfront</a>.</p> <p>By default, only Workfront administrators have access to a direct link to the Workfront Proof site from the Workfront Global Navigation Bar.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   The permission profile you select is granted to the users for each proof that exists within your organization.

1. Click **Save Changes** to complete the update to the user settings.

   >[!NOTE]
   >
   >When you create or update a user in Workfront and the user's Workfront email address matches that of a licensed Workfront Proof user, the system enables proofing for the user within Workfront. For more information, see [User synchronization between Adobe Workfront and Workfront Proof](../../../administration-and-setup/manage-workfront/configure-proofing/user-sync-proofing.md).

### Considerations

Consider the following information when setting permissions:

* If you change a user's permission profile to a profile with fewer permissions, the user might lose visibility to existing proofs within Workfront. This can occur when someone shares a task with a user within Workfront, but doesn't share the proof attached to the task (see [Share a proof within Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) in [Share a proof within Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)).
* You can set Workfront Proof permissions from Workfront only if your Workfront environment is integrated with a Workfront Proof Premium account. If you cannot use proofing as discussed in this section, contact your Workfront administrator.
* At least one user in your Workfront environment must have Administrator permissions for proofing. An error message appears if you try to attempt to remove Administrator permissions for proofing from all users.
* When you change a user's Workfront Access level to any level other than System Administrator, the user's Workfront Proof permission profile defaults to Manager.   

* When you change the Workfront Access level to System Administrator, the Proof Permission profile changes to Administrator.

-->

## 透過Workfront主要功能表為所有使用者設定Workfront Proof存取權 {#configure-workfront-proof-access-via-workfront-main-menu-for-all-users}

依預設，只有在Workfront內具有管理許可權的使用者才能存取Workfront Proof，如所述[從Adobe Workfront存取Workfront Proof](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md)。

您可以聯絡Workfront Proof支援並提交請求，藉此向所有使用者授予Workfront主功能表內Workfront按鈕的存取權。

>[!IMPORTANT]
>
> 如果您打算允許所有Workfront使用者直接從Workfront全域導覽列存取Workfront Proof，請確認每位使用者的許可權設定檔所提供的存取權，不會超過該使用者在Workfront中的存取層級。 這可防止使用者存取Workfront Proof中他們無法在Workfront中存取的校訂。 如需詳細資訊，請參閱[啟用和停用使用者的校訂（僅限舊版計畫）](#enable-and-disable-proofing-for-a-user-legacy-plans-only)。

## 設定案頭校訂檢視器的使用者存取權

如果您組織中的使用者偏好使用「案頭校訂檢視器」而不是「網頁校訂檢視器」來檢閱互動式內容，您可以將「案頭校訂檢視器」設定為在使用者開啟互動式內容校訂時自動啟動。 如需有關這個案頭校訂檢視器的資訊，以及它與Web校訂檢視器的差異，請參閱[瞭解案頭校訂檢視器](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md)和[網頁校訂檢視器與案頭校訂檢視器之間的差異](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md)。

1. 從Workfront，按一下全域導覽列中的Workfront Proof圖示以存取Workfront Proof。

   ![校訂圖示](assets/proof-access-proofhq-350x39.png)

1. 按一下Workfront Proof右上角附近的&#x200B;**帳戶設定**，然後按一下&#x200B;**設定**&#x200B;標籤。

1. 在&#x200B;**校訂預設值**&#x200B;下，在&#x200B;**互動式校訂的案頭校訂檢視器**&#x200B;列的結尾處，按一下&#x200B;**設定**。

1. 修改案頭校訂檢視器設定，如[案頭校訂檢視器](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#desktop-proofing-viewer)文章[設定組織的校訂設定](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md)中所述。

1. 按一下「**儲存**」。

## 設定互動式校樣的自訂裝置

您可以將任何自訂裝置新增到系統中，讓使用者檢閱互動式內容，並模擬內容在使用「案頭校訂檢視器」時顯示在特定裝置上的方式。 (此功能無法在Web Proofing Viewer （使用者可以在其中檢閱互動式內容）中使用，但只能以各種解析度顯示，不能用於各種裝置。)

如需詳細資訊，請參閱[在校訂檢視器中變更互動式校訂解析度](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md)。

1. 從Workfront存取Workfront Proof介面，如[從Adobe Workfront存取Workfront Proof](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md)中所述。
1. 修改案頭校訂檢視器設定，如[設定組織的校訂設定](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md)文章中的[設定校訂的自訂裝置](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#custom-devices-for-proofs)中所述。
