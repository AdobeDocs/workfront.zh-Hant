---
title: 將自訂條件設定為專案的預設值
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: 如果專案的條件型別設定為進度狀態而非手動，Adobe Workfront會在專案進行時自動顯示專案上三個內建預設條件之一（達成目標、有風險或陷入困境），如專案條件和條件型別概觀中所述。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: dba052ed-83a2-44d2-b025-d970783c4151
source-git-commit: 1eab0317bfe72609133e71411ee24263517f1508
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---

# 將自訂條件設定為專案的預設值

{{highlighted-preview}}

如果專案的狀態型別設定為「進度狀態」而非「手動」，Adobe Workfront會在專案進行時，自動顯示專案上三個內建預設狀態之一（「達成目標」、「有風險」或「存在問題」），如[專案狀態與狀態型別概觀](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md)中所述。

專案標題![中的](assets/condition-in-project-header-nwe.png)狀況

您可以將自訂條件設定為預設條件，而不使用這三個內建的預設條件。 例如，您可以將「準時」預設條件變更為在所有專案中顯示為「追蹤良好」。

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

## 設定自訂條件作為所有專案的預設條件：

{{step-1-to-setup}}

1. 按一下&#x200B;**專案偏好設定** > **條件**。

1. 按一下「**專案**」標籤。
1. 按一下&#x200B;**設定預設條件**。
1. 在您要變更之預設條件的下拉式功能表中，按一下您要改用的自訂條件。
1. 針對您要變更的任何其他預設條件，重複上述步驟。
1. 按一下「**儲存**」。

如需有關設定自訂條件作為任務和問題的預設條件的資訊，請參閱[設定自訂條件作為任務和問題的預設值](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md)。

如需關於設定專案以便使用者可以手動更新其條件的資訊，請參閱[更新任務和問題的條件](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md)。
