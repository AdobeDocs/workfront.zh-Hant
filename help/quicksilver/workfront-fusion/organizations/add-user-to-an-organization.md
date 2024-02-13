---
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: 在Adobe Workfront Fusion中新增使用者至組織
description: 您可以在Adobe Workfront Fusion中新增使用者至組織。
author: Becky
feature: Workfront Fusion
exl-id: 98248cca-98f5-4eb5-b203-67e261df33f1
source-git-commit: 5d4434d090c4b6cdefc9c313fecccf6d6e9a510b
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 0%

---

# 在Adobe Workfront Fusion中新增使用者至組織

>[!IMPORTANT]
>
>此頁面中說明的程式僅適用於尚未加入的組織。 [!DNL Adobe Admin Console]. 如果您的組織已上線至 [!DNL Adobe Admin Console]，您必須透過 [!DNL Adobe Admin Console].
>
>有關在中新增使用者的指示[!DNL  Adobe Admin Console]，請參閱文章中的「編輯使用者詳細資訊」一節 [個別管理使用者](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) 或聯絡 [!UICONTROL Adobe Admin Console] 管理員。
>
>如需根據貴組織是否已加入Adobe Admin Console而有所差異的程式清單，請參閱 [平台型管理差異(Adobe Workfront Fusion/Adobe Business Platform)](../../../quicksilver/workfront-fusion/fusion-in-admin-console/fusion-in-admin-console.md).

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
   <p>目前授權需求：否 [!DNL Workfront Fusion] 授權需求。</p>
   <p>或</p>
   <p>舊版授權需求： [！UICONTROL [!DNL Workfront Fusion] 工作自動化與整合]，請參閱[！UICONTROL [!DNL Workfront Fusion] 工作自動化專用]</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">產品</td> 
   <td>
   <p>目前產品需求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 計畫，您的組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述的功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 計畫。</p>
   <p>或</p>
   <p>舊版產品需求：貴組織必須購買 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文所述的功能。</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">存取層級設定*</td> 
   <td> 
     <p>您必須是 [!DNL Workfront Fusion] 您組織的管理員。</p>
     <p>您必須是 [!DNL Workfront Fusion] 您團隊的管理員。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

有關的資訊 [!DNL Adobe Workfront Fusion] 授權，請參閱 [[!DNL Adobe Workfront Fusion] 授權](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 將使用者新增至組織


<!--
<p>The procedure to add a user to your Fusion organization differs based on whether your organization has been onboarded to the Adobe Business Platform. </p>
<ul>
<li> <p><a href="#add-a-user-to-an-organization-that-has-been-onboarded-to-the-adobe-business-platform" class="MCXref xref">Add a user to an organization that has been onboarded to the Adobe Business Platform</a> </p> </li>
<li> <p><a href="#add-a-user-to-an-organization-that-has-not-been-onboarded-to-the-adobe-business-console" class="MCXref xref">Add a user to an organization that has not been onboarded to the Adobe Business Console</a> </p> </li>
</ul>
<div>
<p><strong>Add a user to an organization that has been onboarded to the Adobe Business Platform</strong></p>
<p>If your organization has been onboarded to the Adobe Business Platform, you must perform this action through the Adobe Admin Console.</p>
<p>For instructions on adding a user in the Adobe Admin Console:</p>
<ul>
<li> <p>See <a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md#create" class="MCXref xref">Create users in Workfront with the Adobe Admin Console</a></p> </li>
<li> <p>See the section "Add users" in the article <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li>
<li> <p>Contact your Adobe Admin Console Administrator.</p> </li>
</ul>
<p>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Business Platform, see <a href="../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md" class="MCXref xref">Platform-based administration differences (Adobe Workfront/Adobe Business Platform)</a>.</p>
</div>
<p><strong>Add a user to an organization that has not been onboarded to the Adobe Business Console</strong></p>

-->

若要將使用者新增至組織，您必須是要新增使用者的組織的管理員。 如需角色的相關資訊，請參閱 [中的組織角色 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/organizations/organization-roles.md).

若要將使用者新增至組織：

1. 瀏覽至 **[!UICONTROL 組織]** 在功能表中並選取您要新增使用者的組織。
1. 開啟 **[!UICONTROL 使用者]** 標籤。
1. 按一下 **[!UICONTROL 邀請新使用者]**，填寫表單（電子郵件、訊息、角色），然後按一下以傳送邀請 **[!UICONTROL 傳送]**.

>[!NOTE]
>
>   
><p>如果您看不到[！UICONTROL邀請新使用者]按鈕，表示您的組織已上線 [!DNL Adobe Business Platform.] </p>
>
>   <p>有關將使用者新增至已上線之組織的指示 [!DNL Adobe Business Platform]，請參閱 <a href="#add-a-user-to-an-organization-that-has-been-onboarded-to-the-adobe-business-platform" class="MCXref xref">將使用者新增至已上線的組織 [!DNL Adobe Business Platform]</a></p>

使用者會收到一封邀請電子郵件，讓他們可以接受邀請。
