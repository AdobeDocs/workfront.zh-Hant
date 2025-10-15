---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 報告：預算時數
description: 報告：預算時數
author: Nolan
feature: Reports and Dashboards
exl-id: 2c0b60a6-fae4-4b29-8243-2a7f7d1f574b
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '656'
ht-degree: 1%

---

# 報告：預算時數

<!--Audited: 10/2024-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: From&nbsp;Alina: This is my article, but since it's about building a report, it is in the Reporting section. Please don't remove it -it's linked to Resource Management and it is super important.) </p>
-->

當您想要與無法存取資源規劃工具的其他使用者共用預算時數資訊時，您可以透過建立預算時數報表來執行此操作。 接著，您就可以與他們共用報表。

>[!IMPORTANT]
>
>預算時數通常每小時在Adobe Workfront資料庫中更新一次（少數情況下，最多可能需要三個小時）。 重新整理報告不一定會重新整理報告中的小時資訊。 您可以在每個預算時數報表的右上角，檢視自上次更新以來的經過時間。 重新整理報告只會在上次更新後超過一小時時重新整理其中的資訊。
>
>![預算時數報告時間同步警告](assets/budgeted-hour-report-time-sync-warning-350x74.png)

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
   <p>修改篩選器的貢獻者或請求 </p>
   <p>要修改報告的標準或計畫</p>
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯篩選器、檢視和群組的存取權以修改篩選器</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p>  </td> 
  </tr> 
 </tbody> 
</table>

如需有關此表格的詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 建立預算時數報告

1. 按一下右上角的&#x200B;**主功能表**&#x200B;圖示![主功能表圖示](assets/main-menu-icon.png)，或左上角的&#x200B;**主功能表**&#x200B;圖示![主功能表行](assets/lines-main-menu.png) （如果有的話），然後按一下&#x200B;**報表**。

1. 按一下「**新報告**」>「**更多**」>「**預算時數**」。

   預設檢視會套用至報表。

1. （選擇性）若要讓報表更易於閱讀，請按一下&#x200B;**Bud。 小時**&#x200B;欄，然後&#x200B;**切換到文字模式**，然後按一下&#x200B;**編輯文字模式**。
1. 將`valuefield`行變更為`valueexpreesion`並輸入舍入運算式。

   這會將預算時數四捨五入為您指定的小數。

   如需有關如何在Workfront中舍入數字的資訊，請參閱文章[計算資料運算式概觀](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md)。

1. 按一下「**完成**」。
1. （選擇性）按一下&#x200B;**新增欄**&#x200B;以新增其他欄。
1. （選用）若要讓報表更易於閱讀，建議您將分組新增至報表。 我們建議進行下列分組：

   按一下&#x200B;**群組**&#x200B;標籤，然後執行下列一或數個動作：

   * 按一下&#x200B;**新增群組**&#x200B;並開始輸入「專案名稱」，然後當它出現在清單中時選取它。
   * 按一下&#x200B;**新增群組**&#x200B;並開始輸入「工作角色名稱」，然後當它出現在清單中時選取它。
   * 按一下&#x200B;**新增群組**&#x200B;並開始輸入「分配日期」，當它出現在清單中時選取它，然後從&#x200B;**依**&#x200B;的群組日期欄位中選取您要依其進行群組的時間範圍。

1. （選擇性）按一下&#x200B;**篩選器**&#x200B;以將篩選器新增至報表。
1. （選擇性）按一下&#x200B;**圖表**&#x200B;將圖表新增至報表。
1. 按一下「**儲存並關閉**」。

## 檢閱預算時數報告

下列資訊可於預算時數報表中依預設取得：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">專案 </td> 
   <td>這是與預算時數相關聯的專案名稱。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>工作角色</p> </td> 
   <td>這是與預算時數相關聯的工作角色名稱。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">使用者</td> 
   <td>這是與預算時數相關聯的使用者名稱。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">分配日期</td> 
   <td> <p>這是配置日期。 這是您編列時數預算的一週的第一天（星期日）。</p> <p>秘訣：  <p>如果一週跨越兩個月，這會在報表中產生兩列：一個對應一週的第一天（第一個月內為一週的星期日），第二個對應第二個月的第一天（可能是一週的任何一天）。</p> <p>例如，如果您為使用者編列了6月30日（星期日） - 7月6日（星期六）這週的8小時預算，則兩列會顯示分配日期6月30日和7月1日。</p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">預算小時</td> 
   <td>這些是分配給資源規劃工具中使用者的預算時數。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">計畫 預算小時</td> 
   <td>這些是分配至資源規劃工具中工作角色或專案的預算時數。</td> 
  </tr> 
 </tbody> 
</table>
