---
content-type: reference
navigation-topic: notifications
title: 通知：統一核准
description: 以下通知會提醒您統一核准體驗的核准活動。 如需有關設定您收到哪些通知的資訊，請參閱修改您自己的電子郵件通知。
author: Courtney
feature: Get Started with Workfront
exl-id: 6e60a9ec-4fe0-4f3d-a4dd-8dc09d11b834
last-update: 2026-10-20T00:00:00.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: c042179c-157b-516d-b27c-e3bf303e8567
    internal-label: Get Started with Workfront
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 7957c410d4a0e39b23b4f5a3d29a794e5deec72a
workflow-type: tm+mt
source-wordcount: '1052'
ht-degree: 0%
---
# 通知：統一核准

{{highlighted-preview}}

使用下列通知來隨時瞭解有關統一檢閱和核准的活動。 如需有關設定您收到的電子郵件通知的資訊，請參閱[修改您自己的電子郵件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)。

>[!NOTE]
>
>這些通知只能作為即時通知使用，並且無法在每日摘要中使用。


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>通知</th> 
   <th>包含的欄位</th> 
   <th>預設狀態</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>已完成核准 — 已核准</strong> </p> <p>檔案核准的最終決定為「已核准」。</p> <p>即時通知電子郵件的主旨為： <em>最終決定： （檔案）已核准</em></p> </td> 
   <td> <p>最終決定<br>檔案<br>核准要求日期<br>到期日<br>「前往檢閱」按鈕<br>詳細資訊區塊：檔名稱、檔案詳細資訊、所有收件者</p> <p><em>包含在部分核準時：</em><br>自訂訊息<br>階段<br>專案</p> </td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>核准已完成 — 已核准變更</strong> </p> <p>檔案核准的最終決定為「已核准，但有變更」。</p> <p>即時通知電子郵件的主旨為： <em>最終決定： （檔案）已核准變更</em></p> </td> 
   <td> <p>最終決定<br>檔案<br>核准要求日期<br>到期日<br>「前往檢閱」按鈕<br>詳細資訊區塊：檔名稱、檔案詳細資訊、所有收件者</p> <p><em>包含在部分核準時：</em><br>自訂訊息<br>階段<br>專案</p> </td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>核准已完成 — 需要工作</strong> </p> <p>檔案核准以需求工作的最終決定完成。</p> <p>即時通知電子郵件的主旨為： <em>最終決定： （檔案）需要工作</em></p> </td> 
   <td> <p>最終決定<br>檔案<br>核准要求日期<br>到期日<br>「前往檢閱」按鈕<br>詳細資訊區塊：檔名稱、檔案詳細資訊、所有收件者</p> <p><em>包含在部分核準時：</em><br>自訂訊息<br>階段<br>專案</p> </td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>臨近期限</strong> </p> <p>您參與的檔案核准即將到達截止日期。</p> <p>即時通知電子郵件的主旨為： <em>即將到來的核准期限（檔案）</em></p> </td> 
   <td> <p>請求者<br>您的角色<br>團隊<br>要求核准日期<br>到期日<br>「前往檢閱」按鈕<br>詳細資訊區塊：檔名稱、檔案詳細資訊、所有收件者</p> <p><em>包含在部分核準時：</em><br>檔案預覽<br>自訂訊息<br>階段<br>專案</p> </td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>已超過期限</strong> </p> <p>您參與的檔案核准已超過其期限，但無最終決定。</p> <p>即時通知電子郵件的主旨為： <em>核准截止日期已錯過（檔案）</em></p> </td> 
   <td> <p>固定標題<br>核准要求日期<br>到期日<br>「前往檢閱」按鈕<br>詳細資訊區塊：檔名稱、檔案詳細資訊、所有收件者</p> <p><em>包含在部分核準時：</em><br>階段</p> </td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>檢閱完成</strong> </p> <p>稽核者完成檔案核准的稽核。</p> <p>即時通知電子郵件的主旨為： <em>（檔案）已檢閱</em></p> </td> 
   <td> <p>檢閱者<br>檔案<br>「前往檢閱」按鈕<br>詳細資訊區塊：檔名稱、檔案詳細資訊、所有收件者</p> <p><em>包含在部分核準時：</em><br>檔案預覽<br>階段<br>專案</p> </td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>視訊核准限制接近(80%)</strong> </p> <p>影片核准達到其計畫80%的影片核准限制。</p> <p>即時通知電子郵件的主旨為： <em>您已接近Workfront的年度視訊核准要求限制</em></p> </td> 
   <td> 標題和正文文字<br>要求的視訊核准（目前使用量）<br>總上限（上限）<br>其他收件者<br>「在Workfront中檢視」按鈕<br>「升級至FIO enterprise」按鈕 </td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>視訊核准限制已達</strong> </p> <p>視訊核准達到其計畫的視訊核准限制。</p> <p>即時通知電子郵件的主旨為： <em>您已達到Workfront的年度視訊核准要求限制</em></p> </td> 
   <td> 標題和正文文字<br>要求的視訊核准（目前使用量）<br>總上限（上限）<br>其他收件者<br>「在Workfront中檢視」按鈕<br>「升級至FIO enterprise」按鈕 </td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>已作出決定 — 已核准</strong> </p> <p>核准者在檔案核准上決定為「已核准」。</p> <p>即時通知電子郵件的主旨為： <em>（檔案）核准者（名稱）</em></p> </td> 
   <td> <p>決策者<br>決定<br>檔案和版本<br>「前往檢閱」按鈕<br>詳細資訊區塊：檔名稱、檔案詳細資訊、所有收件者</p> <p><em>包含在部分核準時：</em><br>檔案預覽<br>自訂訊息<br>階段<br>專案</p> </td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>已作出決定 — 已核准變更</strong> </p> <p>核准者對檔案核准做出決定「已核准」，且有變更專案。</p> <p>即時通知電子郵件的主旨為： <em>（檔案）已核准，變更者為（名稱）</em></p> </td> 
   <td> <p>決策者<br>決定<br>檔案和版本<br>「前往檢閱」按鈕<br>詳細資訊區塊：檔名稱、檔案詳細資訊、所有收件者</p> <p><em>包含在部分核準時：</em><br>檔案預覽<br>自訂訊息<br>階段<br>專案</p> </td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>已作出決定 — 需要工作</strong> </p> <p>核准者決定檔案核准需要工作。</p> <p>即時通知電子郵件的主旨為： <em>（檔案）需要由（名稱）</em>工作</p> </td> 
   <td> <p>決策者<br>決定<br>檔案和版本<br>「前往檢閱」按鈕<br>詳細資訊區塊：檔名稱、檔案詳細資訊、所有收件者</p> <p><em>包含在部分核準時：</em><br>檔案預覽<br>自訂訊息<br>階段<br>專案</p> </td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>新增至群組核准或從中移除的檔案</strong> </p> <p>在您所屬的群組檔案核准中新增或移除檔案。</p> <p>即時通知電子郵件的主旨為： <em>檔案已新增至您所屬的核准或從核准中移除</em></p> </td> 
   <td> <p><strong>已新增：</strong><br>要求者<br>群組名稱<br>縮圖預覽<br>日期<br>「前往檢閱」按鈕<br>詳細資訊區塊：群組名稱、資產數目、所有收件者</p> <p><em>包含在部分核準時：</em><br>自訂訊息<br>專案</p> <p><strong>已移除：</strong><br>請求者<br>群組名稱<br>縮圖預覽（無按鈕或詳細資訊區塊）</p> </td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>所有評論已完成</strong> </p> <p>每個稽核者在檔案核准上完成稽核。</p> <p>即時通知電子郵件的主旨為： <em>所有評論完成於（檔案）</em></p> </td> 
   <td> <p>檔案<br>要求核准日期<br>到期日<br>「前往檢閱」按鈕<br>詳細資訊區塊：檔名稱、檔案詳細資訊、所有收件者</p> <p><em>包含在部分核準時：</em><br>自訂訊息<br>階段<br>專案</p> </td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>提醒 — 24小時</strong> </p> <p>您還有24小時來檢閱及核准檔案。</p> <p>即時通知電子郵件的主旨為： <em>提醒： （檔案）</em>需要您的核准</p> </td> 
   <td> <p>請求者<br>您的角色<br>團隊<br>要求核准日期<br>到期日<br>「前往檢閱」按鈕<br>詳細資訊區塊：檔名稱、檔案詳細資訊、所有收件者</p> <p><em>包含在部分核準時：</em><br>檔案預覽<br>自訂訊息<br>階段<br>專案</p> </td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>提醒 — 72小時</strong> </p> <p>您還剩72小時來檢閱及核准檔案。</p> <p>即時通知電子郵件的主旨為： <em>提醒： （檔案）</em>需要您的核准</p> </td> 
   <td> <p>請求者<br>您的角色<br>團隊<br>要求核准日期<br>到期日<br>「前往檢閱」按鈕<br>詳細資訊區塊：檔名稱、檔案詳細資訊、所有收件者</p> <p><em>包含在部分核準時：</em><br>檔案預覽<br>自訂訊息<br>階段<br>專案</p> </td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>已新增為核准者或檢閱者</strong> </p> <p>您會新增為檔案核准的核准者或稽核者。</p> <p>即時通知電子郵件的主旨為： <em>需要您的核准於（檔案）</em></p> </td> 
   <td> <p>請求者<br>您的角色<br>團隊<br>要求核准日期<br>到期日<br>「前往檢閱」按鈕<br>詳細資訊區塊：檔名稱、檔案詳細資訊、所有收件者</p> <p><em>包含在部分核準時：</em><br>檔案預覽<br>自訂訊息<br>階段<br>專案</p> </td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>已移除核准者或檢閱者</strong> </p> <p>您會從檔案核准中移除核准者或稽核者。</p> <p>即時通知電子郵件的主旨為： <em>不再需要您的核准（檔案）</em></p> </td> 
   <td> <p>要求者<br>檔案和版本<br>角色<br>團隊（無按鈕或詳細資訊區塊）</p> <p><em>當部分核準時包含：</em><br>檔案預覽<br>自訂訊息</p> </td> 
   <td><strong>即時</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>角色已變更</strong> </p> <p>您的核准者或稽核者角色在檔案核准上變更。</p> <p>即時通知電子郵件的主旨為： <em>您在（檔案）上的角色已變更</em></p> </td> 
   <td> <p>請求者<br>檔案和版本<br>角色變更方向<br>「前往檢閱」按鈕<br>詳細資訊區塊：檔名稱、檔案詳細資訊、所有收件者</p> <p><em>包含在部分核準時：</em><br>檔案預覽<br>階段<br>專案</p> </td> 
   <td><strong>即時</strong> </td> 
  </tr> 
 </tbody> 
</table>
