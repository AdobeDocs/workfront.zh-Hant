---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 停用作業角色
description: 作為 [!DNL Adobe Workfront] 管理員或具有「作業角色」管理存取權的使用者，可以停用在您的系統中已過時的作業角色。 當您停用工作角色而非將其刪除時，可以保留與其相關聯的任何歷史資訊。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 934cef1a-8157-45db-b000-24a08a94dd18
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 0%

---

# 停用作業角色

作為 [!DNL Adobe Workfront] 管理員或具有「作業角色」管理存取權的使用者，可以停用在您的系統中已過時的作業角色。 當您停用工作角色而非將其刪除時，可以保留與其相關聯的任何歷史資訊。

您也可以重新啟用先前已停用的工作角色。

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront]計畫*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront]許可證*</td> 
   <td>[!UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>對作業角色的管理訪問</p> <p><b>注意</b>:如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 停用作業角色的影響

如果停用工作角色，則不再顯示在下列區域：

* 此 [!UICONTROL 分配] typeahead欄位（適用於任務、模板任務、問題、批准和路由規則）
* 此 [!UICONTROL 分配] 清單和報表中的欄位
* 使用者設定檔

   >[!NOTE]
   >
   >將新角色新增至使用者時，不會顯示停用的工作角色。 但它仍會顯示在 [!UICONTROL 主要角色] 和 [!UICONTROL 其他角色] 欄位中，如果使用者在停用前與工作角色相關聯。

* 此 [!UICONTROL 共用] 對象的對話框，包括佈局模板分配
* 自訂表單中的預先輸入欄位
* 此 [!UICONTROL 池成員] 欄位 [!UICONTROL 資源池]
* 此 [!UICONTROL 工作角色] 欄位a [!UICONTROL 計費率] 當用戶覆蓋項目的計費費率時，編輯螢幕
* 此 [!UICONTROL 向看板板添加分配] 對話框
* 此 [!UICONTROL 工作角色] 當某人使用 [!DNL Adobe Workfront Scenario Planner].

   此 [!DNL Scenario Planner] 只能在新 [!DNL Adobe Workfront] 體驗，且需要額外的授權。 如需 [!DNL Workfront Scenario Planner]，請參閱 [此 [!DNL Scenario Planner] 概述](../../../scenario-planner/scenario-planner-overview.md).

>[!TIP]
>
>停用的角色一律會顯示在清單、報表和其他工具(例如 [!DNL Workload Balancer].

## 停用作業角色前的考量事項

最好停用而非刪除已過時的作業角色，以便保留與您過去可能使用的角色相關聯的所有歷史資訊。

>[!NOTE]
>
>在停用之前，分配給作業角色的任何工作都將保持分配狀態。

建議您先執行下列操作，再停用未使用的工作角色：

* 為分配給您計畫停用的角色的任何對象建立報告，並將它們重新分配給活動的作業角色。 如需建立報表的相關資訊，請參閱 [建立報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

   >[!TIP]
   >
   >您可以建立報表以篩選指派停用角色的任何工作或問題。 然後，使用報告將未完成的任務或問題重新分配給活動角色。

* 清點所有審批流程、當前審批路徑以及分配給您計畫停用的任務職責的工藝路線規則或其他對象，並將它們重新分配給活動職責。

   >[!TIP]
   >
   >使用請求隊列時，如果禁用作為路由規則中預設受託人的作業角色，則該角色將保持不變，並且請求仍被路由到停用的角色。 建議您先更新具有作用中角色的路由規則，然後再停用團隊。

   有關建立審批流程和路由規則的資訊，請參閱以下文章：

   * [建立工作項的審批流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)
   * [建立路由規則](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)

## 停用作業角色

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一&#x200B;下 **[!UICONTROL 作業角色].**
1. （選用）在 **[!UICONTROL 篩選]** 下拉式功能表，選取 **[!UICONTROL 作用中]** 僅顯示活動作業角色。
1. 按一下要停用的作業角色的名稱。
1. 在 **[!UICONTROL 活動]** 下拉式功能表，選取 **[!UICONTROL 否]**.

   ![](assets/deactivate-job-role-edit-role-box-nwe.png)

1. 按一下 **[!UICONTROL 儲存變更]**.

   工作角色已停用，且無法再指派給工作、與版面範本相關聯等。 有關中作業角色的所有使用的資訊 [!DNL Workfront]，請參閱 [工作角色概觀](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).
