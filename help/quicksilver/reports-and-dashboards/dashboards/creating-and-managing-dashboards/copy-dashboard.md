---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: 複製控制面板
description: 您可以複製控制面板及其所有內容（報告、行事曆和外部頁面）。 當您複製儀表板內容時，您可以選擇保留它們在原始儀表板上的顯示方式，或者建立新專案，這些專案是原始儀表板上的副本。 您也可以選擇不轉移或複製新儀表板上的專案。
author: Nolan
feature: Reports and Dashboards
exl-id: a88cc171-2bb1-40f0-a778-8dac7eecb718
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '898'
ht-degree: 0%

---

# 複製控制面板

<!-- Audited: 1/2025 -->

您可以複製控制面板及其所有內容（報告、行事曆和外部頁面）。 當您複製儀表板內容時，您可以選擇保留它們在原始儀表板上的顯示方式，或者建立新專案，這些專案是原始儀表板上的副本。 您也可以選擇不轉移或複製新儀表板上的專案。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront計畫*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront授權*</strong></td> 
    <td> 
      <p>新增：</p>
         <ul>
         <li><p>標準</p></li>
         </ul>
      <p>目前：</p>
         <ul>
         <li><p>規劃</p></li>
         </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>存取層級設定*</strong></td> 
   <td> <p>編輯報告、儀表板和行事曆的存取權</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件許可權</strong></td> 
   <td> <p>檢視控制面板的存取權</p> <p>您將取得複製之控制面板的管理存取權</p></td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

您必須先建立儀表板，才能進行複製。

如需有關建立儀表板的資訊，請參閱[建立儀表板](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md)。

## 複製控制面板

1. 按一下Adobe Workfront右上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon.png)，或（如果有的話）按一下左上角的&#x200B;**[!UICONTROL 主功能表]**&#x200B;圖示![主功能表](/help/_includes/assets/main-menu-icon-left-nav.png)，然後按一下&#x200B;**[!UICONTROL 儀表板]**。

1. 選取您要複製的儀表板，然後按一下&#x200B;**複製** ![復製圖示](assets/copy-icon.png)。\
   或\
   開啟您要複製的儀表板，然後按一下&#x200B;**儀表板動作** > **複製**。\
   「儀表板複製」對話方塊隨即顯示。 原始儀表板上的所有專案都會顯示。

1. 在&#x200B;**儀表板名稱**&#x200B;欄位中，指定儀表板的新名稱。
1. 若要選取現有儀表板上的所有專案，並將它們複製到複製的儀表板，請保留&#x200B;**全部選取**。 依預設，現有儀表板上的報告、行事曆或清單將會複製到新儀表板。\
   或\
   若要僅將特定專案從原始控制面板轉移到新控制面板，請取消選取您不想出現在新控制面板上的專案，然後針對每個選取的專案，從下列選項中選擇：

   * **製作復本：**&#x200B;該專案是從原始儀表板複製而來，且新儀表板會顯示該專案的新版本。 對新儀表板上的專案所做的變更不會反映在原始儀表板的專案中。 同樣地，對原始儀表板上的專案所做的變更也不會反映在新儀表板上的專案中。\
     當您想要修改原始儀表板上的原始報告時，請使用此選項。\
     例如，您複製名為「團隊B」的控制面板，然後將其重新命名為「團隊A」。 「團隊B」控制面板上有一個名為「團隊B報告」的報告。 由於此報表包含專屬於團隊B的資料，因此您選取製作此報表副本的選項，這樣您便可以為團隊A自訂報表，並在稍後將其重新命名為「團隊A報表」。\
     使用此選項，您就可以從複製的報表中移除原始報表的共用許可權。 使用資訊存取權執行此報告在複製的報告上維持不變。

   * **使用原始專案：**&#x200B;在新儀表板上顯示原始專案。 對新儀表板上的專案所做的變更也會反映在原始儀表板的專案中。 同樣地，對原始圖示板上的專案所做的變更會反映在新圖示板上的專案中。\
     使用此選項，您可以保留原始報告的共用許可權。 以資訊的存取許可權執行此報告也保持不變。

1. （選擇性）重新命名選取的任何專案。
1. 按一下&#x200B;**複製儀表板**。
1. （選擇性）如果您想要編輯已複製控制面板上的任何已複製報表、行事曆和外部頁面，請執行下列任一項作業：

   * 若要編輯任何已複製報表的任何資訊，請按一下控制面板上的報表名稱，然後按一下&#x200B;**報表動作** > **編輯**。

     例如，您可能想要編輯檢視、篩選、分組、提示或圖表或複製的報告。

   * 若要恢復所複製報告的許可權，請按一下新儀表板中的報告名稱，然後按一下[報告動作] **> [共用]** **並更新報告的許可權。**

     當您在複製控制面板時複製報告，會移除該報告上的許可權。

   * 若要修改「使用資訊存取權執行此報告」，請在新儀表板上按一下報告名稱，然後按&#x200B;**報告動作** > **編輯** > **報告選項**。\
     複製報表後，只有在下列情況下才會維持使用許可權的存取許可權執行此報表：

     （如果這些條件都不成立，則使用許可權的存取許可權執行此報告會遭到移除，而使用存取許可權的新執行此報告會變更為建立所複製報告的使用者。）

     如果複製控制面板及其報表的使用者擁有管理員存取許可權。

      * 如果複製控制面板及其報表的使用者擁有管理員存取許可權。
      * 如果複製控制面板及其報表的使用者目前被設定為執行此報表，並具有所複製報表的存取權。
      * 如果複製報表的使用者擁有報表的管理許可權。
