---
product-area: reporting
navigation-topic: report-usage
title: 檢視報表使用量
description: 檢視報表使用量
author: Nolan
feature: Reports and Dashboards
exl-id: 51d9067c-8c55-433e-b560-7da241ef33ae
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '997'
ht-degree: 0%

---

# 檢視報表使用量

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: : *** DO NOT CHANGE, REMOVE, CHANGE LINK, RENAME THIS ARTICLE- IT IS LINKED TO THE PENDO GUIDE FOR THE MAIN REPORTS AREA***)</p>
-->

若要了解在您的系統中如何廣泛使用報表，您可以在報表清單中檢視下列資訊：

* 前10個檢視報表的使用者
* 指定時間範圍內的檢視計數

   >[!NOTE]
   >
   >Adobe Workfront會計為每位使用者每天一次檢視。 如果您每天存取相同報表幾次，Workfront會將此報表計為該報表的單一檢視。 如果同一份報表由同一天的其他使用者存取，Workfront會將此計為第二個使用者的新檢視。

* 上一次檢視日期
* 使用者上次檢視次數
* 包含報表的控制面板清單\
   如需顯示控制面板名稱的詳細資訊，而控制面板的名稱可以新增至報表清單中，請參閱文章 [了解如何在控制面板上組織報表](../../../reports-and-dashboards/reports/report-usage/understand-how-organize-reports-dashboard.md).

您可以建立報表清單的檢視，以便顯示此資訊。\
您可以依這些欄位中的某些欄位來篩選報表清單。\
如需可依據篩選報表之欄位的詳細資訊，請參閱文章 [依使用資訊篩選報表清單](#filter-a-report-list-by-usage-information).

## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對報表、控制面板、日曆的存取</p> <p>編輯對篩選器、檢視、群組的存取</p> <p>注意：如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>管理報表權限</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 在報表清單的檢視中顯示報表使用情況資訊

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Workfront的右上角，然後按一下 **報表**.

1. 在報表清單上，按一下 **檢視** 下拉式功能表。
1. （選用）選取 **報表使用量** 檢視以顯示最常見的報表使用情形資訊。\
   或

1. 按一下 **新建視圖** 來建立自訂檢視。
1. 按一下 **添加列**.
1. 開始輸入下列任一欄位，並在欄位下方的清單中顯示時加以選取 **報表** 對象，將它們添加到新列：

   * **最近10位使用者**:顯示最近10個檢視報表的使用者的名稱。
   * **檢視**:顯示以下任意時間範圍內的視圖數：

      * **本月、本季、今年**
      * **上個月，季度，年**
      * **所有檢視**:顯示報表上所有檢視的整體計數
   * **上次檢視者**:顯示上次檢視報表的使用者的相關資訊
   * **上次檢視日期**:顯示上次檢視報表的日期


1. 按一下 **保存視圖**.\
   報表的使用資訊會顯示在您新增至檢視的欄中。\
   您也可以建立報表物件的報表，並在報表中使用此檢視。\
   如需建立報表的詳細資訊，請參閱文章 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).\
   您必須擁有存取層級中報表的編輯存取權，才能建立報表。\
   如需存取報表的詳細資訊，請參閱文章 [授予對報表、控制面板和日曆的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

## 依使用資訊篩選報表清單 {#filter-a-report-list-by-usage-information}

1. 按一下 **主菜單** 圖示 ![](assets/main-menu-icon.png) 在Workfront的右上角，然後按一下 **報表**.
1. 在報表清單上，按一下 **篩選** 下拉式功能表。
1. 按一下 **新增篩選**，然後按一下 **新增篩選規則**.
1. 開始輸入下列任一欄位，並在欄位下方的清單中顯示時加以選取 **報表** 物件，以新增為篩選規則：

   * **檢視**:顯示以下任意時間範圍內的視圖數：

      * **本月、本季、今年**
      * **上個月，季度，年**
      * **所有檢視**
   * **上次檢視者**:顯示上次檢視報表的使用者的相關資訊
   * **上次檢視日期**:顯示上次檢視報表的日期


1. 為欄位選取修改量，然後在出現提示時指定值。\
   ![](assets/qs-report-usage-filter-statistics-350x150.png)

1. 按一下 **儲存篩選**.\
   這會顯示符合您已定義之使用資訊的報表清單。\
   您也可以建立報表物件的報表，並在報表中使用此篩選器。\
   如需建立報表的詳細資訊，請參閱文章 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md). 您必須擁有存取層級中報表的編輯存取權，才能建立報表。\
   如需存取報表的詳細資訊，請參閱文章 [授予對報表、控制面板和日曆的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

## 檢視報表使用量資訊時的例外

>[!IMPORTANT]
>
>自2018年3月起，已收集報表使用資訊。 此日期之前的任何資訊都無法取得。

以下是使用報表使用量資訊時應注意的例外情況：

* 每次在控制面板或自訂標籤上顯示報表時，都會計為一個檢視。 在其控制面板上顯示該報表的使用者會顯示為上次檢視依據：為使用者命名，控制面板顯示的日期則顯示為上次檢視的日期。
* Workfront不會收集內建報表的使用資訊。\
   如需Workfront內建報表的詳細資訊，請參閱文章 [使用Adobe Workfront內建報表](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

* Workfront不會收集已傳送報表的使用情況資訊。 傳送的報表不會計為單一檢視。\
   如需已傳送報表的詳細資訊，請參閱文章 [報表傳送概觀](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

* 當系統或組管理員以其他用戶身份登錄時，系統或組管理員將計算這些視圖並與系統或組管理員關聯。
* Workfront不會依自訂季別收集報表的使用資訊。 在報表使用情況欄位中只引用標準內建季度。
* Workfront不會收集公開共用和檢視之報表的使用資訊。 未登入Workfront的使用者檢視公開報表時，不會計入報表檢視。\
   如需共用報表的詳細資訊，請參閱文章 [在Adobe Workfront中共用報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).
