---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 記錄時間
description: 您可以在Adobe Workfront中記錄工作項目的時間(&N)，以指出您在工作項目上花費的小時數。 您也可以記錄與工作無關的時間，例如休假、病假或您花在會議上的時間。 您的日誌時間顯示在時間表中。
author: Alina
feature: Timesheets
exl-id: 120173a8-95f1-4233-ab40-d3bcfe38c977
source-git-commit: b2859f3d268bd947fba5bb0280677465b3039d93
workflow-type: tm+mt
source-wordcount: '2992'
ht-degree: 0%

---

# 記錄時間

您可以在Adobe Workfront中記錄工作項目的時間，以指出您在工作項目上花費的小時數。 您也可以記錄與工作無關的時間，例如休假、病假或您花在會議上的時間。 您的日誌時間顯示在時間表中。

如需可登入Workfront的時數類型詳細資訊，請參閱 [管理小時類型](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## 存取需求

<!--drafted for P&P - replace the table:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Light or higher</p>
   <p>Legacy license: 
   <ul><li>Review or higher to log General Hours in a timesheet</li>
   <li>Work or higher to log hours on a project, task, or issue</li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to the type of work item you log time for </p> <p>For example, you need Edit access to Issues, to log time for issues</p> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute or higher permissions on the work item you log time for that includes permissions to Log Hours</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

您必須具備下列存取權，才能執行本文所述步驟並記錄專案特定時數：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <ul><li>查看或更新以在時間表中記錄一般小時數</li>
   <li> 工作時間或更高，可記錄項目、任務或問題的時數</li></ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">訪問級別配置*</td> 
   <td> <p>編輯您登錄時間的工作項類型的訪問權限 </p> <p>例如，您需要編輯問題的存取權，才能記錄問題的時間</p> <p>如果您仍無權存取，請洽詢您的Workfront管理員，他們是否在您的存取層級設定其他限制。 如需Workfront管理員如何修改您的存取層級的詳細資訊，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件權限</td> 
   <td> <p>對您登錄時間的工作項目（包括「記錄時間」的權限）貢獻或更高權限。</p> <p>有關請求其他訪問的資訊，請參閱 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">請求對對象的訪問 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*若要了解您擁有的計畫、授權類型或存取權，請聯絡您的Workfront管理員。

## 在Workfront中記錄時的考量事項

* 您可以記錄項目、任務或問題的時間，也可以直接在工時單中記錄時間。

   有關建立工時單的資訊，請參閱 [建立單次使用的工時單](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

* 通過工時表以外的工具記錄的所有時間都顯示在相應時段的時間表中。
* 項目上非當前的任務和問題不會預先填充到時間表中。
* 工時單中記錄的時間會立即應用於任務、問題或項目。
* 時間表包括所有記錄日期的總時間。 即使將時間軸計算設定為排除週末，週末一律包含在內(如 [配置系統範圍的項目首選項](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md))。
* 工時單中顯示的項目數上限為45。 如果有45個以上的項目的日期與時間表時間範圍匹配，則只顯示最近更新的項目。
* 計費帳單記錄中包含的小時條目將呈灰色，無法在工時單中編輯。 如需詳細資訊，請參閱 [建立計費記錄](../../manage-work/projects/project-finances/create-billing-records.md).

## 記錄時間

您可以在Workfront的下列區域登入時間：

* [時程表](#timesheet)
* [首頁](#home)
* [項目、任務或問題](#project-task-or-issue)
* [摘要面板](#summary-panel)
* [展示板](#boards)
* [行動應用程式](#mobile-app)

### 時程表 {#timesheet}

您可以在時間表上記錄一般小時數或項目特定小時數。

>[!NOTE]
>
>查看分配給時間表配置檔案的用戶可以查看時間表頁簽和日誌一般小時數。 但是，他們無法記錄工時表中顯示的分配給他們的任何任務或問題。

1. 按一下 [!UICONTROL **主菜單**] 圖示 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 按一下 [!UICONTROL **工時單**]. 預設顯示當前工時單。
   ![時程表](assets/timesheet-redesigned-nwe.png)

   時間表預先填充了在時間表的時間範圍內分配給您的項目。 有關如何預填工時單的資訊，請參見 [配置工時單和小時首選項](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md). 如果在工時單上沒有看到項目，則可以添加它。

   >[!NOTE]
   >
   >工時單僅預先填入分配給您的項目。 它不會預先填入指派給您的團隊或工作角色的項目。
   >
   >按一下分配給您的團隊的項目上的「工作」(Work On It)，會將項目分配給您，該項目將顯示在您的工時單中。


1. （選用）按一下 **全螢幕** 圖示 ![](assets/full-screen.png) 要以全螢幕模式顯示時間表，請按一下 **exit-full-screen** ![](assets/exit-full-screen.png) 表徵圖，返回到時間表。

   <!-- drafted for the resize columns in timesheet story: 1. (optional) Click on the separator lines between weeks or between the time frame area and the work item area to resize the columns of the timesheet.-->

1. （可選）要將項目、任務或問題添加到時間表，請按一下 **新增項目** 時間表左上角的下拉菜單，然後按一下 **新增專案**, **添加任務**，或 **新增問題**.

   專案、工作或問題清單隨即顯示。

   <!--drafted for full screen mode for add projects story - align it with the rest of the steps when you enable this:: 1. (Optional) Click the **full-screen** icon ![](assets/full-screen.png) to display the list of objects in full-screen mode.-->

1. （選用）按一下搜尋圖示 ![搜尋項目](assets/search-icon.png) 使用關鍵字搜索特定項以添加到時間表。

1. （可選）展開篩選、檢視或分組下拉式功能表，以套用或自訂一個功能表，並檢視您想要的項目資訊。

1. 在清單中選取一或多個項目，然後按一下 **新增**.

   >[!NOTE]
   >
   >將任務或問題添加到時間表時，也會添加項目。


1. （條件性）如果一次添加50個或多個項目，則會顯示一條確認消息，其中顯示添加到工時單的項目數。

   按一下 **全部新增** 添加所有項，或按一下 **取消** 若要停止新增選取的項目，則 **取消** 以關閉項目清單。

   任務和問題會列在項目名稱下。

   >[!NOTE]
   >
   >手動添加到工時單的物料將被固定，並將保留在當前和將來的工時單上，直到手動取消固定它們以刪除它們。 有關取消固定項目以從時間表中刪除它們的資訊，請繼續步驟10。

   <!--(ensure this stays accurate)-->

1. （選用）按一下 **折疊** ![](assets/collapse-icon.png) 或 **展開** ![](assets/expand-icon.png) 項目名稱旁的表徵圖，可顯示或隱藏項目的任務和問題清單。


   >[!TIP]
   >
   >   使用標準QWERTY鍵盤時，在工時表中按一下項目名稱后，按下列一組鍵可折疊或展開項目：
   >   * 要展開項目並顯示其工作項，請執行以下操作：
      >     * Shift + Alt +向上箭頭（適用於Windows電腦）
      >     * 適用於Mac電腦的Shift + Option +向上箭頭
   >   * 要折疊項目並隱藏其工作項，請執行以下操作：
      >     * Shift + Alt +向下箭頭（適用於Windows電腦）
      >     * 適用於Mac電腦的Shift + Option +向下箭頭。



1. （可選）要自動固定顯示在時間表上的項目，請將滑鼠指標暫留在項目名稱上，然後按一下 **pin** 圖示 ![](assets/empty-pin-icon.png).

   >[!TIP]
   >
   >   在按一下工時單中的項目後使用標準QWERTY鍵盤時，按下列一組鍵以固定項目：
   >   * 選項+ P(適用於Windows和Mac電腦)。



1. （選用）按一下搜尋圖示 ![](assets/search-icon.png) 然後開始鍵入關鍵字以查找工時單上的項目、任務或問題。

1. （可選）如果手動添加項目（如步驟3-6中所述），並且您尚未通過取消固定項目來記錄時間，則可以從時間表中刪除項目（項目、任務或問題）。 <!--ensure this stays accurate-->

   您不能根據配置為預填時間表的Workfront系統或組中的時間表首選項自動刪除時間表中包含的項目(如 [配置工時單和小時首選項](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

   從人工添加的工時單中刪除項：

   1. 確保沒有針對項目記錄任何時間。
   1. 按一下 **取消釘選** 圖示 ![固定項目](assets/pin-icon.png) 項目旁邊，從時間表中取消固定項目。

   >[!TIP]
   >
   >   在按一下工時單中的項目後使用標準QWERTY鍵盤時，按下列一組鍵以取消固定項目：
   >   * 選項+ P(適用於Windows和Mac電腦)。



   重新整理頁面後，該項目將從工時單中移除。

1. （條件性）如果您的Workfront或群組管理員已啟用 **手動將作業角色分配給小時條目** 設定後，從下拉式功能表中選取作業角色。 預設情況下，系統將顯示您被分配給工作項時指定的角色。 如果未在對象上分配角色，則預設會顯示您的主要角色。 如需此設定的詳細資訊，請參閱文章 [配置工時單和小時首選項](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

   ![工時單中多個角色的記錄時間](assets/job-role-plus-sign-and-boxes-in-redesigned-timesheet.png)


1. （選用）按一下 **+** 表徵圖，然後從 [!UICONTROL 小時類型] 欄，記錄不同小時類型的時間。

   ![小時類型下拉式功能表](assets/hour-type-drop-down-expanded-redesigned-timesheet.png)

   >[!TIP]
   >
   >   根據您的作業系統或瀏覽器以及使用標準QWERTY鍵盤時，按下列鍵組以添加另一行：
   >   * Ctrl + Option + + for Windows電腦
   >   * 適用於Mac電腦的Cmd + Option + +


   小時類型取決於系統、專案和使用者層級中已定義的內容，如 [定義工時單的工時類型和可用性](define-hour-types-and-availability.md).

   工時單關閉後，無法更改小時類型。

   >[!TIP]
   >
   >如果您先前記錄的時間，而您選取的小時類型現在已停用，則記錄時間的整列會呈現灰色。 選擇另一個小時類型並刷新頁面會從下拉清單中刪除停用的小時類型選項，因此您不能向該小時類型添加其他小時。
   >
   >如果要將停用的小時類型與過去記錄的時間關聯，請考慮為要記錄的附加時間的工作項目添加新行，並選擇新的小時類型。

1. 按一下 **刪除** 圖示  ![](assets/delete.png) 的URL。 也會移除角色記錄的任何時間。

   >[!TIP]
   >
   >   根據您的作業系統或瀏覽器，以及使用標準QWERTY鍵盤時，按下列鍵組以刪除行：
   >   * Ctrl + Option + — 用於Windows電腦
   >   * Cmd +選項+ — 適用於Mac電腦



1. 在時間表的時間軸部分中指定要登錄任何指定日的時間，然後按一下小時框外部以保存小時條目。 小時會自動儲存。 您的日誌時間所在的行以淺藍色突出顯示，而小時輸入框以深藍色列出。

   ![工時單中的日誌時間框](assets/log-time-with-blue-hightlight-redesigned-timesheet.png)

   您以小時或天為單位登錄時間。 此設定由具有計畫許可證的用戶或系統管理員配置，如 [配置時間是以小時還是天記錄](../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md).

   >[!IMPORTANT]
   >
   >如果您記錄的作業角色已變更，且 **手動將作業角色分配給小時條目** 設定已停用，您必須手動儲存時間項目。 只有在已更改的作業角色不再記錄任何時間時，工時單才會自動保存您的時間。
   >
   >如果角色已變更，且 **手動將作業角色分配給小時條目** 設定啟用後，您可以記錄時間或更新角色，並自動儲存您的變更。

1. （可選）在工時單題頭的「特定時段」欄位中指定超時時間。

   >[!TIP]
   >
   >不能記錄比工時單上當前總小時數更多的加班小時數。 例如，如果到目前為止在工時單上記錄了7小時，則無法記錄8小時的加班。

1. （選用）按一下 **註解** 為小時條目添加註釋。

   ![](assets/commment-button-on-hour-log-redesigned-timesheet.png)

   >[!TIP]
   >
   >   按一下小時輸入框後使用標準QWERTY鍵盤時，按下列鍵組以開啟注釋框：
   >   * Shift + F2(適用於Windows和Mac電腦)。


1. 按一下 **完成** 以保存注釋。

   >[!TIP]
   >
   >   使用標準QWERTY鍵盤時，從注釋框內按以下鍵集以保存注釋：
   >   * Ctrl + Enter（Windows電腦）。
   >   * Cmd +返回Mac電腦。



1. （選用）按一下 **顯示注釋** 在工具欄中，在工作項下顯示工時條目注釋。

   ![在工時單中的項目下列出的注釋](assets/comments-expanded-under-tasks-redesigned-timesheet.png)

   >[!TIP]
   >
   >   您對工時單所做的所有更改都將自動保存。

1. （可選）按一下任務或問題的列，然後按一下 **開啟摘要** 在工時單的右上角，添加更新或更新有關任務或問題的資訊。 「摘要」面板隨即開啟。

   ![summary-panel-for-task-opened-in-timestime](assets/summary-panel-for-task-opened-in-timesheet-redesigned-timesheet.png)

   您的更新會顯示在與記錄時間相關聯的工作項的「更新」區域中。

   >[!TIP]
   >
   >您無法對項目或「一般時間」小時條目進行注釋。

1. 按一下 [!UICONTROL **關閉摘要**] 關閉「摘要」面板並返回工時單。

1. （選用）按一下 [!UICONTROL **更新**] 在左側面板中，將更新添加到時間表。 如需Workfront更新的詳細資訊，請參閱 [更新工作](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

   ![enter-an-update-in-redeasided-timesheet-left-panel](assets/enter-an-update-in-redesigned-timesheet-left-panel.png)

   * **關閉**:完成時間表的更新後，關閉該時間表。 只有在時間表未與批准者關聯時，此選項才可用。

   * **提交以供批准：** 只有時間表上有批准者時，此選項才可用。 儲存您的變更並提交以進行核准。 通過按一下，可以在關閉工時單後開啟工時單 **召回**，若尚未授予核准。 如需詳細資訊，請參閱 [提交時間表以進行批准](../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md).

   * **拒絕**:當您是工時單審批人，並且已將工時單提交給您進行審批時，將顯示此選項。 按一下該選項可將工時單的狀態更改為「已拒絕」，工時單保持開啟狀態。

   * **核准**:當您是工時單審批人，並且已將工時單提交給您進行審批時，將顯示此選項。 按一下它可將時間表的狀態更改為已批准，並關閉時間表。
   >[!TIP]
   >
   >當您是系統管理員，且時間表與核准者相關聯時，「拒絕」和「核准」選項也會顯示在您的時間表上。

1. （條件性）如果已關閉或已提交工時單以供審批，請按一下以下選項之一：

   * **重新開啟**:此選項可用於已關閉且沒有批准者的工時單或已批准的工時單。 重新開啟工時單以修改小時條目。
   * **召回**:此選項適用於已提交以供審批但尚未批准或拒絕的時間表。 按一下 **召回** 重新開啟工時單並修改工時條目。

### 首頁 {#home}

您可以在首頁中記錄專案的特定時間。

有關使用「首頁」區域的一般資訊，請參閱 [使用首頁區域](../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

要從「首頁」區域登錄工作項的時間：

1. 在 **工作清單** ，選擇要記錄時間的項目。
1. 在右側面板中，按一下 **記錄時間**.

   ![](assets/log-time-home-350x181.png)

1. 在 **輸入小時數** 下拉式功能表中，選取適當的小時類型。\
   小時類型取決於系統、專案和使用者層級中已定義的內容，如 [定義工時單的工時類型和可用性](../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).
1. （條件性）如果您的Workfront或群組管理員已啟用 **手動將作業角色分配給小時條目** 設定後，從下拉式功能表中選取作業角色。 預設情況下，系統將顯示您被分配給工作項時指定的角色。 如果未在對象上分配角色，則預設會顯示您的主要角色。 如需此設定的詳細資訊，請參閱文章 [配置工時單和小時首選項](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
1. 指定您要記錄的時間，然後按一下 **記錄時間**.

### 項目、任務或問題 {#project-task-or-issue}

您可以記錄專案、任務或問題的特定時間。

#### 記錄時間所需的權限

若要登入專案、任務或問題的數小時，您必須具備特定權限。 您可以在專案、任務或問題的兩個位置登入時間：

* [「更新」頁簽](#updates-tab)
* [「小時」頁簽](#hours-tab)

##### 「更新」頁簽{#updates-tab}

在登錄項目、任務或問題的「更新」頁簽的數小時前，需要執行以下操作：

* 您必須擁有工作或計畫授權。
* 您至少必須對專案、任務或「記錄時數」的存取權有Contribute權限。\
   如需授與專案權限的詳細資訊，請參閱 [在Adobe Workfront中共用專案](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

* 如果您想要直接將時間記錄到專案，Workfront管理員必須在 [!UICONTROL **時間表和小時數** ]> [!UICONTROL **偏好設定**].\
   如需允許使用者直接將數小時記錄至專案的詳細資訊，請參閱 [配置工時單和小時首選項](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

##### 「小時」頁簽{#hours-tab}

在可以登錄項目、任務或問題的「小時」頁簽上，需要以下項：

* 您必須是系統管理員。

或者，您必須具備下列所有條件：

* 您必須擁有計畫許可證，並具有對工時單和工時的管理訪問權限。 有關授予對工時單和小時的管理訪問權限的詳細資訊，請參閱 [授予用戶對特定區域的管理訪問權限](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).
* 您至少必須擁有專案的Contribute權限，且具備「記錄時數」的存取權。 如需授與專案權限的詳細資訊，請參閱 [在Adobe Workfront中共用專案](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
* 如果要直接將時間記錄到項目，您的Workfront管理員必須在「工時單和小時數」>「首選項」下啟用「直接記錄項目時間」設定。 如需允許使用者直接將數小時記錄至專案的詳細資訊，請參閱 [配置工時單和小時首選項](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

登錄項目、任務或問題的時間：

1. 導覽至專案、任務或問題。
1. 在左側面板中，選取 **小時**.
1. 按一下 **記錄時間**.

   「記錄時數」對話框隨即顯示。

1. 指定下列資訊：

   * **所有者：** 您的名稱預設會顯示在此欄位中。\
      如果您正在記錄另一個使用者的小時數，請指定其名稱。

   * **小時**:輸入項目、任務或問題的小時數。
   * **小時類型**:如果下拉式功能表與預設顯示的功能表不同，請選取「小時類型」 。

      根據系統中配置的小時類型，此處的選項可能有所不同。 有關配置小時類型的詳細資訊，請參閱 [定義工時單的工時類型和可用性](../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

   * **工作角色**:（條件性）如果您的Workfront或群組管理員已啟用 **手動將作業角色分配給小時條目** 設定，選擇 **工作角色** 從下拉式功能表。 預設情況下，將顯示在您被分配給對象時指定的角色。 如果未在對象上分配角色，則預設顯示主角色。 如需此設定的詳細資訊，請參閱文章 [配置工時單和小時首選項](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

      ![Screen_Shot_2017-05-03_at_10.16.52_AM.png](assets/screen-shot-2017-05-03-at-10.16.52-am-350x346.png)

1. 按一下 **記錄時數**.

### 摘要面板

您可以在「摘要」面板中記錄任務和問題的時間。
如需詳細資訊，請參閱 [摘要概觀](../../workfront-basics/the-new-workfront-experience/summary-overview.md).

![](assets/summary-hour-log.png)

### 展示板 {#boards}

>[!NOTE]
>
>只有透過Workfront展示板的早期功能選擇，才能使用此功能。

您可以在Workfront主板上的連線卡上登錄時間。 這與記錄任務或問題的時間相同，並且記錄在卡上的小時數儲存在所連接的任務或問題上。
如需詳細資訊，請參閱 [在主板上使用連接的卡](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

### 行動應用程式 {#mobile-app}

您可以從Workfront行動應用程式記錄時間。
如需詳細資訊，請參閱 [Adobe Workfront for Android](/help/quicksilver/workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md) 或 [Adobe Workfront for iOS](/help/quicksilver/workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md).
