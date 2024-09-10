---
title: 存取系統專案狀態清單
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: 使用者可以指定專案狀態，讓其他使用者可以在指定時間檢視專案的目前開發階段。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 1fc91438-1ead-40d2-b0aa-863c1125c2fb
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 0%

---

# 存取系統專案狀態清單

使用者可以指定專案狀態，讓其他使用者可以在指定時間檢視專案的目前開發階段。

Workfront隨附9種系統專案狀態。 您可以變更這些狀態的名稱，但無法刪除它們。

您也可以新增自訂專案狀態以符合組織中的需求。

身為Workfront管理員，您可以為系統中的所有新專案設定預設狀態。 如需指示，請參閱[設定全系統的專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

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
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td><p>新增：標準</p>
       <p>或</p>
       <p>目前：計畫</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td>[！UICONTROL系統管理員]</td>
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 存取專案狀態

身為Workfront管理員，您可以存取系統層級專案狀態的清單。

如需有關編輯系統狀態和建立自訂狀態的資訊，請參閱[建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)。

{{step-1-to-setup}}

1. 按一下&#x200B;**專案偏好設定** > **狀態**。

1. 按一下「**專案**」標籤。

   此標籤會列出Workfront中可用的專案狀態。

   ![](assets/project-status.png)

   如需每個內建系統專案狀態的詳細資訊，請參閱[系統專案狀態概觀](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/system-project-statuses.md)。

## 建立自訂專案狀態和自訂系統狀態

身為Workfront管理員，您可以將系統專案狀態新增至Workfront。 身為群組擁有者，您可以新增專屬於一個群組的自訂狀態。 如需建立自訂狀態或編輯系統狀態的詳細資訊，請參閱[建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)。

當您建立自訂專案狀態時，必須始終將新狀態等同於現有系統狀態。 您必須瞭解系統狀態的行為，才能知道哪個狀態適合將您的自訂狀態等同於。 選取平等狀態後，此選取範圍即無法變更。 如需有關系統專案狀態的詳細資訊，請參閱[系統專案狀態概觀](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/system-project-statuses.md)。
