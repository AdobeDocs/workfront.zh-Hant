---
content-type: overview
product-area: projects;user-management
navigation-topic: plan-a-project
title: 項目所有者和贊助商概覽
description: 您可以為項目指定項目責任人和項目發起人。
author: Alina
feature: Work Management
exl-id: e3e8be3f-105f-4702-8c93-ae8092f5d5d3
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '562'
ht-degree: 0%

---

# 項目所有者和贊助商概覽

您可以為項目指定項目責任人和項目發起人。

項目所有者是負責按時和按預算完成項目的個人。

項目贊助方是項目的重要利益相關方，項目中投入了資源。 項目的完成通常有利於項目贊助商。

有關如何更新項目的項目所有者或贊助商的資訊，請參閱 [更新項目所有者和贊助商](../../../manage-work/projects/planning-a-project/update-project-owners-and-sponsors.md).

## 專案擁有者

您可以在專案或範本上指定專案擁有者，借此指定專案的管理員。

您只能為專案定義一個專案擁有者。

使用「項目所有者」欄位可以執行以下操作：

* 您只能指定一個使用者為專案擁有者。
* 您可以指定「專案擁有者」作為專案的小時核准者。
* 在定義項目、任務或發放審批流程時，您可以將項目責任人指定為一般審批人。 如需核准的相關資訊，請參閱 [編輯核准程式](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md).

   >[!IMPORTANT]
   >
   >當您為項目所有者分配了批准，並且沒有人被指定為項目的所有者時，該批准將重新分配給主Workfront管理員，如「設定」區域的「客戶資訊」部分所示。 如需詳細資訊，請參閱 [配置系統的基本資訊](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).


* 您可以啟用只傳送給專案擁有者的特定通知。

   如需電子郵件通知的詳細資訊，請參閱區段 [為系統中的每個人配置事件通知](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md#modify) 在文章中 [為系統中的每個人配置事件通知](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

* 您可以在報表或清單中顯示「專案擁有者」欄位。

   您也可以在檢視、分組或提示中顯示「專案擁有者」欄位。

   例如，您可以將下列文字模式運算式複製到篩選器中，以顯示登入使用者擁有的專案： 

   ```
   ownerID=$$USER.ID
   ```

如需建立報表的詳細資訊，請參閱文章 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update the Project Owner of a project</h2>
<p>(NOTE:&nbsp;drafted and moved to its own article)</p>
<ol>
<li value="1">Go to the project you want to update.</li>
<li value="2"> Click <strong>Project Details</strong> in the left panel. </li>
<li value="3"> Click&nbsp;the <strong>Edit</strong> icon <img src="assets/qs-edit-icon.png"> in the upper-right corner of the Project&nbsp;Details area, then click&nbsp;<strong>Overview</strong>.  </li>
<li value="4"> <p>Specify the name of a user for the <strong>Project Owner</strong> field.</p> <p>Only active users can be specified as Project Owners.</p> </li>
<li value="5"> Click&nbsp;<strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## 項目贊助商

您可以將系統中的任何用戶指定為項目發起人。 專案贊助者通常是需要了解專案發生狀況的經理、執行官或利害關係人。

指派專案贊助商時，請考量下列事項：

* 專案贊助者不會取得專案的任何其他存取權，但會新增至專案的電子郵件通知中。 如需通知的相關資訊，請參閱文章 [為系統中的每個人配置事件通知](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

* 您只能指定一個項目贊助商。
* 在定義項目、任務或發放審批流程時，您可以指定項目發起人作為一般審批人。 如需核准的相關資訊，請參閱 [編輯核准程式](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md).

   >[!IMPORTANT]
   >
   >當您為項目發起人分配了批准，並且沒有人被指定為項目的發起人時，批准將重新分配給項目責任人。 如果未指定任何人為專案的擁有者，則會將核准指派給Workfront管理員。

* 您可以在報表或清單中顯示「項目贊助商」欄位。

   您也可以在檢視、分組或提示中顯示「專案贊助商」欄位。

   例如，您可以將下列文字模式運算式複製到篩選器中，以顯示由登入使用者贊助的專案：

   ```
   sponsorID=$$USER.ID
   ```

    

   如需建立報表的詳細資訊，請參閱文章 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update the Project Sponsor of a project </h2>
<p>(NOTE: drafted and moved to its own article) </p>
<ol>
<li value="1">Go to the Project you want to update.</li>
<li value="2"> Click <strong>Project Details</strong> in the left panel. </li>
<li value="3"> Click&nbsp;the <strong>Edit</strong> icon <img src="assets/qs-edit-icon.png"> in the upper-right corner of the Project&nbsp;Details area, then click&nbsp;<strong>Overview</strong>.  </li>
<li value="4"> <p>Specify the name of a user for the <strong>Project Sponsor</strong> field.</p> <p>Only active users can be specified as Project Sponsors.</p> </li>
<li value="5"> Click&nbsp;<strong>Save Changes</strong>. </li>
</ol>
</div>
-->
