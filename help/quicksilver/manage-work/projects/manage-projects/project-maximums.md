---
title: 專案限制概觀
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: Adobe Workfront有限制可與專案關聯的物件數。 已設定專案限制，以改善產品效能並提升您使用Workfront的體驗。
author: Alina
feature: Work Management
exl-id: 60576107-89f1-4328-89e2-5b1e5e243fd9
source-git-commit: 809f1c3629c343a55305c0c617f4974dc05439bf
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---

# 專案限制概觀

Adobe Workfront有限制可與專案相關聯的物件數。 已設定專案限制，以改善產品效能並提升您使用Workfront的體驗。

與項目關聯的以下對象具有以下限制：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>任務</p></td> 
   <td>  <p>每個項目的任務數上限為5,000。 當任務數達到此上限時，會顯示警告訊息。 達到上限時，會顯示錯誤訊息，且無法將其他工作新增至專案。</p> <p>為避免達到此最大值，請將已關閉的任務移至為已結束任務指定的另一個項目。 這些項目的報告可能需要調整。</p>

<b>重要</b>

對於任務具有大量依賴項的項目，我們建議項目中的任務數應遠低於允許的5,000個任務的最大數。

可能會影響或阻止重新計算項目時間表的任務依賴關係的一些示例如下：

<ul><li>子代數</li>
   <li>多級任務縮進</li>
   <li>前置任務數</li>
   <li>多項分配</li>
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>問題</p></td> 
   <td>  <p>每個專案的問題數上限為10,000。 當問題數量接近此上限時，會顯示警告訊息。 達到上限時，會顯示錯誤訊息，且無法將其他問題新增至專案。</p> <p>為避免達到此上限，請將關閉的問題移至指定用於關閉問題的另一個專案。 這些項目的報告可能需要調整。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>持續時間</p></td> 
   <td> <p>專案的最長持續時間必須為15年，Workfront才能自動計算其時間軸。 當專案持續時間接近上限時，會顯示警告訊息。 達到上限時，會顯示警告訊息，不再進行自動時間軸計算。</p> <p>只要調整項目中任務的日期，將項目的持續時間縮短到15年以下，自動時間軸計算就會恢復。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>時間軸計算</p></td> 
   <td>Workfront不會為6個月未更新的專案執行自動時間軸計算，且只有進行更新後才會繼續。<p>對於3個月未更新的專案，Workfront會每週執行時間軸計算，而非夜間計算。</p><p>如需計算專案時間軸的相關資訊，請參閱 <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">重新計算項目時間表</a>. </p></td> 
  </tr> 
 </tbody> 
</table>

<!-- Notes from the table: 
     <p>For tasks limits: (This is NOT TRUE , but the PMs always wanted this to stay the way it is because they don't want customers creating projects bigger than this.)</p>
    <p>For issue limits: (this is true only for some clusters; according to Anna A., some clusters are set to a million.)</p>
    -->