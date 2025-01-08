---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: 從展示板新增或移除成員
description: 必須先將人員新增到展示板作為成員，他們才能檢視展示板並獲指派給卡片。
author: Lisa
feature: Agile
exl-id: 8a46846c-f9b8-45cb-9923-e7596854557b
source-git-commit: bf8d566ba9d24310e75d2fbaf523fe5464bb6657
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 0%

---

# 從展示板新增或移除成員

{{highlighted-preview}}

必須先將人員和團隊新增到展示板中作為成員，他們才能檢視展示板。

根據預設，展示板的建立者是擁有者。 展示板擁有者是可在「設定」面板中刪除該展示板或更新其篩選器的唯一人員。 <span class="preview">只有系統管理員或目前的展示板擁有者可以變更展示板擁有者。</span>

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront]</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td> 
   <p>新增：[！UICONTROL Contributor]或以上</p> 
   <p>或</p>
   <p>目前： [！UICONTROL Request]或以上</p>
   </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 將成員新增至展示板

{{step1-to-boards}}

1. 建立新展示板或編輯現有展示板。 如需詳細資訊，請參閱[建立或編輯展示板](../../agile/get-started-with-boards/create-edit-board.md)。
1. 按一下&#x200B;**[!UICONTROL 新增成員]**&#x200B;圖示![新增成員](assets/boards-addmember-spectrum-25x25.png)。
1. 在「**[!UICONTROL 新增成員]**」方塊中，開始輸入名稱，然後在名稱顯示在清單中時選取名稱。

   您可以選取個別成員或專案團隊。 如果您選擇專案團隊，專案團隊本身會新增到展示板中。

   >[!NOTE]
   >
   >個別使用者必須在團隊的存取層級中設定&#x200B;**[!UICONTROL 檢視]**&#x200B;或&#x200B;**[!UICONTROL 編輯]**&#x200B;選項，否則將無法檢視展示板。


   ![新增成員至展示板](assets/boards-add-members.png)

## 從展示板移除成員

{{step1-to-boards}}

1. 建立新展示板或編輯現有展示板。 如需詳細資訊，請參閱[建立或編輯展示板](../../agile/get-started-with-boards/create-edit-board.md)。
1. 按一下&#x200B;**[!UICONTROL 新增成員]**&#x200B;圖示![新增成員](assets/boards-addmember-spectrum-25x25.png)。
1. 在&#x200B;**[!UICONTROL 新增成員]**&#x200B;方塊中，按一下人員或團隊名稱旁的X，即可將其從展示板中移除。

   ![從展示板移除成員](assets/boards-remove-member-from-board-350x367.png)

   當您從展示板中移除成員時，成員不會從指派給他們的任何卡片中移除。 對於已連線的卡片，指派也會在[!DNL Workfront]任務或問題上更新。

   成員只會從此展示板中移除。 它們不會從屬於的其他面板中移除。

   >[!NOTE]
   >
   >您無法移除展示板擁有者。

<div class="preview">

## 變更展示板所有者

>[!NOTE]
>
>只有系統管理員或目前的主機板擁有者可以變更主機板擁有者。 展示板只能有一個擁有者。
>
>基本、追溯和Kanban展示板提供變更展示板擁有者的功能，但動態展示板則不提供。

1. 存取展示板。
1. 按一下主機板名稱旁的&#x200B;**[!UICONTROL 更多]**&#x200B;功能表![更多](assets/more-icon-spectrum.png)，然後選擇&#x200B;**[!UICONTROL 變更主機板擁有者]**。
1. 在「變更展示板擁有者」對話方塊中，搜尋並選取想要成為擁有者的使用者。

   您無法搜尋已是展示板成員的使用者。 若要讓現有成員成為擁有者，您必須先從展示板中將其移除。 讓使用者成為展示板擁有者，會將使用者新增至展示板。

   只有使用者才能是展示板擁有者。 團隊不能是擁有者。

1. 按一下&#x200B;[!UICONTROL **更新**]。

</div>
