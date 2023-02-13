---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: 建立控制面板
description: 您可以建立控制面板，以快速存取報表、日曆和外部頁面中的資訊。
author: Nolan
feature: Reports and Dashboards
exl-id: 6a284df4-f011-4b4c-b44c-2e20918f643f
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# 建立控制面板

您可以建立控制面板，以快速存取報表、日曆和外部頁面中的資訊。

若要進一步了解控制面板，請參閱 [控制面板快速入門](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Adobe Workfront計畫*</strong></p> </td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td> <p><strong>Adobe Workfront授權*</strong></p> </td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td><strong>訪問級別配置*</strong> </td> 
   <td> <p>編輯對報表、控制面板和日曆的存取</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何變更您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>物件權限</strong> </p> </td> 
   <td> <p>您將取得新控制面板的管理權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.<br>如需控制面板權限的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md" class="MCXref xref">共用報表、控制面板和日曆 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 必要條件

您必須先建立下列任一對象，才能將其添加到控制面板：

* **報表**:如需建立報表的詳細資訊，請參閱 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* **日曆**:有關建立日曆的資訊，請參閱 [日曆報表概觀](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

* **外部頁面**:如需建立外部頁面的相關資訊，請參閱 [在控制面板中內嵌外部網頁](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

## 建立控制面板

1. 按一下「主菜單」表徵圖 ![](assets/main-menu-icon.png)，然後按一下 **控制面板。**
1. 按一下 **新控制面板**.\
   隨即顯示「新增控制面板」對話方塊。

1. 指定下列項目：

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>名稱</strong></td>
      <td><p>這是控制面板的名稱。</p><p>如果您未指定名稱，控制面板上第一個報表的名稱依預設會變成控制面板的名稱。</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>說明（可選）</strong></td>
      <td>這是控制面板的說明。</td>
     </tr>
    </tbody>
   </table>

1. 按一下與其對應的選項按鈕，以選取版面。

   預設為單欄配置。

   如需控制面板上報表配置的相關資訊，請參閱 [了解報表在控制面板上的顯示方式](../../../reports-and-dashboards/dashboards/understanding-dashboards/understand-how-reports-display-dashboard.md).

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: Consider adding the information from this article here, at some point, instead of linking to it.)
   </MadCap:conditionalText>
   -->

1. 在 **按名稱或類型搜索……** 欄位，然後將它們拖曳至「配置」窗格（當它們出現在清單中時）。

   >[!NOTE]
   >
   >搜尋項目時，搜尋會傳回最近建立的2,000個報表中的任何一個。 搜尋結果中不會傳回包含Unicode字元的報表名稱。 最佳作法是，在Workfront中透過輸入名稱來命名物件時，避免加入unicode字元，而非從其他來源複製並貼上名稱。

   ![搜尋報表](assets/qs-new-dashboard-ui-0722.png)

1. （選用）按一下 **新增外部頁面** 新增外部頁面至控制面板的方式。\
   如需建立外部頁面及將其嵌入控制面板的詳細資訊，請參閱 [在控制面板中內嵌外部網頁](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

1. 按一下 **儲存+關閉**.\
   時間戳記會顯示在控制面板的右上角。 時間戳記包含上次重新整理控制面板的日期、時間和時區。
