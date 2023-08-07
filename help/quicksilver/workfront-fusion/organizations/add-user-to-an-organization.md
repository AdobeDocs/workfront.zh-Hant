---
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: 在Adobe Workfront Fusion中新增使用者至組織
description: 您可以在Adobe Workfront Fusion中新增使用者至組織。
author: Becky
feature: Workfront Fusion
exl-id: 98248cca-98f5-4eb5-b203-67e261df33f1
source-git-commit: 2884f709ef9ea89f275ff88db41ddde725dbd781
workflow-type: tm+mt
source-wordcount: '586'
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
    <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td> 
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

<p>將使用者新增至您的Fusion組織的程式會根據您的組織是否已上線至「Adobe企業平台」而有所不同。 </p>
<ul>
<li> <p><a href="#add-a-user-to-an-organization-that-has-been-onboarded-to-the-adobe-business-platform" class="MCXref xref">將使用者新增至已上線至Adobe業務平台的組織</a> </p> </li>
<li> <p><a href="#add-a-user-to-an-organization-that-has-not-been-onboarded-to-the-adobe-business-console" class="MCXref xref">將使用者新增至尚未上線至Adobe業務控制檯的組織</a> </p> </li>
</ul>
<div>
<p><strong>將使用者新增至已上線至Adobe業務平台的組織</strong></p>
<p>如果您的組織已加入Adobe Business Platform，您必須透過Adobe Admin Console執行此動作。</p>
<p>如需在Adobe Admin Console中新增使用者的指示：</p>
<ul>
<li> <p>另請參閱 <a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md#create" class="MCXref xref">使用Adobe Admin Console在Workfront中建立使用者</a></p> </li>
<li> <p>請參閱文章中的「新增使用者」一節 <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">個別管理使用者</a></p> </li>
<li> <p>請連絡您的Adobe Admin Console管理員。</p> </li>
</ul>
<p>如需根據貴組織是否已加入Adobe Business Platform而有所差異的程式清單，請參閱 <a href="../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md" class="MCXref xref">平台型管理差異(Adobe Workfront/Adobe Business Platform)</a>.</p>
</div>
<p><strong>將使用者新增至尚未上線至Adobe業務控制檯的組織</strong></p>

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
