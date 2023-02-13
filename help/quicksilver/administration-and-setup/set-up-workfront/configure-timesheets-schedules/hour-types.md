---
user-type: administrator
content-type: reference
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: 管理小時類型
description: 您可以將小時類型與小時條目關聯。 小時類型是用於定義小時條目的標籤。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ad0d141b-3e56-4bb1-be24-4dd9203e7881
source-git-commit: 9f7f8a50bb805b1d6845df79ecffaa329d5abc26
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 0%

---

# 管理小時類型

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
**Linked to Creating Billing Record-->

您可以將小時類型與小時條目關聯。 小時類型是用於定義小時條目的標籤。

有兩組小時類型：

* **專案特定小時類型**:此時已登錄項目、任務和問題。 專案專屬的小時類型可與中任意位置的小時項目關聯 [!DNL Adobe Workfront] 您可以在其中記錄專案、工作和問題的時間。

   登入時 [!DNL Workfront]，可用的專案特定小時類型取決於系統、專案和使用者層級所設定的設定選項。

   下列預設專用小時類型一律可用：

   * 專案時間
   * 任務時間
   * 問題時間

   此 [!DNL Workfront] 管理員確定哪些特定項目小時類型可用，如 [定義工時單的工時類型和可用性](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

   >[!NOTE]
   >
   >如果您在 [!DNL Workfront] 系統中，系統中的每個項目必須至少啟用一個項目特定小時類型。 您無法在系統級別啟用特定於項目的小時類型，並且在項目級別不提供特定於項目的小時類型。

* **一般小時類型**:一般小時數不能與項目、任務或問題相關聯，並直接登錄到時間表。 如需記錄時間的詳細資訊，請參閱 [記錄時間](../../../timesheets/create-and-manage-timesheets/log-time.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront]計畫</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td>[!UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置</td> 
   <td> <p>您必須是 [!DNL Workfront] 管理員。</p> <p><b>注意</b>:如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 內建小時類型

Workfront隨附一組內建的小時類型。 無法編輯這些小時類型，也無法隱藏。

隨附的小時類型 [!DNL Workfront] 為：

* **[!UICONTROL 病假]**:無法與項目、任務或問題上的小時條目關聯的一般小時類型。
* **[!UICONTROL 休假時間]**:無法與項目、任務或問題上的小時條目關聯的一般小時類型。
* **[!UICONTROL 一般開銷]**:無法與項目、任務或問題上的小時條目關聯的一般小時類型。 不過，它可在您的專案規劃程式中計為收入。
* **[!UICONTROL 專案時間]**:一般小時類型，只能與專案上的小時項目相關聯。
* **[!UICONTROL 任務時間]**:一般小時類型，只能與任務上的小時條目相關聯。
* **[!UICONTROL 問題時間]**：一般小時類型，只能與問題上的小時項目相關聯。

## 建立小時類型

As a [!DNL Workfront] 管理員，您可以在系統和專案層級上為組織建立新的小時類型。 在系統和專案層級上建立小時類型後，使用者可以定義哪些小時類型可供特定專案和使用者使用。 如需詳細資訊，請參閱 [定義工時單的工時類型和可用性](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)

要建立新的小時類型：

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe] Workfront，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 按一下 **[!UICONTROL 時間表和小時數]** > **[!UICONTROL 小時類型]**.

1. 按一下 **[!UICONTROL 新小時類型].**
1. 請在 **[!UICONTROL 新小時類型]** 表單：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL名稱]</td> 
      <td>為新的小時類型命名，該名稱在系統中易於識別。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL描述]</td> 
      <td>為您的小時類型添加說明。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL範圍]</td> 
      <td> <p>通過在下拉菜單中選擇正確的範圍，定義小時類型是一般小時類型還是專用小時類型。</p> <p>一般小時類型僅在時間表中可見，不能與項目、任務或問題關聯。</p> <p><b>重要</b>:如果您的自定義小時類型為[!UICONTROL項目特定]，則將其更改為[!UICONTROL一般]，則所有現有任務、問題和項目小時都將設定為其系統預設類型。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL計為收入]</td> 
      <td>如果您希望與此小時類型關聯的小時條目影響收入計算，請選擇此選項。</td> 
     </tr> 
    </tbody> 
   </table>

   **[!UICONTROL 計為收入]**:如果您希望與此小時類型關聯的小時條目影響收入計算，請選擇此選項。

1. 按一下 **[!UICONTROL 建立小時類型].**

## 停用小時類型

如果小時類型已過時，並且您不再希望用戶將其小時條目與它們關聯，則可以停用小時類型。

停用小時類型會從中的任何位置隱藏小時類型 [!DNL Workfront] 顯示小時類型的位置。

停用小時類型：

1. 按一下 **[!UICONTROL 設定]** 在 [!DNL Adobe Workfront] 的下限。

1. 展開 **[!UICONTROL 工時單和工時首選項]**，然後按一下 **[!UICONTROL 小時類型]**.

1. 選擇要停用的小時類型。

1. 按一下 **[!UICONTROL 停用]**.
