---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 在「附註」報表中檢視所有更新
description: 在「附註」報表中檢視所有更新
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: fa5b91e4-b88c-42f0-860c-6864105b4652
source-git-commit: 923c9e25fbd73c9d6a6a20436333c6e7969e9538
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 0%

---

# 在「附註」報表中檢視所有更新

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is a report and it is in the Getting Started/ Updates section because I think it makes more sense to be in this area, where people want to view updates. - added this to this section from Reporting on 7/3/2018 ) </p>
-->

對象的「更新」(Updates)區域預設顯示最多200次更新。 若要查看任何使用者為物件輸入的所有更新，您可以建立「附註」報表以顯示所有更新。

>[!NOTE]
>
>您可以建立報告，在「預覽」中使用日記帳分錄報告查看對象的更新。 如需詳細資訊，請參閱 [更新區域報告](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront計畫*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront授權*</strong></td> 
   <td> <p>計劃</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>訪問級別配置*</strong></td> 
   <td> <p>編輯對以下項目的訪問：</p> 
    <ul> 
     <li> <p>建立報表、控制面板和日曆</p> </li> 
     <li> <p>建立篩選、檢視和群組</p> </li> 
    </ul> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。<br>如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件權限</strong></td> 
   <td> <p>檢視</p> <p>注意：如果您沒有某個對象的「查看」權限或更高版本，則該對象的資訊不會顯示在報告中。</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 建立附註報表

為任何物件建立「附註」報表都相同，無論該物件為何。

例如，要為項目上的所有附註建立附註報表：

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 按一下 **報表**.
1. 按一下 **新增報表**，然後選擇 **附註**.

1. （選用）按一下 **檢視**，然後 **添加列** 若要新增 **名稱** 的 **專案** 在報表檢視中。 

1. （選用）按一下 **分組**，然後 **添加分組** 分組 **專案名稱**，則此量度不會受到任何影響。\
   這可確保將附註依其個別專案分組，讓報告更容易閱讀。 

1. （選用）按一下 **篩選器，** then **新增篩選規則** 僅篩選一個專案或特定專案。

1. （條件式和選用式）設定 **專案名稱** as **等於** 至您要檢視之更新之專案的專案名稱。  

1. 按一下 **儲存+關閉**.\
   所有具有至少「檢視專案」權限的使用者在專案上輸入的所有更新都會顯示在報表中。
