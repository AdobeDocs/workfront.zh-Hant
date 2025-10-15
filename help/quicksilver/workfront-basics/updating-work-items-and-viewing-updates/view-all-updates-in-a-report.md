---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 在備註報告中檢視所有更新
description: 若要檢視任何使用者為物件輸入的所有更新，您可以建立顯示所有更新的Note報告。
author: Alina
feature: Get Started with Workfront
exl-id: fa5b91e4-b88c-42f0-860c-6864105b4652
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---

# 在備註報告中檢視所有更新

<!-- Audited: 10/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is a report and it is in the Getting Started/ Updates section because I think it makes more sense to be in this area, where people want to view updates. - added this to this section from Reporting on 7/3/2018 ) </p>
-->

依預設，物件的「更新」區域最多可顯示200個更新。 若要檢視任何使用者為物件輸入的所有更新，您可以建立顯示所有更新的Note報告。

>[!NOTE]
>
>您可以使用日誌專案報告建置報告以檢視物件在預覽中的更新。 如需詳細資訊，請參閱[日誌專案報告的更新區域](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>標準</p>
   <p>規劃</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯存取權，並建立下列專案：</p> 
    <ul> 
     <li> <p>報告、儀表板和行事曆</p> </li> 
     <li> <p>篩選器、檢視和群組</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視報告中物件的許可權</p>
   </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard </p>
   <p>Current: Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to:</p> 
    <ul> 
     <li> <p>Create Reports, Dashboards, and Calendars</p> </li> 
     <li> <p>Create Filters, Views, and Groupings</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View</p>
    <p>Note: If you do not have View permission or higher to an object, information for that object doesn't display in the report.</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## 建立附註報告

不論物件為何，為任何物件建立附註的報告都是相同的。

例如，若要為專案中的所有附註建立附註報告：

{{step1-to-reports}}

1. 在頁面的左上角，按一下&#x200B;**新增報告**，然後選取&#x200B;**附註**。

1. （選擇性）按一下&#x200B;**（欄）檢視**，然後按一下&#x200B;**新增欄**，將&#x200B;**專案**&#x200B;的&#x200B;**名稱**&#x200B;新增至報表的檢視中。 

1. （選擇性）如果您同時針對多個專案製作報表，請按一下&#x200B;**群組**，然後按一下&#x200B;**新增群組**，依&#x200B;**專案**&#x200B;的&#x200B;**名稱**&#x200B;分組。 這可確保附註按其各自專案分組，使報告更易於閱讀。 

1. （選擇性）按一下&#x200B;**篩選器**，然後&#x200B;**新增篩選器規則**。
1. 為&#x200B;**記事** > **記事文字** > **不是空白的**。

   ![](assets/note-note-text-not-blank-filter.png)

   >[!TIP]
   >
   >   如果專案欄位已更新，但更新時未新增附註，則更新的&#x200B;**附註文字**&#x200B;會顯示為&#x200B;**（未新增文字至更新）**。


1. （選擇性）為&#x200B;**專案** > **名稱** > **等於**&#x200B;新增另一個篩選器，並新增一或多個您要檢視其附註的專案名稱。
1. 按一下&#x200B;**儲存+關閉**。 所有具有專案檢視許可權的使用者在專案中輸入的所有更新都會顯示在報表中。
