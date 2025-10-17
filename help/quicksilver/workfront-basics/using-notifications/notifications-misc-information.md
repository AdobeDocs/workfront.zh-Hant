---
content-type: reference
navigation-topic: notifications
title: 通知：其他資訊
description: 下列通知會提醒您正在贊助的專案上發生的活動。
author: Courtney
feature: Get Started with Workfront
exl-id: fd93a48b-ef09-4489-b93d-5328240ffed6
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '971'
ht-degree: 0%

---

# 通知：其他資訊

下列通知會提醒您正在贊助的專案上發生的活動。

如需有關設定您收到哪些通知的資訊，請參閱[修改您自己的電子郵件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)。

另請參閱[事件通知](../../workfront-basics/using-notifications/event-notifications.md)。

>[!NOTE]
>
>您無法啟用或停用每日通知，並且不會收到此類別中事件的每日摘要電子郵件。 您可以啟用或停用[!UICONTROL 雜項]類別的個別即時通知。

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
   <td> <p><strong>傳送訊息至[!UICONTROL 宣告中心]</strong> </p> <p>您會在新訊息傳送至[!UICONTROL 宣告中心]時收到電子郵件通知。 </p> <p>立即通知電子郵件的主旨為： <em>[!UICONTROL [!DNL Adobe Workfront]宣告]： &lt;宣告的主旨&gt;</em></p> </td> 
   <td> 宣告的主旨<br>包含在宣告中的訊息文字<br>附加檔案<br>傳送宣告的使用者名稱<br>傳送宣告的日期和時間 </td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>任務指派變更影響了我的一名人員</strong> </p> <p>當指定為管理員的使用者的「直接下屬」之一被指派給新任務時，管理員會收到有關指派的電子郵件。 </p> <p>只有在專案狀態為[!UICONTROL 目前]時，才會傳送通知。</p> <p>即時通知電子郵件的主旨為： <em>[!UICONTROL 任務資源指派]： &lt;任務名稱&gt;</em></p> </td> 
   <td>專案名稱<br>任務名稱<br>建立任務的日期與時間<br>建立任務的使用者名稱<br>工作分派名稱<br>到期日（計畫完成日期）<br>任務狀態<br></td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>收到檔案上傳要求後，要求被取消</strong> </p> <p>檔案請求取消時，「檔案請求者」會收到電子郵件通知。</p> <p>即時通知電子郵件的主旨為： <em>&lt;取消要求的使用者名稱&gt;已取消檔案要求。</em></p> <p>電子郵件通知內文包含下列文字：</p> <p><em>[!UICONTROL Hi] &lt;您的名稱&gt;， <br><br>&lt;取消要求的使用者名稱&gt;[!UICONTROL 不再需要您上傳與您先前取得之要求相關的任何資料。 我們只是想讓您知道。]</em> </p> </td> 
   <td>取消要求的使用者名稱<br>原始檔案上傳要求的文字<br>原始檔案要求上方的「[!UICONTROL CANCELED]」橫幅<br>原始檔案要求的日期和時間<br></td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>發現需要我注意的錯誤</strong> </p> <p>當無法傳遞回覆時，透過電子郵件回複評論的使用者會收到電子郵件通知。</p> <p>即時通知電子郵件的主旨為： <em>[!UICONTROL 無法處理於] &lt;原始訊息的主旨&gt;</em></p> <p>如需使用電子郵件回複評論的詳細資訊，請參閱<a href="/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/reply-to-email-notifications.md">回覆電子郵件通知</a>。</p> </td>
   <td> </td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>問題指派變更影響了我的一名人員</strong> </p> <p>將使用者從問題中移除或將其指派給問題時，指派給問題的使用者的經理會收到電子郵件通知。 </p> <p>僅當專案狀態為「目前」或「計畫」時，才會傳送通知。</p> <p>即時通知電子郵件的主旨為： <em>問題指派： &lt;問題名稱&gt;</em></p> </td> 
   <td> <p>問題名稱<br>專案名稱<br>問題參考編號<br>進行指派的使用者名稱<br>問題型別<br>指派給問題的使用者名稱<br>問題日期已輸入<br>問題優先順序<br>主要連絡人<br>問題[!UICONTROL 規劃完成日期]<br>問題狀態<br><strong>[!UICONTROL 檢視更多詳細資料]</strong>按鈕</p> </td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我的其中一個人員已新增至專案</strong> </p> <p>當經理的其中一個使用者新增至專案時，經理會收到電子郵件通知。 無論專案狀態為何，都會傳送此通知。 </p> <p>擁有[!UICONTROL Review]授權的使用者不會收到通知。</p> <p>電子郵件的主旨為： <em>專案指派： &lt;使用者名稱&gt;[&lt;專案GUID&gt;_ &lt;使用者GUID&gt;]</em></p> </td> 
   <td> <p>專案名稱<br>Portfolio名稱<br>專案參考編號<br>將人員加入專案的使用者名稱<br>加入專案的使用者名稱<br>專案[!UICONTROL 計劃開始日期]<br>專案[!UICONTROL 計畫完成日期]<br>專案完成百分比<br>專案上其他人的名稱<br>專案狀態<br>專案所有者<br><strong>[!UICONTROL 檢視更多詳細資料]</strong>按鈕<br><br><br></p> </td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>某人新增專案至我擁有的投資組合或方案</strong> </p> <p>當新專案新增到投資組合或方案時，投資組合和/或方案所有者會收到通知。</p> <p>立即通知電子郵件的主旨為： <em>[!UICONTROL 專案已新增至] &lt;Portfolio名稱&gt;[專案GUID]</em></p> </td> 
   <td> Portfolio名稱<br>專案參考號碼<br>將專案新增至投資組合/方案的使用者名稱<br><br></td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>有人與我共用一個物件</strong> </p> <p>當有人將您新增至物件許可權的[!UICONTROL Sharing]清單時，您會收到電子郵件通知。</p> <p>即時通知電子郵件的主旨為： <em>[!UICONTROL 存取已授予]： &lt;物件名稱&gt;</em></p> <p>僅當專案處於[!UICONTROL 目前]狀態時，才會傳送通知。</p> </td> 
   <td> 物件名稱<br>父系物件名稱<br>物件參考編號<br>物件的原始存取權<br>物件的新存取權<br>授與存取權的日期與時間<br>授與存取權的使用者名稱 </td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>有人與我的團隊共用一個物件</strong> </p> <p>當有人將您的團隊新增至物件的「共用」許可權清單時，您會收到電子郵件通知。</p> <p>即時通知電子郵件的主旨為： <em>[!UICONTROL 存取已授予]： &lt;物件名稱&gt; [存取規則GUID]</em></p> </td> 
   <td> 物件名稱<br>父物件名稱<br>物件參考編號<br>舊存取權<br>新存取權<br>授與存取權的日期和時間<br>您團隊的名稱<br>授與存取權的使用者名稱 </td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我訂閱的任務、問題或專案已更新</strong> </p> <p>當有人對您訂閱的專案發表評論時，您會收到電子郵件通知。</p> <p>訂閱電子郵件的主旨為： <em>[!UICONTROL 已更新您訂閱的] &lt;物件型別&gt;： &lt;物件名稱&gt;</em></p> </td> 
   <td> 物件名稱<br>物件參考號碼<br>對訂閱專案做出註解的使用者名稱<br>做出日期註解<br>新增到訂閱專案的註解  </td> 
   <td><strong>即時</strong> </td> 
  </tr> 
 </tbody> 
</table>
