---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '''報告：預算工時`'
description: '''報告：預算工時`'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2c0b60a6-fae4-4b29-8243-2a7f7d1f574b
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 1%

---

# 報告：預算工時

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: From&nbsp;Alina: This is my article, but since it's about building a report, it is in the Reporting section. Please don't remove it -it's linked to Resouce Management and it is super important.) </p>
-->

如果要與無權訪問資源計畫器的其他用戶共用預算工時資訊，您可以通過構建預算工時報表來執行此操作。 然後，您可以與他們共用報告。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This info is also added and drafted in the article "View Budget Hours in a report" in the Resource Planning section. Consider deleting this article?!)</p>
-->

>[!IMPORTANT]
>
>預算小時數在Adobe Workfront資料庫中每小時更新一次。 刷新報告不一定刷新報告中的工時資訊。 您可以查看自上次更新以來每個預算小時報表右上角的失效時間。 只有在上次更新後超過一小時時，刷新報表才會刷新報表中的資訊。
>
>![](assets/budgeted-hour-report-time-sync-warning-350x74.png)>

## 訪問要求

您必須具有以下訪問權限才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront許可證*</td> 
   <td> <p>計劃 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯對報表、儀表板、日曆的訪問</p> <p>編輯對篩選器、視圖、分組的訪問</p> <p><b>附註</b>

如果您仍然沒有訪問權限，請詢問您的Workfront管理員是否在您的訪問級別設定了其他限制。 有關Workfront管理員如何修改您的訪問級別的資訊，請參見 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自定義訪問級別</a>。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">對象權限</td> 
   <td> <p>管理對報表的權限</p> <p>有關請求附加訪問的資訊，請參見 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求訪問對象 </a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要瞭解您擁有的計畫、許可證類型或訪問權限，請與您的Workfront管理員聯繫。

## 生成預算工時報表

1. 按一下 **主菜單** ![](assets/main-menu-icon.png) 在右上角，按一下 **報告**。

1. 按一下 **新建報表>預算工時**。

   預設視圖將應用於報表。

1. （可選）要使報告更易於閱讀，請按一下 **預算小時數** 列 **切換到文本模式**，然後更改

   ```
   valuefield
   ```

   行

   ```
   valueexpreesion
   ```

   並輸入捨入表達式。

   這會將預算小時數捨入為指定的小數位數。

   有關如何在Workfront對數字進行捨入的資訊，請參閱文章 [計算的資料表達式](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md)。

1. （可選）按一下 **添加列** 的子菜單。
1. （可選）為了使報告更易於閱讀，建議您向其中添加分組。 我們建議進行以下分組：

   按一下 **分組** 頁籤，然後執行下列一項或多項操作：

   1. 按一下 **添加分組** 然後開始鍵入「項目名稱」，然後在清單中顯示時選擇它。
   1. 按一下 **添加分組** 然後開始鍵入「作業角色名稱」，然後在清單中顯示時選擇它。
   1. 按一下 **添加分組** 開始鍵入 **分配日期**，在清單中出現時選擇它，然後從 **分組日期** 的子菜單。

1. （可選）按一下 **篩選器** 來修改選定線條的屬性。
1. （可選）按一下 **圖表** 的子菜單。
1. 按一下 **保存+關閉**。

## 複查預算工時報表

預設情況下，「預算工時」報表中提供了以下資訊：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">專案 </td> 
   <td>這是與預算工時關聯的項目名稱。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>作業角色</p> </td> 
   <td>這是與預算工時關聯的作業角色的名稱。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">使用者</td> 
   <td>這是與預算工時關聯的用戶的名稱。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">分配日期</td> 
   <td> <p>這是分配日期。 這是您預算小時數的一週的第一天（星期日）。</p> <p>提示：  <p>如果一週跨度為兩個月，則會在報表中生成兩行：一個對應於周的第一天（周的星期日，該周在第一個月），另一個對應於第二個月的第一天（可能是周的任何一天）。</p> <p>例如，如果您為用戶預算6月30日（星期日） — 7月6日（星期六）這一週的8小時，這兩行將顯示6月30日和7月1日的分配日期。</p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">預算小時</td> 
   <td>這些是分配給資源計畫器中用戶的預算小時數。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">波蘭茲羅提。 預算小時</td> 
   <td>這些是分配給資源計畫器中任務職責或項目的預算小時數。</td> 
  </tr> 
 </tbody> 
</table>
