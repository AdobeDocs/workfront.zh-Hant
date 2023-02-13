---
title: 停用或重新啟用使用者
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 身為Workfront管理員，您可以停用或重新啟用使用者。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: aba243ba-46c2-4eb7-b704-4368bf0ae3cc
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1139'
ht-degree: 0%

---

# 停用或重新啟用使用者

>[!IMPORTANT]
>
>本頁面上描述的程式僅適用於尚未上線至Admin Console的組織。 如果貴組織已上線至Adobe Admin Console，您必須透過Adobe Admin Console執行此動作。
>
>如需在Adobe Admin Console中停用使用者的指示，請參閱文章中的「移除使用者」一節 [個別管理使用者](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) 或聯絡您的Adobe Admin Console管理員。
>
>如需依貴組織是否已上線至Adobe Admin Console而有所不同的程式清單，請參閱 [平台管理差異(Adobe Workfront/Adobe業務平台)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

您的使用者可能已離開組織，而您可能需要從Adobe Workfront中移除他們。 它們不應在系統中保持活動狀態，因為這樣會在將其他用戶添加到更新或指派其工作時造成混淆。 當您停用使用者時，其他使用者在系統中搜尋人員時，就不會再看見其名稱。

管理員可以在「設定」區域中看到非作用中使用者。

您可以隨時重新啟用使用者。

>[!IMPORTANT]
>
>建議您停用已離開組織的使用者，而非將其刪除。 如果刪除了某個使用者，則與該使用者相關聯的Workfront中所有歷史記錄都會遺失。 這包括其工作分配、與筆記、小時數、文檔的關聯，以及它們建立後的所有其他對象。
>
>在Workfront中停用使用者會移除使用者的Workfront和數位校對授權。 此外，無法再為用戶分配工作。 當使用者停用時，該使用者的Workfront授權和校對授權便可供其他使用者使用；已停用使用者設定檔中的所有其他資訊會維持原狀。
>
>如需刪除和停用使用者的影響的詳細資訊，請參閱 [刪除使用者](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

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
   <td> <p>計劃 </p>   </td> 
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

## 停用使用者

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **使用者** ![](assets/users-icon-in-main-menu.png).

1. 選取使用者，按一下「更多」圖示 ![](assets/more-icon.png)，然後按一下 **停用**.

1. 按一下 **停用** 框中。

## 排程使用者停用

身為經理，您可能想要在使用者實際離開您的組織前，將其標示為停用。 例如，如果您與合約約束的使用者合作，使用者在您的系統中只有一段有限的時間，而您知道他們的終止日期。 您可以排程在該日停用。

Workfront管理員和計畫授權使用者可以在其使用者設定檔中查看停用日期。

要安排用戶停用：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **使用者** ![](assets/users-icon-in-main-menu.png).

1. 選取使用者的名稱。

   或

   （可選）選取多個使用者，以排程大量停用。

1. 按一下「編輯」圖示 ![](assets/edit-icon.png).
1. 在顯示的「編輯使用者」方塊中，按一下 **資源規劃** 去那個地方。
1. 啟用 **計畫停用** 選項。

1. 在顯示的日曆中，指定 **計畫的停用日期**.

   >[!NOTE]
   >
   >* 在時間方塊中，您只能選取整小時的增量，而不能選取分鐘。
   >* 如果您選取當天已過的時間，Workfront會排程第二天凌晨12:00停用。 所選時間與正在計畫停用的用戶的電腦時區匹配。


1. 按一下 **儲存變更**.

   有時候在選取的時間之後，使用者會在選取的日期停用。 如果您選取多個使用者以大量停用，所有選取的使用者有時會在選取的當天之後停用。

建議您為已排程停用的使用者建立報表，以隨時了解即將停用的使用者。 一旦使用者停用，就無法確認停用是否已發生。

## 重新啟用使用者

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **使用者** ![](assets/users-icon-in-main-menu.png).

1. 選取使用者，按一下「更多」圖示 ![](assets/more-icon.png)，然後按一下 **啟動**.

1. 指派新 **存取層級**&#x200B;的下拉式清單。

### 重新啟用使用者時的校對影響

已停用的使用者會失去其指派的預設校對角色和其校樣授權(若您使用Workfront Premium舊版計畫)。 如果您選擇重新啟用使用者，您必須：

* 重新分配許可證(如果您在Workfront Premium舊計畫中)。 如需Workfront校對計畫的詳細資訊，請參閱 [存取Workfront中的校對功能](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).
* 確認他們擁有正確的校樣角色。 已重新啟動的校樣使用者會獲派新使用者指定的預設校樣角色。 請參閱 [配置預設校對角色](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md) 以取得更多資訊。

## 關於停用Workfront管理員和計畫授權使用者

在您停用Workfront管理員或具有計畫授權的使用者之前，請務必檢查Workfront物件和與該人員相關的活動，然後視需要將其與其他Workfront管理員或計畫授權使用者建立關聯。

這些物件和活動可能包括下列項目：

* 指派給使用者的工作或問題
* 使用者擁有的專案
* 設定為以使用者的存取權限執行的報表
* 使用者擁有的範本
* 將用戶設定為資源管理器的項目和模板
* 請求隊列路由規則，其中Workfront管理員或計畫許可證用戶是預設受託人
* 具有階段的核准程式，包括使用者（尤其是如果他們是該階段的唯一核准者）
* 將用戶列為批准者的時間表
* 將用戶列為批准者的時間表配置檔案
* 校對包含使用者的自動化工作流程

## 計畫用戶停用時，資源規劃會影響

當您計畫用戶停用時，資源計畫器中不再顯示用戶可用於預算小時數。 如果它們仍是資源池的一部分，則它們會顯示在資源規劃器中，但從計畫停用的日期開始，它們的可用性將設定為零小時。

Oracle Resource Planner將用戶的所有任務職責和任務的計畫完成日期考慮在內，並據此計算資源。

有關資源計畫員的詳細資訊，請參閱 [資源計畫員概覽](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).
