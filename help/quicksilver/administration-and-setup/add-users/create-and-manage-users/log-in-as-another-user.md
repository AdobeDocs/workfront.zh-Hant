---
title: 以其他使用者身分登入
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 身為Adobe Workfront管理員，您有時可能需要代表其他使用者存取Workfront 。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2f8dd132-1086-4980-9b56-993a68231e96
source-git-commit: 6068c9c53568d3ebec9fae294bfee1cbd365714b
workflow-type: tm+mt
source-wordcount: '738'
ht-degree: 0%

---

# 以另一位使用者身分登入

<!--Audited: 5/2025-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all users only in the Preview environment.</span> -->

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. Also linked to other articles: Creating and Managing Groups, etc.</p>
-->

身為Adobe Workfront管理員，您有時可能需要代表其他使用者存取Workfront 。 或者，作為群組管理員，您可能需要代表您管理群組之成員的使用者存取Workfront。

例如，如果任務在休假的使用者執行特定動作之前無法進度，您可以以該使用者的身分登入，並改為執行動作。

<!--
<note type="note">
Some users, such as executives, need to be able to control which administrators can log in to their accounts, and for how long. Working with your organization, Workfront configures settings that allow this control for these users. When a Workfront administrator or group administrator (associated with one of the user's groups) tries to log in as one of these users, an on-screen message prompts the administrator to contact the user for access. From the user profile area, the user can then grant access to the administrator and specify an expiration time for it. For more information on how the user does this, see
<a href="../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md#access" class="MCXref xref">Access</a> in
<a href="../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Configure My Settings</a>.
<span class="PinkDraftNote">[Add a note about this being only for the Enterprise package if they decide to do it that way]</span>
</note>
-->

>[!NOTE]
>
>由於檔案整合可能會連線到私人個人檔案，因此管理員在作為其他使用者登入時無法存取檔案整合。
>
>如需檔案整合的詳細資訊，請參閱[設定檔案整合](../../../administration-and-setup/configure-integrations/configure-document-integrations.md)。

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
   <td> <p>新增：標準</p>
   <p>或</p>
   <p>目前：計畫</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>使用「系統管理員」存取層級，您可以以任何身分登入。</p> <p>使用標準或規劃師存取層級，如果存取層級中的使用者設定設為編輯存取權，並且在「微調您的設定<img src="assets/gear-icon-in-access-levels.png">」下啟用建立及至少兩個使用者管理員選項中的一個，則您可以以較低授權層級的使用者身分登入。 </p> 
   <p>注意：在這兩個選項中，如果已啟用「使用者管理員（群組使用者）」，您必須是使用者所屬群組的群組管理員。</p></td>
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 以其他使用者身分登入並執行動作

1. 以Workfront管理員或群組管理員身分登入Workfront。

   >[!NOTE]
   >
   >* 如果您是群組管理員，則只能以您管理之群組中的使用者身分登入。 此外，您必須在存取層級中啟用「使用者管理員（群組使用者）」許可權：
   >   
   >  ![群組管理員使用者](assets/group-admin-user.png)
   >   
   >  此設定預設為停用。 如需詳細資訊，請參閱[建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。
   >   
   >* 您無法重設Workfront管理員的密碼。

{{step-1-to-setup}}

1. 在左側面板中，按一下&#x200B;**登入身份**。

1. 在&#x200B;**登入身份**&#x200B;索引標籤的&#x200B;**開始輸入名稱……**&#x200B;方塊中，開始輸入使用者的名稱，然後在其出現在下拉式清單中時按一下該名稱。


   >[!NOTE]
   >* 您選取的使用者必須在Workfront中定義存取層級。 您無法以沒有登入許可權的使用者身分登入Workfront系統。
   >* 群組管理員只能以他們管理之群組成員的使用者身分登入。 他們無法以Workfront管理員身分登入。

1. 按一下&#x200B;**登入**。 您以其他使用者身份登入，畫面上方會顯示通知，說明此問題。

   <!--
   <p> Might come in a future story:</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">click an Access period and then click Request to ask the user for access to log as him or her for the specified period of time. Continue these steps after the user grants access. Specify somewhere here that this is only for the Enterprise package if they decide on that</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Or </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">If a prompt appears indicating that the user has restricted access to their account, contact the user to request access.</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The user can then can grant you "Log in as" access in their user profile. They can also specify an expiration date and time for the access period. </p>
   -->

   <!--
   This triggers an email to let you know that you have access to log in as the user, depending on how your event notifications are enabled. For more information, see <a href="../../../workfront-basics/using-notifications/event-notifications.md" class="MCXref xref">Event notifications</a>.
   </div>
   -->



1. 以使用者身分執行必要的動作後，請按一下畫面頂端的&#x200B;**[登出**]。

## 在管理員以其他使用者身份登入時追蹤和稽核活動

Workfront提供機制，可在管理員以其他使用者身份登入時追蹤和稽核活動。

當您以其他使用者身份登入時，該使用者的上次登入日期將修改為該使用者系統或群組管理員登入的日期。

* [檢視專案上的指標](#view-indicators-on-items)
* [檢視稽核資訊](#view-audit-information)

### 檢視專案上的指標 {#view-indicators-on-items}

當您以其他使用者身分登入Workfront並執行動作時，Workfront會清楚指出您執行的任何動作都是由您代表您登入的使用者所執行。

例如，如果您以其他使用者身份登入時註解某個專案，則說明您在檢視物件的「更新」區段時，代表使用者發表了註解。

### 檢視稽核資訊 {#view-audit-information}

1. 以Workfront管理員或群組管理員身分登入Workfront。
   {{step-1-to-setup}}
   <!--1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![Gear settings icon](assets/gear-icon-settings.png).-->

1. 在左側面板中，按一下&#x200B;**登入身份**，然後按一下&#x200B;**存取記錄檔**&#x200B;索引標籤。

   >[!NOTE]
   >
   >每當系統或群組管理員以其他使用者身份登入Workfront時，該事件就會記錄到稽核軌跡。 此外，當管理員以其他使用者身份登入時，所發生的任何可稽核動作都會登入稽核軌跡。

1. （選擇性）您可以透過下列方式篩選稽核軌跡中顯示的結果：

   * 依已登入的使用者
   * 依登入身份的使用者
   * 依日期和時間
