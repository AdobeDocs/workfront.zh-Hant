---
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: 系統任務狀態
description: Workfront中需要三種內建系統任務狀態，這表示您可以解除鎖定、重新命名和重新排序這些狀態，但無法隱藏或刪除它們。 您也可以新增系統任務狀態，以符合組織的需求。 更改任務的狀態通常是手動過程，但有時會根據系統中發生的其他因素自動更改任務的狀態。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b8c751c3-aed3-4836-a888-f3f8a5f08421
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---

# 系統任務狀態

Workfront中需要三種內建系統任務狀態，這表示您可以解除鎖定、重新命名和重新排序這些狀態，但無法隱藏或刪除它們。

您也可以新增系統任務狀態，以符合組織的需求。

更改任務的狀態通常是手動過程。 但是，根據系統中發生的其他因素，當任務的狀態自動更改時，有時會在以下清單中列出。

您的Workfront執行個體會提供下列任務狀態：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>系統任務狀態</th> 
   <th>發生此狀態時</th> 
   <th>任務處於此狀態時發生的操作</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>新增（必要狀態）</td> 
   <td>這是每個新建立任務的預設狀態。</td> 
   <td>如果任務位於項目上且狀態為「當前」，則任務將顯示在分配給任務的用戶的「工作請求」頁簽中。 使用者現在可以開始處理工作。</td> 
  </tr> 
  <tr> 
   <td>正在進行（必需狀態）</td> 
   <td>您可以將任務置於此狀態，以指示該任務的工作已啟動。</td> 
   <td> <p>將任務標籤為「正在執行中」時，該任務將顯示「實際開始日期」的值。</p> <p>在手動更新任務完成百分比之前，不會記錄任務的進度。</p> </td> 
  </tr> 
  <tr> 
   <td>完成（必要狀態）</td> 
   <td> <p>您可以在完成任務完成時手動標籤任務完成。</p> <p>當任務的「跟蹤模式」設定為「自動完成」時，當任務達到「計畫完成日期」時，該任務將自動標籤為「完成」。</p> </td> 
   <td> <p>任務完成後，任務完成百分比將標籤為100%。 完成任務後，該任務將從「首頁」(Home)區域的受託人的工作清單中刪除。</p> <p>將任務標籤為「完成」時，該任務將顯示實際完成日期的值。</p> <p><b>注意</b>:如果任務有未完成的問題，並且您將任務狀態更改為「完成」，則狀態將自動更改為「完成 — 待定問題」。</p> </td> 
  </tr> 
 </tbody> 
</table>
