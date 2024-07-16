---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: start-with-workfront-administration
title: 管理系統中的可用授權
description: 身為Adobe Workfront管理員，您可以存取有關Workfront帳戶的資訊，包括已為您的組織購買的授權數量，以及目前使用的授權數量。
author: Lisa, Becky
feature: System Setup and Administration
role: Admin
exl-id: ea580dd0-efb7-4f56-beb3-07ad044efc8a
source-git-commit: 834d08d8e9896b80d047d00b2008dd9a002a95da
workflow-type: tm+mt
source-wordcount: '1212'
ht-degree: 0%

---

# 管理系統中的可用授權

<!-- Audited: 12/2023 -->

身為Adobe Workfront管理員，您可以存取有關Workfront帳戶的資訊，包括已為您的組織購買的授權數量，以及目前使用的授權數量。

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
   <td>
    <p>新增：標準</p>
    <p>或</p>
    <p>目前：計畫</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是系統管理員或群組管理員。 群組管理員對授權資訊的檢視有限。</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

>[!NOTE]
>
>下列陳述式僅適用於新計畫。
>
>對於Select計畫：
>
>1. 系統管理員無法設定主群組的限制。
>2. 系統管理員只能看到所有主群組使用的授權總數。
>3. 群組管理員完全無法存取授權頁面。
>
>對於Prime與Ultimate計畫：
>
>1. 系統管理員可以將[主群組]新增到[授權]頁面，以檢視這些群組中的授權使用情況，也可以設定授許可權制。
>2. 群組管理員可以存取「授權」頁面，並檢視系統管理員已新增至「授權」頁面之他們管理的群組中的授權使用情況。
>3. 群組管理員無法檢視其他主群組的資訊或新增最大值。

+++

## 檢視您組織的授權

當您為新增至Workfront的使用者指派存取層級時，會自動更新使用中的授權數量。 如需詳細資訊，請參閱[新增使用者](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)。

若要檢視您系統中的授權資訊：

{{step-1-to-setup}}

1. 在左側面板底部，按一下&#x200B;**系統** > **授權**。

   如需此頁面所列授權的相關詳細資訊，請參閱[授權總覽](../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md)。

   >[!NOTE]
   >
   >校訂授權僅適用於已購買付費Workfront Proof附加元件以及其Workfront授權的客戶。 如需關於此附加元件的資訊，請參閱[Workfront Proof：文章索引](../../workfront-proof/workfront-proof.md)。

1. （視條件而定）如果您看到訊息&#x200B;**若要設定上限，您必須新增主群組**，請在您的系統中新增主群組，如本文中[新增或移除授權頁面](#add-or-remove-a-home-group-to-the-licenses-page)一節所述。

   >[!NOTE]
   >
   >對於新計畫，Select計畫不允許管理員依主群組檢視授權。 您只能看到使用的授權總數。 Prime和Ultimate計畫提供設定每個主群組最大授權數的功能。

## 檢視Workfront附加元件授權的相關資訊

如果您的組織有付費的Workfront Proof附加元件，則會顯示已使用的授權數量和可用的授權數量。 例如，10個校訂授權中的&#x200B;**5個**&#x200B;表示組織目前正在使用他們購買的10個Workfront Proof授權中的5個。

![Workfront附加元件的授權](assets/updated-licenses-page.png)

如果您的組織已購買Workfront Goals，則此產品的授權資訊也會顯示在這裡。 在此情況下，您可以檢視下列資訊：

* 貴公司已購買的Workfront目標授權總數
* 與使用者相關聯的Workfront目標授權數量。 這是在其存取層級中至少授予目標檢視存取許可權的使用者人數。

如需Workfront目標的相關資訊，請參閱[Adobe Workfront目標總覽](../../workfront-goals/goal-management/wf-goals-overview.md)。 如需存取Workfront目標的相關資訊，請參閱[授與Adobe Workfront目標的存取權](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)。

>[!NOTE]
>
>Workfront可讓您指派更多已購買的Workfront Goals授權。 但是，當您指派的授權超過Workfront目標合約所允許的數量時，Workfront客戶經理會聯絡您，告知您已超出合約數量。
>

<!--
If an organization has other paid add-on products, their license information also displays here. If the organization doesn't have any paid add-on products, nothing displays here. (Drafted this because not sure this is accurate: Scenario Planner is an add-on product and its licenses are not displayed there.)
-->

>[!TIP]
>
>沒有管理存取權的使用者可以使用群組報告來檢視授權計數。 在「報表」標籤中，建立新的群組報表並新增下列欄：
>
>* 授權型別限制：工作者限制
>* 授權型別限制：供需規劃員限制
>
>若要進一步瞭解如何建立報告，請參閱[建立自訂報告](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

## 檢視每月校訂和檔案決定分配的相關資訊

>[!IMPORTANT]
>
>校訂和檔案決定限制僅適用於擁有新授權的使用者。 如需詳細資訊，請參閱[新授權總覽](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md)。

所有非付費Workfront授權之校訂和檔案決定皆受限制。 每個月會重設每個使用者的限制。

每個授權的決定限制會依您所使用的計畫而有所不同。 您可以在「設定>授權」中檢視您每月的分配。

如需有關校訂和檔案決定限制的詳細資訊，請參閱[非付費使用者的有限檔案和校訂決定概覽](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md)。

![每月決策分配](assets/monthly-decision-allotment.png)

## 在[授權]頁面新增或移除主群組 {#add-or-remove-a-home-group-to-the-licenses-page}

<!--A Business or Enterprise Workfront Plan is required to use this feature. For more information about the various plans available, see [Workfront Plans.](https://www.workfront.com/plans)-->

每個使用者只能指派給一個主群組。 Workfront會計算每個主群組中已分配且目前使用的授權數量，以提供群組導向的授權計數。

如果您看到訊息&#x200B;**若要設定上限，您必須在[授權]頁面上新增主群組**，您必須在[授權]頁面上至少新增一個主群組。

>[!IMPORTANT]
>
>* 為了有效管理主群組的授權，我們建議在更新最大授權數量之前，先為業務單位設定特定的主群組。 如需詳細資訊，請參閱[主群組總覽](../../administration-and-setup/manage-groups/groups-overview/home-groups.md)。
>* 您只能將最上層群組新增為「主群組」，不能新增為子群組。 如果使用者將子群組指派為其主群組，則其授權會新增到該子群組之上頂層群組的授權計數中。
>

若要在[授權]頁面新增或移除[主群組]：

{{step-1-to-setup}}

1. 在左側面板底部，按一下&#x200B;**系統** > **授權**。

1. 按一下&#x200B;**管理群組清單**。
1. 開始在&#x200B;**主群組**&#x200B;方塊中輸入最上層群組的名稱。
1. 若要新增群組，請在群組出現時按一下其名稱。

   或

   若要移除群組，請按一下其名稱右側的X圖示。

1. 按一下「**儲存**」。

身為Workfront管理員，您可以設定主群組的授權數量上限，以防止業務單位使用為其他業務單位購買的Workfront授權。 如需指示，請參閱本文中的[設定主群組](#set-the-maximum-license-count-for-a-home-group)的最大授權計數。

## 設定主群組的授權數量上限 {#set-the-maximum-license-count-for-a-home-group}

身為Workfront管理員，您可以為系統中的最上層主群組設定授權數量上限。 這可讓您防止業務單位使用為組織內其他業務單位購買的Workfront授權。

根據預設，最大授權數設為N/A，這表示沒有限制。

群組管理員可檢視他們管理之主群組中已分配及使用的授權數目。 如需詳細資訊，請參閱[檢視群組](../../administration-and-setup/manage-groups/create-and-manage-groups/view-number-licenses-allocated-used-group.md)中配置及使用的授權數目。

若要設定主群組的最大授權數量：

{{step-1-to-setup}}

1. 在左側面板底部，按一下&#x200B;**系統** > **授權**。

1. 在清單中找出主群組。
1. 在群組的&#x200B;**Max**&#x200B;欄中，按一下您要設定最大值的值。
1. 輸入最大數字，然後按Enter鍵。

   ![](assets/updated-max.png)

   >[!NOTE]
   >
   >若要將群組的最大授權值設定回預設值，請勿輸入0。 請改為刪除方塊中的數字。 將最大授權值設定為0表示沒有授權配置給該群組。
