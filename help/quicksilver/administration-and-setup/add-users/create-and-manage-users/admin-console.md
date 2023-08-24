---
title: 在Adobe Admin Console中管理使用者
description: 作為Adobe管理員，您可以使用Adobe Admin Console建立Adobe Workfront使用者和系統管理員。
author: Becky, Caroline
feature: System Setup and Administration
role: Admin
exl-id: ae657964-d4a5-4c3b-afc6-8dde7695955d
source-git-commit: 01b60a2fab1188c8510857490ea87f609897b0bb
workflow-type: tm+mt
source-wordcount: '1137'
ht-degree: 0%

---

# 在Adobe Admin Console中管理使用者

>[!IMPORTANT]
>
>本文中的功能僅在您組織的Workfront執行個體已上線到Adobe業務平台時才能使用。
>
>如需根據貴組織是否已加入Adobe Business Platform而有所差異的程式清單，請參閱 [平台型管理差異(Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

作為Adobe管理員，您可以使用Adobe Admin Console建立Adobe Workfront使用者和系統管理員。 主控台是管理整個組織中Adobe許可權的中央位置。 如需詳細資訊，請參閱 [Admin Console概觀](https://helpx.adobe.com/tw/enterprise/using/admin-console.html).

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

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
   <td role="rowheader">Adobe管理員許可權</td> 
   <td> <p>您必須是組織Adobe產品的產品設定管理員</p> </td> 
  </tr> 
 </tbody> 
</table>

## 必要條件

在針對Workfront使用Admin Console之前，您應該會收到一封邀請您加入主控台的電子郵件。

1. 如果您是Adobe的新手，並且已收到一封電子郵件，告知您現在擁有管理貴組織的Adobe軟體與服務的許可權，請按一下電子郵件中的按鈕，以建立Adobe帳戶並開啟Admin Console。

   或

   如果您已有Adobe帳戶，請前往 [Adobe Admin Console頁面](https://adminconsole.adobe.com/).

## 存取您的Workfront生產執行個體的使用者和管理區域 {#access-the-user-and-admin-area-for-your-production-instance-of-workfront}

1. 從 [Adobe Admin Console頁面](https://adminconsole.adobe.com/)，選取 **產品** 索引標籤，然後選取 **Workfront** 產品拼貼。

   ![](assets/admin-product-1.png)

1. 在顯示的清單中，選取頂端的連結。

   這是您的使用者所在的生產執行個體。

   ![](assets/instances-1.png)

   >[!TIP]
   >
   >您的預覽執行個體（清單中的第二個連結）是複製您的即時生產環境的測試環境。 如需詳細資訊，請參閱 [Adobe Workfront預覽沙箱環境](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).
   >
   >
   >您也可能在清單中看到沙箱環境的連結。 如需詳細資訊，請參閱 [Adobe Workfront預覽沙箱環境](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

1. 在顯示的清單中，使用 **產品設定檔** 索引標籤已選取，按一下Workfront產品設定檔連結的名稱。

   ![](assets/prod-profile-1.png)

   此清單包含已指派給您的Workfront生產執行個體的所有使用者。

   >[!IMPORTANT]
   >
   >請勿對產品設定檔本身進行任何變更。

1. 請繼續閱讀本文中下列其中一節：

   * [使用Adobe Admin Console在Workfront中建立使用者](#create-users-in-workfront-with-the-adobe-admin-console)
   * [使用Adobe Admin Console在Workfront中建立系統管理員](#create-system-administrators-in-workfront-with-the-adobe-admin-console)

## 使用Adobe Admin Console在Workfront中建立使用者 {#create-users-in-workfront-with-the-adobe-admin-console}

必須將Workfront使用者新增至Adobe Admin Console。 管理員可以直接在Adobe Admin Console中建立使用者。 群組管理員會在Workfront中建立使用者，然後提交使用者以供核准。 核准後，使用者會新增至Adobe Admin Console。

* [直接在Adobe Admin Console的Workfront中建立使用者](#create-users-in-workfront-directly-in-the-adobe-admin-console)
* [在Workfront中建立使用者並核准他們用於Adobe Admin Console](#create-users-in-workfront-and-approve-them-for-the-adobe-admin-console)

### 直接在Adobe Admin Console的Workfront中建立使用者

1. 如所述，前往Admin Console中的使用者和管理員區域 [存取您的Workfront生產執行個體的使用者和管理區域](#access-the-user-and-admin-area-for-your-production-instance-of-workfront) 本文章內容。
1. 使用 **使用者** 標籤在清單上方選取，選取 **新增使用者**.
1. 在 **將使用者新增至此產品設定檔** 方塊，輸入您要新增的使用者的電子郵件地址或名稱，然後選取 **儲存**.

   在Workfront中建立使用者，且具有請求者存取層級。

   >[!IMPORTANT]
   >
   >請勿對產品設定檔本身進行任何變更。

1. 在Workfront中，變更使用者的存取層級。

   如需有關Workfront管理員如何變更使用者存取層級的指示，請參閱 [編輯使用者設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. 重複步驟3和4以新增更多使用者。

   >[!NOTE]
   >
   >對於新的Adobe使用者，Admin Console會傳送電子郵件邀請他們完成註冊程式。 所有使用者必須完成註冊程式才能存取任何Adobe系統。
   >
   >對於現有的Adobe使用者，使用者可能會收到也可能不會收到有關Workfront可用性的電子郵件。 這是產品的Adobe管理員所控制的偏好設定。

### 在Workfront中建立使用者並核准他們用於Adobe Admin Console

此工作流程可讓沒有Adobe Admin Console存取許可權的群組管理員建立使用者。

首先，群組管理員會在Workfront中建立使用者。 這會建立處於已停用和待核准狀態的使用者。

接著，Workfront管理員會核准使用者。 這會在Workfront中啟用使用者，並將他們新增至Adobe Admin Console。

#### 在Workfront中建立使用者（群組管理員）

如需在Workfront中建立使用者的指示，請參閱 [新增使用者](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/add-users.md).

#### 核准使用者(Workfront管理員)

若要核准使用者，請執行下列動作：

1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) (位於Adobe Workfront的右上角)，然後按一下 **使用者** ![](assets/users-icon-in-main-menu.png).

1. 選取使用者，然後按一下更多圖示 ![](assets/more-icon.png).

1. 若要核准使用者，請按一下 **核准**，然後按一下 **提交**.

   或

   若要拒絕使用者並從Workfront刪除他們，請按一下 **拒絕**，然後按一下 **提交**.

已核准的使用者會自動新增至Adobe Admin Console。

遭拒絕的使用者會自動從Workfront中刪除。



## 使用Adobe Admin Console在Workfront中建立系統管理員 {#create-system-administrators-in-workfront-with-the-adobe-admin-console}

系統管理員存取層級僅在Adobe Admin Console上授予。 您無法從Workfront中授與或移除管理員存取權。

您必須先將使用者新增到Workfront的生產執行個體，然後才能將使用者設為Workfront系統管理員。 如需指示，請參閱 [使用Adobe Admin Console在Workfront中建立使用者](#create-users-in-workfront-with-the-adobe-admin-console) 本文章內容。

1. 如所述，前往Admin Console中的使用者和管理員區域 [存取您的Workfront生產執行個體的使用者和管理區域](#access-the-user-and-admin-area-for-your-production-instance-of-workfront) 本文章內容。
1. 選取 **管理員** 索引標籤的使用者清單上方。
1. 選取 **新增管理員**.
1. 在 **新增產品設定檔管理員** 方塊中，輸入您要新增的管理員電子郵件地址或名稱，然後選取 **儲存**.

   ![](assets/add-admin-1.png)

   系統管理員是在Workfront中建立。

   >[!IMPORTANT]
   >
   >請勿對產品設定檔本身進行任何變更。

## 有關Adobe Admin Console的其他詳細資料：

* Workfront系統管理員可以從Workfront中停用Workfront使用者，但這不會停用Admin Console中的使用者。

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about deactivating a user in Workfront, see </p>
  -->

* 使用者 **主群組** 是根據建立它們的使用者來決定。 目前無法從Admin Console內自訂此專案。
* Workfront系統管理員存取層級只能從Adobe Admin Console內編輯。

  <!--
  DRAFTED IN FLARE:
  How is this done?
  
  -->

* 編輯系統管理員為任何其他存取層級的使用者必須先透過Admin Console完成。

  <!--
   This is not clear
  -->

* 若要從Workfront中的使用者移除系統管理員存取權，您需要使用Adobe Admin Console移除作為產品設定檔管理員的使用者。 這會將使用者的Workfront存取層級從系統管理員變更為請求者。

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
