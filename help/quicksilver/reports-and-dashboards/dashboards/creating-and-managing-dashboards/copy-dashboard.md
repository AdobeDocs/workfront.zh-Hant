---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: 複製控制面板
description: 您可以複製控制面板及其所有內容（報表、日曆和外部頁面）。 複製控制面板的內容時，您可以選擇將其保留在原始控制面板上的顯示狀態，或建立新項目，這些項目是原始控制面板上這些內容的副本。 您也可以選擇不轉移或複製新控制面板上的項目。
author: Nolan
feature: Reports and Dashboards
exl-id: a88cc171-2bb1-40f0-a778-8dac7eecb718
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 0%

---

# 複製控制面板

您可以複製控制面板及其所有內容（報表、日曆和外部頁面）。 複製控制面板的內容時，您可以選擇將其保留在原始控制面板上的顯示狀態，或建立新項目，這些項目是原始控制面板上這些內容的副本。 您也可以選擇不轉移或複製新控制面板上的項目。

## 存取需求

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
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>訪問級別配置*</strong></td> 
   <td> <p>編輯對報表、控制面板和日曆的存取</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件權限</strong></td> 
   <td> <p>檢視控制面板的存取權</p> <p>您將取得複製控制面板的「管理」存取權</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 必要條件

您必須先建立控制面板，才能加以複製。

如需建立控制面板的詳細資訊，請參閱 [建立控制面板](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## 複製控制面板

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png)，然後按一下 **控制面板**.

1. 選取您要複製的控制面板，然後按一下 **複製** ![](assets/copy-icon.png).\
   或\
   開啟您要複製的控制面板，然後按一下 **控制面板動作** > **複製**.\
   「控制面板複製」對話框隨即顯示。 原始控制面板上的所有項目都會顯示。

1. 在 **控制面板名稱** 欄位中指定控制面板的新名稱。
1. 若要選取現有控制面板上的所有項目，並將其複製至複製的控制面板，請保留 **全選** 已選取。 依預設，現有控制面板上的報表、日曆或清單將會複製到新控制面板。\
   或\
   若要僅將特定項目從原始控制面板轉移到新控制面板，請取消選取您不想在新控制面板上顯示的項目，然後針對每個選取的項目，從下列選項中選擇：

   * **製作副本：** 項目會從原始控制面板複製，而新控制面板上會顯示該項目的新版本。 對新控制面板上的項目所做的變更不會反映在原始控制面板上的項目中。 同樣地，對原始控制面板上的項目所做的變更不會反映在新控制面板上的項目中。\
      當您要修改原始控制面板上的原始報表時，請使用此選項。\
      例如，您複製名為「團隊B」的控制面板，然後將其重新命名為「團隊A」。 在「團隊B」控制面板上，有一個名為「團隊B報表」的報表。 由於此報告包含B組的特定資料，因此您選擇製作此報告副本的選項，以便您可以為A組自定義該報告，並稍後將其更名為「A組報告」。\
      使用此選項，您可從複製的報表中移除原始報表的共用權限。 具有資訊存取權限的執行此報表在複製的報表上保持不變。

   * **使用原始：** 在新控制面板上顯示原始項目。 對新控制面板上的項目所做的變更也會反映在原始控制面板上的項目中。 同樣地，對原始控制面板上的項目所做的更改也會反映在新控制面板上的項目中。\
      使用此選項，可保留原始報表的共用權限。 具有資訊存取權限的執行此報表也保持不變。

1. （選用）重新命名您選取的任何項目。
1. 按一下 **複製控制面板**.
1. （可選）如果要編輯複製的控制面板上任何複製的報表、日曆、外部頁面，請執行下列任一操作：

   * 若要編輯任何複製報表的任何資訊，請按一下控制面板上的報表名稱，然後 **報表動作** > **編輯**.

      例如，您可能想要編輯「檢視」、「篩選」、「分組」、「提示」或「圖表」或複製的報表。

   * 若要重建複製報表的權限，請按一下新控制面板中的報表名稱，然後按一下 **報表動作** > **共用** 和更新報表的權限。

      複製控制面板時複製報表時，會移除該報表的權限。

   * 若要修改「使用資訊的存取權限執行此報表」 ，請按一下新控制面板上的報表名稱，然後 **報表動作** > **編輯** > **報表選項**.\
      複製報表後，只有在下列情況下才會維護「使用權限執行此報表」 :

      （如果上述條件均不成立，則會移除「使用權限執行此報表」 ，並將新的「使用存取權限執行此報表」變更為建立複製報表的使用者。）

      如果複製控制面板及其報表的使用者具有管理員存取權限。

      * 如果複製控制面板及其報表的使用者具有管理員存取權限。
      * 如果複製控制面板的使用者及其報表目前設定為執行此報表，且其存取權限為要複製之報表的。
      * 如果複製報表的使用者具有報表的管理權限。
