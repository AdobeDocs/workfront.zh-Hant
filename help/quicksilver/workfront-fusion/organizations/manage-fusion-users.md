---
filename: manage-fusion-users
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: 管理組織中的 [!DNL Adobe Workfront Fusion] 位使用者
description: 管理組織中的 [!DNL Adobe Workfront Fusion] 位使用者
author: Becky
feature: Workfront Fusion
exl-id: fbb858a6-1230-41b4-892a-4ffeb2711922
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# 管理貴組織中的[!DNL Adobe Workfront Fusion]位使用者

[!DNL Adobe Workfront Fusion]管理員可以管理[!DNL Workfront Fusion]內的使用者角色。

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

您必須具有下列存取權才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 計畫*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
   <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
    <td> <p>[！UICONTROL計畫]，[！UICONTROL工作]</p> </td> 
   </tr>
   <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront Fusion]授權**</td> 
   <td>
   <p>目前授權需求：無[!DNL Workfront Fusion]授權需求。</p>
   <p>或</p>
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]，[！UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]計畫，您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]計畫中。</p>
   <p>或</p>
   <p>舊版產品需求：您的組織必須購買[!DNL Adobe Workfront Fusion]及[!DNL Adobe Workfront]，才能使用本文所述的功能。</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">存取層級設定*</td> 
   <td> 
     <p>您必須是組織的[!DNL Workfront Fusion]管理員。</p>
     <p>您必須是團隊的[!DNL Workfront Fusion]管理員。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

如需[!DNL Adobe Workfront Fusion]授權的相關資訊，請參閱[[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 檢視或編輯使用者角色 {#view}

[!DNL Adobe Workfront Fusion]管理員可以檢視和更新使用者角色。

1. 以[!DNL Workfront Fusion]管理員身分登入時，請在左側導覽中選取&#x200B;**[!UICONTROL 使用者]**。
1. 在您要檢視的使用者列中，按一下&#x200B;**[!UICONTROL 詳細資料]**。
1. （可選）若要更新使用者的角色，請在您要變更使用者角色的組織列中，按一下&#x200B;**[!DNL Role]**&#x200B;欄中的下拉式清單，然後選取新角色。

## 檢視或編輯使用者詳細資訊 {#view2}

[!DNL Adobe Workfront Fusion]管理員可以檢視和更新使用者詳細資訊。

1. 以[!DNL Workfront Fusion]管理員身分登入時，請在左側導覽中選取&#x200B;**[!UICONTROL 使用者]**。
1. 在您要檢視的使用者列中，按一下&#x200B;**[!UICONTROL 詳細資料]**。
1. （選擇性）若要更新使用者的詳細資料，請按一下畫面右上角的&#x200B;**[!UICONTROL 選項]**，然後選取&#x200B;**[!UICONTROL 變更詳細資料]**。

## 刪除使用者 {#delete}

[!DNL Adobe Workfront Fusion]管理員可以刪除使用者。

1. 以[!DNL Workfront Fusion]管理員身分登入時，請在左側導覽中選取[!UICONTROL 使用者]。
1. 在您要檢視的使用者列中，按一下&#x200B;**[!UICONTROL 詳細資料]**。
1. （選擇性）若要更新使用者的詳細資料，請按一下畫面右上角的&#x200B;**[!UICONTROL 選項]**，然後選取&#x200B;**[!UICONTROL 刪除]**。

### 在Workfront Fusion中刪除使用者時的注意事項

* 刪除使用者時，會移除使用者的連線、金鑰和Webhook。 屬於使用者的任何案例都會轉移給組織「擁有者」。 必須更新這些案例中的連線，因為屬於使用者的連線已無效。
* 如果刪除的使用者擁有任何應用程式或公用範本，則應用程式或公用範本會轉移至組織「擁有者」。 如果沒有組織「擁有者」，則應用程式或公用範本會轉讓給其他使用者。
