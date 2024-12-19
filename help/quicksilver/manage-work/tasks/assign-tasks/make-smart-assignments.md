---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 進行智慧型指派
description: 您可以使用智慧指派來識別最佳使用者是何人來完成工作。 智慧型指派是Adobe Workfront在您根據演演算法將工作專案指派給資源時為您呈現的使用者、角色或團隊建議，該演演算法會決定最適合工作的資源。 如需智慧指派的相關資訊，請參閱智慧指派概述。
author: Alina
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
source-git-commit: 412645a802bdf9057bb61a5a96df257daa1c3948
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# 進行智慧型指派

<!--Audited: 07/2024-->

<!--keep the yellow around the Rate card job roles and the Preview intro for those-->

<span class="preview">本頁醒目提示的資訊指的是「生產」環境中僅供啟用快速發行之客戶使用的功能。</span>

<span class="preview">如需快速發行資訊，請參閱[為您的組織啟用或停用快速發行](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

<span class="preview">此功能將從「生產」環境中移除，適用於在2025年1月透過25.1版本啟用快速發行的客戶。 如需25.1版的詳細資訊，請參閱[2025年第一季度發行概述](/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-release-overview.md)。

您可以使用智慧指派來識別最佳使用者是何人來完成工作。

智慧型指派是Adobe Workfront將工作專案指派給資源時，為您呈現的使用者、角色或團隊建議。 Workfront的建議以演演算法為基礎，而演演算法會決定最適合這項工作的資源。

<span class="preview">在Workfront中有兩種不同的演演算法，可計算在工作和問題中運作方式不同的智慧指派。</span>

如需有關決定智慧指派所使用的條件的詳細資訊，請參閱[智慧指派總覽](/help/quicksilver/manage-work/tasks/assign-tasks/smart-assignments.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>新增：標準</p>
      或
      <p>目前：工作或以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯任務和問題的存取權</p> <p>檢視或更高專案存取權</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>Contribute或更高的許可權，能夠進行任務和問題的指派</p> </td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 進行智慧型指派

智慧指派適用於大部分可在Workfront中進行指派的位置。

1. 前往下列區域，然後按一下&#x200B;**指派**&#x200B;或&#x200B;**將此指派給**&#x200B;欄位：

   * 任務、問題清單或報告
   * 任務或問題標題
   * 任務或問題摘要面板
   * <span class="preview">新任務</span>或新問題方塊，當您新增<span class="preview">新任務</span>或問題至專案時
   * 工作負載平衡器中的任務或問題

1. 將游標置於「工作總攬」欄位中，並等候兩秒。

   對於問題，智慧指派會顯示在下列區段中：

   * **使用者和團隊**
   * **職位角色**

   ![](assets/smart-assignments-issue-header.png)

   對於任務，智慧型指派會根據演演算法計算識別指派的階段，顯示在下列區段中：

   * <span class="preview">**建議的指派**：顯示任務智慧指派演演算法第一個階段中識別的指派。</span>
   * **使用者和團隊**、**工作角色**，或&#x200B;<span class="preview">**評等卡片工作角色**</span>：在任務智慧指派演演算法計算的第二階段中識別的指派。

   <span class="preview">![](assets/smart-assignments-task-list.png)</span>

   如需詳細資訊，請參閱[智慧指派總覽](../../../manage-work/tasks/assign-tasks/smart-assignments.md)。

1. 按一下資源名稱，在建議清單中選取資源。

1. （選擇性）按一下&#x200B;**指派給我**&#x200B;以指派工作專案給您自己。

   >[!TIP]
   >
   >如果沒有建議，建議清單不會開啟。

1. （選擇性）如果您不想使用智慧指派清單中的任一建議使用者，請開始輸入所需資源的名稱，並在該名稱出現在清單中時選取名稱。
1. 按一下&#x200B;**Enter**&#x200B;以進行指派。

   所選的使用者已指派給任務或問題。
