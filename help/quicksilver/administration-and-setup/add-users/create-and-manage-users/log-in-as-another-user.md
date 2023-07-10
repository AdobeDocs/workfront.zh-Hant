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
source-git-commit: 82f42d81970c7572f43519423ec3a8c0889aaff4
workflow-type: tm+mt
source-wordcount: '895'
ht-degree: 0%

---

# 以其他使用者身分登入


<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅適用於預覽環境中的所有使用者。</span>
<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. Also linked to other articles: Creating and Managing Groups, etc.</p>
-->

>[!IMPORTANT]
>
>本頁所述的程式僅適用於尚未上線至Adobe Admin Console的組織。 如果您的組織已上線至Adobe Admin Console，則無法使用此動作。
>
>如需根據貴組織是否已上線至Adobe Admin Console而有所不同的程式清單，請參閱 [平台式管理差異(Adobe Workfront/Adobe商務平台)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

身為Adobe Workfront管理員，您有時可能需要代表其他使用者存取Workfront。

或者，身為群組管理員，您可能需要代表您管理之群組成員的使用者存取Workfront。

例如，如果任務在休假的使用者執行特定動作之前無法進度，您可以以該使用者身分登入，並改為執行動作。

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
>由於檔案整合可能會連線到私人個人檔案，因此管理員在以其他使用者身份登入時無法存取檔案整合。
>
>如需檔案整合的詳細資訊，請參閱 [設定檔案整合](../../../administration-and-setup/configure-integrations/configure-document-integrations.md)

## 存取需求

您必須具備下列專案才能執行本文所述的步驟：

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
   <td role="rowheader">存取層級設定</td> 
   <td> <p>使用「系統管理員」存取層級，您可以以任何身分登入。 如需有關此存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完全管理存取權</a>. </p> <p>使用「規劃師」存取層級，您可以在下列情況下以授權層級較低的使用者身分登入： <b>使用者</b> 存取層級中的設定已設定為 <b>編輯</b> 存取，使用 <b>建立</b> 和至少兩者之一 <b>使用者管理員</b> 選項啟用於 <b>微調您的設定</b> <img src="assets/gear-icon-in-access-levels.png">. </p> 
   <p><b>注意</b>：這兩個選項中，如果使用者為 <b>管理員（群組使用者）</b> 已啟用，您必須是使用者所屬群組的群組管理員。</p> 
   <p>如需更多有關「 」的資訊， <b>使用者</b> 在存取層級中設定，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取許可權</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 以其他使用者身分登入並執行動作

1. 以Workfront管理員或群組管理員身分登入Workfront。

   >[!NOTE]
   >
   >* 如果您是群組管理員，則只能以您管理之群組中的使用者身分登入。 此外，您必須在存取層級中啟用「使用者管理員（群組使用者）」許可權：
   >   
   >  ![](assets/group-admin-user.png)
   >   
   >  此設定預設為停用。 如需詳細資訊，請參閱 [建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
   >   
   >* 您無法重設Workfront管理員的密碼。

1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) Adobe Workfront右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **登入身份**.

1. 在 **使用者** 方塊(位於 **登入身份** 索引標籤中，開始輸入使用者的名稱，然後在其出現在下拉式清單中時按一下該名稱。

   使用者必須擁有Workfront中定義的存取層級。 您無法以沒有登入許可權的使用者身分登入Workfront系統。

   >[!NOTE]
   >
   >群組管理員只能以他們管理之群組成員的使用者身分登入。 他們無法以Workfront管理員身分登入。

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

   當您以其他使用者身份登入時，畫面頂部會顯示通知以指示此情況。

1. 以使用者身分執行必要的動作後，請按一下 **登出。**

## 在管理員以其他使用者身份登入時追蹤和稽核活動

Workfront提供機制，可在管理員以其他使用者身份登入時追蹤和稽核活動。

當您以其他使用者身份登入時，該使用者的上次登入日期會修改為系統或群組管理員以該使用者身份登入的日期。

* [檢視專案上的指標](#view-indicators-on-items)
* [檢視稽核資訊](#view-audit-information)

### 檢視專案上的指標 {#view-indicators-on-items}

當您以其他使用者身分登入Workfront並執行動作時，Workfront會明確指出您執行的任何動作都是由您代表您以身分登入的使用者所執行。

例如，如果您以其他使用者身份登入時註解某個專案，則會出現一條宣告，指出您是代表該使用者進行註解。

>[!NOTE]
>
><span class="preview">使用新的評論體驗時，評論會新增為以其他使用者身份登入的使用者，且沒有跡象表明他們代表其他人新增評論。
>
>例如，如果Workfront管理員以其他使用者身份登入，則與評論相關聯的使用者為Workfront管理員。 如需詳細資訊，請參閱 [新的評論體驗](../../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). </span>


### 檢視稽核資訊 {#view-audit-information}

1. 以Workfront管理員或群組管理員身分登入Workfront。
1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) Adobe Workfront右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **登入身份，** 然後按一下 **存取記錄** 標籤。

   每當系統或群組管理員以其他使用者身份登入Workfront時，該事件就會記錄到稽核軌跡。 此外，當管理員以其他使用者身份登入時，所發生的任何可稽核動作都會登入稽核軌跡。

1. （選擇性）您可以以下列方式篩選稽核軌跡中顯示的結果：

   * 依已登入的使用者
   * 依登入身份的使用者
   * 依日期
