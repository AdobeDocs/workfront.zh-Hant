---
title: 將自訂條件設為專案的預設值
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: 如果項目的「條件類型」設定為「進度狀態」而非「手動」，則Adobe Workfront會在項目進行時自動顯示項目（在Target上、在風險中或在故障中）的三個內置預設條件之一，如項目條件和條件類型的概述中所述。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: dba052ed-83a2-44d2-b025-d970783c4151
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 1%

---

# 將自訂條件設為專案的預設值

如果專案的「條件類型」設為「進度狀態」而非「手動」，Adobe Workfront會在專案進行時自動顯示專案的三個內建預設條件（「在目標上」、「有風險」或「有問題」）之一，如 [專案條件和條件類型概觀](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

![](assets/condition-in-project-header-nwe.png)

您可以將自訂條件設為預設條件，而不使用這三個內建的預設條件。 例如，您可以將「在目標上」預設條件變更為在所有專案中顯示為「追蹤良好」。

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

## 將自訂條件設為所有專案的預設條件：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，然後按一下 **設定** ![](assets/gear-icon-settings.png).

1. 按一下 **專案偏好設定** > **條件**.

1. 按一下 **專案** 標籤。
1. 按一下 **設定預設條件**.
1. 在您要變更之預設條件旁的下拉式功能表中，按一下您要改用的自訂條件。
1. 對您要變更的任何其他預設條件，重複上一步。
1. 按一下&#x200B;**儲存**。

如需將自訂條件設為工作和問題之預設條件的相關資訊，請參閱 [將自訂條件設為工作和問題的預設值](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md).

如需設定專案以便使用者手動更新其條件的相關資訊，請參閱 [更新任務和問題的條件](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md).

如需自訂條件的相關資訊，請參閱 [自訂條件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
