---
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: 在Adobe Workfront Fusion中新增使用者至組織
description: Adobe Workfront Fusion檔案已移至新位置。 本文已棄用，但包含新文章的連結，內容涵蓋此功能。
author: Becky
feature: Workfront Fusion
exl-id: 98248cca-98f5-4eb5-b203-67e261df33f1
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '700'
ht-degree: 0%

---

# 在Adobe Workfront Fusion中新增使用者至組織或團隊

>[!IMPORTANT]
>
>本文將在近期移除，因為所有組織都已移至Adobe Admin Console。

>[!IMPORTANT]
>
>本頁所述的程式僅適用於尚未上線到[!DNL Adobe Admin Console]的組織。 如果您的組織已加入[!DNL Adobe Admin Console]，您必須透過[!DNL Adobe Admin Console]執行此動作。
>
>如需在貴組織移至[!DNL  Adobe Admin Console]和Adobe統一體驗後新增使用者的指示，請參閱[透過 [!DNL Adobe Admin Console]](/help/quicksilver/workfront-fusion/fusion-in-admin-console/add-fusion-users-admin-console.md)新增使用者至 [!DNL Adobe Workfront Fusion] 。
>
>如需根據貴組織是否已加入Adobe Admin Console而有所差異的程式清單，請參閱[以平台為基礎的管理差異(Adobe Workfront Fusion/Adobe Business Platform)](../../../quicksilver/workfront-fusion/fusion-in-admin-console/fusion-in-admin-console.md)。

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
>[!NOTE]
>
>如果您的組織目前正在移至Adobe Admin Console，您無法在Workfront中管理使用者（新增或刪除使用者）。 完成移轉後，您就可以在Adobe Admin Console中執行這些動作。

若要將使用者新增至組織，您必須是要新增使用者的組織的管理員。 如需角色的相關資訊，請參閱 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/organizations/organization-roles.md)中的[組織角色。

若要將使用者新增至組織：

1. 導覽至功能表中的&#x200B;**[!UICONTROL 組織]**，並選取您要新增使用者的組織。
1. 開啟儀表板中的&#x200B;**[!UICONTROL 使用者]**&#x200B;索引標籤。
1. 按一下&#x200B;**[!UICONTROL 邀請新使用者]**，並按一下&#x200B;**[!UICONTROL 傳送]**&#x200B;以傳送邀請。

   >[!NOTE]
   >
   >   
   >如果您看不到[!UICONTROL 邀請新使用者]按鈕，表示貴組織已加入[!DNL Adobe Business Platform.]
   >
   >  如需新增使用者至已加入[!DNL Adobe Business Platform]之組織的指示，請參閱[透過 [!DNL Adobe Admin Console]](/help/quicksilver/workfront-fusion/fusion-in-admin-console/add-fusion-users-admin-console.md)新增使用者至 [!DNL Adobe Workfront Fusion] 

1. 填寫表單。

   <table style="table-layout:auto">
<col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL電子郵件地址]</td>
      <td>
        輸入使用者的電子郵件地址
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL名稱]</td>
      <td>
        <p>輸入使用者的全名</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL角色] </td>
      <td>選取使用者的角色。 如需角色說明，請參閱<a href="/help/quicksilver/workfront-fusion/organizations/organization-roles.md">組織和團隊角色。</a></p>
   </td>
    </tr>
    <tr>
      <td role="rowheader">團隊</td>
      <td>選取您希望使用者成為其成員的所有團隊。</td>
    </tr>
    <tr>
      <td role="rowheader">備註</td>
      <td>輸入使用者的附註。 此附註會出現在使用者的邀請電子郵件中。</td>
    </tr>
  </tbody>
</table>

使用者會收到一封邀請電子郵件，讓他們可以接受邀請。

## 新增使用者至團隊

建立團隊時，會將您的使用者指派給團隊。 如果需要將現有使用者新增至團隊，您可以將他們新增至團隊的「使用者」頁面。

系統會從該團隊的頁面處理將使用者新增至團隊的程式。

1. 前往您要新增使用者的團隊，方法是選取左側面板中的&#x200B;**組織**，按一下組織頁面上的&#x200B;**團隊**&#x200B;索引標籤，然後選取團隊。

   或

   如果您在另一個團隊的頁面上，請按一下頁面頂端的團隊下拉式清單。

1. 在團隊的頁面（頁面頂端有團隊名稱）上，選取&#x200B;**使用者**&#x200B;索引標籤。
1. 在頁面上找出使用者。 您組織中的使用者即使不是團隊成員，也會出現在此頁面上。
1. 按一下使用者名稱右邊的&#x200B;**無**，然後選取您希望他們在團隊中的角色。

使用者會新增至團隊。