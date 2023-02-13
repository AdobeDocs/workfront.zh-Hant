---
content-type: reference
navigation-topic: notifications
title: '通知：其他資訊'
description: 下列通知會提醒您，您正在贊助的專案中發生的活動。
author: Lisa
feature: Get Started with Workfront
exl-id: fd93a48b-ef09-4489-b93d-5328240ffed6
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '968'
ht-degree: 8%

---

# 通知：其他資訊

下列通知會提醒您，您正在贊助的專案中發生的活動。

如需設定您收到哪些通知的詳細資訊，請參閱 [啟用或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

另請參閱 [事件通知](../../workfront-basics/using-notifications/event-notifications.md).

>[!NOTE]
>
>您無法啟用或停用每日通知，也不會收到此類別事件的每日摘要電子郵件。 您可以為 [!UICONTROL 其他] 類別。

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
   <td> <p><strong>會向[!UICONTROL公告中心]發送消息</strong> </p> <p>當有新郵件發送到[!UICONTROL公告中心]時，您會收到電子郵件通知。 </p> <p>即時通知電子郵件的主旨是： <em>[!UICONTROL [!DNL Adobe Workfront] 公告]: &lt;subject of="" the="" announcement=""&gt;</em></p> </td> 
   <td> 公告的主體<br>公告中包含的報文文本<br>附加的文檔<br>發送公告的用戶名<br>發送公告的日期和時間 </td> 
   <td><strong>立即</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>任務指派變更影響了我的一名人員</strong> </p> <p>當指定為經理的用戶的「直接報告」之一被分配給新任務時，經理將收到有關該分配的電子郵件。 </p> <p>只有在專案狀態為[!UICONTROL目前]時，才會傳送通知。</p> <p>即時通知電子郵件的主旨是： <em>[!UICONTROL任務資源分配]: &lt;task name=""&gt;</em></p> </td> 
   <td>專案名稱<br>任務名稱<br>建立任務的日期和時間<br>建立任務的用戶的名稱<br>分配名稱<br>到期日（計畫完成日期）<br>任務狀態<br></td> 
   <td><strong>立即</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>接收文件上傳要求之後，要求會取消</strong> </p> <p>取消文檔請求時，文檔請求會收到電子郵件通知。</p> <p>即時通知電子郵件的主旨是： <em>&lt;name of="" the="" user="" who="" canceled="" the="" request=""&gt; 已取消文檔請求。 </em></p> <p>電子郵件通知的正文包含下列文字：</p> <p><em>[!UICONTROL Hi] &lt;your name=""&gt;, <br><br>&lt;name of="" the="" user="" who="" canceled="" the="" request=""&gt;[!UICONTROL不再需要您上傳任何與您先前收到的請求相關的內容。 我們只是想告訴你。]</em> </p> </td> 
   <td>取消請求的用戶名<br>原始文檔上載請求的文本<br>原始文檔請求上的「[!UICONTROL CANCELLED]」橫幅<br>原始文檔請求的日期和時間<br></td> 
   <td><strong>立即</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>已發現需要我注意的錯誤</strong> </p> <p>無法傳送回覆時，透過電子郵件回覆留言的使用者會收到電子郵件通知。</p> <p>即時通知電子郵件的主旨是： <em>[!UICONTROL無法處理] &lt;subject of="" original="" message=""&gt;</em></p> <p>如需使用電子郵件回覆留言的相關資訊，請參閱。<strong></strong></p> </td> 
   <td> </td> 
   <td><strong>立即</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>問題指派變更影響了我的一名人員</strong> </p> <p>指派給問題的使用者的管理員會在該使用者從問題中移除或指派給問題時收到電子郵件通知。 </p> <p>僅當項目狀態為「當前」或「計畫」時，才會發送通知。</p> <p>即時通知電子郵件的主旨是： <em>問題分配： &lt;issue name=""&gt;</em></p> </td> 
   <td> <p>問題名稱<br>專案名稱<br>問題參考編號<br>執行分配的用戶的姓名<br>問題類型<br>指派給問題的使用者名稱<br>輸入發行日期<br>問題優先順序<br>主要連絡人<br>問題[!UICONTROL計畫完成日期]<br>問題狀態<br><strong>[!UICONTROL查看更多詳細資訊]</strong> 按鈕</p> </td> 
   <td><strong>立即</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我的一名人員新增至一個專案</strong> </p> <p>當其使用者中一人新增至專案時，經理會收到電子郵件通知。 不論專案的狀態為何，都會傳送此通知。 </p> <p>擁有[!UICONTROL Review]授權的使用者不會收到通知。</p> <p>電子郵件的主旨是： <em>項目分配： &lt;user name=""&gt;[&lt;project guid=""&gt;_ &lt;user guid=""&gt;]</em></p> </td> 
   <td> <p>專案名稱<br>Portfolio名稱<br>項目參考編號<br>將人員新增至專案的使用者名稱<br>已新增至專案的使用者名稱<br>項目[!UICONTROL計劃開始日期]<br>項目[!UICONTROL計畫完成日期]<br>項目完成百分比<br>項目上的其他名稱<br>專案狀態<br>專案擁有者<br><strong>[!UICONTROL查看更多詳細資訊]</strong> 按鈕<br><br><br></p> </td> 
   <td><strong>立即</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>某人將專案新增至我所擁有的投資組合或計劃之中</strong> </p> <p>當新項目添加到產品組合或方案時，產品組合和/或方案所有者接收通知。</p> <p>即時通知電子郵件的主旨是： <em>[!UICONTROL項目已添加到] &lt;portfolio name=""&gt;[項目GUID]</em></p> </td> 
   <td> Portfolio名稱<br>項目參考編號<br>將項目添加到產品組合/方案的用戶的名稱<br><br></td> 
   <td><strong>立即</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>某人員與我共用一個物件</strong> </p> <p>當有人將您新增至物件的[!UICONTROL共用]權限清單時，您會收到電子郵件通知。</p> <p>即時通知電子郵件的主旨是： <em>[!UICONTROL授予的訪問權]: &lt;object name=""&gt;</em></p> <p>只有在專案處於[!UICONTROL目前]狀態時，才會傳送通知。</p> </td> 
   <td> 物件名稱<br>父對象名稱<br>對象引用編號<br>對對象的原始訪問<br>授予物件的新存取權<br>授予存取權的日期和時間 <br>授予存取權的使用者名稱 </td> 
   <td><strong>立即</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>有人員與我的團隊共用一個物件</strong> </p> <p>當有人將您的團隊新增至物件權限的共用清單時，您會收到電子郵件通知。</p> <p>即時通知電子郵件的主旨是： <em>[!UICONTROL授予的訪問權]: &lt;object name=""&gt; [訪問規則GUID]</em></p> </td> 
   <td> 物件名稱<br>父對象名稱<br>對象引用編號<br>舊訪問<br>新存取<br>授予存取權的日期和時間<br>團隊名稱<br>授予存取權的使用者名稱 </td> 
   <td><strong>立即</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>已對我訂閱的任務、問題或專案進行更新</strong> </p> <p>當有人對您訂閱的項目發表評論時，您會收到電子郵件通知。</p> <p>訂閱電子郵件的主旨是： <em>[!UICONTROL已對進行更新] &lt;object type=""&gt; 您已訂閱： &lt;object name=""&gt;</em></p> </td> 
   <td> 物件名稱<br> 對象引用編號<br> 對訂閱項目發表評論的用戶的名稱<br> 日期評論<br> 已新增至訂閱項目的註解  </td> 
   <td><strong>立即</strong> </td> 
  </tr> 
 </tbody> 
</table>
