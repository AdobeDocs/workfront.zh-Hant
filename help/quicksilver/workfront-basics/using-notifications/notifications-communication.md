---
content-type: reference
navigation-topic: notifications
title: '通知：通信'
description: 以下通知會提醒您有關您所涉及工作項目上發生的通信（如更新注釋）。 如需設定您收到哪些通知的相關資訊，請參閱啟用或停用您自己的事件通知。
author: Lisa
feature: Get Started with Workfront
exl-id: 473e1760-f85a-4622-beff-9431046d655e
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '1546'
ht-degree: 4%

---

# 通知：通訊

以下通知會提醒您有關您所涉及工作項目上發生的通信（如更新注釋）。 如需設定您收到哪些通知的詳細資訊，請參閱 [啟用或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>這些通知會提醒您注意已張貼在特定項目上的所有留言。 因此，您必須同時選取或取消選取所有通知，才能在每日摘要電子郵件中傳送。 如果您只想在某些留言發生時收到通知，您可以指定要立即傳送的個別通知。

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
   <td> <p><strong>有人將我加入定向更新</strong> </p> <p>定向更新是指當用戶在更新中特別包括另一個用戶時，如 <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">[!UICONTROL在]更新上標籤其他</a>.</p> <p>在此情況下，包含在定向更新中的使用者會收到有關更新的電子郵件通知。</p> <p>只有在使用者擁有物件的存取權限時，才會傳送電子郵件通知。</p> <p>即時通知電子郵件的主旨是： <em>&lt;name of="" the="" user="" who="" included="" you="" in="" the="" update=""&gt; [!UICONTROL希望您知道]</em></p> <p>每日摘要通知的主旨是： <em>[!UICONTROL通信摘要] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 進行更新的對象名<br>父對象名稱<br>對象引用編號<br>定向更新中包含的所有用戶和團隊的名稱<br>進行更新的日期和時間<br>定向更新的文本<br><strong>[!UICONTROL注釋]</strong> 按鈕<br>*收到的評論總數<br>*每個對象收到的注釋數<br>*<strong>[!UICONTROL查看所有通知]</strong> 按鈕<br>*每日摘要日期<br></td> 
   <td> <p><strong>立即</strong> </p> <p><strong>和每日</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>有人回覆了我的請求</strong> </p> <p>在用戶提交工作請求和其他用戶對該工作請求的答復之後，提交請求的用戶將收到電子郵件通知。</p> <p>如果下列情況，則不會傳送電子郵件通知：</p> 
    <ul> 
     <li> <p>回覆的使用者與提出請求的使用者相同</p> </li> 
     <li> <p>使用者無權查看附註</p> </li> 
    </ul><strong>即時通知電子郵件的主旨是： <em>[!UICONTROL對]的評論 &lt;request name=""&gt; on &lt;project name=""&gt; （參考編號） &lt;request reference="" number=""&gt;)</em></strong> 每日摘要通知的主旨是：<em> [!UICONTROL通信摘要] &lt;date of="" daily="" digest=""&gt;</em></td> 
   <td> 請求名稱<br>專案名稱<br>參考編號<br>回覆您請求的使用者名稱<br>評論的日期和時間<br>對您的請求所做評論的文本<br>*收到的評論總數<br>*每個請求收到的評論數<br>*<strong>[!UICONTROL查看所有通知]</strong> 按鈕<br>*每日摘要日期<br></td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>一個註解已公佈在我的要求上</strong> </p> <p>當在[!UICONTROL幫助台]請求上發佈評論時，問題的主要聯繫人會收到電子郵件通知，除非發佈評論的用戶也是問題的主要聯繫人。</p> <p>直接包含在註解中的任何使用者也會收到電子郵件通知。</p> <p>只有在專案狀態為[!UICONTROL目前]時，才會傳送通知。</p> <p>即時通知電子郵件的主旨是： <em>[!UICONTROL對]的評論 &lt;request name=""&gt; on &lt;project name=""&gt; （參考編號） &lt;request reference="" number=""&gt;)</em></p> <p>每日摘要通知的主旨是：<em> [!UICONTROL通信摘要] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 請求名稱<br>專案名稱<br>參考編號<br>回覆您請求的使用者名稱<br>評論的日期和時間<br>對您的請求所做評論的文本<br>*收到的評論總數<br>*每個請求收到的評論數<br>*專案名稱<br>*<strong>[!UICONTROL查看所有通知]</strong> 按鈕<br>*每日摘要日期<br></td> 
   <td> <p><strong>立即</strong> </p> <p><strong>和每日</strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>一個註解已新增在我的文件</strong> </p> <p>中的文檔的所有者 [!DNL Adobe Workfront] 在文檔上發佈評論時收到電子郵件通知，除非發佈評論的用戶也是文檔所有者。</p> <p>直接包含在註解中的任何使用者也會收到電子郵件通知。</p> <p>只有在專案狀態為[!UICONTROL目前]時，才會傳送通知。 </p> <p>即時通知電子郵件的主旨是： <em>[!UICONTROL對]的評論 &lt;request name=""&gt; on &lt;project name=""&gt; （參考編號） &lt;request reference="" number=""&gt;)</em></p> <p> 每日摘要通知的主旨是：<em> [!UICONTROL通信摘要] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td>文檔名稱<br>項目、任務或問題名稱<br>參考編號<br>回覆您請求的使用者名稱<br>評論的日期和時間<br>對該檔案的評論文本</td> 
   <td> <p><strong>立即</strong> </p> <p><strong>和每日</strong> </p> <p><strong></strong> </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>有人對我所在的執行緒發表了註解</strong> </p> <p>執行緒中的參與者和包含在直接訊息中的使用者，會在使用者在執行緒中留言時收到電子郵件通知。</p> <p>使用者必須擁有[!UICONTROL檢視]存取權才能接收通知。</p> <p>下列使用者不會收到通知：</p> 
    <ul> 
     <li>包含在直接訊息中的團隊</li> 
     <li>票據的所有者</li> 
     <li>主要聯繫人</li> 
    </ul> <p><strong>即時通知電子郵件的主旨是： <em>[!UICONTROL RE:評論] &lt;object name=""&gt;&lt;object type=""&gt; on &lt;project name=""&gt;（參考編號） &lt;object reference="" number=""&gt;</em>)</strong> </p> <p><strong> 每日摘要通知的主旨是：<em> [!UICONTROL通信摘要] &lt;date of="" daily="" digest=""&gt;</em></strong> </p> </td> 
   <td> 物件名稱<br>父對象名稱<br>評論線程的用戶名<br>線程上的注釋文本<br>評論的日期和時間<br>*收到的評論總數<br>*每個對象收到的注釋數<br>*專案名稱<br>*<strong>[!UICONTROL查看所有通知]</strong> 按鈕<br>*每日摘要日期 </td> 
   <td><strong>[!UICONTROL每日]</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>有人對我其中一個工作項目發表評論</strong> </p> <p>工作項目的受託人在用戶向工作項添加更新時收到電子郵件通知，除非添加更新的用戶也是受託人。 </p> <p>在請求上張貼意見時，請傳送電子郵件給問題主要聯絡人。</p> <p>問題的主要聯絡人在請求上張貼評論時會收到電子郵件通知，除非張貼評論的使用者也是問題的主要聯絡人。</p> <p>直接包含在註解中的任何使用者也會收到電子郵件通知。</p> <p>只有在專案狀態為[!UICONTROL目前]時，才會傳送通知。</p> <p>即時通知電子郵件的主旨是： <em>[!UICONTROL對]的評論 &lt;work item="" name=""&gt; on &lt;project name="" ref="" work="" item="" reference="" number=""&gt;)</em></p> <p> 每日摘要通知的主旨是：<em> [!UICONTROL通信摘要] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 工作項名稱<br>專案名稱<br>工作項參考編號<br>對工作項留言的用戶的名稱<br>對工作項作出評論的文本<br>評論的日期和時間<br>*收到的評論總數<br>*每個對象收到的注釋數<br>*專案名稱<br>*<strong>[!UICONTROL查看所有通知]</strong> 按鈕<br>*每日摘要日期 </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>有人將我的團隊加入定向更新</strong> </p> <p>定向更新是指當用戶在更新中特別包括另一個用戶時，如 <a href="../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">在更新時標籤其他人</a>.</p> <p>在此情況下，定向更新中包含的任何團隊成員都會收到有關更新的電子郵件通知。</p> <p>電子郵件通知只會傳送給具有物件存取權限的使用者。</p> <p>如果發送定向更新的用戶是所包括團隊的成員，則發送更新的用戶不會收到電子郵件通知。</p> <p>即時通知電子郵件的主旨是：[!UICONTROL對]的評論 &lt;object name=""&gt; on &lt;parent object="" name=""&gt; （參考編號） &lt;object reference="" number=""&gt;)</p> <p> 每日摘要通知的主旨是：<em> [!UICONTROL通信摘要] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>物件名稱<br>父對象名稱<br>對象引用編號<br>進行定向更新的用戶的名稱<br>定向更新中包含的所有團隊和用戶的名稱<br>進行定向更新的日期和時間<br>定向更新的文本<br><strong>[!UICONTROL注釋]</strong> 按鈕<br>*收到的評論總數<br>*每個對象收到的注釋數<br>*專案名稱<br>*<strong>[!UICONTROL查看所有通知]</strong> 按鈕<br>*每日摘要日期 </p> </td> 
   <td><strong>每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>為您的設定檔發佈一個更新</strong> </p> <p>您可以在使用者物件的[!UICONTROL更新]標籤中對使用者發表評論。 您也可以在編輯使用者的設定時，對使用者發表意見。 對其進行評論的使用者會收到電子郵件，通知他們此評論。 </p> <p>您必須具有至少對用戶[!UICONTROL View]的權限，才能在用戶的[!UICONTROL Updates]頁簽上輸入更新。 您必須對使用者擁有[!UICONTROL編輯]權限，才能編輯使用者的設定。 </p> <p>如需在「更新」標籤中對使用者留言的詳細資訊，請參閱 <a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">更新工作</a>.</p> <p>有關在編輯用戶設定時輸入用戶注釋的詳細資訊，請參閱 <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">配置我的設定</a>.</p> <p>即時通知電子郵件的主旨是： <em>&lt;user name=""&gt; [!UICONTROL希望您知道]</em></p> <p>每日摘要通知的主旨是：<em> [!UICONTROL通信摘要] &lt;date of="" daily="" digest=""&gt;</em></p> </td> 
   <td> 您的使用者名稱<br>添加評論的用戶的名稱<br>注釋文本<br>評論的日期和時間<br>*收到的評論總數<br>*每個對象收到的注釋數<br>*<strong>[!UICONTROL查看所有通知]</strong> 按鈕<br>*每日摘要日期 </td> 
   <td> <p><strong>立即</strong> </p> <p><strong>和每日</strong> </p> </td> 
  </tr> 
 </tbody> 
</table>
