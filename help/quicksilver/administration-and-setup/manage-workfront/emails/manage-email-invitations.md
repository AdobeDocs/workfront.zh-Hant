---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: 管理新使用者的電子郵件邀請
description: 身為Adobe Workfront管理員，您可以使用電子郵件邀請將使用者新增至Workfront，並通知他們已新增。
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: e13e3479-391f-4aec-b998-e9b6057f256b
source-git-commit: 9bcd792139f8f2f0198da943e5c63a2add32e856
workflow-type: tm+mt
source-wordcount: '947'
ht-degree: 0%

---

# 管理新使用者的電子郵件邀請

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

>[!IMPORTANT]
>
>本頁面上描述的程式僅適用於尚未上線至Admin Console的組織。 如果貴組織已上線至Adobe Admin Console，您必須透過Adobe Admin Console執行此動作。
>
>如需依貴組織是否已上線至Adobe Admin Console而有所不同的程式清單，請參閱 [平台管理差異(Adobe Workfront/Adobe業務平台)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

身為Adobe Workfront管理員，您可以使用電子郵件邀請將使用者新增至Workfront，並通知他們已新增。

電子郵件邀請可讓新使用者遵循連結，從中為其Workfront帳戶選擇密碼。 然後，他們就可以完成帳戶的設定。

為確保新帳戶的安全性，我們建議您為新使用者使用電子郵件邀請，讓他們可以選擇自己的密碼。 或者，您也可以在建立新使用者的帳戶時為其選取密碼。 如需新增使用者至Workfront的詳細資訊，請參閱 [新增使用者](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

您可以為下列項目設定新使用者電子郵件：

* 任何新使用者新增至Workfront
* 具有要求者授權新增至Workfront的使用者

所有新使用者在傳送電子郵件邀請時，都會看到相同的電子郵件。

如需接收電子郵件邀請的相關資訊，請參閱 [接收電子郵件邀請並建立Adobe Workfront的密碼](../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/receive-email-invitations.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置</td> 
   <td> <p>系統管理員</p> </td> 
  </tr> 
 </tbody> 
</table>

## 生成電子郵件邀請 {#generate-email-invitations}

在下列情況下會產生電子郵件邀請：

* 建立新使用者並選取 **傳送邀請電子郵件給此人** 在 **新用戶** 表單。 如需建立新使用者的詳細資訊，請參閱 [新增使用者](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).
* 當您匯入多個新使用者，並選取 **傳送邀請電子郵件給這些人** 選項。 如需匯入多個新使用者的詳細資訊，請參閱 [匯入使用者](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).
* 建立使用者後，您可以手動產生邀請給尚未在Workfront註冊帳戶，且尚未建立Workfront密碼的使用者。\
   已建立帳戶但尚未註冊其帳戶的使用者會標示為 **未註冊** 在Workfront。

   >[!NOTE]
   >
   >如果您取消選取 **傳送電子郵件邀請給此人** 框中，無法手動生成電子郵件邀請。 只有在建立原始電子郵件邀請時已傳送該邀請的使用者，才能手動重新傳送電子郵件邀請。 如需建立新使用者的詳細資訊，請參閱 [新增使用者](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

要手動為現有未註冊用戶生成電子郵件邀請，請執行以下操作：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **使用者** ![](assets/users-icon-in-main-menu.png).
1. 選取要顯示 **未註冊** 在名稱后加上標籤。

   ![](assets/unreg-user-qs-350x221.png)

1. 按一下「更多」圖示 ![](assets/more-icon.png)，然後按一下 **提醒用戶註冊**.

   系統會傳送電子郵件邀請給新使用者，並附上新的連結，讓新使用者可以用來建立其Workfront密碼。

   >[!NOTE]
   >
   >如果您的組織已上線至Admin Console，而您透過Workfront新增使用者，則您沒有選項可向新使用者傳送電子郵件邀請。
   >
   >新的Adobe使用者會新增至Admin Console,Admin Console會傳送電子郵件邀請他們完成註冊程式。 所有用戶必須完成註冊過程才能訪問任何Adobe系統。
   >
   >若為現有的Adobe使用者，使用者可能會收到或不會收到有關Workfront可用的電子郵件。 這是由Adobe管理員控制的產品首選項。

## 配置電子郵件邀請 {#configure-email-invitations}

身為Workfront管理員，您可以設定新使用者電子郵件邀請中包含的訊息。

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側的清單中，按一下 **電子郵件** > **邀請**.

1. 在 **一般選項** 區段進行下列任何修改：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>在……天后停用邀請連結</strong> </td> 
      <td> <p>選擇電子郵件邀請不再包含有效Workfront連結的時間長度。 預設天數為45天。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>包含訊息和/或服務期限</strong> </td> 
      <td> <p>如果您要修改所有新增至Workfront的使用者之電子郵件邀請，請選取此選項。 這不包括具有請求者授權的使用者。</p> 
       <ul> 
        <li><strong>訊息</strong>:如果您選取修改所有新使用者的電子郵件邀請，請指定您要納入電子郵件邀請中的文字作為電子郵件內文。</li> 
        <li><strong>條款與條件</strong>:如果您選取修改所有新使用者的電子郵件邀請，請指定您要納入電子郵件邀請中的文字作為條款和條件。<br></li> 
        <li><strong>包括幫助台用戶的消息和/或服務期限</strong>:如果您想要修改新增至Workfront且擁有申請人授權的所有新使用者的電子郵件邀請，請選取此選項。</li> 
        <li><strong>訊息</strong>:如果您選擇修改所有具有申請人授權的新使用者的電子郵件邀請，請指定您要以電子郵件內文形式納入電子郵件邀請中的文字。</li> 
        <li><strong>條款與條件</strong>:如果您選擇修改所有具有申請人授權的新使用者的電子郵件邀請，請指定您要納入電子郵件邀請中的文字作為條款和條件。<br></li> 
        <li> <p>在 <strong>邀請預覽</strong> 區段中，您會看到電子郵件邀請的預覽。 如果您選取在電子郵件邀請中包含自訂訊息，則此區域會顯示自訂訊息。</p> <p> <img src="assets/email-invitation-for-all-users-preview-qs-350x190.png" style="width: 350;height: 190;"> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下&#x200B;**儲存**。
