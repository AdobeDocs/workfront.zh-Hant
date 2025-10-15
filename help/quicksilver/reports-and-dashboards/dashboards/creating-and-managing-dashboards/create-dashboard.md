---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: 建立儀表板
description: 您可以建立控制面板，以快速存取Adobe Workfront中的資訊。 您可以將報告、行事曆和外部頁面新增到控制面板，與他人共用以進行最佳共同作業。
author: Nolan
feature: Reports and Dashboards
exl-id: 6a284df4-f011-4b4c-b44c-2e20918f643f
source-git-commit: c8b7ad473b0c2120ef5ea52374b3501ad6f553f1
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 1%

---

# 建立儀表板

<!--Audited: 01/2025-->

您可以建立控制面板，以快速存取Adobe Workfront中的資訊。 儀表板最多可以新增25個報告、行事曆和外部頁面，您可與其他人共用這些儀表板以獲得最佳共同作業。

若要深入瞭解儀表板，請參閱[開始使用儀表板](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> 
      <p>標準</p>
      <p>規劃</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯報告、儀表板和行事曆的存取權</p></td> 
  </tr>  
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>您將取得您建立之控制面板的管理許可權</p> </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

您必須先建立下列任何物件，才能將其新增到儀表板：

* **報告**：如需建立報告的詳細資訊，請參閱[建立自訂報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

* **行事曆**：如需建立行事曆的相關資訊，請參閱[行事曆報告總覽](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md)。

您可以將現有的外部頁面新增到儀表板，也可以從新儀表板建立外部頁面。 如需建立外部頁面的詳細資訊，請參閱[將外部網頁內嵌在儀表板中](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md)。

## 建立儀表板

{{step1-to-dashboards}}

1. 按一下&#x200B;**新儀表板**。\
   「新儀表板」對話方塊隨即顯示。

1. 指定下列專案：

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>姓名</strong></td>
      <td><p>這是您控制面板的名稱。 我們建議僅使用UTF-8字元以避免相容性問題。</p><p>如果您未指定名稱，則預設情況下，圖示板上第一個報表的名稱會變成圖示板的名稱。</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>說明 (選擇性)</strong></td>
      <td>這是您控制面板的說明。</td>
     </tr>
    </tbody>
   </table>

1. 在&#x200B;**選取配置/新增報告/新增行事曆**&#x200B;區段頂端按一下與其對應的圓鈕，以選取配置。 這是報告、行事曆或外部頁面將顯示在控制面板上的版面配置。

   預設為單欄版面配置。

   如需儀表板上的報告配置相關資訊，請參閱[瞭解報告在儀表板上的顯示方式](../../../reports-and-dashboards/dashboards/understanding-dashboards/understand-how-reports-display-dashboard.md)。

   <!--
   Consider adding the information from this article above here, at some point, instead of linking to it.)
   -->

1. 在&#x200B;**可用的報表和行事曆**&#x200B;區段中，開始在搜尋列中鍵入報表、行事曆或外部頁面的名稱，然後將報表、行事曆或外部頁面在版面配置窗格中拖放到右側。

   >[!NOTE]
   >
   >搜尋專案時，搜尋會傳回最近建立的2,000份報表中的任一份。 搜尋結果不會傳回包含Unicode字元的報表名稱。 最佳做法是，在Workfront中透過輸入名稱來命名物件時，避免包括Unicode字元，而不是從其他來源複製和貼上名稱。

   ![搜尋報告](assets/unshimmed-dashboard-ui.png)

1. （選擇性）按一下&#x200B;**新增外部頁面**，以新增外部頁面至儀表板。

   如需建立外部頁面並將其內嵌到控制面板的詳細資訊，請參閱[在控制面板中內嵌外部網頁](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md)。

1. 按一下「**儲存並關閉**」。

   時間戳記會顯示在控制面板的右上角。 時間戳記包含上次重新整理控制面板的日期、時間和時區。
