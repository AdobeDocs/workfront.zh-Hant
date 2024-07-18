---
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: 系統任務狀態
description: Workfront需要三種內建的系統任務狀態，這表示您可以解除鎖定、重新命名和重新排序這些狀態，但無法隱藏或刪除它們。 您也可以新增新的系統任務狀態，以符合組織中的需求。 變更任務狀態通常是手動程式，但有時任務狀態會根據系統中發生的其他因素自動變更。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b8c751c3-aed3-4836-a888-f3f8a5f08421
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# 系統任務狀態

Workfront需要三種內建的系統任務狀態，這表示您可以解除鎖定、重新命名和重新排序這些狀態，但無法隱藏或刪除它們。

您也可以新增新的系統任務狀態，以符合組織中的需求。

變更任務狀態通常是手動程式。 不過，當任務的狀態根據系統中發生的其他因素自動變更時，有時會在下列清單中概述。

您的Workfront執行個體會提供下列任務狀態：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>系統任務狀態</th> 
   <th>當此狀態發生時</th> 
   <th>任務處於此狀態時發生的動作</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>新增（必要狀態）</td> 
   <td>這是每個新建立任務的預設狀態。</td> 
   <td>如果任務位於狀態為「目前」的專案上，則任務會顯示在指派給任務之使用者的「工作請求」標籤中。 使用者現在可以開始處理任務。</td> 
  </tr> 
  <tr> 
   <td>進行中（必要狀態）</td> 
   <td>您可以將任務置於此狀態，以表示該任務上的工作已開始。</td> 
   <td> <p>將任務標示為「進行中」時，任務會顯示「實際開始日期」的值。</p> <p>在您手動更新任務的完成百分比之前，不會記錄任務的進度。</p> </td> 
  </tr> 
  <tr> 
   <td>完成（必要狀態）</td> 
   <td> <p>當工作完成時，您可以手動將工作標示為完成。</p> <p>當任務的「追蹤模式」設定為「自動完成」時，任務在達到「計畫完成日期」時會自動標籤為「完成」。</p> </td> 
   <td> <p>任務完成時，任務的完成百分比會標籤為100%。 任務完成時，會從首頁區域的受指派人工作清單中移除。</p> <p>將任務標示為「完成」時，任務會顯示「實際完成日期」的值。</p> <p><b>注意</b>：如果任務有未完成的問題，而您將其狀態變更為「完成」，則狀態會自動變更為「完成 — 未決問題」。</p> </td> 
  </tr> 
 </tbody> 
</table>
