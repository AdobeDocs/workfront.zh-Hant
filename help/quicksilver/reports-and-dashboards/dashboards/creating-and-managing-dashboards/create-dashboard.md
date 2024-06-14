---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: 建立儀表板
description: 您可以建立控制面板，以快速存取Adobe Workfront中的資訊。 您可以將報告、行事曆和外部頁面新增到控制面板，與他人共用以進行最佳共同作業。
author: Nolan
feature: Reports and Dashboards
exl-id: 6a284df4-f011-4b4c-b44c-2e20918f643f
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 1%

---

# 建立儀表板

<!--Audited: 01/2024-->

您可以建立控制面板，以快速存取Adobe Workfront中的資訊。 您可以將報告、行事曆和外部頁面新增到控制面板，與他人共用以進行最佳共同作業。

若要深入瞭解儀表板，請參閱 [開始使用儀表板](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

您必須具備下列條件：

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Adobe Workfront計畫</strong></p> </td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td> <p><strong>Adobe Workfront授權*</strong></p> </td> 
   <td> <p>目前：計畫 </p>
   或
   <p>新增：標準 </p> </td> 
  </tr> 
  <tr> 
   <td><strong>存取層級設定</strong> </td> 
   <td> <p>編輯報告、儀表板和行事曆的存取權</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>物件許可權</strong> </p> </td> 
   <td> <p>您將取得您建立之控制面板的管理許可權</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。 如需詳細資訊，請參閱 [Workfront檔案中的存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## 先決條件

您必須先建立下列任何物件，才能將其新增到儀表板：

* **報表**：如需建立報表的詳細資訊，請參閱 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* **行事曆**：如需建立行事曆的相關資訊，請參閱 [行事曆報表總覽](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

您可以將現有的外部頁面新增到儀表板，也可以從新儀表板建立外部頁面。 如需建立外部頁面的詳細資訊，請參閱 [將外部網頁內嵌在控制面板中](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

## 建立儀表板

{{step1-to-dashboards}}

1. 按一下 **新儀表板**.\
   「新儀表板」對話方塊隨即顯示。

1. 指定下列專案：

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>姓名</strong></td>
      <td><p>這是您控制面板的名稱。</p><p>如果您未指定名稱，則預設情況下，圖示板上第一個報表的名稱會變成圖示板的名稱。</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>說明（選擇性）</strong></td>
      <td>這是您控制面板的說明。</td>
     </tr>
    </tbody>
   </table>

1. 按一下頂端與版面配置對應的圓鈕，以選取版面配置。 **選擇佈局/新增報告/新增行事曆** 區段。 這是報告、行事曆或外部頁面將顯示在控制面板上的版面配置。

   預設為單欄版面配置。

   如需關於儀表板報告配置的資訊，請參閱 [瞭解報表在儀表板上的顯示方式](../../../reports-and-dashboards/dashboards/understanding-dashboards/understand-how-reports-display-dashboard.md).

   <!--
   Consider adding the information from this article above here, at some point, instead of linking to it.)
   -->

1. 搜尋中的報告、行事曆或外部頁面 **依名稱或型別搜尋……** 欄位，然後將它們拖曳至配置窗格（當它們出現在清單中時）。

   >[!NOTE]
   >
   >搜尋專案時，搜尋會傳回最近建立的2,000份報表中的任一份。 搜尋結果不會傳回包含Unicode字元的報表名稱。 最佳做法是，在Workfront中透過輸入名稱來命名物件時，避免包括Unicode字元，而不是從其他來源複製和貼上名稱。

   ![搜尋報表](assets/qs-new-dashboard-ui-0722.png)

1. （選用）按一下 **新增外部頁面** 將新的外部頁面新增到儀表板。

   如需建立外部頁面並將其嵌入控制面板的詳細資訊，請參閱 [將外部網頁內嵌在控制面板中](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

1. 按一下「**儲存並關閉**」。

   時間戳記會顯示在控制面板的右上角。 時間戳記包含上次重新整理控制面板的日期、時間和時區。
