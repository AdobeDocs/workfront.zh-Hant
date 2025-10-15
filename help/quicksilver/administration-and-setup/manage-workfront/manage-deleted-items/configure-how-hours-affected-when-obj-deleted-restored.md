---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: 設定刪除和還原物件時數上的效果
description: 您可以設定在有人刪除專案、任務或時數記錄所針對的問題時，時數會發生什麼情況。 您選擇的選項也會決定在稍後還原專案、任務或問題時發生的小時數。 (如需有關在Workfront中還原專案的詳細資訊，請參閱還原已刪除的專案。)
feature: System Setup and Administration
role: Admin
exl-id: 466c3972-8108-49a6-98f6-f65f5fcc3617
source-git-commit: 156341072c291b5c03432da399a509d9772b73ea
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 1%

---

# 設定刪除和還原物件時數上的效果

您可以設定在有人刪除專案、任務或時數記錄所針對的問題時，時數會發生什麼情況。 您選擇的選項也會決定在稍後還原專案、任務或問題時發生的小時數。 (如需有關在Workfront中還原專案的詳細資訊，請參閱[還原已刪除的專案](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md)。)

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront套件</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td><p>標準</p>
       <p>規劃</p></td>
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td>系統管理員</td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 設定刪除和還原專案時如何管理小時

{{step-1-to-setup}}

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
