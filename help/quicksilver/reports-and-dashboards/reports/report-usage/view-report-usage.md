---
product-area: reporting
navigation-topic: report-usage
title: 檢視報表使用情形
description: 檢視報表使用情形
author: Nolan
feature: Reports and Dashboards
exl-id: 51d9067c-8c55-433e-b560-7da241ef33ae
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '1011'
ht-degree: 1%

---

# 檢視報表使用情形

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: : *** DO NOT CHANGE, REMOVE, CHANGE LINK, RENAME THIS ARTICLE- IT IS LINKED TO THE PENDO GUIDE FOR THE MAIN REPORTS AREA***)</p>
-->

若要瞭解系統中已廣泛使用報表的程度，您可以在報表清單中檢視下列資訊：

* 前10名檢視報告的使用者
* 在指定的時間範圍內檢視計數

  >[!NOTE]
  >
  >Adobe Workfront每天計算每個使用者一個檢視次數。 如果您一天存取相同報表幾次，Workfront會將此計為報表的一個檢視。 如果同一天有其他使用者存取相同的報表，Workfront會將此計為第二個使用者的新檢視。

* 上一次檢視日期
* 使用者上次檢視的專案
* 包含報告的控制面板清單\
  如需有關顯示可能在報告清單中新增報告的報告之報告面板名稱的詳細資訊，請參閱文章[瞭解如何在報告面板上組織報告](../../../reports-and-dashboards/reports/report-usage/understand-how-organize-reports-dashboard.md)。

您可以建立報表清單的檢視，以便顯示這項資訊。\
您可以依這些欄位中的部分來篩選報表清單。\
如需您可以依哪些欄位篩選報告的詳細資訊，請參閱文章[依使用情況資訊篩選報告清單](#filter-a-report-list-by-usage-information)。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

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
   <td> <p>規劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權</p> <p>編輯對篩選器、檢視、群組的存取權</p> <p>注意：如果您還是沒有存取權，請詢問您的Workfront管理員，他們是否在您的存取層級中設定其他限制。 如需Workfront管理員如何修改存取層級的詳細資訊，請參閱<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p> <p>如需請求其他存取權的資訊，請參閱<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求物件</a>的存取權。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的Workfront管理員。

## 在報告清單的檢視中顯示報告使用情況資訊

1. 按一下Workfront右上角的&#x200B;**主功能表**&#x200B;圖示![主功能表圖示](assets/main-menu-icon.png)，然後按一下&#x200B;**報表**。

1. 在報表清單中，按一下&#x200B;**檢視**&#x200B;下拉式功能表。
1. （選擇性）選取&#x200B;**報告使用量**&#x200B;檢視以顯示最常用的報告使用量資訊。\
   或

1. 按一下&#x200B;**新增檢視**&#x200B;以建立自訂檢視。
1. 按一下「**新增欄**」。
1. 開始輸入下列任何欄位，並在這些欄位出現在&#x200B;**Report**&#x200B;物件下的清單中時加以選取，以將它們新增至新欄：

   * **前10位使用者**：顯示檢視過報告的前10位使用者名稱。
   * **檢視次數**：顯示下列任一時間範圍內的檢視次數：

      * **本月、季、年**
      * **上個月、季、年**
      * **所有檢視**：顯示報告上所有檢視的總計數

   * **上次檢視者**：顯示上次檢視報表之使用者的相關資訊
   * **上次檢視日期**：顯示上次檢視報告的日期

1. 按一下「**儲存視圖**」。\
   報表的使用情況資訊會顯示在您新增至檢視的欄中。\
   您也可以為報表物件建立報表，並在報表中使用此檢視。\
   如需有關建立報告的詳細資訊，請參閱文章[建立自訂報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。\
   您必須擁有存取層級中報表的編輯存取權，才能建置報表。\
   如需有關存取報告的詳細資訊，請參閱文章[授予報告、儀表板和行事曆的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)。

## 依使用情況資訊篩選報表清單 {#filter-a-report-list-by-usage-information}

1. 按一下Workfront右上角的&#x200B;**主功能表**&#x200B;圖示![主功能表圖示](assets/main-menu-icon.png)，然後按一下&#x200B;**報表**。
1. 在報表清單中，按一下&#x200B;**篩選器**&#x200B;下拉式功能表。
1. 按一下&#x200B;**新增篩選器**，然後按一下&#x200B;**新增篩選器規則**。
1. 開始輸入下列任何欄位，並在這些欄位出現在&#x200B;**Report**&#x200B;物件下的清單中時選取它們，以將它們新增為新的篩選規則：

   * **檢視次數**：顯示下列任一時間範圍內的檢視次數：

      * **本月、季、年**
      * **上個月、季、年**
      * **所有檢視**

   * **上次檢視者**：顯示上次檢視報表之使用者的相關資訊
   * **上次檢視日期**：顯示上次檢視報告的日期

1. 為您的欄位選取修飾元，然後在提示時指定值。\
   ![報告使用情況篩選器統計資料](assets/qs-report-usage-filter-statistics-350x150.png)

1. 按一下「**儲存篩選器**」。\
   這會顯示符合您定義之使用資訊的報告清單。\
   您也可以為報表物件建立報表，並在報表中使用此篩選器。\
   如需有關建立報告的詳細資訊，請參閱文章[建立自訂報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。 您必須擁有存取層級中報表的編輯存取權，才能建置報表。\
   如需有關存取報告的詳細資訊，請參閱文章[授予報告、儀表板和行事曆的存取權](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)。

## 檢視報表使用量資訊時發生例外

>[!IMPORTANT]
>
>自2018年3月起已收集報表使用資訊。 在此日期之前的任何資訊都無法使用。

使用報表使用情況資訊時，應注意下列一些例外情況：

* 每次在儀表板或自訂標籤上顯示報告時，都會計為一個檢視。 在儀表板上顯示該報表的使用者會顯示為「最後檢視者：姓名」使用者，而顯示儀表板的日期會顯示為「最後檢視日期」。
* Workfront不會收集內建報表的使用資訊。\
  如需Workfront內建報表的詳細資訊，請參閱文章[使用Adobe Workfront內建報表](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md)。

* Workfront不會收集已傳送報表的使用資訊。 已傳遞的報表不計為單一檢視。\
  如需已傳送報表的詳細資訊，請參閱文章[報表傳送概觀](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)。

* 當系統或群組管理員以其他使用者身份登入時，這些檢視會被計入系統或群組管理員並與之相關聯。
* Workfront不會依自訂季度收集報表的使用資訊。 報告使用情況欄位中僅會參考標準內建季度。
* Workfront不會收集已共用和公開檢視之報表的使用資訊。 當使用者未登入Workfront即檢視公開報表時，系統不會計算報表檢視次數。\
  如需共用報表的詳細資訊，請參閱文章[在Adobe Workfront中共用報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)。
