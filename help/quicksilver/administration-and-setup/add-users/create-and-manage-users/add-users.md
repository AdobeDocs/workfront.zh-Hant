---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: 新增使用者
description: 身為Workfront管理員或具有完整管理存取權的使用者，您可以在Workfront中新增使用者。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e95dbc32-915b-4ea7-a5ad-e1da99edfbe3
source-git-commit: 9bcd792139f8f2f0198da943e5c63a2add32e856
workflow-type: tm+mt
source-wordcount: '1176'
ht-degree: 1%

---

# 新增使用者

>[!IMPORTANT]
>
>本頁面上描述的程式僅適用於尚未上線至Admin Console的組織。 如果貴組織已上線至Adobe Admin Console，您必須透過Adobe Admin Console執行此動作。
>
>如需在Adobe Admin Console中新增使用者的指示：
>
>* 請參閱 [在Workfront中使用Adobe Admin Console建立使用者](../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md#create)
>* 請參閱文章中的「新增使用者」一節 [個別管理使用者](https://helpx.adobe.com/enterprise/using/manage-users-individually.html)
>* 請連絡您的Adobe Admin Console管理員。
>
>如需依貴組織是否已上線至Adobe Admin Console而有所不同的程式清單，請參閱 [平台管理差異(Adobe Workfront/Adobe業務平台)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

您可以從草稿開始建立個別使用者，或複製現有使用者，借此在Adobe Workfront中新增使用者。

如需如何同時匯入多個使用者的詳細資訊，請參閱 [匯入使用者](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

<!--
Replace this intro with something like the following when we switch to Admin Console:
As an Adobe administrator, you can add users in Adobe Workfront by adding them to your Workfront product profile in the Adobe Admin Console. For instructions, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a>.
-->

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
   <td> <p>您必須具備下列其中一項：</p> 
    <ul> 
     <li> <p>系統管理員訪問級別。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>. </p> </li> 
     <li> <p><b>使用者</b> 在您的存取層級中設定 <b>編輯</b> 存取，使用 <b>建立</b> 和兩者中的至少一個 <b>使用者管理</b> 選項 <b>微調您的設定</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>在這兩個選項中，如果用戶 <b>管理員（群組使用者）</b> 啟用時，您必須是使用者所屬群組的群組管理員。</p> <p>如需 <b>使用者</b> 在存取層級中設定，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取權</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 必要條件

新增使用者之前，請收集下列使用者的相關資訊，並決定您要與該使用者建立關聯的資訊：

* 使用者的個人資訊為何？ 您至少需要下列項目：

   * 全名
   * 使用者名稱
   * 預設密碼
   * 電子郵件地址

   >[!NOTE]
   >
   >您可以在指定Workfront物件的存取層級時，微調「使用者檢視」設定，以判斷使用者是否可以檢視其他使用者的聯絡資訊。 如需詳細資訊，請參閱 [建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* 新使用者在公司內的位置為何？ 此人是否有直接報告？ 此人向誰報告？
* 該人擔任什麼職務？ 此工作角色是否存在於Workfront中？ 可以擔任此職務的人數是否有限制？ 有關建立作業角色的資訊，請參閱 [建立和管理作業角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
* 使用者應具備哪些存取層級？ 它已存在嗎？還是需要建立新的？ 如需詳細資訊，請參閱 [建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
* 此使用者應位於哪個首頁群組？ 該人應屬於多個群組嗎？ 如需群組的相關資訊，請參閱 [群組概觀](../../../administration-and-setup/manage-groups/groups-overview/groups.md).
* 此使用者應屬於哪個主團隊？ 該人應該多個團隊嗎？ 如需團隊的相關資訊，請參閱 [團隊概觀](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).
* 您需要與此使用者建立關聯的自訂資訊為何？

   如果在您建立的自訂欄位中擷取了使用者的相關資訊，則建立使用者時必須準備好自訂表單。 如需自訂表單的相關資訊，請參閱 [建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## 從頭建立用戶

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **使用者** ![](assets/users-icon-in-main-menu.png).

1. 按一下 **新用戶>新用戶** 新增尚未新增至Workfront的使用者。

   或

   按一下 **新用戶>導入用戶** 上傳試算表匯入檔案以新增使用者。

   如果您要匯入使用者，則不需要繼續這些步驟。 如需詳細資訊，請參閱 [匯入使用者](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

1. 在 **新用戶** 框，按一下 **顯示高級選項**，然後配置可用選項以輸入人員資訊。

   如需這些選項的相關資訊，請參閱 [編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. 執行下列任一項作業：

   * 離開 **傳送邀請電子郵件給此人** 已啟用。 若您這麼做，使用者會收到電子郵件，通知他們可以在此連結建立自己的Workfront密碼。 不接受電子郵件邀請並建立Workfront密碼的使用者會在Workfront中列為「未註冊」。
   * 停用 **傳送邀請電子郵件給此人**，然後輸入 **密碼** 並在 **確認密碼** 框。 您需要與Workfront以外的使用者共用此密碼。

   >[!NOTE]
   >
   >若您的Workfront管理員已啟用與Workfront的SSO整合，則唯一允許 &lt;sso configuration=&quot;&quot;> 如果您停用電子郵件邀請，則會隱藏驗證欄位。 聯合ID或 &lt;sso configuration=&quot;&quot;> 使用者名稱欄位仍可見。

   >[!NOTE]
   如果您的組織已上線至Admin Console，而您透過Workfront新增使用者，便無法傳送電子郵件邀請。
   新的Adobe使用者會新增至Admin Console,Admin Console會傳送電子郵件邀請他們完成註冊程式。 所有用戶必須完成註冊過程才能訪問任何Adobe系統。
   若為現有的Adobe使用者，使用者可能會收到或不會收到有關Workfront可用的電子郵件。 這是由Adobe管理員控制的產品首選項。

1. 按一下 **添加此用戶**.

   或

   按一下 **添加人員用戶並啟動另一個用戶** 以保存新用戶並添加另一個用戶。

## 複製使用者以建立新使用者

您可以複製現有使用者，以建立使用者。

>[!NOTE]
以此方式建立用戶時，除以下內容外，所有資訊都會從原始用戶複製到新建立的用戶：
* 「個人資訊」區段中的資訊。
* 登入時，顯示：此方塊中會選取存取層級的預設登錄標籤。
* 直接下屬
>


要通過複製現有用戶來建立新用戶，請執行以下操作：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **使用者** ![](assets/users-icon-in-main-menu.png).
1. 選取您要複製的使用者，然後按一下「複製」圖示 ![](assets/copy-icon.png).
1. 在 **新用戶** 框中，編輯新用戶可用的欄位。

   如需與使用者相關聯的所有欄位資訊，請參閱 [編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. 按一下 **添加此用戶**.

   或

   按一下 **添加人員用戶並啟動另一個用戶** 以保存新用戶並添加另一個用戶。

這會在Workfront中為使用者建立新帳戶。

如果您選取要傳送邀請給使用者的選項，使用者應會收到電子郵件，並可在其中追蹤連結以建立其Workfront密碼。

>[!NOTE]
如果您的組織已上線至Admin Console，而您透過Workfront新增使用者，便無法傳送電子郵件邀請。
新的Adobe使用者會新增至Admin Console,Admin Console會傳送電子郵件邀請他們完成註冊程式。 所有用戶必須完成註冊過程才能訪問任何Adobe系統。
若為現有的Adobe使用者，使用者可能會收到或不會收到有關Workfront可用的電子郵件。 這是由Adobe管理員控制的產品首選項。
