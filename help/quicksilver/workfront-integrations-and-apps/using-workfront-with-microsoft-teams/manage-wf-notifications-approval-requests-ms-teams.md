---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: 管理 [!DNL Adobe Workfront] 團隊中的 [!DNL Microsoft] 通知
description: 您可以接收來自 [!DNL Adobe Workfront] 的通知，內容有關您需要核准的專案、已指派給您的工作分派，或您關聯專案的註解與變更。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 7771a7d7-7e20-4b3d-95e7-1050aeb3af67
source-git-commit: 4cf780aa1b1221cd6ff8e6ce58fbb7d3621f7fa9
workflow-type: tm+mt
source-wordcount: '1434'
ht-degree: 0%

---

# 管理[!DNL Adobe Workfront]中的[!DNL Microsoft Teams]個通知

>[!IMPORTANT]
>
>隨著[Microsoft轉換至「新團隊」使用者端](https://learn.microsoft.com/en-us/microsoftteams/teams-classic-client-end-of-availability)，傳統團隊使用者端在2025年7月1日之後將不再可用。 若要繼續使用Microsoft Teams和Workfront等整合式應用程式，客戶必須在此日期之前轉換至新Teams使用者端。
>
>更新的Workfront整合現在可供使用，並且與新團隊體驗完全相容。 在大多數情況下，使用者轉換後，Workfront會自動顯示。 如果不適用，可從Microsoft Teams App Store手動安裝整合。 若要在New Teams使用者端中安裝或驗證Workfront整合，請參閱[為Microsoft Teams [!DNL Adobe Workfront] 安裝](/help/quicksilver/workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md)。

您可以從[!DNL Adobe Workfront]接收有關您需要核准的專案、已給予您的指派，或您關聯專案的評論和變更的通知。

這些通知包含[!DNL Workfront]個動作，您可以在[!DNL Microsoft Teams]內採取這些動作，不需離開[!DNL Microsoft Teams]即可完成這些動作。

>[!NOTE]
>
>[!DNL Microsoft Teams]不再支援[!DNL Internet Explorer]。 若要使用[!DNL Adobe Workfront for Microsoft Teams integration]，您必須使用[!DNL Internet Explorer]以外的網頁瀏覽器。




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
   <td> <p>標準</p>
   <p>工作或更高</p> </td> 
  </tr> 
 </tbody> 
</table>

如需詳細資訊，請參閱Workfront檔案中的[存取需求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在[!DNL Workfront]中接收[!DNL Microsoft Teams]通知的必要條件

如果符合下列條件，您可以在[!DNL Workfront]中接收[!DNL Microsoft Teams]通知：

* 團隊擁有者已為您的團隊安裝和設定[!DNL Workfront for Microsoft Teams]。
* 您已從[!DNL Workfront]登入[!DNL Microsoft Teams]。
* 您已在[!DNL Workfront]中啟用立即通知。 如需啟用即時通知的詳細資訊，請參閱[修改您自己的電子郵件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)。

如需有關安裝[!DNL Workfront for Microsoft Teams]和登入[!DNL Workfront from Microsoft Teams]的資訊，請參閱[安裝 [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md)。

## 管理[!DNL Workfront]中的[!DNL Microsoft Teams]個通知

安裝[!DNL Workfront for Microsoft Teams]應用程式後，會在[!DNL Workfront]中為該團隊的每個成員建立[!DNL Microsoft Teams]聊天頻道。 在[!DNL Workfront]中執行特定動作時，您可以設定[!DNL Workfront for Microsoft Teams]的設定，以在[!DNL Workfront]的[!DNL Microsoft Teams]聊天頻道中接收有關該動作的通知。

處理來自[!DNL Workfront]的[!DNL Microsoft Teams]個通知時，請考慮下列事項：

* 您無法在[!DNL Workfront]中接收全部，但只能接收選取數量的[!DNL Microsoft Teams]則通知。
* 您從[!DNL Workfront]收到的所有通知都會顯示在[!DNL Workfront]機器人聊天頻道中。

  如需有關安裝[!DNL Workfront]機器人頻道的資訊，請參閱[安裝 [!DNL Workfront] 文章中的 [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md#logging-in-to-workfront)登入[來自 [!DNL Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md)區段。

* 從[!DNL Workfront]中完成更新到您在[!DNL Microsoft Teams]中收到有關該更新的通知之間最多可能有5分鐘的延遲。
* 對於每個[!DNL Microsoft Teams]通知，您也會收到電子郵件通知。

若要管理可在[!DNL Workfront]中收到的[!DNL Microsoft Teams]通知：

1. 按一下&#x200B;**[!UICONTROL 中左側導覽列上的]**&#x200B;更多新增[!DNL Microsoft Teams] （三點）應用程式圖示。

1. 在出現的清單中按一下[!DNL Workfront]。
1. 選取「**[!UICONTROL 設定]**」標籤。

   ![MS Teams設定標籤](assets/ms-teams-settings-tab-350x552.png)

1. 停用您不想接收的任何通知。 您可以啟用或停用通知群組，例如資訊或核准通知，也可以個別管理通知。

   預設會啟用所有通知。

   [!DNL Workfront for Microsoft]團隊的通知設定會自動儲存。

   >[!NOTE]
   >
   >您無法新增更多通知至預設可用的通知。

## 在[!DNL Workfront]中回應[!DNL Microsoft Teams]個通知和核准要求

1. 從[!DNL Workfront]登入[!DNL Microsoft Teams]。\
   如需有關登入[!DNL Workfront]的資訊，請參閱[安裝 [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md)。

1. 前往&#x200B;**[!UICONTROL 聊天]**&#x200B;區域並按一下&#x200B;**[!DNL Workfront]**&#x200B;機器人頻道。\
   此頻道用於您與[!DNL Workfront]機器人的個人聊天。 所有[!DNL Workfront]通知都會顯示在這裡。
1. 根據您收到的通知型別，請前往相關區段：

   * [核准通知](#approval-notifications-approval-notifications)
   * [指派通知](#assignment-notifications-assignment-notifications)
   * [註解通知](#comment-notifications-comment-notifications)
   * [更新通知](#update-notifications-update-notifications)
   * [日期變更通知](#date-change-notifications-date-change-notifications)

### 核准通知 {#approval-notifications}

當您被要求核准物件時（例如任務、時程表或校訂），您會收到核准通知。 不過，您仍然可以在通知上加上註解。您可以在核准通知中執行下列動作：

* **[!UICONTROL 核准]**：按一下以核准專案。
* **[!UICONTROL 變更]**：按一下以核准有變更的專案。
* **[!UICONTROL 拒絕]**：按一下以拒絕專案。
* **[!UICONTROL 註解]**：按一下即可發表註解。 您的註解也會在[!DNL Workfront]中顯示為通知相關物件的更新。
* **[!UICONTROL 前往校訂]**：按一下以開啟校訂。 然後，您可以直接在校訂中做出決定。 如需詳細資訊，請參閱[在校訂檢視器中對校訂做出決定](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)。

>[!NOTE]
>
>一旦您做出核准決定，就無法從通知變更它。

#### 特定核准通知上的可用動作：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>通知</th> 
   <th>[!UICONTROL 核准]</th> 
   <th>[!UICONTROL 拒絕]</th> 
   <th> <p>[!UICONTROL 變更]</p> </th> 
   <th> <p>[!UICONTROL 前往校訂] </p> </th> 
   <th>[!UICONTROL 註解]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">您必須核准專案</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">您需要核准任務</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">您需要核准問題</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">您需要核准檔案</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">您必須核准物件的存取許可權</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">您需要核準時程表</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">有人要您核准此校訂</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">您的時程表已拒絕</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">您的時程表已重新開啟</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">您請求的檔案核准請求已核准</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">您請求的檔案核准請求已核准，但有變更</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">您請求的檔案核准請求被拒絕</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">您的時程表已核准</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

### 指派通知 {#assignment-notifications}

當您或您所在的團隊被指派Workfront中的任務或問題時，您會收到指派通知。 從指定通知，您可以執行下列動作：

* **[!UICONTROL 處理它]**：選取以認可處理專案。 系統會短暫顯示通知，確認您已將新專案新增至工作清單。
* **[!UICONTROL 在[!DNL Workfront]]**&#x200B;中檢視：選取以在Workfront中檢視指派的問題或任務，這會開啟新索引標籤。
* **[!UICONTROL 開始]**：按一下以開始處理專案。 系統會短暫顯示通知，確認您已將新專案新增至工作清單。
* **[!UICONTROL 註解]**：按一下以評論該專案。 您的註解也會顯示在Workfront的專案更新流中。
* **[!UICONTROL 狀態]**：按一下，然後從下拉式功能表中選取工作專案的新狀態。

#### 特定指定通知的可用動作：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>通知</th> 
   <th>[!UICONTROL 開始]</th> 
   <th>[!UICONTROL 註解]</th> 
   <th> <p>[!UICONTROL 狀態]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">您被指派至一個任務</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">您被指派到一個問題</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">您被指派的團隊會收到任務的工作請求</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">您被指派的團隊會收到問題的工作請求</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

### 註解通知 {#comment-notifications}

當有人對與您相關聯的專案發表評論或將您納入更新時，您會收到通訊通知。 在通訊通知中，您可以執行下列動作：

* **Reply**：按一下以回覆註解或[!UICONTROL 更新]。 您的回覆也會出現在更新流中，評論會顯示在Workfront中。
* **[!UICONTROL 在Workfront中檢視]**：選取此選項可檢視在新索引標籤中開啟的Workfront中的註解和專案。
* **[!UICONTROL 狀態]**：按一下，然後為註解或更新相關的工作專案選取新狀態。

#### 特定通訊通知上的可用動作：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>通知</th> 
   <th>[!UICONTROL 回覆]</th> 
   <th> <p>[!UICONTROL 狀態]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">註解已張貼在您的請求上</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">回覆已張貼在您的工作請求上</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">有人對您所在的執行緒發表註解</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">某人備註您的工作專案之一</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">某人備註您核准的時程表</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">註解會新增至您的使用者設定檔頁面，或透過大量編輯多位使用者來進行</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">您的其中一個更新已新增註解</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">註解已新增至您的時程表</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

### 更新通知 {#update-notifications}

當您關聯的專案有更新時，您會收到資訊通知，但您不需要對專案採取任何動作。 從資訊通知中，您可以執行下列動作：

* **[!UICONTROL 回覆]**：按一下以回覆[!UICONTROL 更新]。 您的回覆也會顯示在Workfront的專案更新流中。
* **在Workfront中檢視**：選取此選項可檢視在新索引標籤中開啟的Workfront中的註解和專案。
* **[!UICONTROL 狀態]**：按一下，然後從下拉式功能表中選取專案的新狀態。

#### 特定資訊通知上的可用動作：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>通知</th> 
   <th>[!UICONTROL 回覆]</th> 
   <th> <p>[!UICONTROL 狀態]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">您訂閱的任務、問題或專案已更新</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">有人將您加入定向更新</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">有人將您的團隊加入[!UICONTROL 導向更新]</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

### 日期變更通知 {#date-change-notifications}

當指定給您的工作專案的日期變更時，您會收到日期變更通知。 從日期變更通知中，您可以執行下列動作。

* **[!UICONTROL 註解]**：按一下以評論該專案。 您的註解也會顯示在Workfront的專案更新流中。
* **[!UICONTROL 狀態]**：按一下，然後從下拉式功能表中選取工作專案的新狀態。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>通知</th> 
   <th> <p>[!UICONTROL 註解]</p> </th> 
   <th> <p>[!UICONTROL 狀態]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">在指派給您的任務上變更了到期日期</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>
