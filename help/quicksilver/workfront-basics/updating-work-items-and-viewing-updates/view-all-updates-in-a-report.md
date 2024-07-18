---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 在備註報告中檢視所有更新
description: 在備註報告中檢視所有更新
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: fa5b91e4-b88c-42f0-860c-6864105b4652
source-git-commit: 36bdacb5f6d04245552aeeb4ab82d210597645a2
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 1%

---

# 在備註報告中檢視所有更新

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is a report and it is in the Getting Started/ Updates section because I think it makes more sense to be in this area, where people want to view updates. - added this to this section from Reporting on 7/3/2018 ) </p>
-->

依預設，物件的「更新」區域最多可顯示200個更新。 若要檢視任何使用者為物件輸入的所有更新，您可以建立顯示所有更新的Note報告。

>[!NOTE]
>
>您可以使用日誌專案報告建置報告以檢視物件在預覽中的更新。 如需詳細資訊，請參閱[更新區域報告](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md)。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront計畫</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront授權*</strong></td> 
   <td> <p>新增：標準 </p>
   <p>目前：計畫</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>存取層級設定</strong></td> 
   <td> <p>編輯下列專案的存取權：</p> 
    <ul> 
     <li> <p>建立報告、儀表板和行事曆</p> </li> 
     <li> <p>建立篩選器、檢視和群組</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件許可權</strong></td> 
   <td> <p>檢視</p> <p><b>附註</b></p>
   <p>如果您沒有物件的「檢視」許可權或以上許可權，該物件的資訊不會顯示在報表中。</p>  </td> 
  </tr> 
 </tbody> 
</table>

*如需詳細資訊，請參閱Adobe Workfront中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

## 建立附註報告

不論物件為何，為任何物件建立附註的報告都是相同的。

例如，若要為專案中的所有附註建立附註報告：

1. 按一下Adobe Workfront右上角的&#x200B;**主要功能表**&#x200B;圖示![](assets/main-menu-icon.png)。

1. 按一下&#x200B;**報表**。
1. 按一下&#x200B;**新增報告**，然後選擇&#x200B;**附註**。

1. （選擇性）按一下&#x200B;**檢視**，然後按一下&#x200B;**新增資料行**，將&#x200B;**專案**&#x200B;的&#x200B;**名稱**&#x200B;新增至報表的檢視中。 

1. （選擇性）如果您同時報告多個專案，請按一下&#x200B;**群組**，然後按&#x200B;**新增群組**&#x200B;以依&#x200B;**專案名稱**&#x200B;分組。\
   這可確保附註按其各自專案分組，使報告更易於閱讀。 

1. （選擇性）按一下&#x200B;**篩選器，**&#x200B;然後&#x200B;**新增篩選器規則**。
1. 為&#x200B;**記事** > **記事文字** > **不是空白的**。

   ![](assets/note-note-text-not-blank-filter.png)

   >[!TIP]
   >
   >   如果專案欄位已更新，但更新時未新增附註，則更新的&#x200B;**附註文字**&#x200B;會顯示為&#x200B;**（未新增文字至更新）**。


1. （選擇性）為&#x200B;**專案** > **名稱** > **等於**&#x200B;新增另一個篩選器，並新增一或多個您要檢視其附註的專案名稱。
1. 按一下「**儲存並關閉**」。\
   所有至少擁有檢視專案許可權的使用者在專案中輸入的所有更新都會顯示在報表中。
