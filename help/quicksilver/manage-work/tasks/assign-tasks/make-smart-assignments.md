---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 進行智慧型指派
description: 您可以使用智慧指派來識別最佳使用者是何人來完成工作。 智慧型指派是根據決定最適合工作資源的演演算法，將工作專案指派給資源時，Adobe Workfront會提供給您的使用者建議。 如需智慧指派的相關資訊，請參閱智慧指派概述。
author: Alina
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
source-git-commit: 08a7fa1f3871494c4c6b0c385a98a64735b7f7e4
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 0%

---

# 進行智慧型指派

<!--update "Results" to "Other assignments" with Prod-->

<span class="preview">本頁醒目提示的資訊指出尚未普遍可用的功能。 它僅在預覽環境中可供所有客戶使用。</span>

<span class="preview">如需目前發行排程的詳細資訊，請參閱 [2024年第二季版本總覽](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

您可以使用智慧指派來識別最佳使用者是何人來完成工作。

智慧型指派是根據決定最適合工作資源的演演算法，將工作專案指派給資源時，Adobe Workfront會提供給您的使用者建議。

<span class="preview">Workfront中有兩個用於任務和問題的獨立演演算法。 </span>
如需智慧指派的相關資訊，請參閱 [智慧指派總覽](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>新增：標準</p>
      或
      <p>目前：工作或以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯任務和問題的存取權</p> <p>檢視或更高專案存取權</p> <p><b>附註</b>

如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>分配或更高的許可權，能夠進行任務和問題的指派</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 進行智慧型指派

智慧指派適用於大部分可在Workfront中進行指派的位置。

1. 前往下列區域，然後按一下 **指定任務** 或 **將此指派至** 欄位：

   * 任務、問題清單或報告
   * 任務或問題標題
   * 任務或問題摘要面板
   * 「首頁」區域中列出之專案的「工作總攬」欄位
   * 工作負載平衡器中的任務或問題

1. 將游標置於指派欄位中，並等候兩秒。

   <span class="preview">此 **建議的指派** 清單隨即顯示。</span> <!--check the casing for "assignments" should be lower case in task lists??-->

   >[!TIP]
   >
   >   清單標題隨即顯示 **以下是一些建議** 而非 **建議的指派** 在問題清單中。

   ![](assets/smart-assignments-task-header-nwe-350x302.png)

   如果發生問題，智慧指派建議會顯示在 **建議的指派** 區域。

   對於任務，智慧型指派會根據演演算法計算識別指派的階段，顯示在下列區段中：

   * **建議的指派**：在任務智慧指派的演演算法計算的第一階段中識別的指派。
   * <span class="preview">**結果**：在任務智慧指派的演演算法計算的第二階段中識別的指派。 此區段不適用於問題。 </span> <!--replace this with the new UI: "Other assignments"-->

   ![](assets/smart-assignments-task-list.png)

   如需詳細資訊，請參閱 [智慧指派總覽](../../../manage-work/tasks/assign-tasks/smart-assignments.md) .

1. 按一下使用者名稱，在建議清單中選取使用者。

1. （選用）按一下 **指派給我** 以指派工作專案給您自己。

   >[!TIP]
   >
   >如果沒有建議，建議清單不會開啟。

1. （選擇性）如果您不想使用智慧指派清單中的其中一個建議使用者，請開始輸入所需使用者的名稱，並在該名稱出現在清單中時選取名稱。
1. 按一下 **輸入** 進行指派。

   所選的使用者已指派給任務或問題。
