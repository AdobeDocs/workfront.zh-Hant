---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: 定義工時單的工時類型和可用性
description: 「小時類型」(Hour Type)是標籤，它允許您對時間條目進行分類。 視貴組織的報表需求而定，這可能是記錄時間的重要部分。
author: Alina
feature: Timesheets
exl-id: 3c07a6b0-4751-4fce-ac28-6a83084025d4
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '920'
ht-degree: 0%

---

# 定義工時單的工時類型和可用性

「小時類型」(Hour Type)是標籤，它允許您對時間條目進行分類。 視貴組織的報表需求而定，這可能是記錄時間的重要部分。

Adobe Workfront中有兩組小時類型：

* **一般小時數：** 與項目無關的小時數，例如病假或管理。 您只能記錄時間表上的一般小時數。
* **專案特定時數：** 登入專案、工作和問題的時數。 您可以從任何可以記錄時間的位置記錄專案特定小時。

在Workfront中記錄時間時，可用的專案特定小時類型取決於系統、專案和使用者層級所設定的設定選項。 (一律提供下列專案專用的預設小時類型：項目時間、任務時間和問題時間。)

可用於在記錄時間（對項目、任務和問題）時選擇的小時類型，首先由系統管理員在系統範圍內提供的小時類型確定，然後由在項目和用戶級別選擇的小時類型確定。

設定適當的小時類型後，您就可以從Workfront的多個位置記錄時間，如 [記錄時間](../../timesheets/create-and-manage-timesheets/log-time.md).

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
   <td> <p>計畫或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>系統管理員訪問以定義系統範圍的小時類型和編輯所有用戶</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td>管理專案的存取權，以定義專案的小時類型</td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫或授權類型，請聯絡您的Workfront管理員。

## 在系統級別定義可用性

系統管理員確定哪些特定項目小時類型在系統範圍內可用，如 [管理小時類型](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md) 區段  [管理小時類型](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## 在項目級別定義可用性 {#define-availability-at-the-project-level}

項目所有者確定在系統級別定義的所有小時類型是否在項目上可用（以及項目內的任務和問題），或者是否只有這些小時類型的子集可用。 

1. 轉到要確定小時類型可用性的項目。
1. 按一下 **更多** 菜單，然後按一下 **編輯**.

1. 按一下 **編輯專案**.
1. 在 **設定** 區段，找到 **篩選小時類型** 選項。

1. 選擇 **否** 讓專案上可使用所有專屬小時類型。

   或

   選擇 **是** 要使項目上僅提供項目特定小時類型的子集，請選擇要提供的小時類型。 （按住Shift鍵可選擇多個小時類型。）

   如果選擇此選項，則在記錄項目小時數時（或在項目內的任務和問題時），將僅提供您選擇的小時數類型。 如果您選取此選項，但未選取任何小時類型，則專案只會顯示一般小時類型。

   必須在個別使用者層級進行相同的選取，讓使用者在專案中看到這些小時類型選項。

1. 按一下 **儲存變更**.

## 在用戶級別定義可用性

只有在系統級別、項目級別和用戶級別都提供了該小時類型，您才可以記錄項目、任務和問題的指定小時類型。

如果您讓某個小時類型在用戶級別上可用（如本節所述），但在記錄項目、任務或問題時您沒有看到該小時類型，則該項目上尚未提供該小時類型(如 [在項目級別定義可用性](#define-availability-at-the-project-level))。

要定義用戶可用的小時類型，請執行以下操作：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 按一下左上角的使用者頭像。
1. 按一下 **更多** 功能表，然後按一下 **編輯**.

1. 只有系統管理員可以編輯其他使用者。 如果您有計畫許可證，則可以在自己的配置檔案中編輯小時類型。
1. 在 **資源規劃** 區段中 **可用小時類型** 下拉式選單中，根據您在記錄專案、任務或問題時要提供的小時類型，執行下列其中一項：

   * **要使所有小時類型均可供用戶使用，請執行以下操作：** 選擇所有小時類型。\
      如果您未選取所有小時類型，就與選取所有小時類型在技術上相同。 但在此情況下，所有小時類型僅適用於專案、工作和問題， **否** 在 **篩選小時類型** 選項，如 [在項目級別定義可用性](#define-availability-at-the-project-level).
   * **要僅讓用戶可以使用小時類型的子集：** 僅選擇要提供的小時類型。

      為了讓您在使用者層級選取的小時類型，可供專案、工作和問題使用，您也必須在 **篩選小時類型** 選項，如 [在項目級別定義可用性](#define-availability-at-the-project-level).

1. 按一下 **儲存變更**.

   現在，當您登錄項目、任務或問題的小時數時，如果在項目級別提供了相同的小時數類型，則您選擇的小時數類型可用。
