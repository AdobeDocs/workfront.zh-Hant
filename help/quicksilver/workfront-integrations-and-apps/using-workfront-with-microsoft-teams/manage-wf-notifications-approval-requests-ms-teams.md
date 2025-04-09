---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: 管理 [!DNL Microsoft] 團隊中的 [!DNL Adobe Workfront] 通知
description: 您可以接收來自 [!DNL Adobe Workfront] 的通知，內容有關您需要核准的專案、已指派給您的工作分派，或您關聯專案的註解與變更。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 7771a7d7-7e20-4b3d-95e7-1050aeb3af67
source-git-commit: 41d898e82bc5b06498966ba938b68ed10e742d3b
workflow-type: tm+mt
source-wordcount: '1374'
ht-degree: 0%

---

# 管理[!DNL Microsoft Teams]中的[!DNL Adobe Workfront]個通知

>[!NOTE]
>
>自2025年7月1日起，Microsoft將移除對Classic Teams案頭應用程式的支援。 因此，Classic Teams案頭應用程式無法使用後，將不支援Workfront與Microsoft Teams的整合。

您可以從[!DNL Adobe Workfront]接收有關您需要核准的專案、已給予您的指派，或您關聯專案的評論和變更的通知。

這些通知包含[!DNL Workfront]個動作，您可以在[!DNL Microsoft Teams]內採取這些動作，不需離開[!DNL Microsoft Teams]即可完成這些動作。

>[!NOTE]
>
>[!DNL Microsoft Teams]不再支援[!DNL Internet Explorer]。 若要使用[!DNL Adobe Workfront for Microsoft Teams integration]，您必須使用[!DNL Internet Explorer]以外的網頁瀏覽器。


## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 許可證*</td> 
   <td> <p>[!UICONTROL 工作]、[！UICONTROL 計劃]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要瞭解您擁有的計劃、許可證類型或訪問許可權，請與管理員 [!DNL Workfront] 聯繫。

## 在[!DNL Microsoft Teams]中接收[!DNL Workfront]通知的必要條件

如果符合下列條件，您可以在[!DNL Microsoft Teams]中接收[!DNL Workfront]通知：

* 團隊擁有者已為您的團隊安裝和設定[!DNL Workfront for Microsoft Teams]。
* 您已從[!DNL Microsoft Teams]登入[!DNL Workfront]。
* 您已在 中 [!DNL Workfront]啟用即時通知。 有關啟用即時通知的資訊，請參閱 [修改您自己的電子郵件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)。

有關安裝和 [!DNL Workfront for Microsoft Teams] 記錄的信息 [!DNL Workfront from Microsoft Teams]，請参閱 [安裝 [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md)。

## 管理[!DNL Microsoft Teams]中的[!DNL Workfront]個通知

安裝[!DNL Workfront for Microsoft Teams]應用程式後，會在[!DNL Microsoft Teams]中為該團隊的每個成員建立[!DNL Workfront]聊天頻道。 在[!DNL Workfront]中執行特定動作時，您可以設定[!DNL Workfront for Microsoft Teams]的設定，以在[!DNL Microsoft Teams]的[!DNL Workfront]聊天頻道中接收有關該動作的通知。

處理來自[!DNL Microsoft Teams]的[!DNL Workfront]個通知時，請考慮下列事項：

* 您無法在[!DNL Microsoft Teams]中接收全部，但只能接收選取數量的[!DNL Workfront]則通知。
* 您從[!DNL Workfront]收到的所有通知都會顯示在[!DNL Workfront]機器人聊天頻道中。

  如需有關安裝[!DNL Workfront]機器人頻道的資訊，請參閱[安裝 [!DNL Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md)文章中的[登入 [!DNL Workfront] 來自 [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md#logging-in-to-workfront)區段。

* 從[!DNL Workfront]中完成更新到您在[!DNL Microsoft Teams]中收到有關該更新的通知之間最多可能有5分鐘的延遲。
* 對於每個[!DNL Microsoft Teams]通知，您也會收到電子郵件通知。

若要管理可在[!DNL Microsoft Teams]中收到的[!DNL Workfront]通知：

1. 按一下[!DNL Microsoft Teams]中左側導覽列上的&#x200B;**[!UICONTROL 更多新增]** （三點）應用程式圖示。

1. 在出現的清單中按一下[!DNL Workfront]。
1. 選取「**[!UICONTROL 設定]**」標籤。

   ![MS Teams設定標籤](assets/ms-teams-settings-tab-350x552.png)

1. 停用您不想接收的任何通知。 您可以啟用或停用通知群組，例如資訊或核准通知，也可以個別管理通知。

   預設會啟用所有通知。

   [!DNL Workfront for Microsoft]團隊的通知設定會自動儲存。

   >[!NOTE]
   >
   >您無法新增更多通知至預設可用的通知。

## 在[!DNL Microsoft Teams]中回應[!DNL Workfront]個通知和核准要求

1. 從[!DNL Microsoft Teams]登入[!DNL Workfront]。\
   如需有關登入[!DNL Workfront]的資訊，請參閱[安裝 [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md)。

1. 前往&#x200B;**[!UICONTROL 聊天]**&#x200B;區域並按一下&#x200B;**[!DNL Workfront]**&#x200B;機器人頻道。\
   此通道用於您與機器人進行 [!DNL Workfront] 個人聊天。 所有 [!DNL Workfront] 通知都會顯示在這裡。
1. 根據您收到的通知類型，轉到相關部分：

   * [核准通知](#approval-notifications-approval-notifications)
   * [指派通知](#assignment-notifications-assignment-notifications)
   * [註解通知](#comment-notifications-comment-notifications)
   * [更新通知](#update-notifications-update-notifications)
   * [日期變更通知](#date-change-notifications-date-change-notifications)

### 核准通知 {#approval-notifications}

當系統要求您批准物件（如任務、時程表或證明）時，您會收到審批通知。 不過，您仍可對通知發表評論。您可從核准通知執行以下作：

* **[!UICONTROL 批准]**：按下以批准專案。
* **[!UICONTROL 更改]**：按下以批准包含更改的專案。
* **[!UICONTROL 拒絕]**： 按兩下以拒絕該專案。
* **[!UICONTROL 註解]**：點擊發表評論。 您的註解也會在[!DNL Workfront]中顯示為通知相關物件的更新。
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
   <th>[！UICONTROL核准]</th> 
   <th>[！UICONTROL拒絕]</th> 
   <th> <p>[！UICONTROL變更]</p> </th> 
   <th> <p>[！UICONTROL前往校訂] </p> </th> 
   <th>[！UICONTROL註解]</th> 
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
   <td role="rowheader">您需要批准問題</td> 
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
   <td role="rowheader">您的時程表將重新打開</td> 
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
   <td role="rowheader">您請求的文件審批請求被拒絕</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">您的時程表已獲得批准</td> 
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
   <th>[！UICONTROL開始]</th> 
   <th>[！UICONTROL註解]</th> 
   <th> <p>[！UICONTROL狀態]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">您已被分配到一個任務</td> 
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

當有人對與您相關聯的專案發表評論或將您納入更新時，您會收到通訊通知。 從通信通知，您可以執行以下作：

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
   <th>[！UICONTROL回覆]</th> 
   <th> <p>[！UICONTROL狀態]</p> </th> 
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
   <td role="rowheader">有人評論您所在的線程</td> 
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
   <td role="rowheader">系統會在用戶設定檔頁面上或透過批量编辑多個用戶來新增評論</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">系統會在其中一個更新中添加評論</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">將在時程表上添加註釋</td> 
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
   <th>[！UICONTROL回覆]</th> 
   <th> <p>[！UICONTROL狀態]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">對您訂閱的任務、問題或專案進行了更新</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">有人將您包括在定向更新中</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">有人將您的團隊加入[！UICONTROL導向更新]</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

### 日期變更通知 {#date-change-notifications}

當指定給您的工作專案的日期變更時，您會收到日期變更通知。 從日期變更通知中，您可以執行下列動作。

* **[!UICONTROL 註解]**：按一下以評論該專案。 您的註解也會顯示在Workfront的專案更新流中。
* **[!UICONTROL 狀態]**：按兩下，然後從下拉功能表中選擇工作項的新狀態。

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
   <td role="rowheader">分配給您的任務的截止日期會發生變化</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>
