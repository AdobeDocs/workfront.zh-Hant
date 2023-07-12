---
content-type: reference
navigation-topic: notifications
title: 「通知：指派給我的工作相關資訊」
description: 以下通知會提醒您有關工作專案上發生指派給您的活動。
author: Lisa
feature: Get Started with Workfront
exl-id: 5d7fdee8-cb5c-4ab8-bec3-beff9851b8f6
source-git-commit: 901605917347297a1ee077f00905b03427582650
workflow-type: tm+mt
source-wordcount: '2090'
ht-degree: 6%

---

# 通知：指派給我的工作相關資訊

以下通知會提醒您有關工作專案上發生指派給您的活動。

如需有關設定您會收到哪些通知的資訊，請參閱 [啟用或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

另請參閱 [事件通知](../../workfront-basics/using-notifications/event-notifications.md).

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
   <td> <p><strong>一個指派給我的團隊之任務的前置任務已完成</strong> </p> <p>當指派團隊的其中一項任務的前置任務完成時，指派團隊會收到電子郵件通知。 </p> <p>擁有[！UICONTROL Review]或[！UICONTROL Requestor]授權的使用者不會收到通知。</p> <p>即時通知電子郵件的主旨為： <em>完成： &lt;task name=""&gt;</em></p> <p> 每日摘要通知的主題是： <em> [！UICONTROL指派給您的工作摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>前置任務名稱<br>前置任務專案<br>前置任務參考號碼<br>完成前置任務的使用者名稱<br>前置任務狀態<br>前置任務完成的日期與時間<br>前置任務的前一狀態<br><strong>檢視更多詳細資料</strong> 按鈕<br>*專案名稱<br>*專案參考編號<br>*已完成的前置任務總數<br>*任務名稱<br>*完成任務的使用者名稱<br>*每日摘要日期 </p> </td> 
   <td><strong>每日</strong> </td>
  </tr>
  <tr> 
   <td> <p><strong>我的其中一項任務的前置任務已完成</strong> </p> <p>當任務受指派人的其中一項任務的前置任務完成時，任務受指派人會收到電子郵件通知。 </p> <p>擁有[！UICONTROL Review]或[！UICONTROL Requestor]授權的使用者不會收到通知。</p> <p>即時通知電子郵件的主旨為： <em>[！UICONTROL完成]： &lt;task name=""&gt;</em></p> <p> 每日摘要通知的主題是： <em> [！UICONTROL指派給您的工作摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>前置任務名稱<br>前置任務專案<br>前置任務參考號碼<br>完成前置任務的使用者名稱<br>前置任務狀態<br>前置任務完成的日期與時間<br>前置任務的前一狀態<br><strong>[！UICONTROL檢視更多詳細資料]</strong> 按鈕<br>*專案名稱<br>*專案參考編號<br>*已完成的前置任務總數<br>*任務名稱<br>*完成任務的使用者名稱<br>*每日摘要日期 </p> </td> 
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
   <td> <p><strong>我要完成的一項任務已核准或已拒絕</strong> </p> <p>當任務被核准或拒絕時，任務受指派人會收到電子郵件通知。</p> <p>只有在專案狀態為「目前」時，才會傳送通知。</p> <p>擁有[！UICONTROL Review]或[！UICONTROL Requestor]授權的使用者不會收到通知。</p> <p>即時通知電子郵件的主旨為： <em>[！UICONTROL完成]： &lt;task name=""&gt; 於 &lt;project name=""&gt;</em></p> <p> 每日摘要通知的主題是： <em> [！UICONTROL指派給您的工作摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 任務名稱<br>專案名稱<br>任務參考號碼<br>授予核准的使用者名稱<br>新任務狀態<br>核准或拒絕任務的日期與時間<br>上一個任務狀態<br><strong>[！UICONTROL檢視更多詳細資料]</strong> 按鈕<br>*專案名稱<br>*專案參考編號<br>*已核准或已拒絕的任務總數<br>*任務名稱<br>*核准或拒絕任務的使用者名稱<br>*核准決定（[！UICONTROL已核准]/[！UICONTROL已拒絕]）<br>*每日摘要的日期<br></td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p id="a-task-i-m-assigned-to-is-completed"><strong>指派給我的一項任務已完成</strong> </p> <p>任務受指派人在任務完成時收到電子郵件通知。</p> <p>只有在專案狀態為[！UICONTROL目前]時，才會傳送通知。</p> <p>擁有[！UICONTROL Review]或[！UICONTROL Requestor]授權的使用者不會收到通知。</p> <p>即時通知電子郵件的主旨為： <em>[！UICONTROL完成]： &lt;task name=""&gt; 於 &lt;project name=""&gt;</em></p> <p> <p>注意：如果任務變更為等同於[！UICONTROL完成]的狀態，則電子郵件主旨仍會顯示「完成」。</p> </p> <p> 每日摘要通知的主題是： <em> [！UICONTROL指派給您的工作摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>任務名稱<br>專案名稱<br>任務參考號碼<br>完成任務的使用者名稱<br>工作完成的日期與時間<br>上一個任務狀態<br><strong>[！UICONTROL檢視更多詳細資料]</strong> 按鈕<br>*專案名稱<br>*專案參考編號<br>*已完成的任務總數<br>*任務名稱<br>*完成任務的使用者名稱<br>*每日摘要的日期<br></p> </td> 
   <td><strong>每日</strong> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><strong>所有指派給我的團隊之任務的前置任務皆已完成</strong> </p> <p>當指派團隊中某一項任務的前置任務被標籤為完成時，該團隊會收到電子郵件通知。</p> <p>擁有檢閱或請求者授權的使用者不會收到通知。</p> <p>即時通知電子郵件的主旨為： <em>任務完成： &lt;name&gt;</em></p> <p> 每日摘要通知的主題是： <em> 指派給您的工作摘要 &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 任務名稱<br>任務專案<br>任務參考號碼<br>完成前置任務的使用者名稱<br>前置任務狀態<br>前置任務完成的日期與時間<br>前置任務的前一狀態<br><strong>檢視更多詳細資料</strong> 按鈕<br>*專案名稱<br>*專案參考編號<br>*已完成的任務總數<br>*任務名稱<br>*完成任務的使用者名稱<br>*每日摘要日期 </td>
   <td><strong>立即</strong> </td> 
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
   <td> <p><strong>我的任務之所有前置任務已完成</strong> </p> <p>任務受指派人會收到每個已完成前置任務的電子郵件通知。</p> <p>擁有[！UICONTROL Review]或[！UICONTROL Requestor]授權的使用者不會收到通知。</p> <p>即時通知電子郵件的主旨為： <em>[！UICONTROL完成]： &lt;task name=""&gt;</em><br></p> <p> 每日摘要通知的主題是： <em> [！UICONTROL指派給您的工作摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 任務名稱<br>任務專案<br>任務參考號碼<br>完成前置任務的使用者名稱<br>前置任務狀態<br>前置任務完成的日期與時間<br>前置任務的前一狀態<br><strong>[！UICONTROL檢視更多詳細資料]</strong> 按鈕<br>*專案名稱<br>*專案參考編號<br>*已完成的任務總數<br>*任務名稱<br>*完成任務的使用者名稱<br>*每日摘要日期 </td> 
   <td><strong>立即</strong> </td> 
  </tr>
  <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p><strong>All predecessors of my tasks are completed</strong> </p> <p>The task assignee receives an email notification for each predecessor that is completed.</p> <p>Users with a Review or Requestor license do not receive a notification.</p> <p>The subject of the instant notification email is: <em>Complete: &lt;Task Name&gt;</em><br></p> <p> The subject of the daily digest notification is: <em> Digest of Work Assigned to You &lt;Date of daily digest&gt; </em></p> </td> 
    <td> Task Name<br>Task Project<br>Task Reference Number<br>Name of the user who completed the predecessor task<br>Status of the predecessor task<br>Date and Time when the predecessor was completed<br>Previous Status of the predecessor task<br><strong>See More Details</strong> button<br>*Project Name<br>*Project Reference Number<br>*Total number of tasks completed<br>*Task Name<br>*Name of the user who completed the task<br>*Date of daily digest </td> 
    <td><strong>Instant</strong> </td> 
   </tr>
  --> 
  <tr> 
   <td> <p><strong>我要解決的問題已核准或已拒絕</strong> </p> <p>當做出核准決定（核准或拒絕）時，問題的受分派者會收到電子郵件通知。</p> <p>擁有[！UICONTROL Review]或[！UICONTROL Requestor]授權的使用者不會收到通知。</p> <p>即時通知電子郵件的主旨為： <em>未決核准問題： &lt;planned start="" date=""&gt; &lt;issue reference="" number=""&gt; - &lt;issue name=""&gt; 在 &lt;project name=""&gt;</em></p> <p> 每日摘要通知的主題是： <em> 指派給您的工作摘要 &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 問題名稱<br>專案名稱<br>問題參考號碼<br>核准或拒絕問題的使用者名稱<br>核准決定（已核准或已拒絕）<br>問題狀態<br>要求核准的使用者名稱<br><strong>[！UICONTROL檢視更多詳細資料]</strong> 按鈕<br>*專案名稱<br>*專案參考編號<br>*已核准或已拒絕的問題總數<br>*問題名稱<br>*核准或拒絕問題的使用者名稱<br>*核准決定（已核准或已拒絕）<br>*每日摘要的日期<br></td> 
   <td><strong>每日</strong> </td> 
  </tr>
  <tr> 
   <td> <p><strong>指派給我的一個問題已完成</strong> </p> <p>只有在專案狀態為[！UICONTROL目前]或[！UICONTROL規劃]時，才會傳送通知。</p> <p>擁有[！UICONTROL Review]或[！UICONTROL Requestor]授權的使用者不會收到通知。</p> <p>即時通知電子郵件的主旨為： <em>完成： &lt;issue name=""&gt; 於 &lt;project name=""&gt;</em></p> <p><em> 每日摘要通知的主題是：指派給您的工作摘要 &lt;date of="" daily="" digest=""&gt; </em> </p> </td> 
   <td> 問題名稱<br>專案名稱<br>問題參考號碼<br>完成問題的使用者名稱<br>新問題狀態<br>問題完成的日期和時間<br>上一個任務狀態<br><strong>[！UICONTROL檢視更多詳細資料]</strong> 按鈕<br>*專案名稱<br>*專案參考編號<br>*已完成的問題總數<br>*問題名稱<br>*完成問題的使用者名稱<br>*每日摘要的日期<br></td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>根據我的請求上傳或變更了文件</strong> </p> <p>問題受指派人在上傳檔案或變更其所新增問題的檔案詳細資料時，會收到電子郵件通知。</p> <p>如果觸發問題的使用者是問題受指派人，則不會傳送電子郵件通知。</p> <p>僅當專案狀態為[！UICONTROL目前]且專案已設定為「說明請求佇列」（如所述）時，才會傳送通知 <a href="../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">建立請求佇列</a>)。</p> <p>即時通知電子郵件的主旨為： <em>[！UICONTROL檔案已新增至] &lt;request name=""&gt;</em></p> <p> 每日摘要通知的主題是： <em> [！UICONTROL指派給您的工作摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>請求名稱<br>專案名稱（請求佇列名稱）<br>檔案參考編號 <br>上傳檔案的使用者名稱<br>檔名稱 <br>新增日期<br>檔案詳細資訊（格式、大小、版本號碼）<br>檔案縮圖<br><strong>[！UICONTROL預覽]</strong> 和 <strong>[！UICONTROL下載]</strong> 按鈕<br>*專案名稱<br>*專案參考編號<br>*已上傳或已變更的檔案總數<br>*檔名稱<br>*物件名稱<br>*上傳檔案的使用者名稱<br>*每日摘要日期</p> </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在指派給我的一項任務上變更了到期日期</strong> </p> <p>任務受指派人會在任務的[！UICONTROL規劃完成日期]變更時收到電子郵件通知，除非變更規劃完成日期的使用者同時也是任務受指派人。</p> <p>只有當專案狀態不是[！UICONTROL Planning]時，才會傳送通知。</p> <p>不會傳送有關個人工作的通知。</p> <p> 擁有檢閱或請求者授權的使用者不會收到通知。 </p> <p> 即時通知電子郵件的主旨為： <em>[！UICONTROL到期日期已變更。]</em></p> <p> 每日摘要通知的主題是： <em> [！UICONTROL指派給您的工作摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 任務名稱<br>專案名稱<br>任務參考號碼<br>新的到期日（[！UICONTROL計畫完成日期]）<br>到期日變更的日期與時間<br>變更到期日期的使用者名稱<br>*專案名稱<br>*專案參考編號<br>*到期日（計畫完成日期）變更的任務總數<br>*任務名稱<br>*新的計畫完成日期<br>*變更「到期日」的使用者名稱<br>*每日摘要日期 </td> 
   <td> <p><strong>立即</strong> </p> <p><strong>和每日</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在指派給我的問題上變更到期日期</strong> </p> <p>除非變更[！UICONTROL規劃完成日期]的使用者同時也是受指派人，否則問題受指派人會在[！UICONTROL規劃完成日期]變更時收到電子郵件通知。</p> <p>只有當專案狀態不是[！UICONTROL Planning]時，才會傳送通知。</p> <p>擁有[！UICONTROL Review]或[！UICONTROL Requestor]授權的使用者不會收到通知。</p> <p>即時通知電子郵件的主旨為： <em>[！UICONTROL到期日期已變更]</em></p> <p> </p> <p> 每日摘要通知的主題是： <em> [！UICONTROL指派給您的工作摘要] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>問題名稱<br>專案名稱<br>問題參考號碼<br>新的到期日（[！UICONTROL計畫完成日期]）<br>到期日變更的日期與時間<br>變更到期日期的使用者名稱<br>*專案名稱<br>*專案參考編號<br>*到期日（[！UICONTROL規劃完成日期]）變更的問題總數<br>*問題名稱<br>*新[！UICONTROL規劃完成日期]<br>*變更「到期日」的使用者名稱<br>*每日摘要的日期<br></p> </td> 
   <td> <p><strong>立即</strong> </p> <p><strong>和每日</strong> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>一項指派給我的任務狀態發生變更</strong> <p>任務狀態變更時，「任務受指派人」會收到電子郵件通知，除非變更狀態的使用者同時也是受指派人。</p> <p>注意：當任務狀態變更為完成時，不會傳送此通知。 已完成的任務會使用個別通知。 另請參閱 <a href="#a-task-i-m-assigned-to-is-completed" class="MCXref xref">指派給我的一項任務已完成</a>，以上的。</p> <p>只有在專案狀態為[！UICONTROL目前]時，才會傳送通知。</p> <p>擁有[！UICONTROL Review]或[！UICONTROL Requestor]授權的使用者不會收到通知。</p> <p>即時通知電子郵件的主旨為： <em>&lt;task name=""&gt; 從 &lt;project name=""&gt; 是 &lt;new status=""&gt;</em></p> <p> </p> <p> 每日摘要通知的主題是： <em> [！UICONTROL指派給您的工作摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 任務名稱<br>專案名稱<br>任務參考號碼<br>變更狀態的使用者名稱<br>新狀態<br>狀態變更的日期和時間<br>預覽狀態<br><strong>[！UICONTROL檢視更多詳細資料]</strong> 按鈕<br>*專案名稱<br>*專案參考編號<br>*狀態已變更的任務總數<br>*任務名稱<br>*上一個任務狀態<br>*新任務狀態<br>*變更「狀態」的使用者名稱<br>*每日摘要的日期<br></td> 
   <td><strong>[！UICONTROL每日]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我的工作項目之一的狀態變更</strong> </p> <p>除非您自行變更狀態，否則當您受指派問題的狀態變更時，您會收到電子郵件通知。 </p> <p>只有在專案狀態為[！UICONTROL目前]時，才會傳送通知。</p> <p>擁有[！UICONTROL Review]或[！UICONTROL Requestor]授權的使用者不會收到通知。</p> <p>即時通知電子郵件的主旨為： <em>&lt;issue name=""&gt; 從 &lt;project name=""&gt; 是 &lt;new status=""&gt;</em></p> <p> 每日摘要通知的主題是： <em> [！UICONTROL指派給您的工作摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 問題名稱<br>專案名稱<br>問題參考號碼<br>變更狀態的使用者名稱<br>新狀態<br>狀態變更的日期和時間<br>上一個問題狀態<br><strong>檢視更多詳細資料</strong> 按鈕<br>*專案名稱<br>*專案參考編號<br>*狀態變更的問題總數<br>*任務名稱<br>*上一個問題狀態<br>*新問題狀態<br>*變更「狀態」的使用者名稱<br>*每日摘要日期 </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
 </tbody> 
</table>
