---
content-type: reference
navigation-topic: notifications
title: '通知：通訊'
description: 下列通知會提醒您有關您參與的工作專案上發生的通訊，例如更新註解。 如需有關設定您收到哪些通知的資訊，請參閱修改您自己的電子郵件通知。
author: Lisa
feature: Get Started with Workfront
exl-id: 473e1760-f85a-4622-beff-9431046d655e
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1530'
ht-degree: 0%

---

# 通知：通訊

下列通知會提醒您有關您參與的工作專案上發生的通訊，例如更新註解。 如需有關設定您收到哪些通知的資訊，請參閱[修改您自己的電子郵件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)。

>[!NOTE]
>
>這些通知會提醒您特定專案上已張貼的所有評論。 因此，您必須同時選取或取消選取所有通知，才能在每日摘要電子郵件中傳送。 如果您只想在發生某些評論時收到通知，您可以指定立即傳送的個別通知。

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
   <td> <p><strong>有人將我加入定向更新</strong> </p> <p>定向更新是指當使用者在更新中明確包含另一個使用者時，如<a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">[！UICONTROL在]更新</a>上標籤其他使用者中所述。</p> <p>在這種情況下，包含在定向更新中的使用者會收到有關更新的電子郵件通知。</p> <p>只有當使用者擁有物件的存取許可權時，才會傳送電子郵件通知。</p> <p>即時通知電子郵件的主旨為： <em>&lt;將您包含在更新中的使用者名稱&gt; [！UICONTROL希望您知道]</em></p> <p>每日摘要通知的主旨為： <em>[！UICONTROL通訊摘要] &lt;每日摘要的日期&gt;</em></p> </td> 
   <td> 進行更新的物件名稱<br>父物件名稱<br>物件參考編號<br>包含在定向更新中的所有使用者和團隊的名稱<br>進行更新的日期和時間<br>定向更新的文字<br><strong>[！UICONTROL註解]</strong> button<br>*收到的註解總數<br>*每個物件收到的註解數<br>*<strong>[！UICONTROL檢視所有通知]</strong>按鈕<br>*每日摘要的日期<br></td> 
   <td> <p><strong>即時</strong> </p> <p><strong>和每日</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>某人回覆我的請求</strong> </p> <p>當使用者提交工作請求且另一個使用者回覆該工作請求後，提交請求的使用者會收到電子郵件通知。</p> <p>在下列情況下，不會傳送電子郵件通知：</p> 
    <ul> 
     <li> <p>回覆的使用者與提出要求的使用者相同</p> </li> 
     <li> <p>使用者沒有檢視附註的許可權</p> </li> 
    </ul><strong>即時通知電子郵件的主旨為： <em>[！UICONTROL註解： on] &lt;Request Name&gt; on &lt;Project Name&gt; (ref# &lt;Request Reference Number&gt;)</em></strong>每日摘要通知的主旨為：<em> [！UICONTROL通訊摘要] &lt;每日摘要的日期&gt;</em></td> 
   <td> 要求名稱<br>專案名稱<br>參考編號<br>回覆您要求的使用者名稱<br>發表評論的日期和時間<br>在您的要求上發表的評論文字<br>*收到的評論總數<br>*每個要求收到的評論總數<br>*<strong>[！UICONTROL檢視所有通知]</strong>按鈕<br>*每日摘要的日期<br></td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我的要求已張貼一個註解</strong> </p> <p>在[！UICONTROL服務檯]請求上張貼評論時，問題的主要聯絡人會收到電子郵件通知，除非張貼評論的使用者也是問題的主要聯絡人。</p> <p>直接包含在評論中的任何使用者都會收到電子郵件通知。</p> <p>只有在專案狀態為[！UICONTROL目前]時，才會傳送通知。</p> <p>即時通知電子郵件的主旨為： <em>[！UICONTROL Comment on] &lt;Request Name&gt; on &lt;Project Name&gt; (ref# &lt;Request Reference Number&gt;)</em></p> <p>每日摘要通知的主旨為：<em> [！UICONTROL通訊摘要] &lt;每日摘要的日期&gt;</em></p> </td> 
   <td> 要求名稱<br>專案名稱<br>參考編號<br>回覆您要求的使用者名稱<br>發表評論的日期和時間<br>在您的要求上發表的評論文字<br>*收到的評論總數<br>*每個要求收到的評論總數<br>*專案名稱<br>*<strong>[！UICONTROL檢視所有通知]</strong>按鈕<br>*每日摘要的日期<br></td> 
   <td> <p><strong>即時</strong> </p> <p><strong>和每日</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我的檔案已新增註解</strong> </p> <p>在檔案上張貼評論時，[!DNL Adobe Workfront]中檔案的擁有者會收到電子郵件通知，除非張貼評論的使用者也是檔案擁有者。</p> <p>直接包含在評論中的任何使用者都會收到電子郵件通知。</p> <p>只有在專案狀態為[！UICONTROL目前]時，才會傳送通知。 </p> <p>即時通知電子郵件的主旨為： <em>[！UICONTROL Comment on] &lt;Request Name&gt; on &lt;Project Name&gt; (ref# &lt;Request Reference Number&gt;)</em></p> <p> 每日摘要通知的主旨為：<em> [！UICONTROL通訊摘要] &lt;每日摘要的日期&gt;</em></p> </td> 
   <td>檔名稱<br>專案、任務或問題名稱<br>參考號碼<br>回覆您請求的使用者名稱<br>發表評論的日期和時間<br>在檔案上發表評論的文字</td> 
   <td> <p><strong>即時</strong> </p> <p><strong>和每日</strong> </p> <p><strong></strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>有人對我所在的執行緒發表評論</strong> </p> <p>對話串中的參與者和直接訊息中所包含的使用者，會在使用者在對話串中發表評論時收到電子郵件通知。</p> <p>使用者必須擁有[！UICONTROL檢視]存取權才能接收通知。</p> <p>下列使用者未收到通知：</p> 
    <ul> 
     <li>直接訊息中包含的團隊</li> 
     <li>附註的擁有者</li> 
     <li>主要連絡人</li> 
    </ul> <p><strong>即時通知電子郵件的主旨為： <em>[！UICONTROL RE：註解於] &lt;專案名稱&gt;（ref# &lt;物件參考編號&gt;</em>）</strong>上的&lt;物件名稱&gt;&lt;物件型別&gt; </p> <p><strong>每日摘要通知的主旨為：<em> [！UICONTROL通訊摘要] &lt;每日摘要的日期&gt;</em></strong> </p> </td> 
   <td> 物件名稱<br>父物件名稱<br>對對話串發表評論的使用者名稱<br>對對話串發表評論的文字<br>發表評論的日期和時間<br>*收到的評論總數<br>*每個物件收到的評論數<br>*專案名稱<br>*<strong>[！UICONTROL檢視所有通知]</strong>按鈕<br>*每日摘要的日期 </td> 
   <td><strong>[！UICONTROL每日]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>有人對我其中一個工作專案發表評論</strong> </p> <p>工作專案的受指派人會在使用者新增更新至工作專案時收到電子郵件通知，除非新增更新的使用者也是受指派人。 </p> <p>當請求中張貼評論時，請傳送電子郵件給問題主要連絡人。</p> <p>當在請求上張貼評論時，問題的主要聯絡人會收到電子郵件通知，除非張貼評論的使用者也是問題的主要聯絡人。</p> <p>直接包含在評論中的任何使用者都會收到電子郵件通知。</p> <p>即時通知電子郵件的主旨為： <em>[！UICONTROL Comment on] &lt;Work Item Name&gt; on &lt;Project Name (ref# &lt;Work Item Reference Number&gt;)</em></p> <p> 每日摘要通知的主旨為：<em> [！UICONTROL通訊摘要] &lt;每日摘要的日期&gt;</em></p> </td> 
   <td> 工作專案名稱<br>專案名稱<br>工作專案參考編號<br>對工作專案發表評論的使用者名稱<br>對工作專案發表評論的文字<br>發表評論的日期和時間<br>*收到的評論總數<br>*每個物件收到的評論數<br>*專案名稱<br>*<strong>[！UICONTROL檢視所有通知]</strong>按鈕<br>*每日摘要的日期 </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>有人將我的團隊加入定向更新</strong> </p> <p>定向更新是指當使用者在更新中明確包含另一個使用者時，如<a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">在更新上標籤其他使用者</a>中所述。</p> <p>在這種情況下，定向更新中包含的團隊任何成員都會收到有關更新的電子郵件通知。</p> <p>電子郵件通知只會傳送給具有物件存取許可權的使用者。</p> <p>如果傳送定向更新的使用者是要包含的團隊成員，則傳送更新的使用者不會收到電子郵件通知。</p> <p>即時通知電子郵件的主旨為： [！UICONTROL Comment on] &lt;Object name&gt; on &lt;Parent Object Name&gt; (ref# &lt;Object Reference Number&gt;)</p> <p> 每日摘要通知的主旨為：<em> [！UICONTROL通訊摘要] &lt;每日摘要的日期&gt;</em></p> </td> 
   <td> <p>物件名稱<br>父物件名稱<br>物件參考編號<br>進行導向更新的使用者名稱<br>包含在導向更新中的所有團隊和使用者的名稱<br>進行導向更新的日期和時間<br>導向更新的文字<br><strong>[！UICONTROL Comment]</strong> button<br>*收到的評論總數<br>*每個物件收到的評論數<br>*專案名稱<br>*<strong>[！UICONTROL檢視所有通知]</strong>按鈕14}*每日摘要日期<br> </p> </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>當註解新增至使用者</strong>時 </p> <p>您可以在使用者物件的[！UICONTROL Updates]索引標籤中對使用者進行註解。 您也可以在編輯使用者的設定時對使用者進行註解。 作為評論對象的使用者會收到一封電子郵件，以通知他們此評論。 </p> <p>您必須擁有至少[！UICONTROL View]使用者的許可權，才能在使用者的[！UICONTROL Updates]索引標籤上輸入更新。 您必須具有使用者的[！UICONTROL Edit]許可權，才能編輯使用者的設定。 </p> <p>如需有關在[更新]索引標籤中對使用者進行評論的詳細資訊，請參閱<a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">更新工作</a>。</p> <p>有關編輯使用者的設定時輸入使用者評論的詳細資訊，請參閱<a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">設定我的設定</a>。</p> <p>即時通知電子郵件的主旨為： <em>&lt;使用者名稱&gt; [！UICONTROL希望您知道]</em></p> <p>每日摘要通知的主旨為：<em> [！UICONTROL通訊摘要] &lt;每日摘要的日期&gt;</em></p> </td> 
   <td> 您的使用者名稱<br>新增註解的使用者名稱<br>註解的文字<br>發表註解的日期和時間<br>*收到的註解總數<br>*每個物件收到的註解數<br>*<strong>[！UICONTROL檢視所有通知]</strong>按鈕<br>*每日摘要的日期 </td> 
   <td> <p><strong>即時</strong> </p> <p><strong>和每日</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
