---
content-type: reference
navigation-topic: notifications
title: '''通知：我擁有的專案的相關資訊'
description: 下列通知會提醒您留意您擁有之專案中發生的活動。 如需設定您收到哪些通知的相關資訊，請參閱啟用或停用您自己的事件通知。
author: Lisa
feature: Get Started with Workfront
exl-id: cf605849-bcc0-4982-b8fa-f69eef7a4fb6
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '1713'
ht-degree: 6%

---

# 通知：我擁有之專案的相關資訊

下列通知會提醒您留意您擁有之專案中發生的活動。 如需設定您收到哪些通知的詳細資訊，請參閱 [啟用或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

另請參閱 [事件通知](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>通知</th> 
   <th> <p>包含的欄位 </p> <p> *僅限每日摘要欄位</p> </th> 
   <th>預設狀態</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>向我持有的專案新增一個文件</strong> </p> <p>將文檔添加到項目時，項目所有者將收到電子郵件通知，除非添加文檔的用戶也是項目所有者。</p> <p>僅當項目狀態為[!UICONTROL Current]且文檔不為「專用」時，才會發送通知。</p> <p>即時通知電子郵件的主旨是： <em>[!UICONTROL文檔已添加到] &lt;project name=""&gt;</em></p> <p> 每日摘要通知的主旨是： <em> [!UICONTROL您擁有的項目摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 專案名稱<br>Portfolio名稱<br>項目參考編號<br>添加文檔的用戶的名稱<br>文檔名稱<br>新增日期<br>文檔詳細資訊（格式、大小、版本號）<br><strong>[!UICONTROL預覽]</strong> 和 <strong>[!UICONTROL下載]</strong> 按鈕<br>*專案名稱<br>*項目參考編號<br>*新增的檔案總數<br>*文檔名稱<br>*新增檔案的使用者名稱<br>*每日摘要日期<br></td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在我持有的專案上完成了里程碑任務</strong> </p> <p>僅當項目狀態為[!UICONTROL Current]或[!UICONTROL Planning]時，才會發送通知。</p> <p>即時通知電子郵件的主旨是： <em>[!UICONTROL完成]: &lt;task name=""&gt; on &lt;project name=""&gt;</em></p> <p>注意：如果任務更改為相當於[!UICONTROL Complete]的狀態，則電子郵件的主題仍顯示「[!UICONTROL Complete]」。</p> <p> 每日摘要通知的主旨是： <em> [!UICONTROL您擁有的項目摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 任務名稱<br>專案名稱<br>任務參考編號<br>完成任務的用戶名<br>新任務狀態<br>任務完成的日期和時間<br>上一任務狀態<br><strong>[!UICONTROL查看更多詳細資訊]</strong> 按鈕<br>*專案名稱<br>*項目參考編號<br>*已完成任務總數<br>*任務名稱<br>*完成任務的用戶名<br>*每日摘要日期 </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我持有的專案落後</strong> </p> <p>專案擁有者會在專案延遲時收到電子郵件通知。 當進度狀態為「[!UICONTROL At Risk]」、「[!UICONTROL Bethin]」或「[!UICONTROL Late]」時，項目將落後於計畫。</p> <p>最佳實務是保持此通知作用中。 </p> <p>擁有[!UICONTROL Review]授權的使用者不會收到通知。</p> <p>即時通知電子郵件的主旨是： <em>[!UICONTROL項目進度更改]: &lt;project name=""&gt;</em></p> <p> 每日摘要通知的主旨是： <em> [!UICONTROL您擁有的項目摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>專案名稱<br>Portfolio名稱<br>項目參考編號<br>項目進度狀態<br>項目[!UICONTROL計劃開始日期]<br>項目[!UICONTROL計畫完成日期]<br>專案[!UICONTROL預計開始日期]<br>項目[!UICONTROL預計完成日期]<br>項目完成百分比<br>專案狀態<br>專案擁有者<br>*專案名稱<br>*項目參考編號<br>*項目進度狀態<br>*每日摘要日期<br></p> </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>向我持有的專案新增了一個問題</strong> </p> <p>將問題新增至專案時，專案擁有者會收到電子郵件通知。</p> <p>僅當項目狀態為[!UICONTROL Current]或[!UICONTROL Planning]時，才會發送通知。</p> <p>即時通知電子郵件的主旨是： <em>[!UICONTROL問題已添加到] &lt;project name=""&gt;</em></p> <p> </p> <p> 每日摘要通知的主旨是： <em> [!UICONTROL您擁有的項目摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>專案名稱<br>Portfolio名稱<br>問題參考編號<br>新增問題的使用者名稱<br>問題名稱<br>問題類型<br>輸入日期<br>問題優先順序<br>指派給名稱 <br>問題狀態<br>主要連絡人<br>*專案名稱<br>*項目參考編號<br>*專案新增的問題總數<br>*問題名稱<br>*新增問題的使用者名稱<br>*每日摘要日期</p> </td> 
   <td> <p><strong>立即</strong> </p> <p><strong>和每日</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在我持有的專案上完成了一項任務</strong> </p> <p>專案擁有者在其專案上完成工作時會收到通知。</p> <p>只有在專案狀態為[!UICONTROL目前]時，才會傳送通知。</p> <p>即時通知電子郵件的主旨是： <em>[!UICONTROL完成]: &lt;task name=""&gt; on &lt;project name=""&gt;</em></p> <p> <p>注意：如果任務更改為相當於[!UICONTROL Complete]的狀態，則電子郵件的主題仍顯示「[!UICONTROL Complete]」。</p> </p> <p> 每日摘要通知的主旨是： <em> [!UICONTROL您擁有的項目摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 任務名稱<br>專案名稱<br>任務參考編號<br>完成任務的用戶名 <br>任務狀態<br>任務完成的日期和時間<br>上一任務狀態<br><strong>[!UICONTROL查看更多詳細資訊]</strong> 按鈕<br>*專案名稱<br>*項目參考編號<br>*已完成任務總數 <br>*任務名稱<br>*完成任務的用戶名<br>*每日摘要日期<br></td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我持有專案上的一項任務落後</strong> </p> <p>專案擁有者會在專案上的任務落後時收到電子郵件通知。 當進度狀態為「[!UICONTROL At Risk]」或「[!UICONTROL Bethin]」或「[!UICONTROL Late]」時，任務將滯後於計畫。</p> <p>只有在專案狀態為[!UICONTROL目前]時，才會傳送通知。</p> <p>即時通知電子郵件的主旨是： <em>[!UICONTROL任務進度更改]: &lt;task name=""&gt;</em></p> <p> 每日摘要通知的主旨是： <em> [!UICONTROL您擁有的項目摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 任務名稱<br>專案名稱<br>任務參考編號<br>新任務進度狀態<br>任務[!UICONTROL計劃開始日期]<br>任務[!UICONTROL計畫完成日期]<br>任務[!UICONTROL預計開始日期]<br>任務[!UICONTROL預計完成日期]<br>任務完成百分比<br>任務狀態<br>指派給名稱<br>按名稱輸入<br>*專案名稱<br>*項目參考編號<br>*延遲的任務總數<br>*任務名稱<br>*已分配給名稱<br>*每日摘要日期 </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在我持有的專案上完成了一個問題</strong> </p> <p>專案擁有者在專案上完成問題時，會收到電子郵件通知。</p> <p>僅當項目狀態為[!UICONTROL Current]或[!UICONTROL Planning]時，才會發送通知。</p> <p>擁有[!UICONTROL Review]授權的使用者不會收到通知。 </p> <p>即時通知電子郵件的主旨是： <em>[!UICONTROL完成]: &lt;issue name=""&gt; on &lt;project name=""&gt;</em></p> <p> 每日摘要通知的主旨是： <em> [!UICONTROL您擁有的項目摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> 問題名稱<br>專案名稱<br>問題參考編號<br>完成問題的用戶名<br>問題狀態<br>問題完成的日期和時間<br>上一個問題狀態<br><strong>[!UICONTROL查看更多詳細資訊]</strong> 按鈕 <br>*專案名稱<br>*項目參考編號<br>*已完成問題總數<br>*問題名稱<br>*分配給問題的用戶的名稱<br>*每日摘要日期<br></td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>向我持有的專案新增未指派的問題</strong> </p> <p>將未指派的問題新增至專案時，專案擁有者會收到電子郵件通知。</p> <p>僅當項目狀態為[!UICONTROL Current]或[!UICONTROL Planning]時，才會發送通知。</p> <p>即時通知電子郵件的主旨是： <em>[!UICONTROL應在上為此新問題分配誰] &lt;project name=""&gt;?</em></p> <p> </p> <p> 每日摘要通知的主旨是： <em> 您擁有的專案摘要 &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>專案名稱<br>Portfolio名稱<br>問題參考編號<br>新增問題的使用者名稱<br>問題名稱<br>問題類型<br>輸入日期<br>問題優先順序<br>指派給名稱（空）<br>問題狀態<br>主要連絡人<br>*專案名稱<br>*項目參考編號<br>*新增的問題總數<br>*問題名稱<br>*新增問題的使用者名稱<br>*每日摘要日期<br></p> </td> 
   <td> <p><strong>立即</strong> </p> <p><strong>和每日</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我被設為新專案的所有者</strong> </p> <p>將使用者指派為專案的擁有者時，該使用者會收到電子郵件通知。</p> <p>如果專案擁有者是進行指派的相同使用者，則不會傳送電子郵件通知。</p> <p>擁有[!UICONTROL Review]授權的使用者不會收到通知。</p> <p>開啟這個，因為他們被派去了。 </p> <p> 指派某些東西，共用某些東西，獲取某些東西的訪問權限。</p> <p>即時通知電子郵件的主旨是： <em>[!UICONTROL您現在是的專案擁有者] &lt;project name=""&gt;</em></p> <p>電子郵件通知的正文包含下列文字：<em><br></em></p> <p><em>[!UICONTROL Hi] &lt;your name=""&gt;,<br></em><em>&lt;name of="" the="" user="" who="" assigned="" you="" as="" the="" project="" owner=""&gt; [!UICONTROL使您成為[]的所有者 &lt;project name=""&gt;. [!UICONTROL作為項目所有者，您可能會收到有關項目活動的其他電子郵件通知、批准項目的時數所需的通知，或參與批准與項目相關的工作。 全是你的。]</em> </p> <p> 每日摘要通知的主旨是： <em> [!UICONTROL您擁有的項目摘要] &lt;date of="" daily="" digest=""&gt; </em></p> <p> </p> </td> 
   <td> <p>專案名稱<br>Portfolio名稱<br>項目參考編號<br>項目完成日期<br>*專案名稱<br>*項目參考編號<br>*每日摘要日期</p> </td> 
   <td><strong>立即</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我的其中一項專案上的任務認可日期變更</strong> </p> <p>項目所有者在項目上某項任務的「提交日期」更改時收到電子郵件通知，除非更改了「提交日期」的用戶也是項目所有者。</p> <p>即時通知電子郵件的主旨是： <em>[!UICONTROL的提交日期] &lt;task name=""&gt; [!UICONTROL現在為] &lt;new commit="" date=""&gt;</em></p> <p> 每日摘要通知的主旨是： <em> 您擁有的專案摘要 &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>任務名稱<br>專案名稱<br>任務參考編號<br>更改提交日期的用戶名<br>新提交日期<br>任務[!UICONTROL計畫完成日期]<br>有關項目時間表如何受此更改影響的資訊<br>指派給名稱<br>按名稱輸入<br>專案擁有者<br><strong>[!UICONTROL查看更多詳細資訊]</strong> 按鈕<br>*專案名稱<br>*項目參考編號<br>*其提交日期已更改的任務總數<br>*任務名稱<br>*每日摘要日期<br></p> </td> 
   <td> <p><strong>立即</strong> </p> <p><strong>和[!UICONTROL每日]</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>認可日期因我專案上的一個問題變更</strong> </p> <p>項目所有者在項目問題的「提交日期」更改時收到電子郵件通知，除非更改「提交日期」的用戶與項目所有者相同。</p> <p>即時通知電子郵件的主旨是： <em>[!UICONTROL的提交日期] &lt;issue name=""&gt; [!UICONTROL現在為] &lt;new commit="" date=""&gt;</em></p> <p> 每日摘要通知的主旨是： <em> [!UICONTROL您擁有的項目摘要] &lt;date of="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>問題名稱<br>專案名稱<br>問題參考編號<br>更改提交日期的用戶名<br>新提交日期<br>發放計畫完成日期<br>指派給名稱<br>按名稱輸入<br>專案擁有者<br><strong>[!UICONTROL查看更多詳細資訊]</strong> 按鈕<br>*專案名稱<br>*項目參考編號<br>*提交日期已更改的問題總數<br>*問題名稱<br>*每日摘要日期<br></p> </td> 
   <td> <p><strong>立即</strong> </p> <p><strong>和[!UICONTROL每日]</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
