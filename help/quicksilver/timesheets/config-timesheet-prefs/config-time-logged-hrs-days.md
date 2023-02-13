---
product-area: timesheets;setup
navigation-topic: configure-timesheet-preferences
title: 配置時間是以小時還是天記錄
description: 身為擁有計畫授權的使用者，您可以設定是否在數小時或數天內登入Adobe Workfront。 系統管理員可以為個別使用者或組織中的多位使用者設定此設定。 預設情況下，用戶以小時為單位登錄時間。
author: Alina
feature: Timesheets
exl-id: 4f801a13-182d-4e06-98ea-f6863f6a8edf
source-git-commit: b4ab350af22afa44774f06d82daf1c3fb266d2b9
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 1%

---

# 配置時間是以小時還是天記錄

您是擁有規劃員授權的使用者，可以設定是否以小時或天為單位登入Adobe Workfront。 系統管理員可以為個別使用者或組織中的多位使用者設定此設定。 預設情況下，用戶以小時為單位登錄時間。 如需如何在Workfront中登入時間的詳細資訊，請參閱 [記錄時間](../../timesheets/create-and-manage-timesheets/log-time.md).

>[!NOTE]
>
>建議您在整個組織內以相同方式（小時或天）記錄時間，以確保報表正確無誤。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>規劃者可以為自己配置時間。 只有Workfront管理員可為其他使用者設定時間。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

1. 根據您的目標和系統中的訪問級別，執行下列任一操作：

   * **計畫員用戶為自己配置時間記錄：** 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，按一下個人資料圖片旁的您的使用者名稱。 然後，按一下 **更多** 圖示並選取 **編輯**.

   * **系統管理員為其他人配置時間記錄：** 開始編輯一個或多個用戶帳戶，如 [編輯使用者的設定檔](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. 在產生的對話方塊中， **資源規劃** 區段，找到 **登入時間** 選項。

   ![](assets/new-timesheet-log-hours-350x249.png)

1. （條件性）如果您是同時編輯多個用戶的系統管理員，請選擇 **登入時間**.
1. 從下列記錄時間選項中選取：

   | 選項 | 說明 |
   |---|---|
   | **時數** | 使用者在Workfront中記錄時間時指定小時。 |
   | **天** | 使用者可指定在Workfront中記錄時間的天數。 |

1. （條件性）若您選取以天為單位來記錄時間，請在 **完整Workday的等同小時數** 欄位，輸入等於一天的小時數。 用戶時間表上的某天等於您在此處輸入的小時數。

   設定此設定時，請考量下列事項：

   * 此選項在配置為以小時為單位記錄時間時不可用。
   * 此選項僅用於記錄時間。 此選項與 **排程** 選項（編輯使用者時也可用）。 此 **排程** 計算時間軸時，會在Workfront的其他區域中使用選項。 (如需使用 **排程** 選項，請參閱 [建立排程](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).) 

1. 按一下 **儲存變更**.
