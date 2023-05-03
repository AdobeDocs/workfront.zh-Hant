---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Adobe Workfront中提供的事件通知
description: 事件通知是由物件上各種類型的事件（例如專案、工作和問題）所觸發的電子郵件，如事件通知中所述。
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: de7a995d-ff1e-4631-91f7-4dc895a87c94
source-git-commit: 25625291f691f7858634d9961fccb4465008dc3c
workflow-type: tm+mt
source-wordcount: '5008'
ht-degree: 29%

---

# Adobe Workfront中提供的事件通知

事件通知是由物件上各種類型的事件（例如專案、工作和問題）所觸發的電子郵件，如 [事件通知](../../../workfront-basics/using-notifications/event-notifications.md).

可在系統和組級別配置以下通知：

* 有關在系統級別配置事件通知的資訊，請參見 [為系統中的每個人配置事件通知](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).
* 如需在群組層級設定事件通知的詳細資訊，請參閱 [檢視及設定群組的事件通知](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

個別使用者也可以在其個別設定檔中啟用和停用其個別事件通知。 如需詳細資訊，請參閱 [啟用或停用您自己的事件通知](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

下表列出所有Adobe Workfront事件通知、事件的簡短說明，以及該事件預設為使用中或非使用中。

## 需要動作

另請參閱 [通知：需要的行動](../../../workfront-basics/using-notifications/notifications-action-needed.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>物件類型</th> 
   <th>Event</th> 
   <th>說明</th> 
   <th>預設狀態</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>使用者</p> </td> 
   <td> <p>對用戶的訪問請求</p> </td> 
   <td> <p>某人向我要求存取權.</p> </td> 
   <td> <p>使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>文件</p> <p> </p> </td> 
   <td> <p>請求者的文件請求新增</p> </td> 
   <td> <p>請我上傳檔案。</p> <p>當檔案請求者收到上傳檔案的請求時，他們會收到電子郵件通知。</p> </td> 
   <td> <p>使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>文件</p> </td> 
   <td> <p>文件擱置中，等待核准者核准</p> </td> 
   <td> <p>我需要核准文件.</p> </td> 
   <td> <p>使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>問題</p> </td> 
   <td> <p>「問題指派」到「問題受指派者」</p> </td> 
   <td> <p>我被指派到問題.</p> <p>只有在項目狀態為「當前」且問題狀態為「未關閉」或等於「已關閉」的情況下，問題受託人才會收到電子郵件通知。</p> <p>擁有審核或請求授權的使用者不會收到通知。</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>問題</p> </td> 
   <td> <p>核准者的擱置核准問題</p> </td> 
   <td> <p>我需要核准問題.</p> <p>哪些使用者會收到此事件的電子郵件通知，取決於是否啟用「不需要核准者加入專案團隊（針對包含角色的核准程式）」設定(如 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">配置全局批准設定</a>)。 </p> <p>如果已啟用此選項</strong>，系統會以「核准者」工作角色傳送電子郵件通知給系統中的所有使用者。</p> <p>如果禁用此選項</strong>，只有具有「核准者」工作角色的專案團隊成員會收到電子郵件通知。</p> <p>如果項目處於「計畫」或「當前」狀態，則會發送通知。 </p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>問題</p> </td> 
   <td> <p>給受委派核准者的未決核准問題</p> </td> 
   <td> <p>我需要檢閱已委派的核發核准。</p> <p>當某人將核發核准委派給其他使用者時，會通知該使用者。 </p> <p>只有當專案處於「目前」狀態時，才會傳送通知。</p> </td> 
   <td> <p>使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>專案</p> </td> 
   <td> <p>核准者的專案擱置核准</p> </td> 
   <td> <p>我需要核准專案.</p> <p>哪些使用者會收到此事件的電子郵件通知，取決於是否啟用「不需要核准者加入專案團隊（針對包含工作角色的核准程式）」設定(如 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">配置全局批准設定</a>)。</p> <p>如果已啟用此選項</strong>，系統會以「核准者」工作角色傳送電子郵件通知給系統中的所有使用者。</p> <p>如果禁用此選項</strong>，只有具有「核准者」工作角色的專案團隊成員會收到電子郵件通知。</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td>專案</td> 
   <td>給受委派核准者的專案未決核准</td> 
   <td> <p>我需要審核我所受委派的專案核准.</p> </td> 
   <td> 使用中</td> 
  </tr> 
  <tr> 
   <td> <p>任務</p> </td> 
   <td> <p>「任務指派」到「任務受指派者」</p> </td> 
   <td> <p>我被設為一項任務的主要受指派者.</p> <p>如果任務受託人被確定為任務的主要受託人，則任務受託人會收到電子郵件通知，除非受託人是進行該分配的用戶。</p> <p>如果項目狀態為「當前」且未將任務標籤為「完成」，則會發送通知。</p> <p>擁有審核許可證的用戶不會收到通知。</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務</p> </td> 
   <td> <p>核准者的擱置核准任務</p> </td> 
   <td> <p>我需要核准任務.</p> <p>哪些使用者會收到此事件的電子郵件通知，取決於是否啟用「不需要核准者加入專案團隊（針對包含角色的核准程式）」設定(如 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">配置全局批准設定</a>)。 </p> <p>如果已啟用此選項</strong>，系統會以「核准者」工作角色傳送電子郵件通知給系統中的所有使用者。</p> <p>如果禁用此選項</strong>，只有具有「核准者」工作角色的專案團隊成員會收到電子郵件通知。</p> <p>只有在要求時專案狀態為「目前」時，才會傳送通知。</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務</p> </td> 
   <td> <p>給受委派核准者的任務未決核准</p> </td> 
   <td> <p>我需要審核我所受委派的任務核准.</p> <p>當某人將核發核准委派給其他使用者時，會通知該使用者。 </p> <p>只有在要求時專案狀態為「目前」時，才會傳送通知。</p> </td> 
   <td> <p>使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>時程表</p> </td> 
   <td> <p>使用者的時程表重新開啟</p> </td> 
   <td> <p>我的時程表已重新開啟.</p> <p>重新開啟工時單時，工時單所有者將收到電子郵件通知，除非重新開啟工時單的用戶也是工時單的所有者。</p> <p>僅當時間表狀態為「開啟」時，才會發送電子郵件通知。</p> <p>擁有審核許可證的用戶不會收到通知。</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>時程表</p> </td> 
   <td> <p>使用者的時程表拒絕</p> </td> 
   <td> <p>我的時程表已拒絕.</p> <p>拒絕工時單的用戶也是所有者，否則工時單所有者在工時單被拒絕時收到電子郵件通知。</p> <p>僅當時間表狀態為「拒絕」時，才會發送電子郵件通知。</p> <p>擁有審核許可證的用戶不會收到通知。</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>時程表</p> </td> 
   <td> <p>時程表提交給核准者</p> </td> 
   <td> <p>我需要提交時程表.</p> <p>提交需要批准的時間表時，時間表批准者會收到電子郵件通知，除非提交時間表的用戶也是時間表批准者。</p> <p>僅當已提交時間表狀態時才發送通知。</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>指派</p> </td> 
   <td> <p>對團隊的工作項目請求</p> </td> 
   <td> <p>我的團隊得到新的工作請求.</p> <p>團隊成員在收到新工作請求時會收到電子郵件通知。 （如果提交請求的使用者是團隊成員，則不會收到通知。）</p> <p>只有在提出工作請求時項目狀態為「當前」且工作請求狀態為「新」時，才會發送通知。</p> <p>擁有審核許可證的用戶不會收到通知。</p> </td> 
   <td> <p>使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>指派</p> </td> 
   <td> <p>給工作項目受指派人的工作項目請求</p> </td> 
   <td> <p>我得到一個新工作要求.</p> <p>工作項目的受託人會收到電子郵件通知，除非提出請求的使用者也是受託人。 </p> <p>如果任務狀態為「完成」或問題狀態為「關閉」，則不會發送通知。</p> <p>只有在要求時專案狀態為「目前」時，才會傳送通知。</p> <p>擁有審核許可證的用戶不會收到通知。</p> </td> 
   <td> <p>使用中</p> </td> 
  </tr> 
 </tbody> 
</table>

## 我提出的請求

另請參閱 [通知：我提出的請求](../../../workfront-basics/using-notifications/notifications-requests-i-have-made.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>物件類型</th> 
   <th>Event</th> 
   <th>說明</th> 
   <th> 預設狀態</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>文件</p> </td> 
   <td> <p>請求者的文件核准狀態變更</p> </td> 
   <td> <p>已完成一個文件核准請求.</p> <p>文檔請求者在完成文檔批准請求時接收電子郵件通知。</p> </td> 
   <td> <p>使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>文件</p> </td> 
   <td> <p>請求者的文件請求完成</p> </td> 
   <td> <p>文件上傳要求已完成.</p> <p>當上傳檔案的請求完成時，檔案請求者會收到電子郵件通知。</p> </td> 
   <td> <p>使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>問題</p> </td> 
   <td> <p>「問題新增」到「問題主要連絡人」</p> </td> 
   <td> <p>我想專案新增了問題.</p> <p>問題的主要連絡人在專案中新增問題時，會收到通知。</p> <p>僅當項目狀態為「當前」或「計畫」時，才會發送通知。</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td>問題</td> 
   <td>「問題指派」到「問題主要聯絡人」</td> 
   <td> <p>某位人員已指派到「我是主要聯絡人」的問題.</p> <p>問題的主要聯絡人會在將問題指派給使用者時收到通知。 </p> <p>僅當項目狀態為「當前」或「計畫」時，才會發送通知。</p> </td> 
   <td> 非使用中</td> 
  </tr> 
  <tr> 
   <td> <p>問題</p> </td> 
   <td> <p>「問題完成」到「問題主要連絡人」</p> </td> 
   <td> <p>我是主要連絡人的一個問題已完成.</p> <p>僅當項目狀態為「當前」或「計畫」時，才會發送通知。</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>專案</p> </td> 
   <td> <p>輸入者的專案狀態變更</p> </td> 
   <td> <p>在我建立的專案上變更了狀態.</p> <p>建立專案的使用者會在專案狀態變更時收到電子郵件通知。</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>問題</p> </td> 
   <td> <p>至問題主要連絡人的請求新增</p> </td> 
   <td> <p>我提交一個請求 (確認).</p> <p>問題的主要連絡人在提交問題時會收到電子郵件通知。</p> <p>僅當項目狀態為「當前」且項目使用「是幫助台」視圖時，才會發送通知。</p> </td> 
   <td> <p>使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>問題</p> </td> 
   <td> <p>至問題主要連絡人的請求指派</p> </td> 
   <td> <p>有人指派給我的請求.</p> <p>問題的主要聯繫人在將用戶分配給問題時收到電子郵件通知，除非主要聯繫人和分配的用戶是同一用戶。</p> <p>僅當項目狀態為「當前」且項目使用「是幫助台」視圖時，才會發送通知。</p> </td> 
   <td> <p>使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>問題</p> </td> 
   <td> <p>至問題主要連絡人的請求關閉</p> </td> 
   <td> <p>我的請求已關閉 (確認).</p> <p>請求關閉時，問題的主要聯絡人會收到電子郵件通知。</p> <p>僅當項目狀態為「當前」且項目使用「是幫助台」視圖時，才會發送通知。</p> <p>如果啟用「問題完成」通知，則一律會觸發，而非「關閉給問題主要聯絡人的請求」。 如果您希望觸發此通知，您必須停用「問題完成」通知。</p> </td> 
   <td> <p>使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>文件</p> </td> 
   <td> <p>至問題主要連絡人的請求文件新增</p> </td> 
   <td> <p>在一項我為主要連絡人的問題中已變更或上傳一個文件.</p> <p>當文檔被上載或更改時，問題的主要聯繫人會收到電子郵件通知，除非上傳或更改文檔的用戶也是主要聯繫人。</p> <p>僅當項目狀態為「當前」，並且項目在「隊列設定」頁簽上啟用了「以幫助請求隊列形式發佈」，才會發送通知。</p> </td> 
   <td> <p>使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>問題</p> </td> 
   <td> <p>至問題主要連絡人的服務台要求狀態變更</p> </td> 
   <td> <p>我的請求上的狀態變更.</p> <p>問題的主要聯絡人在問題狀態變更時收到電子郵件通知，除非變更狀態的使用者也是主要聯絡人。</p> <p>僅當項目狀態為「當前」且項目使用「是幫助台」視圖時，才會發送通知。</p> </td> 
   <td> <p>使用中</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE:
       For more information on publishing a project as a Help Request Queue, see 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>.-->

## 溝通

另請參閱 [通知：通訊](../../../workfront-basics/using-notifications/notifications-communication.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>物件類型</th> 
   <th>Event</th> 
   <th>說明</th> 
   <th> 預設狀態</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>文件</p> </td> 
   <td> <p>文檔對文檔所有者的評論</p> </td> 
   <td> <p>一個註解已新增在我的文件.</p> <p>Workfront中檔案的擁有者會在檔案上張貼留言時收到電子郵件通知，除非張貼留言的使用者也是檔案擁有者。</p> <p>直接包含在註解中的任何使用者也會收到電子郵件通知。</p> <p>只有在專案狀態為「目前」時，才會傳送通知。 </p> <p>即時通知電子郵件的主旨是： <em>評論 &lt;request name=""&gt; on &lt;project name=""&gt; （參考編號） &lt;request reference="" number=""&gt;)</em></p> <p> 每日摘要通知的主旨是：<em> 通信摘要 &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>使用中 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>備註</p> </td> 
   <td> <p>至問題主要連絡人的請求備註新增</p> </td> 
   <td> <p>在請求上張貼意見時，請傳送電子郵件給問題主要聯絡人。</p> <p>問題的主要聯絡人在請求上張貼評論時會收到電子郵件通知，除非張貼評論的使用者也是問題的主要聯絡人。</p> <p>直接包含在評論中的任何使用者也會收到電子郵件通知。</p> <p>只有在專案狀態為「目前」時，才會傳送通知。</p> </td> 
   <td> <p>使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>使用者</p> </td> 
   <td>定向更新至用戶</td> 
   <td> <p>有人將我加入定向更新.</p> <p>定向更新是指當用戶在更新中特別包括另一個用戶時，如 <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">在更新時標籤其他人</a>.</p> <p>在此情況下，包含在定向更新中的使用者會收到有關更新的電子郵件通知。</p> <p>只有在使用者擁有物件的存取權限，且在其設定檔中將其保持啟用時，才會傳送電子郵件通知。  </p> <p>此事件通知預設為啟用，無法停用。</p> </td> 
   <td> <p>使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>團隊</p> </td> 
   <td> <p>定向更新至團隊</p> </td> 
   <td> <p>有人將我的團隊加入定向更新.</p> <p>定向更新是指當用戶在更新中特別包括另一個用戶時，如 <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">在更新時標籤其他人</a>.</p> <p>在此情況下，包含在定向更新中的團隊的任何成員都會收到有關更新的電子郵件通知。</p> <p>電子郵件通知只會傳送給具有更新物件存取權限的使用者。</p> <p>如果發送定向更新的用戶是所包括團隊的成員，則發送更新的用戶不會收到電子郵件通知。</p> </td> 
   <td> <p>使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>備註</p> </td> 
   <td> <p>執行緒參與者的工作項目註解</p> </td> 
   <td> <p>有人對我所在的執行緒發表了註解.</p> <p>執行緒中的參與者和包含在直接訊息中的使用者，會在使用者在執行緒中留言時收到電子郵件通知。</p> <p>使用者必須有檢視存取權才能接收通知。</p> <p>下列使用者不會收到通知：</p> 
    <ul> 
     <li> <p>包含在直接訊息中的團隊</p> </li> 
     <li> <p>票據的所有者</p> </li> 
     <li> <p>主要聯繫人</p> </li> 
    </ul> </td> 
   <td> <p>使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>備註</p> </td> 
   <td> <p>給工作項目受指派人的工作項目註解</p> </td> 
   <td> <p>有人對我其中一個工作項目發表評論.</p> <p>工作項目的受託人在用戶向工作項添加更新時收到電子郵件通知，除非添加更新的用戶也是受託人。</p> </td> 
   <td> <p>使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>備註</p> </td> 
   <td> <p>對工作請求者的工作請求回覆</p> </td> 
   <td> <p>有人回覆了我的請求.</p> <p>在用戶提交請求並且其他用戶答復該請求之後，提交請求的用戶將收到電子郵件通知。</p> <p>如果下列情況，則不會傳送電子郵件通知：</p> 
    <ul> 
     <li> <p>回覆的使用者與提出請求的使用者相同</p> </li> 
     <li> <p>使用者無權查看附註</p> </li> 
    </ul> </td> 
   <td> <p>使用中</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE: for the directed update above, it also mentions:
        ... and is not the same user that enters the update-->

## 核准資訊

另請參閱 [通知：核准資訊](../../../workfront-basics/using-notifications/notifications-approval-information.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>物件類型</th> 
   <th>Event</th> 
   <th>說明</th> 
   <th> 預設狀態</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>使用者</p> </td> 
   <td> <p>給其他使用者的核准委派</p> </td> 
   <td> <p>我受委派為核准者.</p> </td> 
   <td> <p>使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>問題</p> </td> 
   <td> <p>受委派問題核准狀態變更</p> </td> 
   <td> <p>受委派問題核准要求已完成. </p> <p>當您將核發核准委派給其他人時，當他們完成核准（無論他們是否核准核發核准），您都會收到電子郵件通知。 </p> </td> 
   <td> <p>使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>專案</p> </td> 
   <td> <p>受委派專案核准狀態變更</p> </td> 
   <td> <p>受委派專案核准要求已完成.</p> <p>當您將項目批准委託給其他人時，當他們完成該批准時（無論他們是批准還是拒絕項目批准），您都會收到電子郵件通知。</p> </td> 
   <td> <p>使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務</p> </td> 
   <td> <p>受委派任務核准狀態變更</p> </td> 
   <td> <p>已完成委派的任務批准狀態。</p> <p>當您將任務批准委派給其他人時，當他們完成該批准時（無論他們是批准還是拒絕任務批准），您都會收到電子郵件通知。</p> </td> 
   <td> <p>使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>文件</p> </td> 
   <td> <p>核准者的文件核准取消</p> </td> 
   <td> <p>文件核准請求已取消.</p> <p>取消文檔批准請求時，文檔的文檔批准者將收到電子郵件通知。</p> </td> 
   <td> <p>使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>時程表</p> </td> 
   <td> <p>「使用者」的「時程表核准」</p> </td> 
   <td> <p>我的時程表已核准.</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
 </tbody> 
</table>

## 關於分配給我的工作的資訊

另請參閱 [通知：關於分配給我的工作的資訊](../../../workfront-basics/using-notifications/notifications-information-about-work-assigned-to-me.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>物件類型</th> 
   <th>Event</th> 
   <th>說明</th> 
   <th> 預設狀態</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>任務</td> 
   <td>「所有前置任務完成」到「所指派團隊的任務依存性」</td> 
   <td> <p>該團隊的所有前任任務均已完成。</p> <p>任務受分配者（團隊的所有成員）會收到電子郵件通知。</p> <p>擁有審核許可證的用戶不會收到通知。</p> </td> 
   <td>非使用中</td> 
  </tr> 
  <tr> 
   <td> <p>任務</p> </td> 
   <td> <p>「所有前置任務完成」到「任務依存性」</p> </td> 
   <td> <p>我的任務之所有前置任務已完成.</p> <p>任務受託人會收到電子郵件通知。</p> <p>擁有審核許可證的用戶不會收到通知。</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>問題</p> </td> 
   <td> <p>核准決策以發放指派給</p> </td> 
   <td> <p>我要解決的問題已核准或已拒絕.</p> <p>問題的受託人會在做出核准決定（核准或拒絕）時收到電子郵件通知。</p> <p>擁有審核許可證的用戶不會收到通知。</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務</p> </td> 
   <td> <p>分配給任務的審批決策</p> </td> 
   <td> <p>我要完成的一項任務已核准或已拒絕.</p> <p>任務受託人在批准或拒絕任務時收到電子郵件通知。</p> <p>只有在專案狀態為「目前」時，才會傳送通知。</p> <p>擁有審核許可證的用戶不會收到通知。</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>問題</p> </td> 
   <td> <p>「問題完成」到「問題受指派者」</p> </td> 
   <td> <p>指派給我的一個問題已完成.</p> <p>僅當項目狀態為「當前」或「計畫」時，才會發送通知。</p> <p>擁有審核許可證的用戶不會收到通知。</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>問題</p> </td> 
   <td> <p>問題計畫完成日期已變更</p> </td> 
   <td> <p>在指派給我的問題上變更到期日期.</p> <p>問題受託人在計畫完成日期更改時收到電子郵件通知，除非更改計畫完成日期的用戶也是受託人。</p> <p>僅當項目狀態為Planning以外的任何狀態時，才會發送通知。</p> </td> 
   <td> <p>使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>問題</p> </td> 
   <td> <p>至「問題受指派者」的問題狀態變更</p> </td> 
   <td> <p>我的工作項目之一的狀態變更.</p> <p>問題的受託人會在狀態變更時收到電子郵件通知，除非變更狀態的使用者也是受託人。</p> <p>只有在專案狀態為「目前」時，才會傳送通知。</p> <p>擁有審核許可證的用戶不會收到通知。</p> </td> 
   <td> <p>使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>文件</p> </td> 
   <td> <p>至問題受指派者的請求文件新增</p> </td> 
   <td> <p>根據我的請求上傳或變更了文件.</p> <p>當檔案上傳或因新增的問題而變更時，問題受託人會收到電子郵件通知。</p> <p>如果輸入問題的使用者是問題受託人，則不會傳送電子郵件通知。</p> <p>僅當項目狀態為「當前」，並且項目在「隊列設定」頁簽上啟用了「以幫助請求隊列形式發佈」，才會發送通知。</p> </td> 
   <td> <p>使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務</p> </td> 
   <td> <p>「任務受指派者」的「任務完成」</p> </td> 
   <td> <p>指派給我的一項任務已完成.</p> <p>任務受託人在任務完成時收到電子郵件通知。 完成個人任務時不會發送通知。</p> <p>只有在專案狀態為「目前」時，才會傳送通知。</p> <p>擁有審核或請求者授權的使用者不會收到通知。</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務</p> </td> 
   <td> <p>「任務從屬項」的「任務完成」</p> </td> 
   <td> <p>我的其中一項任務的前置任務已完成.</p> <p>當任務的其中一個前置任務完成時，任務受託人將收到電子郵件通知。</p> <p>擁有審核許可證的用戶不會收到通知。</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務</p> </td> 
   <td> <p>任務計畫完成日期已變更</p> </td> 
   <td> <p>在指派給我的一項任務上變更了到期日期.</p> <p>當任務的「計畫完成日期」更改時，任務受分配人會收到電子郵件通知，除非更改了「計畫完成日期」的用戶也是任務受分配人。</p> <p>僅當項目狀態為Planning以外的任何狀態時，才會發送通知。</p> <p>不會傳送有關個人任務的通知。</p> </td> 
   <td> <p>使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務</p> </td> 
   <td> <p>受指派者的任務狀態變更</p> </td> 
   <td> <p>一項指派給我的任務狀態發生變更.</p> <p>任務受託人在任務狀態更改時收到電子郵件通知，除非更改了狀態的用戶也是受託人。</p> <p>只有在專案狀態為「目前」時，才會傳送通知。</p> <p>擁有審核許可證的用戶不會收到通知。 </p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE: from the Request document add to issue assigned to: 
        For more information on publishing a project as a Help Request Queue, see 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>. -->

## 關於我正在執行的項目的資訊

另請參閱 [通知：關於我正在執行的項目的資訊](../../../workfront-basics/using-notifications/notifications-information-about-projects-im-on.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>物件類型</th> 
   <th>Event</th> 
   <th>說明</th> 
   <th> 預設狀態</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>專案</p> </td> 
   <td> <p>專案團隊的目前的專案狀態變更</p> </td> 
   <td> <p>我所在的一個專案變為使用中專案.</p> <p>專案的使用者會在專案生效時收到電子郵件通知。</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>文件</p> </td> 
   <td> <p>文件新增到專案團隊</p> </td> 
   <td> <p>向我所在的專案新增一個文件.</p> <p>將檔案新增至專案時，專案團隊中的使用者會收到電子郵件通知，但新增檔案的使用者除外。</p> <p>只有在項目狀態為「當前」且文檔不為「專用」時，才會發送通知。 </p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>問題</p> </td> 
   <td> <p>「問題新增」到「專案團隊」</p> </td> 
   <td> <p>向我所在的專案新增了一個問題.</p> <p>將問題新增至專案時，專案中的使用者會收到電子郵件通知。</p> <p>只有在專案狀態為「目前」時，才會傳送通知。</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>問題</p> </td> 
   <td> <p>專案團隊的問題完成</p> </td> 
   <td> <p>在我所在的專案上完成了一個問題.</p> <p>專案上的任何使用者都會收到通知。</p> <p>僅當項目狀態為「當前」或「計畫」時，才會發送通知。</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務</p> </td> 
   <td> <p>至「專案團隊」的「里程碑任務完成」</p> </td> 
   <td> <p>在我所在的專案上完成了里程碑任務.</p> <p>項目組中的所有用戶在里程碑任務完成時都會收到通知。 </p> <p>僅當項目狀態為「當前」或「計畫」時，才會發送通知。</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>專案</p> </td> 
   <td> <p>「專案團隊」的「專案完成」</p> </td> 
   <td> <p>我所在的專案已完成.</p> <p>專案狀態為「完成」時，專案團隊的使用者會收到電子郵件通知。</p> <p>提示：如果項目定期完成，則啟用此選項可以為在許多項目上任務有限的用戶建立大量電子郵件。 </p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>專案</p> </td> 
   <td> <p>專案團隊的專案狀態變更</p> </td> 
   <td> <p>在我所在的專案上變更了狀態.</p> <p>專案團隊的使用者會在專案狀態變更時收到電子郵件通知。 </p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>專案使用者</p> </td> 
   <td> <p>專案使用者的專案使用者新增</p> </td> 
   <td> <p>我被新增到一個專案.</p> <p>已新增至專案的使用者新增時，會收到電子郵件通知，除非已將使用者自行新增至專案。</p> <p>只有在專案狀態為「目前」時，才會傳送通知。</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務</p> </td> 
   <td> <p>「專案團隊」的「任務完成」</p> </td> 
   <td> <p>在我所在的專案上完成了一項任務.</p> <p>專案團隊的成員會收到電子郵件通知。</p> <p>只有在專案狀態為「目前」時，才會傳送通知。</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>問題</p> </td> 
   <td> <p>至專案團隊的未指派問題新增</p> </td> 
   <td> <p>向我所在的專案新增了一個未指派問題.</p> <p>將未指派的問題新增至專案時，專案的使用者會收到電子郵件通知。</p> <p>只有在專案狀態為「目前」時，才會傳送通知。</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
 </tbody> 
</table>

## 我擁有之專案的相關資訊

另請參閱 [通知：我擁有之專案的相關資訊](../../../workfront-basics/using-notifications/notifications-information-about-projects-i-own.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>物件類型</th> 
   <th>Event</th> 
   <th>說明</th> 
   <th> 預設狀態</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>文件</p> </td> 
   <td> <p>文件新增到專案所有者</p> </td> 
   <td> <p>向我持有的專案新增一個文件.</p> <p>將文檔添加到項目時，項目所有者將收到電子郵件通知，除非添加文檔的用戶也是項目所有者。</p> <p>只有在項目狀態為「當前」且文檔不為「專用」時，才會發送通知。</p> <p>擁有審核許可證的用戶不會收到通知。</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>問題</p> </td> 
   <td> <p>「問題新增」到「專案所有者」</p> </td> 
   <td> <p>向我持有的專案新增了一個問題.</p> <p>將問題新增至專案時，專案擁有者會收到電子郵件通知。</p> <p>僅當項目狀態為「當前」或「計畫」時，才會發送通知。</p> <p>擁有審核許可證的用戶不會收到通知。</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>問題</p> </td> 
   <td> <p>將問題認可日期變更傳送給專案所有者</p> </td> 
   <td> <p>認可日期因我專案上的一個問題變更.</p> <p>項目所有者在項目問題的「提交日期」更改時收到電子郵件通知，除非更改「提交日期」的用戶與項目所有者相同。</p> </td> 
   <td> <p>使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>問題</p> </td> 
   <td> <p>問題完成到專案所有者</p> </td> 
   <td> <p>在我持有的專案上完成了一個問題.</p> <p>專案擁有者會收到電子郵件通知。</p> <p>僅當項目狀態為「當前」或「計畫」時，才會發送通知。</p> <p>擁有審核許可證的用戶不會收到通知。</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務</p> </td> 
   <td> <p>「里程碑任務完成」到「專案所有者」</p> </td> 
   <td> <p>在我持有的專案上完成了里程碑任務.</p> <p>僅當項目狀態為「當前」或「計畫」時，才會發送通知。</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>專案</p> </td> 
   <td> <p>專案所有者的專案所有者指派</p> </td> 
   <td> <p>我被設為新專案的所有者.</p> <p>將使用者指派為專案的擁有者時，該使用者會收到電子郵件通知。</p> <p>如果專案擁有者是進行指派的相同使用者，則不會傳送電子郵件通知</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>專案</p> </td> 
   <td> <p>專案所有者的專案進度變更</p> </td> 
   <td> <p>我持有的專案落後.</p> <p>專案擁有者會在專案延遲時收到電子郵件通知。</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務</p> </td> 
   <td> <p>專案所有者的任務認可日期變更</p> </td> 
   <td> <p>我的其中一項專案上的任務認可日期變更.</p> <p>項目所有者在項目上某項任務的「提交日期」更改時收到電子郵件通知，除非更改了「提交日期」的用戶也是項目所有者。</p> </td> 
   <td> <p>使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務</p> </td> 
   <td> <p>專案所有者的任務完成</p> </td> 
   <td> <p>在我持有的專案上完成了一項任務.</p> <p>專案擁有者會收到通知。 </p> <p>只有在專案狀態為「目前」時，才會傳送通知。</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務</p> </td> 
   <td> <p>任務所有者的專案進度變更</p> </td> 
   <td> <p>我持有專案上的一項任務落後.</p> <p>專案擁有者會在專案上的任務落後時收到電子郵件通知。</p> <p>只有在專案狀態為「目前」時，才會傳送通知。</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>問題</p> </td> 
   <td> <p>至專案所有者的未指派問題新增</p> </td> 
   <td> <p>向我持有的專案新增未指派的問題.</p> <p>將未指派的問題新增至專案時，專案擁有者會收到電子郵件通知。</p> <p>僅當項目狀態為「當前」或「計畫」時，才會發送通知。</p> <p>擁有審核許可證的用戶不會收到通知。</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
 </tbody> 
</table>

## 關於我贊助的項目的資訊

另請參閱 [通知：關於我贊助的項目的資訊](../../../workfront-basics/using-notifications/notifications-information-about-projects-i-sponsor.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>物件類型</th> 
   <th>Event</th> 
   <th>說明</th> 
   <th> 預設狀態</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>文件</p> </td> 
   <td> <p>文件新增到專案贊助者</p> </td> 
   <td> <p>向我贊助的專案新增一個文件.</p> <p>項目發起人在將文檔添加到項目時收到電子郵件通知，除非該文檔由項目發起人添加。</p> <p>僅當項目狀態為「當前」且文檔不為「專用」時，才會發送通知。</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>問題</p> </td> 
   <td> <p>專案贊助者的問題新增</p> </td> 
   <td> <p>向我贊助的專案新增了一個問題.</p> <p>將問題新增至專案時，專案贊助商會收到電子郵件通知。</p> <p>僅當項目狀態為「當前」或「計畫」時，才會發送通知。</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>問題</p> </td> 
   <td> <p>專案贊助者的問題完成</p> </td> 
   <td> <p>在我贊助的專案上完成了一個問題.</p> <p>專案贊助商會收到電子郵件通知。</p> <p>僅當項目狀態為「當前」或「計畫」時，才會發送通知。</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務</p> </td> 
   <td> <p>專案贊助者的里程碑任務完成</p> </td> 
   <td> <p>在我贊助的專案上完成里程碑任務.</p> <p>當項目贊助者所贊助的項目完成里程碑任務時，項目贊助者會收到電子郵件通知。</p> <p>僅當項目狀態為「當前」或「計畫」時，才會發送通知。</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>專案</p> </td> 
   <td> <p>專案贊助者的專案進度變更</p> </td> 
   <td> <p>我贊助的專案落後.</p> <p>當專案落後時，專案贊助人會收到電子郵件通知。</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>專案</p> </td> 
   <td> <p>專案贊助者的專案贊助者指派</p> </td> 
   <td> <p>我被設為專案贊助者.</p> <p>當項目贊助者被設定為項目贊助者時，項目贊助者會收到電子郵件通知。</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務</p> </td> 
   <td> <p>專案贊助者的任務完成</p> </td> 
   <td> <p>在我贊助的專案上完成了一項任務.</p> <p>專案贊助商會收到電子郵件通知。</p> <p>只有在專案狀態為「目前」時，才會傳送通知。</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務</p> </td> 
   <td> <p>專案贊助者的任務進度變更</p> </td> 
   <td> <p>我贊助專案上的一項任務落後.</p> <p>當項目上的任務超出計畫時，項目贊助商會收到電子郵件通知。</p> <p>只有在專案狀態為「目前」時，才會傳送通知。</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>問題</p> </td> 
   <td> <p>專案贊助者的未指派的問題新增</p> </td> 
   <td> <p>向我贊助的專案新增了一個未指派問題.</p> <p>當未指派的問題新增至專案時，專案贊助商會收到電子郵件通知。</p> <p>僅當項目狀態為「當前」或「計畫」時，才會發送通知。</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
 </tbody> 
</table>

## 其他資訊

另請參閱 [通知：其他資訊](../../../workfront-basics/using-notifications/notifications-misc-information.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>物件類型</th> 
   <th>Event</th> 
   <th>說明</th> 
   <th> 預設狀態</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>宣告</td> 
   <td> <p>已新增宣告</p> </td> 
   <td> <p>已將一則訊息傳送至 Announcement Center.</p> </td> 
   <td> <p>使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>文件</p> </td> 
   <td> <p>請求者的文件請求取消</p> </td> 
   <td> <p>取消我的檔案上傳請求。</p> <p>取消文檔請求時，文檔請求會收到電子郵件通知。</p> </td> 
   <td> <p>使用中</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>錯誤通知</p> </td> 
   <td> <p>發現需要注意的錯誤。</p> <p>Workfront嘗試且無法連線至POP帳戶後，會產生電子郵件通知。 25次嘗試後，Workfront會停用與POP帳戶的連線，以保留資源並傳送通知。 </p> <p>如果POP電子郵件與請求隊列關聯，則電子郵件通知將發送給項目所有者；如果POP帳戶與「電子郵件設定」中的「傳入郵件」功能關聯，則電子郵件通知將發送給Workfront管理員。
   </p> </td> 
   <td> <p>使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>問題</p> </td> 
   <td> <p>問題指派到資源所有者</p> </td> 
   <td> <p>問題指派變更影響了我的一名人員.</p> <p>當變更影響其管理的使用者時，「問題受託人管理員」會收到電子郵件通知。</p> <p>僅當項目狀態為「當前」或「計畫」時，才會發送通知。</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>使用者</p> </td> 
   <td> <p>使用者的新使用者</p> </td> 
   <td> <p>在 Workfront 中建立新使用者之後，傳送電子郵件給使用者.</p> <p>建立新使用者後，使用者會收到電子郵件邀請，通知他們已建立Workfront帳戶，並提示他們設定密碼。</p> <p>建立新使用者時，使用者可以選取「傳送邀請電子郵件給此人」選項(如 <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">新增使用者</a><span style="font-weight: 400;">)。 不過，當全域啟用「新使用者對使用者」選項時，無論是否選取「傳送邀請電子郵件給此人」選項，所有新使用者都會收到電子郵件邀請。</span></p> </td> 
   <td> 非使用中 </td> 
  </tr> 
  <tr> 
   <td> <p>團隊</p> </td> 
   <td> <p>分享物件至團隊</p> </td> 
   <td> <p>有人員與我的團隊共用一個物件.</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>使用者</p> </td> 
   <td> <p>分享物件至使用者</p> </td> 
   <td> <p>某人員與我共用一個物件.</p> </td> 
   <td> <p>使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>專案使用者</p> </td> 
   <td> <p>資源所有者的專案使用者新增</p> </td> 
   <td> <p>我的一名人員新增至一個專案.</p> <p>當經理的其中一個直接報表新增至專案時，經理會收到電子郵件通知。</p> <p>擁有審核許可證的用戶不會收到通知。</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>專案</p> </td> 
   <td> <p>新增至投資組合或計劃中的專案</p> </td> 
   <td> <p>某人將專案新增至我所擁有的投資組合或計劃之中.</p> </td> 
   <td> <p>使用中</p> </td> 
  </tr> 
  <tr> 
   <td> <p>任務</p> </td> 
   <td> <p>任務指派到資源所有者</p> </td> 
   <td> <p>任務指派變更影響了我的一名人員.</p> <p>任務受託人的經理會收到電子郵件通知。</p> <p>只有在專案狀態為「目前」時，才會傳送通知。</p> </td> 
   <td> <p>非使用中</p> </td> 
  </tr> 
  <tr> 
   <td> 專案 <br>任務 <br>問題</td> 
   <td>訂閱者的新更新 </td> 
   <td> <p class="p1"><span class="s1 wysiwyg-font-size-medium">當我訂閱的任務、問題或專案進行更新時，會傳送電子郵件。</span> </p> </td> 
   <td>使用中</td> 
  </tr> 
 </tbody> 
</table>

<!--
      DRAFTED IN FLARE: from Error notification above: 
      
       <br>For more information on how to associate a request queue with a POP account, see 
       <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>.
       For more information on how to enable a POP account for incoming mail, see .
      -->

## 委派

另請參閱 [通知：委派](../../../workfront-basics/using-notifications/notifications-delegation.md).

| 物件類型 | Event | 說明 | 預設狀態 |
|------------------|---------------------------------------------|--------------------------------------------------------------|---------------|
| 任務和問題 | 將任務和問題委派給受託人 | 我委派我的任務和問題 (確認) | 使用中 |
| 任務和問題 | 停止將任務和問題委派給受託人 | 我停止委派我的任務和問題 (確認) | 使用中 |
| 任務和問題 | 將任務和問題委派給代理人 | 有人將其任務和問題委派給我 | 使用中 |
| 任務和問題 | 停止任務和要委派的問題委派 | 有人停止將其任務和問題委派給我 | 使用中 |
