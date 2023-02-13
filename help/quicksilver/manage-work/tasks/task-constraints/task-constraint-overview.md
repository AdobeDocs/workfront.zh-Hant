---
content-type: overview
product-area: projects
navigation-topic: task-constraints
title: 任務約束概覽
description: 任務約束確定任務何時應在項目上開始和結束。
author: Alina
feature: Work Management
exl-id: 91b0844b-95a3-4d18-9fdb-a907dd42e1bf
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 10%

---

# 任務約束概覽

任務約束確定任務何時應在項目上開始和結束。

## 任務約束概覽

在建立項目計畫時，您會根據項目任務的順序和時間範圍做出決策。 任務可以獨立於任何任務序列運行，但可能會影響項目時間軸。 任務約束允許項目經理在某些任務可以在項目上啟動或完成時進行計畫。

根據您使用的約束，您可能必須為任務指定計畫起始日期、計畫完成日期或兩者。

要求定義日期的約束類型會影響前置關係。

>[!TIP]
>
>如果使用任務之間的前置關係，請考慮使用不需要特定日期的約束類型。

下表顯示每個約束及其縮寫。 縮寫用於任務清單和建立Kick-Start匯入檔案時。 按一下每個任務約束的連結標題，以了解有關該約束類型的詳細資訊。

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>限制名稱</strong> </p> </th> 
   <th> <p><strong>縮寫</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-soon-as-possible.md" class="MCXref xref">任務約束概覽：盡快</a> </p> </td> 
   <td scope="col"> <p>ASAP</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-late-as-possible.md" class="MCXref xref">任務約束概覽：盡可能晚 </a> </p> </td> 
   <td scope="col"> <p>ALAP</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/earliest-available-time.md" class="MCXref xref">任務約束概覽：最早可用時間</a> </p> </td> 
   <td scope="col"> <p>EAT</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/latest-available-time.md" class="MCXref xref">任務約束概覽：最新可用時間</a> </p> </td> 
   <td scope="col"> <p>LAT</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-earlier-than.md" class="MCXref xref">任務約束概覽：開始時間不早於</a> </p> </td> 
   <td scope="col"> <p>SNET</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-later-than.md" class="MCXref xref">任務約束概覽：不晚於</a> </p> </td> 
   <td scope="col"> <p>SNLT</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-earlier-than.md" class="MCXref xref">任務約束概覽：完成時間不早於</a> </p> </td> 
   <td scope="col"> <p>FNET</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-later-than.md" class="MCXref xref">任務約束概覽：完成時間不晚於</a> </p> </td> 
   <td scope="col"> <p>FNLT</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-start-on.md" class="MCXref xref">任務約束概覽：必須開始</a> </p> </td> 
   <td scope="col"> <p>MSO</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-finish-on.md" class="MCXref xref">任務約束概覽：必須完成</a> </p> </td> 
   <td scope="col"> <p>MFO</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/fixed-dates.md" class="MCXref xref">任務約束概覽：固定日期</a> </p> </td> 
   <td> <p>FIXT</p> </td> 
  </tr> 
 </tbody> 
</table>

## 預設限制概觀

建立新任務時，Workfront將自動選擇任務約束。

Workfront使用兩個變數來決定預設為新任務選取的任務限制：

* 此 **項目計畫自** 欄位。

   有關「項目計畫自」欄位的資訊，請參閱 [編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md).

* 此 **開始日期** 偏好設定由您的Workfront或群組管理員在 **工作與問題** 區域 **設定**.

   有關任務和問題首選項的資訊，請參閱 [配置全系統任務和問題首選項](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

下表顯示了為項目和新任務選擇不同變數時的預設任務約束：

| 項目計畫自 | 任務開始日期 | 任務約束預設值 |
|---|---|---|
| 從開始日期安排 | 基於項目計劃日期 | 盡可能早 |
| 從開始日期安排 | 今天 | 開始時間不早於 |
| 完成日期 | 基於項目計劃日期 | 盡可能晚 |
| 完成日期 | 今天 | 開始時間不晚於 |
