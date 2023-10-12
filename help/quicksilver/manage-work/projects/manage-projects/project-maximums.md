---
title: 專案限制總覽
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: Adobe Workfront對可與專案相關聯的物件數量有限制。 設定專案限制是為了改善產品效能並增強您對Workfront的體驗。
author: Alina
feature: Work Management
exl-id: 60576107-89f1-4328-89e2-5b1e5e243fd9
source-git-commit: 8be7534dfc0a1227bd2274ad093a88ae19b4691d
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---

# 專案限制總覽

Adobe Workfront對可與專案相關聯的物件數量有限制。 設定專案限制是為了改善產品效能並增強您對Workfront的體驗。

下列與專案關聯的物件具有下列限制：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>任務</p></td> 
   <td>  <p>每個專案的最大任務數量為5,000。 當任務數量接近此上限時，系統會顯示警告訊息。 當達到最大時，會顯示錯誤訊息，並且無法將其他任務新增到專案。</p> <p>為避免達到此上限，請將已關閉的任務移動到指定給已關閉任務的另一個專案。 這些專案的報告可能需要調整。</p>

<b>重要</b>

對於任務有許多相依性的專案，計算時間表或在專案中工作時，可能會發生效能降低。

因此，我們建議相依性複雜的專案中的任務數量應遠低於允許的5,000個任務的上限。

可能會影響或阻止重新計算專案時間表的一些任務相依性範例包括：

<ul><li>子項數目</li>
   <li>多個層級的任務縮排</li>
   <li>前置任務數量</li>
   <li>多個指派</li>
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>問題</p></td> 
   <td>  <p>每個專案的問題數量上限為10,000。 當問題數量接近此上限時，系統會顯示警告訊息。 當達到最大時，會顯示錯誤訊息，並且無法將其他問題新增到專案。</p> <p>為避免達到此上限，請將已關閉的問題移動到針對已關閉問題指定的另一個專案。 這些專案的報告可能需要調整。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>持續時間</p></td> 
   <td> <p>專案的最大期間必須為15年，Workfront才能自動計算其時間表。 當專案持續時間接近最大值時會顯示警告訊息。 當達到最大值時，會顯示警告訊息，且不再進行自動時間表計算。</p> <p>一旦專案期間減少到15年以下，就會透過調整專案中任務的日期來恢復自動時間表計算。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>時間表計算</p></td> 
   <td>Workfront不會為在6個月內未更新的專案執行自動時間表計算，並在更新後才會繼續。<p>對於在3個月內未更新的專案，Workfront會每週執行時間表計算，而非每晚執行。</p><p>如需有關計算專案時間表的相關資訊，請參閱 <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">重新計算專案時間表</a>. </p></td> 
  </tr> 
 </tbody> 
</table>

<!-- Notes from the table: 
     <p>For tasks limits: (This is NOT TRUE , but the PMs always wanted this to stay the way it is because they don't want customers creating projects bigger than this.)</p>
    <p>For issue limits: (this is true only for some clusters; according to Anna A., some clusters are set to a million.)</p>
    -->