---
content-type: reference
navigation-topic: notifications
title: 「通知：其他資訊」
description: 下列通知會提醒您正在贊助的專案上發生的活動。
author: Lisa
feature: Get Started with Workfront
exl-id: fd93a48b-ef09-4489-b93d-5328240ffed6
source-git-commit: 298b74c2d228a76c02d34470fa8298028605cab4
workflow-type: tm+mt
source-wordcount: '970'
ht-degree: 8%

---

# 通知：其他資訊

下列通知會提醒您正在贊助的專案上發生的活動。

如需有關設定您接收哪些通知的資訊，請參閱 [修改您自己的電子郵件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

另請參閱 [事件通知](../../workfront-basics/using-notifications/event-notifications.md).

>[!NOTE]
>
>您無法啟用或停用每日通知，並且不會收到此類別中事件的每日摘要電子郵件。 您可以啟用或停用以下專案的個別即時通知： [!UICONTROL 其他] 類別。

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
   <td> <p><strong>已傳送訊息至[！UICONTROL宣告中心]</strong> </p> <p>您會在新訊息傳送至[！UICONTROL宣告中心]時收到電子郵件通知。 </p> <p>即時通知電子郵件的主旨為： <em>[！UICONTROL [!DNL Adobe Workfront] 公告]： &lt;subject of="" the="" announcement=""&gt;</em></p> </td> 
   <td> 宣告的主題<br>包含在宣告中的訊息文字<br>附加檔案<br>傳送宣告的使用者名稱<br>傳送宣告的日期與時間 </td> 
   <td><strong>立即</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>任務指派的變更影響了我的一名人員</strong> </p> <p>當指定為管理員的使用者的「直接下屬」之一被指派給新任務時，管理員會收到有關指派的電子郵件。 </p> <p>只有在專案狀態為[！UICONTROL目前]時，才會傳送通知。</p> <p>即時通知電子郵件的主旨為： <em>[！UICONTROL任務資源指派]： &lt;task name=""&gt;</em></p> </td> 
   <td>專案名稱<br>任務名稱<br>建立任務的日期與時間<br>建立任務的使用者名稱<br>指派名稱<br>到期日（計畫完成日期）<br>任務狀態<br></td> 
   <td><strong>立即</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>接收文件上傳請求之後，請求被取消</strong> </p> <p>檔案請求取消時，「檔案請求者」會收到電子郵件通知。</p> <p>即時通知電子郵件的主旨為： <em>&lt;name of="" the="" user="" who="" canceled="" the="" request=""&gt; 已取消檔案請求。 </em></p> <p>電子郵件通知內文包含下列文字：</p> <p><em>[！UICONTROL Hi] &lt;your name=""&gt;， <br><br>&lt;name of="" the="" user="" who="" canceled="" the="" request=""&gt;[！UICONTROL不再需要您上傳與您之前收到之請求相關的任何專案。 我們只是想讓您知道。]</em> </p> </td> 
   <td>取消請求的使用者名稱<br>原始檔案上傳請求的文字<br>原始檔案請求上方的「[！UICONTROL CANCELED]」橫幅<br>原始檔案請求的日期和時間<br></td> 
   <td><strong>立即</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>已發現需要我注意的錯誤</strong> </p> <p>當無法傳遞回覆時，透過電子郵件回複評論的使用者會收到電子郵件通知。</p> <p>即時通知電子郵件的主旨為： <em>[！UICONTROL無法處理] &lt;subject of="" original="" message=""&gt;</em></p> <p>如需使用電子郵件回複評論的詳細資訊，請參閱 <a href="/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/reply-to-email-notifications.md">回覆電子郵件通知</a>.</p> </td>
   <td> </td> 
   <td><strong>立即</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>問題指派的變更影響了我的一名人員</strong> </p> <p>將使用者從問題中移除或將其指派給問題時，指派給問題的使用者的經理會收到電子郵件通知。 </p> <p>僅當專案狀態為「目前」或「計畫」時，才會傳送通知。</p> <p>即時通知電子郵件的主旨為： <em>問題指派： &lt;issue name=""&gt;</em></p> </td> 
   <td> <p>問題名稱<br>專案名稱<br>問題參考號碼<br>進行指派的使用者名稱<br>問題型別<br>指派給問題的使用者名稱<br>已輸入發行日期<br>問題優先順序<br>主要連絡人<br>問題[！UICONTROL規劃完成日期]<br>問題狀態<br><strong>[！UICONTROL檢視更多詳細資料]</strong> 按鈕</p> </td> 
   <td><strong>立即</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我的一名人員已被新增至一項專案中</strong> </p> <p>當經理的其中一個使用者新增至專案時，經理會收到電子郵件通知。 無論專案狀態為何，都會傳送此通知。 </p> <p>擁有[！UICONTROL Review]授權的使用者不會收到通知。</p> <p>電子郵件的主旨為： <em>專案指定任務： &lt;user name=""&gt;[&lt;project guid=""&gt;_ &lt;user guid=""&gt;]</em></p> </td> 
   <td> <p>專案名稱<br>Portfolio名稱<br>專案參考號碼<br>將人員新增至專案的使用者名稱<br>已新增至專案的使用者名稱<br>專案[！UICONTROL計劃開始日期]<br>專案[！UICONTROL計畫完成日期]<br>專案完成百分比<br>專案中其他人的名稱<br>專案狀態<br>專案所有者<br><strong>[！UICONTROL檢視更多詳細資料]</strong> 按鈕<br><br><br></p> </td> 
   <td><strong>立即</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>有人將專案新增至我所擁有的專案組合或計劃之中</strong> </p> <p>當新專案新增到投資組合或方案時，投資組合和/或方案所有者會收到通知。</p> <p>即時通知電子郵件的主旨為： <em>[！UICONTROL專案已新增到] &lt;portfolio name=""&gt;[專案GUID]</em></p> </td> 
   <td> Portfolio名稱<br>專案參考號碼<br>將專案新增至投資組合/方案的使用者名稱<br><br></td> 
   <td><strong>立即</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>有人與我分享了一個物件</strong> </p> <p>當有人將您新增至物件許可權的[！UICONTROL Sharing]清單時，您會收到電子郵件通知。</p> <p>即時通知電子郵件的主旨為： <em>[！UICONTROL已授予存取權]： &lt;object name=""&gt;</em></p> <p>僅當專案處於[！UICONTROL目前]狀態時，才會傳送通知。</p> </td> 
   <td> 物件名稱<br>父系物件名稱<br>物件參考編號<br>物件的原始存取權<br>授予物件的新存取權<br>授與存取權的日期與時間 <br>授與存取許可權的使用者名稱 </td> 
   <td><strong>立即</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>有人與我的團隊分享了一個物件</strong> </p> <p>當有人將您的團隊新增至物件的「共用」許可權清單時，您會收到電子郵件通知。</p> <p>即時通知電子郵件的主旨為： <em>[！UICONTROL已授予存取權]： &lt;object name=""&gt; [存取規則GUID]</em></p> </td> 
   <td> 物件名稱<br>父系物件名稱<br>物件參考編號<br>舊存取<br>新增存取權<br>授與存取權的日期與時間<br>您的團隊名稱<br>授與存取許可權的使用者名稱 </td> 
   <td><strong>立即</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我訂閱的任務、問題或專案已更新</strong> </p> <p>當有人對您訂閱的專案發表評論時，您會收到電子郵件通知。</p> <p>訂閱電子郵件的主旨為： <em>[！UICONTROL]已更新 &lt;object type=""&gt; 您已訂閱： &lt;object name=""&gt;</em></p> </td> 
   <td> 物件名稱<br> 物件參考編號<br> 對訂閱專案發表評論的使用者名稱<br> 發表評論的日期<br> 已新增到訂閱專案的註解  </td> 
   <td><strong>立即</strong> </td> 
  </tr> 
 </tbody> 
</table>
