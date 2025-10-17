---
title: 停用或重新啟用使用者
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Workfront管理員可以停用或重新啟用使用者。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: aba243ba-46c2-4eb7-b704-4368bf0ae3cc
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '1081'
ht-degree: 2%

---

# 停用或重新啟用使用者 {#deactivate-or-reactivate-a-user}

>[!CONTEXTUALHELP]
>id="wf_users_deactivate_user"
>title="停用使用者"
>abstract="停用使用者，便會從 Workfront 和 Frame.io 中移除該使用者。已停用的使用者之後可以重新啟用。"

<!--Audited 5/2025-->

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on deactivating a user in the Adobe Admin Console, see the section "Remove users" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

-->

如果使用者離開組織，建議在系統中停用他們，以避免當其他使用者將他們新增到更新或指派他們工作時，造成混淆。 當您停用使用者時，其他使用者在系統中搜尋人員時不會再看到其名稱。

管理員可在設定區域中看到非作用中使用者。

您可以隨時重新啟用使用者。

>[!IMPORTANT]
>
>* 建議您停用已離開組織的使用者，而非刪除他們。 如果刪除使用者，則會遺失Workfront中與該使用者相關聯的所有記錄。 這包括他們的工作指派、他們與附註、時數、檔案及他們建立過的所有其他物件的關聯。
>
>* 在Workfront中停用使用者時，會移除使用者對Workfront和數位校訂的授權。 此外，無法再為該使用者指派工作。 當使用者停用時，該使用者的Workfront授權和校訂授權將可供其他使用者使用。 已停用使用者設定檔中的所有其他資訊維持不變。
>
>* 在Workfront中停用使用者時，不會從Adobe Admin Console的Workfront產品設定檔中移除該使用者。 如需詳細資訊，請參閱[刪除使用者](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md)。


## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront套件</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td><p>標準</p><p>規劃</p></td> 
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td> <p>您必須具備下列其中一項：</p> 
    <ul> 
     <li> <p>系統管理員存取層級。 </li> 
     <li> <p>您的存取層級中的<b>使用者</b>設定已設定為<b>編輯</b>存取權，其中<b>建立</b>以及在<b>微調您的設定</b> <b>下啟用的兩個</b>使用者管理員<img src="assets/gear-icon-in-access-levels.png">選項中的至少一個。 </p> <p>在這兩個選項中，如果已啟用<b>使用者管理員（群組使用者）</b>，您必須是使用者所屬群組的群組管理員。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

在停用Workfront管理員或Standard或Plan授權使用者之前，您必須將其物件和活動與其他使用者建立關聯。

如需詳細資訊，請參閱本文中的[關於停用Workfront管理員以及Standard或Plan授權使用者](#about-deactivating-workfront-administrators-and-plan-license-users)。

## 停用使用者

停用使用者時，請注意下列事項：

* 使用者將無法存取系統。
<!--* The user will be removed from Frame.io review links, assets, projects, and accounts.
   * Reactivating the user does not automatically add them back to the Frame.io items. You must reassign the user manually to Workfront projects, tasks, and assets that require Frame.io collaboration.-->
* 將會保留與使用者相關聯的所有資料。
* 您可以將已停用使用者的授權指派給其他使用者。

若要停用使用者：

{{step-1-to-users}}

1. 在使用者清單中選取使用者。
1. 按一下&#x200B;**更多**&#x200B;圖示![更多圖示](assets/more-icon.png)，然後按一下&#x200B;**停用**。

1. 在&#x200B;**停用使用者**&#x200B;對話方塊中，按一下&#x200B;**停用**。

## 排程使用者停用

身為經理，您可能想要在使用者實際離開您的組織之前將其標籤為停用。 例如，如果您與合約繫結的使用者合作，則他們會在您的系統中停留一段有限的時間，而您知道他們的終止日期。 您可以將它們排程為在該日期停用。

Workfront管理員和計畫授權使用者可在他們的使用者設定檔中檢視停用日期。

若要排程使用者停用，請執行下列動作：

{{step-1-to-users}}

1. 在使用者清單中選取使用者。

   或

   （選用）選取多位使用者以排程大量停用。

1. 按一下&#x200B;**編輯**&#x200B;圖示![編輯圖示](assets/edit-icon.png)。
1. 在&#x200B;**編輯使用者**&#x200B;方塊的左側面板中，按一下&#x200B;**資源規劃**。
1. 按一下&#x200B;**設定停用日期**。

1. 選取&#x200B;**停用日期**&#x200B;的日期和時間。

   >[!NOTE]
   >
   >* 在時間方塊中，您只能選取整小時增量，不能選取分鐘。
   >* 如果您選取已通過當天的時間，Workfront會將停用排程定於隔天凌晨12:00。
   >* 選取的時間符合正在排程停用之使用者的電腦時區。

1. 按一下「**儲存**」。

在選取的時間過後就會在選取的日期停用使用者。 如果您選取了多個要大量停用的使用者，則所有選取的使用者在選取的日期晚於選取的時間點停用。

我們建議您為您已排程停用的使用者建立報表，以隨時瞭解即將停用的使用者。 使用者停用後，無法確認是否已發生停用。

## 重新啟用使用者

{{step-1-to-users}}

1. 選取使用者，按一下&#x200B;**更多**&#x200B;圖示![更多圖示](assets/more-icon.png)，然後按一下&#x200B;**啟動**。

1. 在&#x200B;**重新啟用使用者**&#x200B;對話方塊中，從下拉式功能表中選取新的&#x200B;**存取層級**，然後按一下&#x200B;**重新啟用**。
<!--
### Asset review and approval impact when you reactivate a user

Deactivated users lose access to their assigned Frame.io accounts as well as assigned projects, assets, and review links. If you choose to reactivate the user, you must manually reassign them to projects, tasks, and assets that require Frame.io collaboration. -->

### 重新啟用使用者時的校訂影響

已停用的使用者會失去其獲指派的預設校訂角色及其校訂授權(如果您位於Workfront Premium舊版計畫)。 如果您選擇重新啟用使用者，您必須：

* 重新指派授權(如果您使用Workfront Premium舊版計畫)。 如需Workfront校訂計畫的詳細資訊，請參閱[存取Workfront中的校訂功能](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md)。
* 確認他們具有正確的校訂角色。 重新啟用的校訂使用者會被指派任何指定為新使用者預設校訂角色的角色。 如需詳細資訊，請參閱[設定預設校訂角色](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md)。

## 關於停用Workfront管理員和Standard或Plan授權使用者

在停用Workfront管理員或具有Plan授權的使用者之前，請務必檢查與該人員有關的Workfront物件和活動，然後視需要將其與其他Workfront管理員或Plan授權使用者相關聯。

這些物件與活動可能包含下列專案：

* 指派給使用者的任務或問題。
* 使用者擁有的專案。
* 設定為透過使用者的存取許可權執行的報表。
* 使用者擁有的範本。
* 使用者設定為資源管理員的專案和範本。
* 請求佇列路由規則Workfront管理員或計畫授權使用者是預設受指派人。
* 具有包含使用者的階段的核准流程（尤其是如果他們是該階段的唯一核准者）。
* 將使用者列為核准者的時程表。
* 將使用者列為核准者的時程表設定檔。
* 校訂包含使用者的自動化工作流程。

## 排定使用者停用時的資源規劃影響

當您排程停用使用者時，他們不再出現在資源規劃工具中，作為可用於預算時數。 如果它們仍然是資源集區的一部分，它們會出現在資源規劃工具中，但是它們的可用性將從它們排定的停用日期開始設定為零小時。

「資源規劃工具」會考慮使用者的所有職務角色與作業的「計畫完成日期」，並據此計算資源。

如需資源規劃工具的詳細資訊，請參閱[資源規劃工具概觀](../../../resource-mgmt/resource-planning/get-started-resource-planner.md)。

