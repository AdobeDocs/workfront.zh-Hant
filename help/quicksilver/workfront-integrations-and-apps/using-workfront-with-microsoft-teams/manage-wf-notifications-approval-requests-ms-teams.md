---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: 管理 [!DNL Adobe Workfront] 通知 [!DNL Microsoft] 團隊
description: 您可以接收來自 [!DNL Adobe Workfront] 關於需要核准的項目、已指派給您的工作，或您關聯的項目的註解和變更。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 7771a7d7-7e20-4b3d-95e7-1050aeb3af67
source-git-commit: 473a1fe3cb7e247749d9b540e3e5556cbe17a1dd
workflow-type: tm+mt
source-wordcount: '1280'
ht-degree: 0%

---

# 管理 [!DNL Adobe Workfront] 通知 [!DNL Microsoft Teams]

您可以接收來自 [!DNL Adobe Workfront] 關於需要核准的項目、已指派給您的工作，或您關聯的項目的註解和變更。

這些通知包含 [!DNL Workfront] 您可在內採取的動作 [!DNL Microsoft Teams] 不離開 [!DNL Microsoft Teams] 來完成這些任務。

>[!NOTE]
>
>[!DNL Microsoft Teams] 不再支援 [!DNL Internet Explorer]. 若要使用 [!DNL Adobe Workfront for Microsoft Teams integration]，您必須使用 [!DNL Internet Explorer].


## 存取需求

您必須具備下列存取權，才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計劃*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權*</td> 
   <td> <p>[!UICONTROL工作], [!UICONTROL計畫]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要了解您擁有的計畫、授權類型或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 接收的先決條件 [!DNL Workfront] 中的通知 [!DNL Microsoft Teams]

您可以收到 [!DNL Workfront] 通知 [!DNL Microsoft Teams] 若符合下列條件：

* 已安裝並配置了團隊所有者 [!DNL Workfront for Microsoft Teams] 為你的團隊。
* 您已登入 [!DNL Workfront] 從 [!DNL Microsoft Teams].
* 您已在 [!DNL Workfront]. 有關啟用即時通知的資訊，請參閱 [啟用或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

有關安裝的資訊 [!DNL Workfront for Microsoft Teams] 登入 [!DNL Workfront from Microsoft Teams]，請參閱 [安裝 [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

## 管理 [!DNL Workfront] 中的通知 [!DNL Microsoft Teams]

當 [!DNL Workfront for Microsoft Teams] 應用程式已安裝， [!DNL Workfront] 聊天通道建立於 [!DNL Microsoft Teams] 對每個隊員都有幫助。 當 [!DNL Workfront]，您可以為 [!DNL Workfront for Microsoft Teams] 接收 [!DNL Workfront] 聊天通道 [!DNL Microsoft Teams].

使用時請考量下列事項 [!DNL Workfront] 通知 [!DNL Microsoft Teams]:

* 您無法收到全部，但只能收到選取的 [!DNL Workfront] 通知 [!DNL Microsoft Teams].
* 您收到的所有通知 [!DNL Workfront] 在 [!DNL Workfront] 機器人聊天通道。

   如需安裝 [!DNL Workfront] 機器人通道，請參閱 [登入 [!DNL Workfront] 從 [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md#logging-in-to-workfront) 區段 [安裝 [!DNL Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md) 文章。

* 在中進行更新的時間之間，最多可能會延遲5分鐘 [!DNL Workfront] 當您收到 [!DNL Microsoft Teams].
* 針對每個 [!DNL Microsoft Teams] 通知時，您也會收到電子郵件通知。

若要管理 [!DNL Workfront] 您可在 [!DNL Microsoft Teams]:

1. 按一下 **[!UICONTROL 新增更多]** （三點）應用程式圖示，位於 [!DNL Microsoft Teams].

1. 按一下 [!DNL Workfront] 清單中。
1. 選取 **[!UICONTROL 設定]** 標籤。

   ![](assets/ms-teams-settings-tab-350x552.png)

1. 停用您不想接收的任何通知。 您可以啟用或停用通知群組（例如資訊或核准通知），或者也可以個別管理通知。

   預設會啟用所有通知。

   的通知設定 [!DNL Workfront for Microsoft] 系統會自動儲存團隊。

   >[!NOTE]
   >
   >您無法將更多通知新增至預設可用的通知。

## 回應 [!DNL Workfront] 中的通知和核准請求 [!DNL Microsoft Teams]

1. 登入 [!DNL Workfront] 從 [!DNL Microsoft Teams].\
   如需登入的相關資訊，請參閱 [!DNL Workfront]，請參閱 [安裝 [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

1. 前往 **[!UICONTROL 聊天]** ，然後按一下 **[!DNL Workfront]** 機器人通道。\
   此管道是供您與 [!DNL Workfront] 機器人。 全部 [!DNL Workfront] 通知會顯示在此。
1. 視您收到的通知類型而定，請繼續前往相關區段：

   * [核准通知](#approval-notifications-approval-notifications)
   * [分配通知](#assignment-notifications-assignment-notifications)
   * [注釋通知](#comment-notifications-comment-notifications)
   * [更新通知](#update-notifications-update-notifications)
   * [日期變更通知](#date-change-notifications-date-change-notifications)

### 核准通知 {#approval-notifications}

當您被要求批准對象（如任務、時間表或校樣）時，您會收到批准通知。 不過，您仍可以對通知進行註解。從核准通知，您可以執行下列動作：

* **[!UICONTROL 核准]**:按一下以核准項目。
* **[!UICONTROL 變更]**:按一下以核准包含變更的項目。
* **[!UICONTROL 拒絕]**:按一下「 」以拒絕項目。
* **[!UICONTROL 註解]**:按一下「 」以進行註解。 您的評論也會顯示在 [!DNL Workfront] 作為通知所在物件的更新。
* **[!UICONTROL 前往校樣]**:按一下以開啟校樣。 然後，您就可以直接在校樣中做出決定。 如需詳細資訊，請參閱 [在校對檢視器中決定校樣](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

>[!NOTE]
>
>一旦您做出核准決定，便無法從通知中變更。

#### 特定批准通知上可用的操作：

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
   <th>[!UICONTROL批准]</th> 
   <th>[!UICONTROL拒絕]</th> 
   <th> <p>[!UICONTROL更改]</p> </th> 
   <th> <p>[!UICONTROL轉到校樣] </p> </th> 
   <th>[!UICONTROL注釋]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">您需要核准專案</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">您需要批准任務</td> 
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
   <td role="rowheader">您需要批准文檔</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">您需要核准物件的存取權</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">您需要批准時間表</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">有人要你批准這份證明</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">您的時間表被拒絕</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">重新開啟您的時間表</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">您請求的文檔批准請求已獲批准</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">您請求的文檔批准請求已通過更改獲得批准</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">拒絕您請求的文檔批准請求</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">您的時間表已獲批准</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

### 分配通知 {#assignment-notifications}

當您或您所在的團隊被指派給Workfront中的任務或問題時，您會收到指派通知。 在分配通知中，您可以執行以下操作：

* **[!UICONTROL 努力]**:選擇以提交以處理項。 會短暫顯示通知，確認已將新項目新增至您的工作清單。
* **[!UICONTROL 檢視[!DNL Workfront]]**:選取「 」即可在Workfront中檢視指派的問題或任務，並開啟新索引標籤。
* **[!UICONTROL 開始]**:按一下以開始處理項目。 會短暫顯示通知，確認已將新項目新增至您的工作清單。
* **[!UICONTROL 註解]**:按一下「 」，對項目發表評論。 您的評論也會出現在Workfront中項目的更新資料流中。
* **[!UICONTROL 狀態]**:按一下，然後從下拉菜單中選擇工作項的新狀態。

#### 可用於特定分配通知的操作：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>通知</th> 
   <th>[!UICONTROL開始]</th> 
   <th>[!UICONTROL注釋]</th> 
   <th> <p>[!UICONTROL狀態]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">您被分配給任務</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">您被指派給問題</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">您被指派的團隊將接收任務的工作請求</td> 
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

### 注釋通知 {#comment-notifications}

當某人對您關聯的項目發表評論或將您納入更新時，您會收到通訊通知。 在通訊通知中，您可以執行下列動作：

* **代表ly**:按一下以回覆留言或 [!UICONTROL 更新]. 您的回覆也會顯示在更新資料流中，而註解會顯示在Workfront中。
* **[!UICONTROL 在Workfront中檢視]**:選取「 」，即可檢視註解和Workfront中的項目，這會在新索引標籤中開啟。
* **[!UICONTROL 狀態]**:按一下，然後為注釋或更新所在的工作項選擇新狀態。

#### 特定通訊通知上可用的動作：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>通知</th> 
   <th>[!UICONTROL回復]</th> 
   <th> <p>[!UICONTROL狀態]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">您的請求中已發佈評論</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">回覆已發佈在您的工作請求上</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">有人對您所在的線程發表評論</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">某人對您的其中一個工作項目發表評論</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">某人對您批准的工時單進行了評論</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">在您的使用者設定檔頁面上，或大量編輯多個使用者以新增註解</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">您的其中一項更新會新增註解</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">在您的時間表中添加註釋</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

### 更新通知 {#update-notifications}

當與關聯的項有更新時，您會收到資訊通知，但您不需要對該項採取任何操作。 從資訊通知，您可以執行下列動作：

* **[!UICONTROL 回覆]**:按一下以回覆 [!UICONTROL 更新]. 您的回覆也會顯示在Workfront中項目的更新資料流中。
* **在Workfront中檢視**:選取「 」，即可檢視註解和Workfront中的項目，這會在新索引標籤中開啟。
* **[!UICONTROL 狀態]**:按一下，然後從下拉式功能表中選取項目的新狀態。

#### 特定資訊通知上可用的動作：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>通知</th> 
   <th>[!UICONTROL回復]</th> 
   <th> <p>[!UICONTROL狀態]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">會更新您訂閱的任務、問題或專案</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">有人將您納入定向更新</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">有人將您的團隊納入[!UICONTROL定向更新]</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

### 日期變更通知 {#date-change-notifications}

當您被分配到的工作項目上的日期更改時，您將收到日期更改通知。 從日期變更通知開始，您可以執行下列動作。

* **[!UICONTROL 註解]**:按一下「 」，對項目發表評論。 您的評論也會出現在Workfront中項目的更新資料流中。
* **[!UICONTROL 狀態]**:按一下，然後從下拉菜單中選擇工作項的新狀態。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>通知</th> 
   <th> <p>[!UICONTROL注釋]</p> </th> 
   <th> <p>[!UICONTROL狀態]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">您被分配給的任務的到期日更改</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>
