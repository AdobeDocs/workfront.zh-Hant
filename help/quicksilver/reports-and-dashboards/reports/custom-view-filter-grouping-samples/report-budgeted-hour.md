---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '''報告：預算小時數'
description: '''報告：預算小時數'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2c0b60a6-fae4-4b29-8243-2a7f7d1f574b
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 1%

---

# 報告：預算小時數

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: From&nbsp;Alina: This is my article, but since it's about building a report, it is in the Reporting section. Please don't remove it -it's linked to Resouce Management and it is super important.) </p>
-->

如果要與無權訪問資源計畫員的其他用戶共用預算小時資訊，則可以通過建立預算小時報表來共用。 接著，您便可與他們共用報表。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This info is also added and drafted in the article "View Budget Hours in a report" in the Resource Planning section. Consider deleting this article?!)</p>
-->

>[!IMPORTANT]
>
>預算小時數在Adobe Workfront資料庫中每小時更新一次。 重新整理報表不一定會重新整理報表中的小時資訊。 您可以在每個「預算小時」報表的右上角，檢視上次更新後經過的時間。 重新整理報表只會在自上次更新後超過一小時時，才會重新整理報表中的資訊。
>
>![](assets/budgeted-hour-report-time-sync-warning-350x74.png)>

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

## 建立預算小時報表

1. 按一下 **主菜單** ![](assets/main-menu-icon.png) 在右上角，按一下 **報表**.

1. 按一下 **新增報表>預算小時數**.

   預設檢視會套用至報表。

1. （選用）若要讓報表更容易閱讀，請按一下 **預算小時數** 欄，然後 **切換到文本模式**，然後變更

   ```
   valuefield
   ```

   折線圖

   ```
   valueexpreesion
   ```

   並輸入捨入表達式。

   這會將預算小時數捨入為您指定的小數位數。

   如需如何在Workfront中捨入數字的詳細資訊，請參閱文章 [計算資料運算式](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

1. （選用）按一下 **添加列** 以新增其他欄。
1. （選用）為了讓報表更容易閱讀，建議您新增群組至報表。 建議以下群組：

   按一下 **分組** ，然後執行下列一或多個操作：

   1. 按一下 **添加分組** 然後開始鍵入「項目名稱」，然後在清單中出現時選擇它。
   1. 按一下 **添加分組** 然後開始鍵入「作業角色名稱」，然後在清單中出現時選擇它。
   1. 按一下 **添加分組** 開始輸入 **分配日期**，在清單中顯示時選取，然後從 **分組日期依據** 欄位。

1. （選用）按一下 **篩選器** 新增篩選器至報表。
1. （選用）按一下 **圖表** 新增圖表至報表。
1. 按一下 **儲存+關閉**.

## 複查「預算小時」報表

預設情況下，「預算小時」報表中提供下列資訊：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">專案 </td> 
   <td>這是與預算小時數關聯的項目的名稱。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>工作角色</p> </td> 
   <td>這是與「預算小時」關聯的作業角色的名稱。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">使用者</td> 
   <td>這是與預算小時關聯的用戶的名稱。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">分配日期</td> 
   <td> <p>這是分配日期。 這是您為該小時編列預算的一週的第一天（星期日）。</p> <p>提示：  <p>如果一週跨越兩個月，這會在報表中產生兩列：一個對應於一週的第一天（一週的星期日，在第一個月），另一個對應於第二個月的第一天（可能是一週中的任何一天）。</p> <p>例如，若您為某位使用者在6月30日（星期日） — 7月6日（星期六）這一週預算8小時，則兩列會顯示分配日期： 6月30日和7月1日。</p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">預算小時</td> 
   <td>這些是分配給資源計畫員中用戶的預算小時數。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">波蘭。 預算小時</td> 
   <td>這些是分配給資源計畫員中任務職責或項目的預算小時數。</td> 
  </tr> 
 </tbody> 
</table>
