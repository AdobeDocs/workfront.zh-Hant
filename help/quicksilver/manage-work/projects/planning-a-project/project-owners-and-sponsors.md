---
content-type: overview
product-area: projects;user-management
navigation-topic: plan-a-project
title: 專案所有者和贊助者概觀
description: 您可以為專案指定專案所有者和專案贊助者。
author: Alina
feature: Work Management
exl-id: e3e8be3f-105f-4702-8c93-ae8092f5d5d3
source-git-commit: 111c776af19fbc2982c14cc9d3b3778d37bc0be3
workflow-type: tm+mt
source-wordcount: '562'
ht-degree: 0%

---

# 專案所有者和贊助者概觀

<!-- Audited: 1/2024 -->

您可以為專案指定專案所有者和專案贊助者。

專案所有者是負責依照預算準時完成專案的個人。

專案贊助者是專案的重要利害關係人，專案中有資源投資於專案。 專案完成通常有利於專案贊助者。

如需有關如何更新專案的專案所有者或贊助者的資訊，請參閱 [更新專案所有者和贊助者](../../../manage-work/projects/planning-a-project/update-project-owners-and-sponsors.md).

## 專案所有者

您可以在專案或範本上指定專案所有者，以指定專案經理。

您只能為一個專案定義一個專案所有者。

以下為使用「專案所有者」欄位時的可能方式：

* 您只能指定一個使用者作為專案所有者。
* 您可以指定「專案所有者」為專案的時數核准者。
* 在定義專案、任務或問題核准流程時，您可以指定「專案所有者」作為一般核准者。 如需關於核准的資訊，請參閱 [編輯核准流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md).

  >[!IMPORTANT]
  >
  >當您將核准指派給專案所有者，且沒有人被指定為專案的所有者時，核准將重新指派給主要Workfront管理員，如設定區域的客戶資訊區段中所述。 如需詳細資訊，請參閱 [設定系統的基本資訊](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).
  >


* 您可以啟用只傳送給專案所有者的某些通知。

  如需電子郵件通知的詳細資訊，請參閱區段 [為系統中的每個人設定事件通知](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md#modify) 在文章中 [為系統中的每個人設定事件通知](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

* 您可以在報告或清單中顯示「專案所有者」欄位。

  您也可以在檢視、分組或提示中顯示「專案所有者」欄位。

  例如，您可以將下列文字模式運算式複製到篩選中，以顯示登入使用者擁有的專案： 

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

## 專案贊助者

您可以將系統中的任何使用者指定為專案贊助者。 專案贊助者通常是需要瞭解專案情況的經理、執行或利害關係人。

指派專案贊助者時，請考慮下列事項：

* 專案贊助者未取得專案的任何額外存取權，但會新增到專案的電子郵件通知中。 如需有關通知的資訊，請參閱文章 [為系統中的每個人設定事件通知](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

* 您只能指定一個專案贊助者。
* 在定義專案、任務或問題核准流程時，您可以將專案贊助者指定為一般核准者。 如需關於核准的資訊，請參閱 [編輯核准流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md).

  >[!IMPORTANT]
  >
  >當您將核准指派給「專案贊助者」，且沒有指定任何人員作為專案的贊助者時，核准將重新指派給「專案所有者」。 如果未指定任何人為專案的所有者，則會將核准指派給Workfront管理員。

* 您可以在報告或清單中顯示「專案贊助者」欄位。

  您也可以在檢視、分組或提示中顯示專案贊助者欄位。

  例如，您可以將下列文字模式運算式複製到篩選中，以顯示由登入使用者贊助的專案：

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
