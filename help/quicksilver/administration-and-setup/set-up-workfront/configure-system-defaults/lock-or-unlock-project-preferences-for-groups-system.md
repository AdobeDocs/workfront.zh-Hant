---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 鎖定或解除鎖定系統中所有群組的專案偏好設定
description: 您組織中的群組可能需要針對其獨特工作流程以不同方式設定的專案偏好設定。 您可以解鎖整個組織中所有群組的偏好設定，以便他們自行設定。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: f5a94eaf-ebb8-424b-80ff-ba40cc985a6e
source-git-commit: caaba90f4cdd835e1a1fddf16bcefa30995cca0d
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 0%

---

# 鎖定或解除鎖定系統中所有群組的專案偏好設定

您組織中的群組可能需要針對其獨特工作流程以不同方式設定的專案偏好設定。 您可以解鎖整個組織中所有群組的偏好設定，以便他們自行設定。

當偏好設定已解除鎖定且群組管理員修改時，與群組關聯的專案會從群組層級設定（而非系統層級設定）取得該偏好設定的組態。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td><p>新增：[！UICONTROL Standard]</p>
   或
   <p>目前： [！UICONTROL計畫]</p>
   </td> 
  </tr>
  <tr> 
   <td role="rowheader">存取層級設定</td>
   <td>[！UICONTROL系統管理員]</td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 關於鎖定和未鎖定的偏好設定

鎖定已在系統層級設定的專案、任務或問題偏好設定，可確保每個人都使用該偏好設定的相同設定。 雖然您仍然可以重新設定您鎖定的喜好設定，但群組管理員無法為其群組重新設定它。

反之，解鎖專案、任務或問題偏好設定可讓群組管理員擁有更大的彈性，可管理其群組處理這些專案的方式。 解鎖偏好設定時，群組管理員可以為其群組重新設定該偏好設定。

如果欄位沒有鎖定/解鎖切換，則群組管理員無法解鎖該欄位，無法在群組層級進行設定。 組態僅可在系統層級使用。

有關鎖定或解除鎖定系統層級專案、任務或問題偏好設定的說明，請參閱[設定系統範圍的任務和問題偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。

>[!NOTE]
>
>在[!DNL Workfront]管理員在系統層級解除鎖定偏好設定後，任何群組管理員都可以對其進行設定，然後將其鎖定，以確保其群組中的所有人和下面的子群組都使用相同的設定。 此功能與[!DNL Workfront]管理員必須設定並鎖定系統中每個人的偏好設定功能平行。 如需詳細資訊，請參閱[設定群組的專案偏好設定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)以及[鎖定或解除鎖定子群組的專案、任務或問題偏好設定](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md)。

## 解鎖專案偏好設定，讓群組可以設定它

{{step-1-to-setup}}

1. 按一下&#x200B;**[!UICONTROL 專案偏好設定]**，然後按一下&#x200B;**[!UICONTROL 專案]**。

1. 執行下列任一項作業：

   * 如果您希望群組管理員能夠設定其群組的偏好設定，請將其解鎖![](assets/unlock-toggle-button.png)。
   * 如果您希望所有群組都使用您的偏好設定設定，請確定它已被鎖定（這是預設值）。

     >[!IMPORTANT]
     >
     >我們建議您與整個系統群組內的管理員和使用者溝通，以確保以您設定鎖定偏好設定的方式考慮所有需求。 當您鎖定時，系統中的所有群組都會繼承您的設定。 如果偏好設定已解除鎖定任何時間段，您的設定會取代群組管理員可能已進行的設定。

1. 按一下「**[!UICONTROL 儲存]**」。
