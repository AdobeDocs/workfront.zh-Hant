---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: 設定刪除和還原物件時的影響時間
description: 您可以設定在有人刪除專案、任務或時數記錄所針對的問題時，時數會發生什麼情況。 您選擇的選項也會決定在稍後還原專案、任務或問題時發生的小時數。 (如需有關在Workfront中還原專案的詳細資訊，請參閱還原已刪除的專案。)
feature: System Setup and Administration
role: Admin
exl-id: 466c3972-8108-49a6-98f6-f65f5fcc3617
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# 設定刪除和還原物件時的影響時間

您可以設定在有人刪除專案、任務或時數記錄所針對的問題時，時數會發生什麼情況。 您選擇的選項也會決定在稍後還原專案、任務或問題時發生的小時數。 (如需有關在Workfront中還原專案的詳細資訊，請參閱[還原已刪除的專案](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md)。)

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

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
   <td role="rowheader">存取層級設定</td> 
   <td> <p>您必須是Workfront管理員。</p> <p><b>注意</b>：如果您還是沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 設定刪除和還原專案時如何管理小時

1. 按一下Adobe Workfront右上角的&#x200B;**主要功能表**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下&#x200B;**設定** ![](assets/gear-icon-settings.png)。

1. 展開&#x200B;**時程表和時數**，然後按一下&#x200B;**偏好設定**。

1. 找出&#x200B;**專案、任務或問題刪除偏好設定**&#x200B;區段。
1. （視條件而定）若要設定刪除專案時數的管理方式，請在&#x200B;**刪除專案時**&#x200B;區段中選取下列其中一個選項：

   * 保留已新增至時程表的記錄時數作為一般時數（若日後還原此專案，時數仍會保留於時程表中）\
     依預設，會選取此選項。
   * 刪除任何記錄時數（若日後還原此專案，系統會將記錄時數還原至專案）

1. （視條件而定）若要設定刪除任務或問題時數的管理方式，請在&#x200B;**刪除任務或問題時**&#x200B;區段中選取下列其中一個選項：

   * 將任何記錄時數移至任務或問題所在的專案（若日後還原此任務或問題，時數仍會保留於專案）\
     依預設，會選取此選項。
   * 刪除任何記錄時數（若日後還原此任務或問題，記錄時數會還原至任務或問題）

1. 按一下「**儲存**」。
