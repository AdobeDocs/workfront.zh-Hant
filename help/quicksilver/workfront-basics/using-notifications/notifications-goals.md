---
content-type: reference
navigation-topic: notifications
title: 「通知：目標」
description: 「通知：目標」
author: Lisa
feature: Get Started with Workfront
exl-id: 12e66711-4438-4fcf-af79-7fcc2c3b1522
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '567'
ht-degree: 3%

---

# 通知：目標

您可以針對設定檔中發生[!DNL Adobe Workfront Goals]的事件啟用電子郵件通知。 擁有[!UICONTROL 計畫]授權的使用者也可以為其他使用者啟用它們。 如需詳細資訊，請參閱[[!DNL Adobe Workfront] 通知](../../workfront-basics/using-notifications/wf-notifications.md)。

## 存取需求

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: because there are conditions for who sees this, I added this from the How To articles/ template although this is not a How To. But I like the format, so I thought keeping it consistent might help users. We may decide to update this when we have access and prereq for overview-type articles)</p>
-->

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>[！UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權*</strong></td> 
   <td> <p>[！UICONTROL Request]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>產品</strong></td> 
   <td>[!DNL Workfront Goals] <p>如需[!DNL Workfront Goals]的相關資訊，請參閱<a href="../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">[!DNL Adobe Workfront Goals]概述</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>存取層級設定*</strong></td> 
   <td> <p>[！UICONTROL View]存取[!DNL Goals]或更新版本</p> <p>注意：如果您還是沒有存取權，請詢問您的[!DNL Workfront]管理員是否對您的存取層級設定了其他限制。 如需[!DNL Workfront]管理員如何變更您的存取層級的詳細資訊，請參閱<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>。</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>[Insert permissions needed]</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。

## 先決條件

更新[!DNL Goals]通知的使用者必須具備下列條件：

* 包含[!UICONTROL 主要功能表]中[!DNL Goals]區域的配置範本。
* 存取新的[!DNL Adobe Workfront]體驗。

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: we need this here because you can see these notifications from Classic)
  </MadCap:conditionalText>
  -->

## [!UICONTROL 使用者設定檔]區域中的[!DNL Goals]個通知

下表列出的通知會提醒您有關[!DNL Workfront Goals]中發生的事件，例如有人指派目標、結果或活動給您，或有人對您擁有的目標、結果或活動進行更新。 如需有關設定您收到哪些通知的資訊，請參閱[修改您自己的電子郵件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)。

![](assets/goals-notifications-preferences-350x114.png)

>[!NOTE]
>
>[!DNL Goals]的即時通知預設為停用。 您無法啟用或停用每日通知，並且不會收到此類別中事件的每日摘要電子郵件。 您可以啟用或停用[!DNL Goals]類別的個別即時通知。

另請參閱[事件通知](../../workfront-basics/using-notifications/event-notifications.md)。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>通知</strong></td> 
   <td> <p><strong>欄位已包含</strong> </p> <p><strong>*僅即時通知</strong></p> </td> 
  </tr> 
  <tr> 
   <td><strong>有人將結果/活動指派給我</strong></td> 
   <td> <p>將結果或活動指派給您的人員姓名</p> <p>結果或活動的目標期間</p> <p>結果或活動的名稱</p> <p><strong>[！UICONTROL在網頁應用程式中開啟]</strong>按鈕可開啟[！UICONTROL目標詳細資料]面板</p> <p><strong>[！UICONTROL變更通知設定]</strong>按鈕可讓您管理通知。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>有人為我建立了新的個人目標</strong> </td> 
   <td> <p>指派目標的人員名稱</p> <p>目標的期間</p> <p>目標的名稱</p> <p><strong>[！UICONTROL在網頁應用程式中開啟]</strong>按鈕可開啟[！UICONTROL目標詳細資料]面板</p> <p><strong>[！UICONTROL變更通知設定]</strong>按鈕可讓您管理通知。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>有人對我目標上的更新留言</strong></td> 
   <td> <p>留下評論的人員的姓名</p> <p>目標的期間 </p> <p>目標的名稱</p> <p>註解的文字</p> <p><strong>[！UICONTROL在網頁應用程式中開啟]</strong>按鈕可開啟[！UICONTROL目標詳細資料]面板</p> <p><strong>[！UICONTROL變更通知設定]</strong>按鈕可讓您管理通知。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>有人對我目標上的更新點讚</strong></td> 
   <td> <p>喜歡註解的人的名稱</p> <p>目標的期間 </p> <p>目標的名稱</p> <p>註解的文字 </p> <p><strong>[！UICONTROL在網頁應用程式中開啟]</strong>按鈕可開啟[！UICONTROL目標詳細資料]面板</p> <p><strong>[！UICONTROL變更通知設定]</strong>按鈕可讓您管理通知。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>有人對我目標上的更新點讚</strong></td> 
   <td> <p>當有人喜歡您對目標的評論，或者您更新目標上的結果或活動的進度時，您會收到電子郵件。 </p> <p>喜歡此更新的人員姓名</p> <p>目標的期間 </p> <p>目標的名稱</p> <p><strong>[！UICONTROL在網頁應用程式中開啟]</strong>按鈕可開啟[！UICONTROL目標詳細資料]面板</p> <p><strong>[！UICONTROL變更通知設定]</strong>按鈕可讓您管理通知。</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
NOTE FOR NAME OF GOAL IN LAST TABLE CELL: check this. Is this true? Didn't triggger when this was written; add anything else? Maybe the type of the update is mentioned?!
-->
