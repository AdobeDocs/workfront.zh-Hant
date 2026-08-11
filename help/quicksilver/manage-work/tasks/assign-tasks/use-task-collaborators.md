---
title: 使用任務共同作業人員
content-type: reference
description: 瞭解如何使用可指派給Workfront任務的任務共同作業人員、AI共同作業人員。
author: Becky
feature: Work Management, Tasks
source-git-commit: 72921e4a1cb9ca564a5c8b4a7a587e37f6a90cc5
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 2%

---

# 使用任務共同作業人員

{{highlighted-preview-article-level}}

任務共同作業人員是可直接指派給Workfront任務的AI共同作業人員，此外還有用於檔案和資產檢閱的現有檢閱者型別AI共同作業人員。 就像其他AI共同作業人員一樣，任務共同作業人員會在「設定」區域中設定，並像使用者一樣指派給任務。

工作共同作業人員會連線到您已設定的代理程式，很像是MCP伺服器。

如需有關在Workfront中建立工作共同作業人員的資訊和指示，請參閱設定AI共同作業人員一文中的[設定工作共同作業人員](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-task-collaborator)。

## 存取權要求

+++ 展開以檢視這篇文章中所述功能的存取權要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 封裝</td> 
   <td><p>選取、Prime或Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 授權</td> 
   <td><p>[!UICONTROL 標準]</p>
  </tr> 
  <tr> 
   <td>存取層級設定</td> 
   <td>[!UICONTROL 系統管理員]</td> 
  </tr> 
  </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

* 您必須先在Copilot、Claude或Writer.ai中設定代理程式，才能將它當做工作共同作業人員使用。

## 任務共同作業人員總覽

任務共同作業人員是將MCP代理指派給Workfront中特定任務的方法。 您可以在Copilot Studio、Claude或Writer.ai等應用程式中設定代理程式，然後將該代理程式以工作共同作業人員的身分連線至Workfront。 然後，您可以像指派使用者一樣將其指派給任務。

某些範例工作流程可能包括：

* 偵測已上傳至任務的影像、根據提供給代理程式的條件產生變數，並將新影像上傳至任務。
* 從工作說明產生復本、根據代理程式中設定的准則複查復本，並將復本張貼至更新流。
* 讀取事件的詳細資料、識別遺漏的詳細資料，以及在更新流中發佈有關遺漏詳細資料的問題。

>[!NOTE]
>
>* 有關代理程式職責和能力的特定詳細資訊是在建立代理程式的應用程式中設定，而不是在Workfront中設定。
>* 任務共同作業人員目前支援在Copilot Studio、Claude和Writer.ai中建立的代理。
>* 在Copilot Studio中設定代理程式時，您必須將安全性設定為&#x200B;**無驗證**。
>* 如需有關在Workfront中建立工作共同作業人員的資訊和指示，請參閱設定AI共同作業人員一文中的[設定工作共同作業人員](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-task-collaborator)。

## 任務共同作業程式啟動觸發程式

當任務共同作業人員被指派給任務時，它會在滿足以下任何情況時開始工作：

* 已將任務共同作業人員指派給已準備好開始的任務。 （例如，如果任務具有前置任務，則前置任務為完成。）
* 任務共同作業人員和使用者會獲派任務，而任務共同作業人員會先獲派。
* 已經將任務共同作業人員指派給的任務，其已準備好開始，且任務共同作業人員是唯一或主要受指派人。 （例如，如果任務具有前置任務，則前置任務為完成。）
* 已為其指派任務共同作業人員和使用者的任務變為準備開始，且任務共同作業人員已先受指派或為主要受指派人。 （例如，如果任務具有前置任務，則前置任務為完成。）
* 使用者和任務共同作業人員會指派給任務，且使用者會被移除。
* 使用者和任務共同作業人員被指派給任務，任務共同作業人員被設定為該任務的主要受指派人。

下列情況不會導致任務共同作業人員開始處理任務：

* 已將任務共同作業人員指派給已指派使用者的任務。
* 在任務中@mentioned立任務共同作業人員。
* 「任務共同作業人員」會指派給已指派「任務共同作業人員」的任務。 在這種情況下，第一個指派的任務共同作業人員將已開始工作，第二個任務共同作業人員將不會執行任何動作。
* 已將任務共同作業人員指派給未準備好開始的任務。 （例如，如果任務具有前置任務，則前置任務尚未完成。）

## 將任務共同作業人員指派給任務

任務指派給共同作業人員的工作方式，與指派使用者的方式相同。

當您在可用受指派人清單中搜尋任務共同作業人員時，任務共同作業人員的名稱只是名字。

如需指示，請參閱[指派工作](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md)。
