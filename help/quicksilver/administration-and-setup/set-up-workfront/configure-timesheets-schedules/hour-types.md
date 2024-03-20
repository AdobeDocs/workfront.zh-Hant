---
user-type: administrator
content-type: reference
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: 管理小時型別
description: 您可以將時數型別與時數專案建立關聯。 小時型別是您用來定義小時專案的標籤。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ad0d141b-3e56-4bb1-be24-4dd9203e7881
source-git-commit: e881aa57b5175ce5b559180a2713de0c607b3b1d
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 0%

---

# 管理小時型別

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
**Linked to Creating Billing Record-->

您可以將時數型別與時數專案建立關聯。 小時型別是您用來定義小時專案的標籤。

時數型別有兩組：

* **特定專案小時型別**：這是專案、任務和問題的登入時間。 特定專案小時型別可以在中的任何地方與小時專案相關聯 [!DNL Adobe Workfront] 您可在此處記錄專案、任務和問題的時間。

  登入時間時 [!DNL Workfront]，可用的專案特定小時型別取決於在系統、專案和使用者層級設定的設定選項。

  以下專案專屬預設小時型別一律可用：

   * 專案時間
   * 任務時間
   * 問題時間

  此 [!DNL Workfront] 管理員會決定可提供哪些專案特定時數型別，如所述 [定義時程表的小時型別和可用性](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

  >[!NOTE]
  >
  >如果您在「 」中啟用任何特定專案小時型別， [!DNL Workfront] 時，您必須在系統中的每個專案上啟用至少一個特定專案小時型別。 您無法在系統層級啟用特定專案小時型別，且在專案層級沒有可用的特定專案小時型別。

* **一般小時型別**：一般時數無法與專案、任務或問題建立關聯，並直接記錄到時程表中。 如需有關記錄時間的詳細資訊，請參閱 [記錄時間](../../../timesheets/create-and-manage-timesheets/log-time.md).

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront]計畫</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td>[！UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是 [!DNL Workfront] 管理員。</p> <p><b>注意</b>：如果您還是沒有存取權，請詢問您的 [!DNL Workfront] 管理員是否對您的存取層級設定其他限制。 如需瞭解如何 [!DNL Workfront] 管理員可以修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 內建時數型別

Workfront隨附一組內建時數型別。 這些時數型別無法編輯且無法隱藏。

隨附的小時型別 [!DNL Workfront] 為：

* **[!UICONTROL 病假時間]**：一般時數型別，不得與專案、任務或問題的時數專案相關聯。 病假時數無法計算為收入。
* **[!UICONTROL 休假時間]**：一般時數型別，不得與專案、任務或問題的時數專案相關聯。 休假時間不能計為收入。
* **[!UICONTROL 一般管理費用]**：一般時數型別，不得與專案、任務或問題的時數專案相關聯。 不過，它可以在您的專案計畫程式中計為收入。
* **[!UICONTROL 專案時間]**：一般時數型別，只能與專案上的時數專案相關聯。
* **[!UICONTROL 任務時間]**：一般時數型別，只能與任務的時數專案相關聯。
* **[!UICONTROL 問題時間]**：一般時數型別，只能與問題的時數專案相關聯。

## 建立小時型別

作為 [!DNL Workfront] 管理員，您可以在系統和專案層級為貴組織建立新的時數型別。 在系統和專案級別上建立小時型別後，使用者可以定義哪些小時型別可用於特定專案和使用者。 如需詳細資訊，請參閱 [定義時程表的小時型別和可用性](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)

若要建立新的小時型別：

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![](assets/main-menu-icon.png) 位於的右上角 [!DNL Adobe] Workfront，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 按一下 **[!UICONTROL 時程表和時數]** > **[!UICONTROL 小時型別]**.

1. 按一下 **[!UICONTROL 新增小時型別].**
1. 指定下列資訊於 **[!UICONTROL 新增小時型別]** 表單：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL名稱]</td> 
      <td>為您的新時數輸入易於在系統中辨識的名稱。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL說明]</td> 
      <td>新增小時型別的說明。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL範圍]</td> 
      <td> <p>在下拉式選單中選取正確的範圍，定義時數型別是一般或專案特定的時數型別。</p> <p>一般小時型別僅在時程表中可見，並且不能與專案、任務或問題相關聯。</p> <p><b>重要</b>：如果您有特定於[！UICONTROL專案的自訂時數型別，然後您將其變更為[！UICONTROL一般]，則所有現有任務、問題和專案時數都會設定為其系統預設型別。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL計入收入]</td> 
      <td><p>如果您希望與此時數型別相關的時數條目影響您的收入計算，請選取此選項。</p>
      <p>病假和休假時間不計算為收入。</p>
      <p><b>附註</b></p>
      <p>當一般時數型別計入收入時，與記錄時間之使用者的設定檔相關聯的成本費率會與時數成本相關聯。  
      </td> 
     </tr> 
    </tbody> 
   </table>

   **[!UICONTROL 計入收入]**：如果您希望與此時數型別相關聯的時數條目影響您的收入計算，請選取此選項。

1. 按一下 **[!UICONTROL 建立小時型別].**

## 停用小時型別

如果小時型別過時，並且您不再希望使用者將其小時專案與其相關聯，您可以停用小時型別。

停用小時型別會從中的任意位置隱藏小時型別 [!DNL Workfront] 顯示時數型別的位置。

若要停用小時型別：

1. 按一下 **[!UICONTROL 設定]** 靠近的右上角 [!DNL Adobe Workfront] ，位於全域導覽列上。

1. 展開 **[!UICONTROL 時程表和小時喜好設定]**，然後按一下 **[!UICONTROL 小時型別]**.

1. 選取要停用的時數型別。

1. 按一下 **[!UICONTROL 停用]**.
