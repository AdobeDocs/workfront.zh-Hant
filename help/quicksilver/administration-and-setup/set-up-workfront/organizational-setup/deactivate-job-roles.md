---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 停用職位角色
description: 作為 [!DNL Adobe Workfront] 管理員或擁有工作角色管理存取權的使用者，您可以停用系統中過時的工作角色。 當您停用工作角色而不是刪除它時，您可以保留與其相關聯的任何歷史資訊。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 934cef1a-8157-45db-b000-24a08a94dd18
source-git-commit: 9c0160dc5e43f36b65d9f2d4a3498a9c5f39f6f1
workflow-type: tm+mt
source-wordcount: '692'
ht-degree: 0%

---

# 停用職位角色

作為 [!DNL Adobe Workfront] 管理員或擁有工作角色管理存取權的使用者，您可以停用系統中過時的工作角色。 當您停用工作角色而不是刪除它時，您可以保留與其相關聯的任何歷史資訊。

您也可以重新啟用先前已停用的工作角色。

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront]計畫*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront]授權*</td> 
   <td>[！UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>職位角色的管理存取權</p> <p><b>注意</b>：如果您還是無法存取，請詢問您的 [!DNL Workfront] 管理員是否對您的存取層級設定其他限制。 如需如何進行 [!DNL Workfront] 管理員可以修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有哪些計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 停用職務角色的影響

如果您停用工作角色，它不再顯示於以下區域：

* 此 [!UICONTROL 指定任務] 預先輸入欄位（適用於任務、範本任務、問題、核准和路由規則）
* 此 [!UICONTROL 指定任務] 清單和報告中的欄位
* 使用者設定檔

   >[!NOTE]
   >
   >當您將新角色新增到使用者時，停用的工作角色不顯示。 但它確實會繼續顯示在 [!UICONTROL 主要角色] 和 [!UICONTROL 其他角色] 欄位（若使用者在停用之前與工作角色相關聯）。

* 此 [!UICONTROL 共用] 物件的對話方塊，包括配置範本指派
* 自訂表單中的預先輸入欄位
* 此 [!UICONTROL 集區成員] 中的欄位 [!UICONTROL 資源集區]
* 此 [!UICONTROL 工作角色] 欄位 [!UICONTROL 收費率] 當使用者覆寫專案的計費費率時編輯畫面
* 此 [!UICONTROL 新增指派至Kanban面板] 對話方塊
* 此 [!UICONTROL 工作角色] 當有人使用時，為計畫或方案欄位 [!DNL Adobe Workfront Scenario Planner].

   此 [!DNL Scenario Planner] 僅於以下版本提供： [!DNL Adobe Workfront] 體驗並需要額外的授權。 如需關於以下專案的資訊： [!DNL Workfront Scenario Planner]，請參閱 [此 [!DNL Scenario Planner] 概觀](../../../scenario-planner/scenario-planner-overview.md).

>[!TIP]
>
>已停用的角色一律會顯示在清單、報告和其他工具(例如 [!UICONTROL 工作負載平衡器].

## 停用工作角色之前的考量事項

最好是停用，而不是刪除過時的職務角色，這樣您就可以保留與您過去可能使用過之角色相關的所有歷史資訊。

>[!NOTE]
>
>在停用之前指派給工作角色的任何工作都會維持指派狀態。

建議您先執行下列動作，再停用未使用的工作角色：

* 建立指派給您計畫停用之角色的任何物件報告，並將其重新指派給作用中工作角色。 如需建立報表的相關資訊，請參閱 [建立報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

   >[!TIP]
   >
   >您可以建立報告，以篩選已指派停用角色的任何任務或問題。 然後使用報告將未完成的任務或問題重新指派給作用中角色。

* 清查所有核准程式、目前核准路徑、製程規則或指定至您計畫停用之職務角色的其他物件，並將其重新指派給作用中角色。

   >[!TIP]
   >
   >使用請求佇列時，如果您停用在路由規則中指派為預設受指派人的工作角色，角色會保留，請求仍會路由到已停用的角色。 建議您先使用作用中角色更新路由規則，然後再停用專案團隊。

   如需有關建立核准程式和路由規則的資訊，請參閱下列文章：

   * [建立工作專案的核准流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)
   * [建立路由規則](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)

## 停用工作角色

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![](assets/main-menu-icon.png) 右上角的 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下&#x200B;。 **[!UICONTROL 職位角色].**
1. （選用）在 **[!UICONTROL 篩選]** 下拉式功能表，選取 **[!UICONTROL 作用中]** 以僅顯示作用中的職位角色。
1. 按一下要停用的工作角色名稱。
1. 在 **[!UICONTROL 為使用中]** 下拉式功能表，選取 **[!UICONTROL 否]**.

   ![](assets/deactivate-job-role-edit-role-box-nwe.png)

1. 按一下 **[!UICONTROL 儲存變更]**.

   工作角色已停用，無法再指派給工作、與版面配置範本關聯等。 有關職務角色的所有使用的資訊，請參見： [!DNL Workfront]，請參閱 [職務角色概觀](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).
