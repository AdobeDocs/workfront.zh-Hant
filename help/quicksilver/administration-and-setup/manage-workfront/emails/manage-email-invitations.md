---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: 管理新使用者的電子郵件邀請
description: 身為Adobe Workfront管理員，您可以使用電子郵件邀請將使用者新增至Workfront，並通知他們已新增。
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: e13e3479-391f-4aec-b998-e9b6057f256b
source-git-commit: 85aa6cc865bfc28498cca17e1942c146eeb8e4fc
workflow-type: tm+mt
source-wordcount: '932'
ht-degree: 0%

---

# 管理新使用者的電子郵件邀請

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

>[!IMPORTANT]
>
>此頁面中說明的程式僅適用於尚未加入Admin Console的組織。 如果您的組織已加入Adobe Admin Console，您必須透過Adobe Admin Console執行此動作。
>
>如需根據貴組織是否已加入Adobe Admin Console而有所差異的程式清單，請參閱[以平台為基礎的管理差異(Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)。

身為Adobe Workfront管理員，您可以使用電子郵件邀請將使用者新增至Workfront，並通知他們已新增。

電子郵件邀請可讓新使用者追蹤連結，以便選擇Workfront帳戶的密碼。 接著，他們就可以完成帳戶的設定。

為確保新帳戶的安全性，我們建議您為新使用者使用電子郵件邀請，以便他們可以選擇自己的密碼。 或者，您也可以在建立新使用者的帳戶時，為其選取密碼。 如需新增使用者至Workfront的詳細資訊，請參閱[新增使用者](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md)。

您可以為新使用者設定電子郵件：

* 任何新增到Workfront的使用者
* 使用請求者授權新增至Workfront的使用者

傳送電子郵件邀請時，所有新使用者都會看到相同的電子郵件。

如需接收電子郵件邀請的詳細資訊，請參閱[接收電子郵件邀請並建立Adobe Workfront的密碼](../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/receive-email-invitations.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

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
   <td>規劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>系統管理員</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## 產生電子郵件邀請 {#generate-email-invitations}

在下列情況下會產生電子郵件邀請：

* 當您建立新使用者，並在&#x200B;**新增使用者**&#x200B;表單上選取&#x200B;**傳送邀請電子郵件給此人**&#x200B;時。 如需有關建立新使用者的詳細資訊，請參閱[新增使用者](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md)。
* 當您匯入多個新使用者，並選取&#x200B;**傳送邀請電子郵件給這些人員**&#x200B;選項時。 如需有關匯入多個新使用者的詳細資訊，請參閱[匯入使用者](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md)。
* 建立使用者後，您可以手動向尚未在Workfront註冊帳戶且尚未建立Workfront密碼的使用者產生邀請。\
  已建立帳戶但尚未註冊帳戶的使用者，在Workfront中會標示為&#x200B;**已取消註冊**。

  >[!NOTE]
  >
  >如果您在建立使用者時取消選取&#x200B;**傳送電子郵件邀請給此人**&#x200B;方塊，則無法手動產生電子郵件邀請。 只有已在其帳戶建立時傳送原始電子郵件邀請的使用者，才能手動重新傳送電子郵件邀請。 如需有關建立新使用者的詳細資訊，請參閱[新增使用者](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md)。

若要手動產生電子郵件邀請給現有的未註冊使用者：

{{step-1-to-users}}

1. 選取在其名稱后面顯示&#x200B;**已取消註冊**&#x200B;標籤的使用者。

   ![已取消註冊](assets/unreg-user-qs-350x221.png)

1. 按一下「更多」圖示![「更多」圖示](assets/more-icon.png)，然後按一下&#x200B;**「提醒使用者註冊」**。

   系統會傳送電子郵件邀請給新使用者，其中包含可用來建立其Workfront密碼的新連結。

   >[!NOTE]
   >
   >如果您的組織已加入Admin Console，而您透過Workfront新增使用者，則無法選擇傳送電子郵件邀請給新使用者。
   >
   >新的Adobe使用者會新增至Admin Console，而Admin Console會傳送電子郵件邀請他們完成註冊程式。 所有使用者必須完成註冊程式才能存取任何Adobe系統。
   >
   >對於現有的Adobe使用者，使用者可能會收到也可能不會收到有關Workfront可用性的電子郵件。 這是產品的Adobe管理員所控制的偏好設定。

## 設定電子郵件邀請 {#configure-email-invitations}

身為Workfront管理員，您可以設定新使用者的電子郵件邀請所包含的訊息。

{{step-1-to-setup}}

1. 在左邊的清單中，按一下&#x200B;**電子郵件** > **邀請**。

1. 在&#x200B;**一般選項**&#x200B;區段中，進行下列任何修改：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>在……天后停用邀請連結</strong> </td> 
      <td> <p>選擇電子郵件邀請不再包含Workfront有效連結的時間長度。 預設天數是45。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>包含訊息和/或服務條款</strong> </td> 
      <td> <p>如果您想要修改所有新增至Workfront之新使用者的電子郵件邀請，請選取此選項。 這不包括擁有請求者授權的使用者。</p> 
       <ul> 
        <li><strong>訊息</strong>：如果您選擇修改所有新使用者的電子郵件邀請，請指定您要在電子郵件邀請中包含的文字做為電子郵件內文。</li> 
        <li><strong>條款與條件</strong>：如果您選擇修改所有新使用者的電子郵件邀請，請指定要包含在電子郵件邀請中的文字做為條款與條件。<br></li> 
        <li><strong>包括訊息和/或服務條件給服務檯使用者</strong>：如果您要修改新增到Workfront且擁有要求者授權的所有新使用者的電子郵件邀請，請選取此選項。</li> 
        <li><strong>訊息</strong>：如果您選擇修改所有具有要求者授權的新使用者的電子郵件邀請，請指定您要在電子郵件邀請中包含的文字做為電子郵件內文。</li> 
        <li><strong>條款與條件</strong>：如果您選擇修改所有具有要求者授權的新使用者的電子郵件邀請，請指定您要加入電子郵件邀請的文字做為條款與條件。<br></li> 
        <li> <p>在<strong>邀請預覽</strong>區段中，您可以看到電子郵件邀請的預覽。 如果您選取在電子郵件邀請中包含自訂訊息，則自訂訊息會顯示在此區域中。</p> <p> <img src="assets/email-invitation-for-all-users-preview-qs-350x190.png" style="width: 350;height: 190;"> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下「**儲存**」。
