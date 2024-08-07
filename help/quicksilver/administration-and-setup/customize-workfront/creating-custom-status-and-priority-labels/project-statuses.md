---
title: 存取系統專案狀態清單
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: 使用者可以指定專案狀態，讓其他使用者可以在指定時間檢視專案的目前開發階段。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1fc91438-1ead-40d2-b0aa-863c1125c2fb
source-git-commit: 59c3a57e334d1660e3e59da480a90060b1ba81b7
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 0%

---

# 存取系統專案狀態清單

使用者可以指定專案狀態，讓其他使用者可以在指定時間檢視專案的目前開發階段。

Workfront隨附9種系統專案狀態。 您可以變更這些狀態的名稱，但無法刪除它們。

您也可以新增自訂專案狀態以符合組織中的需求。

身為Workfront管理員，您可以為系統中的所有新專案設定預設狀態。 如需指示，請參閱[設定全系統的專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

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

## 存取專案狀態

身為Workfront管理員，您可以存取系統層級專案狀態的清單。

如需有關編輯系統狀態和建立自訂狀態的資訊，請參閱[建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)。

1. 按一下Adobe Workfront右上角的&#x200B;**主要功能表**&#x200B;圖示![](assets/main-menu-icon.png)，然後按一下&#x200B;**設定** ![](assets/gear-icon-settings.png)。

1. 按一下&#x200B;**專案偏好設定** > **狀態**。

1. 按一下「**專案**」標籤。

   此標籤會列出Workfront中可用的專案狀態。

   ![](assets/project-status.png)

   如需每個內建系統專案狀態的詳細資訊，請參閱[系統專案狀態概觀](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/system-project-statuses.md)。

## 建立自訂專案狀態和自訂系統狀態

身為Workfront管理員，您可以將系統專案狀態新增至Workfront。 身為群組擁有者，您可以新增專屬於一個群組的自訂狀態。 如需建立自訂狀態或編輯系統狀態的詳細資訊，請參閱[建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)。

當您建立自訂專案狀態時，必須始終將新狀態等同於現有系統狀態。 您必須瞭解系統狀態的行為，才能知道哪個狀態適合將您的自訂狀態等同於。 選取平等狀態後，此選取範圍即無法變更。 如需有關系統專案狀態的詳細資訊，請參閱[系統專案狀態概觀](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/system-project-statuses.md)。
