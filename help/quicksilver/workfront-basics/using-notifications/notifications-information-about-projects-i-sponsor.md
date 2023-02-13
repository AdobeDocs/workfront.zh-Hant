---
content-type: reference
navigation-topic: notifications
title: '''通知：關於我贊助的項目的資訊'
description: 下列通知會提醒您，您正在贊助的專案中發生的活動。
author: Lisa
feature: Get Started with Workfront
exl-id: b4c7c046-f15f-4e6e-9332-5232c7b7080b
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '1316'
ht-degree: 6%

---

# 通知：關於我贊助的項目的資訊

下列通知會提醒您，您正在贊助的專案中發生的活動。

如需設定您收到哪些通知的詳細資訊，請參閱 [啟用或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>向我贊助的專案新增一個文件</strong> </p> <p>當檔案新增至專案時，專案贊助商會收到電子郵件通知。</p> <p>僅當項目狀態為[!UICONTROL Current]且文檔不為[!UICONTROL Private]時，才會發送通知。</p> <p>即時通知電子郵件的主旨是： <em>[!UICONTROL文檔已添加到] &lt;project name=""&gt;</em></p> <p>每日摘要通知的主旨是：<em> [!UICONTROL您贊助的項目摘要] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 專案名稱<br>Portfolio名稱<br>文檔參考編號<br>添加文檔的用戶的名稱<br>文檔名稱<br>新增日期<br>文檔詳細資訊（格式、大小、版本號）<br>文檔縮圖<br><strong>[!UICONTROL預覽]</strong> 和 <strong>[!UICONTROL下載]</strong> 按鈕<br>*專案名稱<br>*項目參考編號<br>*新增的檔案總數<br>*文檔名稱<br>*新增檔案的使用者名稱<br>*每日摘要日期 </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在我贊助的專案上完成里程碑任務</strong> </p> <p>項目贊助商在其贊助的項目上完成里程碑任務時收到電子郵件通知。</p> <p>僅當項目狀態為[!UICONTROL Current]或[!UICONTROL Planning]時，才會發送通知。</p> <p>即時通知電子郵件的主旨是： <em>[!UICONTROL完成]: &lt;task name=""&gt; on &lt;project name=""&gt;</em></p> <p>注意：如果任務更改為相當於[!UICONTROL Complete]的狀態，則電子郵件的主題仍顯示「[!UICONTROL Complete]」。<br></p> <p>每日摘要通知的主旨是：<em> 您贊助的項目摘要 &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 任務名稱<br>專案名稱<br>任務參考編號<br>完成任務的用戶名<br>新任務狀態<br>任務完成的日期和時間<br>上一任務狀態<br><strong>[!UICONTROL查看更多詳細資訊]</strong> 按鈕 <br>*專案名稱<br>*項目參考編號<br>*已完成任務總數<br>*任務名稱<br>*完成任務的用戶名<br>*每日摘要日期<br></td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我贊助的專案落後</strong> </p> <p>當專案落後時，專案贊助人會收到電子郵件通知。 當進度狀態為「[!UICONTROL At Risk]」或「[!UICONTROL In Faule]」時，項目將落後於計畫。</p> <p>擁有[!UICONTROL Review]授權的使用者不會收到通知。</p> <p>即時通知電子郵件的主旨是： <em>[!UICONTROL項目進度更改]: &lt;project name=""&gt;</em></p> <p>每日摘要通知的主旨是： <em>[!UICONTROL您贊助的項目摘要] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 專案名稱<br>Portfolio名稱<br>項目參考編號<br>項目進度狀態<br>項目[!UICONTROL計劃開始日期]<br>項目[!UICONTROL計畫完成日期]<br>專案[!UICONTROL預計開始日期]<br>項目[!UICONTROL預計完成日期]<br>項目完成百分比<br>專案狀態<br>專案擁有者<br>*專案名稱<br>*項目參考編號<br>*項目進度狀態<br>*每日摘要日期 </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在我贊助的專案上完成了一項任務</strong> </p> <p>專案贊助商會收到電子郵件通知。</p> <p>只有在專案狀態為[!UICONTROL目前]時，才會傳送通知。</p> <p>即時通知電子郵件的主旨是： <em>[!UICONTROL完成]: &lt;task name=""&gt; on &lt;project name=""&gt;</em></p> <p> <p>注意：如果任務更改為相當於[!UICONTROL Complete]的狀態，則電子郵件的主題仍顯示「[!UICONTROL Complete]」。</p> </p> <p>每日摘要通知的主旨是：<em> 您贊助的項目摘要 &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 任務名稱<br>專案名稱<br>任務參考編號<br>完成任務的用戶名<br>任務狀態<br>更改任務狀態的日期和時間<br>上一任務狀態<br><strong>請參閱更多詳細資訊</strong> 按鈕<br>*專案名稱<br>*項目參考編號<br>*已完成任務總數<br>*任務名稱<br>*完成任務的用戶名<br>*每日摘要日期 </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我贊助專案上的一項任務落後</strong> </p> <p>當項目上的任務超出計畫時，項目贊助商會收到電子郵件通知。 當進度狀態為「[!UICONTROL At Risk]」或「[!UICONTROL Bethin]」或「[!UICONTROL Late]」時，任務將滯後於計畫。</p> <p>只有在專案狀態為[!UICONTROL目前]時，才會傳送通知。</p> <p>即時通知電子郵件的主旨是： <em>[!UICONTROL任務進度更改]: &lt;task name=""&gt;</em></p> <p>每日摘要通知的主旨是：<em> [!UICONTROL您贊助的項目摘要] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 任務名稱<br>專案名稱<br>任務參考編號<br>新任務進度狀態<br>任務[!UICONTROL計劃開始日期]<br>任務[!UICONTROL計畫完成日期]<br>任務[!UICONTROL預計開始日期]<br>任務[!UICONTROL預計完成日期]<br>任務完成百分比<br>任務狀態<br>指派給名稱<br>按名稱輸入<br>*專案名稱<br>*項目參考編號<br>*延遲的任務總數<br>*任務名稱<br>*進入任務的用戶名<br>*每日摘要日期 </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>向我贊助的專案新增了一個問題</strong> </p> <p>將問題新增至專案時，專案贊助商會收到電子郵件通知。</p> <p>僅當項目狀態為[!UICONTROL Current]或[!UICONTROL Planning]時，才會發送通知。</p> <p>即時通知電子郵件的主旨是： <em>[!UICONTROL問題已添加到] &lt;project name=""&gt;</em></p> <p>每日摘要通知的主旨是： <em>[!UICONTROL您贊助的項目摘要] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 專案名稱<br>Portfolio名稱<br>問題參考編號<br>新增問題的使用者名稱<br>問題名稱<br>問題類型<br>輸入日期<br>問題優先順序<br>指派給名稱 <br>問題狀態<br>主要連絡人<br>*專案名稱<br>*項目參考編號<br>*專案新增的問題總數<br>*問題名稱<br>*分配給問題的用戶的名稱<br>*每日摘要日期<br><br></td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>在我贊助的專案上完成了一個問題</strong> </p> <p>專案贊助商會收到電子郵件通知。</p> <p>僅當項目狀態為[!UICONTROL Current]或[!UICONTROL Planning]時，才會發送通知。</p> <p>即時通知電子郵件的主旨是： <em>[!UICONTROL完成]: &lt;issue name=""&gt; on &lt;project name=""&gt;</em></p> <p>每日摘要通知的主旨是：<em> 您贊助的項目摘要 &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 問題名稱<br>專案名稱<br>問題參考編號<br>完成問題的用戶名<br>問題狀態<br>問題完成的日期和時間<br>上一個問題狀態<br><strong>請參閱更多詳細資訊</strong> 按鈕<br>*專案名稱<br>*項目參考編號<br>*已完成問題總數<br>*問題名稱<br>*分配給問題的用戶的名稱<br>*每日摘要日期 </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>向我贊助的專案新增了一個未指派問題</strong> </p> <p>當未指派的問題新增至專案時，專案贊助商會收到電子郵件通知。</p> <p>僅當項目狀態為[!UICONTROL Current]或[!UICONTROL Planning]時，才會發送通知。</p> <p>即時通知電子郵件的主旨是： <em>[!UICONTROL應在上為此新問題分配誰] &lt;project name=""&gt;?</em></p> <p>每日摘要通知的主旨是：<em> [!UICONTROL您贊助的項目摘要] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 專案名稱<br>Portfolio名稱<br>問題參考編號<br>新增問題的使用者名稱<br>問題名稱<br>問題類型<br>輸入日期<br>問題優先順序<br>指派給名稱（空）<br>問題狀態<br>主要連絡人<br>*專案名稱<br>*項目參考編號<br>*新增的問題總數<br>*問題名稱<br>*新增問題的使用者名稱<br>*每日摘要日期<br></td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我被設為專案贊助者</strong> </p> <p>當項目贊助者被設定為項目贊助者時，項目贊助者會收到電子郵件通知。<br></p> <p>即時通知電子郵件的主旨是： <em>[!UICONTROL項目贊助商]: &lt;project name=""&gt;</em></p> <p>電子郵件通知的正文包含下列文字：</p> <p><em>[!UICONTROL Hi] &lt;your name=""&gt;,</em> </p> <p><em>&lt;name of="" the="" user="" who="" assigned="" you="" as="" the="" project="" sponsor=""&gt; [!UICONTROL使你成為]的贊助商 &lt;project name=""&gt;. [!UICONTROL作為項目贊助商，您可能會收到有關項目活動的其他電子郵件通知，或參與批准與項目相關的工作。 享受吧。]</em> </p> <p>每日摘要通知的主旨是： <em>您贊助的項目摘要 &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>專案名稱<br>Portfolio名稱<br>項目參考編號<br>項目計畫完成日期<br>*專案名稱<br>*項目參考編號<br>*每日摘要日期</p> </td> 
   <td><strong>立即</strong> </td> 
  </tr> 
 </tbody> 
</table>
