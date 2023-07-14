---
content-type: overview
product-area: projects
navigation-topic: task-constraints
title: 任務限制總覽
description: 任務限制決定任務何時應該在專案上開始和結束。
author: Alina
feature: Work Management
exl-id: 91b0844b-95a3-4d18-9fdb-a907dd42e1bf
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 6%

---

# 任務限制總覽

任務限制決定任務何時應該在專案上開始和結束。

## 任務限制概要

當您建立專案計畫時，您可以決定專案上任務的順序和時間範圍。 任務可以獨立於任何任務序列運作，但可能影響專案時間表。 任務限制可讓專案經理計畫特定任務何時可以在專案上開始或完成。

根據您使用的限制，您可能需要為任務指定計劃開始日期、計畫完成日期或兩者。

需要定義日期的限制型別會影響前置任務關係。

>[!TIP]
>
>如果在任務之間使用前置任務關係，請考慮使用不需要特定日期的限制型別。

下表顯示每個限制及其縮寫。 工作清單和建立Kick-Start匯入檔案時，會使用縮寫。 按一下每個任務限制的連結標題，以取得該型別限制的詳細資訊。

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col>
 <thead> 
  <tr> 
   <th> <p><strong>限制名稱</strong> </p> </th> 
   <th> <p><strong>縮寫</strong> </p> </th> 
   <th> <p><strong>說明</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-soon-as-possible.md" class="MCXref xref">任務限制總覽：儘快</a> </p> </td> 
   <td scope="col"> <p>ASAP</p> </td>
   <td scope="col"> <p>將任務的開始時間儘量放在接近專案開始的時間處。</p> 
   <p>如果專案使用「開始日期」的「排程模式」，且新任務的系統預設開始日期設定為「根據專案計畫日期」，則為預設限制。 </p>
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-late-as-possible.md" class="MCXref xref">任務限制總覽：儘可能遲 </a> </p> </td> 
   <td scope="col"> <p>ALAP</p> </td> 
   <td scope="col"> <p>將任務的完成時間放在儘可能接近專案結尾的地方。</p> 
   <p>當專案「排程模式」是從「完成日期」開始，且任務的「開始日期」的系統或群組預設值是根據「專案計畫日期」時，此為預設限制。 </p>
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/earliest-available-time.md" class="MCXref xref">作業限制概要：最早可用時間</a> </p> </td> 
   <td scope="col"> <p>EAT</p> </td> 
 <td scope="col"> <p>在考慮任何前置任務關係後，將任務排定在最早可用時間開始。</p> </td>
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/latest-available-time.md" class="MCXref xref">任務限制總覽：最新可用時間</a> </p> </td> 
   <td scope="col"> <p>LAT</p> </td> 
   <td scope="col"> <p>在專案中考慮前置任務與後續任務之間的關係後，將任務排程為最晚可用時間開始。</p> </td>
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-earlier-than.md" class="MCXref xref">任務限制總覽：開始時間不早於</a> </p> </td> 
   <td scope="col"> <p>SNET</p> </td> 
   <td scope="col"> <p>將工作排程在您指定的日期之後開始。</p> 
   <p>如果專案的「排程模式」是從「開始日期」開始，且系統或群組為新任務的預設「開始日期」設定為「今天」，則此為預設限制。   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-later-than.md" class="MCXref xref">任務限制總覽：開始時間不晚於</a> </p> </td> 
   <td scope="col"> <p>SNLT</p> </td> 
   <td scope="col"> <p>排程在指定日期之前開始的工作。</p> 
   <p>如果專案的「排程模式」是從「完成日期」開始，且任務的「開始日期」的系統或群組預設值為「今天」，則「開始」為預設限制。 
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-earlier-than.md" class="MCXref xref">作業限制概要：完成時間不早於</a> </p> </td> 
   <td scope="col"> <p>FNET</p> </td>
   <td scope="col"> <p>排程在指定日期之後完成的工作。</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-later-than.md" class="MCXref xref">任務限制總覽：完成時間不晚於</a> </p> </td> 
   <td scope="col"> <p>FNLT</p> </td> 
   <td scope="col"> <p>排程在指定日期之前完成的工作。</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-start-on.md" class="MCXref xref">任務限制總覽：必須開始於</a> </p> </td> 
   <td scope="col"> <p>MSO</p> </td> 
   <td scope="col"> <p>將任務排程為完全在特定日期開始。</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-finish-on.md" class="MCXref xref">任務限制總覽：必須完成日期</a> </p> </td> 
   <td scope="col"> <p>MFO</p> </td> 
   <td scope="col"> <p>排程要在特定日期結束的工作。</p> </td>
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/fixed-dates.md" class="MCXref xref">任務限制總覽：固定日期</a> </p> </td> 
   <td> <p>FIXT</p> </td> 
   <td> <p>排程要在特定日期開始和結束的任務。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 預設限制的總覽

當您建立新任務時，Workfront會自動選取任務限制。

Workfront使用兩個變數來決定預設為新任務選取的任務限制：

* 此 **專案排程開始日期** 欄位。

  如需「專案排程起始日期」欄位的詳細資訊，請參閱 [編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md).

* 此 **開始日期** 由您的Workfront或群組管理員在 **任務和問題** 區域 **設定**.

  如需任務和問題偏好設定的相關資訊，請參閱以下的「新任務預設值」一節： [設定系統範圍的任務和問題偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

下表顯示為您的專案和新任務選擇不同變數時的預設任務限制：

| 專案排程開始日期 | 任務開始日期 | 任務限制預設 |
|---|---|---|
| 開始日期 | 基於項目計劃日期 | 盡可能早 |
| 開始日期 | 今天 | 開始時間不早於 |
| 完成日期 | 基於項目計劃日期 | 儘可能遲 |
| 完成日期 | 今天 | 開始時間不晚於 |
