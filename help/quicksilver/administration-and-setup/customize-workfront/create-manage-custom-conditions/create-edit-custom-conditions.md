---
title: 建立或編輯自訂條件
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: 作為Adobe Workfront管理員，您可以建立或編輯專案、任務和問題的自訂條件，以符合您組織的需求。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 5c950862-4358-4aab-997b-223972662150
source-git-commit: e50afb39f151ae8663ca2903454b475b21aa6f83
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 2%

---

# 建立或編輯自訂條件

作為Adobe Workfront管理員，您可以建立或編輯專案、任務和問題的自訂條件，以符合您組織的需求。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront套件</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront授權</td> 
   <td><p>標準</p>
       <p>規劃</p></td>
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td>系統管理員</td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 建立或編輯自訂條件

{{step-1-to-setup}}

1. 按一下&#x200B;**專案偏好設定** > **條件**。

1. 按一下您想要與條件關聯的物件型別（**專案**、**任務**&#x200B;或&#x200B;**問題**）的標籤。

1. 若要建立新條件，請按一下[新增條件] **&#x200B;**。

   或

   若要編輯現有條件，請按一下條件名稱旁的&#x200B;**編輯**。

   ![編輯自訂條件](assets/custom-conditions-0825.png)

1. 使用下列選項設定自訂條件：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>狀況名稱</td> 
      <td>（必要）輸入條件的描述性名稱。</td> 
     </tr> 
     <tr> 
      <td>說明</td> 
      <td>（選用）為要使用條件的人輸入條件用途說明。</td> 
     </tr> 
     <tr> 
      <td>顏色</td> 
      <td>（可選）按一下顏色圖示，然後選擇條件在專案、任務或問題中顯示時想要的顏色。 您也可以輸入十六進位數字。</td> 
     </tr> 
     <tr> 
      <td>等同於 </td> 
      <td><p>（必要，僅適用於專案）按一下下拉式清單中的選項，該選項最能說明新條件的功能。 例如，針對名為Tracking Well的條件，您可以按一下Target。 這會決定預設條件的運作方式。 您建立的每個條件都必須等同於下拉式選單中的其中一個選項。</p>
      <p>如需預設條件的詳細資訊，請參閱<a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md" class="MCXref xref">將自訂條件設為專案的預設值</a>以及<a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md" class="MCXref xref">將自訂條件設為任務和問題的預設值</a>。</p>
      <p>完成建立條件後，便無法修改此選項。</p></td> 
     </tr> 
     <tr> 
      <td>索引鍵</td> 
      <td><p>（必要）針對專案狀況，輸入使用者可辨識的英數字元縮寫。 若是任務或問題條件，請輸入01到99之間的兩位數數字代碼。 </p>
      <p>此金鑰用於API，且可用於報表用途，對每個物件而言必須是唯一的。</p>
      <p>儲存條件後，您無法變更條件的索引鍵。 </p></td> 
     </tr> 
     <tr> 
      <td>隱藏狀況</td> 
      <td><p>（選用）此選項適用於您不再想要讓人員使用，但因歷史原因而想要保留的自訂條件。 </p>
      <p>如果您隱藏已用於工作專案的自訂條件，則會在您隱藏後繼續顯示在這些工作專案上。 </p></td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >您可以標準化所有三種物件型別的條件術語和顏色。 若要這麼做，請從其中一個標籤（專案、任務、問題）將條件「名稱」和「顏色」十六進位程式碼複製到其他兩個標籤上的對應條件。

1. （選擇性）將![移動圖示](assets/move-icon---dots.png)任何條件拖曳到新位置，以重新排序清單。

   這會變更條件在專案、任務和問題中的顯示順序：

   * 當使用者編輯專案時

     編輯專案時![變更條件](assets/change-condition-edit-project-0825.png)

   * 當使用者在清單檢視中變更任務或問題的條件時：

     ![變更清單](assets/change-conditions-list-dropdown-0925.png)中的狀況

     >[!NOTE]
     >
     >在預設的「條件」檢視中，**條件**&#x200B;欄位是無法內嵌編輯的欄位型別。 當您單獨將&#x200B;**條件**&#x200B;欄位新增到檢視時，它是可編輯的。 如需內嵌編輯的詳細資訊，請參閱[在Adobe Workfront中內嵌編輯清單的專案](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md)。

1. 按一下「**儲存**」。

您可以將自訂條件設定為專案或任務和問題的預設條件。 如需詳細資訊，請參閱[將自訂條件設為專案的預設值](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md)以及[將自訂條件設為任務和問題的預設值](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md)。

如需自訂條件的詳細資訊，請參閱[自訂條件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md)。


<!-- THIS WAS ORIGINALLY BETWEEN THE OTHER TWO BULLETS.
   * When a user is changing the condition for a task or issue on the Updates tab:

     ![Change condition when updating comment](assets/change-condition-update-comment.png)
   -->
