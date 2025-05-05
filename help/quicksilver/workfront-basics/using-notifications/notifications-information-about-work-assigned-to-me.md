---
content-type: reference
navigation-topic: notifications
title: 通知：關於指派給我的工作的資訊
description: 下列通知會提醒您工作專案上發生指派給您的活動。
author: Lisa
feature: Get Started with Workfront
exl-id: 5d7fdee8-cb5c-4ab8-bec3-beff9851b8f6
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '2088'
ht-degree: 1%

---

# 通知：關於指派給我的工作的資訊

下列通知會提醒您工作專案上發生指派給您的活動。

如需有關設定您收到哪些通知的資訊，請參閱[修改您自己的電子郵件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)。

另請參閱[事件通知](../../workfront-basics/using-notifications/event-notifications.md)。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>通知</th> 
   <th> <p>包含的欄位 </p> <p> *僅每日摘要欄位</p> </th> 
   <th>預設狀態</th> 
  </tr> 
 </thead> 
 <tbody>
  <tr> 
   <td> <p><strong>指派給我的團隊之任務的前置任務已完成</strong> </p> <p>當指派團隊的其中一項任務的前置任務完成時，會收到電子郵件通知。 </p> <p>擁有[!UICONTROL Review]或[!UICONTROL Requestor]授權的使用者不會收到通知。</p> <p>即時通知電子郵件的主旨為： <em>完成： &lt;工作名稱&gt;</em></p> <p> 每日摘要通知的主旨為： <em> [!UICONTROL 指派給您的工作摘要] &lt;每日摘要日期&gt; </em></p> </td> 
   <td> <p>前置任務名稱<br>前置任務專案<br>前置任務參考編號<br>完成前置任務的使用者名稱<br>前置任務狀態<br>前置任務完成的日期和時間<br>前置任務的前置任務的前置任務狀態<br><strong>檢視更多詳細資料</strong>按鈕<br>*專案名稱<br>*專案參考編號<br>*已完成前置任務的總數<br>*任務名稱<br>*完成任務的使用者名稱<br>*每日摘要的日期 </p> </td> 
   <td><strong>每日</strong> </td>
  </tr>
  <tr> 
   <td> <p><strong>我的其中一項任務的前置任務已完成</strong> </p> <p>當任務受指派人的其中一項任務的前置任務完成時，該任務受指派人會收到電子郵件通知。 </p> <p>擁有[!UICONTROL Review]或[!UICONTROL Requestor]授權的使用者不會收到通知。</p> <p>即時通知電子郵件的主旨為： <em>[!UICONTROL 完成]： &lt;工作名稱&gt;</em></p> <p> 每日摘要通知的主旨為： <em> [!UICONTROL 指派給您的工作摘要] &lt;每日摘要日期&gt; </em></p> </td> 
   <td> <p>前置任務名稱<br>前置任務專案<br>前置任務參考編號<br>完成前置任務的使用者名稱<br>前置任務狀態<br>前置任務完成的日期和時間<br>前置任務的前置任務的前置任務狀態<br><strong>[!UICONTROL 檢視更多詳細資料]</strong>按鈕<br>*專案名稱<br>*專案參考編號<br>*已完成前置任務的總數<br>*任務名稱<br>*完成前置任務的使用者名稱<br>*日期每日摘要 </p> </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <!--
  <tr data-mc-conditions=""> 
   <td> <p><strong>A predecessor of one of my tasks is completed</strong> </p> <p>The task assignee receives an email notification when a predecessor of one of their tasks is completed. </p> <p>Users with a [!UICONTROL Review] or [!UICONTROL Requestor] license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>[!UICONTROL Complete]: &lt;Task Name></em></p> <p> The subject of the daily digest notification is: <em> [!UICONTROL Digest of Work Assigned to You] &lt;Date of daily digest> </em></p> </td> 
   <td> <p>Assigned by</p> <p>Task Name</p> <p>[!UICONTROL View] button</p> <p>Parent tasks</p> <p>Assignees</p> <p>Task status</p> <p>Task description</p> <p>Task Reference Number</p> <p> <br>Completed predecessor tasks </p> <p>Name of the user who completed the predecessor task<br>Date when the predecessor was completed</p> <p>[!UICONTROL View] button<br>Option to add to the daily digest</p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr> 
  -->
  <tr> 
   <td> <p><strong>我完成的任務已核准或已拒絕</strong> </p> <p>當任務被核准或拒絕時，任務受指派人會收到電子郵件通知。</p> <p>只有在專案狀態為「目前」時，才會傳送通知。</p> <p>擁有[!UICONTROL Review]或[!UICONTROL Requestor]授權的使用者不會收到通知。</p> <p>即時通知電子郵件的主旨為： <em>[!UICONTROL 完成]： &lt;專案名稱&gt;</em>上的&lt;任務名稱&gt;</p> <p> 每日摘要通知的主旨為： <em> [!UICONTROL 指派給您的工作摘要] &lt;每日摘要日期&gt; </em></p> </td> 
   <td> 任務名稱<br>專案名稱<br>任務參考編號<br>授與核准的使用者名稱<br>新任務狀態<br>核准或拒絕任務的日期與時間<br>先前的任務狀態<br><strong>[!UICONTROL 檢視更多詳細資料]</strong>按鈕<br>*專案名稱<br>*專案參考編號<br>*核准或拒絕的任務總數<br>*任務名稱<br>*核准或拒絕任務的使用者名稱<br>*核准決定（[!UICONTROL 已批准]/ [!UICONTROL 已拒絕]）<br>*每日摘要的日期<br></td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p id="a-task-i-m-assigned-to-is-completed"><strong>指派給我的任務已完成</strong> </p> <p>工作受指派人在工作完成時會收到電子郵件通知。</p> <p>只有在專案狀態為[!UICONTROL 目前]時，才會傳送通知。</p> <p>擁有[!UICONTROL Review]或[!UICONTROL Requestor]授權的使用者不會收到通知。</p> <p>即時通知電子郵件的主旨為： <em>[!UICONTROL 完成]： &lt;專案名稱&gt;</em>上的&lt;任務名稱&gt;</p> <p> <p>注意：如果任務變更為等同於[!UICONTROL 完成]的狀態，則電子郵件主旨仍會顯示「完成」。</p> </p> <p> 每日摘要通知的主旨為： <em> [!UICONTROL 指派給您的工作摘要] &lt;每日摘要日期&gt; </em></p> </td> 
   <td> <p>任務名稱<br>專案名稱<br>任務參考編號<br>完成任務的使用者名稱<br>完成任務的日期和時間<br>上一個任務狀態<br><strong>[!UICONTROL 檢視更多詳細資料]</strong>按鈕<br>*專案名稱<br>*專案參考編號<br>*完成的任務總數<br>*任務名稱<br>*完成任務的使用者名稱<br>*每日摘要的日期<br></p> </td> 
   <td><strong>每日</strong> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><strong>指派給我的團隊之任務的所有前置任務已完成</strong> </p> <p>當指派團隊的其中一項任務的前置任務被標籤為完成時，該團隊會收到電子郵件通知。</p> <p>擁有「檢閱」或「請求者」授權的使用者不會收到通知。</p> <p>即時通知電子郵件的主旨為： <em>工作完成： &lt;Name&gt;</em></p> <p> 每日摘要通知的主旨為： <em>指派給您的工作摘要&lt;每日摘要日期&gt; </em></p> </td> 
   <td> 任務名稱<br>任務專案<br>任務參考編號<br>完成前置任務的使用者名稱<br>前置任務狀態<br>前置任務完成的日期與時間<br>前置任務的前置任務狀態<br><strong>檢視更多詳細資料</strong>按鈕<br>*專案名稱<br>*專案參考編號<br>*已完成任務的總數<br>*任務名稱<br>*完成任務的使用者名稱<br>*每日摘要的日期 </td>
   <td><strong>即時</strong> </td> 
  </tr>
  <!--
  <tr data-mc-conditions=""> 
   <td> <p><strong>All predecessors of a task assigned to my team are completed</strong> </p> <p>The assigned team receives an email notification when a predecessor of one of their tasks is marked complete.</p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Task Complete: &lt;Name&gt;</em></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
   <td> <p>Assigned by</p> <p>Task Name</p> <p>View button</p> <p>Parent tasks</p> <p>Assignees</p> <p>Task status</p> <p>Task description</p> <p>Task Reference Number</p> <p> <br>Completed predecessor tasks </p> <p>Name of the user who completed the predecessor task<br>Date when the predecessor was completed</p> <p>View button<br>Option to add to the daily digest<br></p> </td> 
   <td><strong>Instant</strong> </td> 
  </tr>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p><strong>All predecessors of a task assigned to my team are completed</strong> </p> <p>The team assigned receives an email notification for each predecessor that is marked complete. </p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Complete: &lt;Task Name&gt;</em><br></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
    <td> Task Name<br>Task Project<br>Task Reference Number<br>Name of the user who completed the predecessor task<br>Status of the predecessor task<br>Date and Time when the predecessor was completed<br>Previous Status of the predecessor task<br><strong>See More Details</strong> button<br>*Project Name<br>*Project Reference Number<br>*Total number of tasks completed<br>*Task Name<br>*Name of the user who completed the task<br>*Date of daily digest </td> 
    <td><strong>Instant</strong> </td> 
   </tr>
  --> 
  <tr> 
   <td> <p><strong>我的任務的所有前置任務已完成</strong> </p> <p>任務受指派人會收到每個已完成前置任務的電子郵件通知。</p> <p>擁有[!UICONTROL Review]或[!UICONTROL Requestor]授權的使用者不會收到通知。</p> <p>即時通知電子郵件的主旨為： <em>[!UICONTROL 完成]： &lt;工作名稱&gt;</em><br></p> <p> 每日摘要通知的主旨為： <em> [!UICONTROL 指派給您的工作摘要] &lt;每日摘要日期&gt; </em></p> </td> 
   <td> 任務名稱<br>任務專案<br>任務參考編號<br>完成前置任務的使用者名稱<br>前置任務狀態<br>前置任務完成的日期和時間<br>前置任務的前置任務狀態<br><strong>[!UICONTROL 檢視更多詳細資料]</strong>按鈕<br>*專案名稱<br>*專案參考編號<br>*已完成任務的總數<br>*任務名稱<br>*完成任務的使用者名稱<br>*每日摘要的日期 </td> 
   <td><strong>即時</strong> </td> 
  </tr>
  <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p><strong>All predecessors of my tasks are completed</strong> </p> <p>The task assignee receives an email notification for each predecessor that is completed.</p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Complete: &lt;Task Name&gt;</em><br></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
    <td> Task Name<br>Task Project<br>Task Reference Number<br>Name of the user who completed the predecessor task<br>Status of the predecessor task<br>Date and Time when the predecessor was completed<br>Previous Status of the predecessor task<br><strong>See More Details</strong> button<br>*Project Name<br>*Project Reference Number<br>*Total number of tasks completed<br>*Task Name<br>*Name of the user who completed the task<br>*Date of daily digest </td> 
    <td><strong>Instant</strong> </td> 
   </tr>
  --> 
  <tr> 
   <td> <p><strong>我解決的問題已核准或已拒絕</strong> </p> <p>當做出核准決定（核准或拒絕）時，問題的受分派者會收到電子郵件通知。</p> <p>擁有[!UICONTROL Review]或[!UICONTROL Requestor]授權的使用者不會收到通知。</p> <p>即時通知電子郵件的主旨為： <em>擱置核准的問題：&lt;計劃開始日期&gt; &lt;問題參考編號&gt; - &lt;問題名稱&gt; （在&lt;專案名稱&gt;</em>中）</p> <p> 每日摘要通知的主旨為： <em>指派給您的工作摘要&lt;每日摘要日期&gt; </em></p> </td> 
   <td> 問題名稱<br>專案名稱<br>問題參考編號<br>核准或拒絕問題的使用者名稱<br>核准決定（已核准或已拒絕）<br>問題狀態<br>要求核准的使用者名稱<br><strong>[!UICONTROL 檢視更多詳細資料]</strong>按鈕<br>*專案名稱<br>*專案參考編號<br>*已核准或拒絕問題的總數<br>*問題名稱<br>*核准或拒絕問題的使用者名稱<br>*核准決定（已批准或已拒絕）<br>*每日摘要的日期<br></td> 
   <td><strong>每日</strong> </td> 
  </tr>
  <tr> 
   <td> <p><strong>指派給我的問題已完成</strong> </p> <p>只有在專案狀態為[!UICONTROL 目前]或[!UICONTROL 規劃]時，才會傳送通知。</p> <p>擁有[!UICONTROL Review]或[!UICONTROL Requestor]授權的使用者不會收到通知。</p> <p>即時通知電子郵件的主旨為： <em>完成： &lt;專案名稱&gt;</em>上的&lt;問題名稱&gt;</p> <p><em>每日摘要通知的主旨為：指派給您的工作摘要&lt;每日摘要日期&gt; </em> </p> </td> 
   <td> 問題名稱<br>專案名稱<br>問題參考編號<br>完成問題的使用者名稱<br>新問題狀態<br>完成問題的日期與時間<br>上一個任務狀態<br><strong>[!UICONTROL 檢視更多詳細資料]</strong>按鈕<br>*專案名稱<br>*專案參考編號<br>*完成的問題總數<br>*問題名稱<br>*完成問題的使用者名稱<br>*每日摘要的日期<br></td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>已根據指派給我的請求上傳或變更檔案</strong> </p> <p>問題受指派人在上傳檔案或就其新增的問題變更檔案詳細資料時，會收到電子郵件通知。</p> <p>如果觸發問題的使用者是問題受指派人，則不會傳送電子郵件通知。</p> <p>僅當專案狀態為[!UICONTROL 目前]且專案已設定為說明要求佇列（如<a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">建立要求佇列</a>中所述）時，才會傳送通知。</p> <p>即時通知電子郵件的主旨為： <em>[!UICONTROL 檔案已新增到] &lt;要求名稱&gt;</em></p> <p> 每日摘要通知的主旨為： <em> [!UICONTROL 指派給您的工作摘要] &lt;每日摘要日期&gt; </em></p> </td> 
   <td> <p>請求名稱<br>專案名稱（請求佇列名稱）<br>檔案參考編號<br>上傳檔案的使用者名稱<br>檔名稱<br>已於日期新增<br>檔案詳細資訊（格式、大小、版本編號）<br>檔案縮圖<br><strong>[!UICONTROL 預覽]</strong>和<strong>[!UICONTROL 下載]</strong>按鈕<br>*專案名稱<br>*專案參考編號<br>*已上傳或已變更的檔案總數<br> *文檔名稱<br>*對象名稱<br>*上傳文檔的使用者的名稱<br>*每日摘要日期</p> </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>指派給我的一項任務的到期日發生變更</strong> </p> <p>任務的[!UICONTROL 規劃完成日期]變更時，任務受指派人會收到電子郵件通知，除非變更規劃完成日期的使用者同時也是任務受指派人。</p> <p>只有當專案狀態不是[!UICONTROL Planning]時，才會傳送通知。</p> <p>不會傳送有關個人工作的通知。</p> <p> 擁有「檢閱」或「請求者」授權的使用者不會收到通知。 </p> <p> 即時通知電子郵件的主旨為： <em>[!UICONTROL 到期日已變更。]</em></p> <p> 每日摘要通知的主旨為： <em> [!UICONTROL 指派給您的工作摘要] &lt;每日摘要日期&gt; </em></p> </td> 
   <td> 任務名稱<br>專案名稱<br>任務參考編號<br>新到期日（[!UICONTROL 計畫完成日期]）<br>到期日變更的日期和時間<br>變更到期日的使用者名稱<br>*專案名稱<br>*專案參考編號<br>*到期日（計畫完成日期）變更的任務總數<br>*任務名稱<br>*新計畫完成日期<br>*變更到期日的使用者名稱<br>*每日摘要日期 </td> 
   <td> <p><strong>即時</strong> </p> <p><strong>和每日</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在指派給我的問題上變更到期日期</strong> </p> <p>除非變更[!UICONTROL 規劃完成日期]的使用者同時也是受指派人，否則問題受指派人會在[!UICONTROL 規劃完成日期]變更時收到電子郵件通知。</p> <p>只有當專案狀態不是[!UICONTROL Planning]時，才會傳送通知。</p> <p>擁有[!UICONTROL Review]或[!UICONTROL Requestor]授權的使用者不會收到通知。</p> <p>即時通知電子郵件的主旨為： <em>[!UICONTROL 到期日已變更]</em></p> <p> </p> <p> 每日摘要通知的主旨為： <em> [!UICONTROL 指派給您的工作摘要] &lt;每日摘要日期&gt;</em></p> </td> 
   <td> <p>問題名稱<br>專案名稱<br>問題參考編號<br>新到期日（[!UICONTROL 計畫完成日期]）<br>到期日變更的日期和時間<br>變更到期日的使用者名稱<br>*專案名稱<br>*專案參考編號<br>*到期日（[!UICONTROL 計畫完成日期]）變更的問題總數<br>*問題名稱<br>*新[!UICONTROL 計畫完成日期]{10&rbrack; 0}*更改每日摘要的截止日期<br>*日期的使用者名稱稱<br><br></p> </td> 
   <td> <p><strong>即時</strong> </p> <p><strong>和每日</strong> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>指派給我的任務狀態已變更</strong> <p>任務受指派人會在任務狀態變更時收到電子郵件通知，除非變更狀態的使用者也是受指派人。</p> <p>注意：當任務狀態變更為完成時，不會傳送此通知。 已完成的作業會使用個別通知。 請參閱上面的<a href="#a-task-i-m-assigned-to-is-completed" class="MCXref xref">指派給我的任務已完成</a>。</p> <p>只有在專案狀態為[!UICONTROL 目前]時，才會傳送通知。</p> <p>擁有[!UICONTROL Review]或[!UICONTROL Requestor]授權的使用者不會收到通知。</p> <p>即時通知電子郵件的主旨是： &lt;專案名稱&gt;中的<em>&lt;任務名稱&gt;是&lt;新狀態&gt;</em></p> <p> </p> <p> 每日摘要通知的主旨為： <em> [!UICONTROL 指派給您的工作摘要] &lt;每日摘要日期&gt; </em></p> </td> 
   <td> 任務名稱<br>專案名稱<br>任務參考編號<br>變更狀態的使用者名稱<br>新狀態<br>狀態變更的日期和時間<br>預覽狀態<br><strong>[!UICONTROL 檢視更多詳細資料]</strong>按鈕<br>*專案名稱<br>*專案參考編號<br>*狀態變更的任務總數<br>*任務名稱<br>*先前的任務狀態<br>*新任務狀態<br>*名稱更改每日摘要狀態<br>*日期的使用者<br></td> 
   <td><strong>[!UICONTROL 每日]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我其中一個工作專案的狀態變更</strong> </p> <p>除非您自行變更狀態，否則當您受指派問題的狀態變更時，您會收到電子郵件通知。 </p> <p>只有在專案狀態為[!UICONTROL 目前]時，才會傳送通知。</p> <p>擁有[!UICONTROL Review]或[!UICONTROL Requestor]授權的使用者不會收到通知。</p> <p>即時通知電子郵件的主旨是： &lt;專案名稱&gt;中的<em>&lt;問題名稱&gt;是&lt;新狀態&gt;</em></p> <p> 每日摘要通知的主旨為： <em> [!UICONTROL 指派給您的工作摘要] &lt;每日摘要日期&gt; </em></p> </td> 
   <td> 問題名稱<br>專案名稱<br>問題參考編號<br>變更狀態的使用者名稱<br>新狀態<br>狀態變更的日期和時間<br>上一個問題狀態<br><strong>檢視更多詳細資料</strong>按鈕<br>*專案名稱<br>*專案參考編號<br>*狀態變更的問題總數<br>*任務名稱<br>*上一個問題狀態<br>*新問題狀態<br>*狀態變更的使用者名稱<br> 15&rbrace;*每日摘要日期 </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
 </tbody> 
</table>
