---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: start-with-workfront-administration
title: 管理系統中的可用許可證
description: 身為Adobe Workfront管理員，您可以存取Workfront帳戶的相關資訊，包括貴組織購買的授權數量，以及目前使用中的授權數量。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ea580dd0-efb7-4f56-beb3-07ad044efc8a
source-git-commit: 62d1b9563d83bd82b569e143f69e379e2f4ffbc2
workflow-type: tm+mt
source-wordcount: '1105'
ht-degree: 0%

---

# 管理系統中的可用許可證

身為Adobe Workfront管理員，您可以存取Workfront帳戶的相關資訊，包括貴組織購買的授權數量，以及目前使用中的授權數量。

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
   <td> <p>您必須是Workfront管理員。 如需詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完整的管理存取權</a>.</p> <p><b>注意</b>:如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 檢視貴組織的授權

當您將存取層級指派給您新增至Workfront的使用者時，使用中的使用授權數量會自動更新。 如需詳細資訊，請參閱 [新增使用者](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

要查看系統中的許可證資訊，請執行以下操作：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板底部，按一下 **系統** > **授權**.

   有關本頁所列許可證的詳細資訊，請參見 [授權概觀](../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

   >[!NOTE]
   >
   >除了Workfront授權外，證明授權僅適用於已購買付費Workfront Proof附加元件的客戶。 如需此附加元件的詳細資訊，請參閱 [Workfront校樣](../../workfront-proof/workfront-proof.md).

1. （條件性）如果您看到訊息 **要設定最大值，必須添加首頁組**，請在您的系統中新增首頁群組，如 [向「許可證」頁添加或刪除首組](#add-or-remove-a-home-group-to-the-licenses-page) 這篇文章。

## 檢視Workfront附加元件授權的相關資訊

在下面的螢幕截圖中， **10個證明許可證中的5個** 指出此組織具有付費的Workfront Proof附加元件，且目前使用其購買的10個Workfront Proof授權中的5個。

![](assets/updated-licenses-page.png)

如果您的組織已購買Workfront Targets，此產品的授權資訊也會顯示在此處。 在此情況下，您可以檢視下列資訊：

* 貴公司已購買的Workfront Target授權總數
* 與使用者相關聯的Workfront Target授權數量。 這是至少在其存取層級中授予「檢視」目標存取權的使用者人數。

如需Workfront目標的相關資訊，請參閱 [Adobe Workfront目標概覽](../../workfront-goals/goal-management/wf-goals-overview.md). 如需存取Workfront目標的相關資訊，請參閱 [授予Adobe Workfront目標的存取權](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)

>[!NOTE]
>
>Workfront可讓您指派已購買的更多Workfront Target授權。 不過，當您指派的授權數超過Workfront目標合約允許的數量時，Workfront客戶經理會聯絡您，告知您已超出合約編號。

<!--
If an organization has other paid add-on products, their license information also displays here. If the organization doesn't have any paid add-on products, nothing displays here. (Drafted this because not sure this is accurate: Scenario Planner is an add-on product and its licenses are not displayed there.)
-->

>[!TIP]
>
>沒有管理存取權的使用者可以使用群組報表來檢視授權計數。 在「報表」索引標籤中，建立新群組報表並新增下列欄：>
>* 許可證類型限制：工作人員限制
>* 許可證類型限制：計畫員限制
>
>若要進一步了解建立報表，請參閱 [建立自訂報表](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## 查看有關每月證明和文檔決策分配的資訊

>[!IMPORTANT]
>
>證明和檔案決策限制僅適用於新授權上的使用者。 如需詳細資訊，請參閱 [新許可證概述](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md).

所有未付費的Workfront授權均限制舉證和檔案決定。 每月按每位使用者重設的限制。

每個授權的決策限制會因您所執行的計畫而異。 您可以在「設定>授權」中檢視每月分配。

如需證明和檔案決策限制的詳細資訊，請參閱 [非付費使用者的有限檔案和證明決策概觀](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md).

![](assets/monthly-decision-allotment.png)

## 向「許可證」頁添加或刪除首組 {#add-or-remove-a-home-group-to-the-licenses-page}

使用此功能需要企業或企業Workfront計畫。 如需各種可用計畫的詳細資訊，請參閱 [Workfront計畫。](https://www.workfront.com/plans)

每個用戶只能被分配給一個主組。 Workfront會計算每個家庭群組中已分配和目前使用的授權數量，以提供以群組為導向的授權計數。

如果您看到訊息 **要設定最大值，必須添加首頁組** 在「許可證」頁上，您需要至少將一個首頁組添加到「許可證」頁。

>[!IMPORTANT]
>
>* 為了有效地使用主組管理許可證，建議在更新最大許可證數之前為業務單位設定特定的主組。 如需詳細資訊，請參閱 [首頁群組概觀](../../administration-and-setup/manage-groups/groups-overview/home-groups.md).
>* 您只能將頂層群組新增為「首頁群組」，而不能將子群組新增。 如果用戶有一個分組被分配為其「主組」，則其許可證將添加到該分組上方頂級組的許可證計數中。
>


要向「許可證」頁添加或刪除首組，請執行以下操作：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板底部，按一下 **系統** > **授權**.

1. 按一下 **管理群組清單**.
1. 開始在 **家庭組** 框。
1. 若要新增群組，請在顯示群組時按一下其名稱。

   或

   若要移除群組，請按一下群組名稱右側的X圖示。

1. 按一下&#x200B;**儲存**。

身為Workfront管理員，您可以為首頁群組設定最大授權計數，以防止業務單位使用為其他業務單位購買的Workfront授權。 如需指示，請參閱 [設定家庭組的最大許可證計數](#set-the-maximum-license-count-for-a-home-group) 這篇文章。

## 設定家庭組的最大許可證計數 {#set-the-maximum-license-count-for-a-home-group}

身為Workfront管理員，您可以為系統中的頂層首頁群組設定最大授權計數。 這可讓您防止業務單位使用您組織內其他業務單位購買的Workfront授權。

依預設，最大授權計數會設為N/A，這表示沒有限制。

組管理員可以查看他們管理的主組中分配和使用的許可證數量。 如需詳細資訊，請參閱 [在新Adobe Workfront體驗中檢視群組中分配和使用的授權數量](../../administration-and-setup/manage-groups/create-and-manage-groups/view-number-licenses-allocated-used-group.md).

要設定首頁組的最大許可證計數，請執行以下操作：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 在左側面板底部，按一下 **系統** > **授權**.

1. 在清單中找出首頁群組。
1. 在 **Max** 欄，按一下您要為設定最大值的值。
1. 輸入最大數，然後按Enter鍵。

   ![](assets/updated-max.png)

   >[!NOTE]
   >
   >要將組的最大許可值設定回預設值，請不鍵入0。 請改為刪除方塊中的數字。 將最大許可值設定為0表示沒有分配給該組的許可證。
