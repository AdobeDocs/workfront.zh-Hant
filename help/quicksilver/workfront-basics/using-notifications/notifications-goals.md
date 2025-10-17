---
content-type: reference
navigation-topic: notifications
title: 通知：目標
description: 通知：目標
author: Courtney, Alina
feature: Get Started with Workfront
exl-id: 12e66711-4438-4fcf-af79-7fcc2c3b1522
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 2%

---

# 通知：目標

您可以針對設定檔中發生[!DNL Adobe Workfront Goals]的事件啟用電子郵件通知。 擁有[!UICONTROL 計畫]授權的使用者也可以為其他使用者啟用它們。 如需詳細資訊，請參閱[[!DNL Adobe Workfront] 通知](../../workfront-basics/using-notifications/wf-notifications.md)。

## 存取需求

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: because there are conditions for who sees this, I added this from the How To articles/ template although this is not a How To. But I like the format, so I thought keeping it consistent might help users. We may decide to update this when we have access and prereq for overview-type articles)</p>
-->

+++ 展開以檢視本文中功能的存取需求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront package]</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 授權</strong></td> 
   <td>
   <p>投稿人或以上</p>
    <p>要求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>其他產品</strong></td> 
   <td>[!DNL Workfront Goals] <p>如需[!DNL Workfront Goals]的相關資訊，請參閱<a href="../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">[!DNL Adobe Workfront Goals]概述</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>存取層級設定*</strong></td> 
   <td> <p>[!UICONTROL View]存取[!DNL Goals]或更新版本</p></td> 
  </tr>
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

* 您要更新其[!DNL Goals]個通知的使用者必須有包括[!DNL Goals]主要功能表[!UICONTROL 中的]區域的配置範本。


## [!DNL Goals]使用者設定檔[!UICONTROL 區域中的]個通知

下表列出的通知會提醒您有關[!DNL Workfront Goals]中發生的事件，例如有人指派目標、結果或活動給您，或有人對您擁有的目標、結果或活動進行更新。 如需有關設定您收到哪些通知的資訊，請參閱[修改您自己的電子郵件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)。

![通知偏好設定](assets/goals-notifications-preferences-350x114.png)

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
   <td> <p>將結果或活動指派給您的人員姓名</p> <p>結果或活動的目標期間</p> <p>結果或活動的名稱</p> <p><strong>[!UICONTROL 在網頁應用程式中開啟]</strong>按鈕可開啟[!UICONTROL 目標詳細資料]面板</p> <p><strong>[!UICONTROL 變更通知設定]</strong>按鈕可讓您管理通知。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>有人為我建立了新的個人目標</strong> </td> 
   <td> <p>指派目標的人員名稱</p> <p>目標的期間</p> <p>目標的名稱</p> <p><strong>[!UICONTROL 在網頁應用程式中開啟]</strong>按鈕可開啟[!UICONTROL 目標詳細資料]面板</p> <p><strong>[!UICONTROL 變更通知設定]</strong>按鈕可讓您管理通知。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>有人對我目標上的更新留言</strong></td> 
   <td> <p>留下評論的人員的姓名</p> <p>目標的期間 </p> <p>目標的名稱</p> <p>註解的文字</p> <p><strong>[!UICONTROL 在網頁應用程式中開啟]</strong>按鈕可開啟[!UICONTROL 目標詳細資料]面板</p> <p><strong>[!UICONTROL 變更通知設定]</strong>按鈕可讓您管理通知。</p> </td> 
  </tr> 
  <tr> 
  </tbody> 
</table>

<!--these were removed at some point: 

   <td><strong>Someone liked my comment on a Goal</strong></td> 
   <td> <p>The name of the person who liked the comment</p> <p>The Period of the goal </p> <p>The name of the goal</p> <p>The text of the comment </p> <p>The <strong>[!UICONTROL Open in web app]</strong> button which opens the [!UICONTROL Goal Details] panel</p> <p>The <strong>[!UICONTROL Change Notifications Settings]</strong> button which allows you to manage your notifications.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Someone liked an update on my Goal</strong></td> 
   <td> <p>You receive an email when someone likes a comment you made on a goal or when you update the progress of your results or activities on the goal. </p> <p>The name of the person who liked the update</p> <p>The Period of the goal </p> <p>The name of the goal</p> <p>The <strong>[!UICONTROL Open in web app]</strong> button which opens the [!UICONTROL Goal Details] panel</p> <p>The <strong>[!UICONTROL Change Notifications Settings]</strong> button which allows you to manage your notifications.</p> </td> 
  </tr> 
 -->

<!--
NOTE FOR NAME OF GOAL IN LAST TABLE CELL: check this. Is this true? Didn't triggger when this was written; add anything else? Maybe the type of the update is mentioned?!
-->
