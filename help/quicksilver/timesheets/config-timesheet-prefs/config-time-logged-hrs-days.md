---
product-area: timesheets;setup
navigation-topic: configure-timesheet-preferences
title: 設定以小時或天記錄時間
description: 身為擁有Plan授權的使用者，您可以設定以小時或天為單位登入Adobe Workfront的時間。 系統管理員可以為個別使用者或其組織中的多個使用者設定此設定。 依預設，使用者會以小時記錄時間。
author: Alina
feature: Timesheets
exl-id: 4f801a13-182d-4e06-98ea-f6863f6a8edf
source-git-commit: 106ef838bfee5e496cae864eca5c19fd12fdd18e
workflow-type: tm+mt
source-wordcount: '455'
ht-degree: 1%

---

# 設定以小時或天記錄時間

作為具有Planner授權的使用者，您可以設定您是否以小時或天為單位在Adobe Workfront中記錄時間。 系統管理員可以為個別使用者或其組織中的多個使用者設定此設定。 依預設，使用者會以小時記錄時間。 如需有關如何在Workfront中記錄時間的資訊，請參閱[記錄時間](../../timesheets/create-and-manage-timesheets/log-time.md)。

>[!NOTE]
>
>我們建議在整個組織內以相同的方式記錄時間（小時或天數），以確保報告準確性。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

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
   <td> <p>規劃 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>規劃人員可以自行設定時間。 只有Workfront管理員可以為其他使用者設定時間。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

1. 請根據您的目標和系統中的存取層級，執行下列任一項作業：

   * **為自己設定時間記錄的Planner使用者：**&#x200B;按一下Adobe Workfront右上角的&#x200B;**主功能表**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下您的個人資料圖片旁的使用者名稱。 然後，按一下您名稱旁的&#x200B;**更多**&#x200B;圖示，並選取&#x200B;**編輯**。

   * **系統管理員設定其他人的時間記錄：**&#x200B;開始編輯一或多個使用者帳戶，如[編輯使用者的設定檔](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)中所述。

1. 在產生的對話方塊中，在&#x200B;**資源規劃**&#x200B;區段中，找到&#x200B;**在**&#x200B;中記錄時間選項。

   ![以選項](assets/user-profile-log-time-options.png)記錄時間

1. （視條件而定）如果您是同時編輯多個使用者的系統管理員，請選取&#x200B;**在**&#x200B;中記錄時間。
1. 從下列選項中選取記錄時間：

   | 選項 | 說明 |
   |---|---|
   | **小時** | 使用者在Workfront中記錄時間時指定小時。 |
   | **天** | 使用者可在Workfront中指定記錄時間。 |

1. （視條件而定）如果您選取以天為單位記錄時間，請在&#x200B;**完整Workday的同等時數**&#x200B;欄位中，輸入等於一整天的小時數。 在使用者的時程表上的一天等於您在此處輸入的小時數。

   進行此設定時，請考量下列事項：

   * 設定為以小時記錄時間時，此選項無法使用。
   * 此選項僅用於記錄時間。 此選項與編輯使用者時也可使用的&#x200B;**排程**&#x200B;選項無關。 **排程**&#x200B;選項用於計算時間表和Workfront的其他區域。 （如需使用&#x200B;**排程**&#x200B;選項的詳細資訊，請參閱[建立排程](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)。） 

1. 按一下「**儲存變更**」。
