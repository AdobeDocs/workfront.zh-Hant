---
filename: manage-fusion-users
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: 管理 [!DNL Adobe Workfront Fusion] 您組織中的使用者
description: 管理 [!DNL Adobe Workfront Fusion] 您組織中的使用者
author: Becky
feature: Workfront Fusion
exl-id: fbb858a6-1230-41b4-892a-4ffeb2711922
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 0%

---

# 管理 [!DNL Adobe Workfront Fusion] 您組織中的使用者

[!DNL Adobe Workfront Fusion] 管理員可在內管理使用者角色 [!DNL Workfront Fusion].

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on adding a user in the Adobe Admin Console:
>
>* See [Add a user to an organization in Adobe Workfront Fusion](../../workfront-fusion/organizations/add-user-to-an-organization.md#create)
>* See the section "Add users" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html)
>* Contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront Fusion/Adobe Business Platform)](../../workfront-fusion/fusion-in-admin-console/fusion-adobe-admin-console.md).

-->

## 存取需求

您必須具備下列存取權才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
   <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
    <td> <p>[!UICONTROL計畫]、[!UICONTROL工作]</p> </td> 
   </tr>
   <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]授權**</td> 
   <td> <p>Workfront Fusion for Work Automation and Integration,</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>貴組織必須購買 [!DNL Adobe Workfront Fusion] 和 [!DNL Adobe Workfront] 以使用本文所述的功能。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> 
     <p>您必須是 [!DNL Workfront Fusion] 管理員。</p>
     <p>您必須是 [!DNL Workfront Fusion] 管理員。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

如需 [!DNL Adobe Workfront Fusion] 許可證，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 查看或編輯用戶角色 {#view}

[!DNL Adobe Workfront Fusion] 管理員可以檢視和更新使用者角色。

1. 以 [!DNL Workfront Fusion] 管理員，選擇 **[!UICONTROL 使用者]** 的下一頁。
1. 按一下 **[!UICONTROL 詳細資料]** 在您要檢視的使用者列中。
1. （可選）若要更新使用者角色，請按一下 **[!DNL Role]** 列，在要更改用戶角色的組織行中，然後選擇新角色。

## 查看或編輯用戶詳細資訊 {#view2}

[!DNL Adobe Workfront Fusion] 管理員可以檢視和更新使用者詳細資訊。

1. 以 [!DNL Workfront Fusion] 管理員，選擇 **[!UICONTROL 使用者]** 的下一頁。
1. 按一下 **[!UICONTROL 詳細資料]** 在您要檢視的使用者列中。
1. （選用）若要更新使用者的詳細資訊，請按一下 **[!UICONTROL 選項]** 在畫面的右上角，選取 **[!UICONTROL 變更詳細資訊]**.

## 刪除使用者 {#delete}

[!DNL Adobe Workfront Fusion] 管理員可以刪除使用者。

1. 以 [!DNL Workfront Fusion] 管理員，選擇 [!UICONTROL 使用者] 的下一頁。
1. 按一下 **[!UICONTROL 詳細資料]** 在您要檢視的使用者列中。
1. （選用）若要更新使用者的詳細資訊，請按一下 **[!UICONTROL 選項]** 在畫面的右上角，選取 **[!UICONTROL 刪除]**.

### 在Workfront Fusion中刪除使用者時的考量事項

* 刪除用戶後，將刪除用戶的連接、密鑰和Webhook。 屬於用戶的任何方案都將轉移給組織責任人。 這些情況下的連接必須更新，因為屬於用戶的連接不再有效。
* 如果刪除的用戶擁有任何應用程式或公共模板，則應用程式或公共模板將轉移到組織所有者。 如果沒有組織所有者，則應用程式或公共模板將轉移給其他用戶。
