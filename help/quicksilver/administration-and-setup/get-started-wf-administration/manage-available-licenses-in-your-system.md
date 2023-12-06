---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: start-with-workfront-administration
title: 管理系統中的可用授權
description: 身為Adobe Workfront管理員，您可以存取有關Workfront帳戶的資訊，包括已為您的組織購買的授權數量，以及目前使用的授權數量。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ea580dd0-efb7-4f56-beb3-07ad044efc8a
source-git-commit: 7467e75cf468fa6a1dd14dbc0f4fdcda87de1b1e
workflow-type: tm+mt
source-wordcount: '1111'
ht-degree: 0%

---

# 管理系統中的可用授權

身為Adobe Workfront管理員，您可以存取有關Workfront帳戶的資訊，包括已為您的組織購買的授權數量，以及目前使用的授權數量。

## 存取需求

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
   <td>計劃</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員。 如需詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整管理存取權</a>.</p> <p><b>注意</b>：如果您還是沒有存取權，請詢問Workfront管理員是否對您的存取層級設定了其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 檢視您組織的授權

當您將存取層級指派給您新增至Workfront的使用者時，會自動更新使用中的已使用授權數量。 如需詳細資訊，請參閱 [新增使用者](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

若要檢視您系統中的授權資訊：

1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) (位於Adobe Workfront的右上角)，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板底部，按一下 **系統** > **授權**.

   如需有關本頁所列之授權的詳細資訊，請參閱 [授權總覽](../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

   >[!NOTE]
   >
   >校訂授權僅適用於已購買付費的Workfront Proof附加元件以及其Workfront授權的客戶。 如需關於此附加元件的資訊，請參閱 [Workfront Proof：文章索引](../../workfront-proof/workfront-proof.md).

1. （視條件而定）如果您看到訊息 **若要設定上限，您必須新增主群組**，依照一節中的說明在您的系統中新增主群組 [在[授權]頁面新增或移除主群組](#add-or-remove-a-home-group-to-the-licenses-page) 本文章內容。

## 檢視Workfront附加元件授權的相關資訊

在下方的熒幕擷取畫面中， **10個校訂授權中的5個** 表示該組織擁有付費的Workfront Proof附加元件，且目前正在使用他們購買的10個Workfront Proof授權中的5個。

![](assets/updated-licenses-page.png)

如果您的組織已購買Workfront Goals，則此產品的授權資訊也會顯示在這裡。 在此情況下，您可以檢視下列資訊：

* 貴公司已購買的Workfront目標授權總數
* 與使用者相關聯的Workfront目標授權數量。 這是在其存取層級中至少授予目標檢視存取許可權的使用者人數。

如需Workfront目標的相關資訊，請參閱 [Adobe Workfront目標總覽](../../workfront-goals/goal-management/wf-goals-overview.md). 如需存取Workfront目標的相關資訊，請參閱 [授予Adobe Workfront目標的存取權](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)

>[!NOTE]
>
>Workfront可讓您指派更多已購買的Workfront Goals授權。 但是，當您指派的授權超過Workfront目標合約所允許的數量時，Workfront客戶經理會聯絡您，告知您已超出合約數量。
>

<!--
If an organization has other paid add-on products, their license information also displays here. If the organization doesn't have any paid add-on products, nothing displays here. (Drafted this because not sure this is accurate: Scenario Planner is an add-on product and its licenses are not displayed there.)
-->

>[!TIP]
>
>沒有管理存取權的使用者可以使用群組報告來檢視授權計數。 在「報表」標籤中，建立新的群組報表並新增下列欄：>
>* 授權型別限制：工作者限制
>* 授權型別限制：供需規劃員限制
>
>若要進一步瞭解如何建立報告，請參閱 [建立自訂報表](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
>

## 檢視每月校訂和檔案決定分配的相關資訊

>[!IMPORTANT]
>
>校訂和檔案決定限制僅適用於擁有新授權的使用者。 如需詳細資訊，請參閱 [新授權總覽](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md).

所有非付費Workfront授權之校訂和檔案決定皆受限制。 每個月會重設每個使用者的限制。

每個授權的決定限制會依您所使用的計畫而有所不同。 您可以在「設定>授權」中檢視您每月的分配。

如需有關校訂和檔案決定限制的詳細資訊，請參閱 [非付費使用者的有限檔案和校訂決定概覽](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md).

![](assets/monthly-decision-allotment.png)

## 在[授權]頁面新增或移除主群組 {#add-or-remove-a-home-group-to-the-licenses-page}

需要商業或企業Workfront計畫才能使用此功能。 如需各種可用計畫的詳細資訊，請參閱 [Workfront計畫。](https://www.workfront.com/plans)

每個使用者只能指派給一個主群組。 Workfront會計算每個主群組中已分配且目前使用的授權數量，以提供群組導向的授權計數。

如果您看到訊息 **若要設定上限，您必須新增主群組** 在[授權]頁面上，您需要將至少一個主群組新增到[授權]頁面。

>[!IMPORTANT]
>
>* 為了有效管理主群組的授權，我們建議在更新最大授權數量之前，先為業務單位設定特定的主群組。 如需詳細資訊，請參閱 [主群組概觀](../../administration-and-setup/manage-groups/groups-overview/home-groups.md).
>* 您只能將最上層群組新增為「主群組」，不能新增為子群組。 如果使用者將子群組指派為其主群組，則其授權會新增到該子群組之上頂層群組的授權計數中。
>

若要在[授權]頁面新增或移除[主群組]：

1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) (位於Adobe Workfront的右上角)，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板底部，按一下 **系統** > **授權**.

1. 按一下 **管理群組清單**.
1. 開始在「 」中輸入頂層群組的名稱 **主群組** 方塊。
1. 若要新增群組，請在群組出現時按一下其名稱。

   或

   若要移除群組，請按一下其名稱右側的X圖示。

1. 按一下&#x200B;**儲存**。

身為Workfront管理員，您可以設定主群組的授權數量上限，以防止業務單位使用為其他業務單位購買的Workfront授權。 如需指示，請參閱 [設定主群組的授權數量上限](#set-the-maximum-license-count-for-a-home-group) 本文章內容。

## 設定主群組的授權數量上限 {#set-the-maximum-license-count-for-a-home-group}

身為Workfront管理員，您可以為系統中的最上層主群組設定授權數量上限。 這可讓您防止業務單位使用為組織內其他業務單位購買的Workfront授權。

根據預設，最大授權數設為N/A，這表示沒有限制。

群組管理員可檢視他們管理之主群組中已分配及使用的授權數目。 如需詳細資訊，請參閱 [在新的Adobe Workfront體驗中檢視群組中配置及使用的授權數量](../../administration-and-setup/manage-groups/create-and-manage-groups/view-number-licenses-allocated-used-group.md).

設定主群組的授權數量上限：

1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) (位於Adobe Workfront的右上角)，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板底部，按一下 **系統** > **授權**.

1. 在清單中找出主群組。
1. 在 **最大** 欄中，按一下要設定最大值的值。
1. 輸入最大數字，然後按Enter鍵。

   ![](assets/updated-max.png)

   >[!NOTE]
   >
   >若要將群組的最大授權值設定回預設值，請勿輸入0。 請改為刪除方塊中的數字。 將最大授權值設定為0表示沒有授權配置給該群組。
