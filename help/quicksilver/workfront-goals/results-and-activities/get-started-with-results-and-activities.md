---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: 開始使用Adobe Workfront Target中的結果和活動
description: 您必須將結果、活動或對齊目標新增至目標，才能啟用它。 這會將目標狀態從草稿更新為作用中，並開始記錄目標的進度。
author: Alina
feature: Workfront Goals
exl-id: 64fa0aef-cb92-465a-9b74-d863fc232fd1
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 0%

---

# 開始使用Adobe Workfront Target中的結果和活動

<!--drafted for P&P new model: the note at the top will need to be replaced with this:    
    
Your organization must have the following to use the functionality described in this article:    
    
* For the legacy plan and license structure:     
    
  * A Pro or higher [Adobe Workfront plan](https://www.workfront.com/plans).     
  * An Adobe Workfront Goals license in addition to a Workfront license.    
    
* For the current plan and license structure:    
    
  * An Ultimate plan     
        
    Or    
        
    An additional license for Adobe Workfront Goals for the Prime or Select Adobe Workfront plans. <is there a link we can add here for the plans and what they contain?!>    
    
Contact your Workfront account manager to learn about a Workfront Goals license.    
    
For additional information about access to Workfront Goals, see [Requirements to use Workfront Goals](../workfront-goals/goal-management/access-needed-for-wf-goals.md).    
-->

>[!NOTE]
>
>貴組織必須具備下列條件才能使用本文所述的功能：
>
>* Pro或更高版本 [Adobe Workfront計畫](https://www.workfront.com/plans).
>* 除了Adobe Workfront授權，還有Workfront授權。
>
>  請連絡您的Workfront客戶經理，以了解Workfront Target授權。
>
>如需存取Workfront目標的詳細資訊，請參閱 [使用Workfront目標的需求](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).


建立目標時，目標的狀態為「草稿」。 如需建立目標的相關資訊，請參閱 [在Adobe Workfront目標中建立目標](../../workfront-goals/goal-management/create-goals.md).

若要開始記錄目標的進度，您必須啟動該目標。 若要啟動目標並將其狀態變更為「啟用」，您必須先新增下列項目：

* 結果
* 活動
* 專案
* 目標一致

新增至少其中一個項目後，您就可以啟動目標。 您必須更新目標的結果和活動，以指出目標的進度。


>[!IMPORTANT]
>
> 目標的活動、結果、項目或目標之間不能超過1000個。</span>

本文概述活動和結果。 如需協調目標的相關資訊，請參閱 [Adobe Workfront目標中的目標一致性](../../workfront-goals/goal-alignment/goal-alignment.md). 如需將專案連結至目標的相關資訊，請參閱 [將專案新增至Adobe Workfront目標中的目標](../results-and-activities/connect-projects-to-goals-overview.md).

## 結果概述

<!--
<p> This will have additional types in the future - add another section for types?)</p>
-->

結果會衡量目標的進度，或您接近達成目標的程度。 作為目標擁有者，您也可以擁有結果。 目標的結果也可能指派給不同的使用者。

如需將結果新增至目標的相關資訊，請參閱 [將結果新增至Adobe Workfront目標中的目標](../../workfront-goals/results-and-activities/add-results-to-goals.md).

您可以將結果新增至屬於組織中其他實體的您自己的目標或目標。

處理結果時，請考量下列事項：

* 他們回答的問題是：「我如何知道我的目標何時完成？」
* 它們是量度指標。 您可以從下列選項中選取，以指出結果的進度：

   <!--
  this might change (jira, Salesforce, etc))
  -->

   * 貨幣
   * 數量
   * 百分比

如需結果的詳細資訊，請參閱區段中的結果和活動之間的相似度清單 [結果、活動和專案之間的相似性](#similarities-between-results-activities-and-projects) 這篇文章。

## 活動概覽

<!--
This will have additional types in the future - add another section for types?
-->

活動（如結果）是特定和可衡量的，通常包括百分比完成指標。 作為目標擁有者，您也可以擁有與目標相關聯的活動。 目標上的活動也可能指派給不同的使用者。

如需將活動新增至目標的相關資訊，請參閱 [將活動新增至Adobe Workfront目標中的目標](../../workfront-goals/results-and-activities/add-activities-to-goals.md).

將活動與您的目標關聯時，請考慮下列事項：

* 他們回答了「當目標完成時，我將實現什麼？」
* 活動是自訂項目，在完整或不完整方面可想而知。 必須手動更新，以指出目前已完成的活動百分比。

<!--
* You can associate the following activities with goals:

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Manual progress bar </td> 
     <td> <p>Custom entries that can be thought of more in terms of complete or incomplete. They must be manually updated.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader"><p>Project</p></td> 
     <td> <p>Existing projects that you have at least permissions to View and are not in a status of Dead. They are updated automatically, based on the progress of their work items. </p> <p>The projects must exist before associating them with the goal. You can associate a project with multiple goals. For information about adding projects to goals, see <a href="../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md" class="MCXref xref">Add projects to goals in Adobe Workfront Goals</a>.</p>
     <p><span class="preview">In the Preview environment, projects are separate progress indicators, independent from activities. Adding projects to a goal in the Preview environment is different from adding activities. For more information, see <a href="../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md" class="MCXref xref">Add projects to goals in Adobe Workfront Goals</a>.</span></p>
      </td> 
    </tr> 
   </tbody> 
  </table>
-->
<!--drafted for goal redesign: For THE PRODUCTION RELEASE: remove the projects in this article altogether.-->

如需結果和活動的詳細資訊，請參閱區段中的結果和活動之間的相似度清單 [結果、活動和專案之間的相似性](#similarities-between-results-activities-and-projects) 這篇文章。

## 結果、活動和專案之間的相似性 {#similarities-between-results-activities-and-projects}

成果、活動和項目是目標進展指標。

管理專案的方式與管理結果和活動的方式有一些差異。 如需將專案新增至目標的相關資訊，請參閱 [將活動新增至Adobe Workfront目標中的目標](../../workfront-goals/results-and-activities/add-activities-to-goals.md). 如需與目標連結之專案的相關資訊，請參閱 [將專案新增至Adobe Workfront目標中的目標](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

除了結果、活動和項目之外，您還可以將子目標與目標關聯。 兒童目標也是目標的一種進展指標。 如需詳細資訊，請參閱 [在Adobe Workfront目標中將目標連結起來，以協調目標](../goal-alignment/align-goals-by-connecting-them.md). 兒童目標進度指標的進展也推動父項目標的進展。

下表顯示結果、活動和項目之間的相似性和差異，作為目標指標：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b><p>功能</p></b></td> 
   <td><b><p>結果</p></b></td> 
   <td><b><p>活動</p></b></td> 
   <td> <p><strong>專案</strong> </p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td><span style="font-weight: normal;">您可以在Workfront介面中自訂物件名稱</span> </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>您可以將它們新增至過去的目標。</td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>您可以將多個結果、活動或專案與相同目標建立關聯。 </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>您可以將其中一個目標與多個目標建立關聯。</td> 
   <td> </td> 
   <td> </td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>在計算目標進度時，會考慮其進度。 </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>必須在Workfront Target中手動更新</td> 
   <td>✔</td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>它們將於目標的結束日期完成</td> 
   <td>✔</td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>它們只能指派給使用者，而不能指派給團隊、群組或公司。 </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>它們是特定的、可衡量的，並且通常包括指示其進展的設定數。 </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>它們提供介於開始值和結束值之間的值範圍，說明您接近這些值的程度。 與結束值的接近度會計算目標的進度值。 </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
 </tbody> 
</table>
