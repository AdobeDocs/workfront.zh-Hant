---
title: 在Adobe Admin Console中管理使用者
description: 身為Adobe管理員，您可以使用Adobe Admin Console建立Adobe Workfront使用者和系統管理員。
author: Becky, Caroline
feature: System Setup and Administration
role: Admin
exl-id: ae657964-d4a5-4c3b-afc6-8dde7695955d
source-git-commit: 9bcd792139f8f2f0198da943e5c63a2add32e856
workflow-type: tm+mt
source-wordcount: '899'
ht-degree: 0%

---

# 在Adobe Admin Console中管理使用者

>[!IMPORTANT]
>
>只有在貴組織的Workfront例項已上線至Adobe業務平台時，才能使用本文中的功能。
>
>有關根據貴組織是否已上架到AdobeBusiness Platform而有所不同的過程清單，請參見 [平台管理差異(Adobe Workfront/Adobe業務平台)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

身為Adobe管理員，您可以使用Adobe Admin Console建立Adobe Workfront使用者和系統管理員。 主控台是管理整個組織Adobe權益的集中位置。 如需詳細資訊，請參閱 [Admin Console概述](https://helpx.adobe.com/tw/enterprise/using/admin-console.html).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe管理員權限</td> 
   <td> <p>您必須是貴組織Adobe產品的產品組態管理員</p> </td> 
  </tr> 
 </tbody> 
</table>

## 必要條件

使用Workfront適用的Admin Console之前，您應會收到電子郵件，邀請您前往主控台。

1. 如果您是初次Adobe，並收到電子郵件，告知您現在擁有管理貴組織Adobe軟體和服務的權限，請按一下電子郵件中的按鈕以建立Adobe帳戶並開啟Admin Console。

   或

   如果您已有Adobe帳戶，請前往 [Adobe Admin Console頁面](https://adminconsole.adobe.com/).

## 存取您Workfront生產執行個體的使用者和管理區域 {#access-the-user-and-admin-area-for-your-production-instance-of-workfront}

1. 從 [Adobe Admin Console頁面](https://adminconsole.adobe.com/)，請選取 **產品** ，然後選取 **Workfront** 產品方塊。

   ![](assets/admin-product-1.png)

1. 在顯示的清單中，選取頂端的連結。

   這是您的生產執行個體，供您的使用者使用。

   ![](assets/instances-1.png)

   >[!TIP]
   >
   >您的「預覽」實例是清單中的第二個連結，是一個測試環境，可複製您的即時生產環境。 如需詳細資訊，請參閱 [Adobe Workfront預覽沙箱環境](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).
   >
   >
   >清單中也可能會顯示沙箱環境的連結。 如需詳細資訊，請參閱 [Adobe Workfront預覽沙箱環境](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

1. 在顯示的清單中， **產品設定檔** 頁簽，按一下Workfront產品設定檔連結的名稱。

   ![](assets/prod-profile-1.png)

   此清單包含已指派給您Workfront生產執行個體的所有使用者。

   >[!IMPORTANT]
   >
   >請勿對產品設定檔本身進行任何變更。

1. 繼續閱讀本文的以下其中一節：

   * [在Workfront中使用Adobe Admin Console建立使用者](#create-users-in-workfront-with-the-adobe-admin-console)
   * [使用Adobe Admin Console在Workfront中建立系統管理員](#create-system-administrators-in-workfront-with-the-adobe-admin-console)

## 在Workfront中使用Adobe Admin Console建立使用者 {#create-users-in-workfront-with-the-adobe-admin-console}

1. 前往Admin Console中的使用者和管理區域，如 [存取您Workfront生產執行個體的使用者和管理區域](#access-the-user-and-admin-area-for-your-production-instance-of-workfront) 這篇文章。
1. 使用 **使用者** 頁簽，選擇 **添加用戶**.
1. 在 **新增使用者至此產品設定檔** 框中，輸入要添加的用戶的電子郵件地址或名稱，然後選擇 **儲存**.

   使用者是在Workfront中以要求者存取層級建立。

   >[!IMPORTANT]
   >
   >請勿對產品設定檔本身進行任何變更。

1. 在Workfront中，變更使用者的存取層級。

   如需Workfront管理員如何變更使用者存取層級的指示，請參閱 [編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. 重複步驟3和4以新增更多使用者。

   >[!NOTE]
   >
   >對於新的Adobe使用者，Admin Console會傳送電子郵件，邀請他們完成註冊程式。 所有用戶必須完成註冊過程才能訪問任何Adobe系統。
   >
   >若為現有的Adobe使用者，使用者可能會收到或不會收到有關Workfront可用的電子郵件。 這是由Adobe管理員控制的產品首選項。

## 使用Adobe Admin Console在Workfront中建立系統管理員 {#create-system-administrators-in-workfront-with-the-adobe-admin-console}

系統管理員存取層級僅在Adobe Admin Console上授予。 您無法在Workfront內授與或移除管理員存取權。

您必須先將使用者新增至Workfront的生產執行個體，才能讓該使用者成為Workfront系統管理員。 如需指示，請參閱 [在Workfront中使用Adobe Admin Console建立使用者](#create-users-in-workfront-with-the-adobe-admin-console) 這篇文章。

1. 前往Admin Console中的使用者和管理區域，如 [存取您Workfront生產執行個體的使用者和管理區域](#access-the-user-and-admin-area-for-your-production-instance-of-workfront) 這篇文章。
1. 選取 **管理員** 頁簽。
1. 選擇 **新增管理員**.
1. 在 **新增產品設定檔管理員** 框中，輸入要添加的管理員的電子郵件地址或名稱，然後選擇 **儲存**.

   ![](assets/add-admin-1.png)

   系統管理員是在Workfront中建立。

   >[!IMPORTANT]
   >
   >請勿對產品設定檔本身進行任何變更。

## 其他Adobe Admin Console詳細資訊：

* Workfront系統管理員可以從Workfront內停用Workfront使用者，但這不會在Admin Console中停用使用者。

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about deactivating a user in Workfront, see </p>
  -->

* 使用者 **家庭組** 是根據建立使用者來決定。 目前無法從Admin Console內自訂。
* Workfront系統管理員存取層級只能從Adobe Admin Console內編輯。

   <!--
  DRAFTED IN FLARE:
  How is this done?
  
  -->

* 必須先透過Admin Console，將身為系統管理員的使用者編輯至任何其他存取層級。

   <!--
   This is not clear
  -->

* 若要從Workfront中的使用者移除「系統管理員」存取權，您必須使用Adobe Admin Console來將使用者移除為產品設定檔管理員。 這會將使用者的Workfront存取層級從「系統管理員」變更為「請求者」。

   >[!IMPORTANT]
   >
   >請勿對產品設定檔本身進行任何變更。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>You can create Adobe Workfront users and system administrators with the <a href="https://adminconsole.adobe.com/" alt="Admin Console link">Adobe Admin Console</a>. The console is a central location for managing the Adobe entitlements across your organization. For more information, see the <a href="https://helpx.adobe.com/enterprise/using/admin-console.html" alt="Admin Console Overview">Admin Console Overview</a>.</p>
<p>Before using the Admin Console for Workfront, you should receive a receive an email inviting you to the console. Click in the invitation to accept it and create an account. You can also use an existing account, if already available.</p>
<h2>Create users</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Create users in WF with the Adobe admin console</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">May need to add something about oging throug WF -- check with Jonah</p>

<p>To create users in Workfront with the Admin Console:</p>
<ol>
<li value="1"> <p>From the <a href="https://adminconsole.adobe.com/">Admin Console page</a>, select the <b>Products</b> tab and then select the <b>Workfront</b> product tile.</p> </li>
<li value="2"> <p>Select the link to the Workfront instance you want to change.</p> </li>
<li value="3"> <p>Select the Product profile link. This shows a list of the currently-assigned users. If the list is very long, you can also search for users in the search field above the list.</p> </li>
<li value="4"> <p>Select the <b>Add User</b> button.</p> </li>
<li value="5"> <p>In the <b>Add users</b> box, enter the email address or name of the user you want to add. Select <b>Save</b>. The administrator is created in Workfront with <b>Requestor</b> access level.</p> </li>
</ol>
<h2>Create system administrators</h2>
<p>To create system administrators:</p>
<ol>
<li value="1"> <p>Make product profile assignments first. To be a Workfront System Administrator, the user must be assigned the Workfront product profile and be an admin for that product profile.</p> </li>
<li value="2"> <p>From the console, select the <b>Products</b> tab and then select the <b>Admins</b> tab. </p> </li>
<li value="3"> <p>Select <b>Add Admin</b>.</p> </li>
<li value="4"> <p>In the <b>Add product profile administrators</b> box, enter the email address or name of the administrator you want to add. Select <b>Save</b>. The user is created in Workfront with <b>Requestor</b> access level.</p> </li>
</ol>
<h2>Additional details for the Admin Console</h2>
<ul>
<li> <p>System Administrator access level is granted only on the Admin Console. You cannot grant or remove admin access from within Workfront.</p> </li>
</ul>
<ul>
<li> <p>Creating and deleting users inside Workfront is only possible through the Admin Console.</p> </li>
<li> <p>Workfront System Administrators can deactivate Workfront users from within Workfront, but this does not deactivate the user in the Admin Console.</p> </li>
<li> <p>All new users are are assigned <b>Requestor</b> access level upon creation. Also, the user <b>Home Group</b> is determined based on the user who created them. This is currently not customizable from within the Admin Console.</p> </li>
<li> <p>The Workfront System Administrator access level can only be edited from within the Adobe Admin Console.</p> </li>
<li> <p>Editing a user who is a system admin to any other access level must be done through the Admin Console first.</p> </li>
<li> <p>To remove Workfront system admin access, remove users as Product Profile Administrators. This action changes the user access level in Workfront from a system admin to a <b>Requestor</b>.</p> </li>
</ul>
</div>
-->
