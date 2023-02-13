---
content-type: reference
navigation-topic: notifications
title: '通知：需要的操作'
description: 如果您需要對工作項目採取操作，以下通知會通知您。 如需設定您收到哪些通知的相關資訊，請參閱啟用或停用您自己的事件通知。
author: Lisa
feature: Get Started with Workfront
exl-id: dd383bd4-da30-45ea-889e-e6b49416974b
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '2446'
ht-degree: 4%

---

# 通知： [!UICONTROL 需要的行動]

如果您需要對工作項目採取操作，以下通知會通知您。 如需設定您收到哪些通知的詳細資訊，請參閱 [啟用或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

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
   <td> <p><strong>我得到一個新工作要求</strong> </p> <p>工作項目的受託人會收到電子郵件通知，除非提出請求的使用者也是受託人。 </p> <p>如果任務狀態為[!UICONTROL Complete]或問題狀態為[!UICONTROL Closed]，則不會發送通知。</p> <p>擁有[!UICONTROL Review]或[!UICONTROL Requestor]許可的用戶不會收到通知。</p> <p>即時通知電子郵件的主旨是： <em>[!UICONTROL新工作請求]: &lt;request name=""&gt;</em></p> <p>每日摘要通知的主旨是： <em>[!UICONTROL需要的操作摘要] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>任務名稱</p> <p>[!UICONTROL計畫完成日期]</p> <p>父級</p> <p>指派自</p> <p>指派至</p> <p>[!UICONTROL狀態]</p> <p>[!UICONTROL描述]</p> <p>[!UICONTROL視圖]按鈕<br>要新增至每日摘要的選項</p> <br> </td> 
   <td><strong>即時和</strong> <strong>每日</strong></td> 
  </tr> 
  <tr> 
   <td> <p><strong>我需要核准文件</strong> </p> <p>文檔的批准者在被列為批准者時會收到通知。</p> <p>即時通知電子郵件的主旨是： <em>&lt;name of="" the="" user="" who="" submitted="" the="" approval=""&gt; [!UICONTROL要求您核准 [!DNL Adobe Workfront].]</em></p> <p>每日摘要通知的主旨是：<em> [!UICONTROL需要的操作摘要] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> 專案名稱<br>Portfolio名稱<br>提交批准的用戶的名稱<br>文檔名稱<br>文檔參考編號<br>請求批准的日期和時間<br>文檔詳細資訊（格式、大小、版本號）<br><strong>[!UICONTROL作出批准決定]</strong> 按鈕<br>*待審文檔的總數<br>*連結至 <strong>[!UICONTROL文檔批准</strong>*<strong>請參閱所有核准]</strong> 按鈕<br>*每日摘要日期<br></td> 
   <td><strong>即時和每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我需要核准專案</strong> </p> <p>若是作業角色核准，使用者會收到此事件的電子郵件通知，端視「[!UICONTROL核准者不需要加入專案團隊（針對包含角色的核准程式）」設定是否已啟用(如 <a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">配置全局批准設定</a>)。 </p> <p><strong>如果已啟用此選項</strong>，則會傳送電子郵件通知給系統中具有與核准相關聯之工作角色的所有使用者。 </p> <p><strong>如果禁用此選項</strong>，只有具有與核准程式相關聯的工作角色的專案團隊成員會收到電子郵件通知。</p> <p>如果核准與使用者相關聯，該使用者會收到通知。</p> <p>即時通知電子郵件的主旨是： <em>[!UICONTROL項目待批准]: &lt;project name=""&gt;</em></p> <p> 每日摘要通知的主旨是： <em> [!UICONTROL需要的操作摘要] &lt;date of="" the="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>專案名稱<br>Portfolio名稱<br>項目參考編號<br>提交批准的用戶名<br>待批准狀態<br>請求批准的日期和時間<br>專案優先順序<br>待批准的批准步驟<br>等待批准的決定數<br>批准者名稱（僅限用戶）<br>[!UICONTROL項目計畫完成日期] <br><strong>[!UICONTROL作出批准決定]</strong> 按鈕<br>*待審項目批准總數 <br>*連結至 <strong>[!UICONTROL項目批准]</strong><br>*<strong>[!UICONTROL查看所有批准]</strong> 按鈕<br>*每日摘要日期</p> </td> 
   <td><strong>即時和每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我需要核准任務</strong> </p> <p>若是作業角色核准，使用者會收到此事件的電子郵件通知，端視「[!UICONTROL核准者不需要加入專案團隊（針對包含角色的核准程式）」設定是否已啟用(如 <a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">配置全局批准設定</a>)。 </p> <p><strong>如果已啟用此選項</strong>，則會傳送電子郵件通知給系統中具有與核准相關聯之工作角色的所有使用者。 </p> <p><strong>如果禁用此選項</strong>，只有具有與核准程式相關聯的工作角色的專案團隊成員會收到電子郵件通知。</p> <p>如果核准與使用者相關聯，該使用者會收到通知。 </p> <p>只有在專案狀態為[!UICONTROL目前]時，才會傳送通知。</p> <p>即時通知電子郵件的主旨是： <em>[!UICONTROL任務待批准]: &lt;task name=""&gt;</em></p> <p> 每日摘要通知的主旨是： <em> [!UICONTROL需要的操作摘要] &lt;date of="" the="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>任務名稱<br>專案名稱<br>提交批准的用戶的名稱<br>待批准狀態<br>請求批准的日期和時間<br>任務優先順序<br>批准階段名稱<br>批准者名稱<br>[!UICONTROL任務計畫完成日期]<br><strong>[!UICONTROL作出批准決定]</strong> 按鈕<br>*待審任務批准總數<br>*連結至<strong>[!UICONTROL任務批准*請參閱所有批准]</strong> 按鈕<strong></strong>*每日摘要日期<br></p> </td> 
   <td><strong>即時和每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我需要提交時程表</strong> </p> <p>提交需要批准的時間表時，時間表批准者會收到電子郵件通知，除非提交時間表的用戶也是時間表批准者。</p> <p>僅當時間表的狀態為[!UICONTROL已提交]時，才會發送通知。</p> <p>即時通知電子郵件的主旨是： <em>[!UICONTROL時間表已提交]: &lt;timesheet owner=""&gt;, &lt;timesheet start="" date=""&gt; - &lt;timesheet end="" date=""&gt;</em></p> <p> 每日摘要通知的主旨是： <em> [!UICONTROL需要的操作摘要] &lt;date of="" the="" daily="" digest=""&gt; </em></p> </td> 
   <td> 提交工時單以進行審批的用戶的名稱<br>提交時間表的日期和時間<br>時間表的狀態<br>時間表的開始和結束日期<br>工時單上記錄的小時數<br>工時單上記錄的加班小時數<br><strong>[!UICONTROL Review]</strong> 和 <strong>[!UICONTROL批准]</strong> 按鈕<br>*待審時間表批准的總數<br>*連結至 <strong>[!UICONTROL時間表批准]</strong><br><strong>[!UICONTROL *請參閱所有批准]</strong> 按鈕<br>*每日摘要日期 </td> 
   <td><strong>即時和</strong> <strong>每日</strong></td> 
  </tr> 
  <tr> 
   <td> <p><strong>我需要核准問題</strong> </p> <p>若是作業角色核准，使用者會收到此事件的電子郵件通知，端視「[!UICONTROL核准者不需要加入專案團隊（針對包含角色的核准程式）」設定是否已啟用(如 <a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">[!UICONTROL配置全局批准]設定</a>)。 </p> <p><strong>如果已啟用此選項</strong>，則會傳送電子郵件通知給系統中具有與核准相關聯之工作角色的所有使用者。 </p> <p><strong>如果禁用此選項</strong>，只有具有與核准程式相關聯的工作角色的專案團隊成員會收到電子郵件通知。</p> <p>如果核准與使用者相關聯，該使用者會收到通知。 </p> <p>只有在專案狀態為[!UICONTROL目前]時，才會傳送通知。</p> <p>即時通知電子郵件的主旨是： <em>[!UICONTROL待批准問題]: &lt;issue name=""&gt;</em></p> <p> 每日摘要通知的主旨是： <em> [!UICONTROL需要的操作摘要] &lt;date of="" the="" daily="" digest=""&gt; </em></p> </td> 
   <td> 問題名稱<br>專案名稱<br>問題參考編號<br>提交問題以供批准的用戶的名稱<br>待批准狀態<br>請求批准的日期和時間<br>問題優先順序<br>核准階段<br>批准者的名稱<br>[!UICONTROL發行計畫完成日期]<br>[!UICONTROL主要聯繫人]<br><strong>[!UICONTROL作出批准決定]</strong> 按鈕<br>*待審問題批准的總數<br>*連結至 <strong>[!UICONTROL問題批准]</strong><br><strong>[!UICONTROL *請參閱所有批准]</strong> 按鈕<br>*每日摘要日期 </td> 
   <td><strong>即時和</strong> <strong>每日</strong></td> 
  </tr> 
  <tr> 
   <td> <p><strong>我需要審核我所受委派的專案核准</strong> </p> <p>已將項目批准委託給您，您需要對其進行審核。</p> <p>即時通知電子郵件的主旨是： <em>[!UICONTROL委派的項目批准 — 請查看] &lt;project name=""&gt;</em></p> <p><em>每日摘要通知的主旨是：[!UICONTROL需要的操作摘要] &lt;date of="" the="" daily="" digest=""&gt;</em> </p> </td> 
   <td> 專案名稱<br>Portfolio名稱<br>項目參考編號<br>請求批准的用戶的名稱<br>您代表其批准項目的用戶名<br>待批准狀態<br>請求批准的日期和時間<br>專案優先順序<br>核准步驟<br>批准者的名稱<br>[!UICONTROL項目計畫完成日期]<br><strong>[!UICONTROL作出批准決定]</strong> 按鈕<br>*待審項目批准總數<br>*連結至 <strong>[!UICONTROL項目批准*請參閱所有批准]</strong> 按鈕 <br>*每日摘要日期 </td> 
   <td><strong>即時和每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我需要審核我所受委派的任務核准</strong> </p> <p>已將任務批准委託給您，您需要對其進行審核。</p> <p>即時通知電子郵件的主旨是： <em>[!UICONTROL委派任務批准 — 請查看]&lt;task name=""&gt;</em></p> <p>每日摘要通知的主旨是：<em> [!UICONTROL需要的操作摘要] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> 任務名稱<br>專案名稱<br>任務參考編號<br>請求批准的用戶的名稱<br>您代表其批准任務的用戶的名稱<br>待批准狀態<br>請求批准的日期和時間<br>任務優先順序<br>核准階段<br>批准者的名稱<br>[!UICONTROL任務計畫完成日期]<br><strong>[!UICONTROL作出批准決定]</strong> 按鈕 <br>*待審任務批准總數<br>*連結至 <strong>[!UICONTROL任務批准*請參閱所有批准]</strong> 按鈕<br>*每日摘要日期 </td> 
   <td><strong>即時和每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我需要審核我所受委派的問題核准</strong> </p> <p>已委派核發給您，您需要加以檢閱。</p> <p>即時通知電子郵件的主旨是： <em>[!UICONTROL委派的發行批准 — 請查看] &lt;issue name=""&gt;</em></p> <p>每日摘要通知的主旨是：<em> [!UICONTROL需要的操作摘要] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> 問題名稱<br>專案名稱<br>問題參考編號<br>請求批准的用戶的名稱<br>您要代表其核准問題的用戶的名稱<br>待批准狀態<br>請求批准的日期和時間<br>問題優先順序<br>核准階段<br>批准者的名稱<br>發放計畫完成日期<br>主要連絡人<br><strong>[!UICONTROL作出批准決定]</strong> 按鈕<br>*待審問題批准的總數<br>*連結至 <strong>[!UICONTROL問題批准]</strong><br><strong>[!UICONTROL *請參閱所有批准]</strong> 按鈕<br>*每日摘要日期<br></td> 
   <td><strong>即時和每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我被指派到問題</strong> </p> <p>問題受託人會收到電子郵件通知。 如果問題狀態為或等於[!UICONTROL已關閉]，則問題受託人不會收到電子郵件。</p> <p>擁有[!UICONTROL Review]或[!UICONTROL Requestor]許可的用戶不會收到通知。</p> <p>只有在專案狀態為[!UICONTROL目前]時，才會傳送通知。</p> <p>即時通知電子郵件的主旨是： <em>[!UICONTROL新工作請求]: &lt;issue name=""&gt;</em></p> <p>每日摘要通知的主旨是：<em> [!UICONTROL需要的操作摘要] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>問題名稱<br>專案名稱<br>[!UICONTROL問題參考編號]<br>您的名稱<br>發出到期日（[!UICONTROL計畫完成日期]）<br>將問題指派給您的使用者名稱<br><strong>[!UICONTROL Work It]</strong> 按鈕<br>*分配總數<br>*分配給您的任務和問題總數<br>*連結至 <strong>[!UICONTROL工作請求]</strong><br>*每日摘要日期<br></p> </td> 
   <td><strong>即時和每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我被設為一項任務的主要受指派者</strong> </p> <p>如果任務受託人被確定為任務的主要受託人，則任務受託人會收到電子郵件通知，除非受託人是進行分配的用戶。</p> <p>如果項目狀態為[!UICONTROL Current]且任務未標籤為[!UICONTROL Complete]，則會發送通知。</p> <p>擁有[!UICONTROL Review]或[!UICONTROL Requestor]許可的用戶不會收到通知。</p> <p>即時通知電子郵件的主旨是： <em>[!UICONTROL新工作請求]: &lt;task name=""&gt;</em></p> <p>每日摘要通知的主旨是：<em> [!UICONTROL需要的操作摘要] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> 任務名稱<br>專案名稱<br>任務參考編號<br>您的名稱<br>任務到期日（[!UICONTROL計畫完成日期]）<br>將任務分配給您的用戶的名稱<br><strong>[!UICONTROL Work It]</strong> 按鈕<br>*分配給您的任務和問題總數<br>*連結至 <strong>[!UICONTROL工作請求]</strong>*每日摘要日期 </td> 
   <td><strong>即時和每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我的團隊得到新的工作請求</strong> </p> <p>團隊成員在收到新工作請求時會收到電子郵件通知。 （提交請求的使用者若是團隊成員，不會收到通知。）</p> <p>僅當項目狀態為[!UICONTROL Current]且工作請求狀態為[!UICONTROL New]時，才會發送通知。</p> <p>擁有[!UICONTROL Review]授權的使用者不會收到通知。</p> <p>即時通知電子郵件的主旨是： <em>[!UICONTROL新工作請求]: &lt;request name=""&gt;</em></p> <p>每日摘要通知的主旨是： <em>[!UICONTROL需要的操作摘要] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p> 問題名稱<br>專案名稱（請求佇列名稱）<br>問題參考編號<br>團隊名稱<br>發行到期日（計畫完成日期）<br>提交請求的用戶名<br><strong>[!UICONTROL Work It]</strong> 按鈕<br>*指派給您團隊的請求總數</p> <p>*工作請求名稱</p> <p>[!UICONTROL *計畫完成日期]</p> <p>*提交請求的用戶名<br>*連結至 <strong>[!UICONTROL團隊請求]</strong><br>*每日摘要日期 </p> <p><span class="preview">*團隊分配</span> </p> </td> 
   <td><strong>即時和每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我的時程表已重新開啟</strong> </p> <p>重新開啟工時單時，工時單所有者將收到電子郵件通知，除非重新開啟工時單的用戶也是工時單的所有者。</p> <p>僅當時間表狀態為[!UICONTROL Open]時，才會發送電子郵件通知。</p> <p>即時通知電子郵件的主旨是： <em>[!UICONTROL時間表重新開啟]: &lt;timesheet start="" date=""&gt; - &lt;timesheet end="" date=""&gt;</em></p> <p>注意：您無法為每日摘要電子郵件設定此通知。</p> </td> 
   <td> 重新開啟工時單的用戶的名稱<br>重新開啟時間表的日期和時間<br>時間表的狀態（[!UICONTROL重新開啟]）<br>工時單上記錄的總小時數<br>工時單上記錄的加班小時數<br><strong>[!UICONTROL Review]</strong> 按鈕 </td> 
   <td><strong>立即</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我的時程表已拒絕</strong> </p> <p>拒絕工時單的用戶也是所有者，否則工時單所有者在工時單被拒絕時收到電子郵件通知。</p> <p>僅當時間表狀態為[!UICONTROL已拒絕]時，才會發送電子郵件通知。</p> <p>即時通知電子郵件的主旨是： <em>[!UICONTROL已拒絕時間表]:&lt;start date="" of="" the="" timesheet=""&gt; - &lt;end date="" of="" the="" timesheet=""&gt;</em></p> <p>注意：您無法為每日摘要電子郵件設定此通知。</p> </td> 
   <td> 拒絕工時單的用戶名<br>時間表的狀態（[!UICONTROL已拒絕]）<br>時間表被拒絕的日期和時間<br><strong>[!UICONTROL Review]</strong> 按鈕 </td> 
   <td><strong>立即</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>某人向我要求存取權</strong> </p> <p>讓我做點什麼，開啟它。</p> <p>建立專案的人員可存取專案。</p> <p>這是當有人要求存取時，讓使用者收到通知的原因。</p> <p>即時通知電子郵件的主旨是： <em>&lt;name of="" user="" who="" requested="" the="" access=""&gt; [!UICONTROL需要訪問] &lt;object name=""&gt;</em></p> <p>每日摘要通知的主旨是：<em> [!UICONTROL需要的操作摘要] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>物件名稱<br>父對象名稱<br>對象引用編號<br>請求訪問權限的用戶的名稱<br>用戶請求的訪問類型<br><strong>[!UICONTROL授予] &lt;name of="" the="" access="" requested=""&gt; 存取</strong> 和 <strong>[!UICONTROL授予不同的訪問權]</strong> 按鈕<br>*待審訪問請求批准的總數<br>*連結至 <strong>[!UICONTROL訪問請求]</strong> 核准<br>*每日摘要日期</p> </td> 
   <td><strong>即時和每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>有人要求我上傳文件</strong> </p> <p>當使用者收到上傳檔案的請求時，檔案請求會收到電子郵件通知。</p> <p>即時通知電子郵件的主旨是： <em>&lt;name of="" the="" user="" requesting="" the="" document=""&gt; 在 [!DNL Workfront].]</em></p> <p> <p>注意：您無法為每日摘要電子郵件設定此通知。</p> </p> </td> 
   <td> 請求文檔的用戶的名稱<br>應上載文檔的對象的名稱<br><strong>[!UICONTROL將其附加在此處]</strong> 連結 </td> 
   <td><strong>立即</strong> </td> 
  </tr> 
 </tbody> 
</table>
