---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 鎖定或解鎖系統中所有組的項目首選項
description: 組織中的群組可能需要針對其唯一工作流程以不同方式設定專案偏好設定。 您可以解除鎖定組織中所有群組的偏好設定，讓他們能夠自行設定。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f5a94eaf-ebb8-424b-80ff-ba40cc985a6e
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '518'
ht-degree: 0%

---

# 鎖定或解鎖系統中所有組的項目首選項

組織中的群組可能需要針對其唯一工作流程以不同方式設定專案偏好設定。 您可以解除鎖定組織中所有群組的偏好設定，讓他們能夠自行設定。

當首選項被解除鎖定，並且組管理員修改它時，與組相關聯的項目從組級別設定而不是從系統級別設定獲取該首選項的配置。

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

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
   <td>[!UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置</td> 
   <td> <p>您必須是 [!DNL Workfront] 管理員。</p> <p><b>注意</b>:如果您仍無法存取，請詢問您的 [!DNL Workfront] 管理員。 若要了解 [!DNL Workfront] 管理員可修改您的存取層級，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 關於鎖定和解除鎖定的偏好設定

鎖定您在系統級別配置的項目、任務或問題首選項可確保每個人使用該首選項的相同設定。 雖然您仍可以重新設定您鎖定的偏好設定，但群組管理員無法為其群組重新設定該偏好設定。

反之，解鎖項目、任務或問題首選項使組管理員能夠更靈活地管理其組處理這些項目的方式。 當首選項解除鎖定時，組管理員可以為其組重新配置它。

有關鎖定或解鎖系統級項目、任務或問題首選項的說明，請參閱 [配置全系統任務和問題首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!NOTE]
>
>之後 [!DNL Workfront] 管理員在系統級別解除對首選項的鎖定，任何組管理員都可以對其進行配置，然後將其鎖定，以確保組中的每個人以及下面的子組都使用相同的配置。 這與 [!DNL Workfront] 管理員必須配置並鎖定系統中每個人的首選項。 如需詳細資訊，請參閱 [配置組的項目首選項](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) 和 [鎖定或解除鎖定子組的項目、任務或問題首選項](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

## 解除鎖定專案偏好設定，讓群組可加以設定

1. 按一下 **[!UICONTROL 主菜單]** 圖示 ![](assets/main-menu-icon.png) 在 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 按一下 **[!UICONTROL 專案偏好設定]**，然後按一下 **[!UICONTROL 專案]**.

1. 執行下列任一操作：

   * 如果希望組管理員能夠為其組配置首選項，請解除鎖定 ![](assets/unlock-toggle-button.png).
   * 如果希望所有組都使用您的配置來獲取首選項，請確保它已鎖定（這是預設值）。

      >[!IMPORTANT]
      >
      >建議您與整個系統中群組的管理員和使用者通訊，以確保以您設定鎖定偏好設定的方式滿足所有需求。 當您鎖定它時，系統中的所有群組都會繼承您的設定。 如果首選項已在任意時間段內解除鎖定，則您的配置將替換組管理員可能所做的配置。

1. 按一下&#x200B;**[!UICONTROL 儲存]**。
