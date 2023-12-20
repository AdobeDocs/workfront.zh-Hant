---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 進行智慧型指派
description: 您可以使用智慧指派來識別最佳使用者是何人來完成工作。 智慧型指派是根據決定最適合工作資源的演演算法，將工作專案指派給資源時，Adobe Workfront會提供給您的使用者建議。 如需智慧指派的相關資訊，請參閱智慧指派概述。
author: Alina
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
source-git-commit: daba001c28df268721c87df7d2516ffb76e535d9
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---

# 進行智慧型指派

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers.</span>   
  
<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span> 
-->

您可以使用智慧指派來識別最佳使用者是何人來完成工作。 智慧型指派是根據決定最適合工作資源的演演算法，將工作專案指派給資源時，Adobe Workfront會提供給您的使用者建議。 如需智慧指派的相關資訊，請參閱 [智慧指派總覽](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

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
   * 「排程」或「排程」區域中的任務或問題
   * 工作負載平衡器中的任務或問題

1. 將游標置於指派欄位中，並等候兩秒。 此 **建議的指派** 或 **以下是一些建議** 清單隨即顯示。

   <!--check the casing for "assignments" should be lower case in task lists??-->

   <!--replace the last sentence above with this when we release smarter assignments:
   The **Suggested assignments** list displays. 
   NOTE (********and add preview tags for the note*****)
   The list header displays **Here are a few recommendations** instead of **Suggested assignments** in an issue list.
   -->

   ![](assets/smart-assignments-task-header-nwe-350x302.png)

   此清單中顯示的使用者是任務或問題的智慧指派建議。

   如需智慧指派顯示位置的詳細資訊，請參閱文章中的「尋找智慧指派建議」一節 [智慧指派總覽](../../../manage-work/tasks/assign-tasks/smart-assignments.md) .

1. 按一下使用者名稱，在建議清單中選取使用者。 按一下 **指派給我** 指派工作專案給您自己。

   >[!TIP]
   >
   >如果沒有建議，建議清單不會開啟。

1. （選擇性）如果您不想使用智慧指派清單中的其中一個建議使用者，請開始輸入所需使用者的名稱，並在該名稱出現在清單中時選取名稱。
1. 按一下 **輸入** 進行指派。

   所選的使用者已指派給任務或問題。
