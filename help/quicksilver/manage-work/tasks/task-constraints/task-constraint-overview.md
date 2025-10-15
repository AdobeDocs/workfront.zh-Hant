---
content-type: overview
product-area: projects
navigation-topic: task-constraints
title: 任務限制總覽
description: 任務限制決定任務在專案上何時開始和結束。
author: Alina
feature: Work Management
exl-id: 91b0844b-95a3-4d18-9fdb-a907dd42e1bf
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 6%

---

# 任務限制總覽

<!-- Audited: 12/2023 -->

任務限制決定任務在專案上何時開始和結束。

## 任務限制概要

當您建立專案計畫時，您可以決定專案上任務的順序和時間範圍。 任務可以獨立於任何任務序列運行，但它們可能會影響專案時間表。 任務限制可讓專案經理計畫特定任務何時可在專案上開始或完成。

根據您使用的限制，您可能需要為任務指定計劃開始日期、計畫完成日期或兩者。

需要定義日期的限制型別會影響前置任務關係。

>[!TIP]
>
>如果您在任務之間使用前置任務關係，請考慮使用不需要特定日期的限制型別。

下表顯示每個限制及其縮寫。 任務清單和建立Kick-Start匯入檔案時會使用縮寫。 按一下每個任務限制的連結標題，以取得該型別限制的詳細資訊。

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col>
 <thead> 
  <tr> 
   <th> <p><strong>條件約束名稱</strong> </p> </th> 
   <th> <p><strong>縮寫</strong> </p> </th> 
   <th> <p><strong>說明</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-soon-as-possible.md" class="MCXref xref">任務限制總覽：儘快</a> </p> </td> 
   <td scope="col"> <p>ASAP</p> </td>
   <td scope="col"> <p>將任務的開始時間儘可能放置在專案開頭附近。</p> 
   <p>如果專案使用從開始日期起的「排程模式」，並且新任務的系統預設開始日期設定為「根據專案計畫日期」，則為預設限制。 </p>
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-late-as-possible.md" class="MCXref xref">任務限制總覽：儘可能遲</a> </p> </td> 
   <td scope="col"> <p>ALAP</p> </td> 
   <td scope="col"> <p>將任務的完成時間儘可能放置在專案結尾處。</p> 
   <p>當專案「排程模式」為「完成日期」，且任務的「開始日期」的系統或群組預設值設定為「根據專案計畫日期」時，此為預設限制。 </p>
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/earliest-available-time.md" class="MCXref xref">任務限制總覽：最早可用時間</a> </p> </td> 
   <td scope="col"> <p>EAT</p> </td> 
 <td scope="col"> <p>在考量任何前置任務關係後，排程任務在最早可用時間開始。</p> </td>
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/latest-available-time.md" class="MCXref xref">任務限制總覽：最新可用時間</a> </p> </td> 
   <td scope="col"> <p>LAT</p> </td> 
   <td scope="col"> <p>在專案中考慮前置任務與後續任務之間的關係後，將任務排程為最晚可用時間開始。</p> </td>
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-earlier-than.md" class="MCXref xref">任務限制總覽：開始時間不早於</a> </p> </td> 
   <td scope="col"> <p>SNET</p> </td> 
   <td scope="col"> <p>排程在指定日期之後開始的工作。</p> 
   <p>如果專案「排程模式」是從「開始日期」開始，且系統或群組預設新任務的「開始日期」設定為「今天」，則這是預設限制。   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-later-than.md" class="MCXref xref">任務限制總覽：開始時間不晚於</a> </p> </td> 
   <td scope="col"> <p>SNLT</p> </td> 
   <td scope="col"> <p>排程在指定日期之前開始的工作。</p> 
   <p>如果專案的「排程模式」是從「完成日期」開始，且系統或群組對任務「開始日期」的預設設定為「今天」，則這是預設限制。 
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-earlier-than.md" class="MCXref xref">任務限制總覽：完成時間不早於</a> </p> </td> 
   <td scope="col"> <p>FNET</p> </td>
   <td scope="col"> <p>排程在指定日期之後完成的工作。</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-later-than.md" class="MCXref xref">任務限制總覽：完成時間不晚於</a> </p> </td> 
   <td scope="col"> <p>FNLT</p> </td> 
   <td scope="col"> <p>排程在您指定日期之前完成的工作。</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-start-on.md" class="MCXref xref">任務限制總覽：必須從</a>開始 </p> </td> 
   <td scope="col"> <p>MSO</p> </td> 
   <td scope="col"> <p>將任務排程為完全在特定日期開始。</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-finish-on.md" class="MCXref xref">任務限制總覽：必須在</a>完成 </p> </td> 
   <td scope="col"> <p>MFO</p> </td> 
   <td scope="col"> <p>排程要在特定日期結束的工作。</p> </td>
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/fixed-dates.md" class="MCXref xref">任務限制總覽：固定日期</a> </p> </td> 
   <td> <p>FIXT</p> </td> 
   <td> <p>排定在特定日期開始和結束的工作。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 預設限制的總覽

當您建立新任務時，Workfront會自動選取任務限制。

Workfront使用兩個變數來決定預設為新任務選取哪個任務限制：

* 專案上的&#x200B;**專案排程**&#x200B;欄位。

  如需「專案排程起始日期」欄位的詳細資訊，請參閱[編輯專案](../../../manage-work/projects/manage-projects/edit-projects.md)。

* 您的Workfront或群組管理員在&#x200B;**設定**&#x200B;的&#x200B;**任務和問題**&#x200B;區域中設定的&#x200B;**開始日期**&#x200B;偏好設定。

  有關任務和問題偏好設定的資訊，請參閱[設定系統範圍的任務和問題偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md#new-task-defaults)中的[新任務預設值](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)區段。

下表顯示為您的專案和新任務選擇不同變數時的預設任務限制：

| 專案排程開始日期 | 任務開始日期 | 任務限制預設 |
|---|---|---|
| 開始日期 | 基於項目計劃日期 | 盡可能早 |
| 開始日期 | 今天 | 開始時間不早於 |
| 完成日期 | 基於項目計劃日期 | 儘可能遲 |
| 完成日期 | 今天 | 開始時間不晚於 |
