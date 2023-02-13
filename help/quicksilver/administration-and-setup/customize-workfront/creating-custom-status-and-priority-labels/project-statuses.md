---
title: 訪問系統項目狀態清單
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: 使用者可指定專案的狀態，讓其他使用者在指定的時間，就能查看專案目前的開發階段。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1fc91438-1ead-40d2-b0aa-863c1125c2fb
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 0%

---

# 訪問系統項目狀態清單

使用者可指定專案的狀態，讓其他使用者在指定的時間，就能查看專案目前的開發階段。

Workfront提供9種系統專案狀態。 您可以變更這些狀態的名稱，但無法刪除。

您也可以新增自訂專案狀態，以符合組織的需求。

您是Workfront管理員，可為系統中的所有新專案設定預設狀態。 如需指示，請參閱 [配置系統範圍的項目首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

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

## 存取專案狀態

身為Workfront管理員，您可以存取系統層級專案狀態清單。

有關編輯系統狀態和建立自定義狀態的資訊，請參閱 [建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **專案偏好設定** > **狀態**.

1. 按一下 **專案** 標籤。

   此標籤會列出Workfront中可用的專案狀態。

   ![](assets/project-status.png)

   如需每個內建系統專案狀態的詳細資訊，請參閱 [系統項目狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/system-project-statuses.md).

## 建立自訂專案狀態和自訂系統狀態

身為Workfront管理員，您可以將系統專案狀態新增至Workfront。 作為群組擁有者，您可以新增特定於一個群組的自訂狀態。 有關建立自定義狀態或編輯系統狀態的詳細資訊，請參閱 [建立或編輯狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

建立自訂專案狀態時，您必須一律將新狀態與現有系統狀態等同。 您必須了解系統狀態的行為，才能知道哪個狀態適合將自訂狀態等同於。 在您選擇了等於狀態後，無法更改此選擇。 有關係統項目狀態的詳細資訊，請參閱 [系統項目狀態](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/system-project-statuses.md).
