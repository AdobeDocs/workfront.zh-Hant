---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: 新增使用者
description: 身為Workfront管理員或具有完整管理存取權的使用者，您可以在Workfront中新增使用者。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: e95dbc32-915b-4ea7-a5ad-e1da99edfbe3
source-git-commit: 198129edd8690393e3214f5041b183b5516617a7
workflow-type: tm+mt
source-wordcount: '1207'
ht-degree: 1%

---

# 新增使用者

<!--Audited 2/2024-->

>[!IMPORTANT]
>
>如果您的組織已上線Adobe Admin Console，您必須透過Adobe Admin Console建立系統管理員。
>
>如需在Adobe Admin Console中建立系統管理員的指示，請參閱 [在Adobe Admin Console中管理系統管理員](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).
>
>已加入Adobe Admin Console的組織中，群組管理員可使用此程式來建立使用者並提交使用者以供管理員核准。
>
>如需根據貴組織是否已加入Adobe Admin Console而有所差異的程式清單，請參閱 [平台型管理差異(Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

您可以從頭開始建立個別使用者，或複製現有使用者，以便在Adobe Workfront中新增使用者。

如需如何同時匯入多個使用者的詳細資訊，請參閱 [匯入使用者](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

<!--
Replace this intro with something like the following when we switch to Admin Console:
As an Adobe administrator, you can add users in Adobe Workfront by adding them to your Workfront product profile in the Adobe Admin Console. For instructions, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a>.
-->

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
   <td><p>新增：標準</p><p>或</p><p>目前：計畫</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須具備下列其中一項：</p> 
    <ul> 
     <li> <p>系統管理員存取層級。 如需詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整管理存取權</a>. </p> </li> 
     <li> <p><b>使用者</b> 將存取層級中的設定設為 <b>編輯</b> 存取，使用 <b>建立</b> 以及兩者中的至少一個 <b>使用者管理員</b> 選項已啟用於 <b>微調您的設定</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>這兩個選項中，如果使用者 <b>管理員（群組使用者）</b> 已啟用，您必須是使用者所屬群組的群組管理員。</p> <p>如需關於的詳細資訊 <b>使用者</b> 在存取層級中設定，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予使用者存取許可權</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 先決條件

在新增使用者之前，請收集下列使用者的相關資訊，並決定要與該使用者建立關聯的資訊：

* 什麼是使用者的個人資訊？ 您至少需要下列專案：

   * 完整名稱
   * 使用者名稱
   * 預設密碼
   * 電子郵件地址

  >[!NOTE]
  >
  >您可以在指定Workfront物件的存取層級時，微調「使用者檢視」設定，以判斷使用者是否可以檢視其他使用者的聯絡資訊。 如需詳細資訊，請參閱 [建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* 新使用者在公司中的位置為何？ 此人是否擁有任何直接下屬？ 此人會向誰報告？
* 人員會擔任什麼工作角色？ Workfront中是否有此工作角色？ 可以填補此職務角色的人數是否有限制？ 如需有關建立工作角色的資訊，請參閱 [建立和管理職位角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
* 使用者應該具有哪個存取層級？ 它已經存在嗎？還是您需要建立一個新的？ 如需詳細資訊，請參閱 [建立或修改自訂存取層級](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
* 此使用者應位於哪個主群組？ 此人是否應該屬於多個群組？ 如需群組的相關資訊，請參閱 [群組概述](../../../administration-and-setup/manage-groups/groups-overview/groups.md).
* 此使用者應該屬於哪個主團隊？ 此人是否應該隸屬於多個團隊？ 如需有關團隊的資訊，請參閱 [團隊概觀](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).
* 您需要將哪些自訂資訊與此使用者建立關聯？

  如果在您建立的自訂欄位中擷取有關使用者的資訊，則建立使用者時必須準備好自訂表單。 如需自訂表單的相關資訊，請參閱 [建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## 從頭開始建立使用者

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon.png) 在Adobe Workfront的右上角，或（如果有的話）按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon-left-nav.png) 然後按一下「 」 **使用者** ![](assets/users-icon-in-main-menu.png).

1. 按一下 **新增使用者>新增使用者** 新增尚未新增至Workfront的使用者。

   或

   按一下 **新增使用者>匯入使用者** 以上傳試算表匯入檔案來新增使用者。

   如果您正在匯入使用者，則不需要繼續這些步驟。 如需詳細資訊，請參閱 [匯入使用者](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

1. 在 **新使用者** 方塊中，按一下 **顯示進階選項**，然後設定可用的選項以輸入人員資訊。

   如需這些選項的相關資訊，請參閱 [編輯使用者設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. 執行下列其中一項：

   * 離開 **傳送邀請電子郵件給此人** 已啟用。 若您這麼做，使用者會收到電子郵件，追蹤連結以建立自己的Workfront密碼。 不接受電子郵件邀請並建立Workfront密碼的使用者，在Workfront中會列為「未註冊」。
   * 停用 **傳送邀請電子郵件給此人**，然後輸入 **密碼** ，並在中確認 **確認密碼** 方塊。 您需要與Workfront外部的使用者共用此密碼。

   >[!NOTE]
   >
   >* 如果您的Workfront管理員啟用了與Workfront的SSO整合，則僅允許 &lt;sso configuration=&quot;&quot;> 如果您停用電子郵件邀請，則會隱藏驗證欄位。 同盟ID或 &lt;sso configuration=&quot;&quot;> 使用者名稱欄位保持可見。
   >
   * 如果您的組織已加入Admin Console，而您透過Workfront新增使用者，則無法傳送電子郵件邀請。
   >
   對於現有的Adobe使用者，使用者可能會收到也可能不會收到有關Workfront可用性的電子郵件。 這是產品的Adobe管理員所控制的偏好設定。

1. 按一下 **新增此人**.

   或

   按一下 **新增人員並開始另一人員** 以儲存新使用者並新增另一個使用者。

   >[!NOTE]
   >
   如果您是群組管理員，負責將使用者新增至已加入Adobe Admin Console的組織，此步驟的選項為 **提交使用者以供管理員核准** 和 **提交以供核准並開始另一個**. 系統會在已停用及未決核准狀態中建立使用者。 Workfront管理員必須核准使用者，這樣才能在Workfront中啟用使用者，並將他們新增至Adobe Admin Console。

## 複製使用者以建立新使用者

您可以複製現有使用者來建立使用者。

>[!NOTE]
>
當您以這種方式建立使用者時，所有資訊都會從原始使用者複製到新建立的使用者，以下資訊除外：
>
* 「個人資訊」區段中的資訊。
* 當我登入時，顯示：在此方塊中會選取存取層級的預設登陸標籤。
* 直接下屬
>

若要複製現有使用者來建立新使用者，請執行下列動作：

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon.png) 在Adobe Workfront的右上角，或（如果有的話）按一下 **[!UICONTROL 主要功能表]** 圖示 ![主要功能表](/help/_includes/assets/main-menu-icon-left-nav.png) 然後按一下「 」 **使用者** ![](assets/users-icon-in-main-menu.png).
1. 選取您要複製的使用者，然後按一下復製圖示 ![](assets/copy-icon.png).
1. 在 **複製使用者** 方塊中，編輯新使用者可用的欄位。

   如需與使用者相關聯之所有欄位的詳細資訊，請參閱 [編輯使用者設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. 按一下 **新增此人**.

   或

   按一下 **新增人員並開始另一人員** 以儲存新使用者並新增另一個使用者。

這會在使用者的Workfront中建立新帳戶。

如果您選取傳送邀請給使用者的選項，使用者應會收到電子郵件，在其中他們可以依照連結建立其Workfront密碼。

>[!NOTE]
>
如果您的組織已加入Admin Console，而您透過Workfront新增使用者，則無法傳送電子郵件邀請。
>
對於現有的Adobe使用者，使用者可能會收到也可能不會收到有關Workfront可用性的電子郵件。 這是產品的Adobe管理員所控制的偏好設定。
