---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 任務期間與期間型別概觀
description: 任務期間是任務的計畫完成日期與計劃開始日期之間的差額。 「持續時間」表示任務可用的完成時間範圍。
author: Alina
feature: Work Management
recommendations: noDisplay, noCatalog
exl-id: c81e485a-7e8c-4907-8e6c-9991681c3541
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '1653'
ht-degree: 1%

---

# 任務期間與期間型別概觀

<!-- Audited: 12/2023 -->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

任務期間是任務的計畫完成日期與計劃開始日期之間的差額。 「持續時間」表示任務可用的完成時間範圍。

任務的工期型別可識別指派給任務的資源數量、總工作量及任務工期總計之間的關係。

## 任務期間概觀

如果任務的「實際開始日期」與「實際完成日期」在專案、主要受指派人或預設排程的排程之外，則任務「工期」為零。

>[!BEGINSHADEBOX]

**範例**
如果您的排程從上午9:00開始，到中午12:00結束，而工作排程從下午2:00開始，到下午4:00結束，則工作的期間為零。


>[!ENDSHADEBOX]

在Adobe Workfront中計算持續時間時，有兩種情況存在：

* 如果任務指派給一位使用者：

   1. Workfront會考慮專案或指派給任務之使用者的排程。

      當任務指派給一位使用者時，您的Workfront或群組管理員會決定Workfront使用的排程。 如需詳細資訊，請參閱[設定全系統的專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

   1. 如果使用者或專案沒有排程，Workfront會使用系統預設排程。

      這些步驟類似於瞭解Workfront使用哪個排程來計算持續時間後的第一個案例。

* 如果任務指派給多個使用者：

   1. Workfront會考慮專案或主要受指派人的排程。

      當任務指派給多個使用者時，您的Workfront或群組管理員會決定Workfront使用的排程。 如需詳細資訊，請參閱[設定全系統的專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

   1. 如果主要受指派人或專案沒有排程，Workfront會使用系統預設排程。

  這些步驟類似於瞭解Workfront使用哪個排程來計算持續時間後的第一個案例。

>[!NOTE]
>
>若將專案的主要受指派人休假列入考量，任務的計畫日期可能會調整，但任務的期間保持不變。 如需有關在規劃專案時考慮主要受指派人休假的資訊，請參閱[設定全系統專案偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

## 任務期間的時間單位

您可以指定正常時間與計劃開始與計畫完成日期之間經過的時間中的任務工期。

更新清單中工作的期間時，您可以使用下列縮寫來表示Workfront中的時間單位：

| 時間單位 | 縮寫 |
|---|---|
| 分鐘 | 一 |
| 時數 | H |
| 天。 這是預設值。 | D |
| 週 | 週 |
| 月 | T， MO |
| 經過的分鐘數 | EM |
| 經過的時數 | EH |
| 經過的天數 | ED |
| 經過的週數 | EW |
| 經過的月數 | ET |

{style="table-layout:auto"}

>[!BEGINSHADEBOX]

**範例**

如果您想要指出任務的期間是3個經過的天數，應在任務清單的「期間」欄位中輸入「3 ED」。  您也可以在編輯任務時，從可用的下拉式功能表或「任務詳細資訊」區段中，選取「期間單位」的偏好選項。 如需有關編輯任務的資訊，請參閱[編輯任務](../../../manage-work/tasks/manage-tasks/edit-tasks.md)。


>[!ENDSHADEBOX]

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: stays QS only forever; for the pictures below: make the first one classic at preview time and the second one stays QS always. The second one is yellow >> take out at 21.2 production!!)</p>
-->

![](assets/duration-elapsed-days-tasks-nwe-350x282.png)

指示任務的期間時，請考量下列事項：

* 經過的時間是任務期間的時間單位。 這是任務的計劃開始日期與計畫完成日期之間的時間，包括假日、週末和休假。 換句話說，經過的時間就是行事曆的天數。
* 天數代表系統中定義的工作日，可在「設定」區域中設定。 在大多數情況下，一天包含8小時。
* 正常時間（日或工作日）會考量假日、週末和休假，並將它們排除在任務的工期之外。
* 當您以周為單位指出任務的期間時，Workfront會根據您的Workfront管理員在「設定」的「專案偏好設定」區域中設定的「每週一般工作天數」和「每工作日一般小時數」設定，以天和小時計算期間。
* Workfront在計算「月持續時間」時，會使用4週的預設一個月持續時間。

## 任務期間型別概觀

管理作業的「工期型別」可讓您根據作業的需求來設定一致的資源指定。

持續時間型別可協助回答下列問題：

* 我們有多忙？
* 這項工作有多大？
* 需要多久？

![duration_type_triangle.png](assets/duration_type_triangle.png)

## 定義期間型別

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th scope="row"><p><strong>期間類型</strong></p></th> 
   <th scope="col"> <p><strong>函式</strong> </p> </th> 
   <th scope="col"> <p><strong>資源如何影響它</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <th scope="col"> <p><strong>計算的工作分派</strong> </p> </th> 
   <td scope="col"> <p>計算任務中每個受指派人的配置百分比。 </p> <p>選擇此「期間型別」時，您可以為任務輸入個別的「期間」和「計畫時數」。 Workfront將計畫時數除以任務期間內的時數，再除以指派給任務的資源數，以計算每個受指派人的分配。</p> <p>如需詳細資訊，請參閱<a href="../../../manage-work/tasks/taskdurtn/calculated-assignment.md" class="MCXref xref">期間型別總覽：計算的指派</a>。</p> </td> 
   <td scope="col">將受指派者新增或移除至任務時，持續時間和計畫時數未變更。 </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>已計算的工作</strong> </p> </th> 
   <td scope="col"> <p>決定完成任務所需的計畫時數（工作量）。</p> <p>通常用於指派給任務的資源被配置給任務的整個期間時。</p> <p>選擇此「期間型別」時，您就可以為任務輸入個別期間。 Workfront計算任務的「計畫時數」，方法是將「工期」中的天數乘以排程中的工作時數，再乘以任務的受指派人數。 </p> <p>您可以手動將每個受指派人的配置百分比變更為任務，這會縮短計畫時數的數量。</p> <p>如需詳細資訊，請參閱<a href="../../../manage-work/tasks/taskdurtn/calculated-work.md" class="MCXref xref">期間型別總覽：計算的工作量</a>。</p> </td> 
   <td scope="col"> <p>當受指派人新增至任務時，計畫時數會增加。 </p> <p>當受指派人從任務中移除時，計畫時數便會減少。</p> </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>投入比導向</strong></p> </th> 
   <td scope="col"> <p>根據資源數量決定計畫時數。</p> <p>選擇此「期間型別」時，您就可以為任務輸入個別期間。 Workfront計算任務的「計畫時數」，方法是將「工期」中的天數乘以排程中的工作時數，再除以任務的受指派人數。 </p> <p>您可以手動變更每個受指派人至任務的配置百分比，但計畫時數保持不變。</p> <p>如需詳細資訊，請參閱<a href="../../../manage-work/tasks/taskdurtn/effort-driven.md" class="MCXref xref">期間型別總覽：投入比導向</a>。</p> </td> 
   <td scope="col"> <p>當受指派人從任務中移除時，計畫時數會增加。</p> <p>當受指派人新增至任務時，計畫時數便會減少。 </p> <p>期間不會變更，無論受指派人數或其排程有何變更。 </p> <p>期間等於計畫時數。 計畫期間等於計畫時數除以受指派人數。</p> </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>簡單</strong> </p> </th> 
   <td scope="col"> <p>根據每個被指定者被分配的時數決定計畫時數與持續時間（對於此持續時間型別是相同的）。 </p> <p>Workfront計算計畫時數的方法為加總每個受指派人的計劃分配時數。 </p> <p>您可以手動變更每個受指派人分配的時數，而計畫時數和「期間」量會隨之變更。 如果您選擇所有受指派人的分配時數總計，則該數字會平均分配給每個受指派人。</p> <p>如需詳細資訊，請參閱<a href="../../../manage-work/tasks/taskdurtn/simple-duration-type.md" class="MCXref xref">期間型別概觀：簡單</a>。</p> </td> 
   <td scope="col"> <p>如果您選擇分配時數的總數，則時數會在被指定者之間平均分配。 不過，身為專案經理，您可以手動調整每個受指派人的時數。 </p> <p>您可以編輯內嵌或任務層級具有「簡單期間型別」之任務的計畫時數與期間。 </p> <p>如果將敏捷團隊指派給任務，則「持續時間型別」會自動設定為「簡單」，且無法變更。 敏捷團隊的任務持續時間必須大於0分鐘。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 新任務的期間型別

新任務的期間型別符合系統中設定的期間型別。 預設期間型別為已計算的任務指派。 您的Workfront管理員或群組管理員可以為您的系統或與專案關聯的群組更新預設期間型別。 如需詳細資訊，請參閱[設定全系統的任務和問題偏好設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。

## 父系任務的原始期間

任務的原始期間是任務成為父任務之前的原始期間（以分鐘為單位）。

當任務成為父系時，最早子系的計劃開始日期與最後一個子系的計畫完成日期之間的期間會累計至父系任務，並成為父系任務的期間。 這會取代原始任務的工期。

當子系使用「經過天數」的「持續時間」單位，而父系使用「天數」的「持續時間」單位時，Workfront計算父系任務的「持續時間」的方式可能會有差異。

請考量下列事項：

* 期間單位「經過天數」代表工作歷天數，一律包括每天24小時。
* 持續時間單位Days代表系統中定義的工作日，且可設定。 在大多數情況下，每天會包含8小時。
* 計算父系任務持續時間的公式如下：

  `Parent task duration = Planned Completion Date of the child task that is planned to end the latest - Planned Start Date of the child task that starts the earliest`

* 計算父系任務的工期時，系統會先使用上述公式計算工期，然後套用排程。


如需詳細資訊，請參閱[任務原始期間與原始計畫時數概觀](/help/quicksilver/manage-work/tasks/task-information/task-original-duration-and-original-planned-hours.md)。

## 變更任務的期間型別

如需有關變更任務期間型別的資訊，請參閱[更新任務的期間型別](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md)。
