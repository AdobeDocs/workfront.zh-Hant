---
product-area: reporting;setup
navigation-topic: create-and-manage-reports
title: 報表傳送概觀
description: 報表傳送概觀
author: Nolan
feature: Reports and Dashboards
exl-id: 1637df59-ca1d-4cf6-b83d-2b27936cdb96
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1528'
ht-degree: 0%

---

# 報表傳送概觀

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This is linked to the UI in the Send Report box inside the Preview sandbox. If you change title, log bug for Dev to fix the link) </p>
-->

您可以排程報表以依定義的排程自動傳送給使用者，或手動傳送報表一次。 從Adobe Workfront傳送報表時，使用者會收到另一個附件中含有Workfront報表的電子郵件。

如需設定要傳送之報表的相關資訊，請參閱文章 [排程自動報表傳送](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).

您無法排程報表的傳送，也無法在「預覽沙箱」環境中手動傳送。 如需預覽沙箱的詳細資訊，請參閱文章 [Adobe Workfront預覽沙箱環境](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).\
如需在「預覽沙箱」環境中傳送報表的詳細資訊，請參閱文章 [在預覽沙箱環境中傳送報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/send-report-preview-sandbox-environment.md).

## 報表傳送限制

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This information is shared between "Exporting Data" and "Setting Up Report Deliveries."])</p>
-->

排程傳送報表時，請考量下列事項：

* 您最多可以為任何指定報表排程10個重複報表傳送。
* 只有在您是報表的建立者時，才可排程要傳送的報表。 如果您需要傳送您未建立的報表，可以手動傳送。

## 匯出限制

有數個大小限制會影響報表在Workfront中的顯示方式，以及這些報表透過手動匯出、傳送的報表或API匯出的方式：

* **5MB檔案大小：** 已排程傳送之任何匯出報表的檔案大小限制。 如果附加至電子郵件的匯出檔案大於5MB，則會以電子郵件傳送可下載檔案的連結，而非附加的匯出報表。 

   >[!NOTE]
   >
   >大於5MB的Excel .xlsx檔案不會產生電子郵件。 您可以手動將報表匯出為此格式。 如需匯出報表的相關資訊，請參閱 [匯出資料](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

* **50,000列：** 匯出.pdf和Tab分隔檔案的報表中允許的資料列數。

   對於Excel .xls檔案，此限制為 **65,000列**.

   若為Excel .xlsx檔案，此限制為 **100,000列**.

   這些限制會排除欄標題，以及報表中分組的列。 例如，若報表中有6個群組，以及50,000列或資料，則匯出的檔案將會有50,000列。

   如果您的報表項目超過這些限制，您會收到報表匯出和傳送不成功的錯誤。 將您在畫面上看到的項目數減少為小於或等於這些限制，以便能夠傳送結果。 如果要匯出所有資料，建議您使用篩選器來取得較少的資料載入，然後執行多個匯出。 如需詳細資訊，請參閱 [Adobe Workfront中的篩選器概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

   這些限制適用於：

   * 手動匯出報表。
   * 排程報表。
   * 透過API整合匯出。 
   * 透過啟動匯出的資料。

      如需透過啟動匯出資料的詳細資訊，請參閱文章 [透過Kick-Starts從Adobe Workfront匯出資料](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

      >[!NOTE]
      您可以將啟動檔案中的50,000列匯出，但只能匯出為Excel格式檔案。 

   * 導出項目的利用率資訊。

      有關導出項目的利用率資訊的詳細資訊，請參見 [資源利用率報告概覽](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

* **65,530個超連結：** 這是Excel對包含65,530個以上超連結的檔案所施加的限制。 手動匯出或在傳送的報表中傳送這些檔案時，無法開啟這些檔案。 請注意， Excel文檔可能只有200行資料，但如果文檔內有65,530個以上的連結，則該文檔不會開啟。 此限制僅存在於Excel檔案中，不存在於其他支援的格式中。 
* **256欄**：這是Excel對包含256欄以上的檔案所施加的限制。 無法手動匯出這些檔案，或在傳送的報表中傳送。 此限制僅存在於Excel檔案中，不存在於其他支援的格式中。 

如果您嘗試匯出超過限制的資料，可能不會在匯出中收到所有預期的資料。 而是在限制內產生修改的報表。 

此外，執行超過60分鐘的報表將會暫停。

若您對限制有疑慮或有問題，請聯絡Workfront技術支援。

## 了解已傳送報表上的時間戳記

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Note about if this is delivered at a time based on the user's time zone settings?)</p>
-->

在電子郵件中收到報表時，如果您要在Workfront中同時檢視報表，則報表的時間戳記和時間格式可能不符合Workfront中的格式。 

請考量下列事項： 

* 在瀏覽器中檢視報表時，報表上的時間戳記和格式會符合瀏覽器的地區設定和時區，如瀏覽器設定所定義。
* 以電子郵件傳送報表時，報表的傳送時間戳記和格式會與Workfront設定檔中指定的「使用者地區」和「時區」相符。\
   如需Workfront中「使用者地區設定」和「時區」的詳細資訊，請參閱文章 [編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## 具有特殊檢視的報表 {#reports-with-a-special-view}

將特殊檢視套用至報表時，特殊檢視會顯示在Workfront中報表的「詳細資料」標籤中。

當您排程傳送具有特殊檢視的報表時，預設的「詳細資料」索引標籤會傳送在已傳送電子郵件的附件中，而非特殊檢視中。

以下為特殊檢視：

* 專案報表上的里程碑檢視
* 項目或任務報告上的甘特視圖
* 以圖表為預設索引標籤的報表

>[!NOTE]
如果除了具有特殊檢視的預設標籤外，報表上還有「矩陣」標籤，則報表的傳送方式會如「矩陣」標籤上所顯示。

如需如何將特殊檢視套用至報表的詳細資訊，請參閱文章 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## 使用傳遞的檔案

 當您從Workfront傳送報表時，使用者會收到一封電子郵件，內含報表（附件）。 

* [主旨行、附件名稱和報表標題](#subject-line-attachment-name-and-report-title)
* [時間戳記](#timestamps)
* [品牌化](#branding)
* [格式](#formatting)
* [連結](#links)

### 主旨行、附件名稱和報表標題 {#subject-line-attachment-name-and-report-title}

如需已傳送報表電子郵件主旨行的詳細資訊，請參閱 [排程自動報表傳送](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).

附加報表的名稱為： *The_Name_Of_The_Report*&#x200B;後跟匯出的檔案格式。 

如果您將傳送的報表排程為PDF或HTML檔案格式，報表標題將會是：

*報表名稱。*

排程以Excel、Excel(.xlsx)或TSV格式傳送的報表沒有標題。

>[!NOTE]
如果報表有說明，則如果檔案的格式為PDF或HTML檔案，則該說明將包含在導出的檔案中。

### 時間戳記 {#timestamps}

只有在檔案格式為.pdf時，附加檔案上才會顯示時間戳記。 時間戳記位於附加檔案的頁尾中。

時間戳記包括：

* 日期
* 時間
* 報表傳送時區

### 品牌化 {#branding}

如果您的Workfront管理員已將自訂品牌新增至您的Workfront執行個體，則以.pdf格式傳送的報表也會包含您的個人化標誌。

以所有其他格式傳送的報表無法以您的標誌個人化。

如需將Workfront例項品牌化的詳細資訊，請參閱文章 [品牌化您的Adobe Workfront執行個體](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).

### 格式 {#formatting}

在傳送或排程傳送報表時，除非報表有特殊檢視，否則一律會收到報表的預設索引標籤。

如果您的報表在Web應用程式中有特殊格式，當「詳細資訊」和「矩陣」索引標籤僅針對.pdf和Excel檔案傳送時，應以特殊格式傳送報表。

傳送的檔案中不包含報表的篩選、檢視或分組。 只有在以PDF檔案傳送報表時，才會包含報表的說明。

如需接收具有特殊檢視之報表的詳細資訊，請參閱文章 [具有特殊檢視的報表](#reports-with-a-special-view).\
如需選取報表預設標籤以及特殊格式的相關資訊，請參閱 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

### 連結 {#links}

將報表從Workfront傳送至PDF或Excel格式時，原始檔案中存在的任何工作連結在已傳送的檔案中仍為現時狀態。 連結可以指向Workfront中支援連結的任何物件。

電子郵件訊息中的報表名稱也是連結。

## 排程報表的報表

您可以建立下列項目，查看報表是否已設定為傳送：

* **檢視** 對於清單中的報表對象或報表的報表：建立報表清單或報表報表的檢視，並新增下列欄至檢視：\
   *排程報表名稱。\
   *為該報告排程的所有傳送名稱會列在項目符號清單的欄中。\
   ![scheduled_reports_info_in_view.png](assets/scheduled-reports-info-in-view-350x294.png)

* **篩選** 報表物件：使用下列陳述式，在報表清單或報表上建立篩選器： *排程報表ID不得空白*.\
   這只會顯示已排程在清單或報表中的報表。\
   ![](assets/qs-scheduled-report-filter-350x101.png)\
   如需建立報表的詳細資訊，請參閱 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md). 如需建立報表報表的相關資訊，請參閱 [建立報告活動的報告](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md).

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Scheduling a Repeating&nbsp;Report Delivery</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can schedule up to 10 repeating report deliveries for any given report.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can schedule a report to be delivered only if you are the creator of the report. If you need to send a report that you did not create, you can send it on a manual basis.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To schedule&nbsp;a report for automatic delivery or to edit an existing report delivery:&nbsp;​</p>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">Navigate to and click the name of the report for which you want to schedule delivery.&nbsp;</li>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Report Actions</strong>, then&nbsp;<strong>Send Report</strong>.<br> The <strong>Send Report</strong> dialog box is displayed.</li>
   -->

<!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the <strong>Repeating Deliveries</strong>&nbsp;tab.<br><img src="assets/report-delivery-schedule-350x169.png" alt="" style="width: 350;height: 169;"></li>
   -->

<!--
   <li value="4" data-mc-conditions="QuicksilverOrClassic.Draft mode">(Conditional)&nbsp;To modify an existing repeating report delivery, select the report delivery in the <strong>Repeating Deliveries</strong>&nbsp;section.</li>
   -->

<!--
   <li value="5" data-mc-conditions="QuicksilverOrClassic.Draft mode">Specify the following information:
   <ul>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Send to:</strong> Begin typing the name of the user, group, team, or role who you want to send&nbsp;the report to, then click the name when it appears in the drop-down list.<br>Or<br>Specify the email address of a person external to the Workfront system who you want to have access to the report.<br> Repeat this process to send the report to multiple users, groups, teams, or roles.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Email Subject:</strong> Specify a subject for the email notification.<br> By default, the email subject is: <em>Workfront Report: <Name of the report> Date of the Export</em>.<strong></strong></li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Email Message:</strong> Specify a message to include in the email.<br>By default, the email message is:&nbsp;<em>Attached is the <report frequency> report <Name of the report> generated by Workfront on <Date>.</em><br>
   <note type="note">
   For reports delivered as an Excel file only, the following message is also added to the email: "Please be aware that with MS Excel (XLS) file types, there is a limit (65,530) on the number of hyperlinks these file types support. If you exceed those limits, your file will not open and it is recommended to resend without the hyperlinks.&nbsp;Please go back to the report scheduler&nbsp;to remove hyperlinks and resend the report." The "please go back to the report scheduler" phrase is a link back to the report.&nbsp;
   </note>
   </li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Deliver this report with the Access Rights of:</strong>&nbsp;Begin typing the name of a user who has access to the report, then click the name when it appears&nbsp;in the drop-down list. Users who receive the report will be granted the same level of access to the report as the user that you specify&nbsp;here.<br> For more information, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">Run and deliver a report with the access rights of another user</a>
   <note type="note">
   This field does not support wildcards. For example, using the wildcard $$User.ID does not run the report with the access rights of the user who is receiving the report.
   </note>
   </li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Format:</strong> Select in which of the following formats you want the report to be delivered:
   <ul>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> HTML</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">PDF</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">MS&nbsp;Excel</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">MS Excel (.xlsx)</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">TSV &nbsp;</li>
   </ul></li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Include Links:</strong>&nbsp;This option is available&nbsp;only when <strong>MS Excel</strong> is selected in the <strong>Format</strong> drop-down menu. When this option is enabled, any hyperlinks are included in the exported Excel document. <br>Documents that contain more than 65,530 links cannot be opened. If the exported document will contain more than 65,530 links, deselect this option.<br>This option is enabled by default.&nbsp;</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Summary:</strong> Displays a summary of when the delivery repeats.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Repeats:</strong> Select whether the report should be delivered daily, weekly, monthly, or yearly.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Repeats Every:</strong> Select the frequency with which you want&nbsp;the delivery to repeat. The value you select for this option is&nbsp;based on the option that is selected in the <strong>Repeats</strong>&nbsp;drop-down list.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Time:</strong> Select the time of day for the delivery to be sent.</li>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Repeats On:</strong>&nbsp;This option is available when the <strong>Repeats</strong>&nbsp;option is set to either <strong>Weekly</strong>&nbsp;or <strong>Monthly</strong>.</p>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">When the <strong>Repeats</strong>&nbsp;option is set to <strong>Weekly</strong>: Select the days of the week that the delivery is sent.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">When the <strong>Repeats</strong>&nbsp;option is set to <strong>Monthly</strong>: Select whether the delivery is sent on the day of the month, day of the week, or last day of the month (these options leverage the date that you select in the <strong>Starts On</strong>&nbsp;field).</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Starts On:</strong> Select the date for the scheduled delivery to begin.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Ends On:</strong> Select a date for the scheduled delivery to end. <br>Or</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Select <strong>Never</strong>&nbsp;if you want the scheduled delivery to last indefinitely.</li>
   -->

<!--
   <li value="6" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Save</strong>&nbsp;to save the report delivery.<br> The report is saved in the <strong>Repeating Deliveries</strong>&nbsp;section&nbsp;(in the <strong>Send Report</strong> dialog box).<br> The report will be sent at the schedule time<br>Or<br>To manually send the report, click <strong>Send Now</strong>.<br>For more information about sending the report instantly or manually, see&nbsp;.</li>
   -->

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Deleting a Scheduled Report Delivery</h2>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">Go to the report with the delivery you want to delete.</li>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Report Actions</strong>, then <strong>Send Report</strong>.&nbsp;</li>
   -->

<!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Repeating Deliveries</strong>.&nbsp;</li>
   -->

<!--
   <li value="4" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click the name of the scheduled delivery you want to delete, then click <strong>Delete</strong>. The report is no longer set up for the scheduled delivery.&nbsp;</li>
   -->

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Sending a Report Manually, on a One-Time Basis</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can manually send a report&nbsp;that has been previously scheduled, or you can create a single-use report delivery.​</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a title="Setting Up Report Deliveries" href="#sending-a-scheduled-report-now" class="MCXref xref">Sending a Scheduled Report Now</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a title="Setting Up Report Deliveries" href="#sending-a-report-one-time-only" class="MCXref xref">Sending a Report (One Time Only)</a> </li>
  -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="sending-a-scheduled-report-now">Sending a Scheduled Report Now</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">After a scheduled report has been set up, you can manually send the report rather than&nbsp;waiting until the scheduled time.</p>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">Navigate to and click the name of the report that you want to send now.</li>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Report Actions</strong>, then&nbsp;<strong>Send Report</strong>.<br> The Send Report dialog box is displayed.</li>
   -->

<!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click the <strong>Repeating Deliveries</strong> tab.</li>
   -->

<!--
   <li value="4" data-mc-conditions="QuicksilverOrClassic.Draft mode">In the <strong>Repeating Deliveries</strong>&nbsp;section, select the report delivery that was previously created.<br><img src="assets/report-delivery-schedule-send-350x160.png" alt="" style="width: 350;height: 160;"></li>
   -->

<!--
   <li value="5" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Send Now</strong>.<br> The report is sent to all users identified in the scheduled delivery.</li>
   -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="sending-a-report-one-time-only">Sending a Report (One Time Only)</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can manually send a report at any time. When you send a report in this way, delivery information (such as&nbsp;the users you are sending to and&nbsp;the email subject) are not saved. If you want to create a report delivery that you can save for later use, create a repeating scheduled report.&nbsp;</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To send a report to users (one time only):</p>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">Navigate to and click the name of the report that you want to send now.</li>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Report Actions</strong>, then&nbsp;<strong>Send Report</strong>.<br> The <strong>Send Report</strong> dialog box is displayed.<br><img src="assets/report-delivery-sendnow-350x351.png" alt="" style="width: 350;height: 351;"></li>
   -->

<!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">On the <strong>Send Now</strong>&nbsp;tab, specify the following information:
   <ul>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Send to:</strong> Begin typing the name of the user, group, team, or role who you want to send&nbsp;the report to, then click the name when it appears in the drop-down list.&nbsp;Or, specify the email address of a person external to the Workfront system who you want to have access to the report.<br> Repeat this process to send the report to multiple users, groups, teams, or roles.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Email Subject:</strong> Specify a subject for the email notification.<br> By default, the email subject is: <em>Workfront Report: <Name of the report> Date of the Export</em>.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Email Message:</strong> Specify a message to include in the email.<br>By default, the email message is:&nbsp;<em>Attached is the <report frequency> report <Name of the report> generated by Workfront on <Date>.</em><br>
   <note type="note">
   For reports delivered as an Excel file only, the following message is also added to the email: "Please be aware that with MS Excel (XLS) file types, there is a limit (65,530) on the number of hyperlinks these file types support. If you exceed those limits, your file will not open and it is recommended to resend without the hyperlinks.&nbsp;Please go back to the report scheduler&nbsp;to remove hyperlinks and resend the report." The "please go back to the report scheduler" phrase is a link back to the report.&nbsp;
   </note>
   </li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Deliver this report with the Access Rights of:</strong>&nbsp;Begin typing the name of a user who has access to the report, then click the name when it appears&nbsp;in the drop-down list. Users who receive the report will be granted the same level of access to the report as the user that you specify&nbsp;here.<br> For more information, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">Run and deliver a report with the access rights of another user</a>.
   <note type="note">
   This field does not support wildcards. For example, using the wildcard $$User.ID does not run the report with the access rights of the user who is receiving the report.
   </note>
   </li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Format:</strong> Select in which of the following formats you want the report to be delivered:
   <ul>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> HTML</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">PDF</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">MS Excel</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">MS&nbsp;Excel (.xlsx)</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">TSV</li>
   </ul></li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Include Links:</strong>&nbsp;This option is available&nbsp;only when <strong>MS Excel</strong> is selected in the <strong>Format</strong> drop-down menu. When this option is enabled, any hyperlinks are included in the exported Excel document. <br>Documents that contain more than 65,000 links cannot be opened. If the exported document will contain more than 65,000 links, deselect this option.<br>This option is enabled by default.</li>
   </ul></li>
   -->

<!--
   <li value="4" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Send Now</strong>.<br> The report is sent to all users that you identified.<br> Or<br> Click <strong>Make Repeating Delivery</strong>&nbsp;if you want to set up&nbsp;a scheduled delivery with this same information, then complete the additional information regarding the frequency of when the report is sent.</li>
   -->
