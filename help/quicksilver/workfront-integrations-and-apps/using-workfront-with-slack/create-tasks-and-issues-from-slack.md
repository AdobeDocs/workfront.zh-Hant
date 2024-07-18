---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: 從Slack建立任務和問題
description: 安裝並設定 [!DNL Adobe Workfront] 以進行Slack後，您可以從Slack建立任務和問題，並將它們與Workfront中的專案建立關聯。
author: Becky
feature: Workfront Integrations and Apps
exl-id: cf4a514a-fe69-4c2f-8e35-5738dfaab24e
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---

# 從[!DNL Slack]建立任務和問題

安裝並設定[!DNL Adobe Workfront for Slack]後，您可以從[!DNL Slack]建立任務和問題，並將它們與[!DNL Workfront]中的專案建立關聯。

如需使用[!DNL Slack]設定[!DNL Workfront]的詳細資訊，請參閱[設定 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)。

您必須有存取權才能在存取層級中建立任務和問題，而且您必須對建立任務和問題關聯的專案具有[!UICONTROL Contribute]許可權。

如需存取層級的詳細資訊，請參閱[存取層級概觀](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)。 如需物件許可權的詳細資訊，請參閱[物件許可權共用簡介](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。

## 存取需求

您必須具備下列條件：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront]計畫]</a>*</td> 
   <td> <p>[！UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請連絡您的[!DNL Workfront]管理員。\

## 先決條件

在您可以從[!DNL Slack]建立任務和問題之前，您必須

* 設定[!DNL Workfront]以進行Slack\
   如需設定[!DNL Workfront for Slack]的說明，請參閱[設定 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)。

## 從[!DNL Slack]建立任務

1. 登入您的[!DNL Slack]執行個體並從[!DNL Slack]登入[!DNL Workfront]。\
   如需有關從[!DNL Slack]登入Workfront的詳細資訊，請參閱[存取 [!DNL Adobe Workfront] 從 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)中的「從[!DNL Slack]登入[!DNL Workfront]」區段。

1. 從任何通道中，開始在訊息欄位中輸入以下命令：

   `/workfront add task <Task Name>`

   >[!NOTE]
   >
   >命令區分大小寫。 您可以使用`/wf`來啟動命令，而非`/workfront`。
   >  
   >必須輸入工作名稱，因為它會顯示在[!DNL Workfront]介面中，不含括弧或引號。

1. （選擇性）開始輸入專案名稱，以與新任務建立關聯，並在專案出現在清單中時選取它。\
   您會收到一則確認訊息，指出任務已新增至選取的專案。
1. （選擇性）在確認訊息中按一下工作名稱，以在新的瀏覽器分頁中的[!DNL Workfront]中開啟。

## 從[!DNL Slack]建立問題

1. 登入您的[!DNL Slack]執行個體並從[!DNL Slack]登入[!DNL Workfront]。\
   如需有關從[!DNL Slack]登入[!DNL Workfront]的詳細資訊，請參閱[Access [!DNL Adobe Workfront] from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)中的「從[!DNL Slack]登入[!DNL Workfront]」區段。

1. 從任何通道中，開始在訊息欄位中輸入以下命令：

   `/workfront add issue <Issue Name>`

   >[!NOTE]
   >
   >命令區分大小寫。 您可以使用「/wf」而不是「/workfront」來啟動命令。 \
   >必須輸入問題名稱，因為它將出現在[!DNL Workfront]介面中，不帶括弧或引號。

1. （可選）開始輸入專案名稱，您要將新問題與其建立關聯，並在它出現在清單中時選取它。\
   您會收到一則確認訊息，指出問題已新增至選取的專案。
1. （選擇性）在確認訊息中按一下問題名稱，以在新的瀏覽器分頁中的[!DNL Workfront]中開啟。
