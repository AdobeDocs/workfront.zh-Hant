---
content-type: reference
navigation-topic: notifications
title: 「通知：需要動作」
description: 下列通知可讓您知道您是否需要對工作專案採取行動。 如需有關設定您收到哪些通知的資訊，請參閱修改您自己的電子郵件通知。
author: Lisa
feature: Get Started with Workfront
exl-id: dd383bd4-da30-45ea-889e-e6b49416974b
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '2442'
ht-degree: 4%

---

# 通知： [!UICONTROL 需要動作]

下列通知可讓您知道您是否需要對工作專案採取行動。 如需有關設定您接收哪些通知的資訊，請參閱 [修改您自己的電子郵件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

另請參閱 [事件通知](../../workfront-basics/using-notifications/event-notifications.md).

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
   <td> <p><strong>我收到一個新的工作請求</strong> </p> <p>工作專案的受指派人會收到電子郵件通知，除非提出請求的使用者同時也是受指派人。 </p> <p>如果任務狀態為[！UICONTROL完成]或問題狀態為[！UICONTROL已關閉]，則不會傳送通知。</p> <p>擁有[！UICONTROL Review]或[！UICONTROL Requestor]授權的使用者不會收到通知。</p> <p>即時通知電子郵件的主旨為： <em>[！UICONTROL新工作請求]： &lt;request name=""&gt;</em></p> <p>每日摘要通知的主題為： <em>[！UICONTROL所需動作摘要] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>任務名稱</p> <p>[！UICONTROL計畫完成日期]</p> <p>父級</p> <p>指派自</p> <p>指派至</p> <p>[！UICONTROL狀態]</p> <p>[！UICONTROL說明]</p> <p>[！UICONTROL檢視]按鈕<br>要新增到每日摘要的選項</p> <br> </td> 
   <td><strong>即時和</strong> <strong>每日</strong></td> 
  </tr> 
  <tr> 
   <td> <p><strong>我需要核准文件</strong> </p> <p>檔案核准者會在被列為核准者時收到通知。</p> <p>即時通知電子郵件的主旨為： <em>&lt;name of="" the="" user="" who="" submitted="" the="" approval=""&gt; [！UICONTROL要求您核准檔案 [!DNL Adobe Workfront].]</em></p> <p>每日摘要通知的主題為：<em> [！UICONTROL所需動作摘要] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> 專案名稱<br>Portfolio名稱<br>提交核准的使用者名稱<br>檔名稱<br>檔案參考編號<br>要求的核准日期和時間<br>檔案詳細資訊（格式、大小、版本號碼）<br><strong>[！UICONTROL進行核准決定]</strong> 按鈕<br>*擱置檔案核准總數<br>*連結至 <strong>[！UICONTROL檔案核准</strong>*<strong>檢視所有核准]</strong> 按鈕<br>*每日摘要的日期<br></td> 
   <td><strong>即時與每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我需要核准專案</strong> </p> <p>若為工作角色核准，哪些使用者會收到此事件的電子郵件通知，取決於是否已啟用「[！UICONTROL核准者（針對包含角色的核准流程）]」設定（如所述），而此核准者不需要位於專案團隊中 <a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">設定全域核准設定</a>)。 </p> <p><strong>如果已啟用此選項</strong>，系統會傳送電子郵件通知給系統中所有使用者，該使用者具有與核准相關聯的工作角色。 </p> <p><strong>如果停用此選項</strong>，只有工作角色與核准流程關聯的專案團隊成員會收到電子郵件通知。</p> <p>如果核准與使用者相關聯，則該使用者會收到通知。</p> <p>即時通知電子郵件的主旨為： <em>[！UICONTROL專案待核准]： &lt;project name=""&gt;</em></p> <p> 每日摘要通知的主題為： <em> [！UICONTROL所需動作摘要] &lt;date of="" the="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>專案名稱<br>Portfolio名稱<br>專案參考號碼<br>提交核准的使用者名稱<br>未決核准狀態<br>要求的核准日期和時間<br>專案優先順序<br>核准步驟未決核准<br>等待核准的決策數<br>核准者名稱（僅限使用者）<br>[！UICONTROL專案計畫完成日期] <br><strong>[！UICONTROL進行核准決定]</strong> 按鈕<br>*擱置專案核准總數 <br>*連結至 <strong>[！UICONTROL專案核准]</strong><br>*<strong>[！UICONTROL檢視所有核准]</strong> 按鈕<br>*每日摘要的日期</p> </td> 
   <td><strong>即時與每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我需要核准任務</strong> </p> <p>若為工作角色核准，哪些使用者會收到此事件的電子郵件通知，取決於是否已啟用「[！UICONTROL核准者（針對包含角色的核准流程）]」設定（如所述），而此核准者不需要位於專案團隊中 <a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">設定全域核准設定</a>)。 </p> <p><strong>如果已啟用此選項</strong>，系統會傳送電子郵件通知給系統中所有使用者，該使用者具有與核准相關聯的工作角色。 </p> <p><strong>如果停用此選項</strong>，只有工作角色與核准流程關聯的專案團隊成員會收到電子郵件通知。</p> <p>如果核准與使用者相關聯，則該使用者會收到通知。 </p> <p>只有在專案狀態為[！UICONTROL目前]時，才會傳送通知。</p> <p>即時通知電子郵件的主旨為： <em>[！UICONTROL任務未決核准]： &lt;task name=""&gt;</em></p> <p> 每日摘要通知的主題為： <em> [！UICONTROL所需動作摘要] &lt;date of="" the="" daily="" digest=""&gt; </em></p> </td> 
   <td> <p>任務名稱<br>專案名稱<br>提交核准的使用者名稱<br>未決核准狀態<br>要求的核准日期和時間<br>任務優先順序<br>核准階段名稱<br>核准者名稱<br>[！UICONTROL任務計畫完成日期]<br><strong>[！UICONTROL進行核准決定]</strong> 按鈕<br>*擱置任務核准總數<br>*連結至<strong>[！UICONTROL任務核准*檢視所有核准]</strong> 按鈕<strong></strong>*每日摘要的日期<br></p> </td> 
   <td><strong>即時與每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我需要核准時程表</strong> </p> <p>時程表核准者會在提交需要核准的時程表時收到電子郵件通知，除非提交時程表的使用者也是時程表核准者。</p> <p>只有在時程表的狀態為[！UICONTROL已提交]時，才會傳送通知。</p> <p>即時通知電子郵件的主旨為： <em>[！UICONTROL時程表已提交]： &lt;timesheet owner=""&gt;， &lt;timesheet start="" date=""&gt; - &lt;timesheet end="" date=""&gt;</em></p> <p> 每日摘要通知的主題為： <em> [！UICONTROL所需動作摘要] &lt;date of="" the="" daily="" digest=""&gt; </em></p> </td> 
   <td> 提交時程表以供核准的使用者名稱<br>提交時程表的日期與時間<br>時程表的狀態<br>時程表的開始和結束日期<br>時程表上記錄的小時數<br>時程表上記錄的加班小時數<br><strong>[！UICONTROL評論]</strong> 和 <strong>[！UICONTROL核准]</strong> 按鈕<br>*擱置時程表核准總數<br>*連結至 <strong>[！UICONTROL時程表核准]</strong><br><strong>[！UICONTROL *檢視所有核准]</strong> 按鈕<br>*每日摘要的日期 </td> 
   <td><strong>即時和</strong> <strong>每日</strong></td> 
  </tr> 
  <tr> 
   <td> <p><strong>我需要核准問題</strong> </p> <p>若為工作角色核准，哪些使用者會收到此事件的電子郵件通知，取決於是否已啟用「[！UICONTROL核准者（針對包含角色的核准流程）]」設定（如所述），而此核准者不需要位於專案團隊中 <a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">[！UICONTROL設定全域核准]設定</a>)。 </p> <p><strong>如果已啟用此選項</strong>，系統會傳送電子郵件通知給系統中所有使用者，該使用者具有與核准相關聯的工作角色。 </p> <p><strong>如果停用此選項</strong>，只有工作角色與核准流程關聯的專案團隊成員會收到電子郵件通知。</p> <p>如果核准與使用者相關聯，則該使用者會收到通知。 </p> <p>只有在專案狀態為[！UICONTROL目前]時，才會傳送通知。</p> <p>即時通知電子郵件的主旨為： <em>[！UICONTROL問題未決核准]： &lt;issue name=""&gt;</em></p> <p> 每日摘要通知的主題為： <em> [！UICONTROL所需動作摘要] &lt;date of="" the="" daily="" digest=""&gt; </em></p> </td> 
   <td> 問題名稱<br>專案名稱<br>問題參考號碼<br>提交問題以供核准的使用者名稱<br>未決核准狀態<br>要求的核准日期和時間<br>問題優先順序<br>核准階段<br>核准者姓名<br>[！UICONTROL問題計畫完成日期]<br>[！UICONTROL主要連絡人]<br><strong>[！UICONTROL進行核准決定]</strong> 按鈕<br>*未決問題核准總數<br>*連結至 <strong>[！UICONTROL問題核准]</strong><br><strong>[！UICONTROL *檢視所有核准]</strong> 按鈕<br>*每日摘要的日期 </td> 
   <td><strong>即時和</strong> <strong>每日</strong></td> 
  </tr> 
  <tr> 
   <td> <p><strong>我需要檢閱委派給我核准的專案</strong> </p> <p>專案核准已委派給您，您需要進行稽核。</p> <p>即時通知電子郵件的主旨為： <em>[！UICONTROL受委派專案核准 — 請檢閱] &lt;project name=""&gt;</em></p> <p><em>每日摘要通知的主旨為：[！UICONTROL所需動作摘要] &lt;date of="" the="" daily="" digest=""&gt;</em> </p> </td> 
   <td> 專案名稱<br>Portfolio名稱<br>專案參考號碼<br>要求核准的使用者名稱<br>您要代表其核准專案的使用者名稱<br>未決核准狀態<br>要求的核准日期和時間<br>專案優先順序<br>核准步驟<br>核准者姓名<br>[！UICONTROL專案計畫完成日期]<br><strong>[！UICONTROL進行核准決定]</strong> 按鈕<br>*擱置專案核准總數<br>*連結至 <strong>[！UICONTROL專案核准*檢視所有核准]</strong> 按鈕 <br>*每日摘要的日期 </td> 
   <td><strong>即時與每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我需要檢閱委派給我的任務核准</strong> </p> <p>任務核准已委派給您，您需要檢視它。</p> <p>即時通知電子郵件的主旨為： <em>[！UICONTROL受委派任務核准 — 請檢閱]&lt;task name=""&gt;</em></p> <p>每日摘要通知的主題為：<em> [！UICONTROL所需動作摘要] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> 任務名稱<br>專案名稱<br>任務參考號碼<br>要求核准的使用者名稱<br>您要代表其核准任務的使用者名稱<br>未決核准狀態<br>要求的核准日期和時間<br>任務優先順序<br>核准階段<br>核准者姓名<br>[！UICONTROL任務計畫完成日期]<br><strong>[！UICONTROL進行核准決定]</strong> 按鈕 <br>*擱置任務核准總數<br>*連結至 <strong>[！UICONTROL任務核准*檢視所有核准]</strong> 按鈕<br>*每日摘要的日期 </td> 
   <td><strong>即時與每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我需要檢閱委派給我核准的問題</strong> </p> <p>問題核准已委派給您，您需要對其進行稽核。</p> <p>即時通知電子郵件的主旨為： <em>[！UICONTROL受委派問題核准 — 請檢閱] &lt;issue name=""&gt;</em></p> <p>每日摘要通知的主題為：<em> [！UICONTROL所需動作摘要] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> 問題名稱<br>專案名稱<br>問題參考號碼<br>要求核准的使用者名稱<br>您要代表其核准問題的使用者名稱<br>未決核准狀態<br>要求的核准日期和時間<br>問題優先順序<br>核准階段<br>核准者姓名<br>問題計畫完成日期<br>主要連絡人<br><strong>[！UICONTROL進行核准決定]</strong> 按鈕<br>*未決問題核准總數<br>*連結至 <strong>[！UICONTROL問題核准]</strong><br><strong>[！UICONTROL *檢視所有核准]</strong> 按鈕<br>*每日摘要的日期<br></td> 
   <td><strong>即時與每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>有問題指派給我</strong> </p> <p>問題受指派人會收到電子郵件通知。 如果問題的狀態為或等同於[！UICONTROL已關閉]，則問題受指派人不會收到電子郵件。</p> <p>擁有[！UICONTROL Review]或[！UICONTROL Requestor]授權的使用者不會收到通知。</p> <p>只有在專案狀態為[！UICONTROL目前]時，才會傳送通知。</p> <p>即時通知電子郵件的主旨為： <em>[！UICONTROL新工作請求]： &lt;issue name=""&gt;</em></p> <p>每日摘要通知的主題為：<em> [！UICONTROL所需動作摘要] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>問題名稱<br>專案名稱<br>[！UICONTROL問題參考編號]<br>您的姓名<br>問題到期日期（[！UICONTROL規劃完成日期]）<br>指派問題給您的使用者名稱<br><strong>[！UICONTROL處理它]</strong> 按鈕<br>*指派總數<br>*指派給您的任務和問題總數<br>*連結至 <strong>[！UICONTROL工作請求]</strong><br>*每日摘要的日期<br></p> </td> 
   <td><strong>即時與每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我被設為一項任務的主要受指派者</strong> </p> <p>如果工作受指派人是工作的主要受指派人，則工作受指派人會收到電子郵件通知，除非受指派人是進行指派的使用者。</p> <p>如果專案狀態為[！UICONTROL目前]且任務未標籤為[！UICONTROL完成]，則會傳送通知。</p> <p>擁有[！UICONTROL Review]或[！UICONTROL Requestor]授權的使用者不會收到通知。</p> <p>即時通知電子郵件的主旨為： <em>[！UICONTROL新工作請求]： &lt;task name=""&gt;</em></p> <p>每日摘要通知的主題為：<em> [！UICONTROL所需動作摘要] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> 任務名稱<br>專案名稱<br>任務參考號碼<br>您的姓名<br>任務到期日（[！UICONTROL計畫完成日期]）<br>指派任務給您的使用者名稱<br><strong>[！UICONTROL處理它]</strong> 按鈕<br>*指派給您的任務和問題總數<br>*連結至 <strong>[！UICONTROL工作請求]</strong>*每日摘要的日期 </td> 
   <td><strong>即時與每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我的團隊收到一個新的工作請求</strong> </p> <p>當團隊收到新的工作請求時，團隊成員會收到電子郵件通知。 （提交請求的使用者若是團隊成員，則不會收到通知。）</p> <p>僅當專案狀態為[！UICONTROL目前]且工作請求狀態為[！UICONTROL新]時，才會傳送通知。</p> <p>擁有[！UICONTROL Review]授權的使用者不會收到通知。</p> <p>即時通知電子郵件的主旨為： <em>[！UICONTROL新工作請求]： &lt;request name=""&gt;</em></p> <p>每日摘要通知的主題為： <em>[！UICONTROL所需動作摘要] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p> 問題名稱<br>專案名稱（請求佇列名稱）<br>問題參考號碼<br>團隊名稱<br>問題到期日（計畫完成日期）<br>提交請求的使用者名稱<br><strong>[！UICONTROL處理它]</strong> 按鈕<br>*指派給團隊的要求總數</p> <p>*工作請求名稱</p> <p>[！UICONTROL *規劃完成日期]</p> <p>*提交請求的使用者名稱<br>*連結至 <strong>[！UICONTROL團隊請求]</strong><br>*每日摘要的日期 </p> <p><span class="preview">*團隊指派</span> </p> </td> 
   <td><strong>即時與每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我的時程表已重新開啟</strong> </p> <p>時程表所有者會在時程表重新開啟時收到電子郵件通知，除非重新開啟時程表的使用者同時也是時程表的所有者。</p> <p>只有在時程表狀態為[！UICONTROL未完成]時，才會傳送電子郵件通知。</p> <p>即時通知電子郵件的主旨為： <em>[！UICONTROL時程表重新開啟]： &lt;timesheet start="" date=""&gt; - &lt;timesheet end="" date=""&gt;</em></p> <p>注意：您無法設定每日摘要電子郵件的此通知。</p> </td> 
   <td> 重新開啟時程表的使用者名稱<br>重新開啟時程表的日期與時間<br>時程表的狀態（[！UICONTROL重新開啟]）<br>時程表上記錄的總時數<br>時程表上記錄的加班小時數<br><strong>[！UICONTROL評論]</strong> 按鈕 </td> 
   <td><strong>立即</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>我的時程表已被拒絕</strong> </p> <p>時程表所有者會在時程表被拒絕時收到電子郵件通知，除非拒絕時程表的使用者也是所有者。</p> <p>只有在時程表狀態為[！UICONTROL已拒絕]時，才會傳送電子郵件通知。</p> <p>即時通知電子郵件的主旨為： <em>[！UICONTROL時程表已拒絕]：&lt;start date="" of="" the="" timesheet=""&gt; - &lt;end date="" of="" the="" timesheet=""&gt;</em></p> <p>注意：您無法設定每日摘要電子郵件的此通知。</p> </td> 
   <td> 拒絕時程表的使用者名稱<br>時程表的狀態（[！UICONTROL已拒絕]）<br>時程表遭拒絕的日期與時間<br><strong>[！UICONTROL評論]</strong> 按鈕 </td> 
   <td><strong>立即</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>有人向我申請存取權</strong> </p> <p>要求我做點什麼，所以請開啟。</p> <p>建立專案的人可存取該專案。</p> <p>這就是當有人請求存取權時，使用者收到通知的原因。</p> <p>即時通知電子郵件的主旨為： <em>&lt;name of="" user="" who="" requested="" the="" access=""&gt; [！UICONTROL需要存取] &lt;object name=""&gt;</em></p> <p>每日摘要通知的主題為：<em> [！UICONTROL所需動作摘要] &lt;date of="" the="" daily="" digest=""&gt;</em></p> </td> 
   <td> <p>物件名稱<br>父系物件名稱<br>物件參考編號<br>要求存取許可權的使用者名稱<br>使用者要求的存取型別<br><strong>[！UICONTROL授予] &lt;name of="" the="" access="" requested=""&gt; 存取</strong> 和 <strong>[！UICONTROL授予不同存取權]</strong> 按鈕<br>*擱置中的存取要求核准總數<br>*連結至 <strong>[！UICONTROL存取要求]</strong> 核准<br>*每日摘要日期</p> </td> 
   <td><strong>即時與每日</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>有人請求我上傳文件</strong> </p> <p>當使用者收到上傳檔案的請求時，檔案請求者會收到電子郵件通知。</p> <p>即時通知電子郵件的主旨為： <em>&lt;name of="" the="" user="" requesting="" the="" document=""&gt; [！UICONTROL需要您提供的檔案，位於 [!DNL Workfront].]</em></p> <p> <p>注意：您無法設定每日摘要電子郵件的此通知。</p> </p> </td> 
   <td> 請求檔案的使用者的名稱<br>應上傳檔案的物件名稱<br><strong>[！UICONTROL附加至此處]</strong> 連結 </td> 
   <td><strong>立即</strong> </td> 
  </tr> 
 </tbody> 
</table>
