---
content-type: reference
navigation-topic: notifications
title: 「通知：關於我擁有的專案資訊」
description: 下列通知會提醒您擁有的專案中發生活動。 如需有關設定您收到哪些通知的資訊，請參閱修改您自己的電子郵件通知。
author: Lisa
feature: Get Started with Workfront
exl-id: cf605849-bcc0-4982-b8fa-f69eef7a4fb6
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1709'
ht-degree: 6%

---

# 通知：關於我擁有的專案資訊

下列通知會提醒您擁有的專案中發生活動。 如需有關設定您接收哪些通知的資訊，請參閱 [修改您自己的電子郵件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>我擁有的專案中新增了一個文件</strong> </p> <p>除非新增檔案的使用者也是專案所有者，否則當檔案新增至專案時，專案所有者會收到電子郵件通知。</p> <p>只有在專案狀態為[！UICONTROL目前]且檔案不是「私人」時，才會傳送通知。</p> <p>即時通知電子郵件的主旨為： <em>[！UICONTROL檔案已新增到] &lt;project name=""&gt;</em></p> <p> 每日摘要通知的主題為： <em> [！UICONTROL您擁有的專案摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 專案名稱<br>Portfolio名稱<br>專案參考號碼<br>新增檔案的使用者名稱<br>檔名稱<br>新增日期<br>檔案詳細資訊（格式、大小、版本號碼）<br><strong>[！UICONTROL預覽]</strong> 和 <strong>[！UICONTROL下載]</strong> 按鈕<br>*專案名稱<br>*專案參考編號<br>*新增的檔案總數<br>*檔名稱<br>*新增檔案的使用者名稱<br>*每日摘要的日期<br></td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我擁有的專案中有一項里程碑任務已完成</strong> </p> <p>只有在專案狀態為[！UICONTROL目前]或[！UICONTROL規劃]時，才會傳送通知。</p> <p>即時通知電子郵件的主旨為： <em>[！UICONTROL完成]： &lt;task name=""&gt; 於 &lt;project name=""&gt;</em></p> <p>注意：如果任務變更為等於[！UICONTROL完成]的狀態，則電子郵件主旨仍會顯示「[！UICONTROL完成]」。</p> <p> 每日摘要通知的主題為： <em> [！UICONTROL您擁有的專案摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 任務名稱<br>專案名稱<br>任務參考號碼<br>完成任務的使用者名稱<br>新任務狀態<br>工作完成的日期與時間<br>前一個任務狀態<br><strong>[！UICONTROL檢視更多詳細資料]</strong> 按鈕<br>*專案名稱<br>*專案參考編號<br>*已完成的任務總數<br>*任務名稱<br>*完成任務的使用者名稱<br>*每日摘要日期 </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我擁有的一項專案進度落後</strong> </p> <p>當專案進度落後時，專案所有者會收到電子郵件通知。 當進度狀態為「[！UICONTROL有風險]」、「[！UICONTROL落後]」或「[！UICONTROL延遲]」時，專案進度落後。</p> <p>最佳實務建議將此通知保持作用中。 </p> <p>擁有[！UICONTROL Review]授權的使用者不會收到通知。</p> <p>即時通知電子郵件的主旨為： <em>[！UICONTROL專案進度變更]： &lt;project name=""&gt;</em></p> <p> 每日摘要通知的主題為： <em> [！UICONTROL您擁有的專案摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>專案名稱<br>Portfolio名稱<br>專案參考號碼<br>專案進度狀態<br>專案[！UICONTROL計劃開始日期]<br>專案[！UICONTROL計畫完成日期]<br>專案[！UICONTROL預計開始日期]<br>專案[！UICONTROL預計完成日期]<br>專案完成百分比<br>專案狀態<br>專案所有者<br>*專案名稱<br>*專案參考編號<br>*專案進度狀態<br>*每日摘要的日期<br></p> </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我擁有的專案中新增了一個問題</strong> </p> <p>將問題新增到專案時，專案所有者會收到電子郵件通知。</p> <p>只有在專案狀態為[！UICONTROL目前]或[！UICONTROL規劃]時，才會傳送通知。</p> <p>即時通知電子郵件的主旨為： <em>[！UICONTROL問題已新增到] &lt;project name=""&gt;</em></p> <p> </p> <p> 每日摘要通知的主題為： <em> [！UICONTROL您擁有的專案摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>專案名稱<br>Portfolio名稱<br>問題參考號碼<br>新增問題的使用者名稱<br>問題名稱<br>問題型別<br>輸入日期<br>問題優先順序<br>指派至名稱 <br>問題狀態<br>主要連絡人<br>*專案名稱<br>*專案參考編號<br>*新增至專案的問題總數<br>*問題名稱<br>*新增問題的使用者名稱<br>*每日摘要日期</p> </td> 
   <td> <p><strong>立即</strong> </p> <p><strong>和每日</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我擁有的專案中有一項任務已完成</strong> </p> <p>專案所有者會在專案上完成任務時收到通知。</p> <p>只有在專案狀態為[！UICONTROL目前]時，才會傳送通知。</p> <p>即時通知電子郵件的主旨為： <em>[！UICONTROL完成]： &lt;task name=""&gt; 於 &lt;project name=""&gt;</em></p> <p> <p>注意：如果任務變更為等於[！UICONTROL完成]的狀態，則電子郵件主旨仍會顯示「[！UICONTROL完成]」。</p> </p> <p> 每日摘要通知的主題為： <em> [！UICONTROL您擁有的專案摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 任務名稱<br>專案名稱<br>任務參考號碼<br>完成任務的使用者名稱 <br>任務狀態<br>完成工作的日期與時間<br>前一個任務狀態<br><strong>[！UICONTROL檢視更多詳細資料]</strong> 按鈕<br>*專案名稱<br>*專案參考編號<br>*已完成的任務總數 <br>*任務名稱<br>*完成任務的使用者名稱<br>*每日摘要的日期<br></td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我擁有的專案中有一項任務進度落後</strong> </p> <p>專案上的任務進度落後時，專案所有者會收到電子郵件通知。 當進度狀態為「[！UICONTROL有風險]」、「[！UICONTROL落後]」或「[！UICONTROL延遲]」時，任務進度落後。</p> <p>只有在專案狀態為[！UICONTROL目前]時，才會傳送通知。</p> <p>即時通知電子郵件的主旨為： <em>[！UICONTROL任務進度變更]： &lt;task name=""&gt;</em></p> <p> 每日摘要通知的主題為： <em> [！UICONTROL您擁有的專案摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 任務名稱<br>專案名稱<br>任務參考號碼<br>新任務進度狀態<br>任務[！UICONTROL計劃開始日期]<br>任務[！UICONTROL計畫完成日期]<br>任務[！UICONTROL預計開始日期]<br>任務[！UICONTROL預計完成日期]<br>任務完成百分比<br>任務狀態<br>指派至名稱<br>依名稱輸入<br>*專案名稱<br>*專案參考編號<br>*排程較後的任務總數<br>*任務名稱<br>*指派至名稱<br>*每日摘要日期 </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我擁有的專案中有一個問題完成了</strong> </p> <p>專案所有者的專案問題完成時，專案所有者會收到電子郵件通知。</p> <p>只有在專案狀態為[！UICONTROL目前]或[！UICONTROL規劃]時，才會傳送通知。</p> <p>擁有[！UICONTROL Review]授權的使用者不會收到通知。 </p> <p>即時通知電子郵件的主旨為： <em>[！UICONTROL完成]： &lt;issue name=""&gt; 於 &lt;project name=""&gt;</em></p> <p> 每日摘要通知的主題為： <em> [！UICONTROL您擁有的專案摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 問題名稱<br>專案名稱<br>問題參考號碼<br>完成問題的使用者名稱<br>問題狀態<br>完成問題的日期與時間<br>上一個問題狀態<br><strong>[！UICONTROL檢視更多詳細資料]</strong> 按鈕 <br>*專案名稱<br>*專案參考編號<br>*已完成的問題總數<br>*問題名稱<br>*指派給問題的使用者名稱<br>*每日摘要的日期<br></td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我擁有的專案中新增了一個未指派的問題</strong> </p> <p>當未指派的問題新增到專案時，專案所有者會收到電子郵件通知。</p> <p>只有在專案狀態為[！UICONTROL目前]或[！UICONTROL規劃]時，才會傳送通知。</p> <p>即時通知電子郵件的主旨為： <em>[！UICONTROL應該指派給此新問題的人員於] &lt;project name=""&gt;？</em></p> <p> </p> <p> 每日摘要通知的主題為： <em> 您擁有的專案摘要 &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>專案名稱<br>Portfolio名稱<br>問題參考號碼<br>新增問題的使用者名稱<br>問題名稱<br>問題型別<br>輸入日期<br>問題優先順序<br>指派至名稱（空白）<br>問題狀態<br>主要連絡人<br>*專案名稱<br>*專案參考編號<br>*新增的問題總數<br>*問題名稱<br>*新增問題的使用者名稱<br>*每日摘要的日期<br></p> </td> 
   <td> <p><strong>立即</strong> </p> <p><strong>和每日</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我被設為新專案的擁有者</strong> </p> <p>當使用者被指派為專案的所有者時，該使用者會收到電子郵件通知。</p> <p>如果專案所有者是進行指派的相同使用者，則不會傳送電子郵件通知。</p> <p>擁有[！UICONTROL Review]授權的使用者不會收到通知。</p> <p>因為正在將他們指派給某些專案，所以請開啟此專案。 </p> <p> 指派某專案、共用某專案、取得某專案的存取權。</p> <p>即時通知電子郵件的主旨為： <em>[！UICONTROL您現在是]的專案所有者 &lt;project name=""&gt;</em></p> <p>電子郵件通知內文包含下列文字：<em><br></em></p> <p><em>[！UICONTROL Hi] &lt;your name=""&gt;，<br></em><em>&lt;name of="" the="" user="" who="" assigned="" you="" as="" the="" project="" owner=""&gt; [！UICONTROL讓您成為] &lt;project name=""&gt;. [！UICONTROL身為專案所有者，您可能會收到關於專案活動的其他電子郵件通知、需要核准專案的時數或參與專案相關的核准工作。 全部都歸你了。]</em> </p> <p> 每日摘要通知的主題為： <em> [！UICONTROL您擁有的專案摘要] &lt;date of="" daily="" digest=""&gt; </em></p> <p> </p> </td> 
   <td> <p>專案名稱<br>Portfolio名稱<br>專案參考號碼<br>專案完成日期<br>*專案名稱<br>*專案參考編號<br>*每日摘要日期</p> </td> 
   <td><strong>立即</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我的專案中有一項任務的提交日期發生變更</strong> </p> <p>當專案上任務的「認可日期」變更時，專案所有者會收到電子郵件通知，除非變更「認可日期」的使用者同時也是專案所有者。</p> <p>即時通知電子郵件的主旨為： <em>[！UICONTROL Commit date for] &lt;task name=""&gt; [！UICONTROL現在是] &lt;new commit="" date=""&gt;</em></p> <p> 每日摘要通知的主題為： <em> 您擁有的專案摘要 &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>任務名稱<br>專案名稱<br>任務參考號碼<br>變更認可日期的使用者名稱<br>新認可日期<br>任務[！UICONTROL計畫完成日期]<br>此變更對專案時間表的影響資訊<br>指派至名稱<br>依名稱輸入<br>專案所有者<br><strong>[！UICONTROL檢視更多詳細資料]</strong> 按鈕<br>*專案名稱<br>*專案參考編號<br>*認可日期已變更的任務總數<br>*任務名稱<br>*每日摘要的日期<br></p> </td> 
   <td> <p><strong>立即</strong> </p> <p><strong>和[！UICONTROL Daily]</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我的專案中有一個問題的提交日期發生變更</strong> </p> <p>當專案的問題認可日期變更時，專案所有者會收到電子郵件通知，除非變更認可日期的使用者與專案所有者的使用者相同。</p> <p>即時通知電子郵件的主旨為： <em>[！UICONTROL Commit date for] &lt;issue name=""&gt; [！UICONTROL現在是] &lt;new commit="" date=""&gt;</em></p> <p> 每日摘要通知的主題為： <em> [！UICONTROL您擁有的專案摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>問題名稱<br>專案名稱<br>問題參考號碼<br>變更認可日期的使用者名稱<br>新認可日期<br>問題計畫完成日期<br>指派至名稱<br>依名稱輸入<br>專案所有者<br><strong>[！UICONTROL檢視更多詳細資料]</strong> 按鈕<br>*專案名稱<br>*專案參考編號<br>*認可日期已變更的問題總數<br>*問題名稱<br>*每日摘要的日期<br></p> </td> 
   <td> <p><strong>立即</strong> </p> <p><strong>和[！UICONTROL Daily]</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
