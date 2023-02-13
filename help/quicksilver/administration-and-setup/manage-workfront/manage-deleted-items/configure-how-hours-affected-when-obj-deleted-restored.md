---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: 配置對象被刪除和還原時對時間的影響
description: 您可以設定當某人刪除專案、任務或記錄該小時時，會發生什麼情況。 您選擇的選項也決定了稍後還原專案、任務或問題時的時數。 (如需在Workfront中還原項目的詳細資訊，請參閱還原已刪除的項目。)
feature: System Setup and Administration
role: Admin
exl-id: 466c3972-8108-49a6-98f6-f65f5fcc3617
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# 配置對象被刪除和還原時對時間的影響

您可以設定當某人刪除專案、任務或記錄該小時時，會發生什麼情況。 您選擇的選項也決定了稍後還原專案、任務或問題時的時數。 (如需在Workfront中還原項目的詳細資訊，請參閱 [還原已刪除的項](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).)

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
   <td> <p>您必須是Workfront管理員。</p> <p><b>注意</b>:如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 配置刪除和還原項時如何管理小時

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 展開 **工時單和小時數**，然後按一下&#x200B;**偏好設定**.

1. 找出 **項目、任務或問題刪除首選項** 區段。
1. （條件性）若要設定刪除專案時的管理小時數，請在 **刪除專案時** 小節：

   * 將已添加到工時單的記錄小時數保留為一般小時數（如果此項目稍後恢復，則工時數將保留在工時單中）\
      預設會選取此選項。
   * 刪除任何記錄的小時數（如果此專案稍後還原，則記錄的小時數會還原至專案）

1. （條件性）若要設定在刪除任務或問題時如何管理小時，請在 **刪除任務或問題時** 小節：

   * 將任何記錄的小時數移至任務或問題所在的專案（如果稍後還原此任務或問題，則該小時數仍保留在專案中）\
      預設會選取此選項。
   * 刪除任何記錄的小時數（如果稍後還原了此任務或問題，則將將記錄的小時數還原為任務或問題）

1. 按一下&#x200B;**儲存**。
