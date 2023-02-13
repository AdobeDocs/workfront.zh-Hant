---
title: 以其他使用者身分登入
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 身為Adobe Workfront管理員，您有時可能需要代表其他使用者存取Workfront。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2f8dd132-1086-4980-9b56-993a68231e96
source-git-commit: 7fa4791e19a84d7215e341e8bbde8dd4d4d8ccc6
workflow-type: tm+mt
source-wordcount: '809'
ht-degree: 0%

---

# 以其他使用者身分登入

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. Also linked to other articles: Creating and Managing Groups, etc.</p>
-->

>[!IMPORTANT]
>
>本頁所述的程式僅適用於尚未上線至Adobe Admin Console的組織。 如果貴組織已上線至Adobe Admin Console，則此動作無法使用。
>
>如需依貴組織是否已上線至Adobe Admin Console而有所不同的程式清單，請參閱 [平台管理差異(Adobe Workfront/Adobe業務平台)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

身為Adobe Workfront管理員，您有時可能需要代表其他使用者存取Workfront。

或者，身為群組管理員，您可能需要代表您所管理之群組的成員使用者存取Workfront。

例如，如果在休假的用戶執行某個操作之前，任務無法進行，則可以以該用戶身份登錄，然後改為執行操作。

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
>由於檔案整合可能會連線至私人個人檔案，因此管理員在以其他使用者身分登入時無法存取檔案整合。
>
>如需檔案整合的詳細資訊，請參閱 [配置文檔整合](../../../administration-and-setup/configure-integrations/configure-document-integrations.md)

## 存取需求

您必須具備下列條件才能執行本文所述步驟：

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
   <td> <p>使用「系統管理員」訪問級別，您可以以任何人身份登錄。 有關此訪問級別的資訊，請參見 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>. </p> <p>使用計畫員訪問級別，您可以以具有較低許可級別的用戶身份登錄(如果 <b>使用者</b> 在存取層級中的設定，設定為 <b>編輯</b> 存取，使用 <b>建立</b> 和兩者中的至少一個 <b>使用者管理</b> 選項 <b>微調您的設定</b> <img src="assets/gear-icon-in-access-levels.png">. </p> 
   <p><b>注意</b>:在這兩個選項中，如果用戶 <b>管理員（群組使用者）</b> 啟用時，您必須是使用者所屬群組的群組管理員。</p> 
   <p>如需 <b>使用者</b> 在存取層級中設定，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取權</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 以其他使用者身分登入並執行動作

1. 以Workfront管理員或群組管理員身分登入Workfront。

   >[!NOTE]
   >
   >* 如果您是群組管理員，則只能以您管理之群組中使用者身分登入。 此外，您必須在存取層級中啟用使用者管理員（群組使用者）權限：
   >   
   >  ![](assets/group-admin-user.png)
   >   
   >  預設會停用此設定。 如需詳細資訊，請參閱 [建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
   >   
   >* 您無法重設Workfront管理員的密碼。


1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **登入方式**.

1. 在 **使用者** 框 **登入方式** 頁簽，開始鍵入用戶的名稱，然後在下拉清單中顯示該名稱時按一下該名稱。

   使用者必須具有Workfront中定義的存取層級。 您無法以沒有登入權限的使用者身分登入Workfront系統。

   >[!NOTE]
   >
   >群組管理員只能以其所管理群組成員的使用者身分登入。 他們無法以Workfront管理員身分登入。

1. 按一下 **登入。**

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Might come in a future story:</p>
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

   當您以其他使用者身分登入時，畫面頂端會顯示通知以指出這點。

1. 以使用者身分執行必要動作後，按一下 **登出。**

## 在管理員以其他使用者身分登入時追蹤和稽核活動

Workfront提供追蹤和稽核活動的機制，當管理員以其他使用者身分登入時，就會發生此活動。

當您以其他用戶身份登錄時，系統或組管理員將修改該用戶的上次登錄日期，直至該用戶身份登錄的日期。

* [查看項的指標](#view-indicators-on-items)
* [查看審核資訊](#view-audit-information)

### 查看項的指標 {#view-indicators-on-items}

當您以其他使用者身分登入Workfront並執行動作時，Workfront會清楚指出您執行的任何動作都是由您代表以登入身分登入的使用者所執行。

例如，如果您在以其他使用者身分登入時對項目發表評論，陳述式會指出您是代表該使用者發表評論的。

### 查看審核資訊 {#view-audit-information}

1. 以Workfront管理員或群組管理員身分登入Workfront。
1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **登入方式，** 然後按一下 **訪問日誌** 標籤。

   每當系統或群組管理員以其他使用者身分登入Workfront時，事件即會記錄在稽核軌跡中。 此外，管理員以其他使用者身分登入時發生的任何可稽核動作都會記錄在稽核軌跡中。

1. （選用）您可以透過下列方式篩選稽核軌跡中顯示的結果：

   * 已登入的使用者
   * 已登入為的使用者
   * 依日期
