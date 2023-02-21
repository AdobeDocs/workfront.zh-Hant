---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: 存取 [!DNL Adobe Workfront] 從 [!DNL Slack]
description: 整合 [!DNL Adobe Workfront] with [!DNL Slack] 可讓您存取 [!DNL Workfront] ，或在 [!DNL Workfront] 使用斜線命令。 整合可透過任何 [!DNL Slack] 環境，包括 [!DNL Slack] 行動應用程式。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 5f531217-3bd6-4156-8b9f-eabc95d4df10
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: tm+mt
source-wordcount: '1075'
ht-degree: 1%

---

# 存取 [!DNL Adobe Workfront] 從 [!DNL Slack]

整合 [!DNL Adobe Workfront] with [!DNL Slack] 可讓您存取 [!DNL Workfront] 從 [!DNL Slack]，或執行 [!DNL Workfront] 使用斜線命令。 整合可透過任何 [!DNL Slack] 環境，包括 [!DNL Slack] 行動應用程式。

您或您的 [!DNL Slack] 管理員必須安裝 [!DNL Workfront] 應用程式 [!DNL Slack] 例項 [!DNL Workfront] 從 [!DNL Slack]. 如需詳細資訊，請參閱 [設定Adobe Workfront以Slack](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## 關於斜線命令 {#about-slash-commands}

使用時 [!DNL Slack]，請在訊息欄位內輸入訊息。 當您以斜線啟動訊息時，訊息會變成命令，其行為與簡單訊息不同。 命令會告訴 [!DNL Slack] 來執行動作。

您可以存取 [!DNL Workfront] 執行個體 [!DNL Slack] 在任何 [!DNL Slack] 頻道。

在中使用斜線命令時，請記住以下事項 [!DNL Slack] 存取 [!DNL Workfront]:

* 斜線命令區分大小寫。
* 的命令 [!DNL Workfront] 只會顯示給您，無論您在哪個管道輸入。
* 命令應一律以開頭 `/workfront` 或 `/wf`，後面接著空格，以及您要在中執行之動作的名稱 [!DNL Workfront].

   這表示您的命令適用於 [!DNL Workfront] 應用程式。 的命令 [!DNL Workfront] 僅當已配置時才工作 [!DNL Workfront] 應用程式 [!DNL Slack] 例項。

對於可從Slack運行的所有命令的清單 [!DNL Workfront]，請參閱 [存取 [!DNL Workfront] 從 [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack).

## 登入 [!DNL Workfront] 從 [!DNL Slack] {#log-in-to-workfront-from-slack}

在Slack的訊息欄位中輸入任何命令時，系統會要求您登入 [!DNL Workfront] 第一個。\
如需 [!DNL Workfront] 命令 [!DNL Slack]，請參閱 [存取 [!DNL Workfront] 從 [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack) 一節。

登入 [!DNL Workfront] 從 [!DNL Slack]:

1. 登入 [!DNL Slack] 例項。
1. 在任何通道中鍵入以下命令之一：\
   `/workfront log in`

   或

   `/wf log in`

1. 按一下 [!DNL Workfront] **[!UICONTROL 登入]** 回應中顯示的連結。\
   新索引標籤隨即開啟，其中包含 [!DNL Workfront] 憑證。

1. 按照提示登錄 [!DNL Workfront] 使用增強驗證、OAuth 2.0或您的安全斷言標籤語言(SAML)URL。

   >[!NOTE]
   >
   >* 當系統提示您輸入主機時 [!DNL Workfront] 帳戶，請使用此格式輸入： *yourCompany&#39;sDomain.my.workfront.com*. 您公司的網域通常是您公司的名稱。
   >* 增強驗證必須在 [!DNL Workfront] 管理員會啟用此整合。



   的設定頁面 [!DNL Workfront] 通知 [!DNL Slack] 開啟。

1. （選用）停用任何 [!DNL Workfront] 您不想在 [!DNL Slack].

   如需設定的相關資訊 [!DNL Workfront] 設定 [!DNL Slack]，請參閱 [配置設定](#configure-settings-configure-settings) 本文章節

1. 導覽回您的 [!DNL Slack] 頻道。

   您已登入 [!DNL Workfront] 從 [!DNL Slack] 例項。

## 存取 [!DNL Workfront] 從 [!DNL Slack]

* [關於斜線命令](#about-slash-commands-about-slash-commands)
* [存取 [!DNL Workfront] 從 [!DNL Slack]](#access-workfront-from-a-shared-link-in-slack-access-workfront-from-a-shared-link-in-slack)

## 存取 [!DNL Workfront] 從 [!DNL Slack] {#access-workfront-from-a-slash-command-in-slack}

1. 登入 [!DNL Slack] 執行個體和登入 [!DNL Workfront] 從 [!DNL Slack].\
   如需登入的詳細資訊，請參閱 [!DNL Workfront] 從 [!DNL Slack]，請參閱 [登入 [!DNL Workfront] 從 [!DNL Slack]](#log-in-to-workfront-from-slack-log-in-to-workfront-from-slack)

1. 從任何通道，開始在消息欄位中鍵入以下命令：

   `/workfront help`

   或

   `/wf help`

1. 從以下命令中選擇：

   * `/wf home`

      顯示可從中訪問任務、問題和批准清單的按鈕。 按一下其中一個按鈕，會顯示 [!DNL Slack].

      如需管理的詳細資訊 [!DNL Workfront] 工作項 [!DNL Slack]，請參閱 [管理您的工作和批准 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf add task <TaskName>`

      在中納入要顯示的任務名稱 [!DNL Workfront] 介面。

      將任務添加到 [!DNL Workfront].

      有關將任務添加到 [!DNL Workfront] 從Slack，請參閱「從 [!DNL Slack]「 」部分 [從建立任務和問題 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md).

   * `/wf add issue <Issue Name>`

      在中納入問題的名稱，使其顯示於 [!DNL Workfront] 介面。

      將問題新增至 [!DNL Workfront]

      如需將問題新增至 [!DNL Workfront] 從 [!DNL Slack]，請參閱「建立問題來自 [!DNL Slack]「 」部分 [從建立任務和問題 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md).

   * `/wf favorites`

      顯示 [!DNL Workfront] 我的最愛。

      有關從訪問收藏夾的詳細資訊 [!DNL Slack]，請參閱 [存取您的 [!UICONTROL 我的最愛] 清單來源 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-favorites) 區段 [從以下位置訪問收藏夾和最近的項目 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md) 文章。

   * `/wf recent`

      顯示您最近存取的項目清單，位於 [!DNL Workfront].

      有關從以下位置訪問最近的項目的詳細資訊 [!DNL Slack]，請參閱 [存取您的 [!UICONTROL 最近項目] 清單來源 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-recent-items) section in the [[!UICONTROL Access your favorites] 和 [!UICONTROL 最近的項目 [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md) 文章。

   * `wf tasks`

      顯示任務清單。

      有關管理任務的詳細資訊，請參閱 [!DNL Slack]，請參閱「管理您的任務： [!DNL Slack]「 」部分 [管理您的工作和批准 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf issues`

      顯示問題清單。

      如需管理問題的詳細資訊，請參閱 [!DNL Slack]，請參閱「管理您的問題： [!DNL Slack]「 」部分 [管理您的工作和批准 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf approvals` 顯示您的 [!DNL Workfront] 批准。\

      如需管理核准的詳細資訊，請參閱 [!DNL Slack]，請參閱「管理您的核准」 [!DNL Slack]「 」部分 [管理您的工作和批准 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf search <keyword>`

      包含關鍵字。

      搜尋特定關鍵字。 可以搜索以下類型對象：

      * 專案
      * 任務
      * 問題
      * 報告
      * 人員
      * 範本
      * 文件
      * 專案組合
      * 方案
      * 儀表板
      * 公司
      * 備註  \

         如需有關在中搜尋的詳細資訊 [!DNL Slack]，請參閱 [搜尋 [!DNL Adobe Workfront] 項目來自Slack](../../workfront-integrations-and-apps/using-workfront-with-slack/search-for-wf-items-from-slack.md).
   * `/wf log in`

      將您登入 [!DNL Workfront] 從 [!DNL Slack].

   * `/wf log out `

      將您登出 [!DNL Workfront] 從 [!DNL Slack]. 您仍保持登入狀態 [!DNL Workfront] 如果您有 [!DNL Workfront] 例項會在另一個應用程式上的其他瀏覽器標籤中開啟。
   * `/wf settings`

      提供您設定 [!DNL Workfront] 設定 [!DNL Slack].

      如需設定的相關資訊 [!DNL Workfront] Slack中的設定，請參閱 [配置設定](#configure-settings-configure-settings).

   * `/wf help`
顯示命令的完整清單 [!DNL Workfront].


   * `Visit Workfront Help`:開啟 [!UICONTROL Slack] 區段 [!DNL Workfront] 說明網站（在新的瀏覽器標籤中）。


1. （可選）要刪除任何命令的消息，請將滑鼠移到包含該命令的Slack消息的右上角，然後按一&#x200B;下&#x200B;**[!UICONTROL 顯示消息操作]**，然後按一下 **[!UICONTROL 刪除訊息]**.

1. （選用和條件式）按一下 **[!UICONTROL 刪除]** 確認要刪除此郵件。

### 存取 [!DNL Workfront] 從 [!DNL Slack] {#access-workfront-from-a-shared-link-in-slack}

您可以存取 [!DNL Workfront] 對象從連結到與您共用的對象 [!DNL Slack].

如需有關存取的詳細資訊 [!DNL Workfront] 從共用連結，請參閱 [存取 [!DNL Adobe Workfront] 對象來自 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-wf-objects-from-shared-linked-in-slack.md).

## 配置設定 {#configure-settings}

1. 內 [!DNL Slack] 消息欄位，鍵入以下命令：

   `/workfront settings`

   或

   `/wf settings`

   預設會啟用所有設定。

1. 取消選取下列選項，以停用Workfront的設定：

   * 在 **[!UICONTROL 一般設定]** 區域，禁用 **[!UICONTROL 貼上 [!DNL Workfront] URL，在 [!DNL Slack] 管道，顯示其他說明、到期日或請求者名稱]**&#x200B;設定 [!DNL Slack] 新增關於 [!DNL Workfront] 對象 [!UICONTROL Slack].

   * 在 **[!UICONTROL 通知設定]** 區域中，禁用您要停止接收來自Workfront的通知。\

      有關接收的資訊 [!DNL Workfront] 通知 [!DNL Slack]，請參閱 [接收 [!DNL Adobe Workfront] 通知 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md).

## 登出 [!DNL Workfront] 從 [!DNL Slack]

1. 內 [!DNL Slack] 消息欄位，鍵入以下命令：\
   `/workfront log out` 或\
   `/wf log out`\
   您會收到確認，確認您已登出 [!DNL Workfront].\
   您仍保持登入狀態 [!DNL Workfront] 如果您有 [!DNL Workfront] 例項會在另一個應用程式上的其他瀏覽器標籤中開啟。
