---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: 編輯劇本資訊
description: 在Kanban板上檢視內文拼貼時，可以直接從內文拼貼編輯某些資訊。
author: Lisa
feature: Agile
exl-id: a22a7b61-b331-4c98-9421-e7fccedcd096
source-git-commit: 9da0c8234f563a0202cd15017b37a341476f7406
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---

# 編輯劇本資訊

## 瞭解哪些資訊可以檢視和編輯 {#understand-what-information-can-be-viewed-and-edited}

在[!UICONTROL Kanban]展示板上檢視劇本拼貼時，可使用下表中的資訊。 您可以直接從內文拼貼內嵌編輯大部分資訊。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>資訊</strong> </th> 
   <th><strong>可見</strong> </th> 
   <th><strong>可編輯的內嵌</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>內文名稱，內有直接指向任務或問題的連結</td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>含有直接連結至專案的專案名稱</p> </td> 
   <td>✓ (A) </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>內文的完成點數或時數，以及指派給內文的點數或時數<br>這些數字用於計算並顯示每個內文的完成百分比。</p> </td> 
   <td>✓ (A)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>每個內文和問題的[！UICONTROL完成百分比]。<br>[！UICONTROL反複運算的完成百分比]是根據每個內文的[！UICONTROL完成百分比]計算的。<br></p> <p>更新內文或問題的[！UICONTROL完成百分比]時，您可以選擇0到100之間的任何數字。</p> </td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td> <p>將劇本指派給誰</p> </td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td> <p>圖磚的顏色或類別</p> </td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
  <tr> 
   <td> <p>任何可能透過修改敏捷檢視新增到敏捷檢視的其他欄位（包括自訂欄位），如[!DNL Adobe Workfront]</a>中<a href="../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">檢視總覽的「建立和自訂敏捷檢視」中所述</p> </td> 
   <td>✓ (A)</td> 
   <td>✓ (A)</td> 
  </tr> 
 </tbody> 
</table>

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計畫*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權*</strong></td> 
   <td> <p>[！UICONTROL Work]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>存取層級設定*</strong></td> 
   <td> <p>[！UICONTROL Worker]或更高版本</p> <p>注意：如果您還是沒有存取權，請詢問您的[!DNL Workfront]管理員是否對您的存取層級設定了其他限制。 如需[!DNL Workfront]管理員如何變更您的存取層級的詳細資訊，請參閱<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

## 檢視和編輯內文拼貼上的資訊

1. 按一下[!DNL Adobe Workfront]右上角的&#x200B;*[!UICONTROL *主功能表]**圖示![](assets/main-menu-icon.png)，然後按一下&#x200B;**[!UICONTROL 團隊]**。

1. （選擇性）按一下&#x200B;**[!UICONTROL 切換團隊]**&#x200B;圖示![切換團隊圖示](assets/switch-team-icon.png)，然後從下拉式選單中選取新的Kanban團隊或在搜尋列中搜尋團隊。

1. 移至[!UICONTROL Kanban]面板。
1. 展開內文拼貼以檢視與內文相關聯的所有欄位。

   ![](assets/story-expanded-on-kanban-board-2021-350x405.png)

1. （可選）若要編輯欄位，請按一下該欄位，然後進行任何變更。\
   您必須擁有任務或問題的[!UICONTROL 編輯]許可權，才能編輯劇本拼貼。\
   如需每個欄位及其是否可以編輯的詳細資訊，請參閱[瞭解哪些資訊可以檢視和編輯](#understand-what-information-can-be-viewed-and-edited)。

>[!NOTE]
>
>若要變更[!UICONTROL 完成百分比]，您必須輸入介於0到100之間的數字。 此欄位不是您可以移動的滑桿。
