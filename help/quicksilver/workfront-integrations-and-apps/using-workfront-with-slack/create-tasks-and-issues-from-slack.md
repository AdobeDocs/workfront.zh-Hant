---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: 從Slack建立任務和問題
description: 為Slack安裝並設定 [!DNL Adobe Workfront] 後，您可以從Slack建立任務和問題，並將它們與Workfront中的專案建立關聯。
author: Becky
feature: Workfront Integrations and Apps
exl-id: cf4a514a-fe69-4c2f-8e35-5738dfaab24e
source-git-commit: 6178cabbf021fbf92bd8795c5c2bd0346801d64d
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 0%

---

# 從[!DNL Slack]建立任務和問題

安裝並設定[!DNL Adobe Workfront for Slack]後，您可以從[!DNL Slack]建立任務和問題，並將它們與[!DNL Workfront]中的專案建立關聯。

如需使用[!DNL Workfront]設定[!DNL Slack]的詳細資訊，請參閱[設定 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)。

您必須有存取權才能在存取層級中建立任務和問題，而且您必須對建立任務和問題關聯的專案具有[!UICONTROL Contribute]許可權。

如需存取層級的詳細資訊，請參閱[存取層級概觀](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)。 如需物件許可權的詳細資訊，請參閱[物件許可權共用簡介](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。

## 存取需求

+++ 展開以檢視本文中功能的存取需求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront套件</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權</td> 
   <td> <p>任何</p>
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先決條件

在您可以從[!DNL Slack]建立任務和問題之前，您必須

* 為Slack設定[!DNL Workfront]\
   如需設定[!DNL Workfront for Slack]的說明，請參閱[設定 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)。

## 從[!DNL Slack]建立任務

1. 登入您的[!DNL Slack]執行個體並從[!DNL Workfront]登入[!DNL Slack]。\
   如需有關從[!DNL Slack]登入Workfront的詳細資訊，請參閱[!DNL Workfront]存取[!DNL Slack]從[中的「從 [!DNL Adobe Workfront] 登入 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)」區段。

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

1. 登入您的[!DNL Slack]執行個體並從[!DNL Workfront]登入[!DNL Slack]。\
   如需有關從[!DNL Workfront]登入[!DNL Slack]的詳細資訊，請參閱[!DNL Workfront]Access[!DNL Slack]from[中的「從 [!DNL Adobe Workfront] 登入 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)」區段。

1. 從任何通道中，開始在訊息欄位中輸入以下命令：

   `/workfront add issue <Issue Name>`

   >[!NOTE]
   >
   >命令區分大小寫。 您可以使用「/wf」而不是「/workfront」來啟動命令。 \
   >必須輸入問題名稱，因為它將出現在[!DNL Workfront]介面中，不帶括弧或引號。

1. （可選）開始輸入專案名稱，您要將新問題與其建立關聯，並在它出現在清單中時選取它。\
   您會收到一則確認訊息，指出問題已新增至選取的專案。
1. （選擇性）在確認訊息中按一下問題名稱，以在新的瀏覽器分頁中的[!DNL Workfront]中開啟。
